# Comparing `tmp/datasette_sqlite_http-0.1.0a2-py3-none-any.whl.zip` & `tmp/datasette_sqlite_http-0.1.0a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2275 bytes, number of entries: 7
--rw-r--r--  2.0 unx      511 b- defN 23-Mar-28 04:23 datasette_sqlite_http/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-28 04:23 datasette_sqlite_http/version.py
--rw-r--r--  2.0 unx      563 b- defN 23-Mar-28 04:23 datasette_sqlite_http-0.1.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 04:23 datasette_sqlite_http-0.1.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Mar-28 04:23 datasette_sqlite_http-0.1.0a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Mar-28 04:23 datasette_sqlite_http-0.1.0a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      648 b- defN 23-Mar-28 04:23 datasette_sqlite_http-0.1.0a2.dist-info/RECORD
-7 files, 1963 bytes uncompressed, 1095 bytes compressed:  44.2%
+Zip file size: 2276 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      511 b- defN 23-Jun-06 23:22 datasette_sqlite_http/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-06 23:22 datasette_sqlite_http/version.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Jun-06 23:22 datasette_sqlite_http-0.1.0a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 23:22 datasette_sqlite_http-0.1.0a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-06 23:22 datasette_sqlite_http-0.1.0a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-06 23:22 datasette_sqlite_http-0.1.0a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      648 b- defN 23-Jun-06 23:22 datasette_sqlite_http-0.1.0a3.dist-info/RECORD
+7 files, 1963 bytes uncompressed, 1096 bytes compressed:  44.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_http/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_http/version.py
 Comment: 
 
-Filename: datasette_sqlite_http-0.1.0a2.dist-info/METADATA
+Filename: datasette_sqlite_http-0.1.0a3.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_http-0.1.0a2.dist-info/WHEEL
+Filename: datasette_sqlite_http-0.1.0a3.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_http-0.1.0a2.dist-info/entry_points.txt
+Filename: datasette_sqlite_http-0.1.0a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_http-0.1.0a2.dist-info/top_level.txt
+Filename: datasette_sqlite_http-0.1.0a3.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_http-0.1.0a2.dist-info/RECORD
+Filename: datasette_sqlite_http-0.1.0a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_http/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.2"
+__version__ = "0.1.0-alpha.3"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_http-0.1.0a2.dist-info/METADATA` & `datasette_sqlite_http-0.1.0a3.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-http
-Version: 0.1.0a2
+Version: 0.1.0a3
 Home-page: https://github.com/asg017/sqlite-http
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-http/issues
 Project-URL: CI, https://github.com/asg017/sqlite-http/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-http/releases
 Requires-Python: >=3.7
```

