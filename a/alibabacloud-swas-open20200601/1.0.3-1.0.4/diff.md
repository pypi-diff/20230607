# Comparing `tmp/alibabacloud_swas-open20200601-1.0.3.tar.gz` & `tmp/alibabacloud_swas-open20200601-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_swas-open20200601-1.0.3.tar", last modified: Thu Mar  2 02:24:21 2023, max compression
+gzip compressed data, was "dist/alibabacloud_swas-open20200601-1.0.4.tar", last modified: Wed Jun  7 10:03:53 2023, max compression
```

## Comparing `alibabacloud_swas-open20200601-1.0.3.tar` & `alibabacloud_swas-open20200601-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      108 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/alibabacloud_swas_open20200601/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/alibabacloud_swas_open20200601/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150751 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/alibabacloud_swas_open20200601/client.py
--rw-r--r--   0 root         (0) root         (0)   219824 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/alibabacloud_swas_open20200601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/alibabacloud_swas_open20200601.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/alibabacloud_swas_open20200601.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/alibabacloud_swas_open20200601.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/alibabacloud_swas_open20200601.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/alibabacloud_swas_open20200601.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/alibabacloud_swas_open20200601.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2642 2023-03-02 02:24:21.000000 alibabacloud_swas-open20200601-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      516 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/alibabacloud_swas_open20200601/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/alibabacloud_swas_open20200601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   356879 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/alibabacloud_swas_open20200601/client.py
+-rw-r--r--   0 root         (0) root         (0)   366174 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/alibabacloud_swas_open20200601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/alibabacloud_swas_open20200601.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/alibabacloud_swas_open20200601.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/alibabacloud_swas_open20200601.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/alibabacloud_swas_open20200601.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/alibabacloud_swas_open20200601.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/alibabacloud_swas_open20200601.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-06-07 10:03:53.000000 alibabacloud_swas-open20200601-1.0.4/setup.py
```

### Comparing `alibabacloud_swas-open20200601-1.0.3/LICENSE` & `alibabacloud_swas-open20200601-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_swas-open20200601-1.0.3/PKG-INFO` & `alibabacloud_swas-open20200601-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_swas-open20200601
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud SWAS-OPEN (20200601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_swas-open20200601-1.0.3/README-CN.md` & `alibabacloud_swas-open20200601-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_swas-open20200601-1.0.3/README.md` & `alibabacloud_swas-open20200601-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_swas-open20200601-1.0.3/alibabacloud_swas_open20200601.egg-info/PKG-INFO` & `alibabacloud_swas-open20200601-1.0.4/alibabacloud_swas_open20200601.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-swas-open20200601
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud SWAS-OPEN (20200601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_swas-open20200601-1.0.3/setup.py` & `alibabacloud_swas-open20200601-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_swas-open20200601.
 
-Created on 02/03/2023
+Created on 07/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_swas_open20200601"
 NAME = "alibabacloud_swas-open20200601" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud SWAS-OPEN (20200601) SDK Library for Python"
```

