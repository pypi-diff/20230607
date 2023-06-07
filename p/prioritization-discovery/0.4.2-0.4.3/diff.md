# Comparing `tmp/prioritization_discovery-0.4.2.tar.gz` & `tmp/prioritization_discovery-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prioritization_discovery-0.4.2.tar", max compression
+gzip compressed data, was "prioritization_discovery-0.4.3.tar", max compression
```

## Comparing `prioritization_discovery-0.4.2.tar` & `prioritization_discovery-0.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11349 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/LICENSE
--rw-r--r--   0        0        0     2040 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/README.md
--rw-r--r--   0        0        0      702 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/pyproject.toml
--rw-r--r--   0        0        0       43 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/src/prioritization_discovery/__init__.py
--rw-r--r--   0        0        0      883 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/src/prioritization_discovery/config.py
--rw-r--r--   0        0        0     4984 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/src/prioritization_discovery/discovery.py
--rw-r--r--   0        0        0    12584 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/src/prioritization_discovery/rules.py
--rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 prioritization_discovery-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2040 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/README.md
+-rw-r--r--   0        0        0      702 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/src/prioritization_discovery/__init__.py
+-rw-r--r--   0        0        0      883 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/src/prioritization_discovery/config.py
+-rw-r--r--   0        0        0     4984 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/src/prioritization_discovery/discovery.py
+-rw-r--r--   0        0        0    12584 2023-06-07 14:23:44.885117 prioritization_discovery-0.4.3/src/prioritization_discovery/rules.py
+-rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 prioritization_discovery-0.4.3/PKG-INFO
```

### Comparing `prioritization_discovery-0.4.2/LICENSE` & `prioritization_discovery-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prioritization_discovery-0.4.2/README.md` & `prioritization_discovery-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `prioritization_discovery-0.4.2/pyproject.toml` & `prioritization_discovery-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prioritization-discovery"
-version = "0.4.2"
+version = "0.4.3"
 description = "Python algorithm to discover, from an event log, prioritization rules that lead to one activity instance to be executed before another."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "prioritization_discovery", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `prioritization_discovery-0.4.2/src/prioritization_discovery/config.py` & `prioritization_discovery-0.4.3/src/prioritization_discovery/config.py`

 * *Files identical despite different names*

### Comparing `prioritization_discovery-0.4.2/src/prioritization_discovery/discovery.py` & `prioritization_discovery-0.4.3/src/prioritization_discovery/discovery.py`

 * *Files identical despite different names*

### Comparing `prioritization_discovery-0.4.2/src/prioritization_discovery/rules.py` & `prioritization_discovery-0.4.3/src/prioritization_discovery/rules.py`

 * *Files identical despite different names*

### Comparing `prioritization_discovery-0.4.2/PKG-INFO` & `prioritization_discovery-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prioritization-discovery
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python algorithm to discover, from an event log, prioritization rules that lead to one activity instance to be executed before another.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

