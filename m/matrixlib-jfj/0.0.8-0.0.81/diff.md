# Comparing `tmp/matrixlib_jfj-0.0.8.tar.gz` & `tmp/matrixlib_jfj-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixlib_jfj-0.0.8.tar", last modified: Wed Jun  7 16:54:01 2023, max compression
+gzip compressed data, was "matrixlib_jfj-0.0.81.tar", last modified: Wed Jun  7 17:28:01 2023, max compression
```

## Comparing `matrixlib_jfj-0.0.8.tar` & `matrixlib_jfj-0.0.81.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 16:54:01.077444 matrixlib_jfj-0.0.8/
--rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.8/LICENSE.md
--rw-rw-rw-   0        0        0     1407 2023-06-07 16:54:01.077444 matrixlib_jfj-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-06-07 16:53:28.000000 matrixlib_jfj-0.0.8/README.md
--rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1003 2023-06-07 16:54:01.086422 matrixlib_jfj-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:54:00.964707 matrixlib_jfj-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 16:54:01.037549 matrixlib_jfj-0.0.8/src/matrixlib_jfj/
--rw-rw-rw-   0        0        0      960 2023-06-07 16:53:35.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj/__init__.py
--rw-rw-rw-   0        0        0    14898 2023-06-07 16:51:26.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj/matrix.py
--rw-rw-rw-   0        0        0      461 2023-06-07 15:32:43.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj/utils.py
--rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj/vector.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:54:01.073454 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/
--rw-rw-rw-   0        0        0     1407 2023-06-07 16:54:00.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-06-07 16:54:00.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 16:54:00.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-07 16:54:00.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 16:54:00.000000 matrixlib_jfj-0.0.8/src/matrixlib_jfj.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 17:28:01.077806 matrixlib_jfj-0.0.81/
+-rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.81/LICENSE.md
+-rw-rw-rw-   0        0        0     3198 2023-06-07 17:28:01.078801 matrixlib_jfj-0.0.81/PKG-INFO
+-rw-rw-rw-   0        0        0     2319 2023-06-07 17:27:42.000000 matrixlib_jfj-0.0.81/README.md
+-rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.81/pyproject.toml
+-rw-rw-rw-   0        0        0     1003 2023-06-07 17:28:01.085795 matrixlib_jfj-0.0.81/setup.cfg
+-rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.81/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:28:00.983034 matrixlib_jfj-0.0.81/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 17:28:01.043899 matrixlib_jfj-0.0.81/src/matrixlib_jfj/
+-rw-rw-rw-   0        0        0      962 2023-06-07 17:27:55.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj/__init__.py
+-rw-rw-rw-   0        0        0    14926 2023-06-07 17:13:01.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj/matrix.py
+-rw-rw-rw-   0        0        0      461 2023-06-07 15:32:43.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj/utils.py
+-rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj/vector.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:28:01.074813 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/
+-rw-rw-rw-   0        0        0     3198 2023-06-07 17:28:00.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-06-07 17:28:00.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 17:28:00.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-07 17:28:00.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 17:28:00.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/top_level.txt
```

### Comparing `matrixlib_jfj-0.0.8/LICENSE.md` & `matrixlib_jfj-0.0.81/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.8/pyproject.toml` & `matrixlib_jfj-0.0.81/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.8/setup.cfg` & `matrixlib_jfj-0.0.81/setup.cfg`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.8/src/matrixlib_jfj/__init__.py` & `matrixlib_jfj-0.0.81/src/matrixlib_jfj/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
  	print(transposed) # Output:
 
  	0 0 0\n
 	0 0 0\n
  	6 0 0
 
-Version: 0.0.8
+Version: 0.0.81
 
 Author: Jemma Starecki
 
 Made By <a href="https://github.com/JemmaFromJupiter" target="_blank">JemmaFromJupiter</a> On Github.
 """
 from __future__ import annotations
 from . import matrix
 from . import vector
 from . import utils
 
-__version__ = "0.0.8"
+__version__ = "0.0.81"
 __author__ = "JemmaFromJupiter"
 
 __all__ = [
 	"matrix",
 	"vector",
 	"utils"
 ]
```

### Comparing `matrixlib_jfj-0.0.8/src/matrixlib_jfj/matrix.py` & `matrixlib_jfj-0.0.81/src/matrixlib_jfj/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,15 @@
 		self.fill(1)
 
 	def identity(self):
 		if self.get_shape()[1] != self.get_shape()[0]:
 			raise ValueError("Matrix Needs To Be Square.")
 		for i in range(len(self)):
 			for j in range(len(self[0])):
+				self.set_value(i, j, 0)
 				if i == j:
 					self.set_value(i, j, 1)
 
 	def scalar(self, val: Union[int, float]):
 		if self.get_shape()[1] != self.get_shape()[0]:
 			raise ValueError("Matrix Needs To Be Square.")
 		for i in range(len(self)):
```

