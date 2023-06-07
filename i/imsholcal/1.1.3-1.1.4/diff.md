# Comparing `tmp/imsholcal-1.1.3.tar.gz` & `tmp/imsholcal-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsholcal-1.1.3.tar", last modified: Sat May 13 23:01:41 2023, max compression
+gzip compressed data, was "imsholcal-1.1.4.tar", last modified: Wed Jun  7 06:32:46 2023, max compression
```

## Comparing `imsholcal-1.1.3.tar` & `imsholcal-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:01:41.068122 imsholcal-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:01:41.056121 imsholcal-1.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:01:41.060122 imsholcal-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-13 23:01:24.000000 imsholcal-1.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-13 23:01:24.000000 imsholcal-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-13 23:01:41.064122 imsholcal-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-13 23:01:24.000000 imsholcal-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 23:01:24.000000 imsholcal-1.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 23:01:24.000000 imsholcal-1.1.3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-13 23:01:24.000000 imsholcal-1.1.3/exchange_holidays.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:01:41.064122 imsholcal-1.1.3/imsholcal/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 23:01:24.000000 imsholcal-1.1.3/imsholcal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-13 23:01:24.000000 imsholcal-1.1.3/imsholcal/business_day.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:01:41.064122 imsholcal-1.1.3/imsholcal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-13 23:01:41.000000 imsholcal-1.1.3/imsholcal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-13 23:01:41.000000 imsholcal-1.1.3/imsholcal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 23:01:41.000000 imsholcal-1.1.3/imsholcal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-13 23:01:41.000000 imsholcal-1.1.3/imsholcal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-13 23:01:41.000000 imsholcal-1.1.3/imsholcal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 23:01:41.068122 imsholcal-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-13 23:01:24.000000 imsholcal-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:32:46.541921 imsholcal-1.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:32:46.537920 imsholcal-1.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:32:46.541921 imsholcal-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-07 06:32:30.000000 imsholcal-1.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 06:32:30.000000 imsholcal-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-07 06:32:46.541921 imsholcal-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-07 06:32:30.000000 imsholcal-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 06:32:30.000000 imsholcal-1.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:32:30.000000 imsholcal-1.1.4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-07 06:32:30.000000 imsholcal-1.1.4/exchange_holidays.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:32:46.541921 imsholcal-1.1.4/imsholcal/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:32:30.000000 imsholcal-1.1.4/imsholcal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-07 06:32:30.000000 imsholcal-1.1.4/imsholcal/business_day.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:32:46.541921 imsholcal-1.1.4/imsholcal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-07 06:32:46.000000 imsholcal-1.1.4/imsholcal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-07 06:32:46.000000 imsholcal-1.1.4/imsholcal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:32:46.000000 imsholcal-1.1.4/imsholcal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 06:32:46.000000 imsholcal-1.1.4/imsholcal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 06:32:46.000000 imsholcal-1.1.4/imsholcal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 06:32:46.541921 imsholcal-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-07 06:32:30.000000 imsholcal-1.1.4/setup.py
```

### Comparing `imsholcal-1.1.3/.github/workflows/python-publish.yml` & `imsholcal-1.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `imsholcal-1.1.3/setup.py` & `imsholcal-1.1.4/setup.py`

 * *Files identical despite different names*

