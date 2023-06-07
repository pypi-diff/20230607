# Comparing `tmp/auto_route-0.1.4.tar.gz` & `tmp/auto_route-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_route-0.1.4.tar", last modified: Wed Jun  7 00:21:54 2023, max compression
+gzip compressed data, was "auto_route-0.1.5.tar", last modified: Wed Jun  7 00:33:16 2023, max compression
```

## Comparing `auto_route-0.1.4.tar` & `auto_route-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:21:54.811912 auto_route-0.1.4/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4980 2023-06-07 00:21:54.811912 auto_route-0.1.4/PKG-INFO
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4582 2023-06-06 23:59:56.000000 auto_route-0.1.4/README.rst
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:21:54.811912 auto_route-0.1.4/auto_app/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:09:47.000000 auto_route-0.1.4/auto_app/__init__.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     3725 2023-06-07 00:19:44.000000 auto_route-0.1.4/auto_app/auto_app.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     1608 2023-05-25 16:57:12.000000 auto_route-0.1.4/auto_app/cli_auto_app.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      779 2023-05-25 16:57:12.000000 auto_route-0.1.4/auto_app/streamlit_demo.py
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:21:54.811912 auto_route-0.1.4/auto_route/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-05-12 18:05:03.000000 auto_route-0.1.4/auto_route/__init__.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     7067 2023-05-25 21:33:21.000000 auto_route-0.1.4/auto_route/auto_route.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     2657 2023-05-23 23:28:52.000000 auto_route-0.1.4/auto_route/create_composed_class.py
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:21:54.811912 auto_route-0.1.4/auto_route.egg-info/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4980 2023-06-07 00:21:54.000000 auto_route-0.1.4/auto_route.egg-info/PKG-INFO
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      366 2023-06-07 00:21:54.000000 auto_route-0.1.4/auto_route.egg-info/SOURCES.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        1 2023-06-07 00:21:54.000000 auto_route-0.1.4/auto_route.egg-info/dependency_links.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       25 2023-06-07 00:21:54.000000 auto_route-0.1.4/auto_route.egg-info/requires.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       20 2023-06-07 00:21:54.000000 auto_route-0.1.4/auto_route.egg-info/top_level.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       38 2023-06-07 00:21:54.811912 auto_route-0.1.4/setup.cfg
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      693 2023-06-07 00:21:52.000000 auto_route-0.1.4/setup.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:33:16.795373 auto_route-0.1.5/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     4983 2023-06-07 00:33:16.795373 auto_route-0.1.5/PKG-INFO
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     4582 2023-06-06 23:59:56.000000 auto_route-0.1.5/README.rst
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:33:16.795373 auto_route-0.1.5/auto_app/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:09:47.000000 auto_route-0.1.5/auto_app/__init__.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     3725 2023-06-07 00:19:44.000000 auto_route-0.1.5/auto_app/auto_app.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     1608 2023-05-25 16:57:12.000000 auto_route-0.1.5/auto_app/cli_auto_app.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      779 2023-05-25 16:57:12.000000 auto_route-0.1.5/auto_app/streamlit_demo.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:33:16.795373 auto_route-0.1.5/auto_route/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-05-12 18:05:03.000000 auto_route-0.1.5/auto_route/__init__.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     7067 2023-05-25 21:33:21.000000 auto_route-0.1.5/auto_route/auto_route.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     2657 2023-05-23 23:28:52.000000 auto_route-0.1.5/auto_route/create_composed_class.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:33:16.795373 auto_route-0.1.5/auto_route.egg-info/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     4983 2023-06-07 00:33:16.000000 auto_route-0.1.5/auto_route.egg-info/PKG-INFO
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      366 2023-06-07 00:33:16.000000 auto_route-0.1.5/auto_route.egg-info/SOURCES.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        1 2023-06-07 00:33:16.000000 auto_route-0.1.5/auto_route.egg-info/dependency_links.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       25 2023-06-07 00:33:16.000000 auto_route-0.1.5/auto_route.egg-info/requires.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       20 2023-06-07 00:33:16.000000 auto_route-0.1.5/auto_route.egg-info/top_level.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       38 2023-06-07 00:33:16.795373 auto_route-0.1.5/setup.cfg
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      696 2023-06-07 00:29:35.000000 auto_route-0.1.5/setup.py
```

### Comparing `auto_route-0.1.4/PKG-INFO` & `auto_route-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: auto_route
-Version: 0.1.4
+Version: 0.1.5
 Summary: Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
-Home-page: http://github.com/yourname/auto_route
+Home-page: https://github.com/Bucanero06/auto_route
 Author: Ruben Fernandez
 Author-email: ruben@carbonyl.org
 Description-Content-Type: text/x-rst
 
 Contributing to the AutoRoute Project
 =====================================
```

### Comparing `auto_route-0.1.4/README.rst` & `auto_route-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.4/auto_app/auto_app.py` & `auto_route-0.1.5/auto_app/auto_app.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.4/auto_app/cli_auto_app.py` & `auto_route-0.1.5/auto_app/cli_auto_app.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.4/auto_app/streamlit_demo.py` & `auto_route-0.1.5/auto_app/streamlit_demo.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.4/auto_route/auto_route.py` & `auto_route-0.1.5/auto_route/auto_route.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.4/auto_route/create_composed_class.py` & `auto_route-0.1.5/auto_route/create_composed_class.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.4/auto_route.egg-info/PKG-INFO` & `auto_route-0.1.5/auto_route.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: auto-route
-Version: 0.1.4
+Version: 0.1.5
 Summary: Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
-Home-page: http://github.com/yourname/auto_route
+Home-page: https://github.com/Bucanero06/auto_route
 Author: Ruben Fernandez
 Author-email: ruben@carbonyl.org
 Description-Content-Type: text/x-rst
 
 Contributing to the AutoRoute Project
 =====================================
```

### Comparing `auto_route-0.1.4/setup.py` & `auto_route-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='auto_route',
-    version='0.1.4',  # Semantic Versioning
+    version='0.1.5',  # Semantic Versioning
     packages=["auto_route", "auto_app"],
     author='Ruben Fernandez',
     author_email='ruben@carbonyl.org',
     description="Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and "
                 "automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.",
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
-    url='http://github.com/yourname/auto_route',
+    url='https://github.com/Bucanero06/auto_route',
     install_requires=[
         "fastapi",
         "pydantic",
         "uvicorn",
     ],
 )
```

