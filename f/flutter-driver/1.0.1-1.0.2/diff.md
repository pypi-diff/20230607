# Comparing `tmp/flutter-driver-1.0.1.tar.gz` & `tmp/flutter-driver-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flutter-driver-1.0.1.tar", last modified: Wed Jun  7 08:15:36 2023, max compression
+gzip compressed data, was "flutter-driver-1.0.2.tar", last modified: Wed Jun  7 08:24:43 2023, max compression
```

## Comparing `flutter-driver-1.0.1.tar` & `flutter-driver-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 08:15:36.524618 flutter-driver-1.0.1/
--rw-rw-rw-   0        0        0     1087 2023-05-04 06:13:55.000000 flutter-driver-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5709 2023-06-07 08:15:36.523625 flutter-driver-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4642 2023-06-07 07:44:09.000000 flutter-driver-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 08:15:36.521148 flutter-driver-1.0.1/flutter_driver.egg-info/
--rw-rw-rw-   0        0        0     5709 2023-06-07 08:15:36.000000 flutter-driver-1.0.1/flutter_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-07 08:15:36.000000 flutter-driver-1.0.1/flutter_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 08:15:36.000000 flutter-driver-1.0.1/flutter_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 08:15:36.000000 flutter-driver-1.0.1/flutter_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 08:15:36.524618 flutter-driver-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-06-07 08:13:57.000000 flutter-driver-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:24:43.374565 flutter-driver-1.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-05-04 06:13:55.000000 flutter-driver-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5709 2023-06-07 08:24:43.373573 flutter-driver-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4642 2023-06-07 07:44:09.000000 flutter-driver-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 08:24:43.361669 flutter-driver-1.0.2/flutter_driver/
+-rw-rw-rw-   0        0        0       79 2023-05-22 00:27:16.000000 flutter-driver-1.0.2/flutter_driver/__init__.py
+-rw-rw-rw-   0        0        0     5064 2023-06-07 06:48:20.000000 flutter-driver-1.0.2/flutter_driver/command.py
+-rw-rw-rw-   0        0        0     8385 2023-06-07 07:15:31.000000 flutter-driver-1.0.2/flutter_driver/driver.py
+-rw-rw-rw-   0        0        0     5935 2023-05-22 00:43:02.000000 flutter-driver-1.0.2/flutter_driver/jsonrpc.py
+-rw-rw-rw-   0        0        0     3003 2023-06-07 07:27:49.000000 flutter-driver-1.0.2/flutter_driver/runner.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:24:43.370597 flutter-driver-1.0.2/flutter_driver.egg-info/
+-rw-rw-rw-   0        0        0     5709 2023-06-07 08:24:43.000000 flutter-driver-1.0.2/flutter_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-07 08:24:43.000000 flutter-driver-1.0.2/flutter_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 08:24:43.000000 flutter-driver-1.0.2/flutter_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-07 08:24:43.000000 flutter-driver-1.0.2/flutter_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 08:24:43.375558 flutter-driver-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1384 2023-06-07 08:24:41.000000 flutter-driver-1.0.2/setup.py
```

### Comparing `flutter-driver-1.0.1/LICENSE.txt` & `flutter-driver-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flutter-driver-1.0.1/PKG-INFO` & `flutter-driver-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flutter-driver
-Version: 1.0.1
+Version: 1.0.2
 Summary: An flutter automation driver for python
 Home-page: https://github.com/183181731/flutter-driver
 Author: ndaeqa-wang
 Author-email: 183181731@qq.com
 License: MIT
 Keywords: flutter windows,python client,ui automation
 Platform: UNKNOWN
```

### Comparing `flutter-driver-1.0.1/README.md` & `flutter-driver-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flutter-driver-1.0.1/flutter_driver.egg-info/PKG-INFO` & `flutter-driver-1.0.2/flutter_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flutter-driver
-Version: 1.0.1
+Version: 1.0.2
 Summary: An flutter automation driver for python
 Home-page: https://github.com/183181731/flutter-driver
 Author: ndaeqa-wang
 Author-email: 183181731@qq.com
 License: MIT
 Keywords: flutter windows,python client,ui automation
 Platform: UNKNOWN
```

### Comparing `flutter-driver-1.0.1/setup.py` & `flutter-driver-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import io
 import os
 
 from setuptools import find_packages, setup
 
 setup(
     name='flutter-driver',
-    version='1.0.1',
+    version='1.0.2',
     description='An flutter automation driver for python',
     long_description=io.open(os.path.join(os.path.dirname('__file__'), 'README.md'), encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     keywords=[
         'flutter windows',
         'python client',
         'ui automation'
     ],
     author='ndaeqa-wang',
     author_email='183181731@qq.com',
     url='https://github.com/183181731/flutter-driver',
-    packages=find_packages(include=['flutter-driver*']),
+    packages=find_packages(include=['flutter_driver','tests']),
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

