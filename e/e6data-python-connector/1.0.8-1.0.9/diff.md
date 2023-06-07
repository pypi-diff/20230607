# Comparing `tmp/e6data-python-connector-1.0.8.tar.gz` & `tmp/e6data-python-connector-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e6data-python-connector-1.0.8.tar", last modified: Sat Jun  3 06:39:52 2023, max compression
+gzip compressed data, was "e6data-python-connector-1.0.9.tar", last modified: Wed Jun  7 06:14:32 2023, max compression
```

## Comparing `e6data-python-connector-1.0.8.tar` & `e6data-python-connector-1.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-03 06:39:52.539787 e6data-python-connector-1.0.8/
--rw-r--r--   0 vishalanand   (501) staff       (20)    11357 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/LICENSE
--rw-r--r--   0 vishalanand   (501) staff       (20)       55 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/MANIFEST.in
--rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-06-03 06:39:52.540313 e6data-python-connector-1.0.8/PKG-INFO
--rw-r--r--   0 vishalanand   (501) staff       (20)     5189 2023-06-03 05:39:57.000000 e6data-python-connector-1.0.8/README.md
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-03 06:39:52.419907 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/
--rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 vishalanand   (501) staff       (20)      632 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)        1 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       63 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/entry_points.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       66 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/requires.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)        6 2023-06-03 06:39:52.000000 e6data-python-connector-1.0.8/e6data_python_connector.egg-info/top_level.txt
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-03 06:39:52.519562 e6data-python-connector-1.0.8/e6xdb/
--rw-r--r--   0 vishalanand   (501) staff       (20)      334 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/__init__.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     9958 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/common.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      682 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/constants.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     6052 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/datainputstream.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    13623 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/date_time_utils.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    17377 2023-06-03 05:40:26.000000 e6data-python-connector-1.0.8/e6xdb/e6x.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      382 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/exceptions.py
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-03 06:39:52.538623 e6data-python-connector-1.0.8/e6xdb/server/
--rw-r--r--   0 vishalanand   (501) staff       (20)   206971 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.8/e6xdb/server/QueryEngineService.py
--rw-r--r--   0 vishalanand   (501) staff       (20)       56 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/server/__init__.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/server/constants.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    21227 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.8/e6xdb/server/ttypes.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    11833 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/sqlalchemy_e6x.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     1777 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/e6xdb/typeId.py
--rw-r--r--   0 vishalanand   (501) staff       (20)       64 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.8/pyproject.toml
--rw-r--r--   0 vishalanand   (501) staff       (20)       73 2023-06-03 06:39:52.544712 e6data-python-connector-1.0.8/setup.cfg
--rw-r--r--   0 vishalanand   (501) staff       (20)     1925 2023-06-03 05:39:57.000000 e6data-python-connector-1.0.8/setup.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-07 06:14:32.505863 e6data-python-connector-1.0.9/
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11357 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/LICENSE
+-rw-r--r--   0 vishalanand   (501) staff       (20)       55 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/MANIFEST.in
+-rw-r--r--   0 vishalanand   (501) staff       (20)     7548 2023-06-07 06:14:32.506001 e6data-python-connector-1.0.9/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)     5380 2023-06-07 06:14:30.000000 e6data-python-connector-1.0.9/README.md
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-07 06:14:32.485676 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/
+-rw-r--r--   0 vishalanand   (501) staff       (20)     7548 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)      632 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)        1 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       63 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/entry_points.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       66 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/requires.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)        6 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/top_level.txt
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-07 06:14:32.499096 e6data-python-connector-1.0.9/e6xdb/
+-rw-r--r--   0 vishalanand   (501) staff       (20)      334 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     9958 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/common.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      682 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     6052 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/datainputstream.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    13623 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/date_time_utils.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    17760 2023-06-06 12:43:44.000000 e6data-python-connector-1.0.9/e6xdb/e6x.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      382 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/exceptions.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-07 06:14:32.504535 e6data-python-connector-1.0.9/e6xdb/server/
+-rw-r--r--   0 vishalanand   (501) staff       (20)   206971 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.9/e6xdb/server/QueryEngineService.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)       56 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/server/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/server/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    21227 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.9/e6xdb/server/ttypes.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11833 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/sqlalchemy_e6x.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1777 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/typeId.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)       64 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/pyproject.toml
+-rw-r--r--   0 vishalanand   (501) staff       (20)       73 2023-06-07 06:14:32.508451 e6data-python-connector-1.0.9/setup.cfg
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1925 2023-06-07 06:14:30.000000 e6data-python-connector-1.0.9/setup.py
```

### Comparing `e6data-python-connector-1.0.8/LICENSE` & `e6data-python-connector-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.8/PKG-INFO` & `e6data-python-connector-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: e6data-python-connector
-Version: 1.0.8
+Version: 1.0.9
 Summary: Client for the e6data distributed SQL Engine.
 Home-page: https://github.com/e6x-labs/e6data-python-connector
 Author: Uniphi, Inc.
 Author-email: info@e6data.com
 License: Apache 2.0
 Description: # e6data Python Connector
         
