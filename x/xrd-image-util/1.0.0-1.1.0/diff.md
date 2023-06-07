# Comparing `tmp/xrd-image-util-1.0.0.tar.gz` & `tmp/xrd-image-util-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrd-image-util-1.0.0.tar", last modified: Mon May 22 15:47:07 2023, max compression
+gzip compressed data, was "xrd-image-util-1.1.0.tar", last modified: Wed Jun  7 16:17:54 2023, max compression
```

## Comparing `xrd-image-util-1.0.0.tar` & `xrd-image-util-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:47:07.270236 xrd-image-util-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-22 15:46:54.000000 xrd-image-util-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-22 15:47:07.270236 xrd-image-util-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-22 15:46:54.000000 xrd-image-util-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:47:07.270236 xrd-image-util-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:47:07.266236 xrd-image-util-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/tests/test_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:47:07.266236 xrd-image-util-1.0.0/xrd_image_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-22 15:47:07.000000 xrd-image-util-1.0.0/xrd_image_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-22 15:47:07.000000 xrd-image-util-1.0.0/xrd_image_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:47:07.000000 xrd-image-util-1.0.0/xrd_image_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 15:47:07.000000 xrd-image-util-1.0.0/xrd_image_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 15:47:07.000000 xrd-image-util-1.0.0/xrd_image_util.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:47:07.266236 xrd-image-util-1.0.0/xrdimageutil/
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/xrdimageutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/xrdimageutil/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-22 15:46:55.000000 xrd-image-util-1.0.0/xrdimageutil/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/tests/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/xrd_image_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-07 16:17:54.000000 xrd-image-util-1.1.0/xrd_image_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-07 16:17:54.000000 xrd-image-util-1.1.0/xrd_image_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:17:54.000000 xrd-image-util-1.1.0/xrd_image_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 16:17:54.000000 xrd-image-util-1.1.0/xrd_image_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 16:17:54.000000 xrd-image-util-1.1.0/xrd_image_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/xrdimageutil/
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/xrdimageutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19687 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/xrdimageutil/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/xrdimageutil/utils.py
```

### Comparing `xrd-image-util-1.0.0/LICENSE.txt` & `xrd-image-util-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.0.0/PKG-INFO` & `xrd-image-util-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrd-image-util
-Version: 1.0.0
+Version: 1.1.0
 Summary: Utility package for handling XRD image data.
 Author-email: Henry Smith <henryjsmith12@outlook.com>
 License: Copyright (c) UChicago Argonne, LLC. All rights reserved.
         
         Copyright UChicago Argonne, LLC. This software was produced
         under U.S. Government contract DE-AC02-06CH11357 for Argonne National
         Laboratory (ANL), which is operated by UChicago Argonne, LLC for the
```

### Comparing `xrd-image-util-1.0.0/README.md` & `xrd-image-util-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.0.0/pyproject.toml` & `xrd-image-util-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xrd-image-util"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
     {name = "Henry Smith", email = "henryjsmith12@outlook.com"},
 ]
 description = "Utility package for handling XRD image data."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xrd-image-util-1.0.0/tests/test_catalog.py` & `xrd-image-util-1.1.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.0.0/tests/test_scan.py` & `xrd-image-util-1.1.0/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.0.0/xrd_image_util.egg-info/PKG-INFO` & `xrd-image-util-1.1.0/xrd_image_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrd-image-util
-Version: 1.0.0
+Version: 1.1.0
 Summary: Utility package for handling XRD image data.
 Author-email: Henry Smith <henryjsmith12@outlook.com>
 License: Copyright (c) UChicago Argonne, LLC. All rights reserved.
         
         Copyright UChicago Argonne, LLC. This software was produced
         under U.S. Government contract DE-AC02-06CH11357 for Argonne National
         Laboratory (ANL), which is operated by UChicago Argonne, LLC for the
```

### Comparing `xrd-image-util-1.0.0/xrdimageutil/__init__.py` & `xrd-image-util-1.1.0/xrdimageutil/__init__.py`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.0.0/xrdimageutil/utils.py` & `xrd-image-util-1.1.0/xrdimageutil/utils.py`

 * *Files identical despite different names*

