# Comparing `tmp/pymultilint-1.0.4.tar.gz` & `tmp/pymultilint-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultilint-1.0.4.tar", max compression
+gzip compressed data, was "pymultilint-1.1.0.tar", max compression
```

## Comparing `pymultilint-1.0.4.tar` & `pymultilint-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-04-13 19:09:22.469416 pymultilint-1.0.4/LICENSE
--rw-r--r--   0        0        0     4518 2023-04-13 19:09:22.469416 pymultilint-1.0.4/README.md
--rwxr-xr-x   0        0        0    18125 2023-04-13 19:09:22.469416 pymultilint-1.0.4/multilint.py
--rw-r--r--   0        0        0     1281 2023-04-13 19:09:22.469416 pymultilint-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     5587 1970-01-01 00:00:00.000000 pymultilint-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-07 20:14:01.125575 pymultilint-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4518 2023-06-07 20:14:01.125575 pymultilint-1.1.0/README.md
+-rwxr-xr-x   0        0        0    18125 2023-06-07 20:14:01.125575 pymultilint-1.1.0/multilint.py
+-rw-r--r--   0        0        0     1281 2023-06-07 20:14:01.129576 pymultilint-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5587 1970-01-01 00:00:00.000000 pymultilint-1.1.0/PKG-INFO
```

### Comparing `pymultilint-1.0.4/LICENSE` & `pymultilint-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymultilint-1.0.4/README.md` & `pymultilint-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pymultilint-1.0.4/multilint.py` & `pymultilint-1.1.0/multilint.py`

 * *Files identical despite different names*

### Comparing `pymultilint-1.0.4/pyproject.toml` & `pymultilint-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pymultilint"
 packages = [{include = "multilint.py"}]
-version = "1.0.4"
+version = "1.1.0"
 description = "Utility tying multiple code quality tools together"
 authors = ["George Kontridze <george.kontridze@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/gkze/multilint"
 repository = "https://github.com/gkze/multilint"
 documentation = "https://gkze.github.io/multilint/multilint.html"
```

### Comparing `pymultilint-1.0.4/PKG-INFO` & `pymultilint-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultilint
-Version: 1.0.4
+Version: 1.1.0
 Summary: Utility tying multiple code quality tools together
 Home-page: https://github.com/gkze/multilint
 License: MIT
 Keywords: lint,code-quality,tools
 Author: George Kontridze
 Author-email: george.kontridze@gmail.com
 Requires-Python: >=3.8,<4.0
```

