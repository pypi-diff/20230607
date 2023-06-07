# Comparing `tmp/gradio_client-0.2.5.tar.gz` & `tmp/gradio_client-0.2.6.tar.gz`

## Comparing `gradio_client-0.2.5.tar` & `gradio_client-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.5/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.5/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/__init__.py
--rw-r--r--   0        0        0    47450 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/client.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/media_data.py
--rw-r--r--   0        0        0    19194 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/serializing.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/types.json
--rw-r--r--   0        0        0    16262 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/version.txt
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 gradio_client-0.2.5/.gitignore
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.6/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.6/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/__init__.py
+-rw-r--r--   0        0        0    47504 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/client.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/media_data.py
+-rw-r--r--   0        0        0    19138 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/serializing.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/types.json
+-rw-r--r--   0        0        0    16093 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/version.txt
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 gradio_client-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 gradio_client-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 gradio_client-0.2.6/PKG-INFO
```

### Comparing `gradio_client-0.2.5/README.md` & `gradio_client-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.5/gradio_client/client.py` & `gradio_client-0.2.6/gradio_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             token=hf_token,
             library_name="gradio_client",
             library_version=utils.__version__,
         )
         self.space_id = None
 
         if src.startswith("http://") or src.startswith("https://"):
-            _src = src
+            _src = src if src.endswith("/") else src + "/"
         else:
             _src = self._space_name_to_src(src)
             if _src is None:
                 raise ValueError(
                     f"Could not find Space: {src}. If it is a private Space, please provide an hf_token."
                 )
             self.space_id = src
@@ -606,15 +606,14 @@
     def __repr__(self):
         return f"Endpoint src: {self.client.src}, api_name: {self.api_name}, fn_index: {self.fn_index}"
 
     def __str__(self):
         return self.__repr__()
 
     def make_end_to_end_fn(self, helper: Communicator | None = None):
-
         _predict = self.make_predict(helper)
 
         def _inner(*data):
             if not self.is_valid:
                 raise utils.InvalidAPIEndpointError()
             data = self.insert_state(*data)
             if self.client.serialize:
@@ -782,16 +781,16 @@
 
         files = [
             f
             for f, t in zip(data, self.input_component_types)
             if t in ["file", "uploadbutton"]
         ]
         uploaded_files = self._upload(files)
-        self._add_uploaded_files_to_data(uploaded_files, list(data))
-
+        data = list(data)
+        self._add_uploaded_files_to_data(uploaded_files, data)
         o = tuple([s.serialize(d) for s, d in zip(self.serializers, data)])
         return o
 
     def deserialize(self, *data) -> tuple:
         assert len(data) == len(
             self.deserializers
         ), f"Expected {len(self.deserializers)} outputs, got {len(data)}"
```

### Comparing `gradio_client-0.2.5/gradio_client/documentation.py` & `gradio_client-0.2.6/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.5/gradio_client/media_data.py` & `gradio_client-0.2.6/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.5/gradio_client/serializing.py` & `gradio_client-0.2.6/gradio_client/serializing.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,19 +282,17 @@
                 filepath = x.get("name")
                 assert filepath is not None, f"The 'name' field is missing in {x}"
                 if root_url is not None:
                     file_name = utils.download_tmp_copy_of_file(
                         root_url + "file=" + filepath,
                         hf_token=hf_token,
                         dir=save_dir,
-                    ).name
+                    )
                 else:
