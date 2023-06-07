# Comparing `tmp/Fict-1.0.0.tar.gz` & `tmp/Fict-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fict-1.0.0.tar", last modified: Wed Jun  7 02:04:03 2023, max compression
+gzip compressed data, was "Fict-1.0.1.tar", last modified: Wed Jun  7 02:05:18 2023, max compression
```

## Comparing `Fict-1.0.0.tar` & `Fict-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 yam       (1000) yam       (1000)        0 2023-06-07 02:04:03.927108 Fict-1.0.0/
-drwxrwxrwx   0 yam       (1000) yam       (1000)        0 2023-06-07 02:04:03.917108 Fict-1.0.0/Fict.egg-info/
--rwxrwxrwx   0 yam       (1000) yam       (1000)     2708 2023-06-07 02:04:03.000000 Fict-1.0.0/Fict.egg-info/PKG-INFO
--rwxrwxrwx   0 yam       (1000) yam       (1000)      205 2023-06-07 02:04:03.000000 Fict-1.0.0/Fict.egg-info/SOURCES.txt
--rwxrwxrwx   0 yam       (1000) yam       (1000)        1 2023-06-07 02:04:03.000000 Fict-1.0.0/Fict.egg-info/dependency_links.txt
--rwxrwxrwx   0 yam       (1000) yam       (1000)       33 2023-06-07 02:04:03.000000 Fict-1.0.0/Fict.egg-info/requires.txt
--rwxrwxrwx   0 yam       (1000) yam       (1000)        4 2023-06-07 02:04:03.000000 Fict-1.0.0/Fict.egg-info/top_level.txt
--rwxrwxrwx   0 yam       (1000) yam       (1000)     2708 2023-06-07 02:04:03.927108 Fict-1.0.0/PKG-INFO
--rw-rw-r--   0 yam       (1000) yam       (1000)     1947 2023-06-07 02:02:19.000000 Fict-1.0.0/README.md
--rwxrwxr-x   0 yam       (1000) yam       (1000)     1254 2023-06-03 19:44:17.000000 Fict-1.0.0/fict
-drwxrwxrwx   0 yam       (1000) yam       (1000)        0 2023-06-07 02:04:03.924108 Fict-1.0.0/lib/
--rw-rw-r--   0 yam       (1000) yam       (1000)        0 2021-11-06 03:42:29.000000 Fict-1.0.0/lib/__init__.py
--rwxrwxr-x   0 yam       (1000) yam       (1000)     8439 2023-06-03 20:39:27.000000 Fict-1.0.0/lib/core.py
--rwxrwxr-x   0 yam       (1000) yam       (1000)     5592 2023-06-03 20:31:21.000000 Fict-1.0.0/lib/fileobj.py
--rwxrwxrwx   0 yam       (1000) yam       (1000)       38 2023-06-07 02:04:03.928108 Fict-1.0.0/setup.cfg
--rw-rw-r--   0 yam       (1000) yam       (1000)      721 2023-06-07 02:03:52.000000 Fict-1.0.0/setup.py
+drwxrwxrwx   0 yam       (1000) yam       (1000)        0 2023-06-07 02:05:18.308046 Fict-1.0.1/
+drwxrwxrwx   0 yam       (1000) yam       (1000)        0 2023-06-07 02:05:18.300046 Fict-1.0.1/Fict.egg-info/
+-rwxrwxrwx   0 yam       (1000) yam       (1000)     2708 2023-06-07 02:05:18.000000 Fict-1.0.1/Fict.egg-info/PKG-INFO
+-rwxrwxrwx   0 yam       (1000) yam       (1000)      205 2023-06-07 02:05:18.000000 Fict-1.0.1/Fict.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yam       (1000) yam       (1000)        1 2023-06-07 02:05:18.000000 Fict-1.0.1/Fict.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yam       (1000) yam       (1000)       33 2023-06-07 02:05:18.000000 Fict-1.0.1/Fict.egg-info/requires.txt
+-rwxrwxrwx   0 yam       (1000) yam       (1000)        4 2023-06-07 02:05:18.000000 Fict-1.0.1/Fict.egg-info/top_level.txt
+-rwxrwxrwx   0 yam       (1000) yam       (1000)     2708 2023-06-07 02:05:18.307046 Fict-1.0.1/PKG-INFO
+-rw-rw-r--   0 yam       (1000) yam       (1000)     1947 2023-06-07 02:02:19.000000 Fict-1.0.1/README.md
+-rwxrwxr-x   0 yam       (1000) yam       (1000)     1254 2023-06-03 19:44:17.000000 Fict-1.0.1/fict
+drwxrwxrwx   0 yam       (1000) yam       (1000)        0 2023-06-07 02:05:18.305046 Fict-1.0.1/lib/
+-rw-rw-r--   0 yam       (1000) yam       (1000)        0 2021-11-06 03:42:29.000000 Fict-1.0.1/lib/__init__.py
+-rwxrwxr-x   0 yam       (1000) yam       (1000)     8439 2023-06-03 20:39:27.000000 Fict-1.0.1/lib/core.py
+-rwxrwxr-x   0 yam       (1000) yam       (1000)     5592 2023-06-03 20:31:21.000000 Fict-1.0.1/lib/fileobj.py
+-rwxrwxrwx   0 yam       (1000) yam       (1000)       38 2023-06-07 02:05:18.309046 Fict-1.0.1/setup.cfg
+-rw-rw-r--   0 yam       (1000) yam       (1000)      721 2023-06-07 02:04:50.000000 Fict-1.0.1/setup.py
```

### Comparing `Fict-1.0.0/Fict.egg-info/PKG-INFO` & `Fict-1.0.1/Fict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fict
-Version: 1.0.0
+Version: 1.0.1
 Summary: File integrity checking tool
 Home-page: https://github.com/vhp/fict
 Author: Vincent Perricone
 Author-email: vhp@fastmail.fm
 License: Simplified FreeBSD License
 Download-URL: https://github.com/vhp/fict
 Description: # FICT is a simple file integrity checking tool.
```

### Comparing `Fict-1.0.0/PKG-INFO` & `Fict-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fict
-Version: 1.0.0
+Version: 1.0.1
 Summary: File integrity checking tool
 Home-page: https://github.com/vhp/fict
 Author: Vincent Perricone
 Author-email: vhp@fastmail.fm
 License: Simplified FreeBSD License
 Download-URL: https://github.com/vhp/fict
 Description: # FICT is a simple file integrity checking tool.
```

### Comparing `Fict-1.0.0/README.md` & `Fict-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Fict-1.0.0/fict` & `Fict-1.0.1/fict`

 * *Files identical despite different names*

### Comparing `Fict-1.0.0/lib/core.py` & `Fict-1.0.1/lib/core.py`

 * *Files identical despite different names*

### Comparing `Fict-1.0.0/lib/fileobj.py` & `Fict-1.0.1/lib/fileobj.py`

 * *Files identical despite different names*

### Comparing `Fict-1.0.0/setup.py` & `Fict-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'Fict',
-    version = "1.0.0",
+    version = "1.0.1",
     description = 'File integrity checking tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Vincent Perricone',
     author_email = 'vhp@fastmail.fm',
     url = 'https://github.com/vhp/fict',
     download_url = 'https://github.com/vhp/fict',
```

