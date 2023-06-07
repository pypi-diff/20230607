# Comparing `tmp/cfg-argparser-1.2.0.tar.gz` & `tmp/cfg-argparser-1.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfg-argparser-1.2.0.tar", last modified: Wed Jun  7 05:59:14 2023, max compression
+gzip compressed data, was "cfg-argparser-1.2.0.post1.tar", last modified: Wed Jun  7 18:25:11 2023, max compression
```

## Comparing `cfg-argparser-1.2.0.tar` & `cfg-argparser-1.2.0.post1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 05:59:14.646680 cfg-argparser-1.2.0/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.2.0/LICENSE
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1667 2023-06-07 05:59:14.646680 cfg-argparser-1.2.0/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      812 2023-06-07 05:54:45.000000 cfg-argparser-1.2.0/README.md
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      929 2023-06-07 04:30:47.000000 cfg-argparser-1.2.0/pyproject.toml
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-06-07 05:59:14.646680 cfg-argparser-1.2.0/setup.cfg
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 05:59:14.640013 cfg-argparser-1.2.0/src/
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 05:59:14.643346 cfg-argparser-1.2.0/src/cfg_argparser/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      316 2023-06-07 03:20:42.000000 cfg-argparser-1.2.0/src/cfg_argparser/__init__.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     9978 2023-06-07 01:13:05.000000 cfg-argparser-1.2.0/src/cfg_argparser/argparse_config.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2882 2023-06-07 05:11:51.000000 cfg-argparser-1.2.0/src/cfg_argparser/cfg_dict.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1486 2023-06-07 05:55:21.000000 cfg-argparser-1.2.0/src/cfg_argparser/function_config_wrapper.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1391 2023-06-07 04:44:11.000000 cfg-argparser-1.2.0/src/cfg_argparser/save_handlers.py
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 05:59:14.643346 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1667 2023-06-07 05:59:14.000000 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      413 2023-06-07 05:59:14.000000 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/SOURCES.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-06-07 05:59:14.000000 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/dependency_links.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       20 2023-06-07 05:59:14.000000 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/requires.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-06-07 05:59:14.000000 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/top_level.txt
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 18:25:11.526805 cfg-argparser-1.2.0.post1/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.2.0.post1/LICENSE
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1632 2023-06-07 18:25:11.523472 cfg-argparser-1.2.0.post1/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      771 2023-06-07 15:54:57.000000 cfg-argparser-1.2.0.post1/README.md
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      959 2023-06-07 18:24:48.000000 cfg-argparser-1.2.0.post1/pyproject.toml
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-06-07 18:25:11.526805 cfg-argparser-1.2.0.post1/setup.cfg
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 18:25:11.523472 cfg-argparser-1.2.0.post1/src/
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 18:25:11.523472 cfg-argparser-1.2.0.post1/src/cfg_argparser/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      316 2023-06-07 03:20:42.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser/__init__.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     9978 2023-06-07 01:13:05.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser/argparse_config.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2882 2023-06-07 05:11:51.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser/cfg_dict.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1486 2023-06-07 05:55:21.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser/function_config_wrapper.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1391 2023-06-07 18:09:29.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser/save_handlers.py
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 18:25:11.523472 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1632 2023-06-07 18:25:11.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      413 2023-06-07 18:25:11.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/SOURCES.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-06-07 18:25:11.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/dependency_links.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       25 2023-06-07 18:25:11.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/requires.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-06-07 18:25:11.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/top_level.txt
```

### Comparing `cfg-argparser-1.2.0/LICENSE` & `cfg-argparser-1.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.2.0/PKG-INFO` & `cfg-argparser-1.2.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.2.0
+Version: 1.2.0.post1
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: typer
 License-File: LICENSE
 
-# cfg_argparser 1.1.5
+# cfg_argparser 1.2.0
 
-a config wrapper I made to be easily applied to argparse objects.
+a config wrapper I made.
 
 ## Installation
 
 ```bash
 # from pypi:
 pip install cfg-argparser
```

### Comparing `cfg-argparser-1.2.0/README.md` & `cfg-argparser-1.2.0.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# cfg_argparser 1.1.5
+# cfg_argparser 1.2.0
 
-a config wrapper I made to be easily applied to argparse objects.
+a config wrapper I made.
 
 ## Installation
 
 ```bash
 # from pypi:
 pip install cfg-argparser
```

### Comparing `cfg-argparser-1.2.0/pyproject.toml` & `cfg-argparser-1.2.0.post1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "toml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfg-argparser"
-version = "1.2.0"
+version = "1.2.0-1"
 authors = [{ name = "Zeptofine", email = "zeptofine@gmail.com" }]
 description = "A package designed to simplify configurable defaults from argparse."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
@@ -16,14 +16,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = ["toml"]
 
 [project.urls]
 "Homepage" = "https://github.com/zeptofine/cfg-argparser"
 "Bug Tracker" = "https://github.com/zeptofine/cfg-argparser/issues"
 
+
 [project.optional-dependencies]
-typer=['typer[all]']
+typer = ['typer[all]']
```

### Comparing `cfg-argparser-1.2.0/src/cfg_argparser/argparse_config.py` & `cfg-argparser-1.2.0.post1/src/cfg_argparser/argparse_config.py`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.2.0/src/cfg_argparser/cfg_dict.py` & `cfg-argparser-1.2.0.post1/src/cfg_argparser/cfg_dict.py`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.2.0/src/cfg_argparser/function_config_wrapper.py` & `cfg-argparser-1.2.0.post1/src/cfg_argparser/function_config_wrapper.py`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.2.0/src/cfg_argparser/save_handlers.py` & `cfg-argparser-1.2.0.post1/src/cfg_argparser/save_handlers.py`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.2.0/src/cfg_argparser.egg-info/PKG-INFO` & `cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.2.0
+Version: 1.2.0.post1
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: typer
 License-File: LICENSE
 
-# cfg_argparser 1.1.5
+# cfg_argparser 1.2.0
 
-a config wrapper I made to be easily applied to argparse objects.
+a config wrapper I made.
 
 ## Installation
 
 ```bash
 # from pypi:
 pip install cfg-argparser
```

