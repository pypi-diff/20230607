# Comparing `tmp/matrixlib_jfj-0.0.2.tar.gz` & `tmp/matrixlib_jfj-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixlib_jfj-0.0.2.tar", last modified: Wed Jun  7 01:50:23 2023, max compression
+gzip compressed data, was "matrixlib_jfj-0.0.3.tar", last modified: Wed Jun  7 02:00:06 2023, max compression
```

## Comparing `matrixlib_jfj-0.0.2.tar` & `matrixlib_jfj-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:50:23.477674 matrixlib_jfj-0.0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)    35148 2023-06-06 20:50:00.000000 matrixlib_jfj-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 01:50:23.477674 matrixlib_jfj-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-06-06 20:36:36.000000 matrixlib_jfj-0.0.2/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)     1014 2023-06-07 01:46:06.000000 matrixlib_jfj-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      965 2023-06-07 01:50:23.481674 matrixlib_jfj-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)       65 2023-06-07 01:15:59.000000 matrixlib_jfj-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:50:23.473674 matrixlib_jfj-0.0.2/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:50:23.477674 matrixlib_jfj-0.0.2/src/matrixlib_jfj/
--rw-r--r--   0 runner    (1000) runner    (1000)      960 2023-06-07 01:50:21.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13499 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj/matrix.py
--rw-r--r--   0 runner    (1000) runner    (1000)      270 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj/utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)      213 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj/vector.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 01:50:23.477674 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 01:50:23.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      371 2023-06-07 01:50:23.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-07 01:50:23.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2023-06-07 01:50:23.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-06-07 01:50:23.000000 matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 02:00:06.044809 matrixlib_jfj-0.0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)    35148 2023-06-06 20:50:00.000000 matrixlib_jfj-0.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 02:00:06.044809 matrixlib_jfj-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-06-06 20:36:36.000000 matrixlib_jfj-0.0.3/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)     1014 2023-06-07 01:46:06.000000 matrixlib_jfj-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      965 2023-06-07 02:00:06.044809 matrixlib_jfj-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)       65 2023-06-07 01:15:59.000000 matrixlib_jfj-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 02:00:06.008809 matrixlib_jfj-0.0.3/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 02:00:06.044809 matrixlib_jfj-0.0.3/src/matrixlib_jfj/
+-rw-r--r--   0 runner    (1000) runner    (1000)      960 2023-06-07 02:00:02.000000 matrixlib_jfj-0.0.3/src/matrixlib_jfj/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13688 2023-06-07 01:58:36.000000 matrixlib_jfj-0.0.3/src/matrixlib_jfj/matrix.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      270 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.3/src/matrixlib_jfj/utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      213 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.3/src/matrixlib_jfj/vector.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 02:00:06.044809 matrixlib_jfj-0.0.3/src/matrixlib_jfj.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 02:00:05.000000 matrixlib_jfj-0.0.3/src/matrixlib_jfj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      371 2023-06-07 02:00:05.000000 matrixlib_jfj-0.0.3/src/matrixlib_jfj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-07 02:00:05.000000 matrixlib_jfj-0.0.3/src/matrixlib_jfj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2023-06-07 02:00:05.000000 matrixlib_jfj-0.0.3/src/matrixlib_jfj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-06-07 02:00:05.000000 matrixlib_jfj-0.0.3/src/matrixlib_jfj.egg-info/top_level.txt
```

### Comparing `matrixlib_jfj-0.0.2/LICENSE.md` & `matrixlib_jfj-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.2/PKG-INFO` & `matrixlib_jfj-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib_jfj
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `matrixlib_jfj-0.0.2/pyproject.toml` & `matrixlib_jfj-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.2/setup.cfg` & `matrixlib_jfj-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.2/src/matrixlib_jfj/__init__.py` & `matrixlib_jfj-0.0.3/src/matrixlib_jfj/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
  	print(transposed) # Output:
 
  	0 0 0\n
 	0 0 0\n
  	6 0 0
 
-Version: 0.0.2
+Version: 0.0.3
 
 Author: Jemma Starecki
 
 Made By <a href="https://github.com/JemmaFromJupiter" target="_blank">JemmaFromJupiter</a> On Github.
 """
 from __future__ import annotations
 from . import matrix
 from . import vector
 from . import utils
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __author__ = "JemmaFromJupiter"
 
 __all__ = [
 	"matrix",
 	"vector",
 	"utils"
 ]
```

### Comparing `matrixlib_jfj-0.0.2/src/matrixlib_jfj/matrix.py` & `matrixlib_jfj-0.0.3/src/matrixlib_jfj/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,20 +313,23 @@
 					cumsum += self.get_value(i, j)
 					result.set_value(i, j, cumsum)
 			return result
 		else:
 			raise ValueError("Axis Out Of Bounds")
 
 	def determinant(self, submatrix: Matrix = None):
-		if submatrix is None:
-			submatrix = self
-		if self.get_shape() == (1, 1):
-			return self.get_value(1, 1)
-		else:
-			raise NotImplemented("")
+		if len(self) != len(self[0]):
+			raise ValueError("Matrix Must Be Square")
+		if self.shape == (1, 1):
+			return self[0][0]
+		if self.shape == (2, 2):
+			return (self.get_value(0, 0) * self.get_value(1, 1)) - (self.get_value(0, 1) * self.get_value(1, 0))
+
+		raise NotImplementedError("This Function Hasnt Been Implemented yet")
+			
 	
 	def __hash__(self):
 		return hash(tuple(map(tuple, self)))
 
 	def __add__(self, other: Union[Matrix, int, float]) -> Matrix:
 		if isinstance(other, Matrix):
 			if self.get_shape() != other.get_shape():
```

### Comparing `matrixlib_jfj-0.0.2/src/matrixlib_jfj.egg-info/PKG-INFO` & `matrixlib_jfj-0.0.3/src/matrixlib_jfj.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib-jfj
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

