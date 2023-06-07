# Comparing `tmp/hkkang_utils-0.1.98.tar.gz` & `tmp/hkkang_utils-0.1.99.tar.gz`

## Comparing `hkkang_utils-0.1.98.tar` & `hkkang_utils-0.1.99.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/.github/workflows/deploy_doc.yml
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/.vscode/settings.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/docs/make.bat
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/docs/source/conf.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/docs/source/index.rst
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/__init__.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/concurrent.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/file.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/io.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/list.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/logger.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/metrics.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/misc.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/ml.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/pattern.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/pg.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/slack.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/socket.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/sql.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/string.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/tensor.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/testing.py
--rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/__init__.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_concurrent.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_file.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_io.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_list.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_metrics.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_misc.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_pattern.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_sql.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_string.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_testing.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_tensor/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_tensor/test_tensor.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_tensor/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/LICENSE
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/pyproject.toml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/.github/workflows/deploy_doc.yml
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/.vscode/settings.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/docs/make.bat
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/docs/source/conf.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/docs/source/index.rst
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/__init__.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/concurrent.py
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/file.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/io.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/list.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/logger.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/metrics.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/misc.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/ml.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/pattern.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/pg.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/slack.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/socket.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/sql.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/string.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/tensor.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/testing.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/src/hkkang_utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/__init__.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_concurrent.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_file.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_io.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_list.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_metrics.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_misc.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_pattern.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_sql.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_string.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_testing.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_tensor/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_tensor/test_tensor.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/tests/test_tensor/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/LICENSE
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hkkang_utils-0.1.99/PKG-INFO
```

### Comparing `hkkang_utils-0.1.98/.github/workflows/deploy_doc.yml` & `hkkang_utils-0.1.99/.github/workflows/deploy_doc.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/.github/workflows/unittest.yml` & `hkkang_utils-0.1.99/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/docs/Makefile` & `hkkang_utils-0.1.99/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/docs/make.bat` & `hkkang_utils-0.1.99/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/docs/source/conf.py` & `hkkang_utils-0.1.99/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/__init__.py` & `hkkang_utils-0.1.99/src/hkkang_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/concurrent.py` & `hkkang_utils-0.1.99/src/hkkang_utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/file.py` & `hkkang_utils-0.1.99/src/hkkang_utils/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import csv
 import inspect
-import ujson
 import os
 import pathlib
 import pickle
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import omegaconf
 import tqdm
+import ujson
 import yaml
 
 
 def get_files_in_directory(
     dir_path: str, filter_func: Optional[callable] = None, return_with_dir=False
 ) -> list:
     """Get paths of files in a directory
@@ -212,26 +212,33 @@
 
 # Related to csv file
 def read_csv_file(
     file_path: str,
     delimiter: str = ",",
     quotechar: str = '"',
     show_progress: bool = False,
+    first_row_as_header: bool = True,
     process_row_func: Callable = None,
-) -> List[Dict[str, Any]]:
+) -> List[Union[Dict[str, Any], List[Any]]]:
     dict_list = []
     with open(file_path, "r") as f:
         tsv_file_reader = csv.reader(f, delimiter=delimiter, quotechar=quotechar)
-        # Get headers
-        header = next(tsv_file_reader)
+        if first_row_as_header:
+            # Get headers
+            header = next(tsv_file_reader)
         # Get values
         file_iterator = tqdm.tqdm(tsv_file_reader) if show_progress else tsv_file_reader
         for row in file_iterator:
             row = process_row_func(row) if process_row_func else row
-            dict_list.append(dict(zip(header, row)))
+            if first_row_as_header:
+                # Save a dict if header is available
+                dict_list.append(dict(zip(header, row)))
+            else:
+                # Save a list if header is not available
+                dict_list.append(row)
     return dict_list
 
 
 def write_csv_file(
     list_of_dict: List[Dict[str, Any]], file_path: str, delimiter: str = ","
 ) -> None:
     with open(file_path, "w") as f:
```

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/list.py` & `hkkang_utils-0.1.99/src/hkkang_utils/list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/metrics.py` & `hkkang_utils-0.1.99/src/hkkang_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/misc.py` & `hkkang_utils-0.1.99/src/hkkang_utils/misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/ml.py` & `hkkang_utils-0.1.99/src/hkkang_utils/ml.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/pattern.py` & `hkkang_utils-0.1.99/src/hkkang_utils/pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/pg.py` & `hkkang_utils-0.1.99/src/hkkang_utils/pg.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/slack.py` & `hkkang_utils-0.1.99/src/hkkang_utils/slack.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import html
 import logging
 import os
 
 import attrs
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackApiError
 
@@ -64,15 +65,16 @@
         ip = socket_utils.get_local_ip()
         host_name = socket_utils.get_host_name()
         text_with_prefix = f"Message from {host_name}({ip}):\n{text}"
 
     # Send message
     try:
         response = client.chat_postMessage(channel=channel, text=text_with_prefix)
-        assert response["message"]["text"] == text_with_prefix
+        decoded_text = html.unescape(response["message"]["text"])
+        assert decoded_text == text_with_prefix, f"{decoded_text}"
         logger.info(f"Sending message to channel {channel}: {text}")
     except SlackApiError as e:
         # You will get a SlackApiError if "ok" is False
         assert e.response["ok"] is False
         assert e.response["error"], "channel_not_found"
         logger.info(f"Got an error: {e.response['error']}")
```

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/sql.py` & `hkkang_utils-0.1.99/src/hkkang_utils/sql.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/string.py` & `hkkang_utils-0.1.99/src/hkkang_utils/string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/tensor.py` & `hkkang_utils-0.1.99/src/hkkang_utils/tensor.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/src/hkkang_utils/time.py` & `hkkang_utils-0.1.99/src/hkkang_utils/time.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_concurrent.py` & `hkkang_utils-0.1.99/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_file.py` & `hkkang_utils-0.1.99/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_io.py` & `hkkang_utils-0.1.99/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_list.py` & `hkkang_utils-0.1.99/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_metrics.py` & `hkkang_utils-0.1.99/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_misc.py` & `hkkang_utils-0.1.99/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_pattern.py` & `hkkang_utils-0.1.99/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_string.py` & `hkkang_utils-0.1.99/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_testing.py` & `hkkang_utils-0.1.99/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_time.py` & `hkkang_utils-0.1.99/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_tensor/test_tensor.py` & `hkkang_utils-0.1.99/tests/test_tensor/test_tensor.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/tests/test_tensor/utils.py` & `hkkang_utils-0.1.99/tests/test_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/.gitignore` & `hkkang_utils-0.1.99/.gitignore`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/LICENSE` & `hkkang_utils-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.98/pyproject.toml` & `hkkang_utils-0.1.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hkkang_utils"
-version = "0.1.98"
+version = "0.1.99"
 authors = [{name="Hyukkyu Kang", email="hyukkyukang@gmail.com"}]
 description = "A collection of useful util functions"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hkkang_utils-0.1.98/PKG-INFO` & `hkkang_utils-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkkang_utils
-Version: 0.1.98
+Version: 0.1.99
 Summary: A collection of useful util functions
 Project-URL: Homepage, https://github.com/hyukkyukang/python_utils
 Project-URL: Bug Tracker, https://github.com/hyukkyukang/python_utils/issues
 Author-email: Hyukkyu Kang <hyukkyukang@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

