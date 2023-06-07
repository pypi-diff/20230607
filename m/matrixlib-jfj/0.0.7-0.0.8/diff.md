# Comparing `tmp/matrixlib_jfj-0.0.7.tar.gz` & `tmp/matrixlib_jfj-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixlib_jfj-0.0.7.tar", last modified: Wed Jun  7 16:46:24 2023, max compression
+gzip compressed data, was "matrixlib_jfj-0.0.8.tar", last modified: Wed Jun  7 16:54:01 2023, max compression
```

## Comparing `matrixlib_jfj-0.0.7.tar` & `matrixlib_jfj-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 16:46:24.928056 matrixlib_jfj-0.0.7/
--rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.7/LICENSE.md
--rw-rw-rw-   0        0        0     1116 2023-06-07 16:46:24.929057 matrixlib_jfj-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.7/README.md
--rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0     1003 2023-06-07 16:46:24.937031 matrixlib_jfj-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:46:24.820295 matrixlib_jfj-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 16:46:24.891804 matrixlib_jfj-0.0.7/src/matrixlib_jfj/
--rw-rw-rw-   0        0        0      960 2023-06-07 16:46:09.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj/__init__.py
--rw-rw-rw-   0        0        0    15021 2023-06-07 16:37:30.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj/matrix.py
--rw-rw-rw-   0        0        0      461 2023-06-07 15:32:43.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj/utils.py
--rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj/vector.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:46:24.924071 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/
--rw-rw-rw-   0        0        0     1116 2023-06-07 16:46:24.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-06-07 16:46:24.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 16:46:24.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-07 16:46:24.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 16:46:24.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 16:54:01.077444 matrixlib_jfj-0.0.8/
+-rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.8/LICENSE.md
+-rw-rw-rw-   0        0        0     1407 2023-06-07 16:54:01.077444 matrixlib_jfj-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-06-07 16:53:28.000000 matrixlib_jfj-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1003 2023-06-07 16:54:01.086422 matrixlib_jfj-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:54:00.964707 matrixlib_jfj-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 16:54:01.037549 matrixlib_jfj-0.0.8/src/matrixlib_jfj/
+-rw-rw-rw-   0        0        0      960 2023-06-07 16:53:35.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj/__init__.py
+-rw-rw-rw-   0        0        0    14898 2023-06-07 16:51:26.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj/matrix.py
+-rw-rw-rw-   0        0        0      461 2023-06-07 15:32:43.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj/utils.py
+-rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj/vector.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:54:01.073454 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/
+-rw-rw-rw-   0        0        0     1407 2023-06-07 16:54:00.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-06-07 16:54:00.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 16:54:00.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-07 16:54:00.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 16:54:00.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/top_level.txt
```

### Comparing `matrixlib_jfj-0.0.7/LICENSE.md` & `matrixlib_jfj-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.7/PKG-INFO` & `matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: matrixlib_jfj
-Version: 0.0.7
+Name: matrixlib-jfj
+Version: 0.0.8
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
@@ -14,7 +14,13 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Matrixlib
 A basic library for matrix and vector operations. Any feedback is highly encouraged. I enjoy trying to create modules and programs that work with mathematical functions and data. I also like looking into higher end modules and researching the processes and programs they use to perform tasks. Any feedback will be taken and acted upon.
+
+# Update 0.0.7
+Added "get_submatrix" function that gets the submatrix of any square matrix, added the "det" function which gets the determinant of a square matrix.
+
+# Update 0.0.8
+Fixed bug where an external program would run when the user of the package would run their own program.
```

### Comparing `matrixlib_jfj-0.0.7/pyproject.toml` & `matrixlib_jfj-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.7/setup.cfg` & `matrixlib_jfj-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.7/src/matrixlib_jfj/__init__.py` & `matrixlib_jfj-0.0.8/src/matrixlib_jfj/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
  	print(transposed) # Output:
 
  	0 0 0\n
 	0 0 0\n
  	6 0 0
 
-Version: 0.0.7
+Version: 0.0.8
 
 Author: Jemma Starecki
 
 Made By <a href="https://github.com/JemmaFromJupiter" target="_blank">JemmaFromJupiter</a> On Github.
 """
 from __future__ import annotations
 from . import matrix
 from . import vector
 from . import utils
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 __author__ = "JemmaFromJupiter"
 
 __all__ = [
 	"matrix",
 	"vector",
 	"utils"
 ]
```

### Comparing `matrixlib_jfj-0.0.7/src/matrixlib_jfj/matrix.py` & `matrixlib_jfj-0.0.8/src/matrixlib_jfj/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import Union, Optional
 import math
 import random as r
 import numpy as np
-# from . import vector
-# from . import utils
+from . import vector
+from . import utils
 
 class Matrix(list):
 	"""Initialises a Matrix that can be used for numerous things
 
 Parameters
 ----------
 rowcols (Union[tuple, list]) : The how many rows and columns are in the matrix.
@@ -579,16 +579,8 @@
 					if self[i][j] == other[i][j]:
 						return False
 			return True
 		else:
 			return False
 		
 	def max(self):
-		return max(max(self, key=max))
-	
-matrix = Matrix(rowcols=(10, 10))
-
-matrix.random(1, 100)
-
-print(matrix, end="\n\n")
-
-print(matrix.det(), end="\n\n")
+		return max(max(self, key=max))
```

### Comparing `matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/PKG-INFO` & `matrixlib_jfj-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: matrixlib-jfj
-Version: 0.0.7
+Name: matrixlib_jfj
+Version: 0.0.8
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
@@ -14,7 +14,13 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Matrixlib
 A basic library for matrix and vector operations. Any feedback is highly encouraged. I enjoy trying to create modules and programs that work with mathematical functions and data. I also like looking into higher end modules and researching the processes and programs they use to perform tasks. Any feedback will be taken and acted upon.
+
+# Update 0.0.7
+Added "get_submatrix" function that gets the submatrix of any square matrix, added the "det" function which gets the determinant of a square matrix.
+
+# Update 0.0.8
+Fixed bug where an external program would run when the user of the package would run their own program.
```

