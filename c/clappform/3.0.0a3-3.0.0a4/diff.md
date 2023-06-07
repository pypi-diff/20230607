# Comparing `tmp/clappform-3.0.0a3.tar.gz` & `tmp/clappform-3.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clappform-3.0.0a3.tar", last modified: Wed Jun  7 13:45:35 2023, max compression
+gzip compressed data, was "clappform-3.0.0a4.tar", last modified: Wed Jun  7 14:13:50 2023, max compression
```

## Comparing `clappform-3.0.0a3.tar` & `clappform-3.0.0a4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:45:35.886432 clappform-3.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 13:45:21.000000 clappform-3.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-07 13:45:35.886432 clappform-3.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 13:45:21.000000 clappform-3.0.0a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-07 13:45:21.000000 clappform-3.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:45:35.886432 clappform-3.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:45:35.886432 clappform-3.0.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:45:35.886432 clappform-3.0.0a3/src/clappform/
--rw-r--r--   0 runner    (1001) docker     (123)    24500 2023-06-07 13:45:21.000000 clappform-3.0.0a3/src/clappform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-06-07 13:45:21.000000 clappform-3.0.0a3/src/clappform/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-07 13:45:21.000000 clappform-3.0.0a3/src/clappform/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:45:35.886432 clappform-3.0.0a3/src/clappform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-07 13:45:35.000000 clappform-3.0.0a3/src/clappform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-07 13:45:35.000000 clappform-3.0.0a3/src/clappform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:45:35.000000 clappform-3.0.0a3/src/clappform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 13:45:35.000000 clappform-3.0.0a3/src/clappform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 13:45:35.000000 clappform-3.0.0a3/src/clappform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 13:45:21.000000 clappform-3.0.0a3/src/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:13:50.693729 clappform-3.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 14:13:39.000000 clappform-3.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-07 14:13:50.693729 clappform-3.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 14:13:39.000000 clappform-3.0.0a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-07 14:13:39.000000 clappform-3.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:13:50.693729 clappform-3.0.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:13:50.693729 clappform-3.0.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:13:50.693729 clappform-3.0.0a4/src/clappform/
+-rw-r--r--   0 runner    (1001) docker     (123)    24656 2023-06-07 14:13:39.000000 clappform-3.0.0a4/src/clappform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-06-07 14:13:39.000000 clappform-3.0.0a4/src/clappform/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-07 14:13:39.000000 clappform-3.0.0a4/src/clappform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:13:50.693729 clappform-3.0.0a4/src/clappform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-07 14:13:50.000000 clappform-3.0.0a4/src/clappform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-07 14:13:50.000000 clappform-3.0.0a4/src/clappform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:13:50.000000 clappform-3.0.0a4/src/clappform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 14:13:50.000000 clappform-3.0.0a4/src/clappform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 14:13:50.000000 clappform-3.0.0a4/src/clappform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 14:13:39.000000 clappform-3.0.0a4/src/debug.py
```

### Comparing `clappform-3.0.0a3/LICENSE` & `clappform-3.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a3/PKG-INFO` & `clappform-3.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clappform-3.0.0a3/README.md` & `clappform-3.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a3/pyproject.toml` & `clappform-3.0.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clappform"
-version = "3.0.0-alpha.3"
+version = "3.0.0-alpha.4"
 authors= [
     { name="Clappform B.V.", email="info@clappform.com" },
 ]
 description = "Clappform Python API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `clappform-3.0.0a3/src/clappform/__init__.py` & `clappform-3.0.0a4/src/clappform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     HTTPError,
     PaginationTotalError,
     PaginationKeyError,
 )
 
 
 # Metadata
-__version__ = "3.0.0-alpha.3"
+__version__ = "3.0.0-alpha.4"
 __author__ = "Clappform B.V."
 __email__ = "info@clappform.com"
 __license__ = "MIT"
 __doc__ = "Clappform Python API wrapper"
 
 
 class Clappform:
@@ -433,23 +433,26 @@
         :param interval_timeout: Optional time to sleep per request, defaults to:
             ``0.0``.
         :type interval_timeout: int
 
         Usage::
 
             >>> from clappform import Clappform
+            >>> import clappform.dataclasses as r
+            >>> import pandas as pd
             >>> c = Clappform(
             ...     "https://app.clappform.com",
             ...     "j.doe@clappform.com",
             ...     "S3cr3tP4ssw0rd!"
             ... )
-            >>> query = c.get_query("foo")
-            >>> it = c.read_dataframe(query)
-            >>> for i in it:
-            ...     print(i)
+            >>> query = c.get(r.Query(slug="foo")
+            >>> list_df = []
+            >>> for df in c.read_dataframe(query):
+            ...     list_df.append(df)
+            >>> master_df = pd.concat(list_df)
 
         :returns: Generator to read dataframe
         :rtype: :class:`generator`
         """
         path = "/dataframe/read_data"
         params = {
             "method": "POST",
```

### Comparing `clappform-3.0.0a3/src/clappform/dataclasses.py` & `clappform-3.0.0a4/src/clappform/dataclasses.py`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a3/src/clappform/exceptions.py` & `clappform-3.0.0a4/src/clappform/exceptions.py`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a3/src/clappform.egg-info/PKG-INFO` & `clappform-3.0.0a4/src/clappform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

