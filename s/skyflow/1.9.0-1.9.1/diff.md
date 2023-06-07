# Comparing `tmp/skyflow-1.9.0.tar.gz` & `tmp/skyflow-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyflow-1.9.0.tar", last modified: Wed Jun  7 11:54:49 2023, max compression
+gzip compressed data, was "skyflow-1.9.1.tar", last modified: Wed Jun  7 15:44:17 2023, max compression
```

## Comparing `skyflow-1.9.0.tar` & `skyflow-1.9.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 11:54:36.000000 skyflow-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-07 11:54:49.768780 skyflow-1.9.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-06-07 11:54:36.000000 skyflow-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 11:54:49.768780 skyflow-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-07 11:54:46.000000 skyflow-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/skyflow/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/skyflow/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/errors/_skyflow_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/skyflow/service_account/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/service_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/service_account/_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/service_account/_validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/skyflow/vault/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_detokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_get_by_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/skyflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-07 11:54:49.000000 skyflow-1.9.0/skyflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 11:54:49.000000 skyflow-1.9.0/skyflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:54:49.000000 skyflow-1.9.0/skyflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 11:54:49.000000 skyflow-1.9.0/skyflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 11:54:49.000000 skyflow-1.9.0/skyflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:44:17.159722 skyflow-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 15:44:04.000000 skyflow-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-07 15:44:17.159722 skyflow-1.9.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-06-07 15:44:04.000000 skyflow-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:44:17.159722 skyflow-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-07 15:44:14.000000 skyflow-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:44:17.159722 skyflow-1.9.1/skyflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:44:17.159722 skyflow-1.9.1/skyflow/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/errors/_skyflow_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:44:17.159722 skyflow-1.9.1/skyflow/service_account/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/service_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/service_account/_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/service_account/_validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:44:17.159722 skyflow-1.9.1/skyflow/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/vault/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/vault/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/vault/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/vault/_detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/vault/_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/vault/_get_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/vault/_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/vault/_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-07 15:44:04.000000 skyflow-1.9.1/skyflow/vault/_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 15:44:14.000000 skyflow-1.9.1/skyflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:44:17.159722 skyflow-1.9.1/skyflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-07 15:44:17.000000 skyflow-1.9.1/skyflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-07 15:44:17.000000 skyflow-1.9.1/skyflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:44:17.000000 skyflow-1.9.1/skyflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 15:44:17.000000 skyflow-1.9.1/skyflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 15:44:17.000000 skyflow-1.9.1/skyflow.egg-info/top_level.txt
```

### Comparing `skyflow-1.9.0/LICENSE` & `skyflow-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/PKG-INFO` & `skyflow-1.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyflow
-Version: 1.9.0
+Version: 1.9.1
 Summary: Skyflow SDK for the Python programming language
 Home-page: https://github.com/skyflowapi/skyflow-python/
 Author: Skyflow
 Author-email: service-ops@skyflow.com
 License: LICENSE
 Requires-Python: >=3.7
 License-File: LICENSE
```

### Comparing `skyflow-1.9.0/README.rst` & `skyflow-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/setup.py` & `skyflow-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 	Copyright (c) 2022 Skyflow, Inc.
 '''
 from setuptools import setup, find_packages
 import sys
 
 if sys.version_info < (3, 7):
     raise RuntimeError("skyflow requires Python 3.7+")
-current_version = '1.9.0'
+current_version = '1.9.1'
 
 setup(
     name='skyflow',
     version=current_version,
     author='Skyflow',
     author_email='service-ops@skyflow.com',
     packages=find_packages(where='.', exclude=['test*']),
```

### Comparing `skyflow-1.9.0/skyflow/_utils.py` & `skyflow-1.9.1/skyflow/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 	Copyright (c) 2022 Skyflow, Inc.
 '''
 import urllib.parse
 import logging
 from enum import Enum
 import platform
 import sys
-from version import SDK_VERSION
+from skyflow.version import SDK_VERSION
 
 skyflowLog = logging.getLogger('skyflow')
 skyflowLog.setLevel(logging.ERROR)
 
 supported_content_types = {
     "JSON": 'application/json',
     "PLAINTEXT": 'text/plain',
```

### Comparing `skyflow-1.9.0/skyflow/errors/_skyflow_errors.py` & `skyflow-1.9.1/skyflow/errors/_skyflow_errors.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow/service_account/_token.py` & `skyflow-1.9.1/skyflow/service_account/_token.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow/service_account/_validity.py` & `skyflow-1.9.1/skyflow/service_account/_validity.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow/vault/_client.py` & `skyflow-1.9.1/skyflow/vault/_client.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow/vault/_config.py` & `skyflow-1.9.1/skyflow/vault/_config.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow/vault/_connection.py` & `skyflow-1.9.1/skyflow/vault/_connection.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow/vault/_detokenize.py` & `skyflow-1.9.1/skyflow/vault/_detokenize.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow/vault/_get.py` & `skyflow-1.9.1/skyflow/vault/_get.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow/vault/_get_by_id.py` & `skyflow-1.9.1/skyflow/vault/_get_by_id.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow/vault/_insert.py` & `skyflow-1.9.1/skyflow/vault/_insert.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow/vault/_token.py` & `skyflow-1.9.1/skyflow/vault/_token.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow/vault/_update.py` & `skyflow-1.9.1/skyflow/vault/_update.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.9.0/skyflow.egg-info/PKG-INFO` & `skyflow-1.9.1/skyflow.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyflow
-Version: 1.9.0
+Version: 1.9.1
 Summary: Skyflow SDK for the Python programming language
 Home-page: https://github.com/skyflowapi/skyflow-python/
 Author: Skyflow
 Author-email: service-ops@skyflow.com
 License: LICENSE
 Requires-Python: >=3.7
 License-File: LICENSE
```

### Comparing `skyflow-1.9.0/skyflow.egg-info/SOURCES.txt` & `skyflow-1.9.1/skyflow.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.rst
 setup.py
 skyflow/__init__.py
 skyflow/_utils.py
+skyflow/version.py
 skyflow.egg-info/PKG-INFO
 skyflow.egg-info/SOURCES.txt
 skyflow.egg-info/dependency_links.txt
 skyflow.egg-info/requires.txt
 skyflow.egg-info/top_level.txt
 skyflow/errors/__init__.py
 skyflow/errors/_skyflow_errors.py
```

