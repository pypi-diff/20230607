# Comparing `tmp/LiamHsieh toolbox-0.3.4.tar.gz` & `tmp/LiamHsieh toolbox-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LiamHsieh toolbox-0.3.4.tar", last modified: Tue Jun  6 22:26:42 2023, max compression
+gzip compressed data, was "LiamHsieh toolbox-0.3.5.tar", last modified: Wed Jun  7 00:07:14 2023, max compression
```

## Comparing `LiamHsieh toolbox-0.3.4.tar` & `LiamHsieh toolbox-0.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-06 22:26:42.511184 LiamHsieh toolbox-0.3.4/
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-06 22:26:42.511184 LiamHsieh toolbox-0.3.4/LiamHsieh_toolbox.egg-info/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1262 2023-06-06 22:26:42.000000 LiamHsieh toolbox-0.3.4/LiamHsieh_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      241 2023-06-06 22:26:42.000000 LiamHsieh toolbox-0.3.4/LiamHsieh_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        1 2023-06-06 22:26:42.000000 LiamHsieh toolbox-0.3.4/LiamHsieh_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      308 2023-06-06 22:26:42.000000 LiamHsieh toolbox-0.3.4/LiamHsieh_toolbox.egg-info/requires.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        1 2023-06-06 22:26:42.000000 LiamHsieh toolbox-0.3.4/LiamHsieh_toolbox.egg-info/top_level.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1262 2023-06-06 22:26:42.511184 LiamHsieh toolbox-0.3.4/PKG-INFO
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      836 2023-06-06 22:25:15.000000 LiamHsieh toolbox-0.3.4/README.md
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       38 2023-06-06 22:26:42.511184 LiamHsieh toolbox-0.3.4/setup.cfg
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1410 2023-06-06 22:25:23.000000 LiamHsieh toolbox-0.3.4/setup.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-06 22:26:42.511184 LiamHsieh toolbox-0.3.4/toolbox/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     2513 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4/toolbox/utility.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:07:14.661184 LiamHsieh toolbox-0.3.5/
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:07:14.661184 LiamHsieh toolbox-0.3.5/LiamHsieh_toolbox.egg-info/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1261 2023-06-07 00:07:14.000000 LiamHsieh toolbox-0.3.5/LiamHsieh_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      241 2023-06-07 00:07:14.000000 LiamHsieh toolbox-0.3.5/LiamHsieh_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        1 2023-06-07 00:07:14.000000 LiamHsieh toolbox-0.3.5/LiamHsieh_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      308 2023-06-07 00:07:14.000000 LiamHsieh toolbox-0.3.5/LiamHsieh_toolbox.egg-info/requires.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        1 2023-06-07 00:07:14.000000 LiamHsieh toolbox-0.3.5/LiamHsieh_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1261 2023-06-07 00:07:14.661184 LiamHsieh toolbox-0.3.5/PKG-INFO
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      836 2023-06-06 22:25:15.000000 LiamHsieh toolbox-0.3.5/README.md
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       38 2023-06-07 00:07:14.661184 LiamHsieh toolbox-0.3.5/setup.cfg
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1409 2023-06-07 00:05:44.000000 LiamHsieh toolbox-0.3.5/setup.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:07:14.661184 LiamHsieh toolbox-0.3.5/toolbox/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     2513 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.5/toolbox/utility.py
```

### Comparing `LiamHsieh toolbox-0.3.4/LiamHsieh_toolbox.egg-info/PKG-INFO` & `LiamHsieh toolbox-0.3.5/LiamHsieh_toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: LiamHsieh-toolbox
-Version: 0.3.4
+Version: 0.3.5
 Summary: Collections of Python utility, suppose to be built with Jonathan Carson but he left
 Author: Liam Y. Hsieh, PhD
 Author-email: liamhsieh@ieee.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # LiamHsieh toolbox
 Author: Liam Hsieh  
 Latest update: Dec 21, 2022
 
 This package is a collection of Python utilities created for benefiting my development of prototypes/applications regarding data-driven decision science a bit easier.
```

### Comparing `LiamHsieh toolbox-0.3.4/PKG-INFO` & `LiamHsieh toolbox-0.3.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: LiamHsieh toolbox
-Version: 0.3.4
+Version: 0.3.5
 Summary: Collections of Python utility, suppose to be built with Jonathan Carson but he left
 Author: Liam Y. Hsieh, PhD
 Author-email: liamhsieh@ieee.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # LiamHsieh toolbox
 Author: Liam Hsieh  
 Latest update: Dec 21, 2022
 
 This package is a collection of Python utilities created for benefiting my development of prototypes/applications regarding data-driven decision science a bit easier.
```

### Comparing `LiamHsieh toolbox-0.3.4/README.md` & `LiamHsieh toolbox-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4/setup.py` & `LiamHsieh toolbox-0.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="LiamHsieh toolbox",
-    version = '0.3.4',
+    version = '0.3.5',
     description = "Collections of Python utility, suppose to be built with Jonathan Carson but he left",
     author = 'Liam Y. Hsieh, PhD',
     author_email = 'liamhsieh@ieee.org',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = setuptools.find_packages(),
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Development Status :: 2 - Pre-Alpha",
     ],
     #packages = ['toolbox'], #, since I only have a subfolder, toolbox, below setup.py and I don't wanna include docs as well, I just manually list what I need  
-    python_requires='>=3.10',
+    python_requires='>=3.9',
     install_requires=[
         'pandas>=2.0',
         'sqlalchemy>=1.4.40',
         'openpyxl>=3.0.10',
         'pyxlsb>=1.0.9',
         'dask>=2022.8.1',
         'filetype>=1.1.0',
```

### Comparing `LiamHsieh toolbox-0.3.4/toolbox/utility.py` & `LiamHsieh toolbox-0.3.5/toolbox/utility.py`

 * *Files identical despite different names*

