# Comparing `tmp/rblx-open-cloud-1.3.0.tar.gz` & `tmp/rblx-open-cloud-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rblx-open-cloud-1.3.0.tar", last modified: Fri Jun  2 07:05:48 2023, max compression
+gzip compressed data, was "rblx-open-cloud-1.3.1.tar", last modified: Wed Jun  7 14:13:18 2023, max compression
```

## Comparing `rblx-open-cloud-1.3.0.tar` & `rblx-open-cloud-1.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:05:48.802884 rblx-open-cloud-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-02 07:05:48.802884 rblx-open-cloud-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:05:48.802884 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-02 07:05:48.000000 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-02 07:05:48.000000 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:05:48.000000 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 07:05:48.000000 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 07:05:48.000000 rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:05:48.802884 rblx-open-cloud-1.3.0/rblxopencloud/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/experience.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/rblxopencloud/user.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 07:05:48.806884 rblx-open-cloud-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-02 07:05:35.000000 rblx-open-cloud-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:13:18.474059 rblx-open-cloud-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 14:13:02.000000 rblx-open-cloud-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-07 14:13:18.474059 rblx-open-cloud-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-07 14:13:02.000000 rblx-open-cloud-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:13:18.470059 rblx-open-cloud-1.3.1/rblx_open_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-07 14:13:18.000000 rblx-open-cloud-1.3.1/rblx_open_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-07 14:13:18.000000 rblx-open-cloud-1.3.1/rblx_open_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:13:18.000000 rblx-open-cloud-1.3.1/rblx_open_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 14:13:18.000000 rblx-open-cloud-1.3.1/rblx_open_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 14:13:18.000000 rblx-open-cloud-1.3.1/rblx_open_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:13:18.474059 rblx-open-cloud-1.3.1/rblxopencloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 14:13:02.000000 rblx-open-cloud-1.3.1/rblxopencloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-07 14:13:02.000000 rblx-open-cloud-1.3.1/rblxopencloud/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-06-07 14:13:02.000000 rblx-open-cloud-1.3.1/rblxopencloud/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-07 14:13:02.000000 rblx-open-cloud-1.3.1/rblxopencloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-07 14:13:02.000000 rblx-open-cloud-1.3.1/rblxopencloud/experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-07 14:13:02.000000 rblx-open-cloud-1.3.1/rblxopencloud/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-06-07 14:13:02.000000 rblx-open-cloud-1.3.1/rblxopencloud/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-07 14:13:02.000000 rblx-open-cloud-1.3.1/rblxopencloud/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:13:18.474059 rblx-open-cloud-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-07 14:13:02.000000 rblx-open-cloud-1.3.1/setup.py
```

### Comparing `rblx-open-cloud-1.3.0/LICENSE` & `rblx-open-cloud-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rblx-open-cloud-1.3.0/PKG-INFO` & `rblx-open-cloud-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rblx-open-cloud
-Version: 1.3.0
+Version: 1.3.1
 Summary: API wrapper for Roblox Open Cloud
 Home-page: https://github.com/TreeBen77/rblx-open-cloud
 Author: TreeBen77
 License: MIT
 Keywords: roblox,open-cloud,data-store,place-publishing,mesageing-service
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `rblx-open-cloud-1.3.0/README.md` & `rblx-open-cloud-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rblx-open-cloud-1.3.0/rblx_open_cloud.egg-info/PKG-INFO` & `rblx-open-cloud-1.3.1/rblx_open_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rblx-open-cloud
-Version: 1.3.0
+Version: 1.3.1
 Summary: API wrapper for Roblox Open Cloud
 Home-page: https://github.com/TreeBen77/rblx-open-cloud
 Author: TreeBen77
 License: MIT
 Keywords: roblox,open-cloud,data-store,place-publishing,mesageing-service
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `rblx-open-cloud-1.3.0/rblxopencloud/creator.py` & `rblx-open-cloud-1.3.1/rblxopencloud/creator.py`

 * *Files identical despite different names*

### Comparing `rblx-open-cloud-1.3.0/rblxopencloud/datastore.py` & `rblx-open-cloud-1.3.1/rblxopencloud/datastore.py`

 * *Files identical despite different names*

### Comparing `rblx-open-cloud-1.3.0/rblxopencloud/exceptions.py` & `rblx-open-cloud-1.3.1/rblxopencloud/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "NotFound",
     "InvalidKey",
     "RateLimited",
     "ServiceUnavailable",
     "PreconditionFailed",
     "InsufficientScope",
     "InvalidAsset",
-    "InvalidCode"
+    "InvalidCode",
     "ModeratedText"
 )
 
 class rblx_opencloudException(Exception): pass
 class NotFound(rblx_opencloudException): pass
 class InvalidKey(rblx_opencloudException): pass
 class RateLimited(rblx_opencloudException): pass
```

### Comparing `rblx-open-cloud-1.3.0/rblxopencloud/experience.py` & `rblx-open-cloud-1.3.1/rblxopencloud/experience.py`

 * *Files identical despite different names*

### Comparing `rblx-open-cloud-1.3.0/rblxopencloud/oauth2.py` & `rblx-open-cloud-1.3.1/rblxopencloud/oauth2.py`

 * *Files identical despite different names*

### Comparing `rblx-open-cloud-1.3.0/rblxopencloud/user.py` & `rblx-open-cloud-1.3.1/rblxopencloud/user.py`

 * *Files identical despite different names*

### Comparing `rblx-open-cloud-1.3.0/setup.py` & `rblx-open-cloud-1.3.1/setup.py`

 * *Files identical despite different names*

