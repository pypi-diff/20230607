# Comparing `tmp/matrixlib_jfj-0.1.82.tar.gz` & `tmp/matrixlib_jfj-0.1.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixlib_jfj-0.1.82.tar", last modified: Wed Jun  7 20:02:43 2023, max compression
+gzip compressed data, was "matrixlib_jfj-0.1.83.tar", last modified: Wed Jun  7 20:09:00 2023, max compression
```

## Comparing `matrixlib_jfj-0.1.82.tar` & `matrixlib_jfj-0.1.83.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 20:02:43.523793 matrixlib_jfj-0.1.82/
--rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.82/LICENSE.md
--rw-rw-rw-   0        0        0     3391 2023-06-07 20:02:43.523793 matrixlib_jfj-0.1.82/PKG-INFO
--rw-rw-rw-   0        0        0     2504 2023-06-07 20:02:38.000000 matrixlib_jfj-0.1.82/README.md
--rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.82/pyproject.toml
--rw-rw-rw-   0        0        0     1003 2023-06-07 20:02:43.529775 matrixlib_jfj-0.1.82/setup.cfg
--rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.82/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:02:43.390399 matrixlib_jfj-0.1.82/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 20:02:43.475231 matrixlib_jfj-0.1.82/src/matrixlib_jfj/
--rw-rw-rw-   0        0        0      962 2023-06-07 20:01:06.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj/__init__.py
--rw-rw-rw-   0        0        0    14748 2023-06-07 19:46:02.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj/matrix.py
--rw-rw-rw-   0        0        0       35 2023-06-07 19:57:42.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj/utils.py
--rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj/vector.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:02:43.520798 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/
--rw-rw-rw-   0        0        0     3391 2023-06-07 20:02:43.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-06-07 20:02:43.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 20:02:43.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-07 20:02:43.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 20:02:43.000000 matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 20:09:00.182506 matrixlib_jfj-0.1.83/
+-rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.83/LICENSE.md
+-rw-rw-rw-   0        0        0     3391 2023-06-07 20:09:00.183488 matrixlib_jfj-0.1.83/PKG-INFO
+-rw-rw-rw-   0        0        0     2504 2023-06-07 20:02:38.000000 matrixlib_jfj-0.1.83/README.md
+-rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.83/pyproject.toml
+-rw-rw-rw-   0        0        0     1003 2023-06-07 20:09:00.190739 matrixlib_jfj-0.1.83/setup.cfg
+-rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.83/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:09:00.049036 matrixlib_jfj-0.1.83/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 20:09:00.139153 matrixlib_jfj-0.1.83/src/matrixlib_jfj/
+-rw-rw-rw-   0        0        0      962 2023-06-07 20:08:54.000000 matrixlib_jfj-0.1.83/src/matrixlib_jfj/__init__.py
+-rw-rw-rw-   0        0        0    14749 2023-06-07 20:08:07.000000 matrixlib_jfj-0.1.83/src/matrixlib_jfj/matrix.py
+-rw-rw-rw-   0        0        0       35 2023-06-07 19:57:42.000000 matrixlib_jfj-0.1.83/src/matrixlib_jfj/utils.py
+-rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.1.83/src/matrixlib_jfj/vector.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:09:00.177505 matrixlib_jfj-0.1.83/src/matrixlib_jfj.egg-info/
+-rw-rw-rw-   0        0        0     3391 2023-06-07 20:08:59.000000 matrixlib_jfj-0.1.83/src/matrixlib_jfj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-06-07 20:08:59.000000 matrixlib_jfj-0.1.83/src/matrixlib_jfj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 20:08:59.000000 matrixlib_jfj-0.1.83/src/matrixlib_jfj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-07 20:08:59.000000 matrixlib_jfj-0.1.83/src/matrixlib_jfj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 20:08:59.000000 matrixlib_jfj-0.1.83/src/matrixlib_jfj.egg-info/top_level.txt
```

### Comparing `matrixlib_jfj-0.1.82/LICENSE.md` & `matrixlib_jfj-0.1.83/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.1.82/PKG-INFO` & `matrixlib_jfj-0.1.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib_jfj
-Version: 0.1.82
+Version: 0.1.83
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `matrixlib_jfj-0.1.82/README.md` & `matrixlib_jfj-0.1.83/README.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.1.82/pyproject.toml` & `matrixlib_jfj-0.1.83/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.1.82/setup.cfg` & `matrixlib_jfj-0.1.83/setup.cfg`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.1.82/src/matrixlib_jfj/__init__.py` & `matrixlib_jfj-0.1.83/src/matrixlib_jfj/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
  	print(transposed) # Output:
 
  	0 0 0\n
 	0 0 0\n
  	6 0 0
 
-Version: 0.1.82
+Version: 0.1.83
 
 Author: Jemma Starecki
 
 Made By <a href="https://github.com/JemmaFromJupiter" target="_blank">JemmaFromJupiter</a> On Github.
 """
 from __future__ import annotations
 from . import matrix
 from . import vector
 from . import utils
 
-__version__ = "0.1.82"
+__version__ = "0.1.83"
 __author__ = "JemmaFromJupiter"
 
 __all__ = [
 	"matrix",
 	"vector",
 	"utils"
 ]
```

### Comparing `matrixlib_jfj-0.1.82/src/matrixlib_jfj/matrix.py` & `matrixlib_jfj-0.1.83/src/matrixlib_jfj/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,15 +446,15 @@
 
 	def __isub__(self, other: Matrix | float) -> Matrix:
 		return self - other
 
 	def __rsub__(self, other: Matrix | float) -> Matrix:
 		return self - other
 
-	def __mul__(self, other: int, float) -> Matrix:
+	def __mul__(self, other: int | float) -> Matrix:
 		if isinstance(other, Matrix):
 			return self @ other
 		result = Matrix(self.get_shape())
 		for i in range(len(self)):
 			for j in range(len(self[0])):
 				result.set_value(i, j, self.get_value(i, j) * other)
```

### Comparing `matrixlib_jfj-0.1.82/src/matrixlib_jfj.egg-info/PKG-INFO` & `matrixlib_jfj-0.1.83/src/matrixlib_jfj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib-jfj
-Version: 0.1.82
+Version: 0.1.83
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

