# Comparing `tmp/sqlsprinkler_python_GT3CH1-0.0.8-py3-none-any.whl.zip` & `tmp/sqlsprinkler_python_GT3CH1-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5747 bytes, number of entries: 9
+Zip file size: 5751 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      107 b- defN 23-May-03 22:05 sqlsprinkler/__init__.py
 -rw-r--r--  2.0 unx      222 b- defN 23-May-03 22:30 sqlsprinkler/api.py
--rw-r--r--  2.0 unx     7383 b- defN 23-Jun-07 00:17 sqlsprinkler/system.py
+-rw-r--r--  2.0 unx     7386 b- defN 23-Jun-07 00:24 sqlsprinkler/system.py
 -rw-r--r--  2.0 unx     4361 b- defN 23-Jun-07 00:20 sqlsprinkler/zone.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-07 00:21 sqlsprinkler_python_GT3CH1-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      830 b- defN 23-Jun-07 00:21 sqlsprinkler_python_GT3CH1-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 00:21 sqlsprinkler_python_GT3CH1-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-07 00:21 sqlsprinkler_python_GT3CH1-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      791 b- defN 23-Jun-07 00:21 sqlsprinkler_python_GT3CH1-0.0.8.dist-info/RECORD
-9 files, 14867 bytes uncompressed, 4363 bytes compressed:  70.7%
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-07 00:25 sqlsprinkler_python_GT3CH1-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      830 b- defN 23-Jun-07 00:25 sqlsprinkler_python_GT3CH1-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 00:25 sqlsprinkler_python_GT3CH1-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-07 00:25 sqlsprinkler_python_GT3CH1-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      791 b- defN 23-Jun-07 00:25 sqlsprinkler_python_GT3CH1-0.0.9.dist-info/RECORD
+9 files, 14870 bytes uncompressed, 4367 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: sqlsprinkler/system.py
 Comment: 
 
 Filename: sqlsprinkler/zone.py
 Comment: 
 
-Filename: sqlsprinkler_python_GT3CH1-0.0.8.dist-info/LICENSE
+Filename: sqlsprinkler_python_GT3CH1-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: sqlsprinkler_python_GT3CH1-0.0.8.dist-info/METADATA
+Filename: sqlsprinkler_python_GT3CH1-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: sqlsprinkler_python_GT3CH1-0.0.8.dist-info/WHEEL
+Filename: sqlsprinkler_python_GT3CH1-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: sqlsprinkler_python_GT3CH1-0.0.8.dist-info/top_level.txt
+Filename: sqlsprinkler_python_GT3CH1-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlsprinkler_python_GT3CH1-0.0.8.dist-info/RECORD
+Filename: sqlsprinkler_python_GT3CH1-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlsprinkler/system.py

```diff
@@ -102,18 +102,18 @@
 
     def turn_on(self):
         self.set_system_state(True)
 
     def turn_off(self):
         self.set_system_state(False)
 
-    async def async_turn_on(self)
+    async def async_turn_on(self):
         self.async_set_system_state(True)
 
-    async def async_turn_on(self)
+    async def async_turn_off(self):
         self.async_set_system_state(False)
 
     def set_system_state(self, state: bool) -> None:
         """
         Sets the system state.
         :param state: The state to set.
         :return: None
```

## Comparing `sqlsprinkler_python_GT3CH1-0.0.8.dist-info/LICENSE` & `sqlsprinkler_python_GT3CH1-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sqlsprinkler_python_GT3CH1-0.0.8.dist-info/METADATA` & `sqlsprinkler_python_GT3CH1-0.0.9.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsprinkler-python-GT3CH1
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python library to control a SQLSprinkler system
 Home-page: https://github.com/GT3CH1/sqlsprinkler_python
 Author: Gavin Pease
 Author-email: gavinpease@gmail.com
 Project-URL: Bug Tracker, https://github.com/GT3CH1/sqlsprinkler_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

