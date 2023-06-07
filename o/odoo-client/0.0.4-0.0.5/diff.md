# Comparing `tmp/odoo_client-0.0.4.tar.gz` & `tmp/odoo_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_client-0.0.4.tar", last modified: Wed Jun  7 14:51:32 2023, max compression
+gzip compressed data, was "odoo_client-0.0.5.tar", last modified: Wed Jun  7 15:03:32 2023, max compression
```

## Comparing `odoo_client-0.0.4.tar` & `odoo_client-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 14:51:32.400477 odoo_client-0.0.4/
--rw-r--r--   0 mfarwell   (501) staff       (20)     1078 2023-06-07 14:18:19.000000 odoo_client-0.0.4/LICENSE
--rw-r--r--   0 mfarwell   (501) staff       (20)     1289 2023-06-07 14:51:32.400360 odoo_client-0.0.4/PKG-INFO
--rw-r--r--   0 mfarwell   (501) staff       (20)      743 2023-06-07 14:28:04.000000 odoo_client-0.0.4/README.md
-drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 14:51:32.396719 odoo_client-0.0.4/odoo_client/
--rw-r--r--   0 mfarwell   (501) staff       (20)       62 2023-06-07 13:52:51.000000 odoo_client-0.0.4/odoo_client/__init__.py
--rw-r--r--   0 mfarwell   (501) staff       (20)     1237 2023-06-07 13:19:29.000000 odoo_client-0.0.4/odoo_client/client.py
--rw-r--r--   0 mfarwell   (501) staff       (20)     1615 2023-06-07 13:19:29.000000 odoo_client-0.0.4/odoo_client/model.py
--rw-r--r--   0 mfarwell   (501) staff       (20)     5255 2023-06-07 13:19:05.000000 odoo_client-0.0.4/odoo_client/object.py
-drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 14:51:32.400026 odoo_client-0.0.4/odoo_client.egg-info/
--rw-r--r--   0 mfarwell   (501) staff       (20)     1289 2023-06-07 14:51:32.000000 odoo_client-0.0.4/odoo_client.egg-info/PKG-INFO
--rw-r--r--   0 mfarwell   (501) staff       (20)      255 2023-06-07 14:51:32.000000 odoo_client-0.0.4/odoo_client.egg-info/SOURCES.txt
--rw-r--r--   0 mfarwell   (501) staff       (20)        1 2023-06-07 14:51:32.000000 odoo_client-0.0.4/odoo_client.egg-info/dependency_links.txt
--rw-r--r--   0 mfarwell   (501) staff       (20)       12 2023-06-07 14:51:32.000000 odoo_client-0.0.4/odoo_client.egg-info/top_level.txt
--rw-r--r--   0 mfarwell   (501) staff       (20)       38 2023-06-07 14:51:32.400516 odoo_client-0.0.4/setup.cfg
--rw-r--r--   0 mfarwell   (501) staff       (20)      876 2023-06-07 14:51:19.000000 odoo_client-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:03:32.987496 odoo_client-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-07 15:03:23.000000 odoo_client-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-07 15:03:32.987496 odoo_client-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-07 15:03:23.000000 odoo_client-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:03:32.983497 odoo_client-0.0.5/odoo_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 15:03:23.000000 odoo_client-0.0.5/odoo_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-07 15:03:23.000000 odoo_client-0.0.5/odoo_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-07 15:03:23.000000 odoo_client-0.0.5/odoo_client/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-07 15:03:23.000000 odoo_client-0.0.5/odoo_client/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:03:32.987496 odoo_client-0.0.5/odoo_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-07 15:03:32.000000 odoo_client-0.0.5/odoo_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-07 15:03:32.000000 odoo_client-0.0.5/odoo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:03:32.000000 odoo_client-0.0.5/odoo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 15:03:32.000000 odoo_client-0.0.5/odoo_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:03:32.987496 odoo_client-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-07 15:03:23.000000 odoo_client-0.0.5/setup.py
```

### Comparing `odoo_client-0.0.4/LICENSE` & `odoo_client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `odoo_client-0.0.4/PKG-INFO` & `odoo_client-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo_client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple API wrapper for Odoo's External API
 Home-page: https://github.com/LNTW/odoo-python-api
 Author: Michael Farwell
 Author-email: mike@lie-nielsen.com
 License: MIT
 Keywords: python,odoo,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `odoo_client-0.0.4/README.md` & `odoo_client-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `odoo_client-0.0.4/odoo_client/client.py` & `odoo_client-0.0.5/odoo_client/client.py`

 * *Files identical despite different names*

### Comparing `odoo_client-0.0.4/odoo_client/model.py` & `odoo_client-0.0.5/odoo_client/model.py`

 * *Files identical despite different names*

### Comparing `odoo_client-0.0.4/odoo_client/object.py` & `odoo_client-0.0.5/odoo_client/object.py`

 * *Files identical despite different names*

### Comparing `odoo_client-0.0.4/odoo_client.egg-info/PKG-INFO` & `odoo_client-0.0.5/odoo_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple API wrapper for Odoo's External API
 Home-page: https://github.com/LNTW/odoo-python-api
 Author: Michael Farwell
 Author-email: mike@lie-nielsen.com
 License: MIT
 Keywords: python,odoo,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `odoo_client-0.0.4/setup.py` & `odoo_client-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = "Simple API wrapper for Odoo's External API"
 LONG_DESCRIPTION = readme
 
 setup(
     name="odoo_client",
     version=VERSION,
     author="Michael Farwell",
```

