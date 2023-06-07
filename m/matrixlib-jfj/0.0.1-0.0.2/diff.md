# Comparing `tmp/matrixlib_jfj-0.0.1.tar.gz` & `tmp/matrixlib_jfj-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixlib_jfj-0.0.1.tar", last modified: Wed Jun  7 01:20:59 2023, max compression
+gzip compressed data, was "matrixlib_jfj-0.0.2.tar", last modified: Wed Jun  7 01:50:23 2023, max compression
```

## Comparing `matrixlib_jfj-0.0.1.tar` & `matrixlib_jfj-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:20:59.880294 matrixlib_jfj-0.0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)    35148 2023-06-06 20:50:00.000000 matrixlib_jfj-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 01:20:59.880294 matrixlib_jfj-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-06-06 20:36:36.000000 matrixlib_jfj-0.0.1/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)     1014 2023-06-07 01:18:30.000000 matrixlib_jfj-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      965 2023-06-07 01:20:59.880294 matrixlib_jfj-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)       65 2023-06-07 01:15:59.000000 matrixlib_jfj-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:20:59.872294 matrixlib_jfj-0.0.1/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:20:59.876294 matrixlib_jfj-0.0.1/src/matrixlib_jfj/
--rw-r--r--   0 runner    (1000) runner    (1000)      960 2023-06-07 01:20:44.000000 matrixlib_jfj-0.0.1/src/matrixlib_jfj/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13427 2023-06-07 01:14:49.000000 matrixlib_jfj-0.0.1/src/matrixlib_jfj/matrix.py
--rw-r--r--   0 runner    (1000) runner    (1000)      270 2023-06-07 01:15:01.000000 matrixlib_jfj-0.0.1/src/matrixlib_jfj/utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)      213 2023-06-07 01:15:14.000000 matrixlib_jfj-0.0.1/src/matrixlib_jfj/vector.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:20:59.880294 matrixlib_jfj-0.0.1/src/matrixlib_jfj.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 01:20:59.000000 matrixlib_jfj-0.0.1/src/matrixlib_jfj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      371 2023-06-07 01:20:59.000000 matrixlib_jfj-0.0.1/src/matrixlib_jfj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-07 01:20:59.000000 matrixlib_jfj-0.0.1/src/matrixlib_jfj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2023-06-07 01:20:59.000000 matrixlib_jfj-0.0.1/src/matrixlib_jfj.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-06-07 01:20:59.000000 matrixlib_jfj-0.0.1/src/matrixlib_jfj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:50:23.477674 matrixlib_jfj-0.0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)    35148 2023-06-06 20:50:00.000000 matrixlib_jfj-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 01:50:23.477674 matrixlib_jfj-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-06-06 20:36:36.000000 matrixlib_jfj-0.0.2/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)     1014 2023-06-07 01:46:06.000000 matrixlib_jfj-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      965 2023-06-07 01:50:23.481674 matrixlib_jfj-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)       65 2023-06-07 01:15:59.000000 matrixlib_jfj-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:50:23.473674 matrixlib_jfj-0.0.2/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:50:23.477674 matrixlib_jfj-0.0.2/src/matrixlib_jfj/
+-rw-r--r--   0 runner    (1000) runner    (1000)      960 2023-06-07 01:50:21.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13499 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj/matrix.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      270 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj/utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      213 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj/vector.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:50:23.477674 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 01:50:23.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      371 2023-06-07 01:50:23.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-07 01:50:23.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2023-06-07 01:50:23.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-06-07 01:50:23.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/top_level.txt
```

### Comparing `matrixlib_jfj-0.0.1/LICENSE.md` & `matrixlib_jfj-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.1/PKG-INFO` & `matrixlib_jfj-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib_jfj
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `matrixlib_jfj-0.0.1/pyproject.toml` & `matrixlib_jfj-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.1/setup.cfg` & `matrixlib_jfj-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.1/src/matrixlib_jfj/__init__.py` & `matrixlib_jfj-0.0.2/src/matrixlib_jfj/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
  	print(transposed) # Output:
 
  	0 0 0\n
 	0 0 0\n
  	6 0 0
 
-Version: 0.0.1
+Version: 0.0.2
 
 Author: Jemma Starecki
 
 Made By <a href="https://github.com/JemmaFromJupiter" target="_blank">JemmaFromJupiter</a> On Github.
 """
 from __future__ import annotations
 from . import matrix
 from . import vector
 from . import utils
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __author__ = "JemmaFromJupiter"
 
 __all__ = [
 	"matrix",
 	"vector",
 	"utils"
 ]
```

### Comparing `matrixlib_jfj-0.0.1/src/matrixlib_jfj/matrix.py` & `matrixlib_jfj-0.0.2/src/matrixlib_jfj/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 from typing import Union, Optional
 import math
 import random as r
-from . import vector
-from . import utils
+"""from . import vector
+from . import utils"""
 
 class Matrix(list):
 	"""Initialises a Matrix that can be used for numerous things
 
 Parameters
 ----------
 rowcols (Union[tuple, list]) : The how many rows and columns are in the matrix.
@@ -87,16 +87,18 @@
 			return super().__new__(cls, rowcols=rowcols)
 		if values is not None:
 			return super().__new__(cls, values=values)
 
 	def __init__(self, rowcols: Union[tuple, list] = None, values: list = None):
 		if rowcols is not None:
 			super().__init__([[0] * rowcols[1] for _ in range(rowcols[0])])
+			self.shape = self.get_shape()
 		if values is not None:
 			super().__init__(values)
+			self.shape = self.get_shape()
 
 	def __str__(self):
 		rows = self.get_shape()[0]
 		max = len(str(self.max()))
 		result = []
 		for row in range(rows):
 			result.append("|" + "   ".join(map(lambda el: f"{el:^{max}}", self[row])) + "|\n")
```

### Comparing `matrixlib_jfj-0.0.1/src/matrixlib_jfj.egg-info/PKG-INFO` & `matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib-jfj
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

