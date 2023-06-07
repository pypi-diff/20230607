# Comparing `tmp/datasette_sqlite_jsonschema-0.2.2a4-py3-none-any.whl.zip` & `tmp/datasette_sqlite_jsonschema-0.2.3a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2284 bytes, number of entries: 7
--rw-r--r--  2.0 unx      284 b- defN 23-Feb-23 01:30 datasette_sqlite_jsonschema/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Feb-23 01:30 datasette_sqlite_jsonschema/version.py
--rw-r--r--  2.0 unx      599 b- defN 23-Feb-23 01:30 datasette_sqlite_jsonschema-0.2.2a4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-23 01:30 datasette_sqlite_jsonschema-0.2.2a4.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-Feb-23 01:30 datasette_sqlite_jsonschema-0.2.2a4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 23-Feb-23 01:30 datasette_sqlite_jsonschema-0.2.2a4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      690 b- defN 23-Feb-23 01:30 datasette_sqlite_jsonschema-0.2.2a4.dist-info/RECORD
-7 files, 1832 bytes uncompressed, 1020 bytes compressed:  44.3%
+Zip file size: 2283 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      284 b- defN 23-Jun-07 17:45 datasette_sqlite_jsonschema/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 17:45 datasette_sqlite_jsonschema/version.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Jun-07 17:45 datasette_sqlite_jsonschema-0.2.3a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 17:45 datasette_sqlite_jsonschema-0.2.3a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-07 17:45 datasette_sqlite_jsonschema-0.2.3a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-07 17:45 datasette_sqlite_jsonschema-0.2.3a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      690 b- defN 23-Jun-07 17:45 datasette_sqlite_jsonschema-0.2.3a2.dist-info/RECORD
+7 files, 1832 bytes uncompressed, 1019 bytes compressed:  44.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_jsonschema/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_jsonschema/version.py
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.2a4.dist-info/METADATA
+Filename: datasette_sqlite_jsonschema-0.2.3a2.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.2a4.dist-info/WHEEL
+Filename: datasette_sqlite_jsonschema-0.2.3a2.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.2a4.dist-info/entry_points.txt
+Filename: datasette_sqlite_jsonschema-0.2.3a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.2a4.dist-info/top_level.txt
+Filename: datasette_sqlite_jsonschema-0.2.3a2.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.2a4.dist-info/RECORD
+Filename: datasette_sqlite_jsonschema-0.2.3a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_jsonschema/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.2-alpha.4"
+__version__ = "0.2.3-alpha.2"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_jsonschema-0.2.2a4.dist-info/METADATA` & `datasette_sqlite_jsonschema-0.2.3a2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-jsonschema
-Version: 0.2.2a4
+Version: 0.2.3a2
 Home-page: https://github.com/asg017/sqlite-jsonschema
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-jsonschema/issues
 Project-URL: CI, https://github.com/asg017/sqlite-jsonschema/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-jsonschema/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_jsonschema-0.2.2a4.dist-info/RECORD` & `datasette_sqlite_jsonschema-0.2.3a2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_jsonschema/__init__.py,sha256=CkEgCNG1ogAHTmP5eAR4aQ3TdxqqmgBIs9kLzsEp29U,284
-datasette_sqlite_jsonschema/version.py,sha256=ZR7p8L1sdx-uepiKJp6WCkcT4-VNE82_12TAWOqhqqQ,79
-datasette_sqlite_jsonschema-0.2.2a4.dist-info/METADATA,sha256=89aOZNY7gHOl_6n4HJqfkdbbzE2aNvPPSAXrGNANeYA,599
-datasette_sqlite_jsonschema-0.2.2a4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-datasette_sqlite_jsonschema-0.2.2a4.dist-info/entry_points.txt,sha256=GudkqSm13Ou5ZqFjwDzCYFo5oo9FSVgstqZWdGYOGTo,60
-datasette_sqlite_jsonschema-0.2.2a4.dist-info/top_level.txt,sha256=gGoRXv89K-JydhKqkfeF25P05Er5OkO8wqnHPcKfim0,28
-datasette_sqlite_jsonschema-0.2.2a4.dist-info/RECORD,,
+datasette_sqlite_jsonschema/version.py,sha256=CiLr9a3lNs_Q4jcYe5bYLUkmRoSwjm3Eh7gyiqKDwGU,79
+datasette_sqlite_jsonschema-0.2.3a2.dist-info/METADATA,sha256=0XjKsPuWI8ArSmDRLVoWQvAS8eLg8_hVK-H7SWANarc,599
+datasette_sqlite_jsonschema-0.2.3a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+datasette_sqlite_jsonschema-0.2.3a2.dist-info/entry_points.txt,sha256=GudkqSm13Ou5ZqFjwDzCYFo5oo9FSVgstqZWdGYOGTo,60
+datasette_sqlite_jsonschema-0.2.3a2.dist-info/top_level.txt,sha256=gGoRXv89K-JydhKqkfeF25P05Er5OkO8wqnHPcKfim0,28
+datasette_sqlite_jsonschema-0.2.3a2.dist-info/RECORD,,
```

