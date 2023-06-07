# Comparing `tmp/datasette_sqlite_regex-0.2.3a5-py3-none-any.whl.zip` & `tmp/datasette_sqlite_regex-0.2.3a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2193 bytes, number of entries: 7
--rw-r--r--  2.0 unx      269 b- defN 23-Jun-07 17:45 datasette_sqlite_regex/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 17:45 datasette_sqlite_regex/version.py
--rw-r--r--  2.0 unx      569 b- defN 23-Jun-07 17:45 datasette_sqlite_regex-0.2.3a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 17:45 datasette_sqlite_regex-0.2.3a5.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jun-07 17:45 datasette_sqlite_regex-0.2.3a5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-07 17:45 datasette_sqlite_regex-0.2.3a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      655 b- defN 23-Jun-07 17:45 datasette_sqlite_regex-0.2.3a5.dist-info/RECORD
-7 files, 1737 bytes uncompressed, 999 bytes compressed:  42.5%
+Zip file size: 2192 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      269 b- defN 23-Jun-07 18:19 datasette_sqlite_regex/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 18:19 datasette_sqlite_regex/version.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Jun-07 18:20 datasette_sqlite_regex-0.2.3a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 18:20 datasette_sqlite_regex-0.2.3a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-07 18:20 datasette_sqlite_regex-0.2.3a6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-07 18:20 datasette_sqlite_regex-0.2.3a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jun-07 18:20 datasette_sqlite_regex-0.2.3a6.dist-info/RECORD
+7 files, 1737 bytes uncompressed, 998 bytes compressed:  42.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_regex/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_regex/version.py
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a5.dist-info/METADATA
+Filename: datasette_sqlite_regex-0.2.3a6.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a5.dist-info/WHEEL
+Filename: datasette_sqlite_regex-0.2.3a6.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a5.dist-info/entry_points.txt
+Filename: datasette_sqlite_regex-0.2.3a6.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a5.dist-info/top_level.txt
+Filename: datasette_sqlite_regex-0.2.3a6.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a5.dist-info/RECORD
+Filename: datasette_sqlite_regex-0.2.3a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_regex/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.3-alpha.5"
+__version__ = "0.2.3-alpha.6"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_regex-0.2.3a5.dist-info/RECORD` & `datasette_sqlite_regex-0.2.3a6.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_regex/__init__.py,sha256=gAZZGeI-BnNoB0cNpqhiiUcVh-BrAfdojdzff9v0B-o,269
-datasette_sqlite_regex/version.py,sha256=o6GdM3-8whcUNqnr6UQj86FWQQbmlnj0V8Xg5Cb8FSI,79
-datasette_sqlite_regex-0.2.3a5.dist-info/METADATA,sha256=B6xQq-Rl5Uovxy5B19cWZdR8XrDHi0h3YpHdQFRb4fM,569
-datasette_sqlite_regex-0.2.3a5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_regex-0.2.3a5.dist-info/entry_points.txt,sha256=Zk3m397tATyr9K3ZSBiMtwjGslB-xitDauEcT8TTE4k,50
-datasette_sqlite_regex-0.2.3a5.dist-info/top_level.txt,sha256=B9-o0e-bXWWM2wW4Z2fCLlpdh_xevETnuqjaWZ0a5qg,23
-datasette_sqlite_regex-0.2.3a5.dist-info/RECORD,,
+datasette_sqlite_regex/version.py,sha256=lJ1zT0l1sW8a6j7QSzGGs7rWHxwIQ2jpDfsHr9yJSAM,79
+datasette_sqlite_regex-0.2.3a6.dist-info/METADATA,sha256=F16HpjNqY3RItMkU4nR5cXiJvHWBSnkAe8YedbajC2I,569
+datasette_sqlite_regex-0.2.3a6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+datasette_sqlite_regex-0.2.3a6.dist-info/entry_points.txt,sha256=Zk3m397tATyr9K3ZSBiMtwjGslB-xitDauEcT8TTE4k,50
+datasette_sqlite_regex-0.2.3a6.dist-info/top_level.txt,sha256=B9-o0e-bXWWM2wW4Z2fCLlpdh_xevETnuqjaWZ0a5qg,23
+datasette_sqlite_regex-0.2.3a6.dist-info/RECORD,,
```