-        ![version](https://img.shields.io/badge/version-1.0.8-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.0.9-blue.svg)
         
         ## Introduction
         
         The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
         
         To install the Python package, use the command below:
         ```shell
@@ -72,14 +72,21 @@
         
         To fetch limited records:
         ```python
         limit = 500
         records = cursor.fetchmany(limit)
         ```
         
+        To fetch all the records in buffer to reduce memory consumption:
+        ```python
+        records_iterator = cursor.fetchall_buffer()  # Returns generator
+        for item in records_iterator:
+            print(item)
+        ```
+        
         To get the execution plan after query execution:
         ```python
         import json
         
         query_planner = json.loads(cursor.explain_analyse())
         ```
```

### Comparing `e6data-python-connector-1.0.8/README.md` & `e6data-python-connector-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # e6data Python Connector
 
-![version](https://img.shields.io/badge/version-1.0.8-blue.svg)
+![version](https://img.shields.io/badge/version-1.0.9-blue.svg)
 
 ## Introduction
 
 The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
 
 To install the Python package, use the command below:
 ```shell
@@ -64,14 +64,21 @@
 
 To fetch limited records:
 ```python
 limit = 500
 records = cursor.fetchmany(limit)
 ```
 
+To fetch all the records in buffer to reduce memory consumption:
+```python
+records_iterator = cursor.fetchall_buffer()  # Returns generator
+for item in records_iterator:
+    print(item)
+```
+
 To get the execution plan after query execution:
 ```python
 import json
 
 query_planner = json.loads(cursor.explain_analyse())
 ```
```

### Comparing `e6data-python-connector-1.0.8/e6data_python_connector.egg-info/PKG-INFO` & `e6data-python-connector-1.0.9/e6data_python_connector.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: e6data-python-connector
-Version: 1.0.8
+Version: 1.0.9
 Summary: Client for the e6data distributed SQL Engine.
 Home-page: https://github.com/e6x-labs/e6data-python-connector
 Author: Uniphi, Inc.
 Author-email: info@e6data.com
 License: Apache 2.0
 Description: # e6data Python Connector
         
-        ![version](https://img.shields.io/badge/version-1.0.8-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.0.9-blue.svg)
         
         ## Introduction
         
         The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
         
         To install the Python package, use the command below:
         ```shell
@@ -72,14 +72,21 @@
         
         To fetch limited records:
         ```python
         limit = 500
         records = cursor.fetchmany(limit)
         ```
         
+        To fetch all the records in buffer to reduce memory consumption:
+        ```python
+        records_iterator = cursor.fetchall_buffer()  # Returns generator
+        for item in records_iterator:
+            print(item)
+        ```
+        
         To get the execution plan after query execution:
         ```python
         import json
         
         query_planner = json.loads(cursor.explain_analyse())
         ```
```

### Comparing `e6data-python-connector-1.0.8/e6data_python_connector.egg-info/SOURCES.txt` & `e6data-python-connector-1.0.9/e6data_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.8/e6xdb/common.py` & `e6data-python-connector-1.0.9/e6xdb/common.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.8/e6xdb/constants.py` & `e6data-python-connector-1.0.9/e6xdb/constants.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.8/e6xdb/datainputstream.py` & `e6data-python-connector-1.0.9/e6xdb/datainputstream.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.8/e6xdb/date_time_utils.py` & `e6data-python-connector-1.0.9/e6xdb/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.8/e6xdb/e6x.py` & `e6data-python-connector-1.0.9/e6xdb/e6x.py`

 * *Files 2% similar despite different names*

```diff
@@ -421,33 +421,46 @@
             if rows is None:
                 break
             self._data = self._data + rows
         rows = self._data
         self._data = None
         return rows
 
+    def fetchall_buffer(self, query_id=None):
+        if query_id:
+            self._query_id = query_id
+        while True:
+            rows = self.fetch_batch()
+            if not rows:
+                return
+            yield rows
+
     def fetch_batch(self):
         # _logger.debug("fetching next batch from e6data")
         client = self.connection.client
         buffer = client.getNextResultBatch(self.connection.get_session_id, self._query_id)
         if not self._is_metadata_updated:
             self.update_mete_data()
             self._is_metadata_updated = True
         if not buffer:
             return None
         buffer = BytesIO(buffer)
         dis = DataInputStream(buffer)
         # one batch retrieves the predefined set of rows
         return read_rows_from_batch(self._query_columns_description, dis)
 
-    def fetchall(self):
+    def fetchall(self, query_id=None):
+        if query_id:
+            self._query_id = query_id
         return self._fetch_all()
 
-    def fetchmany(self, size=None):
+    def fetchmany(self, size=None, query_id=None):
         # _logger.info("fetching all from overriden method")
+        if query_id:
+            self._query_id = query_id
         if size is None:
             size = self.arraysize
         if self._data is None:
             self._data = list()
         while len(self._data) < size:
             # _logger.info("fetching next batch from fetch many")
             rows = self.fetch_batch()
```

### Comparing `e6data-python-connector-1.0.8/e6xdb/server/QueryEngineService.py` & `e6data-python-connector-1.0.9/e6xdb/server/QueryEngineService.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.8/e6xdb/server/ttypes.py` & `e6data-python-connector-1.0.9/e6xdb/server/ttypes.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.8/e6xdb/sqlalchemy_e6x.py` & `e6data-python-connector-1.0.9/e6xdb/sqlalchemy_e6x.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.8/e6xdb/typeId.py` & `e6data-python-connector-1.0.9/e6xdb/typeId.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.8/setup.py` & `e6data-python-connector-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import os
 
 import setuptools
 
 envstring = lambda var: os.environ.get(var) or ""
 
-VERSION = [1, 0, 8]
+VERSION = [1, 0, 9]
 
 
 def get_long_desc():
     with open("README.md", "r") as fh:
         long_description = fh.read()
     return long_description
```

