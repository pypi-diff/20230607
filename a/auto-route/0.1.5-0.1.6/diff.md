# Comparing `tmp/auto_route-0.1.5.tar.gz` & `tmp/auto_route-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_route-0.1.5.tar", last modified: Wed Jun  7 00:33:16 2023, max compression
+gzip compressed data, was "auto_route-0.1.6.tar", last modified: Wed Jun  7 00:45:01 2023, max compression
```

## Comparing `auto_route-0.1.5.tar` & `auto_route-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:33:16.795373 auto_route-0.1.5/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4983 2023-06-07 00:33:16.795373 auto_route-0.1.5/PKG-INFO
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4582 2023-06-06 23:59:56.000000 auto_route-0.1.5/README.rst
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:33:16.795373 auto_route-0.1.5/auto_app/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:09:47.000000 auto_route-0.1.5/auto_app/__init__.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     3725 2023-06-07 00:19:44.000000 auto_route-0.1.5/auto_app/auto_app.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     1608 2023-05-25 16:57:12.000000 auto_route-0.1.5/auto_app/cli_auto_app.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      779 2023-05-25 16:57:12.000000 auto_route-0.1.5/auto_app/streamlit_demo.py
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:33:16.795373 auto_route-0.1.5/auto_route/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-05-12 18:05:03.000000 auto_route-0.1.5/auto_route/__init__.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     7067 2023-05-25 21:33:21.000000 auto_route-0.1.5/auto_route/auto_route.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     2657 2023-05-23 23:28:52.000000 auto_route-0.1.5/auto_route/create_composed_class.py
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:33:16.795373 auto_route-0.1.5/auto_route.egg-info/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4983 2023-06-07 00:33:16.000000 auto_route-0.1.5/auto_route.egg-info/PKG-INFO
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      366 2023-06-07 00:33:16.000000 auto_route-0.1.5/auto_route.egg-info/SOURCES.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        1 2023-06-07 00:33:16.000000 auto_route-0.1.5/auto_route.egg-info/dependency_links.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       25 2023-06-07 00:33:16.000000 auto_route-0.1.5/auto_route.egg-info/requires.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       20 2023-06-07 00:33:16.000000 auto_route-0.1.5/auto_route.egg-info/top_level.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       38 2023-06-07 00:33:16.795373 auto_route-0.1.5/setup.cfg
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      696 2023-06-07 00:29:35.000000 auto_route-0.1.5/setup.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:45:01.110287 auto_route-0.1.6/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)    35149 2023-06-07 00:39:57.000000 auto_route-0.1.6/LICENSE
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     5005 2023-06-07 00:45:01.110287 auto_route-0.1.6/PKG-INFO
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     4582 2023-06-07 00:39:57.000000 auto_route-0.1.6/README.rst
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:45:01.110287 auto_route-0.1.6/auto_app/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_app/__init__.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     3725 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_app/auto_app.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     1608 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_app/cli_auto_app.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      779 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_app/streamlit_demo.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:45:01.110287 auto_route-0.1.6/auto_route/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_route/__init__.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     7067 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_route/auto_route.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     2657 2023-06-07 00:39:57.000000 auto_route-0.1.6/auto_route/create_composed_class.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      349 2023-05-21 20:56:14.000000 auto_route-0.1.6/auto_route/generator.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:45:01.110287 auto_route-0.1.6/auto_route.egg-info/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     5005 2023-06-07 00:45:01.000000 auto_route-0.1.6/auto_route.egg-info/PKG-INFO
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      398 2023-06-07 00:45:01.000000 auto_route-0.1.6/auto_route.egg-info/SOURCES.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        1 2023-06-07 00:45:01.000000 auto_route-0.1.6/auto_route.egg-info/dependency_links.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       25 2023-06-07 00:45:01.000000 auto_route-0.1.6/auto_route.egg-info/requires.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       20 2023-06-07 00:45:01.000000 auto_route-0.1.6/auto_route.egg-info/top_level.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       38 2023-06-07 00:45:01.110287 auto_route-0.1.6/setup.cfg
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      696 2023-06-07 00:44:58.000000 auto_route-0.1.6/setup.py
```

### Comparing `auto_route-0.1.5/PKG-INFO` & `auto_route-0.1.6/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: auto_route
-Version: 0.1.5
-Summary: Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
-Home-page: https://github.com/Bucanero06/auto_route
-Author: Ruben Fernandez
-Author-email: ruben@carbonyl.org
-Description-Content-Type: text/x-rst
-
 Contributing to the AutoRoute Project
 =====================================
 
 Introduction
 ------------
 
 Thank you for your interest in contributing to the AutoRoute project!
```

### Comparing `auto_route-0.1.5/README.rst` & `auto_route-0.1.6/auto_route.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: auto-route
+Version: 0.1.6
+Summary: Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
+Home-page: https://github.com/Bucanero06/auto_route
+Author: Ruben Fernandez
+Author-email: ruben@carbonyl.org
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 Contributing to the AutoRoute Project
 =====================================
 
 Introduction
 ------------
 
 Thank you for your interest in contributing to the AutoRoute project!
```

### Comparing `auto_route-0.1.5/auto_app/auto_app.py` & `auto_route-0.1.6/auto_app/auto_app.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.5/auto_app/cli_auto_app.py` & `auto_route-0.1.6/auto_app/cli_auto_app.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.5/auto_app/streamlit_demo.py` & `auto_route-0.1.6/auto_app/streamlit_demo.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.5/auto_route/auto_route.py` & `auto_route-0.1.6/auto_route/auto_route.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.5/auto_route/create_composed_class.py` & `auto_route-0.1.6/auto_route/create_composed_class.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.5/auto_route.egg-info/PKG-INFO` & `auto_route-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: auto-route
-Version: 0.1.5
+Name: auto_route
+Version: 0.1.6
 Summary: Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
 Home-page: https://github.com/Bucanero06/auto_route
 Author: Ruben Fernandez
 Author-email: ruben@carbonyl.org
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 
 Contributing to the AutoRoute Project
 =====================================
 
 Introduction
 ------------
```

### Comparing `auto_route-0.1.5/setup.py` & `auto_route-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='auto_route',
-    version='0.1.5',  # Semantic Versioning
+    version='0.1.6',  # Semantic Versioning
     packages=["auto_route", "auto_app"],
     author='Ruben Fernandez',
     author_email='ruben@carbonyl.org',
     description="Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and "
                 "automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.",
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
```

