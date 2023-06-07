# Comparing `tmp/ensta-0.8.tar.gz` & `tmp/ensta-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-0.8.tar", last modified: Wed Jun  7 07:26:23 2023, max compression
+gzip compressed data, was "ensta-0.9.tar", last modified: Wed Jun  7 07:29:35 2023, max compression
```

## Comparing `ensta-0.8.tar` & `ensta-0.9.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 07:26:23.752055 ensta-0.8/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     1687 2023-06-07 07:26:23.752055 ensta-0.8/PKG-INFO
--rw-rw-rw-   0        0        0      964 2023-06-06 15:54:53.000000 ensta-0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 07:26:23.736679 ensta-0.8/ensta/
--rw-rw-rw-   0        0        0    15707 2023-06-07 07:24:35.000000 ensta-0.8/ensta/Guest.py
--rw-rw-rw-   0        0        0     6508 2023-06-07 07:25:37.000000 ensta-0.8/ensta/Host.py
--rw-rw-rw-   0        0        0       60 2023-06-07 07:03:08.000000 ensta-0.8/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:26:23.752055 ensta-0.8/ensta.egg-info/
--rw-rw-rw-   0        0        0     1687 2023-06-07 07:26:23.000000 ensta-0.8/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-07 07:26:23.000000 ensta-0.8/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 07:26:23.000000 ensta-0.8/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 07:26:23.000000 ensta-0.8/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 07:26:23.000000 ensta-0.8/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-07 07:26:23.752055 ensta-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-06-07 07:26:11.000000 ensta-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:29:35.199913 ensta-0.9/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     1687 2023-06-07 07:29:35.199913 ensta-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2023-06-06 15:54:53.000000 ensta-0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 07:29:35.168829 ensta-0.9/ensta/
+-rw-rw-rw-   0        0        0    15707 2023-06-07 07:24:35.000000 ensta-0.9/ensta/Guest.py
+-rw-rw-rw-   0        0        0     6508 2023-06-07 07:25:37.000000 ensta-0.9/ensta/Host.py
+-rw-rw-rw-   0        0        0       60 2023-06-07 07:03:08.000000 ensta-0.9/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:29:35.184286 ensta-0.9/ensta/lib/
+-rw-rw-rw-   0        0        0     1363 2023-06-07 07:22:50.000000 ensta-0.9/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0      217 2023-06-05 12:51:10.000000 ensta-0.9/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:23:02.000000 ensta-0.9/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:29:35.184286 ensta-0.9/ensta.egg-info/
+-rw-rw-rw-   0        0        0     1687 2023-06-07 07:29:35.000000 ensta-0.9/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-07 07:29:35.000000 ensta-0.9/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 07:29:35.000000 ensta-0.9/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 07:29:35.000000 ensta-0.9/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 07:29:35.000000 ensta-0.9/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-07 07:29:35.199913 ensta-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2023-06-07 07:29:33.000000 ensta-0.9/setup.py
```

### Comparing `ensta-0.8/LICENSE.txt` & `ensta-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-0.8/PKG-INFO` & `ensta-0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 0.8
+Version: 0.9
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v0.1.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
```

### Comparing `ensta-0.8/README.md` & `ensta-0.9/README.md`

 * *Files identical despite different names*

### Comparing `ensta-0.8/ensta/Guest.py` & `ensta-0.9/ensta/Guest.py`

 * *Files identical despite different names*

### Comparing `ensta-0.8/ensta/Host.py` & `ensta-0.9/ensta/Host.py`

 * *Files identical despite different names*

### Comparing `ensta-0.8/ensta.egg-info/PKG-INFO` & `ensta-0.9/ensta.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 0.8
+Version: 0.9
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v0.1.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
```

### Comparing `ensta-0.8/setup.py` & `ensta-0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from distutils.core import setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="ensta",
-    packages=["ensta"],
-    version="0.8",
+    packages=["ensta", "ensta.lib"],
+    version="0.9",
     license="MIT",
     description="Simple & Up-to-date Instagram API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
```

