# Comparing `tmp/prettyc-1.0.1.tar.gz` & `tmp/prettyc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettyc-1.0.1.tar", last modified: Wed Jun  7 13:56:16 2023, max compression
+gzip compressed data, was "prettyc-1.0.2.tar", last modified: Wed Jun  7 14:03:34 2023, max compression
```

## Comparing `prettyc-1.0.1.tar` & `prettyc-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 13:56:16.228129 prettyc-1.0.1/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.1/LICENSE
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1688 2023-06-07 13:56:16.228129 prettyc-1.0.1/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      753 2023-06-07 13:13:13.000000 prettyc-1.0.1/README.md
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 13:56:16.228129 prettyc-1.0.1/prettyc.egg-info/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1688 2023-06-07 13:56:16.000000 prettyc-1.0.1/prettyc.egg-info/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-07 13:56:16.000000 prettyc-1.0.1/prettyc.egg-info/SOURCES.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-07 13:56:16.000000 prettyc-1.0.1/prettyc.egg-info/dependency_links.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-07 13:56:16.000000 prettyc-1.0.1/prettyc.egg-info/entry_points.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-07 13:56:16.000000 prettyc-1.0.1/prettyc.egg-info/top_level.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)   261617 2023-06-07 13:54:04.000000 prettyc-1.0.1/prettyc.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-07 13:56:16.228129 prettyc-1.0.1/setup.cfg
--rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.1/setup.py
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 14:03:34.332135 prettyc-1.0.2/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.2/LICENSE
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-07 14:03:34.332135 prettyc-1.0.2/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      797 2023-06-07 14:02:40.000000 prettyc-1.0.2/README.md
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 14:03:34.332135 prettyc-1.0.2/prettyc.egg-info/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-07 14:03:34.000000 prettyc-1.0.2/prettyc.egg-info/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-07 14:03:34.000000 prettyc-1.0.2/prettyc.egg-info/SOURCES.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-07 14:03:34.000000 prettyc-1.0.2/prettyc.egg-info/dependency_links.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-07 14:03:34.000000 prettyc-1.0.2/prettyc.egg-info/entry_points.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-07 14:03:34.000000 prettyc-1.0.2/prettyc.egg-info/top_level.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)   261617 2023-06-07 14:03:02.000000 prettyc-1.0.2/prettyc.py
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-07 14:03:34.332135 prettyc-1.0.2/setup.cfg
+-rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.2/setup.py
```

### Comparing `prettyc-1.0.1/LICENSE` & `prettyc-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.1/PKG-INFO` & `prettyc-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
@@ -47,14 +47,20 @@
 For full usage instructions, run:
 
 
 ```bash
 prettyc --help
 ```
 
+## How to use:
+
+```bash
+prettyc --help
+```
+
 ## Development
 
 Create virtual environment.
 ```bash
 make venv
 ```
```

### Comparing `prettyc-1.0.1/README.md` & `prettyc-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 For full usage instructions, run:
 
 
 ```bash
 prettyc --help
 ```
 
+## How to use:
+
+```bash
+prettyc --help
+```
+
 ## Development
 
 Create virtual environment.
 ```bash
 make venv
 ```
```

### Comparing `prettyc-1.0.1/prettyc.egg-info/PKG-INFO` & `prettyc-1.0.2/prettyc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
@@ -47,14 +47,20 @@
 For full usage instructions, run:
 
 
 ```bash
 prettyc --help
 ```
 
+## How to use:
+
+```bash
+prettyc --help
+```
+
 ## Development
 
 Create virtual environment.
 ```bash
 make venv
 ```
```

### Comparing `prettyc-1.0.1/prettyc.py` & `prettyc-1.0.2/prettyc.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 import sysconfig
 import unicodedata
 import xml.etree.ElementTree
 
 # if empty, use defaults
 _valid_extensions = set([])
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 __verbose__ = False
 
 try:
   #  -- pylint: disable=used-before-assignment
   xrange          # Python 2
 except NameError:
   #  -- pylint: disable=redefined-builtin
```

### Comparing `prettyc-1.0.1/setup.py` & `prettyc-1.0.2/setup.py`

 * *Files identical despite different names*

