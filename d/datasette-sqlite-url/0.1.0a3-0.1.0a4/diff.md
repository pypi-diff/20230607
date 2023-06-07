# Comparing `tmp/datasette_sqlite_url-0.1.0a3-py3-none-any.whl.zip` & `tmp/datasette_sqlite_url-0.1.0a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2149 bytes, number of entries: 7
--rw-r--r--  2.0 unx      263 b- defN 23-Mar-28 01:25 datasette_sqlite_url/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-28 01:25 datasette_sqlite_url/version.py
--rw-r--r--  2.0 unx      557 b- defN 23-Mar-28 01:25 datasette_sqlite_url-0.1.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 01:25 datasette_sqlite_url-0.1.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Mar-28 01:25 datasette_sqlite_url-0.1.0a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Mar-28 01:25 datasette_sqlite_url-0.1.0a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      641 b- defN 23-Mar-28 01:25 datasette_sqlite_url-0.1.0a3.dist-info/RECORD
-7 files, 1699 bytes uncompressed, 983 bytes compressed:  42.1%
+Zip file size: 2151 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      263 b- defN 23-Jun-07 00:16 datasette_sqlite_url/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 00:16 datasette_sqlite_url/version.py
+-rw-r--r--  2.0 unx      557 b- defN 23-Jun-07 00:16 datasette_sqlite_url-0.1.0a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 00:16 datasette_sqlite_url-0.1.0a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-07 00:16 datasette_sqlite_url-0.1.0a4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-07 00:16 datasette_sqlite_url-0.1.0a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      641 b- defN 23-Jun-07 00:16 datasette_sqlite_url-0.1.0a4.dist-info/RECORD
+7 files, 1699 bytes uncompressed, 985 bytes compressed:  42.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_url/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_url/version.py
 Comment: 
 
-Filename: datasette_sqlite_url-0.1.0a3.dist-info/METADATA
+Filename: datasette_sqlite_url-0.1.0a4.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_url-0.1.0a3.dist-info/WHEEL
+Filename: datasette_sqlite_url-0.1.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_url-0.1.0a3.dist-info/entry_points.txt
+Filename: datasette_sqlite_url-0.1.0a4.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_url-0.1.0a3.dist-info/top_level.txt
+Filename: datasette_sqlite_url-0.1.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_url-0.1.0a3.dist-info/RECORD
+Filename: datasette_sqlite_url-0.1.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_url/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.3"
+__version__ = "0.1.0-alpha.4"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_url-0.1.0a3.dist-info/METADATA` & `datasette_sqlite_url-0.1.0a4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-url
-Version: 0.1.0a3
+Version: 0.1.0a4
 Home-page: https://github.com/asg017/sqlite-url
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-url/issues
 Project-URL: CI, https://github.com/asg017/sqlite-url/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-url/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_url-0.1.0a3.dist-info/RECORD` & `datasette_sqlite_url-0.1.0a4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_url/__init__.py,sha256=Bra1WL27mDdTpOJmzat4PYilifTCRMRt-6w-7wMnUiQ,263
-datasette_sqlite_url/version.py,sha256=UsYOyUf0to_Ob8SXHxxquepi8gVho4EnFOtvMVe3xNc,79
-datasette_sqlite_url-0.1.0a3.dist-info/METADATA,sha256=T6BCnVB6hJ0V-JALPA05kwc_4YfLGpEZCJtuoCAlPAs,557
-datasette_sqlite_url-0.1.0a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_url-0.1.0a3.dist-info/entry_points.txt,sha256=HQEiMzI1CmR1lBCK-ESrNKvjreOtJPaVPxmzHl-ad8Y,46
-datasette_sqlite_url-0.1.0a3.dist-info/top_level.txt,sha256=V3MvfLt8BiVG8tbH9khaAX-QHgIKham-ba85tSCTu98,21
-datasette_sqlite_url-0.1.0a3.dist-info/RECORD,,
+datasette_sqlite_url/version.py,sha256=_9iw-Vd8eX6yNm_UJ00B-r49sQ9eJXJWWZXiQTepATw,79
+datasette_sqlite_url-0.1.0a4.dist-info/METADATA,sha256=tpu_6rDJvTpjGfRxmiuXmvQRd7HuWMKNbTGmHswBbXA,557
+datasette_sqlite_url-0.1.0a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+datasette_sqlite_url-0.1.0a4.dist-info/entry_points.txt,sha256=HQEiMzI1CmR1lBCK-ESrNKvjreOtJPaVPxmzHl-ad8Y,46
+datasette_sqlite_url-0.1.0a4.dist-info/top_level.txt,sha256=V3MvfLt8BiVG8tbH9khaAX-QHgIKham-ba85tSCTu98,21
+datasette_sqlite_url-0.1.0a4.dist-info/RECORD,,
```

