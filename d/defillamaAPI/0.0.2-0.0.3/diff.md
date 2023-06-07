# Comparing `tmp/defillamaAPI-0.0.2.tar.gz` & `tmp/defillamaAPI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defillamaAPI-0.0.2.tar", last modified: Wed Jun  7 13:38:31 2023, max compression
+gzip compressed data, was "defillamaAPI-0.0.3.tar", last modified: Wed Jun  7 13:55:41 2023, max compression
```

## Comparing `defillamaAPI-0.0.2.tar` & `defillamaAPI-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 13:38:31.285631 defillamaAPI-0.0.2/
--rw-rw-rw-   0        0        0     1212 2023-06-07 13:38:31.284647 defillamaAPI-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-06-07 13:18:47.000000 defillamaAPI-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 13:38:31.273479 defillamaAPI-0.0.2/defillamaAPI/
--rw-rw-rw-   0        0        0       36 2023-05-30 15:31:20.000000 defillamaAPI-0.0.2/defillamaAPI/__init__.py
--rw-rw-rw-   0        0        0      294 2023-06-07 13:38:17.000000 defillamaAPI-0.0.2/defillamaAPI/__version__.py
--rw-rw-rw-   0        0        0    20000 2023-06-07 13:18:31.000000 defillamaAPI-0.0.2/defillamaAPI/defillamaAPI.py
-drwxrwxrwx   0        0        0        0 2023-06-07 13:38:31.283633 defillamaAPI-0.0.2/defillamaAPI.egg-info/
--rw-rw-rw-   0        0        0     1212 2023-06-07 13:38:31.000000 defillamaAPI-0.0.2/defillamaAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-06-07 13:38:31.000000 defillamaAPI-0.0.2/defillamaAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 13:38:31.000000 defillamaAPI-0.0.2/defillamaAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-07 13:38:31.000000 defillamaAPI-0.0.2/defillamaAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-07 13:38:31.000000 defillamaAPI-0.0.2/defillamaAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      596 2023-06-07 13:38:07.000000 defillamaAPI-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 13:38:31.285631 defillamaAPI-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      944 2023-05-30 15:42:21.000000 defillamaAPI-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:55:41.146147 defillamaAPI-0.0.3/
+-rw-rw-rw-   0        0        0     1212 2023-06-07 13:55:41.145143 defillamaAPI-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2023-06-07 13:18:47.000000 defillamaAPI-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 13:55:41.134140 defillamaAPI-0.0.3/defillamaAPI/
+-rw-rw-rw-   0        0        0      103 2023-06-07 13:52:53.000000 defillamaAPI-0.0.3/defillamaAPI/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-06-07 13:54:56.000000 defillamaAPI-0.0.3/defillamaAPI/__version__.py
+-rw-rw-rw-   0        0        0    20000 2023-06-07 13:18:31.000000 defillamaAPI-0.0.3/defillamaAPI/defillamaAPI.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:55:41.143120 defillamaAPI-0.0.3/defillamaAPI.egg-info/
+-rw-rw-rw-   0        0        0     1212 2023-06-07 13:55:41.000000 defillamaAPI-0.0.3/defillamaAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-07 13:55:41.000000 defillamaAPI-0.0.3/defillamaAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 13:55:41.000000 defillamaAPI-0.0.3/defillamaAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-07 13:55:41.000000 defillamaAPI-0.0.3/defillamaAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-07 13:55:41.000000 defillamaAPI-0.0.3/defillamaAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      596 2023-06-07 13:55:12.000000 defillamaAPI-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 13:55:41.146147 defillamaAPI-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-05-30 15:42:21.000000 defillamaAPI-0.0.3/setup.py
```

### Comparing `defillamaAPI-0.0.2/PKG-INFO` & `defillamaAPI-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defillamaAPI
-Version: 0.0.2
+Version: 0.0.3
 Summary: defillama API Module
 Home-page: https://github.com/jafark92/defillamaAPI
 Author: Jafar Sadiq
 Author-email: Jafar Sadiq <jsadiqk92@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/jafark92/defillamaAPI
 Project-URL: Bug Tracker, https://github.com/jafark92/defillamaAPI/issues
```

### Comparing `defillamaAPI-0.0.2/README.md` & `defillamaAPI-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `defillamaAPI-0.0.2/defillamaAPI/defillamaAPI.py` & `defillamaAPI-0.0.3/defillamaAPI/defillamaAPI.py`

 * *Files identical despite different names*

### Comparing `defillamaAPI-0.0.2/defillamaAPI.egg-info/PKG-INFO` & `defillamaAPI-0.0.3/defillamaAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defillamaAPI
-Version: 0.0.2
+Version: 0.0.3
 Summary: defillama API Module
 Home-page: https://github.com/jafark92/defillamaAPI
 Author: Jafar Sadiq
 Author-email: Jafar Sadiq <jsadiqk92@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/jafark92/defillamaAPI
 Project-URL: Bug Tracker, https://github.com/jafark92/defillamaAPI/issues
```

### Comparing `defillamaAPI-0.0.2/pyproject.toml` & `defillamaAPI-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "defillamaAPI"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jafar Sadiq", email="jsadiqk92@gmail.com" },
 ]
 description = "defillama API Module"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `defillamaAPI-0.0.2/setup.py` & `defillamaAPI-0.0.3/setup.py`

 * *Files identical despite different names*

