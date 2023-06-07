# Comparing `tmp/plugin2cube-2.2.6.tar.gz` & `tmp/plugin2cube-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugin2cube-2.2.6.tar", last modified: Fri Jan 20 23:12:29 2023, max compression
+gzip compressed data, was "plugin2cube-2.2.8.tar", last modified: Sat Jan 21 20:06:47 2023, max compression
```

## Comparing `plugin2cube-2.2.6.tar` & `plugin2cube-2.2.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-20 23:12:29.790956 plugin2cube-2.2.6/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2023-01-06 22:23:07.000000 plugin2cube-2.2.6/LICENSE
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8226 2023-01-20 23:12:29.790956 plugin2cube-2.2.6/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7660 2023-01-20 23:11:15.000000 plugin2cube-2.2.6/README.rst
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-20 23:12:29.788956 plugin2cube-2.2.6/control/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    19000 2023-01-20 23:09:41.000000 plugin2cube-2.2.6/control/action.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     2543 2023-01-06 22:23:07.000000 plugin2cube-2.2.6/control/filter.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     5982 2023-01-19 17:02:38.000000 plugin2cube-2.2.6/control/jobber.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-20 23:12:29.789955 plugin2cube-2.2.6/logic/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      915 2023-01-06 22:23:07.000000 plugin2cube-2.2.6/logic/behavior.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-20 23:12:29.789955 plugin2cube-2.2.6/plugin2cube/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-12 20:07:08.000000 plugin2cube-2.2.6/plugin2cube/__init__.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    15137 2023-01-20 22:57:09.000000 plugin2cube-2.2.6/plugin2cube/__main__.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     4415 2023-01-20 22:58:33.000000 plugin2cube-2.2.6/plugin2cube/plugin2cube.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-20 23:12:29.789955 plugin2cube-2.2.6/plugin2cube.egg-info/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8226 2023-01-20 23:12:29.000000 plugin2cube-2.2.6/plugin2cube.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      400 2023-01-20 23:12:29.000000 plugin2cube-2.2.6/plugin2cube.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-01-20 23:12:29.000000 plugin2cube-2.2.6/plugin2cube.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       58 2023-01-20 23:12:29.000000 plugin2cube-2.2.6/plugin2cube.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       75 2023-01-20 23:12:29.000000 plugin2cube-2.2.6/plugin2cube.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       32 2023-01-20 23:12:29.000000 plugin2cube-2.2.6/plugin2cube.egg-info/top_level.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2023-01-20 23:12:29.790956 plugin2cube-2.2.6/setup.cfg
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1919 2023-01-12 19:51:13.000000 plugin2cube-2.2.6/setup.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-20 23:12:29.789955 plugin2cube-2.2.6/state/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8330 2023-01-20 16:54:59.000000 plugin2cube-2.2.6/state/data.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-21 20:06:47.453184 plugin2cube-2.2.8/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2023-01-06 22:23:07.000000 plugin2cube-2.2.8/LICENSE
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8226 2023-01-21 20:06:47.453184 plugin2cube-2.2.8/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7660 2023-01-20 23:11:15.000000 plugin2cube-2.2.8/README.rst
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-21 20:06:47.451184 plugin2cube-2.2.8/control/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    19000 2023-01-20 23:09:41.000000 plugin2cube-2.2.8/control/action.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     2543 2023-01-06 22:23:07.000000 plugin2cube-2.2.8/control/filter.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     5982 2023-01-19 17:02:38.000000 plugin2cube-2.2.8/control/jobber.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-21 20:06:47.451184 plugin2cube-2.2.8/logic/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      915 2023-01-06 22:23:07.000000 plugin2cube-2.2.8/logic/behavior.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-21 20:06:47.451184 plugin2cube-2.2.8/plugin2cube/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-12 20:07:08.000000 plugin2cube-2.2.8/plugin2cube/__init__.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    15137 2023-01-20 22:57:09.000000 plugin2cube-2.2.8/plugin2cube/__main__.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     4415 2023-01-21 20:05:55.000000 plugin2cube-2.2.8/plugin2cube/plugin2cube.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-21 20:06:47.452184 plugin2cube-2.2.8/plugin2cube.egg-info/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8226 2023-01-21 20:06:46.000000 plugin2cube-2.2.8/plugin2cube.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      400 2023-01-21 20:06:47.000000 plugin2cube-2.2.8/plugin2cube.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-01-21 20:06:46.000000 plugin2cube-2.2.8/plugin2cube.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       58 2023-01-21 20:06:47.000000 plugin2cube-2.2.8/plugin2cube.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       75 2023-01-21 20:06:47.000000 plugin2cube-2.2.8/plugin2cube.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       32 2023-01-21 20:06:47.000000 plugin2cube-2.2.8/plugin2cube.egg-info/top_level.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2023-01-21 20:06:47.453184 plugin2cube-2.2.8/setup.cfg
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1919 2023-01-12 19:51:13.000000 plugin2cube-2.2.8/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-01-21 20:06:47.452184 plugin2cube-2.2.8/state/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8363 2023-01-21 20:05:35.000000 plugin2cube-2.2.8/state/data.py
```

### Comparing `plugin2cube-2.2.6/LICENSE` & `plugin2cube-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `plugin2cube-2.2.6/PKG-INFO` & `plugin2cube-2.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugin2cube
-Version: 2.2.6
+Version: 2.2.8
 Summary: A ChRIS helper app that registers a plugin to a CUBE instance
 Home-page: https://github.com/FNNDSC/plugin2cube
 Author: FNNDSC
 Author-email: rudolph.pienaar@childrens.harvard.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `plugin2cube-2.2.6/README.rst` & `plugin2cube-2.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `plugin2cube-2.2.6/control/action.py` & `plugin2cube-2.2.8/control/action.py`

 * *Files identical despite different names*

