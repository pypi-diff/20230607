# Comparing `tmp/EnToFa-1.4.tar.gz` & `tmp/EnToFa-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnToFa-1.4.tar", last modified: Wed Jun  7 04:31:08 2023, max compression
+gzip compressed data, was "EnToFa-1.4.1.tar", last modified: Wed Jun  7 04:54:02 2023, max compression
```

## Comparing `EnToFa-1.4.tar` & `EnToFa-1.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:31:08.209662 EnToFa-1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:31:08.209662 EnToFa-1.4/EnToFa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 04:31:08.000000 EnToFa-1.4/EnToFa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-07 04:30:58.000000 EnToFa-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-07 04:31:08.209662 EnToFa-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-07 04:30:58.000000 EnToFa-1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 04:31:08.209662 EnToFa-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-07 04:30:58.000000 EnToFa-1.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-07 04:30:58.000000 EnToFa-1.4/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:54:02.904998 EnToFa-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:54:02.904998 EnToFa-1.4.1/EnToFa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-07 04:53:52.000000 EnToFa-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 04:54:02.904998 EnToFa-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-07 04:53:52.000000 EnToFa-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 04:54:02.904998 EnToFa-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-07 04:53:52.000000 EnToFa-1.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-07 04:53:52.000000 EnToFa-1.4.1/translator.py
```

### Comparing `EnToFa-1.4/LICENSE` & `EnToFa-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EnToFa-1.4/translator.py` & `EnToFa-1.4.1/translator.py`

 * *Files identical despite different names*

