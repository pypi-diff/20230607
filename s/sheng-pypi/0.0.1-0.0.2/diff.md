# Comparing `tmp/sheng-pypi-0.0.1.tar.gz` & `tmp/sheng-pypi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheng-pypi-0.0.1.tar", last modified: Tue Jun  6 22:29:58 2023, max compression
+gzip compressed data, was "sheng-pypi-0.0.2.tar", last modified: Tue Jun  6 23:03:27 2023, max compression
```

## Comparing `sheng-pypi-0.0.1.tar` & `sheng-pypi-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 shengpang   (501) staff       (20)        0 2023-06-06 22:29:58.170335 sheng-pypi-0.0.1/
--rw-r--r--   0 shengpang   (501) staff       (20)      415 2023-06-06 22:29:58.170211 sheng-pypi-0.0.1/PKG-INFO
--rw-r--r--   0 shengpang   (501) staff       (20)       38 2023-06-06 22:29:58.170369 sheng-pypi-0.0.1/setup.cfg
--rw-r--r--   0 shengpang   (501) staff       (20)      643 2023-06-06 22:25:55.000000 sheng-pypi-0.0.1/setup.py
-drwxr-xr-x   0 shengpang   (501) staff       (20)        0 2023-06-06 22:29:58.170037 sheng-pypi-0.0.1/sheng_pypi.egg-info/
--rw-r--r--   0 shengpang   (501) staff       (20)      415 2023-06-06 22:29:58.000000 sheng-pypi-0.0.1/sheng_pypi.egg-info/PKG-INFO
--rw-r--r--   0 shengpang   (501) staff       (20)      144 2023-06-06 22:29:58.000000 sheng-pypi-0.0.1/sheng_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 shengpang   (501) staff       (20)        1 2023-06-06 22:29:58.000000 sheng-pypi-0.0.1/sheng_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 shengpang   (501) staff       (20)        1 2023-06-06 22:29:58.000000 sheng-pypi-0.0.1/sheng_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 shengpang   (501) staff       (20)        0 2023-06-06 23:03:27.752257 sheng-pypi-0.0.2/
+-rw-r--r--   0 shengpang   (501) staff       (20)      415 2023-06-06 23:03:27.752123 sheng-pypi-0.0.2/PKG-INFO
+-rw-r--r--   0 shengpang   (501) staff       (20)       38 2023-06-06 23:03:27.752296 sheng-pypi-0.0.2/setup.cfg
+-rw-r--r--   0 shengpang   (501) staff       (20)      643 2023-06-06 22:57:41.000000 sheng-pypi-0.0.2/setup.py
+drwxr-xr-x   0 shengpang   (501) staff       (20)        0 2023-06-06 23:03:27.751933 sheng-pypi-0.0.2/sheng_pypi.egg-info/
+-rw-r--r--   0 shengpang   (501) staff       (20)      415 2023-06-06 23:03:27.000000 sheng-pypi-0.0.2/sheng_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 shengpang   (501) staff       (20)      144 2023-06-06 23:03:27.000000 sheng-pypi-0.0.2/sheng_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 shengpang   (501) staff       (20)        1 2023-06-06 23:03:27.000000 sheng-pypi-0.0.2/sheng_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 shengpang   (501) staff       (20)        1 2023-06-06 23:03:27.000000 sheng-pypi-0.0.2/sheng_pypi.egg-info/top_level.txt
```

### Comparing `sheng-pypi-0.0.1/setup.py` & `sheng-pypi-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'sheng-pypi'
 
 # Setting up
 setup(
     name="sheng-pypi",
     version=VERSION,
     author="Sheng",
```

