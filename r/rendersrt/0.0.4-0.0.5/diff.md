# Comparing `tmp/rendersrt-0.0.4.tar.gz` & `tmp/rendersrt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rendersrt-0.0.4.tar", last modified: Sat Jun  3 18:15:51 2023, max compression
+gzip compressed data, was "rendersrt-0.0.5.tar", last modified: Wed Jun  7 15:14:09 2023, max compression
```

## Comparing `rendersrt-0.0.4.tar` & `rendersrt-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 18:15:51.840502 rendersrt-0.0.4/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1561 2023-06-03 18:15:51.840502 rendersrt-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 18:15:51.809772 rendersrt-0.0.4/rendersrt/
--rw-rw-rw-   0        0        0     9549 2023-06-03 18:15:40.000000 rendersrt-0.0.4/rendersrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:15:51.838254 rendersrt-0.0.4/rendersrt.egg-info/
--rw-rw-rw-   0        0        0     1561 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-03 18:15:51.000000 rendersrt-0.0.4/rendersrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-03 18:15:51.842749 rendersrt-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1360 2023-06-02 22:10:10.000000 rendersrt-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:14:09.179800 rendersrt-0.0.5/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1563 2023-06-07 15:14:09.180549 rendersrt-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 15:14:09.122926 rendersrt-0.0.5/rendersrt/
+-rw-rw-rw-   0        0        0    58233 2023-06-07 15:12:20.000000 rendersrt-0.0.5/rendersrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:14:09.177552 rendersrt-0.0.5/rendersrt.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-07 15:14:09.184851 rendersrt-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1362 2023-06-07 15:11:16.000000 rendersrt-0.0.5/setup.py
```

### Comparing `rendersrt-0.0.4/LICENSE` & `rendersrt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.4/PKG-INFO` & `rendersrt-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.4
+Version: 0.0.5
 Summary: a utility for rendering subtitle file into video file
-Home-page: https://github.com/botbahlul/autosrt
+Home-page: https://github.com/botbahlul/rendersrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rendersrt-0.0.4/README.md` & `rendersrt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.4/rendersrt.egg-info/PKG-INFO` & `rendersrt-0.0.5/rendersrt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.4
+Version: 0.0.5
 Summary: a utility for rendering subtitle file into video file
-Home-page: https://github.com/botbahlul/autosrt
+Home-page: https://github.com/botbahlul/rendersrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rendersrt-0.0.4/setup.py` & `rendersrt-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 setup(
     name="rendersrt",
     version=get_version(),
     description="a utility for rendering subtitle file into video file",
     long_description = long_description,
     author="Bot Bahlul",
     author_email="bot.bahlul@gmail.com",
-    url="https://github.com/botbahlul/autosrt",
+    url="https://github.com/botbahlul/rendersrt",
     packages=["rendersrt"],
     entry_points={
         "console_scripts": [
             "rendersrt = rendersrt:main",
         ],
     },
     install_requires=install_requires,
```

