# Comparing `tmp/demosdkpypi-1.9.2.tar.gz` & `tmp/demosdkpypi-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demosdkpypi-1.9.2.tar", last modified: Wed Jun  7 12:52:12 2023, max compression
+gzip compressed data, was "demosdkpypi-1.9.3.tar", last modified: Wed Jun  7 12:57:38 2023, max compression
```

## Comparing `demosdkpypi-1.9.2.tar` & `demosdkpypi-1.9.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:12.534118 demosdkpypi-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-07 12:52:12.534118 demosdkpypi-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 12:51:56.000000 demosdkpypi-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:12.534118 demosdkpypi-1.9.2/demosdkpypi/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 12:51:56.000000 demosdkpypi-1.9.2/demosdkpypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 12:51:56.000000 demosdkpypi-1.9.2/demosdkpypi/hello.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 12:51:56.000000 demosdkpypi-1.9.2/demosdkpypi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:12.534118 demosdkpypi-1.9.2/demosdkpypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-07 12:52:12.000000 demosdkpypi-1.9.2/demosdkpypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-07 12:52:12.000000 demosdkpypi-1.9.2/demosdkpypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:52:12.000000 demosdkpypi-1.9.2/demosdkpypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 12:52:12.000000 demosdkpypi-1.9.2/demosdkpypi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:52:12.534118 demosdkpypi-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-07 12:52:07.000000 demosdkpypi-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:57:38.687816 demosdkpypi-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-07 12:57:38.687816 demosdkpypi-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 12:57:23.000000 demosdkpypi-1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:57:38.687816 demosdkpypi-1.9.3/demosdkpypi/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 12:57:23.000000 demosdkpypi-1.9.3/demosdkpypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 12:57:23.000000 demosdkpypi-1.9.3/demosdkpypi/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 12:57:23.000000 demosdkpypi-1.9.3/demosdkpypi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:57:38.687816 demosdkpypi-1.9.3/demosdkpypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-07 12:57:38.000000 demosdkpypi-1.9.3/demosdkpypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-07 12:57:38.000000 demosdkpypi-1.9.3/demosdkpypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:57:38.000000 demosdkpypi-1.9.3/demosdkpypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 12:57:38.000000 demosdkpypi-1.9.3/demosdkpypi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:57:38.687816 demosdkpypi-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-07 12:57:35.000000 demosdkpypi-1.9.3/setup.py
```

### Comparing `demosdkpypi-1.9.2/setup.py` & `demosdkpypi-1.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import sys
 
 if sys.version_info < (3, 7):
     raise RuntimeError("my demo requires Python 3.7+")
-current_version = '1.9.2'
+current_version = '1.9.3'
 
 setup(
     name='demosdkpypi',
     version=current_version,
     author='Bharti',
     author_email='bharti.sagar@skyflow.com',
     packages=find_packages(),
```

