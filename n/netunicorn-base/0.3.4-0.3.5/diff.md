# Comparing `tmp/netunicorn-base-0.3.4.tar.gz` & `tmp/netunicorn-base-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-base-0.3.4.tar", last modified: Wed Jun  7 00:22:59 2023, max compression
+gzip compressed data, was "netunicorn-base-0.3.5.tar", last modified: Wed Jun  7 02:22:58 2023, max compression
```

## Comparing `netunicorn-base-0.3.4.tar` & `netunicorn-base-0.3.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.607789 netunicorn-base-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-07 00:22:59.603789 netunicorn-base-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 00:22:59.607789 netunicorn-base-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.599789 netunicorn-base-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.599789 netunicorn-base-0.3.4/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.599789 netunicorn-base-0.3.4/src/netunicorn/base/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/environment_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.595789 netunicorn-base-0.3.4/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.603789 netunicorn-base-0.3.4/src/netunicorn/director/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.603789 netunicorn-base-0.3.4/src/netunicorn/director/base/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/connectors/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/connectors/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.603789 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-07 00:22:59.000000 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-07 00:22:59.000000 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:22:59.000000 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 00:22:59.000000 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 00:22:59.000000 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:22:58.275951 netunicorn-base-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-07 02:22:58.275951 netunicorn-base-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 02:22:58.275951 netunicorn-base-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:22:58.271951 netunicorn-base-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:22:58.275951 netunicorn-base-0.3.5/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:22:58.275951 netunicorn-base-0.3.5/src/netunicorn/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/base/architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/base/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/base/environment_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/base/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/base/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/base/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:22:58.271951 netunicorn-base-0.3.5/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:22:58.275951 netunicorn-base-0.3.5/src/netunicorn/director/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/director/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:22:58.275951 netunicorn-base-0.3.5/src/netunicorn/director/base/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/director/base/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/director/base/connectors/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/director/base/connectors/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/director/base/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/director/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/director/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:22:46.000000 netunicorn-base-0.3.5/src/netunicorn/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:22:58.275951 netunicorn-base-0.3.5/src/netunicorn_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-07 02:22:58.000000 netunicorn-base-0.3.5/src/netunicorn_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-07 02:22:58.000000 netunicorn-base-0.3.5/src/netunicorn_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:22:58.000000 netunicorn-base-0.3.5/src/netunicorn_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 02:22:58.000000 netunicorn-base-0.3.5/src/netunicorn_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 02:22:58.000000 netunicorn-base-0.3.5/src/netunicorn_base.egg-info/top_level.txt
```

### Comparing `netunicorn-base-0.3.4/pyproject.toml` & `netunicorn-base-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-base"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn base module"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-base-0.3.4/src/netunicorn/base/__init__.py` & `netunicorn-base-0.3.5/src/netunicorn/base/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.4/src/netunicorn/base/deployment.py` & `netunicorn-base-0.3.5/src/netunicorn/base/deployment.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.4/src/netunicorn/base/environment_definitions.py` & `netunicorn-base-0.3.5/src/netunicorn/base/environment_definitions.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.4/src/netunicorn/base/experiment.py` & `netunicorn-base-0.3.5/src/netunicorn/base/experiment.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.4/src/netunicorn/base/nodes.py` & `netunicorn-base-0.3.5/src/netunicorn/base/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,14 +367,17 @@
         return str(
             f"<Uncountable node pool with next node template: {self._node_template}>"
         )
 
     def __repr__(self) -> str:
         return str(self)
 
+    def __iter__(self) -> Iterator[Node]:
+        return self
+
     def __next__(self) -> Node:
         """
         Generate and returns the next node in the pool.
 
         :return: next node
         """
         node = deepcopy(next(self._nodes))
```

### Comparing `netunicorn-base-0.3.4/src/netunicorn/base/pipeline.py` & `netunicorn-base-0.3.5/src/netunicorn/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.4/src/netunicorn/base/task.py` & `netunicorn-base-0.3.5/src/netunicorn/base/task.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.4/src/netunicorn/base/types.py` & `netunicorn-base-0.3.5/src/netunicorn/base/types.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.4/src/netunicorn/base/utils.py` & `netunicorn-base-0.3.5/src/netunicorn/base/utils.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.4/src/netunicorn/director/base/connectors/protocol.py` & `netunicorn-base-0.3.5/src/netunicorn/director/base/connectors/protocol.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.4/src/netunicorn/director/base/resources.py` & `netunicorn-base-0.3.5/src/netunicorn/director/base/resources.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.4/src/netunicorn_base.egg-info/SOURCES.txt` & `netunicorn-base-0.3.5/src/netunicorn_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

