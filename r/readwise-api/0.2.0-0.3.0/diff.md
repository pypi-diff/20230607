# Comparing `tmp/readwise_api-0.2.0.tar.gz` & `tmp/readwise_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readwise_api-0.2.0.tar", max compression
+gzip compressed data, was "readwise_api-0.3.0.tar", max compression
```

## Comparing `readwise_api-0.2.0.tar` & `readwise_api-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-06-05 11:23:17.984758 readwise_api-0.2.0/LICENSE
--rw-r--r--   0        0        0      894 2023-06-05 11:24:44.440149 readwise_api-0.2.0/README.md
--rw-r--r--   0        0        0     1087 2023-06-06 09:22:35.213685 readwise_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      166 2023-06-05 19:41:30.855444 readwise_api-0.2.0/readwise/__init__.py
--rw-r--r--   0        0        0       67 2023-06-02 19:13:02.464917 readwise_api-0.2.0/readwise/__main__.py
--rw-r--r--   0        0        0     2382 2023-06-06 09:14:51.713351 readwise_api-0.2.0/readwise/api.py
--rw-r--r--   0        0        0     1029 2023-06-06 09:18:20.557441 readwise_api-0.2.0/readwise/cli.py
--rw-r--r--   0        0        0     1241 2023-06-05 13:16:45.999100 readwise_api-0.2.0/readwise/model.py
--rw-r--r--   0        0        0        0 2023-06-02 20:46:07.677659 readwise_api-0.2.0/readwise/py.typed
--rw-r--r--   0        0        0      143 2023-06-06 09:18:02.734226 readwise_api-0.2.0/readwise/version.py
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 readwise_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-05 11:23:17.984758 readwise_api-0.3.0/LICENSE
+-rw-r--r--   0        0        0      943 2023-06-06 09:26:28.497618 readwise_api-0.3.0/README.md
+-rw-r--r--   0        0        0     1087 2023-06-07 20:06:32.473743 readwise_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      198 2023-06-07 19:19:47.146091 readwise_api-0.3.0/readwise/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-02 19:13:02.464917 readwise_api-0.3.0/readwise/__main__.py
+-rw-r--r--   0        0        0     3647 2023-06-07 19:26:59.822693 readwise_api-0.3.0/readwise/api.py
+-rw-r--r--   0        0        0     1566 2023-06-07 20:04:43.746525 readwise_api-0.3.0/readwise/cli.py
+-rw-r--r--   0        0        0     3686 2023-06-07 19:35:31.075354 readwise_api-0.3.0/readwise/model.py
+-rw-r--r--   0        0        0        0 2023-06-02 20:46:07.677659 readwise_api-0.3.0/readwise/py.typed
+-rw-r--r--   0        0        0      144 2023-06-06 12:30:01.572615 readwise_api-0.3.0/readwise/version.py
+-rw-r--r--   0        0        0     1538 1970-01-01 00:00:00.000000 readwise_api-0.3.0/PKG-INFO
```

### Comparing `readwise_api-0.2.0/LICENSE` & `readwise_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readwise_api-0.2.0/README.md` & `readwise_api-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![logo](logo.png)
+![logo](https://github.com/floscha/readwise-api/raw/main/logo.png)
 
 # Readwise API
 
 An unofficial Python client for the [Readwise Reader API](https://readwise.io/reader_api).
 
 ## Installation
```

### Comparing `readwise_api-0.2.0/pyproject.toml` & `readwise_api-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "readwise-api"
-version = "0.2.0"
+version = "0.3.0"
 description = "An unofficial Python client for the Readwise Reader API."
 authors = ["Florian Schäfer <florian.joh.schaefer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "readwise"}]
 
 [tool.poetry.dependencies]
```

### Comparing `readwise_api-0.2.0/readwise/cli.py` & `readwise_api-0.3.0/readwise/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from typing import Optional
 
 import typer
 from typing_extensions import Annotated
 
-from readwise import get_document_by_id, get_documents
+from readwise import get_document_by_id, get_documents, save_document
 
 app = typer.Typer()
 
 
 @app.command()
 def list(location: str, n: Annotated[Optional[int], typer.Option("--number", "-n")] = None) -> None:
     """List documents.
@@ -33,7 +33,24 @@
         $ readwise get <document_id>
     """
     doc = get_document_by_id(id)
     if doc:
         print(doc.json(indent=2))
     else:
         print(f"No document with ID {id!r} could be found.")
+
+
+@app.command()
+def save(url: str) -> None:
+    """Save a document to Reader.
+
+    Params:
+        url (str): URL to the document from where it will be scraped by Readwise.
+
+    Usage:
+        $ readwise save "https://www.youtube.com/watch?v=dQw4w9WgXcQ"
+    """
+    document_already_exists, document_info = save_document(url)
+    if document_already_exists:
+        print(f"This document has already been saved earlier with ID {document_info.id!r}.")
+    else:
+        print(f"Saved new document {document_info.id!r}.")
```

### Comparing `readwise_api-0.2.0/PKG-INFO` & `readwise_api-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: readwise-api
-Version: 0.2.0
+Version: 0.3.0
 Summary: An unofficial Python client for the Readwise Reader API.
 License: MIT
 Author: Florian Schäfer
 Author-email: florian.joh.schaefer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
-![logo](logo.png)
+![logo](https://github.com/floscha/readwise-api/raw/main/logo.png)
 
 # Readwise API
 
 An unofficial Python client for the [Readwise Reader API](https://readwise.io/reader_api).
 
 ## Installation
```

