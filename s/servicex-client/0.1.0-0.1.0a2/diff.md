# Comparing `tmp/servicex_client-0.1.0.tar.gz` & `tmp/servicex_client-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex_client-0.1.0.tar", max compression
+gzip compressed data, was "servicex_client-0.1.0a2.tar", max compression
```

## Comparing `servicex_client-0.1.0.tar` & `servicex_client-0.1.0a2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1499 2023-05-26 18:52:10.210423 servicex_client-0.1.0/LICENSE
--rw-r--r--   0        0        0       57 2023-05-26 18:52:10.210581 servicex_client-0.1.0/README.md
--rw-r--r--   0        0        0      858 2023-06-07 19:44:06.043549 servicex_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1535 2023-05-18 20:52:47.301125 servicex_client-0.1.0/servicex_client/__init__.py
--rw-r--r--   0        0        0      103 2023-05-24 11:39:06.420202 servicex_client-0.1.0/servicex_client/_version.py
--rw-r--r--   0        0        0     1535 2023-05-24 11:34:26.308135 servicex_client-0.1.0/servicex_client/app/__init__.py
--rw-r--r--   0        0        0     3018 2023-06-05 18:16:48.039413 servicex_client-0.1.0/servicex_client/app/cache.py
--rw-r--r--   0        0        0     1776 2023-06-05 18:23:48.980974 servicex_client-0.1.0/servicex_client/app/cli_options.py
--rw-r--r--   0        0        0     2647 2023-06-05 18:24:00.998098 servicex_client-0.1.0/servicex_client/app/main.py
--rw-r--r--   0        0        0     5272 2023-06-05 18:23:24.168440 servicex_client-0.1.0/servicex_client/app/transforms.py
--rw-r--r--   0        0        0     3304 2023-06-05 18:19:54.291689 servicex_client-0.1.0/servicex_client/configuration.py
--rw-r--r--   0        0        0     2700 2023-06-07 13:47:35.328751 servicex_client-0.1.0/servicex_client/dataset_identifier.py
--rw-r--r--   0        0        0     1535 2023-05-23 17:07:05.088270 servicex_client-0.1.0/servicex_client/func_adl/__init__.py
--rw-r--r--   0        0        0    20427 2023-06-07 12:23:01.886699 servicex_client-0.1.0/servicex_client/func_adl/servicex_dataset_source.py
--rw-r--r--   0        0        0     2656 2023-06-05 18:26:12.937923 servicex_client-0.1.0/servicex_client/func_adl/servicex_func_adl_uproot.py
--rw-r--r--   0        0        0     4013 2023-06-05 18:26:02.017120 servicex_client-0.1.0/servicex_client/func_adl/util.py
--rw-r--r--   0        0        0     3322 2023-06-05 18:22:03.961042 servicex_client-0.1.0/servicex_client/minio_adpater.py
--rw-r--r--   0        0        0     4158 2023-06-05 18:20:08.959305 servicex_client-0.1.0/servicex_client/models.py
--rw-r--r--   0        0        0     4311 2023-06-07 16:41:26.592863 servicex_client-0.1.0/servicex_client/query_cache.py
--rw-r--r--   0        0        0     5436 2023-06-05 18:20:38.984922 servicex_client-0.1.0/servicex_client/servicex_adapter.py
--rw-r--r--   0        0        0     4241 2023-06-05 18:22:24.984197 servicex_client-0.1.0/servicex_client/servicex_client.py
--rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 servicex_client-0.1.0/setup.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 servicex_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1499 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0       57 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/README.md
+-rw-r--r--   0        0        0      834 2023-06-07 20:13:16.367989 servicex_client-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1535 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/_version.py
+-rw-r--r--   0        0        0     1535 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/app/__init__.py
+-rw-r--r--   0        0        0     3018 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/app/cache.py
+-rw-r--r--   0        0        0     1776 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/app/cli_options.py
+-rw-r--r--   0        0        0     2647 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/app/main.py
+-rw-r--r--   0        0        0     5272 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/app/transforms.py
+-rw-r--r--   0        0        0     3304 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/configuration.py
+-rw-r--r--   0        0        0     2700 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/dataset_identifier.py
+-rw-r--r--   0        0        0     1535 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/func_adl/__init__.py
+-rw-r--r--   0        0        0    20427 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/func_adl/servicex_dataset_source.py
+-rw-r--r--   0        0        0     2656 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/func_adl/servicex_func_adl_uproot.py
+-rw-r--r--   0        0        0     4013 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/func_adl/util.py
+-rw-r--r--   0        0        0     3322 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/minio_adpater.py
+-rw-r--r--   0        0        0     4158 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/models.py
+-rw-r--r--   0        0        0     4311 2023-06-07 20:12:36.703505 servicex_client-0.1.0a2/servicex_client/query_cache.py
+-rw-r--r--   0        0        0     5436 2023-06-07 20:12:36.707505 servicex_client-0.1.0a2/servicex_client/servicex_adapter.py
+-rw-r--r--   0        0        0     4241 2023-06-07 20:12:36.707505 servicex_client-0.1.0a2/servicex_client/servicex_client.py
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 servicex_client-0.1.0a2/setup.py
+-rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 servicex_client-0.1.0a2/PKG-INFO
```

### Comparing `servicex_client-0.1.0/LICENSE` & `servicex_client-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/pyproject.toml` & `servicex_client-0.1.0a2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "servicex-client"
-version = "0.1.0"
+version = "0.1.0-alpha.2"
 description = ""
