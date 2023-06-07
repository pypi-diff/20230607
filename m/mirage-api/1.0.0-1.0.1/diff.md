# Comparing `tmp/mirage-api-1.0.0.tar.gz` & `tmp/mirage-api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirage-api-1.0.0.tar", last modified: Wed Jun  7 09:14:47 2023, max compression
+gzip compressed data, was "mirage-api-1.0.1.tar", last modified: Wed Jun  7 09:19:07 2023, max compression
```

## Comparing `mirage-api-1.0.0.tar` & `mirage-api-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:14:47.088295 mirage-api-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 09:14:34.000000 mirage-api-1.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-07 09:14:34.000000 mirage-api-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-07 09:14:34.000000 mirage-api-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-06-07 09:14:47.084295 mirage-api-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-06-07 09:14:34.000000 mirage-api-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:14:47.084295 mirage-api-1.0.0/mirage_api/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-07 09:14:34.000000 mirage-api-1.0.0/mirage_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:14:47.084295 mirage-api-1.0.0/mirage_api/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:14:34.000000 mirage-api-1.0.0/mirage_api/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-07 09:14:34.000000 mirage-api-1.0.0/mirage_api/resources/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-07 09:14:34.000000 mirage-api-1.0.0/mirage_api/resources/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:14:47.084295 mirage-api-1.0.0/mirage_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-06-07 09:14:47.000000 mirage-api-1.0.0/mirage_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-07 09:14:47.000000 mirage-api-1.0.0/mirage_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:14:47.000000 mirage-api-1.0.0/mirage_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:14:47.000000 mirage-api-1.0.0/mirage_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 09:14:47.000000 mirage-api-1.0.0/mirage_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:14:47.088295 mirage-api-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-07 09:14:34.000000 mirage-api-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:19:07.754032 mirage-api-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 09:18:57.000000 mirage-api-1.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-07 09:18:57.000000 mirage-api-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-07 09:18:57.000000 mirage-api-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-06-07 09:19:07.754032 mirage-api-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-06-07 09:18:57.000000 mirage-api-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:19:07.754032 mirage-api-1.0.1/mirage_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-07 09:18:57.000000 mirage-api-1.0.1/mirage_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:19:07.754032 mirage-api-1.0.1/mirage_api/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:18:57.000000 mirage-api-1.0.1/mirage_api/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-07 09:18:57.000000 mirage-api-1.0.1/mirage_api/resources/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-07 09:18:57.000000 mirage-api-1.0.1/mirage_api/resources/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:19:07.754032 mirage-api-1.0.1/mirage_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-06-07 09:19:07.000000 mirage-api-1.0.1/mirage_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-07 09:19:07.000000 mirage-api-1.0.1/mirage_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:19:07.000000 mirage-api-1.0.1/mirage_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:19:07.000000 mirage-api-1.0.1/mirage_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 09:19:07.000000 mirage-api-1.0.1/mirage_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:19:07.754032 mirage-api-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-07 09:18:57.000000 mirage-api-1.0.1/setup.py
```

### Comparing `mirage-api-1.0.0/LICENSE` & `mirage-api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mirage-api-1.0.0/PKG-INFO` & `mirage-api-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirage-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Mirage API Python wrapper.
 Home-page: https://github.com/mirage-ai-com/python-mirage-api
 Author: Valerian Saliou
 Author-email: valerian@valeriansaliou.name
 License: MIT - http://opensource.org/licenses/mit-license.php
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `mirage-api-1.0.0/README.md` & `mirage-api-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mirage-api-1.0.0/mirage_api/__init__.py` & `mirage-api-1.0.1/mirage_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     # Convert data to body string
     body = str(json.dumps(data)).encode("utf-8")
 
     # Generate request headers
     headers = {
       "Content-Type": "application/json",
-      "User-Agent": "python-mirage-api/1.0.0",
+      "User-Agent": "python-mirage-api/1.0.1",
       "Authorization": self.__generate_auth()
     }
 
     # Open POST request
     req = request.Request(url, data=body, headers=headers, method="POST")
 
     try:
```

### Comparing `mirage-api-1.0.0/mirage_api/resources/task.py` & `mirage-api-1.0.1/mirage_api/resources/task.py`

 * *Files identical despite different names*

### Comparing `mirage-api-1.0.0/mirage_api.egg-info/PKG-INFO` & `mirage-api-1.0.1/mirage_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirage-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Mirage API Python wrapper.
 Home-page: https://github.com/mirage-ai-com/python-mirage-api
 Author: Valerian Saliou
 Author-email: valerian@valeriansaliou.name
 License: MIT - http://opensource.org/licenses/mit-license.php
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `mirage-api-1.0.0/setup.py` & `mirage-api-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 from distutils.core import setup
 from setuptools import find_packages
 
 
 setup(
     name='mirage-api',
-    version='1.0.0',
+    version='1.0.1',
     author=u'Valerian Saliou',
     author_email='valerian@valeriansaliou.name',
     packages=find_packages(),
     include_package_data=True,
     url='https://github.com/mirage-ai-com/python-mirage-api',
     license='MIT - http://opensource.org/licenses/mit-license.php',
     description='Mirage API Python wrapper.',
     long_description=open('README.md').read(),
-    long_description_content_type="text/markdown",
+    long_description_content_type='text/markdown',
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Programming Language :: Python',
     ],
     zip_safe=False,
```

