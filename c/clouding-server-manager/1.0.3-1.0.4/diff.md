# Comparing `tmp/clouding_server_manager-1.0.3.tar.gz` & `tmp/clouding_server_manager-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clouding_server_manager-1.0.3.tar", max compression
+gzip compressed data, was "clouding_server_manager-1.0.4.tar", max compression
```

## Comparing `clouding_server_manager-1.0.3.tar` & `clouding_server_manager-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-01 21:40:31.138645 clouding_server_manager-1.0.3/LICENSE
--rw-r--r--   0        0        0     6956 2023-05-31 12:43:05.495556 clouding_server_manager-1.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-25 23:26:38.831500 clouding_server_manager-1.0.3/clouding_server_manager/__init__.py
--rw-r--r--   0        0        0      590 2023-05-26 10:08:29.138115 clouding_server_manager-1.0.3/clouding_server_manager/__main__.py
--rw-r--r--   0        0        0     3998 2023-05-26 09:45:25.433435 clouding_server_manager-1.0.3/clouding_server_manager/commands.py
--rw-r--r--   0        0        0      782 2023-05-26 09:45:32.340190 clouding_server_manager-1.0.3/clouding_server_manager/constants.py
--rw-r--r--   0        0        0     7418 2023-05-26 09:45:23.540078 clouding_server_manager-1.0.3/clouding_server_manager/helpers.py
--rw-r--r--   0        0        0      898 2023-05-31 12:41:43.478012 clouding_server_manager-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     7565 1970-01-01 00:00:00.000000 clouding_server_manager-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-01 21:40:31.138645 clouding_server_manager-1.0.4/LICENSE
+-rw-r--r--   0        0        0     6956 2023-06-06 10:05:32.541615 clouding_server_manager-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 23:26:38.831500 clouding_server_manager-1.0.4/clouding_server_manager/__init__.py
+-rw-r--r--   0        0        0      590 2023-05-26 10:08:29.138115 clouding_server_manager-1.0.4/clouding_server_manager/__main__.py
+-rw-r--r--   0        0        0     3998 2023-05-26 09:45:25.433435 clouding_server_manager-1.0.4/clouding_server_manager/commands.py
+-rw-r--r--   0        0        0      782 2023-06-06 10:06:49.903304 clouding_server_manager-1.0.4/clouding_server_manager/constants.py
+-rw-r--r--   0        0        0     7418 2023-05-26 09:45:23.540078 clouding_server_manager-1.0.4/clouding_server_manager/helpers.py
+-rw-r--r--   0        0        0      898 2023-06-06 10:06:22.916055 clouding_server_manager-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7565 1970-01-01 00:00:00.000000 clouding_server_manager-1.0.4/PKG-INFO
```

### Comparing `clouding_server_manager-1.0.3/LICENSE` & `clouding_server_manager-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.3/README.md` & `clouding_server_manager-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Clouding Server Manager
-![Version](https://img.shields.io/badge/Version-1.0.3-brightgreen.svg)
+![Version](https://img.shields.io/badge/Version-1.0.4-brightgreen.svg)
 ![Python](https://img.shields.io/badge/Python-3.9-brightgreen.svg)
 ![License](https://img.shields.io/badge/License-MIT-blue.svg)
 
 Clouding Server Manager is a Python project that allows you to manage your Clouding servers from the command line. It is designed to list, archive, and unarchive servers in your Clouding account. It uses the [Clouding API](https://api.clouding.io/docs) to perform the actions.
 
 ## Table of Contents
 * [Features](#features)
```

### Comparing `clouding_server_manager-1.0.3/clouding_server_manager/__main__.py` & `clouding_server_manager-1.0.4/clouding_server_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.3/clouding_server_manager/commands.py` & `clouding_server_manager-1.0.4/clouding_server_manager/commands.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.3/clouding_server_manager/constants.py` & `clouding_server_manager-1.0.4/clouding_server_manager/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module contains the constants used in the project"""
 
 BASE_URL = "https://api.clouding.io/v1"
 """The base URL of the API"""
 
-WAIT_TIME = 15
+WAIT_TIME = 10
 """The time to wait between each request to the API when archiving or unarchiving servers"""
 
 MAX_TOTAL_WAIT_TIME = 300
 """The maximum total time to wait for all servers to be unarchived or archived"""
 
 API_ALREADY_ARCHIVED_ERROR_MESSAGE = "Command 'shelve' cannot be issued while server is in the current state"
 """The error message returned by the API when trying to archive a server that is already archived"""
```

### Comparing `clouding_server_manager-1.0.3/clouding_server_manager/helpers.py` & `clouding_server_manager-1.0.4/clouding_server_manager/helpers.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.3/pyproject.toml` & `clouding_server_manager-1.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clouding-server-manager"
-version = "1.0.3"
+version = "1.0.4"
 description = "A Python project to easily manage Clouding servers from the command line."
 authors = ["dmarts05 <dmarts05@estudiantes.unileon.es>"]
 readme = "README.md"
 packages = [{include = "clouding_server_manager"}]
 
 [tool.poetry.scripts]
 clouding-sm = "clouding_server_manager.__main__:main"
```

### Comparing `clouding_server_manager-1.0.3/PKG-INFO` & `clouding_server_manager-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: clouding-server-manager
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python project to easily manage Clouding servers from the command line.
 Author: dmarts05
 Author-email: dmarts05@estudiantes.unileon.es
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Clouding Server Manager
-![Version](https://img.shields.io/badge/Version-1.0.3-brightgreen.svg)
+![Version](https://img.shields.io/badge/Version-1.0.4-brightgreen.svg)
 ![Python](https://img.shields.io/badge/Python-3.9-brightgreen.svg)
 ![License](https://img.shields.io/badge/License-MIT-blue.svg)
 
 Clouding Server Manager is a Python project that allows you to manage your Clouding servers from the command line. It is designed to list, archive, and unarchive servers in your Clouding account. It uses the [Clouding API](https://api.clouding.io/docs) to perform the actions.
 
 ## Table of Contents
 * [Features](#features)
```

