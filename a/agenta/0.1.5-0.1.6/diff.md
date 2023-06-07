# Comparing `tmp/agenta-0.1.5.tar.gz` & `tmp/agenta-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agenta-0.1.5.tar", max compression
+gzip compressed data, was "agenta-0.1.6.tar", max compression
```

## Comparing `agenta-0.1.5.tar` & `agenta-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.5/README.md
--rw-r--r--   0        0        0       53 2023-06-05 15:08:40.153249 agenta-0.1.5/agenta/__init__.py
--rw-r--r--   0        0        0     3079 2023-06-05 15:08:40.153705 agenta-0.1.5/agenta/agenta.py
--rw-r--r--   0        0        0     2378 2023-06-05 14:29:35.924380 agenta-0.1.5/agenta/cli/helper.py
--rw-r--r--   0        0        0     2108 2023-06-05 14:29:35.924670 agenta-0.1.5/agenta/cli/main.py
--rw-r--r--   0        0        0     8450 2023-06-05 14:29:35.924942 agenta-0.1.5/agenta/cli/variant_commands.py
--rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.5/agenta/client/Readme.md
--rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.5/agenta/client/__init__.py
--rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.5/agenta/client/api_models.py
--rw-r--r--   0        0        0     4355 2023-06-05 14:29:35.925335 agenta-0.1.5/agenta/client/client.py
--rw-r--r--   0        0        0      641 2023-06-05 14:29:35.925644 agenta-0.1.5/agenta/config.py
--rw-r--r--   0        0        0      131 2023-06-05 14:29:35.926009 agenta-0.1.5/agenta/config.toml
--rw-r--r--   0        0        0      337 2023-05-24 09:05:58.092867 agenta-0.1.5/agenta/docker/docker-assets/Dockerfile.template
--rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.5/agenta/docker/docker-assets/README.md
--rw-r--r--   0        0        0      256 2023-05-20 06:49:49.205919 agenta-0.1.5/agenta/docker/docker-assets/main.py
--rw-r--r--   0        0        0     2585 2023-06-05 15:08:40.154263 agenta-0.1.5/agenta/docker/docker_utils.py
--rw-r--r--   0        0        0      482 2023-05-31 17:12:43.842983 agenta-0.1.5/agenta/templates/simple_prompt/README.md
--rw-r--r--   0        0        0      660 2023-05-31 17:02:48.853909 agenta-0.1.5/agenta/templates/simple_prompt/app.py
--rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.5/agenta/templates/simple_prompt/requirements.txt
--rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.5/agenta/templates/simple_prompt/template.toml
--rw-r--r--   0        0        0      570 2023-06-05 17:24:54.120338 agenta-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 agenta-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.6/README.md
+-rw-r--r--   0        0        0       48 2023-06-07 08:35:40.016460 agenta-0.1.6/agenta/__init__.py
+-rw-r--r--   0        0        0     3198 2023-06-07 08:35:40.016930 agenta-0.1.6/agenta/agenta.py
+-rw-r--r--   0        0        0     2378 2023-06-05 14:29:35.924380 agenta-0.1.6/agenta/cli/helper.py
+-rw-r--r--   0        0        0     2108 2023-06-05 14:29:35.924670 agenta-0.1.6/agenta/cli/main.py
+-rw-r--r--   0        0        0     8450 2023-06-05 14:29:35.924942 agenta-0.1.6/agenta/cli/variant_commands.py
+-rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.6/agenta/client/Readme.md
+-rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.6/agenta/client/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.6/agenta/client/api_models.py
+-rw-r--r--   0        0        0     4355 2023-06-05 14:29:35.925335 agenta-0.1.6/agenta/client/client.py
+-rw-r--r--   0        0        0      641 2023-06-05 14:29:35.925644 agenta-0.1.6/agenta/config.py
+-rw-r--r--   0        0        0      131 2023-06-05 14:29:35.926009 agenta-0.1.6/agenta/config.toml
+-rw-r--r--   0        0        0      374 2023-06-07 08:59:05.567568 agenta-0.1.6/agenta/docker/docker-assets/Dockerfile.template
+-rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.6/agenta/docker/docker-assets/README.md
+-rw-r--r--   0        0        0      256 2023-05-20 06:49:49.205919 agenta-0.1.6/agenta/docker/docker-assets/main.py
+-rw-r--r--   0        0        0     2702 2023-06-07 09:02:57.670742 agenta-0.1.6/agenta/docker/docker_utils.py
+-rw-r--r--   0        0        0       43 2023-06-07 08:37:18.934913 agenta-0.1.6/agenta/templates/simple_prompt/.env.example
+-rw-r--r--   0        0        0      482 2023-05-31 17:12:43.842983 agenta-0.1.6/agenta/templates/simple_prompt/README.md
+-rw-r--r--   0        0        0      660 2023-05-31 17:02:48.853909 agenta-0.1.6/agenta/templates/simple_prompt/app.py
+-rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.6/agenta/templates/simple_prompt/requirements.txt
+-rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.6/agenta/templates/simple_prompt/template.toml
+-rw-r--r--   0        0        0      570 2023-06-07 09:11:07.717998 agenta-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 agenta-0.1.6/PKG-INFO
```

### Comparing `agenta-0.1.5/agenta/agenta.py` & `agenta-0.1.6/agenta/agenta.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """The code for the Agenta SDK"""
 import argparse
 import functools
 import inspect
 import os
 import sys
