# Comparing `tmp/demosdkpypi-1.8.2b2.tar.gz` & `tmp/demosdkpypi-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demosdkpypi-1.8.2b2.tar", last modified: Wed May 31 18:05:00 2023, max compression
+gzip compressed data, was "demosdkpypi-1.9.0.tar", last modified: Wed Jun  7 12:41:34 2023, max compression
```

## Comparing `demosdkpypi-1.8.2b2.tar` & `demosdkpypi-1.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:05:00.127552 demosdkpypi-1.8.2b2/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 18:05:00.127552 demosdkpypi-1.8.2b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 18:04:49.000000 demosdkpypi-1.8.2b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:05:00.127552 demosdkpypi-1.8.2b2/demosdkpypi/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 18:04:49.000000 demosdkpypi-1.8.2b2/demosdkpypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 18:04:49.000000 demosdkpypi-1.8.2b2/demosdkpypi/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:05:00.127552 demosdkpypi-1.8.2b2/demosdkpypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 18:05:00.000000 demosdkpypi-1.8.2b2/demosdkpypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-31 18:05:00.000000 demosdkpypi-1.8.2b2/demosdkpypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:05:00.000000 demosdkpypi-1.8.2b2/demosdkpypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 18:05:00.000000 demosdkpypi-1.8.2b2/demosdkpypi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:05:00.127552 demosdkpypi-1.8.2b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-31 18:04:58.000000 demosdkpypi-1.8.2b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:41:34.759393 demosdkpypi-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-07 12:41:34.759393 demosdkpypi-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 12:41:16.000000 demosdkpypi-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:41:34.759393 demosdkpypi-1.9.0/demosdkpypi/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 12:41:16.000000 demosdkpypi-1.9.0/demosdkpypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-07 12:41:16.000000 demosdkpypi-1.9.0/demosdkpypi/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:41:34.759393 demosdkpypi-1.9.0/demosdkpypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-07 12:41:34.000000 demosdkpypi-1.9.0/demosdkpypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-07 12:41:34.000000 demosdkpypi-1.9.0/demosdkpypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:41:34.000000 demosdkpypi-1.9.0/demosdkpypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 12:41:34.000000 demosdkpypi-1.9.0/demosdkpypi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:41:34.759393 demosdkpypi-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-07 12:41:31.000000 demosdkpypi-1.9.0/setup.py
```

### Comparing `demosdkpypi-1.8.2b2/setup.py` & `demosdkpypi-1.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import sys
 
 if sys.version_info < (3, 7):
     raise RuntimeError("my demo requires Python 3.7+")
-current_version = '1.8.2beta2'
+current_version = '1.9.0'
 
 setup(
     name='demosdkpypi',
     version=current_version,
     author='Bharti',
     author_email='bharti.sagar@skyflow.com',
     packages=find_packages(),
```

