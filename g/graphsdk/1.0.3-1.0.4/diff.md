# Comparing `tmp/graphsdk-1.0.3.tar.gz` & `tmp/graphsdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphsdk-1.0.3.tar", last modified: Wed Jun  7 12:19:44 2023, max compression
+gzip compressed data, was "graphsdk-1.0.4.tar", last modified: Wed Jun  7 12:41:54 2023, max compression
```

## Comparing `graphsdk-1.0.3.tar` & `graphsdk-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 12:19:44.134545 graphsdk-1.0.3/
--rw-rw-r--   0 codiant   (1000) codiant   (1000)     1079 2023-06-07 09:28:43.000000 graphsdk-1.0.3/LICENSE.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)     1658 2023-06-07 12:19:44.134545 graphsdk-1.0.3/PKG-INFO
--rw-rw-r--   0 codiant   (1000) codiant   (1000)       62 2023-06-07 09:23:51.000000 graphsdk-1.0.3/README.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)       85 2023-06-07 09:22:22.000000 graphsdk-1.0.3/pyproject.toml
--rw-rw-r--   0 codiant   (1000) codiant   (1000)      909 2023-06-07 12:19:44.134545 graphsdk-1.0.3/setup.cfg
-drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 12:19:44.134545 graphsdk-1.0.3/src/
-drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 12:19:44.134545 graphsdk-1.0.3/src/graphsdk.egg-info/
--rw-rw-r--   0 codiant   (1000) codiant   (1000)     1658 2023-06-07 12:19:44.000000 graphsdk-1.0.3/src/graphsdk.egg-info/PKG-INFO
--rw-rw-r--   0 codiant   (1000) codiant   (1000)      226 2023-06-07 12:19:44.000000 graphsdk-1.0.3/src/graphsdk.egg-info/SOURCES.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 12:19:44.000000 graphsdk-1.0.3/src/graphsdk.egg-info/dependency_links.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)      162 2023-06-07 12:19:44.000000 graphsdk-1.0.3/src/graphsdk.egg-info/requires.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 12:19:44.000000 graphsdk-1.0.3/src/graphsdk.egg-info/top_level.txt
+drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 12:41:54.791565 graphsdk-1.0.4/
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)     1079 2023-06-07 09:28:43.000000 graphsdk-1.0.4/LICENSE.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)     1658 2023-06-07 12:41:54.791565 graphsdk-1.0.4/PKG-INFO
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)       62 2023-06-07 09:23:51.000000 graphsdk-1.0.4/README.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)       85 2023-06-07 09:22:22.000000 graphsdk-1.0.4/pyproject.toml
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)      909 2023-06-07 12:41:54.791565 graphsdk-1.0.4/setup.cfg
+drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 12:41:54.791565 graphsdk-1.0.4/src/
+drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 12:41:54.791565 graphsdk-1.0.4/src/graphsdk.egg-info/
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)     1658 2023-06-07 12:41:54.000000 graphsdk-1.0.4/src/graphsdk.egg-info/PKG-INFO
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)      226 2023-06-07 12:41:54.000000 graphsdk-1.0.4/src/graphsdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 12:41:54.000000 graphsdk-1.0.4/src/graphsdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)      162 2023-06-07 12:41:54.000000 graphsdk-1.0.4/src/graphsdk.egg-info/requires.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 12:41:54.000000 graphsdk-1.0.4/src/graphsdk.egg-info/top_level.txt
```

### Comparing `graphsdk-1.0.3/LICENSE.txt` & `graphsdk-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graphsdk-1.0.3/PKG-INFO` & `graphsdk-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphsdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for accessing Graph Api
 Home-page: https://github.com/Ajay7415/graphapi
 Author: Ajay Vishwakarma
 Author-email: ajay.vishwakarma@codiant.com
 Project-URL: Bug Tracker, https://github.com/Ajay7415/graphapi/issues
 Project-URL: repository, https://github.com/Ajay7415/graphapi
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphsdk-1.0.3/setup.cfg` & `graphsdk-1.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = graphsdk
-version = 1.0.3
+version = 1.0.4
 author = Ajay Vishwakarma
 author_email = ajay.vishwakarma@codiant.com
 description = A package for accessing Graph Api
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/Ajay7415/graphapi
 project_urls =
```

### Comparing `graphsdk-1.0.3/src/graphsdk.egg-info/PKG-INFO` & `graphsdk-1.0.4/src/graphsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphsdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for accessing Graph Api
 Home-page: https://github.com/Ajay7415/graphapi
 Author: Ajay Vishwakarma
 Author-email: ajay.vishwakarma@codiant.com
 Project-URL: Bug Tracker, https://github.com/Ajay7415/graphapi/issues
 Project-URL: repository, https://github.com/Ajay7415/graphapi
 Classifier: Programming Language :: Python :: 3
```

