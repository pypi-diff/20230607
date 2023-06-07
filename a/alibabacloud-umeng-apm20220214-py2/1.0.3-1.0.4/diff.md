# Comparing `tmp/alibabacloud_umeng-apm20220214_py2-1.0.3.tar.gz` & `tmp/alibabacloud_umeng-apm20220214_py2-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_umeng-apm20220214_py2-1.0.3.tar", last modified: Mon Nov 28 07:51:19 2022, max compression
+gzip compressed data, was "dist/alibabacloud_umeng-apm20220214_py2-1.0.4.tar", last modified: Wed Jun  7 06:52:14 2023, max compression
```

## Comparing `alibabacloud_umeng-apm20220214_py2-1.0.3.tar` & `alibabacloud_umeng-apm20220214_py2-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      117 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2508 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/alibabacloud_umeng_apm20220214/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/alibabacloud_umeng_apm20220214/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6860 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/alibabacloud_umeng_apm20220214/client.py
--rw-r--r--   0 root         (0) root         (0)    21870 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/alibabacloud_umeng_apm20220214/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/alibabacloud_umeng_apm20220214_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2508 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/alibabacloud_umeng_apm20220214_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/alibabacloud_umeng_apm20220214_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/alibabacloud_umeng_apm20220214_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/alibabacloud_umeng_apm20220214_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/alibabacloud_umeng_apm20220214_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2935 2022-11-28 07:51:19.000000 alibabacloud_umeng-apm20220214_py2-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:52:14.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-07 06:52:13.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-07 06:52:13.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-07 06:52:13.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-07 06:52:14.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-07 06:52:13.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-06-07 06:52:13.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:52:14.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/alibabacloud_umeng_apm20220214/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-07 06:52:13.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/alibabacloud_umeng_apm20220214/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12873 2023-06-07 06:52:13.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/alibabacloud_umeng_apm20220214/client.py
+-rw-r--r--   0 root         (0) root         (0)    51871 2023-06-07 06:52:13.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/alibabacloud_umeng_apm20220214/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:52:14.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/alibabacloud_umeng_apm20220214_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-07 06:52:14.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/alibabacloud_umeng_apm20220214_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2023-06-07 06:52:14.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/alibabacloud_umeng_apm20220214_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 06:52:14.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/alibabacloud_umeng_apm20220214_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-07 06:52:14.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/alibabacloud_umeng_apm20220214_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-07 06:52:14.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/alibabacloud_umeng_apm20220214_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-07 06:52:14.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-06-07 06:52:13.000000 alibabacloud_umeng-apm20220214_py2-1.0.4/setup.py
```

### Comparing `alibabacloud_umeng-apm20220214_py2-1.0.3/LICENSE` & `alibabacloud_umeng-apm20220214_py2-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214_py2-1.0.3/PKG-INFO` & `alibabacloud_umeng-apm20220214_py2-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_umeng-apm20220214_py2
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud umeng-apm (20220214) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_umeng-apm20220214_py2-1.0.3/README-CN.md` & `alibabacloud_umeng-apm20220214_py2-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214_py2-1.0.3/README.md` & `alibabacloud_umeng-apm20220214_py2-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214_py2-1.0.3/alibabacloud_umeng_apm20220214_py2.egg-info/PKG-INFO` & `alibabacloud_umeng-apm20220214_py2-1.0.4/alibabacloud_umeng_apm20220214_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-umeng-apm20220214-py2
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud umeng-apm (20220214) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_umeng-apm20220214_py2-1.0.3/setup.py` & `alibabacloud_umeng-apm20220214_py2-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_umeng-apm20220214_py2.
 
-Created on 28/11/2022
+Created on 07/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_umeng_apm20220214"
 NAME = "alibabacloud_umeng-apm20220214_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud umeng-apm (20220214) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.1.0, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

