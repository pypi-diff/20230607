# Comparing `tmp/odoo_client-0.0.2.tar.gz` & `tmp/odoo_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_client-0.0.2.tar", last modified: Wed Jun  7 13:54:48 2023, max compression
+gzip compressed data, was "odoo_client-0.0.3.tar", last modified: Wed Jun  7 14:28:41 2023, max compression
```

## Comparing `odoo_client-0.0.2.tar` & `odoo_client-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 13:54:48.804886 odoo_client-0.0.2/
--rw-r--r--   0 mfarwell   (501) staff       (20)      372 2023-06-07 13:54:48.804789 odoo_client-0.0.2/PKG-INFO
--rw-r--r--   0 mfarwell   (501) staff       (20)       17 2023-06-07 13:48:35.000000 odoo_client-0.0.2/README.md
-drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 13:54:48.804277 odoo_client-0.0.2/odoo_client/
--rw-r--r--   0 mfarwell   (501) staff       (20)       62 2023-06-07 13:52:51.000000 odoo_client-0.0.2/odoo_client/__init__.py
--rw-r--r--   0 mfarwell   (501) staff       (20)     1237 2023-06-07 13:19:29.000000 odoo_client-0.0.2/odoo_client/client.py
--rw-r--r--   0 mfarwell   (501) staff       (20)     1615 2023-06-07 13:19:29.000000 odoo_client-0.0.2/odoo_client/model.py
--rw-r--r--   0 mfarwell   (501) staff       (20)     5255 2023-06-07 13:19:05.000000 odoo_client-0.0.2/odoo_client/object.py
-drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 13:54:48.804669 odoo_client-0.0.2/odoo_client.egg-info/
--rw-r--r--   0 mfarwell   (501) staff       (20)      372 2023-06-07 13:54:48.000000 odoo_client-0.0.2/odoo_client.egg-info/PKG-INFO
--rw-r--r--   0 mfarwell   (501) staff       (20)      247 2023-06-07 13:54:48.000000 odoo_client-0.0.2/odoo_client.egg-info/SOURCES.txt
--rw-r--r--   0 mfarwell   (501) staff       (20)        1 2023-06-07 13:54:48.000000 odoo_client-0.0.2/odoo_client.egg-info/dependency_links.txt
--rw-r--r--   0 mfarwell   (501) staff       (20)       12 2023-06-07 13:54:48.000000 odoo_client-0.0.2/odoo_client.egg-info/top_level.txt
--rw-r--r--   0 mfarwell   (501) staff       (20)       38 2023-06-07 13:54:48.804912 odoo_client-0.0.2/setup.cfg
--rw-r--r--   0 mfarwell   (501) staff       (20)      632 2023-06-07 13:54:42.000000 odoo_client-0.0.2/setup.py
+drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 14:28:41.594950 odoo_client-0.0.3/
+-rw-r--r--   0 mfarwell   (501) staff       (20)     1078 2023-06-07 14:18:19.000000 odoo_client-0.0.3/LICENSE
+-rw-r--r--   0 mfarwell   (501) staff       (20)      445 2023-06-07 14:28:41.594853 odoo_client-0.0.3/PKG-INFO
+-rw-r--r--   0 mfarwell   (501) staff       (20)      743 2023-06-07 14:28:04.000000 odoo_client-0.0.3/README.md
+drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 14:28:41.594312 odoo_client-0.0.3/odoo_client/
+-rw-r--r--   0 mfarwell   (501) staff       (20)       62 2023-06-07 13:52:51.000000 odoo_client-0.0.3/odoo_client/__init__.py
+-rw-r--r--   0 mfarwell   (501) staff       (20)     1237 2023-06-07 13:19:29.000000 odoo_client-0.0.3/odoo_client/client.py
+-rw-r--r--   0 mfarwell   (501) staff       (20)     1615 2023-06-07 13:19:29.000000 odoo_client-0.0.3/odoo_client/model.py
+-rw-r--r--   0 mfarwell   (501) staff       (20)     5255 2023-06-07 13:19:05.000000 odoo_client-0.0.3/odoo_client/object.py
+drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 14:28:41.594714 odoo_client-0.0.3/odoo_client.egg-info/
+-rw-r--r--   0 mfarwell   (501) staff       (20)      445 2023-06-07 14:28:41.000000 odoo_client-0.0.3/odoo_client.egg-info/PKG-INFO
+-rw-r--r--   0 mfarwell   (501) staff       (20)      255 2023-06-07 14:28:41.000000 odoo_client-0.0.3/odoo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mfarwell   (501) staff       (20)        1 2023-06-07 14:28:41.000000 odoo_client-0.0.3/odoo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mfarwell   (501) staff       (20)       12 2023-06-07 14:28:41.000000 odoo_client-0.0.3/odoo_client.egg-info/top_level.txt
+-rw-r--r--   0 mfarwell   (501) staff       (20)       38 2023-06-07 14:28:41.594979 odoo_client-0.0.3/setup.cfg
+-rw-r--r--   0 mfarwell   (501) staff       (20)      683 2023-06-07 14:05:30.000000 odoo_client-0.0.3/setup.py
```

### Comparing `odoo_client-0.0.2/odoo_client/client.py` & `odoo_client-0.0.3/odoo_client/client.py`

 * *Files identical despite different names*

### Comparing `odoo_client-0.0.2/odoo_client/model.py` & `odoo_client-0.0.3/odoo_client/model.py`

 * *Files identical despite different names*

### Comparing `odoo_client-0.0.2/odoo_client/object.py` & `odoo_client-0.0.3/odoo_client/object.py`

 * *Files identical despite different names*

### Comparing `odoo_client-0.0.2/setup.py` & `odoo_client-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "Simple API wrapper for Odoo's External API"
 LONG_DESCRIPTION = "Simple API wrapper for Odoo's External API"
 
 setup(
     name="odoo_client",
     version=VERSION,
     author="Michael Farwell",
     author_email="mike@lie-nielsen.com",
+    url="https://github.com/LNTW/odoo-python-api",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=["python", "odoo", "api"],
     classifiers=[
         "Development Status :: 3 - Alpha",
```