+import traceback
 from typing import Any, Callable, Optional
 
 from dotenv import load_dotenv
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
+from fastapi.responses import JSONResponse
 
 app = FastAPI()
 
 origins = [
     "http://localhost:3000",
     "http://localhost:3001",
 ]
@@ -52,15 +54,19 @@
     for name, param in app_params.items():
         default_value = param.default if param.default is not param.empty else None
         app_params[name] = default_value
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         kwargs = {**app_params, **kwargs}
-        return func(*args, **kwargs)
+        try:
+            return func(*args, **kwargs)
+        except Exception as e:
+            traceback_str = ''.join(traceback.format_exception(etype=type(e), value=e, tb=e.__traceback__))
+            return JSONResponse(status_code=500, content={"error": str(e), "traceback": traceback_str})
 
     new_params = []
     for name, param in sig.parameters.items():
         if name in app_params:
             new_params.append(
                 inspect.Parameter(
                     name,
@@ -91,21 +97,7 @@
                 # For required parameters, we add them as arguments
                 parser.add_argument(name, type=param.annotation)
 
         args = parser.parse_args()
         print(func(**vars(args)))
 
     return wrapper
-
-
-def get(func):
-    """get decorator
-
-    Arguments:
-        func -- _description_
-
-    Returns:
-        _description_
-    """
-    route = f"/{func.__name__}"
-    app.get(route)(func)
-    return func
```

### Comparing `agenta-0.1.5/agenta/cli/helper.py` & `agenta-0.1.6/agenta/cli/helper.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.5/agenta/cli/main.py` & `agenta-0.1.6/agenta/cli/main.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.5/agenta/cli/variant_commands.py` & `agenta-0.1.6/agenta/cli/variant_commands.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.5/agenta/client/client.py` & `agenta-0.1.6/agenta/client/client.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.5/agenta/config.py` & `agenta-0.1.6/agenta/config.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.5/agenta/docker/docker_utils.py` & `agenta-0.1.6/agenta/docker/docker_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import logging
 import os
 import shutil
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import docker
 from agenta.config import settings
 from docker.models.images import Image
 
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+
 
 def create_dockerfile(out_folder: Path):
     """Creates a dockerfile based on the template in the out_folder.
 
     Arguments:
         out_folder -- Folder in which to create the Dockerfile.
     """
@@ -54,21 +58,21 @@
         print("Building Docker image...")
         try:
             image, build_log = client.images.build(
                 path=temp_dir,
                 tag=tag,
                 rm=True  # Remove intermediate containers after a successful build
             )
-        except docker.errors.BuildError as e:
-            print("Error building Docker image:\n", e)
-            raise e
-
-        # Print the build log
-        for line in build_log:
-            print(line)
+
+        except docker.errors.BuildError as ex:
+            logger.error("Error building Docker image:\n" + ex)
+            # Print the build log
+            for line in ex.build_log:
+                logger.error(line)
+            raise ex
         # Upload the Docker image to the Agenta registry
         print("Uploading Docker image...")
         client.images.push(repository=f"{registry}", tag="latest")
         print("Docker image uploaded successfully.")
 
         # Clean up the temporary Dockerfile
         dockerfile_path.unlink()
```

### Comparing `agenta-0.1.5/agenta/templates/simple_prompt/app.py` & `agenta-0.1.6/agenta/templates/simple_prompt/app.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.5/pyproject.toml` & `agenta-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agenta"
-version = "0.1.5"
+version = "0.1.6"
 description = "Code for the SDK and CLI for the Agenta Lab platform"
 authors = ["Mahmoud Mabrouk <mahmoudmabrouk.mail@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docker = "^6.1.1"
```

### Comparing `agenta-0.1.5/PKG-INFO` & `agenta-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agenta
-Version: 0.1.5
+Version: 0.1.6
 Summary: Code for the SDK and CLI for the Agenta Lab platform
 Author: Mahmoud Mabrouk
 Author-email: mahmoudmabrouk.mail@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

