# Comparing `tmp/ezkl-0.0.3.tar.gz` & `tmp/ezkl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezkl-0.0.3.tar", max compression
+gzip compressed data, was "ezkl-0.0.4.tar", max compression
```

## Comparing `ezkl-0.0.3.tar` & `ezkl-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-07 12:54:22.645108 ezkl-0.0.3/LICENSE
--rw-r--r--   0        0        0     2307 2023-06-07 12:54:22.645108 ezkl-0.0.3/README.md
--rw-r--r--   0        0        0      272 2023-06-07 12:54:22.645108 ezkl-0.0.3/ezkl/__init__.py
--rw-r--r--   0        0        0     3232 2023-06-07 12:54:22.645108 ezkl-0.0.3/ezkl/export.py
--rw-r--r--   0        0        0      879 2023-06-07 12:54:22.645108 ezkl-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 ezkl-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-07 15:16:07.799754 ezkl-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2307 2023-06-07 15:16:07.799754 ezkl-0.0.4/README.md
+-rw-r--r--   0        0        0      273 2023-06-07 15:16:07.799754 ezkl-0.0.4/ezkl/__init__.py
+-rw-r--r--   0        0        0     3232 2023-06-07 15:16:07.799754 ezkl-0.0.4/ezkl/export.py
+-rw-r--r--   0        0        0      879 2023-06-07 15:16:20.439833 ezkl-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 ezkl-0.0.4/PKG-INFO
```

### Comparing `ezkl-0.0.3/LICENSE` & `ezkl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ezkl-0.0.3/README.md` & `ezkl-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ezkl-0.0.3/ezkl/export.py` & `ezkl-0.0.4/ezkl/export.py`

 * *Files identical despite different names*

### Comparing `ezkl-0.0.3/pyproject.toml` & `ezkl-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ezkl"
-version = "0.0.3"
+version = "0.0.4"
 description = "Easy zero-knowledge learning in Python"
 authors = [
   "Jason Morton <jason@zkonduit.com>",
   "Dante Camuto <jason@zkonduit.com>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `ezkl-0.0.3/PKG-INFO` & `ezkl-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezkl
-Version: 0.0.3
+Version: 0.0.4
 Summary: Easy zero-knowledge learning in Python
 Home-page: https://github.com/zkonduit/pyezkl
 License: Apache-2.0
 Author: Jason Morton
 Author-email: jason@zkonduit.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
```

