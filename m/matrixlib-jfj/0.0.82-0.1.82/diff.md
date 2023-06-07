# Comparing `tmp/matrixlib_jfj-0.0.82.tar.gz` & `tmp/matrixlib_jfj-0.1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixlib_jfj-0.0.82.tar", last modified: Wed Jun  7 19:40:36 2023, max compression
+gzip compressed data, was "matrixlib_jfj-0.1.82.tar", last modified: Wed Jun  7 20:02:43 2023, max compression
```

## Comparing `matrixlib_jfj-0.0.82.tar` & `matrixlib_jfj-0.1.82.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 19:40:36.388260 matrixlib_jfj-0.0.82/
--rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.82/LICENSE.md
--rw-rw-rw-   0        0        0     3249 2023-06-07 19:40:36.389263 matrixlib_jfj-0.0.82/PKG-INFO
--rw-rw-rw-   0        0        0     2366 2023-06-07 19:40:29.000000 matrixlib_jfj-0.0.82/README.md
--rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.82/pyproject.toml
--rw-rw-rw-   0        0        0     1003 2023-06-07 19:40:36.400158 matrixlib_jfj-0.0.82/setup.cfg
--rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.82/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:40:36.258697 matrixlib_jfj-0.0.82/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 19:40:36.339233 matrixlib_jfj-0.0.82/src/matrixlib_jfj/
--rw-rw-rw-   0        0        0      962 2023-06-07 19:40:07.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj/__init__.py
--rw-rw-rw-   0        0        0    14754 2023-06-07 19:39:13.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj/matrix.py
--rw-rw-rw-   0        0        0      461 2023-06-07 15:32:43.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj/utils.py
--rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj/vector.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:40:36.384343 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/
--rw-rw-rw-   0        0        0     3249 2023-06-07 19:40:35.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-06-07 19:40:36.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 19:40:35.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-07 19:40:35.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 19:40:35.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 20:02:43.523793 matrixlib_jfj-0.1.82/
+-rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.82/LICENSE.md
+-rw-rw-rw-   0        0        0     3391 2023-06-07 20:02:43.523793 matrixlib_jfj-0.1.82/PKG-INFO
+-rw-rw-rw-   0        0        0     2504 2023-06-07 20:02:38.000000 matrixlib_jfj-0.1.82/README.md
+-rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.82/pyproject.toml
+-rw-rw-rw-   0        0        0     1003 2023-06-07 20:02:43.529775 matrixlib_jfj-0.1.82/setup.cfg
+-rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.82/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:02:43.390399 matrixlib_jfj-0.1.82/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 20:02:43.475231 matrixlib_jfj-0.1.82/src/matrixlib_jfj/
+-rw-rw-rw-   0        0        0      962 2023-06-07 20:01:06.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj/__init__.py
+-rw-rw-rw-   0        0        0    14748 2023-06-07 19:46:02.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj/matrix.py
+-rw-rw-rw-   0        0        0       35 2023-06-07 19:57:42.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj/utils.py
+-rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj/vector.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:02:43.520798 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/
+-rw-rw-rw-   0        0        0     3391 2023-06-07 20:02:43.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-06-07 20:02:43.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 20:02:43.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-07 20:02:43.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 20:02:43.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/top_level.txt
```

### Comparing `matrixlib_jfj-0.0.82/LICENSE.md` & `matrixlib_jfj-0.1.82/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.82/PKG-INFO` & `matrixlib_jfj-0.1.82/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib_jfj
-Version: 0.0.82
+Version: 0.1.82
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
@@ -114,14 +114,18 @@
 Updated README file to reflect certain information.
 <br>
 
 ## Update 0.0.82
 Fixed Type Annotations.
 <br>
 
+## Update 0.1.82
+Removed Deprecations, Removed functionality in utils.py (Temporary) added better typing, improved cumsum function.
+<br>
+
 # Contributing
 
 ---
 Any and All feedback and help is highly encouraged. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 <br>
```

### Comparing `matrixlib_jfj-0.0.82/README.md` & `matrixlib_jfj-0.1.82/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -96,14 +96,18 @@
 Updated README file to reflect certain information.
 <br>
 
 ## Update 0.0.82
 Fixed Type Annotations.
 <br>
 
+## Update 0.1.82
+Removed Deprecations, Removed functionality in utils.py (Temporary) added better typing, improved cumsum function.
+<br>
+
 # Contributing
 
 ---
 Any and All feedback and help is highly encouraged. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 <br>
```

### Comparing `matrixlib_jfj-0.0.82/pyproject.toml` & `matrixlib_jfj-0.1.82/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.82/setup.cfg` & `matrixlib_jfj-0.1.82/setup.cfg`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.82/src/matrixlib_jfj/__init__.py` & `matrixlib_jfj-0.1.82/src/matrixlib_jfj/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
  	print(transposed) # Output:
 
  	0 0 0\n
 	0 0 0\n
  	6 0 0
 
-Version: 0.0.82
+Version: 0.1.82
 
 Author: Jemma Starecki
 
 Made By <a href="https://github.com/JemmaFromJupiter" target="_blank">JemmaFromJupiter</a> On Github.
 """
 from __future__ import annotations
 from . import matrix
 from . import vector
 from . import utils
 
-__version__ = "0.0.82"
+__version__ = "0.1.82"
 __author__ = "JemmaFromJupiter"
 
 __all__ = [
 	"matrix",
 	"vector",
 	"utils"
 ]
```

### Comparing `matrixlib_jfj-0.0.82/src/matrixlib_jfj/matrix.py` & `matrixlib_jfj-0.1.82/src/matrixlib_jfj/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import Union, Optional
 import math
 import random as r
 import numpy as np
-"""from . import vector
-from . import utils"""
+from . import vector
+from . import utils
 
 class Matrix(list[list[float]]):
 	"""Initialises a Matrix that can be used for numerous things
 
 Parameters
 ----------
 rowcols (Union[tuple, list]) : The how many rows and columns are in the matrix.
```

### Comparing `matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/PKG-INFO` & `matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib-jfj
-Version: 0.0.82
+Version: 0.1.82
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
@@ -114,14 +114,18 @@
 Updated README file to reflect certain information.
 <br>
 
 ## Update 0.0.82
 Fixed Type Annotations.
 <br>
 
+## Update 0.1.82
+Removed Deprecations, Removed functionality in utils.py (Temporary) added better typing, improved cumsum function.
+<br>
+
 # Contributing
 
 ---
 Any and All feedback and help is highly encouraged. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 <br>
```

