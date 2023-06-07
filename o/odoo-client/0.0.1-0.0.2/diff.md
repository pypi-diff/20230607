# Comparing `tmp/odoo_client-0.0.1.tar.gz` & `tmp/odoo_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_client-0.0.1.tar", last modified: Wed Jun  7 13:28:14 2023, max compression
+gzip compressed data, was "odoo_client-0.0.2.tar", last modified: Wed Jun  7 13:54:48 2023, max compression
```

## Comparing `odoo_client-0.0.1.tar` & `odoo_client-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 13:28:14.508564 odoo_client-0.0.1/
--rw-r--r--   0 mfarwell   (501) staff       (20)      474 2023-06-07 13:28:14.508465 odoo_client-0.0.1/PKG-INFO
-drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 13:28:14.507865 odoo_client-0.0.1/odoo_client/
--rw-r--r--   0 mfarwell   (501) staff       (20)      157 2023-06-07 13:20:34.000000 odoo_client-0.0.1/odoo_client/__init__.py
--rw-r--r--   0 mfarwell   (501) staff       (20)     1237 2023-06-07 13:19:29.000000 odoo_client-0.0.1/odoo_client/client.py
--rw-r--r--   0 mfarwell   (501) staff       (20)     1615 2023-06-07 13:19:29.000000 odoo_client-0.0.1/odoo_client/model.py
--rw-r--r--   0 mfarwell   (501) staff       (20)     5255 2023-06-07 13:19:05.000000 odoo_client-0.0.1/odoo_client/object.py
-drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 13:28:14.508328 odoo_client-0.0.1/odoo_client.egg-info/
--rw-r--r--   0 mfarwell   (501) staff       (20)      474 2023-06-07 13:28:14.000000 odoo_client-0.0.1/odoo_client.egg-info/PKG-INFO
--rw-r--r--   0 mfarwell   (501) staff       (20)      237 2023-06-07 13:28:14.000000 odoo_client-0.0.1/odoo_client.egg-info/SOURCES.txt
--rw-r--r--   0 mfarwell   (501) staff       (20)        1 2023-06-07 13:28:14.000000 odoo_client-0.0.1/odoo_client.egg-info/dependency_links.txt
--rw-r--r--   0 mfarwell   (501) staff       (20)       12 2023-06-07 13:28:14.000000 odoo_client-0.0.1/odoo_client.egg-info/top_level.txt
--rw-r--r--   0 mfarwell   (501) staff       (20)       38 2023-06-07 13:28:14.508595 odoo_client-0.0.1/setup.cfg
--rw-r--r--   0 mfarwell   (501) staff       (20)      731 2023-06-07 13:26:38.000000 odoo_client-0.0.1/setup.py
+drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 13:54:48.804886 odoo_client-0.0.2/
+-rw-r--r--   0 mfarwell   (501) staff       (20)      372 2023-06-07 13:54:48.804789 odoo_client-0.0.2/PKG-INFO
+-rw-r--r--   0 mfarwell   (501) staff       (20)       17 2023-06-07 13:48:35.000000 odoo_client-0.0.2/README.md
+drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 13:54:48.804277 odoo_client-0.0.2/odoo_client/
+-rw-r--r--   0 mfarwell   (501) staff       (20)       62 2023-06-07 13:52:51.000000 odoo_client-0.0.2/odoo_client/__init__.py
+-rw-r--r--   0 mfarwell   (501) staff       (20)     1237 2023-06-07 13:19:29.000000 odoo_client-0.0.2/odoo_client/client.py
+-rw-r--r--   0 mfarwell   (501) staff       (20)     1615 2023-06-07 13:19:29.000000 odoo_client-0.0.2/odoo_client/model.py
+-rw-r--r--   0 mfarwell   (501) staff       (20)     5255 2023-06-07 13:19:05.000000 odoo_client-0.0.2/odoo_client/object.py
+drwxr-xr-x   0 mfarwell   (501) staff       (20)        0 2023-06-07 13:54:48.804669 odoo_client-0.0.2/odoo_client.egg-info/
+-rw-r--r--   0 mfarwell   (501) staff       (20)      372 2023-06-07 13:54:48.000000 odoo_client-0.0.2/odoo_client.egg-info/PKG-INFO
+-rw-r--r--   0 mfarwell   (501) staff       (20)      247 2023-06-07 13:54:48.000000 odoo_client-0.0.2/odoo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mfarwell   (501) staff       (20)        1 2023-06-07 13:54:48.000000 odoo_client-0.0.2/odoo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mfarwell   (501) staff       (20)       12 2023-06-07 13:54:48.000000 odoo_client-0.0.2/odoo_client.egg-info/top_level.txt
+-rw-r--r--   0 mfarwell   (501) staff       (20)       38 2023-06-07 13:54:48.804912 odoo_client-0.0.2/setup.cfg
+-rw-r--r--   0 mfarwell   (501) staff       (20)      632 2023-06-07 13:54:42.000000 odoo_client-0.0.2/setup.py
```

### Comparing `odoo_client-0.0.1/odoo_client/client.py` & `odoo_client-0.0.2/odoo_client/client.py`

 * *Files identical despite different names*

### Comparing `odoo_client-0.0.1/odoo_client/model.py` & `odoo_client-0.0.2/odoo_client/model.py`

 * *Files identical despite different names*

### Comparing `odoo_client-0.0.1/odoo_client/object.py` & `odoo_client-0.0.2/odoo_client/object.py`

 * *Files identical despite different names*

