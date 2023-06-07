# Comparing `tmp/vtiger_cloudsdk_restapi-1.1.tar.gz` & `tmp/vtiger_cloudsdk_restapi-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtiger_cloudsdk_restapi-1.1.tar", last modified: Tue Jun  6 14:24:13 2023, max compression
+gzip compressed data, was "vtiger_cloudsdk_restapi-1.2.tar", last modified: Wed Jun  7 03:38:12 2023, max compression
```

## Comparing `vtiger_cloudsdk_restapi-1.1.tar` & `vtiger_cloudsdk_restapi-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-06 14:24:13.804143 vtiger_cloudsdk_restapi-1.1/
--rw-rw-r--   0 prasad    (1000) prasad    (1000)      249 2023-06-06 14:24:13.804143 vtiger_cloudsdk_restapi-1.1/PKG-INFO
--rw-rw-r--   0 prasad    (1000) prasad    (1000)       38 2023-06-06 14:24:13.804143 vtiger_cloudsdk_restapi-1.1/setup.cfg
--rw-r--r--   0 prasad    (1000) prasad    (1000)      350 2023-06-06 14:23:19.000000 vtiger_cloudsdk_restapi-1.1/setup.py
-drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-06 14:24:13.804143 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi/
--rw-r--r--   0 prasad    (1000) prasad    (1000)     6042 2023-06-06 14:22:42.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi/__init__.py
-drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-06 14:24:13.804143 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/
--rw-rw-r--   0 prasad    (1000) prasad    (1000)      249 2023-06-06 14:24:13.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/PKG-INFO
--rw-rw-r--   0 prasad    (1000) prasad    (1000)      324 2023-06-06 14:24:13.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/SOURCES.txt
--rw-rw-r--   0 prasad    (1000) prasad    (1000)        1 2023-06-06 14:24:13.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/dependency_links.txt
--rw-rw-r--   0 prasad    (1000) prasad    (1000)        1 2023-06-05 10:50:14.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/not-zip-safe
--rw-rw-r--   0 prasad    (1000) prasad    (1000)        9 2023-06-06 14:24:13.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/requires.txt
--rw-rw-r--   0 prasad    (1000) prasad    (1000)       24 2023-06-06 14:24:13.000000 vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi.egg-info/top_level.txt
+drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-07 03:38:12.840965 vtiger_cloudsdk_restapi-1.2/
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)      249 2023-06-07 03:38:12.840965 vtiger_cloudsdk_restapi-1.2/PKG-INFO
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)       38 2023-06-07 03:38:12.840965 vtiger_cloudsdk_restapi-1.2/setup.cfg
+-rw-r--r--   0 prasad    (1000) prasad    (1000)      350 2023-06-07 03:37:37.000000 vtiger_cloudsdk_restapi-1.2/setup.py
+drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-07 03:38:12.840965 vtiger_cloudsdk_restapi-1.2/vtiger_cloudsdk_restapi/
+-rw-r--r--   0 prasad    (1000) prasad    (1000)     6213 2023-06-07 03:35:45.000000 vtiger_cloudsdk_restapi-1.2/vtiger_cloudsdk_restapi/__init__.py
+drwxrwxr-x   0 prasad    (1000) prasad    (1000)        0 2023-06-07 03:38:12.840965 vtiger_cloudsdk_restapi-1.2/vtiger_cloudsdk_restapi.egg-info/
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)      249 2023-06-07 03:38:12.000000 vtiger_cloudsdk_restapi-1.2/vtiger_cloudsdk_restapi.egg-info/PKG-INFO
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)      324 2023-06-07 03:38:12.000000 vtiger_cloudsdk_restapi-1.2/vtiger_cloudsdk_restapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)        1 2023-06-07 03:38:12.000000 vtiger_cloudsdk_restapi-1.2/vtiger_cloudsdk_restapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)        1 2023-06-05 10:50:14.000000 vtiger_cloudsdk_restapi-1.2/vtiger_cloudsdk_restapi.egg-info/not-zip-safe
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)        9 2023-06-07 03:38:12.000000 vtiger_cloudsdk_restapi-1.2/vtiger_cloudsdk_restapi.egg-info/requires.txt
+-rw-rw-r--   0 prasad    (1000) prasad    (1000)       24 2023-06-07 03:38:12.000000 vtiger_cloudsdk_restapi-1.2/vtiger_cloudsdk_restapi.egg-info/top_level.txt
```

### Comparing `vtiger_cloudsdk_restapi-1.1/vtiger_cloudsdk_restapi/__init__.py` & `vtiger_cloudsdk_restapi-1.2/vtiger_cloudsdk_restapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # The content of this file is subject to ("Vtiger Public License 1.2") refer to LIECENSE for more details.
 # Copyright (c) Vtiger.
 # All Rights Reserved.
 
 from requests import Request, Session
 import json
-import urllib
+
+# python 2.x or 3.x
+try:
+    from urllib import quote
+except ImportError:
+    from urllib.parse import quote
+
+# python 3.x onwards
+try:
+    basestring
+except NameError:
+    basestring = str
 
 class Client:
 
 	def __init__(self, domain, username, password):
 		self.__endpoint = None
 		self.__username = None
 		self.__password = None
@@ -59,15 +70,15 @@
 		if parameters is not None:
 			if method == "GET":
 				pairs = []
 				for k in parameters:
 					v = parameters[k]
 					if isinstance(v, basestring) is False:
 						v = json.dumps(v)
-					pairs.append(k + "=" + urllib.quote(v))
+					pairs.append(k + "=" + quote(v))
 				url = url + "?" + ("&".join(pairs))
 				parameters = None
 			else:
 				for k in parameters:
 					v = parameters[k]
 					if isinstance(v, basestring) is False:
 						parameters[k] = json.dumps(v)
@@ -246,8 +257,8 @@
 			}
 		})
 
 	def reopen(self, id):
 		return self.__operation("POST", "/reopen", {"id": id})
 
 	def account_hierarchy(self, id):
-		return self.__operation("GET", "/get_account_hierarchy", {"id": id})
+		return self.__operation("GET", "/get_account_hierarchy", {"id": id})
```