### Comparing `plugin2cube-2.2.6/control/filter.py` & `plugin2cube-2.2.8/control/filter.py`

 * *Files identical despite different names*

### Comparing `plugin2cube-2.2.6/control/jobber.py` & `plugin2cube-2.2.8/control/jobber.py`

 * *Files identical despite different names*

### Comparing `plugin2cube-2.2.6/logic/behavior.py` & `plugin2cube-2.2.8/logic/behavior.py`

 * *Files identical despite different names*

### Comparing `plugin2cube-2.2.6/plugin2cube/__main__.py` & `plugin2cube-2.2.8/plugin2cube/__main__.py`

 * *Files identical despite different names*

### Comparing `plugin2cube-2.2.6/plugin2cube/plugin2cube.py` & `plugin2cube-2.2.8/plugin2cube/plugin2cube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-__version__ = '2.2.6'
+__version__ = '2.2.8'
 
 from    pathlib                 import Path
 
 import  os, sys, json
 import  pudb
 from    pudb.remote             import set_trace
```

### Comparing `plugin2cube-2.2.6/plugin2cube.egg-info/PKG-INFO` & `plugin2cube-2.2.8/plugin2cube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugin2cube
-Version: 2.2.6
+Version: 2.2.8
 Summary: A ChRIS helper app that registers a plugin to a CUBE instance
 Home-page: https://github.com/FNNDSC/plugin2cube
 Author: FNNDSC
 Author-email: rudolph.pienaar@childrens.harvard.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `plugin2cube-2.2.6/setup.py` & `plugin2cube-2.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `plugin2cube-2.2.6/state/data.py` & `plugin2cube-2.2.8/state/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         self.CUBE       : CUBEinstance      = CUBEinstance()
         self.debug      : dict              = {
             'do'        : False,
             'termsize'  : (80,25),
             'port'      : 7900,
             'host'      : '0.0.0.0'
         }
+        os.chdir(self._inputdir)
 
     def DEBUG(self, *args, **kwargs):
         level   : int   = 1
         for k,v in kwargs.items():
             if k == 'level' : level = v
         if int(self.options.verbosity) >= level:
             logger.opt(depth=1, colors=True).debug(*args)
```

