# Comparing `tmp/matrixlib_jfj-0.0.6.tar.gz` & `tmp/matrixlib_jfj-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixlib_jfj-0.0.6.tar", last modified: Wed Jun  7 15:36:56 2023, max compression
+gzip compressed data, was "matrixlib_jfj-0.0.7.tar", last modified: Wed Jun  7 16:46:24 2023, max compression
```

## Comparing `matrixlib_jfj-0.0.6.tar` & `matrixlib_jfj-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 15:36:56.952968 matrixlib_jfj-0.0.6/
--rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.6/LICENSE.md
--rw-rw-rw-   0        0        0     1116 2023-06-07 15:36:56.952968 matrixlib_jfj-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.6/README.md
--rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     1003 2023-06-07 15:36:56.961941 matrixlib_jfj-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:36:56.838302 matrixlib_jfj-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 15:36:56.917518 matrixlib_jfj-0.0.6/src/matrixlib_jfj/
--rw-rw-rw-   0        0        0      960 2023-06-07 15:36:41.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj/__init__.py
--rw-rw-rw-   0        0        0    13782 2023-06-07 15:36:32.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj/matrix.py
--rw-rw-rw-   0        0        0      461 2023-06-07 15:32:43.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj/utils.py
--rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj/vector.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:36:56.949972 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/
--rw-rw-rw-   0        0        0     1116 2023-06-07 15:36:56.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-06-07 15:36:56.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 15:36:56.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-07 15:36:56.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 15:36:56.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 16:46:24.928056 matrixlib_jfj-0.0.7/
+-rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.7/LICENSE.md
+-rw-rw-rw-   0        0        0     1116 2023-06-07 16:46:24.929057 matrixlib_jfj-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1003 2023-06-07 16:46:24.937031 matrixlib_jfj-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:46:24.820295 matrixlib_jfj-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 16:46:24.891804 matrixlib_jfj-0.0.7/src/matrixlib_jfj/
+-rw-rw-rw-   0        0        0      960 2023-06-07 16:46:09.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj/__init__.py
+-rw-rw-rw-   0        0        0    15021 2023-06-07 16:37:30.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj/matrix.py
+-rw-rw-rw-   0        0        0      461 2023-06-07 15:32:43.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj/utils.py
+-rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj/vector.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:46:24.924071 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/
+-rw-rw-rw-   0        0        0     1116 2023-06-07 16:46:24.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-06-07 16:46:24.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 16:46:24.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-07 16:46:24.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 16:46:24.000000 matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/top_level.txt
```

### Comparing `matrixlib_jfj-0.0.6/LICENSE.md` & `matrixlib_jfj-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.6/PKG-INFO` & `matrixlib_jfj-0.0.7/src/matrixlib_jfj.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: matrixlib_jfj
-Version: 0.0.6
+Name: matrixlib-jfj
+Version: 0.0.7
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `matrixlib_jfj-0.0.6/pyproject.toml` & `matrixlib_jfj-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.6/setup.cfg` & `matrixlib_jfj-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.6/src/matrixlib_jfj/__init__.py` & `matrixlib_jfj-0.0.7/src/matrixlib_jfj/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
  	print(transposed) # Output:
 
  	0 0 0\n
 	0 0 0\n
  	6 0 0
 
-Version: 0.0.6
+Version: 0.0.7
 
 Author: Jemma Starecki
 
 Made By <a href="https://github.com/JemmaFromJupiter" target="_blank">JemmaFromJupiter</a> On Github.
 """
 from __future__ import annotations
 from . import matrix
 from . import vector
 from . import utils
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 __author__ = "JemmaFromJupiter"
 
 __all__ = [
 	"matrix",
 	"vector",
 	"utils"
 ]
```

### Comparing `matrixlib_jfj-0.0.6/src/matrixlib_jfj/matrix.py` & `matrixlib_jfj-0.0.7/src/matrixlib_jfj/matrix.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import Union, Optional
 import math
 import random as r
 import numpy as np
