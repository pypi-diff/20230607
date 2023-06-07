# Comparing `tmp/LumosWeb-1.0.2.tar.gz` & `tmp/LumosWeb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LumosWeb-1.0.2.tar", last modified: Sat Jun  3 14:08:11 2023, max compression
+gzip compressed data, was "LumosWeb-1.0.3.tar", last modified: Wed Jun  7 07:39:56 2023, max compression
```

## Comparing `LumosWeb-1.0.2.tar` & `LumosWeb-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-03 14:08:11.747745 LumosWeb-1.0.2/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-03 14:08:11.377385 LumosWeb-1.0.2/LumosWeb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-1.0.2/LumosWeb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5438 2023-06-03 13:53:15.000000 LumosWeb-1.0.2/LumosWeb/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-05-31 20:54:27.000000 LumosWeb-1.0.2/LumosWeb/cli.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-1.0.2/LumosWeb/middleware.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      976 2023-05-31 12:39:35.000000 LumosWeb-1.0.2/LumosWeb/response.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-03 14:08:11.688496 LumosWeb-1.0.2/LumosWeb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4332 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      309 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4332 2023-06-03 14:08:11.740742 LumosWeb-1.0.2/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4162 2023-06-03 11:15:30.000000 LumosWeb-1.0.2/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-03 14:08:11.751058 LumosWeb-1.0.2/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-06-03 14:07:04.000000 LumosWeb-1.0.2/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 07:39:56.274551 LumosWeb-1.0.3/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 07:39:55.951808 LumosWeb-1.0.3/LumosWeb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-1.0.3/LumosWeb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5438 2023-06-03 13:53:15.000000 LumosWeb-1.0.3/LumosWeb/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-05-31 20:54:27.000000 LumosWeb-1.0.3/LumosWeb/cli.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-1.0.3/LumosWeb/middleware.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6349 2023-06-07 07:36:56.000000 LumosWeb-1.0.3/LumosWeb/orm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      976 2023-05-31 12:39:35.000000 LumosWeb-1.0.3/LumosWeb/response.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 07:39:56.221969 LumosWeb-1.0.3/LumosWeb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4417 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4417 2023-06-07 07:39:56.268591 LumosWeb-1.0.3/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4249 2023-06-03 20:19:34.000000 LumosWeb-1.0.3/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-07 07:39:56.278043 LumosWeb-1.0.3/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-06-07 07:39:22.000000 LumosWeb-1.0.3/setup.py
```

### Comparing `LumosWeb-1.0.2/LumosWeb/api.py` & `LumosWeb-1.0.3/LumosWeb/api.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.2/LumosWeb/cli.py` & `LumosWeb-1.0.3/LumosWeb/cli.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.2/LumosWeb/middleware.py` & `LumosWeb-1.0.3/LumosWeb/middleware.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.2/LumosWeb/response.py` & `LumosWeb-1.0.3/LumosWeb/response.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.2/LumosWeb.egg-info/PKG-INFO` & `LumosWeb-1.0.3/LumosWeb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 1.0.2
+Version: 1.0.3
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
-## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
+# LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 - To ensure compatibility and access the latest features and improvements, it is highly recommended to use version 1.0.0 or higher of the package. 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 - [PyPI Release](https://pypi.org/project/LumosWeb/)
 - [Sample App](https://github.com/Sddilora/LumosWeb-SampleApp)
 
 
 
 ## Installation
 ```shell
 pip install LumosWeb==<latest_version>
-e.g. pip install LumosWeb==0.0.2
+e.g. pip install LumosWeb==1.0.0
 ```
 
 ## Getting Started
 
-### Basic usage
+## Basic usage
 
 ### Define App
 
 ```python
 from LumosWeb.api import API()
 app = API()  # We created our api instance
 ```
@@ -54,16 +54,18 @@
 def handler(req, resp):
     resp.text = "We don't have to use decorators!"
 
 app.add_route("/sample", handler, allowed_methods=["get", "post"])
 
 
 ```
-### Run Server
+### Run Server 
+Go to the directory on Terminal where your api instance is located
 > Lumosweb --app <module_name> run
+And lights are on!
 
 ### Unit Test
 
 The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
 that you may want to use when writing unit tests with LumosWeb. The first one is `app` which is an instance of the main `API` class:
 ```python
 def test_basic_route_adding(api):
```

### Comparing `LumosWeb-1.0.2/PKG-INFO` & `LumosWeb-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 1.0.2
+Version: 1.0.3
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
-## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
+# LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 - To ensure compatibility and access the latest features and improvements, it is highly recommended to use version 1.0.0 or higher of the package. 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 - [PyPI Release](https://pypi.org/project/LumosWeb/)
 - [Sample App](https://github.com/Sddilora/LumosWeb-SampleApp)
 
 
 
 ## Installation
 ```shell
 pip install LumosWeb==<latest_version>
-e.g. pip install LumosWeb==0.0.2
+e.g. pip install LumosWeb==1.0.0
 ```
 
 ## Getting Started
 
-### Basic usage
+## Basic usage
 
 ### Define App
 
 ```python
 from LumosWeb.api import API()
 app = API()  # We created our api instance
 ```
@@ -54,16 +54,18 @@
 def handler(req, resp):
     resp.text = "We don't have to use decorators!"
 
 app.add_route("/sample", handler, allowed_methods=["get", "post"])
 
 
 ```
-### Run Server
+### Run Server 
+Go to the directory on Terminal where your api instance is located
 > Lumosweb --app <module_name> run
+And lights are on!
 
 ### Unit Test
 
 The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
 that you may want to use when writing unit tests with LumosWeb. The first one is `app` which is an instance of the main `API` class:
 ```python
 def test_basic_route_adding(api):
```

### Comparing `LumosWeb-1.0.2/README.md` & `LumosWeb-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
+# LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 - To ensure compatibility and access the latest features and improvements, it is highly recommended to use version 1.0.0 or higher of the package. 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 - [PyPI Release](https://pypi.org/project/LumosWeb/)
 - [Sample App](https://github.com/Sddilora/LumosWeb-SampleApp)
 
 
 
 ## Installation
 ```shell
 pip install LumosWeb==<latest_version>
-e.g. pip install LumosWeb==0.0.2
+e.g. pip install LumosWeb==1.0.0
 ```
 
 ## Getting Started
 
-### Basic usage
+## Basic usage
 
 ### Define App
 
 ```python
 from LumosWeb.api import API()
 app = API()  # We created our api instance
 ```
@@ -42,16 +42,18 @@
 def handler(req, resp):
     resp.text = "We don't have to use decorators!"
 
 app.add_route("/sample", handler, allowed_methods=["get", "post"])
 
 
 ```
-### Run Server
+### Run Server 
+Go to the directory on Terminal where your api instance is located
 > Lumosweb --app <module_name> run
+And lights are on!
 
 ### Unit Test
 
 The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
 that you may want to use when writing unit tests with LumosWeb. The first one is `app` which is an instance of the main `API` class:
 ```python
 def test_basic_route_adding(api):
```

### Comparing `LumosWeb-1.0.2/setup.py` & `LumosWeb-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "LumosWeb"
 DESCRIPTION = "LumosWeb is web framework, simple and effective usage"
 EMAIL = "sumeyyedilaradogan@gmail.com"
 AUTHOR = "Sddilora"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

