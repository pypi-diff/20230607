# Comparing `tmp/sheng-pypi-0.0.2.tar.gz` & `tmp/sheng-pypi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheng-pypi-0.0.2.tar", last modified: Tue Jun  6 23:03:27 2023, max compression
+gzip compressed data, was "sheng-pypi-0.0.3.tar", last modified: Tue Jun  6 23:14:36 2023, max compression
```

## Comparing `sheng-pypi-0.0.2.tar` & `sheng-pypi-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 shengpang   (501) staff       (20)        0 2023-06-06 23:03:27.752257 sheng-pypi-0.0.2/
--rw-r--r--   0 shengpang   (501) staff       (20)      415 2023-06-06 23:03:27.752123 sheng-pypi-0.0.2/PKG-INFO
--rw-r--r--   0 shengpang   (501) staff       (20)       38 2023-06-06 23:03:27.752296 sheng-pypi-0.0.2/setup.cfg
--rw-r--r--   0 shengpang   (501) staff       (20)      643 2023-06-06 22:57:41.000000 sheng-pypi-0.0.2/setup.py
-drwxr-xr-x   0 shengpang   (501) staff       (20)        0 2023-06-06 23:03:27.751933 sheng-pypi-0.0.2/sheng_pypi.egg-info/
--rw-r--r--   0 shengpang   (501) staff       (20)      415 2023-06-06 23:03:27.000000 sheng-pypi-0.0.2/sheng_pypi.egg-info/PKG-INFO
--rw-r--r--   0 shengpang   (501) staff       (20)      144 2023-06-06 23:03:27.000000 sheng-pypi-0.0.2/sheng_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 shengpang   (501) staff       (20)        1 2023-06-06 23:03:27.000000 sheng-pypi-0.0.2/sheng_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 shengpang   (501) staff       (20)        1 2023-06-06 23:03:27.000000 sheng-pypi-0.0.2/sheng_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 shengpang   (501) staff       (20)        0 2023-06-06 23:14:36.600436 sheng-pypi-0.0.3/
+-rw-r--r--   0 shengpang   (501) staff       (20)      415 2023-06-06 23:14:36.600302 sheng-pypi-0.0.3/PKG-INFO
+-rw-r--r--   0 shengpang   (501) staff       (20)       38 2023-06-06 23:14:36.600473 sheng-pypi-0.0.3/setup.cfg
+-rw-r--r--   0 shengpang   (501) staff       (20)      643 2023-06-06 23:14:00.000000 sheng-pypi-0.0.3/setup.py
+drwxr-xr-x   0 shengpang   (501) staff       (20)        0 2023-06-06 23:14:36.600141 sheng-pypi-0.0.3/sheng_pypi.egg-info/
+-rw-r--r--   0 shengpang   (501) staff       (20)      415 2023-06-06 23:14:36.000000 sheng-pypi-0.0.3/sheng_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 shengpang   (501) staff       (20)      144 2023-06-06 23:14:36.000000 sheng-pypi-0.0.3/sheng_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 shengpang   (501) staff       (20)        1 2023-06-06 23:14:36.000000 sheng-pypi-0.0.3/sheng_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 shengpang   (501) staff       (20)        1 2023-06-06 23:14:36.000000 sheng-pypi-0.0.3/sheng_pypi.egg-info/top_level.txt
```

### Comparing `sheng-pypi-0.0.2/setup.py` & `sheng-pypi-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'sheng-pypi'
 
 # Setting up
 setup(
     name="sheng-pypi",
     version=VERSION,
     author="Sheng",
```