-from . import vector
-from . import utils
+# from . import vector
+# from . import utils
 
 class Matrix(list):
 	"""Initialises a Matrix that can be used for numerous things
 
 Parameters
 ----------
 rowcols (Union[tuple, list]) : The how many rows and columns are in the matrix.
@@ -99,25 +99,58 @@
 
 	def __str__(self):
 		rows = self.get_shape()[0]
 		max = len(str(self.max()))
 		result = []
 		for row in range(rows):
 			result.append("|" + "   ".join(map(lambda el: f"{el:^{max}}", self[row])) + "|\n")
-		center_space = " "*(len(result[1])-5)
+		if len(self) == 1:
+			center_space = " "*(len(result[0])-5)
+		else:
+			center_space = " "*(len(result[1])-5)
 		result.append("+-" + center_space + "-+")
 		result.insert(0, "+-" + center_space + "-+\n")
 		return "".join(result)
 
 	def __repr__(self):
 		return self
 	
 	def rank(self):
+		"""rank = self.shape[1]
+		for row in range(0, rank, 1):
+
+			if self[row][row] != 0:
+				for col in range(0, self.shape[0], 1):
+					if col != row:
+						multiplier = (self[col][row] / self[row][row])
+
+						for i in range(rank):
+							self[col][i] -= (multiplier * self[row][i])
+			else:
+				reduce = True
+
+				for i in range(row + 1, self.shape[0], 1):
+					if self[i][row] != 0:
+						for j in range(self.shape[1]):
+							temp = self[row][j]
+							self[row][j] = self[row+1][i]
+							self[row+1][i] = temp
+						reduce = False
+				if reduce:
+					rank -= 1
+
+					for i in range(0, self.shape[0], 1):
+						self[i][row] = self[i][rank]
+				row -= 1
+		return (rank)"""
+
 		raise NotImplementedError("Function Not Implemented")
 
+							
+
 
 	
 	def fill(self, val: Union[int, float]):
 		"""
 		Fill the Matrix with a specified value.
 
  		Parameters
@@ -152,17 +185,15 @@
 		----------
 		matrix = Matrix((3, 3))
 
  		matrix.set_value(1, 2, 8) # Result: [[0, 8, 0], [0, 0, 0], [0, 0, 0]]
 
 	 	matrix.set_value(3, 1, 5) # Result: [[0, 8, 0], [0, 0, 0], [5, 0, 0]]
     """
-		self[row - 1][
-		 col -
-		 1] = n  # Subtracting 1 so if the user inputs 1, the index will be auto set to 0
+		self[row][col] = n  # Subtracting 1 so if the user inputs 1, the index will be auto set to 0
 
 	def get_value(self, row: int, col: int) -> Union[int, float]:
 		"""
 		Gets the value at a specified row and column.
 
 		Parameters
 		----------
@@ -178,15 +209,15 @@
 		----------
 		matrix -> [[0, 0, 0], [1, 7, 0], [0, 1, 5]]
 
 		print(matrix.get_value(2, 2)) # Output: 7
 
  		print(matrix.get_value(3, 2)) # Output: 1
 		"""
-		return self[row - 1][col - 1]
+		return self[row][col]
 
 	def random(self, a: int = None, b: int = None):
 		if a is None:
 			a = 0
 		if b is None:
 			b = 1
 		for i in range(len(self)):
@@ -320,24 +351,48 @@
 				cumsum = 0
 				for j in range(1, self.get_shape()[1] + 1):
 					cumsum += self.get_value(i, j)
 					result.set_value(i, j, cumsum)
 			return result
 		else:
 			raise ValueError("Axis Out Of Bounds")
+		
+	def get_submatrix(self, current_col: int = 0):
+		if len(self) != len(self[0]):
+			raise ValueError("Matrix Must Be Square")
+		result = Matrix((self.shape[0]-1, self.shape[1]-1))
+		for i in range(1, len(self)):
+			k = 0
+			for j in range(len(self[0])):
+				# print(i, j, self[i][j])
+				if j != current_col:
+					result.set_value(i-1, k, self.get_value(i, j))
+					k += 1
+
+		return result
 
-	def determinant(self):
+	def det(self):
 		if len(self) != len(self[0]):
 			raise ValueError("Matrix Must Be Square")
 		if self.shape == (1, 1):
 			return self[0][0]
-		if self.shape == (2, 2):
-			return (self.get_value(0, 0) * self.get_value(1, 1)) - (self.get_value(0, 1) * self.get_value(1, 0))
 
-		raise NotImplementedError("Function Not Implemented Yet.")
+		det = 0
+		sign = 1
+
+		for i in range(len(self[0])):
+			submatrix = self.get_submatrix(i)
+
+			sub_det = submatrix.det()
+
+			det += sign * (self[0][i] * sub_det)
+
+			sign *= -1
+
+		return det
 			
 	
 	def __hash__(self):
 		return hash(tuple(map(tuple, self)))
 
 	def __add__(self, other: Union[Matrix, int, float]) -> Matrix:
 		if isinstance(other, Matrix):
@@ -524,8 +579,16 @@
 					if self[i][j] == other[i][j]:
 						return False
 			return True
 		else:
 			return False
 		
 	def max(self):
-		return max(max(self, key=max))
+		return max(max(self, key=max))
+	
+matrix = Matrix(rowcols=(10, 10))
+
+matrix.random(1, 100)
+
+print(matrix, end="\n\n")
+
+print(matrix.det(), end="\n\n")
```

### Comparing `matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/PKG-INFO` & `matrixlib_jfj-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: matrixlib-jfj
-Version: 0.0.6
+Name: matrixlib_jfj
+Version: 0.0.7
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

