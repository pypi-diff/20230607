# Comparing `tmp/torchbricks-0.0.1.tar.gz` & `tmp/torchbricks-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbricks-0.0.1.tar", last modified: Tue Jun  6 21:27:32 2023, max compression
+gzip compressed data, was "torchbricks-0.0.4.tar", last modified: Tue Jun  6 23:00:59 2023, max compression
```

## Comparing `torchbricks-0.0.1.tar` & `torchbricks-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,21 @@
-drwxrwxr-x   0 petemachine  (1000) petemachine  (1000)        0 2023-06-06 21:27:32.158803 torchbricks-0.0.1/
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)       86 2023-06-06 21:20:18.000000 torchbricks-0.0.1/Containerfile
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)      229 2023-05-22 21:35:14.000000 torchbricks-0.0.1/HISTORY.md
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)     1075 2023-06-06 19:15:20.000000 torchbricks-0.0.1/LICENSE
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)       97 2023-06-06 21:22:56.000000 torchbricks-0.0.1/MANIFEST.in
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)     3155 2023-06-06 21:27:32.158803 torchbricks-0.0.1/PKG-INFO
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)     1365 2023-06-06 20:47:19.000000 torchbricks-0.0.1/README.md
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)     1140 2023-06-06 20:59:13.000000 torchbricks-0.0.1/pyproject.toml
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)       38 2023-06-06 21:27:32.158803 torchbricks-0.0.1/setup.cfg
-drwxrwxr-x   0 petemachine  (1000) petemachine  (1000)        0 2023-06-06 21:27:32.154803 torchbricks-0.0.1/src/
-drwxrwxr-x   0 petemachine  (1000) petemachine  (1000)        0 2023-06-06 21:27:32.158803 torchbricks-0.0.1/src/torchbricks/
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)        6 2023-05-22 21:35:14.000000 torchbricks-0.0.1/src/torchbricks/VERSION
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)       22 2023-06-06 20:31:21.000000 torchbricks-0.0.1/src/torchbricks/__init__.py
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)     9122 2023-06-03 23:42:56.000000 torchbricks-0.0.1/src/torchbricks/bricks.py
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)     1069 2023-05-23 21:59:46.000000 torchbricks-0.0.1/src/torchbricks/custom_metrics.py
-drwxrwxr-x   0 petemachine  (1000) petemachine  (1000)        0 2023-06-06 21:27:32.158803 torchbricks-0.0.1/src/torchbricks.egg-info/
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)     3155 2023-06-06 21:27:32.000000 torchbricks-0.0.1/src/torchbricks.egg-info/PKG-INFO
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)      458 2023-06-06 21:27:32.000000 torchbricks-0.0.1/src/torchbricks.egg-info/SOURCES.txt
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)        1 2023-06-06 21:27:32.000000 torchbricks-0.0.1/src/torchbricks.egg-info/dependency_links.txt
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)       32 2023-06-06 21:27:32.000000 torchbricks-0.0.1/src/torchbricks.egg-info/requires.txt
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)       12 2023-06-06 21:27:32.000000 torchbricks-0.0.1/src/torchbricks.egg-info/top_level.txt
-drwxrwxr-x   0 petemachine  (1000) petemachine  (1000)        0 2023-06-06 21:27:32.158803 torchbricks-0.0.1/tests/
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)        0 2023-05-22 21:35:14.000000 torchbricks-0.0.1/tests/__init__.py
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)      398 2023-05-23 21:43:28.000000 torchbricks-0.0.1/tests/conftest.py
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)     8083 2023-06-06 20:39:32.000000 torchbricks-0.0.1/tests/lightning_module.py
--rw-rw-r--   0 petemachine  (1000) petemachine  (1000)     3299 2023-06-06 20:39:20.000000 torchbricks-0.0.1/tests/test_bricks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:00:59.260885 torchbricks-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-06 23:00:40.000000 torchbricks-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-06 23:00:40.000000 torchbricks-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-06 23:00:59.260885 torchbricks-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-06 23:00:40.000000 torchbricks-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-06 23:00:40.000000 torchbricks-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 23:00:59.260885 torchbricks-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:00:59.256885 torchbricks-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:00:59.260885 torchbricks-0.0.4/src/torchbricks/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 23:00:40.000000 torchbricks-0.0.4/src/torchbricks/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 23:00:40.000000 torchbricks-0.0.4/src/torchbricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-06-06 23:00:40.000000 torchbricks-0.0.4/src/torchbricks/bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-06 23:00:40.000000 torchbricks-0.0.4/src/torchbricks/custom_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:00:59.260885 torchbricks-0.0.4/src/torchbricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-06 23:00:59.000000 torchbricks-0.0.4/src/torchbricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-06 23:00:59.000000 torchbricks-0.0.4/src/torchbricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:00:59.000000 torchbricks-0.0.4/src/torchbricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 23:00:59.000000 torchbricks-0.0.4/src/torchbricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 23:00:59.000000 torchbricks-0.0.4/src/torchbricks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:00:59.260885 torchbricks-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-06 23:00:40.000000 torchbricks-0.0.4/tests/test_bricks.py
```

### Comparing `torchbricks-0.0.1/LICENSE` & `torchbricks-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.1/PKG-INFO` & `torchbricks-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbricks
-Version: 0.0.1
+Version: 0.0.4
 Summary: Decoupled and modular approach to building multi-task ML models
 Author-email: Peter Hviid Christianse <PeterHviidChristiansen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Christiansen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `torchbricks-0.0.1/README.md` & `torchbricks-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.1/pyproject.toml` & `torchbricks-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.ruff]
 line-length = 140
 
 [project]
 name = "torchbricks"
-version = "0.0.1"
+version = "0.0.4"
 description = "Decoupled and modular approach to building multi-task ML models"
 readme = "README.md"
 authors = [{ name = "Peter Hviid Christianse", email = "PeterHviidChristiansen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -23,15 +23,15 @@
 requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/PeteHeine/torchbricks"
 
 # bumpver update --patch | --minor | --major --dry
 [tool.bumpver]
-current_version = "0.0.1"
+current_version = "0.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]  # Specify all files containging version-numbers
```

### Comparing `torchbricks-0.0.1/src/torchbricks/bricks.py` & `torchbricks-0.0.4/src/torchbricks/bricks.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.1/src/torchbricks/custom_metrics.py` & `torchbricks-0.0.4/src/torchbricks/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.1/src/torchbricks.egg-info/PKG-INFO` & `torchbricks-0.0.4/src/torchbricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbricks
-Version: 0.0.1
+Version: 0.0.4
 Summary: Decoupled and modular approach to building multi-task ML models
 Author-email: Peter Hviid Christianse <PeterHviidChristiansen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Christiansen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `torchbricks-0.0.1/tests/test_bricks.py` & `torchbricks-0.0.4/tests/test_bricks.py`

 * *Files identical despite different names*

