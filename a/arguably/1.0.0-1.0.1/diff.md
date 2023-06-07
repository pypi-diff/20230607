# Comparing `tmp/arguably-1.0.0.tar.gz` & `tmp/arguably-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arguably-1.0.0.tar", max compression
+gzip compressed data, was "arguably-1.0.1.tar", max compression
```

## Comparing `arguably-1.0.0.tar` & `arguably-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1538 2023-06-07 13:34:46.505098 arguably-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     4616 2023-06-07 13:34:46.505098 arguably-1.0.0/README.md
--rw-r--r--   0        0        0    72211 2023-06-07 13:34:46.509098 arguably-1.0.0/arguably/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 13:34:46.509098 arguably-1.0.0/arguably/py.typed
--rw-r--r--   0        0        0      857 2023-06-07 13:34:46.509098 arguably-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5226 1970-01-01 00:00:00.000000 arguably-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-06-07 14:36:36.505951 arguably-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0    72211 2023-06-07 14:36:36.505951 arguably-1.0.1/arguably/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:36:36.505951 arguably-1.0.1/arguably/py.typed
+-rw-r--r--   0        0        0     4442 2023-06-07 14:36:36.505951 arguably-1.0.1/assets/PYPI_README.md
+-rw-r--r--   0        0        0      869 2023-06-07 14:36:36.505951 arguably-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5052 1970-01-01 00:00:00.000000 arguably-1.0.1/PKG-INFO
```

### Comparing `arguably-1.0.0/LICENSE.txt` & `arguably-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arguably-1.0.0/README.md` & `arguably-1.0.1/assets/PYPI_README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 <p align="center">
-    <picture>
-      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/treykeown/arguably/main/assets/arguably_white.png">
       <img alt="arguably logo" src="https://raw.githubusercontent.com/treykeown/arguably/main/assets/arguably_black.png">
-    </picture>
 </p>
 
 <p align="center">
     <em>
         turns functions into command line interfaces
     </em>
 </p>
```

### Comparing `arguably-1.0.0/arguably/__init__.py` & `arguably-1.0.1/arguably/__init__.py`

 * *Files identical despite different names*

### Comparing `arguably-1.0.0/pyproject.toml` & `arguably-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "arguably"
-version = "1.0.0"
+version = "1.0.1"
 description = "turns functions into command line interfaces"
 authors = ["treykeown <2755914+treykeown@users.noreply.github.com>"]
-readme = "README.md"
+readme = "assets/PYPI_README.md"
 homepage = "https://github.com/treykeown/arguably"
 repository = "https://github.com/treykeown/arguably"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docstring-parser = "^0.15"
```

### Comparing `arguably-1.0.0/PKG-INFO` & `arguably-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: arguably
-Version: 1.0.0
+Version: 1.0.1
 Summary: turns functions into command line interfaces
 Home-page: https://github.com/treykeown/arguably
 Author: treykeown
 Author-email: 2755914+treykeown@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Project-URL: Repository, https://github.com/treykeown/arguably
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <picture>
-      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/treykeown/arguably/main/assets/arguably_white.png">
       <img alt="arguably logo" src="https://raw.githubusercontent.com/treykeown/arguably/main/assets/arguably_black.png">
-    </picture>
 </p>
 
 <p align="center">
     <em>
         turns functions into command line interfaces
     </em>
 </p>
```