-                    file_name = utils.create_tmp_copy_of_file(
-                        filepath, dir=save_dir
-                    ).name
+                    file_name = utils.create_tmp_copy_of_file(filepath, dir=save_dir)
             else:
                 data = x.get("data")
                 assert data is not None, f"The 'data' field is missing in {x}"
                 file_name = utils.decode_base64_to_file(data, dir=save_dir).name
         else:
             raise ValueError(
                 f"A FileSerializable component can only deserialize a string or a dict, not a {type(x)}: {x}"
```

### Comparing `gradio_client-0.2.5/gradio_client/types.json` & `gradio_client-0.2.6/gradio_client/types.json`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.5/gradio_client/utils.py` & `gradio_client-0.2.6/gradio_client/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio
 import base64
 import json
 import mimetypes
 import os
 import pkgutil
+import secrets
 import shutil
 import tempfile
 from concurrent.futures import CancelledError
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
@@ -19,22 +20,22 @@
 import fsspec.asyn
 import httpx
 import huggingface_hub
 import requests
 from huggingface_hub import SpaceStage
 from websockets.legacy.protocol import WebSocketCommonProtocol
 
-API_URL = "/api/predict/"
-WS_URL = "/queue/join"
-UPLOAD_URL = "/upload"
-CONFIG_URL = "/config"
-API_INFO_URL = "/info"
-RAW_API_INFO_URL = "/info?serialize=False"
+API_URL = "api/predict/"
+WS_URL = "queue/join"
+UPLOAD_URL = "upload"
+CONFIG_URL = "config"
+API_INFO_URL = "info"
+RAW_API_INFO_URL = "info?serialize=False"
 SPACE_FETCHER_URL = "https://gradio-space-api-fetcher-v2.hf.space/api"
-RESET_URL = "/reset"
+RESET_URL = "reset"
 SPACE_URL = "https://hf.space/{}"
 
 STATE_COMPONENT = "state"
 INVALID_RUNTIME = [
     SpaceStage.NO_APP_FILE,
     SpaceStage.CONFIG_ERROR,
     SpaceStage.BUILD_ERROR,
@@ -269,48 +270,35 @@
 ########################
 # Data processing utils
 ########################
 
 
 def download_tmp_copy_of_file(
     url_path: str, hf_token: str | None = None, dir: str | None = None
-) -> tempfile._TemporaryFileWrapper:
+) -> str:
     if dir is not None:
         os.makedirs(dir, exist_ok=True)
     headers = {"Authorization": "Bearer " + hf_token} if hf_token else {}
-    prefix = Path(url_path).stem
-    suffix = Path(url_path).suffix
-    file_obj = tempfile.NamedTemporaryFile(
-        delete=False,
-        prefix=prefix,
-        suffix=suffix,
-        dir=dir,
-    )
+    directory = Path(dir or tempfile.gettempdir()) / secrets.token_hex(20)
+    directory.mkdir(exist_ok=True, parents=True)
+    file_path = directory / Path(url_path).name
+
     with requests.get(url_path, headers=headers, stream=True) as r, open(
-        file_obj.name, "wb"
+        file_path, "wb"
     ) as f:
         shutil.copyfileobj(r.raw, f)
-    return file_obj
+    return str(file_path.resolve())
 
 
-def create_tmp_copy_of_file(
-    file_path: str, dir: str | None = None
-) -> tempfile._TemporaryFileWrapper:
-    if dir is not None:
-        os.makedirs(dir, exist_ok=True)
-    prefix = Path(file_path).stem
-    suffix = Path(file_path).suffix
-    file_obj = tempfile.NamedTemporaryFile(
-        delete=False,
-        prefix=prefix,
-        suffix=suffix,
-        dir=dir,
-    )
-    shutil.copy2(file_path, file_obj.name)
-    return file_obj
+def create_tmp_copy_of_file(file_path: str, dir: str | None = None) -> str:
+    directory = Path(dir or tempfile.gettempdir()) / secrets.token_hex(20)
+    directory.mkdir(exist_ok=True, parents=True)
+    dest = directory / Path(file_path).name
+    shutil.copy2(file_path, dest)
+    return str(dest.resolve())
 
 
 def get_mimetype(filename: str) -> str | None:
     if filename.endswith(".vtt"):
         return "text/vtt"
     mimetype = mimetypes.guess_type(filename)[0]
     if mimetype is not None:
```

### Comparing `gradio_client-0.2.5/.gitignore` & `gradio_client-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.5/pyproject.toml` & `gradio_client-0.2.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,30 @@
   { name = "Dawood Khan", email = "team@gradio.app" },
   { name = "Ahsen Khaliq", email = "team@gradio.app" },
   { name = "Pete Allen", email = "team@gradio.app" },
   { name = "Freddy Boulton", email = "team@gradio.app" },
 ]
 keywords = ["machine learning", "client", "API"]
 
+classifiers = [
+  'Development Status :: 4 - Beta',
+  'License :: OSI Approved :: Apache Software License',
+  'Operating System :: OS Independent',
+  'Programming Language :: Python :: 3',
+  'Programming Language :: Python :: 3 :: Only',
+  'Programming Language :: Python :: 3.7',
+  'Programming Language :: Python :: 3.8',
+  'Programming Language :: Python :: 3.9',
+  'Programming Language :: Python :: 3.10',
+  'Programming Language :: Python :: 3.11',
+  'Topic :: Scientific/Engineering',
+  'Topic :: Scientific/Engineering :: Artificial Intelligence',
+  'Topic :: Software Development :: User Interfaces',
+]
+
 [project.urls]
 Homepage = "https://github.com/gradio-app/gradio"
 
 [tool.hatch.version]
 path = "gradio_client/version.txt"
 pattern = "(?P<version>.+)"
```

### Comparing `gradio_client-0.2.5/PKG-INFO` & `gradio_client-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Requires-Dist: fsspec
 Requires-Dist: httpx
 Requires-Dist: huggingface-hub>=0.13.0
 Requires-Dist: packaging
 Requires-Dist: requests
 Requires-Dist: typing-extensions
```

