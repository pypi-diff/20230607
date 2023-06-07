# Comparing `tmp/weave-py-api-1.0.0.tar.gz` & `tmp/weave-py-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weave-py-api-1.0.0.tar", last modified: Wed Jun  7 06:33:34 2023, max compression
+gzip compressed data, was "weave-py-api-1.1.0.tar", last modified: Wed Jun  7 06:52:56 2023, max compression
```

## Comparing `weave-py-api-1.0.0.tar` & `weave-py-api-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 06:33:34.705804 weave-py-api-1.0.0/
--rw-rw-rw-   0        0        0     1086 2023-06-07 05:54:07.000000 weave-py-api-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       15 2023-06-07 06:24:55.000000 weave-py-api-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1972 2023-06-07 06:33:34.691800 weave-py-api-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      169 2023-06-07 06:32:45.000000 weave-py-api-1.0.0/README.md
--rw-rw-rw-   0        0        0     1436 2023-06-07 06:32:02.000000 weave-py-api-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 06:33:34.706799 weave-py-api-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-07 06:33:34.666798 weave-py-api-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 06:33:34.689799 weave-py-api-1.0.0/src/weave_py_api.egg-info/
--rw-rw-rw-   0        0        0     1972 2023-06-07 06:33:34.000000 weave-py-api-1.0.0/src/weave_py_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-06-07 06:33:34.000000 weave-py-api-1.0.0/src/weave_py_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 06:33:34.000000 weave-py-api-1.0.0/src/weave_py_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      178 2023-06-07 06:33:34.000000 weave-py-api-1.0.0/src/weave_py_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 06:33:34.000000 weave-py-api-1.0.0/src/weave_py_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 06:33:34.690800 weave-py-api-1.0.0/src/weaveapi/
--rw-rw-rw-   0        0        0      543 2023-06-07 06:00:12.000000 weave-py-api-1.0.0/src/weaveapi/config.toml
+drwxrwxrwx   0        0        0        0 2023-06-07 06:52:56.108037 weave-py-api-1.1.0/
+-rw-rw-rw-   0        0        0     1086 2023-06-07 05:54:07.000000 weave-py-api-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       15 2023-06-07 06:24:55.000000 weave-py-api-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1972 2023-06-07 06:52:56.108037 weave-py-api-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2023-06-07 06:32:45.000000 weave-py-api-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1436 2023-06-07 06:48:40.000000 weave-py-api-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 06:52:56.108037 weave-py-api-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 06:52:56.072039 weave-py-api-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 06:52:56.083036 weave-py-api-1.1.0/src/weave_py_api.egg-info/
+-rw-rw-rw-   0        0        0     1972 2023-06-07 06:52:56.000000 weave-py-api-1.1.0/src/weave_py_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-06-07 06:52:56.000000 weave-py-api-1.1.0/src/weave_py_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 06:52:56.000000 weave-py-api-1.1.0/src/weave_py_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      178 2023-06-07 06:52:56.000000 weave-py-api-1.1.0/src/weave_py_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 06:52:56.000000 weave-py-api-1.1.0/src/weave_py_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 06:52:56.107038 weave-py-api-1.1.0/src/weaveapi/
+-rw-rw-rw-   0        0        0        0 2022-03-20 14:22:30.000000 weave-py-api-1.1.0/src/weaveapi/__init__.py
+-rw-rw-rw-   0        0        0     3817 2023-01-27 18:40:16.000000 weave-py-api-1.1.0/src/weaveapi/apicontext.py
+-rw-rw-rw-   0        0        0    34203 2023-05-09 11:29:57.000000 weave-py-api-1.1.0/src/weaveapi/clienthttp.py
+-rw-rw-rw-   0        0        0    40963 2023-05-09 11:29:57.000000 weave-py-api-1.1.0/src/weaveapi/clientws.py
+-rw-rw-rw-   0        0        0     3968 2023-02-28 07:27:53.000000 weave-py-api-1.1.0/src/weaveapi/filter.py
+-rw-rw-rw-   0        0        0      363 2022-03-20 14:22:30.000000 weave-py-api-1.1.0/src/weaveapi/futures.py
+-rw-rw-rw-   0        0        0     5015 2022-12-30 12:27:54.000000 weave-py-api-1.1.0/src/weaveapi/javarandom.py
+-rw-rw-rw-   0        0        0     3455 2022-12-12 12:20:08.000000 weave-py-api-1.1.0/src/weaveapi/keys.py
+-rw-rw-rw-   0        0        0    14919 2023-05-09 11:29:57.000000 weave-py-api-1.1.0/src/weaveapi/nodeapi.py
+-rw-rw-rw-   0        0        0    14300 2023-04-05 10:54:57.000000 weave-py-api-1.1.0/src/weaveapi/options.py
+-rw-rw-rw-   0        0        0      984 2022-12-30 12:27:54.000000 weave-py-api-1.1.0/src/weaveapi/records.py
+-rw-rw-rw-   0        0        0      884 2023-01-23 13:53:04.000000 weave-py-api-1.1.0/src/weaveapi/session.py
+-rw-rw-rw-   0        0        0      894 2022-03-28 18:45:18.000000 weave-py-api-1.1.0/src/weaveapi/setup.py
+-rw-rw-rw-   0        0        0     4282 2023-01-25 16:39:28.000000 weave-py-api-1.1.0/src/weaveapi/utils.py
+-rw-rw-rw-   0        0        0       81 2022-03-20 14:22:30.000000 weave-py-api-1.1.0/src/weaveapi/weaveapi.py
+-rw-rw-rw-   0        0        0     4980 2023-03-15 09:17:36.000000 weave-py-api-1.1.0/src/weaveapi/weaveh.py
```

### Comparing `weave-py-api-1.0.0/LICENSE` & `weave-py-api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.0.0/PKG-INFO` & `weave-py-api-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weave-py-api
-Version: 1.0.0
+Version: 1.1.0
 Summary: Weavechain Python API
 Author-email: Weavechain <support@weavechain.com>
 License: MIT License
         
         Copyright (c) 2023 Weavechain
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,15 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/weavechain/weave-py-api
 Keywords: weavechain,weave,api,layer-0,data,sharing,monetization,compute,node
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ## Weavechain Python API
 
 [https://weavechain.com](https://weavechain.com): Layer-0 For Data
```

### Comparing `weave-py-api-1.0.0/pyproject.toml` & `weave-py-api-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "weave-py-api"
-version = "1.0.0"
+version = "1.1.0"
 description = "Weavechain Python API"
 readme = "README.md"
 authors = [{ name = "Weavechain", email = "support@weavechain.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -26,26 +26,26 @@
     "websocket-client",
     "cryptography",
     "PyCryptodome",
     "paramiko",
     "java-random",
     'tomli; python_version < "3.11"',
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.5"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/weavechain/weave-py-api"
 
 [project.scripts]
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `weave-py-api-1.0.0/src/weave_py_api.egg-info/PKG-INFO` & `weave-py-api-1.1.0/src/weave_py_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weave-py-api
-Version: 1.0.0
+Version: 1.1.0
 Summary: Weavechain Python API
 Author-email: Weavechain <support@weavechain.com>
 License: MIT License
         
         Copyright (c) 2023 Weavechain
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,15 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/weavechain/weave-py-api
 Keywords: weavechain,weave,api,layer-0,data,sharing,monetization,compute,node
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ## Weavechain Python API
 
 [https://weavechain.com](https://weavechain.com): Layer-0 For Data
```

