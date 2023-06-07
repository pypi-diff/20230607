# Comparing `tmp/datasette_sqlite_regex-0.2.3a3-py3-none-any.whl.zip` & `tmp/datasette_sqlite_regex-0.2.3a5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2190 bytes, number of entries: 7
--rw-r--r--  2.0 unx      269 b- defN 23-Mar-23 17:34 datasette_sqlite_regex/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-23 17:34 datasette_sqlite_regex/version.py
--rw-r--r--  2.0 unx      569 b- defN 23-Mar-23 17:35 datasette_sqlite_regex-0.2.3a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-23 17:35 datasette_sqlite_regex-0.2.3a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Mar-23 17:35 datasette_sqlite_regex-0.2.3a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Mar-23 17:35 datasette_sqlite_regex-0.2.3a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      655 b- defN 23-Mar-23 17:35 datasette_sqlite_regex-0.2.3a3.dist-info/RECORD
-7 files, 1737 bytes uncompressed, 996 bytes compressed:  42.7%
+Zip file size: 2193 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      269 b- defN 23-Jun-07 17:45 datasette_sqlite_regex/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 17:45 datasette_sqlite_regex/version.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Jun-07 17:45 datasette_sqlite_regex-0.2.3a5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 17:45 datasette_sqlite_regex-0.2.3a5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-07 17:45 datasette_sqlite_regex-0.2.3a5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-07 17:45 datasette_sqlite_regex-0.2.3a5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jun-07 17:45 datasette_sqlite_regex-0.2.3a5.dist-info/RECORD
+7 files, 1737 bytes uncompressed, 999 bytes compressed:  42.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_regex/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_regex/version.py
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a3.dist-info/METADATA
+Filename: datasette_sqlite_regex-0.2.3a5.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a3.dist-info/WHEEL
+Filename: datasette_sqlite_regex-0.2.3a5.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a3.dist-info/entry_points.txt
+Filename: datasette_sqlite_regex-0.2.3a5.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a3.dist-info/top_level.txt
+Filename: datasette_sqlite_regex-0.2.3a5.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a3.dist-info/RECORD
+Filename: datasette_sqlite_regex-0.2.3a5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_regex/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.3-alpha.3"
+__version__ = "0.2.3-alpha.5"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_regex-0.2.3a3.dist-info/METADATA` & `datasette_sqlite_regex-0.2.3a5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-regex
-Version: 0.2.3a3
+Version: 0.2.3a5
 Home-page: https://github.com/asg017/sqlite-regex
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-regex/issues
 Project-URL: CI, https://github.com/asg017/sqlite-regex/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-regex/releases
 Requires-Python: >=3.7
```

