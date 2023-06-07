# Comparing `tmp/xtalx-1.0.2.tar.gz` & `tmp/xtalx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtalx-1.0.2.tar", last modified: Tue Jun  6 00:05:25 2023, max compression
+gzip compressed data, was "xtalx-1.0.3.tar", last modified: Wed Jun  7 20:32:24 2023, max compression
```

## Comparing `xtalx-1.0.2.tar` & `xtalx-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-06 00:05:25.361720 xtalx-1.0.2/
--rw-r--r--   0 greent7    (502) staff       (20)     1092 2023-06-05 20:34:21.000000 xtalx-1.0.2/LICENSE
--rw-r--r--   0 greent7    (502) staff       (20)     2685 2023-06-06 00:05:25.361777 xtalx-1.0.2/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)     2190 2023-06-05 20:34:21.000000 xtalx-1.0.2/README.rst
--rw-r--r--   0 greent7    (502) staff       (20)      782 2023-06-06 00:05:25.362029 xtalx-1.0.2/setup.cfg
--rw-r--r--   0 greent7    (502) staff       (20)       38 2023-06-05 20:34:21.000000 xtalx-1.0.2/setup.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-06 00:05:25.360702 xtalx-1.0.2/xtalx/
--rw-r--r--   0 greent7    (502) staff       (20)      222 2023-06-05 20:34:21.000000 xtalx-1.0.2/xtalx/__init__.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-06 00:05:25.361638 xtalx-1.0.2/xtalx/tools/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2023-06-05 20:34:21.000000 xtalx-1.0.2/xtalx/tools/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      498 2023-06-05 20:34:21.000000 xtalx-1.0.2/xtalx/tools/discover.py
--rw-r--r--   0 greent7    (502) staff       (20)     1265 2023-06-05 20:34:21.000000 xtalx-1.0.2/xtalx/tools/xtalx_test_read.py
--rw-r--r--   0 greent7    (502) staff       (20)     1575 2023-06-05 20:54:27.000000 xtalx-1.0.2/xtalx/tools/xtalx_test_yield.py
--rw-r--r--   0 greent7    (502) staff       (20)    13776 2023-06-05 20:56:37.000000 xtalx-1.0.2/xtalx/xtalx.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-06 00:05:25.361272 xtalx-1.0.2/xtalx.egg-info/
--rw-r--r--   0 greent7    (502) staff       (20)     2685 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)      357 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/SOURCES.txt
--rw-r--r--   0 greent7    (502) staff       (20)        1 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/dependency_links.txt
--rw-r--r--   0 greent7    (502) staff       (20)      110 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/entry_points.txt
--rw-r--r--   0 greent7    (502) staff       (20)       26 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/requires.txt
--rw-r--r--   0 greent7    (502) staff       (20)        6 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/top_level.txt
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-07 20:32:24.937243 xtalx-1.0.3/
+-rw-r--r--   0 greent7    (502) staff       (20)     1092 2023-06-05 20:34:21.000000 xtalx-1.0.3/LICENSE
+-rw-r--r--   0 greent7    (502) staff       (20)     2685 2023-06-07 20:32:24.937316 xtalx-1.0.3/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)     2190 2023-06-05 20:34:21.000000 xtalx-1.0.3/README.rst
+-rw-r--r--   0 greent7    (502) staff       (20)      782 2023-06-07 20:32:24.937591 xtalx-1.0.3/setup.cfg
+-rw-r--r--   0 greent7    (502) staff       (20)       38 2023-06-05 20:34:21.000000 xtalx-1.0.3/setup.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-07 20:32:24.936155 xtalx-1.0.3/xtalx/
+-rw-r--r--   0 greent7    (502) staff       (20)      222 2023-06-05 20:34:21.000000 xtalx-1.0.3/xtalx/__init__.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-07 20:32:24.937144 xtalx-1.0.3/xtalx/tools/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-06-05 20:34:21.000000 xtalx-1.0.3/xtalx/tools/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      498 2023-06-05 20:34:21.000000 xtalx-1.0.3/xtalx/tools/discover.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1265 2023-06-05 20:34:21.000000 xtalx-1.0.3/xtalx/tools/xtalx_test_read.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3024 2023-06-07 19:01:41.000000 xtalx-1.0.3/xtalx/tools/xtalx_test_yield.py
+-rw-r--r--   0 greent7    (502) staff       (20)    13776 2023-06-05 20:56:37.000000 xtalx-1.0.3/xtalx/xtalx.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-07 20:32:24.936738 xtalx-1.0.3/xtalx.egg-info/
+-rw-r--r--   0 greent7    (502) staff       (20)     2685 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)      357 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/SOURCES.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        1 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/dependency_links.txt
+-rw-r--r--   0 greent7    (502) staff       (20)      110 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/entry_points.txt
+-rw-r--r--   0 greent7    (502) staff       (20)       26 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/requires.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        6 2023-06-07 20:32:24.000000 xtalx-1.0.3/xtalx.egg-info/top_level.txt
```

### Comparing `xtalx-1.0.2/LICENSE` & `xtalx-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xtalx-1.0.2/PKG-INFO` & `xtalx-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtalx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python library for the XtalX sensor.
 Home-page: https://github.com/phasesensors/xtalx_python
 Author: Phase Advanced Sensor Systems Corp.
 Author-email: tgreeniaus@phasesensors.com
 License: MIT
 Keywords: xtalx
 Classifier: Operating System :: OS Independent
```

### Comparing `xtalx-1.0.2/README.rst` & `xtalx-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `xtalx-1.0.2/setup.cfg` & `xtalx-1.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xtalx
-version = 1.0.2
+version = 1.0.3
 author = Phase Advanced Sensor Systems Corp.
 author_email = tgreeniaus@phasesensors.com
 description = Python library for the XtalX sensor.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = xtalx
 url = https://github.com/phasesensors/xtalx_python
```

### Comparing `xtalx-1.0.2/xtalx/tools/xtalx_test_read.py` & `xtalx-1.0.3/xtalx/tools/xtalx_test_read.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.0.2/xtalx/xtalx.py` & `xtalx-1.0.3/xtalx/xtalx.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.0.2/xtalx.egg-info/PKG-INFO` & `xtalx-1.0.3/xtalx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtalx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python library for the XtalX sensor.
 Home-page: https://github.com/phasesensors/xtalx_python
 Author: Phase Advanced Sensor Systems Corp.
 Author-email: tgreeniaus@phasesensors.com
 License: MIT
 Keywords: xtalx
 Classifier: Operating System :: OS Independent
```