-authors = ["Ben Galewsky <bengal1@illinois.edu>", "Gordon Watts <gwatts@uw.edu>"]
+authors = ["Ben Galewsky <bengal1@illinois.edu>"]
 readme = "README.md"
 packages = [{include = "servicex_client"}]
 
 [tool.poetry.scripts]
 servicex = "servicex_client.app.main:app"
 
 [tool.poetry.dependencies]
```

### Comparing `servicex_client-0.1.0/servicex_client/__init__.py` & `servicex_client-0.1.0a2/servicex_client/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/app/__init__.py` & `servicex_client-0.1.0a2/servicex_client/app/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/app/cache.py` & `servicex_client-0.1.0a2/servicex_client/app/cache.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/app/cli_options.py` & `servicex_client-0.1.0a2/servicex_client/app/cli_options.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/app/main.py` & `servicex_client-0.1.0a2/servicex_client/app/main.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/app/transforms.py` & `servicex_client-0.1.0a2/servicex_client/app/transforms.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/configuration.py` & `servicex_client-0.1.0a2/servicex_client/configuration.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/dataset_identifier.py` & `servicex_client-0.1.0a2/servicex_client/dataset_identifier.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/func_adl/__init__.py` & `servicex_client-0.1.0a2/servicex_client/func_adl/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/func_adl/servicex_dataset_source.py` & `servicex_client-0.1.0a2/servicex_client/func_adl/servicex_dataset_source.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/func_adl/servicex_func_adl_uproot.py` & `servicex_client-0.1.0a2/servicex_client/func_adl/servicex_func_adl_uproot.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/func_adl/util.py` & `servicex_client-0.1.0a2/servicex_client/func_adl/util.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/minio_adpater.py` & `servicex_client-0.1.0a2/servicex_client/minio_adpater.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/models.py` & `servicex_client-0.1.0a2/servicex_client/models.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/query_cache.py` & `servicex_client-0.1.0a2/servicex_client/query_cache.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/servicex_adapter.py` & `servicex_client-0.1.0a2/servicex_client/servicex_adapter.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/servicex_client/servicex_client.py` & `servicex_client-0.1.0a2/servicex_client/servicex_client.py`

 * *Files identical despite different names*

### Comparing `servicex_client-0.1.0/setup.py` & `servicex_client-0.1.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'types-PyYAML>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['servicex = servicex_client.app.main:app']}
 
 setup_kwargs = {
     'name': 'servicex-client',
-    'version': '0.1.0',
+    'version': '0.1.0a2',
     'description': '',
     'long_description': '# servicex_client\nPython SDK and CLI Client for ServiceX\n',
     'author': 'Ben Galewsky',
     'author_email': 'bengal1@illinois.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `servicex_client-0.1.0/PKG-INFO` & `servicex_client-0.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicex-client
-Version: 0.1.0
+Version: 0.1.0a2
 Summary: 
 Author: Ben Galewsky
 Author-email: bengal1@illinois.edu
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

