# Comparing `tmp/isikukood-1.0.1.tar.gz` & `tmp/isikukood-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/isikukood-1.0.1.tar", last modified: Wed Jun  7 21:12:37 2023, max compression
+gzip compressed data, was "dist/isikukood-1.0.2.tar", last modified: Wed Jun  7 21:17:55 2023, max compression
```

## Comparing `isikukood-1.0.1.tar` & `isikukood-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 21:12:37.000000 isikukood-1.0.1/
--rw-r--r--   0 user      (1000) user      (1000)    35149 2023-05-30 11:16:14.000000 isikukood-1.0.1/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    11479 2023-06-07 21:12:37.000000 isikukood-1.0.1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)    10783 2023-06-07 20:58:43.000000 isikukood-1.0.1/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood/
--rw-r--r--   0 user      (1000) user      (1000)      482 2023-06-03 15:39:16.000000 isikukood-1.0.1/isikukood/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     5606 2023-06-07 08:19:34.000000 isikukood-1.0.1/isikukood/assertions.py
--rw-r--r--   0 user      (1000) user      (1000)      149 2023-05-30 13:24:27.000000 isikukood-1.0.1/isikukood/errors.py
--rw-r--r--   0 user      (1000) user      (1000)     6854 2023-06-07 19:57:01.000000 isikukood-1.0.1/isikukood/functions.py
--rw-r--r--   0 user      (1000) user      (1000)     4107 2023-06-07 20:47:46.000000 isikukood-1.0.1/isikukood/isikukood.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    11479 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      302 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       12 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       10 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-07 21:12:37.000000 isikukood-1.0.1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1077 2023-06-07 21:12:01.000000 isikukood-1.0.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 21:17:55.000000 isikukood-1.0.2/
+-rw-r--r--   0 user      (1000) user      (1000)    35149 2023-05-30 11:16:14.000000 isikukood-1.0.2/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    11492 2023-06-07 21:17:55.000000 isikukood-1.0.2/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)    10783 2023-06-07 20:58:43.000000 isikukood-1.0.2/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 21:17:55.000000 isikukood-1.0.2/isikukood/
+-rw-r--r--   0 user      (1000) user      (1000)      482 2023-06-03 15:39:16.000000 isikukood-1.0.2/isikukood/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5606 2023-06-07 08:19:34.000000 isikukood-1.0.2/isikukood/assertions.py
+-rw-r--r--   0 user      (1000) user      (1000)      149 2023-05-30 13:24:27.000000 isikukood-1.0.2/isikukood/errors.py
+-rw-r--r--   0 user      (1000) user      (1000)     6854 2023-06-07 19:57:01.000000 isikukood-1.0.2/isikukood/functions.py
+-rw-r--r--   0 user      (1000) user      (1000)     4107 2023-06-07 20:47:46.000000 isikukood-1.0.2/isikukood/isikukood.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 21:17:55.000000 isikukood-1.0.2/isikukood.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    11492 2023-06-07 21:17:55.000000 isikukood-1.0.2/isikukood.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      302 2023-06-07 21:17:55.000000 isikukood-1.0.2/isikukood.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-07 21:17:55.000000 isikukood-1.0.2/isikukood.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       12 2023-06-07 21:17:55.000000 isikukood-1.0.2/isikukood.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       10 2023-06-07 21:17:55.000000 isikukood-1.0.2/isikukood.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-07 21:17:55.000000 isikukood-1.0.2/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1090 2023-06-07 21:17:51.000000 isikukood-1.0.2/setup.py
```

### Comparing `isikukood-1.0.1/LICENSE` & `isikukood-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isikukood-1.0.1/PKG-INFO` & `isikukood-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: isikukood
-Version: 1.0.1
+Version: 1.0.2
 Summary: Estonian SSN library
 Home-page: https://github.com/ui-1/isikukood
 Author: ui-1
 Author-email: ui-1@posteo.org
 License: GPLv3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
```

### Comparing `isikukood-1.0.1/README.md` & `isikukood-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `isikukood-1.0.1/isikukood/assertions.py` & `isikukood-1.0.2/isikukood/assertions.py`

 * *Files identical despite different names*

### Comparing `isikukood-1.0.1/isikukood/functions.py` & `isikukood-1.0.2/isikukood/functions.py`

 * *Files identical despite different names*

### Comparing `isikukood-1.0.1/isikukood/isikukood.py` & `isikukood-1.0.2/isikukood/isikukood.py`

 * *Files identical despite different names*

### Comparing `isikukood-1.0.1/isikukood.egg-info/PKG-INFO` & `isikukood-1.0.2/isikukood.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: isikukood
-Version: 1.0.1
+Version: 1.0.2
 Summary: Estonian SSN library
 Home-page: https://github.com/ui-1/isikukood
 Author: ui-1
 Author-email: ui-1@posteo.org
 License: GPLv3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
```

### Comparing `isikukood-1.0.1/setup.py` & `isikukood-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="isikukood",
-    version="1.0.1",
+    version="1.0.2",
     description="Estonian SSN library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ui-1/isikukood",
     author="ui-1",
     author_email="ui-1@posteo.org",
     license="GPLv3",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Operating System :: OS Independent",
```

