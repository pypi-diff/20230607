# Comparing `tmp/flutter-driver-1.0.tar.gz` & `tmp/flutter-driver-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flutter-driver-1.0.tar", last modified: Wed Jun  7 07:46:31 2023, max compression
+gzip compressed data, was "flutter-driver-1.0.1.tar", last modified: Wed Jun  7 08:15:36 2023, max compression
```

## Comparing `flutter-driver-1.0.tar` & `flutter-driver-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 07:46:30.939413 flutter-driver-1.0/
--rw-rw-rw-   0        0        0     1087 2023-05-04 06:13:55.000000 flutter-driver-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     5707 2023-06-07 07:46:30.938917 flutter-driver-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4642 2023-06-07 07:44:09.000000 flutter-driver-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 07:46:30.936933 flutter-driver-1.0/flutter_driver.egg-info/
--rw-rw-rw-   0        0        0     5707 2023-06-07 07:46:30.000000 flutter-driver-1.0/flutter_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-07 07:46:30.000000 flutter-driver-1.0/flutter_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 07:46:30.000000 flutter-driver-1.0/flutter_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 07:46:30.000000 flutter-driver-1.0/flutter_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 07:46:30.939909 flutter-driver-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1375 2023-06-07 07:17:33.000000 flutter-driver-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:15:36.524618 flutter-driver-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-05-04 06:13:55.000000 flutter-driver-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     5709 2023-06-07 08:15:36.523625 flutter-driver-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4642 2023-06-07 07:44:09.000000 flutter-driver-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 08:15:36.521148 flutter-driver-1.0.1/flutter_driver.egg-info/
+-rw-rw-rw-   0        0        0     5709 2023-06-07 08:15:36.000000 flutter-driver-1.0.1/flutter_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-07 08:15:36.000000 flutter-driver-1.0.1/flutter_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 08:15:36.000000 flutter-driver-1.0.1/flutter_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 08:15:36.000000 flutter-driver-1.0.1/flutter_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 08:15:36.524618 flutter-driver-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-06-07 08:13:57.000000 flutter-driver-1.0.1/setup.py
```

### Comparing `flutter-driver-1.0/LICENSE.txt` & `flutter-driver-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flutter-driver-1.0/PKG-INFO` & `flutter-driver-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flutter-driver
-Version: 1.0
+Version: 1.0.1
 Summary: An flutter automation driver for python
 Home-page: https://github.com/183181731/flutter-driver
 Author: ndaeqa-wang
 Author-email: 183181731@qq.com
 License: MIT
 Keywords: flutter windows,python client,ui automation
 Platform: UNKNOWN
```

### Comparing `flutter-driver-1.0/README.md` & `flutter-driver-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `flutter-driver-1.0/flutter_driver.egg-info/PKG-INFO` & `flutter-driver-1.0.1/flutter_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flutter-driver
-Version: 1.0
+Version: 1.0.1
 Summary: An flutter automation driver for python
 Home-page: https://github.com/183181731/flutter-driver
 Author: ndaeqa-wang
 Author-email: 183181731@qq.com
 License: MIT
 Keywords: flutter windows,python client,ui automation
 Platform: UNKNOWN
```

### Comparing `flutter-driver-1.0/setup.py` & `flutter-driver-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import io
 import os
 
 from setuptools import find_packages, setup
 
 setup(
     name='flutter-driver',
-    version='1.0',
+    version='1.0.1',
     description='An flutter automation driver for python',
     long_description=io.open(os.path.join(os.path.dirname('__file__'), 'README.md'), encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     keywords=[
         'flutter windows',
         'python client',
         'ui automation'
```

