# Comparing `tmp/graphsdk-1.0.1.tar.gz` & `tmp/graphsdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphsdk-1.0.1.tar", last modified: Wed Jun  7 11:21:55 2023, max compression
+gzip compressed data, was "graphsdk-1.0.2.tar", last modified: Wed Jun  7 12:03:19 2023, max compression
```

## Comparing `graphsdk-1.0.1.tar` & `graphsdk-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 11:21:55.168110 graphsdk-1.0.1/
--rw-rw-r--   0 codiant   (1000) codiant   (1000)     1079 2023-06-07 09:28:43.000000 graphsdk-1.0.1/LICENSE.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)     1658 2023-06-07 11:21:55.168110 graphsdk-1.0.1/PKG-INFO
--rw-rw-r--   0 codiant   (1000) codiant   (1000)       62 2023-06-07 09:23:51.000000 graphsdk-1.0.1/README.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)       85 2023-06-07 09:22:22.000000 graphsdk-1.0.1/pyproject.toml
--rw-rw-r--   0 codiant   (1000) codiant   (1000)      904 2023-06-07 11:21:55.168110 graphsdk-1.0.1/setup.cfg
-drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 11:21:55.168110 graphsdk-1.0.1/src/
-drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 11:21:55.168110 graphsdk-1.0.1/src/graphsdk.egg-info/
--rw-rw-r--   0 codiant   (1000) codiant   (1000)     1658 2023-06-07 11:21:55.000000 graphsdk-1.0.1/src/graphsdk.egg-info/PKG-INFO
--rw-rw-r--   0 codiant   (1000) codiant   (1000)      226 2023-06-07 11:21:55.000000 graphsdk-1.0.1/src/graphsdk.egg-info/SOURCES.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 11:21:55.000000 graphsdk-1.0.1/src/graphsdk.egg-info/dependency_links.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)      162 2023-06-07 11:21:55.000000 graphsdk-1.0.1/src/graphsdk.egg-info/requires.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 11:21:55.000000 graphsdk-1.0.1/src/graphsdk.egg-info/top_level.txt
+drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 12:03:19.467981 graphsdk-1.0.2/
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)     1079 2023-06-07 09:28:43.000000 graphsdk-1.0.2/LICENSE.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)     1658 2023-06-07 12:03:19.467981 graphsdk-1.0.2/PKG-INFO
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)       62 2023-06-07 09:23:51.000000 graphsdk-1.0.2/README.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)       85 2023-06-07 09:22:22.000000 graphsdk-1.0.2/pyproject.toml
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)      904 2023-06-07 12:03:19.467981 graphsdk-1.0.2/setup.cfg
+drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 12:03:19.463981 graphsdk-1.0.2/src/
+drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 12:03:19.467981 graphsdk-1.0.2/src/graphsdk.egg-info/
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)     1658 2023-06-07 12:03:19.000000 graphsdk-1.0.2/src/graphsdk.egg-info/PKG-INFO
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)      226 2023-06-07 12:03:19.000000 graphsdk-1.0.2/src/graphsdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 12:03:19.000000 graphsdk-1.0.2/src/graphsdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)      162 2023-06-07 12:03:19.000000 graphsdk-1.0.2/src/graphsdk.egg-info/requires.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 12:03:19.000000 graphsdk-1.0.2/src/graphsdk.egg-info/top_level.txt
```

### Comparing `graphsdk-1.0.1/LICENSE.txt` & `graphsdk-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graphsdk-1.0.1/PKG-INFO` & `graphsdk-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphsdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for accessing Graph Api
 Home-page: https://github.com/Ajay7415/graphapi
 Author: Ajay Vishwakarma
 Author-email: ajay.vishwakarma@codiant.com
 Project-URL: Bug Tracker, https://github.com/Ajay7415/graphapi/issues
 Project-URL: repository, https://github.com/Ajay7415/graphapi
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphsdk-1.0.1/setup.cfg` & `graphsdk-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = graphsdk
-version = 1.0.1
+version = 1.0.2
 author = Ajay Vishwakarma
 author_email = ajay.vishwakarma@codiant.com
 description = A package for accessing Graph Api
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/Ajay7415/graphapi
 project_urls =
```

### Comparing `graphsdk-1.0.1/src/graphsdk.egg-info/PKG-INFO` & `graphsdk-1.0.2/src/graphsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphsdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for accessing Graph Api
 Home-page: https://github.com/Ajay7415/graphapi
 Author: Ajay Vishwakarma
 Author-email: ajay.vishwakarma@codiant.com
 Project-URL: Bug Tracker, https://github.com/Ajay7415/graphapi/issues
 Project-URL: repository, https://github.com/Ajay7415/graphapi
 Classifier: Programming Language :: Python :: 3
```

