# Comparing `tmp/canonicalwebteam_store_api-4.1.0.tar.gz` & `tmp/canonicalwebteam_store_api-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canonicalwebteam_store_api-4.1.0.tar", max compression
+gzip compressed data, was "canonicalwebteam_store_api-4.2.0.tar", max compression
```

## Comparing `canonicalwebteam_store_api-4.1.0.tar` & `canonicalwebteam_store_api-4.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     7652 2023-03-16 14:06:20.876876 canonicalwebteam_store_api-4.1.0/LICENSE
--rw-r--r--   0        0        0     1430 2023-03-16 14:06:20.876876 canonicalwebteam_store_api-4.1.0/README.md
--rw-r--r--   0        0        0       65 2023-03-16 14:06:20.876876 canonicalwebteam_store_api-4.1.0/canonicalwebteam/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 14:06:20.876876 canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/__init__.py
--rw-r--r--   0        0        0     1517 2023-03-16 14:06:20.876876 canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/exceptions.py
--rw-r--r--   0        0        0    10632 2023-03-16 14:06:20.876876 canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/publisher.py
--rw-r--r--   0        0        0     7075 2023-03-16 14:06:20.880876 canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/store.py
--rw-r--r--   0        0        0        0 2023-03-16 14:06:20.880876 canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/stores/__init__.py
--rw-r--r--   0        0        0     9736 2023-03-16 14:06:20.880876 canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/stores/charmstore.py
--rw-r--r--   0        0        0    10172 2023-03-16 14:06:20.880876 canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/stores/snapstore.py
--rw-r--r--   0        0        0      493 2023-03-16 14:06:20.880876 canonicalwebteam_store_api-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     2213 1970-01-01 00:00:00.000000 canonicalwebteam_store_api-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-07 13:12:48.786214 canonicalwebteam_store_api-4.2.0/LICENSE
+-rw-r--r--   0        0        0     1430 2023-06-07 13:12:48.786214 canonicalwebteam_store_api-4.2.0/README.md
+-rw-r--r--   0        0        0       65 2023-06-07 13:12:48.786214 canonicalwebteam_store_api-4.2.0/canonicalwebteam/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:12:48.786214 canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/__init__.py
+-rw-r--r--   0        0        0     1517 2023-06-07 13:12:48.786214 canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/exceptions.py
+-rw-r--r--   0        0        0    10632 2023-06-07 13:12:48.786214 canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/publisher.py
+-rw-r--r--   0        0        0     7075 2023-06-07 13:12:48.786214 canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/store.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:12:48.786214 canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/stores/__init__.py
+-rw-r--r--   0        0        0     9736 2023-06-07 13:12:48.786214 canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/stores/charmstore.py
+-rw-r--r--   0        0        0    10193 2023-06-07 13:12:48.786214 canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/stores/snapstore.py
+-rw-r--r--   0        0        0      493 2023-06-07 13:12:48.790214 canonicalwebteam_store_api-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2213 1970-01-01 00:00:00.000000 canonicalwebteam_store_api-4.2.0/PKG-INFO
```

### Comparing `canonicalwebteam_store_api-4.1.0/LICENSE` & `canonicalwebteam_store_api-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.1.0/README.md` & `canonicalwebteam_store_api-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/exceptions.py` & `canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/publisher.py` & `canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/publisher.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/store.py` & `canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/store.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/stores/charmstore.py` & `canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/stores/charmstore.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.1.0/canonicalwebteam/store_api/stores/snapstore.py` & `canonicalwebteam_store_api-4.2.0/canonicalwebteam/store_api/stores/snapstore.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
             "download",
             "version",
             "created-at",
             "confinement",
             "categories",
             "trending",
             "unlisted",
+            "links",
         ],
         api_version=1,
     ):
         return super(SnapStore, self).get_item_details(
             name, None, fields, api_version
         )
```

### Comparing `canonicalwebteam_store_api-4.1.0/PKG-INFO` & `canonicalwebteam_store_api-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam-store-api
-Version: 4.1.0
+Version: 4.2.0
 Summary: 
 License: LGPL-3.0
 Author: Canonical Web Team
 Author-email: webteam@canonical.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
```

