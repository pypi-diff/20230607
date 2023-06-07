# Comparing `tmp/monday_sdk-0.1.0.tar.gz` & `tmp/monday_sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monday_sdk-0.1.0.tar", max compression
+gzip compressed data, was "monday_sdk-1.0.0.tar", max compression
```

## Comparing `monday_sdk-0.1.0.tar` & `monday_sdk-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-08 16:00:48.272318 monday_sdk-0.1.0/monday_sdk/__init__.py
--rw-r--r--   0        0        0     2239 2023-06-07 00:14:15.237710 monday_sdk-0.1.0/monday_sdk/authentication.py
--rw-r--r--   0        0        0      514 2023-06-07 00:14:23.454810 monday_sdk-0.1.0/monday_sdk/graphql_loader.py
--rw-r--r--   0        0        0     3031 2023-06-07 00:14:49.820809 monday_sdk-0.1.0/monday_sdk/monday.py
--rw-r--r--   0        0        0      327 2023-06-07 00:19:09.179256 monday_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       29 2023-06-07 00:12:01.661191 monday_sdk-0.1.0/README.md
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 monday_sdk-0.1.0/setup.py
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 monday_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-08 16:00:48.272318 monday_sdk-1.0.0/monday_sdk/__init__.py
+-rw-r--r--   0        0        0     2239 2023-06-07 00:14:15.237710 monday_sdk-1.0.0/monday_sdk/authentication.py
+-rw-r--r--   0        0        0      514 2023-06-07 00:14:23.454810 monday_sdk-1.0.0/monday_sdk/graphql_loader.py
+-rw-r--r--   0        0        0     3031 2023-06-07 00:14:49.820809 monday_sdk-1.0.0/monday_sdk/monday.py
+-rw-r--r--   0        0        0      327 2023-06-07 00:20:02.572906 monday_sdk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-06-07 00:12:01.661191 monday_sdk-1.0.0/README.md
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 monday_sdk-1.0.0/setup.py
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 monday_sdk-1.0.0/PKG-INFO
```

### Comparing `monday_sdk-0.1.0/monday_sdk/authentication.py` & `monday_sdk-1.0.0/monday_sdk/authentication.py`

 * *Files identical despite different names*

### Comparing `monday_sdk-0.1.0/monday_sdk/graphql_loader.py` & `monday_sdk-1.0.0/monday_sdk/graphql_loader.py`

 * *Files identical despite different names*

### Comparing `monday_sdk-0.1.0/monday_sdk/monday.py` & `monday_sdk-1.0.0/monday_sdk/monday.py`

 * *Files identical despite different names*

### Comparing `monday_sdk-0.1.0/setup.py` & `monday_sdk-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['fastapi>=0.88.0,<0.89.0', 'pendulum>=2.1.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'monday-sdk',
-    'version': '0.1.0',
+    'version': '1.0.0',
     'description': '',
     'long_description': '# Python SDK for monday.com\n',
     'author': 'Jonathan Crum',
     'author_email': 'jcrum@theobogroup.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

