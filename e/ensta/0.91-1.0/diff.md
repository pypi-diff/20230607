# Comparing `tmp/ensta-0.91.tar.gz` & `tmp/ensta-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-0.91.tar", last modified: Wed Jun  7 07:40:44 2023, max compression
+gzip compressed data, was "ensta-1.0.tar", last modified: Wed Jun  7 08:06:14 2023, max compression
```

## Comparing `ensta-0.91.tar` & `ensta-1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 07:40:44.361421 ensta-0.91/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-0.91/LICENSE.txt
--rw-rw-rw-   0        0        0     1688 2023-06-07 07:40:44.361421 ensta-0.91/PKG-INFO
--rw-rw-rw-   0        0        0      964 2023-06-06 15:54:53.000000 ensta-0.91/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 07:40:44.345722 ensta-0.91/ensta/
--rw-rw-rw-   0        0        0    15694 2023-06-07 07:35:55.000000 ensta-0.91/ensta/Guest.py
--rw-rw-rw-   0        0        0     6495 2023-06-07 07:37:23.000000 ensta-0.91/ensta/Host.py
--rw-rw-rw-   0        0        0       60 2023-06-07 07:03:08.000000 ensta-0.91/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:40:44.361421 ensta-0.91/ensta/lib/
--rw-rw-rw-   0        0        0     1169 2023-06-07 07:34:14.000000 ensta-0.91/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0      217 2023-06-05 12:51:10.000000 ensta-0.91/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      197 2023-06-07 07:37:50.000000 ensta-0.91/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:40:44.361421 ensta-0.91/ensta.egg-info/
--rw-rw-rw-   0        0        0     1688 2023-06-07 07:40:44.000000 ensta-0.91/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-07 07:40:44.000000 ensta-0.91/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 07:40:44.000000 ensta-0.91/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 07:40:44.000000 ensta-0.91/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 07:40:44.000000 ensta-0.91/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-07 07:40:44.361421 ensta-0.91/setup.cfg
--rw-rw-rw-   0        0        0     1034 2023-06-07 07:40:38.000000 ensta-0.91/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:06:14.191179 ensta-1.0/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1687 2023-06-07 08:06:14.191179 ensta-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2023-06-06 15:54:53.000000 ensta-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 08:06:14.156010 ensta-1.0/ensta/
+-rw-rw-rw-   0        0        0    15694 2023-06-07 07:35:55.000000 ensta-1.0/ensta/Guest.py
+-rw-rw-rw-   0        0        0     6495 2023-06-07 07:37:23.000000 ensta-1.0/ensta/Host.py
+-rw-rw-rw-   0        0        0       60 2023-06-07 07:03:08.000000 ensta-1.0/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:06:14.191179 ensta-1.0/ensta/lib/
+-rw-rw-rw-   0        0        0     1169 2023-06-07 07:34:14.000000 ensta-1.0/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0      217 2023-06-05 12:51:10.000000 ensta-1.0/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      197 2023-06-07 07:37:50.000000 ensta-1.0/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:06:14.175345 ensta-1.0/ensta.egg-info/
+-rw-rw-rw-   0        0        0     1687 2023-06-07 08:06:14.000000 ensta-1.0/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-07 08:06:14.000000 ensta-1.0/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 08:06:14.000000 ensta-1.0/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 08:06:14.000000 ensta-1.0/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 08:06:14.000000 ensta-1.0/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-07 08:06:14.206847 ensta-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2023-06-07 07:50:24.000000 ensta-1.0/setup.py
```

### Comparing `ensta-0.91/LICENSE.txt` & `ensta-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-0.91/PKG-INFO` & `ensta-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 0.91
+Version: 1.0
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v0.1.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.0.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ensta-0.91/README.md` & `ensta-1.0/README.md`

 * *Files identical despite different names*

### Comparing `ensta-0.91/ensta/Guest.py` & `ensta-1.0/ensta/Guest.py`

 * *Files identical despite different names*

### Comparing `ensta-0.91/ensta/Host.py` & `ensta-1.0/ensta/Host.py`

 * *Files identical despite different names*

### Comparing `ensta-0.91/ensta/lib/Commons.py` & `ensta-1.0/ensta/lib/Commons.py`

 * *Files identical despite different names*

### Comparing `ensta-0.91/ensta.egg-info/PKG-INFO` & `ensta-1.0/ensta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 0.91
+Version: 1.0
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v0.1.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.0.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ensta-0.91/setup.py` & `ensta-1.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="ensta",
     packages=["ensta", "ensta.lib"],
-    version="0.91",
+    version="1.0",
     license="MIT",
     description="Simple & Up-to-date Instagram API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v0.1.tar.gz",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.0.tar.gz",
     keywords=["instagram", "web", "private", "api", "scraper", "easy", "download", "upload"],
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
```

