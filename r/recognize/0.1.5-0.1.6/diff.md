# Comparing `tmp/recognize-0.1.5.tar.gz` & `tmp/recognize-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recognize-0.1.5.tar", max compression
+gzip compressed data, was "recognize-0.1.6.tar", max compression
```

## Comparing `recognize-0.1.5.tar` & `recognize-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.5/README.md
--rw-r--r--   0        0        0      411 2023-06-05 15:51:01.923676 recognize-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.5/recognize/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.5/recognize/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.5/recognize/commands/lib/__init__.py
--rw-r--r--   0        0        0     3403 2023-06-05 15:43:18.737969 recognize-0.1.5/recognize/commands/lib/client.py
--rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.5/recognize/commands/lib/entries.py
--rw-r--r--   0        0        0     1187 2023-06-05 13:50:58.064038 recognize-0.1.5/recognize/commands/lib/helpers.py
--rw-r--r--   0        0        0     2940 2023-06-05 15:23:37.455666 recognize-0.1.5/recognize/commands/search.py
--rw-r--r--   0        0        0     1046 2023-06-05 15:23:37.447161 recognize-0.1.5/recognize/commands/upload.py
--rw-r--r--   0        0        0      192 2023-06-05 13:59:14.826793 recognize-0.1.5/recognize/main.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 recognize-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.6/README.md
+-rw-r--r--   0        0        0      436 2023-06-07 15:56:14.645202 recognize-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.6/recognize/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.6/recognize/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.6/recognize/commands/lib/__init__.py
+-rw-r--r--   0        0        0     4380 2023-06-07 15:55:40.787734 recognize-0.1.6/recognize/commands/lib/client.py
+-rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.6/recognize/commands/lib/entries.py
+-rw-r--r--   0        0        0     1574 2023-06-07 14:04:50.724674 recognize-0.1.6/recognize/commands/lib/helpers.py
+-rw-r--r--   0        0        0     3288 2023-06-07 14:12:08.572874 recognize-0.1.6/recognize/commands/search.py
+-rw-r--r--   0        0        0     1723 2023-06-07 14:12:08.612866 recognize-0.1.6/recognize/commands/upload.py
+-rw-r--r--   0        0        0      713 2023-06-07 15:55:18.465021 recognize-0.1.6/recognize/main.py
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 recognize-0.1.6/PKG-INFO
```

### Comparing `recognize-0.1.5/recognize/commands/lib/helpers.py` & `recognize-0.1.6/recognize/commands/lib/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import os
 import re
 from asyncio import Semaphore
 from pathlib import Path
-from typing import Generator, Tuple
+from typing import Generator, Tuple, Optional
 
 import httpx
 from httpx import HTTPStatusError
 
+WRITE_TIMEOUT = 60 * 3
 
-async def upload_file(semaphore: Semaphore, file_path: str, url: str) -> Tuple[str, bool]:
+
+async def upload_file(semaphore: Semaphore, file_path: str, url: str, dev: bool) -> Tuple[str, bool, Optional[str]]:
     """Asynchronously upload a file to a given URL."""
     with open(file_path, 'rb') as fp:
         files = {'file': (fp.name, fp)}
-
-        async with httpx.AsyncClient(timeout=120.0) as client:
-            async with semaphore:
-                async with client.stream('POST', url, files=files) as response:
-                    try:
-                        response.raise_for_status()
-                        return file_path, True
-                    except HTTPStatusError:  # Ensure we get a 2xx response
-                        return file_path, False
+        try:
+            async with httpx.AsyncClient(timeout=WRITE_TIMEOUT) as client:
+                async with semaphore:
+                    async with client.stream('POST', url, files=files, params={"dev": dev}) as response:
+                        try:
+                            response.raise_for_status()
+                            return file_path, True, None
+                        except HTTPStatusError as e:  # Ensure we get a 2xx response
+                            return file_path, False, str(e)
+        except httpx.WriteTimeout:
+            return file_path, False, "Upload took too long, check connection and try again."
+        except Exception:
+            return file_path, False, "Something went wrong uploading this file."
 
 
 def find_files(filepath: Path) -> Generator[str, None, None]:
     # pattern = re.compile(r'\.(jpeg|jpg|png|mp4|mov)$')
     pattern = re.compile(r'\.(mp4|mov)$')
     for root, dirs, files in os.walk(filepath.absolute()):
         for file in files:
```

### Comparing `recognize-0.1.5/recognize/commands/search.py` & `recognize-0.1.6/recognize/commands/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 import typer
 from typing_extensions import Annotated
 
 from .lib.client import DataAPI
 from .lib.entries import LabelEntryType
 
@@ -12,62 +12,68 @@
 
 
 @app.command()
 def keywords(
         words: Annotated[List[str], typer.Argument()],
         output: Annotated[Path, typer.Option()],
         json: Annotated[bool, typer.Option("--json")] = False,
-        dev: Annotated[bool, typer.Option("--dev")] = False
+        dev: Annotated[bool, typer.Option("--dev")] = False,
+        url: Annotated[Optional[str], typer.Option()] = None
 ):
     """
     Execute a keyword search.
 
+    :param url: URL override for the API
     :param words: A list of keywords to search for.
     :param output: The output path where the search results will be stored.
     :param json: An optional flag indicating whether the output should be in JSON format. If False, the output is CSV.
     :param dev: An optional flag indicating whether to use the dev stack. Uses dev stack if True.
     :return: The result of the search operation.
     """
-    api = DataAPI(dev=dev)
+    api = DataAPI(dev=dev, url=url)
     return api.keyword_search(words, output, response_type="csv" if not json else "json")
 
 
 @app.command()
 def entry(
         entry_type: Annotated[LabelEntryType, typer.Argument()],
         output: Annotated[Path, typer.Option()],
         json: Annotated[bool, typer.Option("--json")] = False,
-        dev: Annotated[bool, typer.Option("--dev")] = False
+        dev: Annotated[bool, typer.Option("--dev")] = False,
+        url: Annotated[Optional[str], typer.Option()] = None
 ):
     """
     Execute a search for entries of a specific type.
 
+    :param url: URL override for the API.
     :param entry_type: The type of entries to search for.
     :param output: The output path where the search results will be stored.
     :param json: An optional flag indicating whether the output should be in JSON format. If False, the output is CSV.
     :param dev: An optional flag indicating whether to use the dev stack. Uses dev stack if True.
     :return: The result of the search operation.
     """
-    api = DataAPI(dev=dev)
+    api = DataAPI(dev=dev, url=url)
     return api.entry_search(entry_type, output, response_type="csv" if not json else "json")
 
 
 @app.command()
 def faces(
         image_file: Annotated[Path, typer.Argument()],
         output: Annotated[Path, typer.Option()],
         json: Annotated[bool, typer.Option("--json")] = False,
-        dev: Annotated[bool, typer.Option("--dev")] = False
+        dev: Annotated[bool, typer.Option("--dev")] = False,
+        url: Annotated[Optional[str], typer.Option()] = None
 ):
     """
     Execute a face search using a provided image file.
 
+    :param url: URL override for the API.
     :param image_file: The path to the image file that will be used for the face search.
     :param output: The output path where the search results will be stored.
     :param json: An optional flag indicating whether the output should be in JSON format. If False, the output is CSV.
     :param dev: An optional flag indicating whether to use the dev stack. Uses dev stack if True.
     :return: The result of the search operation.
     """
-    api = DataAPI(dev=dev)
+    api = DataAPI(dev=dev, url=url)
 
     with open(image_file, 'rb') as fp:
         return api.faces_search(fp, output, response_type="csv" if not json else "json")
```

