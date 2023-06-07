# Comparing `tmp/auto_route-0.1.2.tar.gz` & `tmp/auto_route-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_route-0.1.2.tar", last modified: Wed Jun  7 00:18:59 2023, max compression
+gzip compressed data, was "auto_route-0.1.3.tar", last modified: Wed Jun  7 00:19:47 2023, max compression
```

## Comparing `auto_route-0.1.2.tar` & `auto_route-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:18:59.196745 auto_route-0.1.2/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4980 2023-06-07 00:18:59.196745 auto_route-0.1.2/PKG-INFO
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4582 2023-06-06 23:59:56.000000 auto_route-0.1.2/README.rst
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:18:59.192745 auto_route-0.1.2/auto_app/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:09:47.000000 auto_route-0.1.2/auto_app/__init__.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     3736 2023-06-07 00:18:29.000000 auto_route-0.1.2/auto_app/auto_app.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     1608 2023-05-25 16:57:12.000000 auto_route-0.1.2/auto_app/cli_auto_app.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      779 2023-05-25 16:57:12.000000 auto_route-0.1.2/auto_app/streamlit_demo.py
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:18:59.192745 auto_route-0.1.2/auto_route/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-05-12 18:05:03.000000 auto_route-0.1.2/auto_route/__init__.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     7067 2023-05-25 21:33:21.000000 auto_route-0.1.2/auto_route/auto_route.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     2657 2023-05-23 23:28:52.000000 auto_route-0.1.2/auto_route/create_composed_class.py
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:18:59.192745 auto_route-0.1.2/auto_route.egg-info/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4980 2023-06-07 00:18:59.000000 auto_route-0.1.2/auto_route.egg-info/PKG-INFO
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      366 2023-06-07 00:18:59.000000 auto_route-0.1.2/auto_route.egg-info/SOURCES.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        1 2023-06-07 00:18:59.000000 auto_route-0.1.2/auto_route.egg-info/dependency_links.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       17 2023-06-07 00:18:59.000000 auto_route-0.1.2/auto_route.egg-info/requires.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       20 2023-06-07 00:18:59.000000 auto_route-0.1.2/auto_route.egg-info/top_level.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       38 2023-06-07 00:18:59.196745 auto_route-0.1.2/setup.cfg
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      674 2023-06-07 00:18:52.000000 auto_route-0.1.2/setup.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:19:47.732470 auto_route-0.1.3/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     4980 2023-06-07 00:19:47.732470 auto_route-0.1.3/PKG-INFO
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     4582 2023-06-06 23:59:56.000000 auto_route-0.1.3/README.rst
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:19:47.732470 auto_route-0.1.3/auto_app/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:09:47.000000 auto_route-0.1.3/auto_app/__init__.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     3725 2023-06-07 00:19:44.000000 auto_route-0.1.3/auto_app/auto_app.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     1608 2023-05-25 16:57:12.000000 auto_route-0.1.3/auto_app/cli_auto_app.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      779 2023-05-25 16:57:12.000000 auto_route-0.1.3/auto_app/streamlit_demo.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:19:47.732470 auto_route-0.1.3/auto_route/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-05-12 18:05:03.000000 auto_route-0.1.3/auto_route/__init__.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     7067 2023-05-25 21:33:21.000000 auto_route-0.1.3/auto_route/auto_route.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     2657 2023-05-23 23:28:52.000000 auto_route-0.1.3/auto_route/create_composed_class.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:19:47.732470 auto_route-0.1.3/auto_route.egg-info/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     4980 2023-06-07 00:19:47.000000 auto_route-0.1.3/auto_route.egg-info/PKG-INFO
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      366 2023-06-07 00:19:47.000000 auto_route-0.1.3/auto_route.egg-info/SOURCES.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        1 2023-06-07 00:19:47.000000 auto_route-0.1.3/auto_route.egg-info/dependency_links.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       17 2023-06-07 00:19:47.000000 auto_route-0.1.3/auto_route.egg-info/requires.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       20 2023-06-07 00:19:47.000000 auto_route-0.1.3/auto_route.egg-info/top_level.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       38 2023-06-07 00:19:47.732470 auto_route-0.1.3/setup.cfg
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      674 2023-06-07 00:19:44.000000 auto_route-0.1.3/setup.py
```

### Comparing `auto_route-0.1.2/PKG-INFO` & `auto_route-0.1.3/auto_route.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: auto_route
-Version: 0.1.2
+Name: auto-route
+Version: 0.1.3
 Summary: Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
 Home-page: http://github.com/yourname/auto_route
 Author: Ruben Fernandez
 Author-email: ruben@carbonyl.org
 Description-Content-Type: text/x-rst
 
 Contributing to the AutoRoute Project
```

### Comparing `auto_route-0.1.2/README.rst` & `auto_route-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.2/auto_app/auto_app.py` & `auto_route-0.1.3/auto_app/auto_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 class APIAutoApp:
     def __init__(self, routers_list: List[APIRouter and str] = None):
         self.routers_list = routers_list
 
     def load_routers_to_app(self, app: FastAPI, routers) -> None:
 
         for router in routers:
-            from auto_route.auto_route.auto_route import APIAutoRouter
+            from auto_route.auto_route import APIAutoRouter
             if isinstance(router, AutoLoadRouterConfigObject):
                 # fixme relative paths
                 module_path = router.module_path.replace(".py", "").replace("/", ".")
                 current_dir = os.path.dirname(__file__)
                 parent_dir = os.path.abspath(os.path.join(current_dir, os.pardir))
                 # path_to_add = os.path.abspath(os.path.join(current_dir, module_path))
                 sys.path.insert(0, parent_dir)
```

### Comparing `auto_route-0.1.2/auto_app/cli_auto_app.py` & `auto_route-0.1.3/auto_app/cli_auto_app.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.2/auto_app/streamlit_demo.py` & `auto_route-0.1.3/auto_app/streamlit_demo.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.2/auto_route/auto_route.py` & `auto_route-0.1.3/auto_route/auto_route.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.2/auto_route/create_composed_class.py` & `auto_route-0.1.3/auto_route/create_composed_class.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.2/auto_route.egg-info/PKG-INFO` & `auto_route-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: auto-route
-Version: 0.1.2
+Name: auto_route
+Version: 0.1.3
 Summary: Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
 Home-page: http://github.com/yourname/auto_route
 Author: Ruben Fernandez
 Author-email: ruben@carbonyl.org
 Description-Content-Type: text/x-rst
 
 Contributing to the AutoRoute Project
```

### Comparing `auto_route-0.1.2/setup.py` & `auto_route-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='auto_route',
-    version='0.1.2',  # Semantic Versioning
+    version='0.1.3',  # Semantic Versioning
     packages=["auto_route", "auto_app"],
     author='Ruben Fernandez',
     author_email='ruben@carbonyl.org',
     description="Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and "
                 "automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.",
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
```

