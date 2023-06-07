# Comparing `tmp/mlplatformutils-0.9.1.1.tar.gz` & `tmp/mlplatformutils-0.9.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.1.1.tar", last modified: Wed Jun  7 03:23:17 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.1.2.tar", last modified: Wed Jun  7 03:35:14 2023, max compression
```

## Comparing `mlplatformutils-0.9.1.1.tar` & `mlplatformutils-0.9.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 03:23:17.277786 mlplatformutils-0.9.1.1/
--rw-rw-rw-   0        0        0     3470 2023-06-07 03:23:17.278786 mlplatformutils-0.9.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.1.1/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-07 03:23:17.283793 mlplatformutils-0.9.1.1/setup.cfg
--rw-rw-rw-   0        0        0      810 2023-06-07 03:22:31.000000 mlplatformutils-0.9.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:23:17.023757 mlplatformutils-0.9.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 03:23:17.046097 mlplatformutils-0.9.1.1/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.1.1/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:23:17.274788 mlplatformutils-0.9.1.1/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.1.1/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.1.1/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.1.1/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     9560 2023-06-07 03:21:53.000000 mlplatformutils-0.9.1.1/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.1.1/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7879 2023-06-06 22:09:17.000000 mlplatformutils-0.9.1.1/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       21 2023-06-07 03:17:18.000000 mlplatformutils-0.9.1.1/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:23:17.093645 mlplatformutils-0.9.1.1/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     3470 2023-06-07 03:23:16.000000 mlplatformutils-0.9.1.1/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-07 03:23:16.000000 mlplatformutils-0.9.1.1/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 03:23:16.000000 mlplatformutils-0.9.1.1/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-07 03:23:16.000000 mlplatformutils-0.9.1.1/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-07 03:23:16.000000 mlplatformutils-0.9.1.1/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 03:35:14.833687 mlplatformutils-0.9.1.2/
+-rw-rw-rw-   0        0        0     3470 2023-06-07 03:35:14.833687 mlplatformutils-0.9.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.1.2/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-07 03:35:14.836690 mlplatformutils-0.9.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      810 2023-06-07 03:35:10.000000 mlplatformutils-0.9.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:35:14.756849 mlplatformutils-0.9.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 03:35:14.770110 mlplatformutils-0.9.1.2/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:35:14.830689 mlplatformutils-0.9.1.2/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     9560 2023-06-07 03:21:53.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7879 2023-06-06 22:09:17.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       23 2023-06-07 03:35:03.000000 mlplatformutils-0.9.1.2/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:35:14.801161 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3470 2023-06-07 03:35:14.000000 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-07 03:35:14.000000 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 03:35:14.000000 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-07 03:35:14.000000 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 03:35:14.000000 mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.1.1/PKG-INFO` & `mlplatformutils-0.9.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.1.1
+Version: 0.9.1.2
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.1.1/setup.py` & `mlplatformutils-0.9.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.1.1',
+    version='0.9.1.2',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.9.1.1/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.1.2/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.1/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.1.2/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.1/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.1.2/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.1/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.1.2/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.1/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.1.2/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.1.1/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.1.1
+Version: 0.9.1.2
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.1.1/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.1.2/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

