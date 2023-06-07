# Comparing `tmp/erode-python-0.7.tar.gz` & `tmp/erode-python-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erode-python-0.7.tar", last modified: Mon Sep  5 21:29:55 2022, max compression
+gzip compressed data, was "erode-python-0.7.1.tar", last modified: Wed Jun  7 15:18:38 2023, max compression
```

## Comparing `erode-python-0.7.tar` & `erode-python-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:29:55.233757 erode-python-0.7/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-05 21:29:38.000000 erode-python-0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-05 21:29:55.233757 erode-python-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-05 21:29:38.000000 erode-python-0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-05 21:29:39.000000 erode-python-0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:29:55.229757 erode-python-0.7/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:29:55.229757 erode-python-0.7/python/erode/
--rw-r--r--   0 runner    (1001) docker     (121)     8980 2022-09-05 21:29:39.000000 erode-python-0.7/python/erode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 21:29:55.233757 erode-python-0.7/python/erode_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-05 21:29:55.000000 erode-python-0.7/python/erode_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-09-05 21:29:55.000000 erode-python-0.7/python/erode_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 21:29:55.000000 erode-python-0.7/python/erode_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-05 21:29:55.000000 erode-python-0.7/python/erode_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-05 21:29:55.000000 erode-python-0.7/python/erode_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-05 21:29:55.233757 erode-python-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-09-05 21:29:39.000000 erode-python-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:38.128701 erode-python-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 15:18:28.000000 erode-python-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-07 15:18:38.128701 erode-python-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-07 15:18:28.000000 erode-python-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-07 15:18:28.000000 erode-python-0.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:38.124701 erode-python-0.7.1/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:38.128701 erode-python-0.7.1/python/erode_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-07 15:18:37.000000 erode-python-0.7.1/python/erode_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-07 15:18:37.000000 erode-python-0.7.1/python/erode_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:18:37.000000 erode-python-0.7.1/python/erode_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 15:18:37.000000 erode-python-0.7.1/python/erode_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:18:37.000000 erode-python-0.7.1/python/erode_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-07 15:18:38.132701 erode-python-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-07 15:18:28.000000 erode-python-0.7.1/setup.py
```

### Comparing `erode-python-0.7/setup.py` & `erode-python-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import zipfile
 
 import setuptools.command.build_py
 from setuptools import setup
 
 import logging
 
-VERSION = "0.7"
+VERSION = "0.7.1"
 
 if not VERSION.replace("9",""):
     branch = "main"
 else:
     branch = f"v{VERSION}"
 
 JAR_URL = f"https://github.com/colomoto/ERODE-CoLoMoTo/raw/{branch}/it.sssa.erode.colomoto/distr/erode4Colomoto.jar"
```

