# Comparing `tmp/matrixlib_jfj-0.0.81.tar.gz` & `tmp/matrixlib_jfj-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixlib_jfj-0.0.81.tar", last modified: Wed Jun  7 17:28:01 2023, max compression
+gzip compressed data, was "matrixlib_jfj-0.0.82.tar", last modified: Wed Jun  7 19:40:36 2023, max compression
```

## Comparing `matrixlib_jfj-0.0.81.tar` & `matrixlib_jfj-0.0.82.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 17:28:01.077806 matrixlib_jfj-0.0.81/
--rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.81/LICENSE.md
--rw-rw-rw-   0        0        0     3198 2023-06-07 17:28:01.078801 matrixlib_jfj-0.0.81/PKG-INFO
--rw-rw-rw-   0        0        0     2319 2023-06-07 17:27:42.000000 matrixlib_jfj-0.0.81/README.md
--rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.81/pyproject.toml
--rw-rw-rw-   0        0        0     1003 2023-06-07 17:28:01.085795 matrixlib_jfj-0.0.81/setup.cfg
--rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.81/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:28:00.983034 matrixlib_jfj-0.0.81/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 17:28:01.043899 matrixlib_jfj-0.0.81/src/matrixlib_jfj/
--rw-rw-rw-   0        0        0      962 2023-06-07 17:27:55.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj/__init__.py
--rw-rw-rw-   0        0        0    14926 2023-06-07 17:13:01.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj/matrix.py
--rw-rw-rw-   0        0        0      461 2023-06-07 15:32:43.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj/utils.py
--rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj/vector.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:28:01.074813 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/
--rw-rw-rw-   0        0        0     3198 2023-06-07 17:28:00.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-06-07 17:28:00.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 17:28:00.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-07 17:28:00.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 17:28:00.000000 matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 19:40:36.388260 matrixlib_jfj-0.0.82/
+-rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.82/LICENSE.md
+-rw-rw-rw-   0        0        0     3249 2023-06-07 19:40:36.389263 matrixlib_jfj-0.0.82/PKG-INFO
+-rw-rw-rw-   0        0        0     2366 2023-06-07 19:40:29.000000 matrixlib_jfj-0.0.82/README.md
+-rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.82/pyproject.toml
+-rw-rw-rw-   0        0        0     1003 2023-06-07 19:40:36.400158 matrixlib_jfj-0.0.82/setup.cfg
+-rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.82/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:40:36.258697 matrixlib_jfj-0.0.82/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 19:40:36.339233 matrixlib_jfj-0.0.82/src/matrixlib_jfj/
+-rw-rw-rw-   0        0        0      962 2023-06-07 19:40:07.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj/__init__.py
+-rw-rw-rw-   0        0        0    14754 2023-06-07 19:39:13.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj/matrix.py
+-rw-rw-rw-   0        0        0      461 2023-06-07 15:32:43.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj/utils.py
+-rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj/vector.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:40:36.384343 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/
+-rw-rw-rw-   0        0        0     3249 2023-06-07 19:40:35.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-06-07 19:40:36.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 19:40:35.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-07 19:40:35.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 19:40:35.000000 matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/top_level.txt
```

### Comparing `matrixlib_jfj-0.0.81/LICENSE.md` & `matrixlib_jfj-0.0.82/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.81/PKG-INFO` & `matrixlib_jfj-0.0.82/src/matrixlib_jfj.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: matrixlib_jfj
-Version: 0.0.81
+Name: matrixlib-jfj
+Version: 0.0.82
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
@@ -110,14 +110,18 @@
 Fixed bug where an external program would run when the user of the package would run their own program.
 <br>
 
 ## Update 0.0.81
 Updated README file to reflect certain information.
 <br>
 
+## Update 0.0.82
+Fixed Type Annotations.
+<br>
+
 # Contributing
 
 ---
 Any and All feedback and help is highly encouraged. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 <br>
```

### Comparing `matrixlib_jfj-0.0.81/README.md` & `matrixlib_jfj-0.0.82/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -92,14 +92,18 @@
 Fixed bug where an external program would run when the user of the package would run their own program.
 <br>
 
 ## Update 0.0.81
 Updated README file to reflect certain information.
 <br>
 
+## Update 0.0.82
+Fixed Type Annotations.
+<br>
+
 # Contributing
 
 ---
 Any and All feedback and help is highly encouraged. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 <br>
```

### Comparing `matrixlib_jfj-0.0.81/pyproject.toml` & `matrixlib_jfj-0.0.82/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.81/setup.cfg` & `matrixlib_jfj-0.0.82/setup.cfg`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.81/src/matrixlib_jfj/__init__.py` & `matrixlib_jfj-0.0.82/src/matrixlib_jfj/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
  	print(transposed) # Output:
 
  	0 0 0\n
 	0 0 0\n
  	6 0 0
 
-Version: 0.0.81
+Version: 0.0.82
 
 Author: Jemma Starecki
 
 Made By <a href="https://github.com/JemmaFromJupiter" target="_blank">JemmaFromJupiter</a> On Github.
 """
 from __future__ import annotations
 from . import matrix
 from . import vector
 from . import utils
 
-__version__ = "0.0.81"
+__version__ = "0.0.82"
 __author__ = "JemmaFromJupiter"
 
 __all__ = [
 	"matrix",
 	"vector",
 	"utils"
 ]
```

### Comparing `matrixlib_jfj-0.0.81/src/matrixlib_jfj/matrix.py` & `matrixlib_jfj-0.0.82/src/matrixlib_jfj/matrix.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 from typing import Union, Optional
 import math
 import random as r
 import numpy as np
-from . import vector
-from . import utils
+"""from . import vector
+from . import utils"""
 
-class Matrix(list):
+class Matrix(list[list[float]]):
 	"""Initialises a Matrix that can be used for numerous things
 
 Parameters
 ----------
 rowcols (Union[tuple, list]) : The how many rows and columns are in the matrix.
 
 Returns
@@ -79,21 +79,21 @@
 
 > print(matrix) # Output:\n
 0 0 0\n
 0 0 0\n
 0 0 0
 """
 
-	def __new__(cls, rowcols: Union[tuple, list] = None, values: list = None):
+	def __new__(cls, rowcols: tuple | list = None, values: list = None):
 		if rowcols is not None:
 			return super().__new__(cls, rowcols=rowcols)
 		if values is not None:
 			return super().__new__(cls, values=values)
 
-	def __init__(self, rowcols: Union[tuple, list] = None, values: list = None):
+	def __init__(self, rowcols: tuple | list = None, values: list = None):
 		if rowcols is not None:
 			super().__init__([[0] * rowcols[1] for _ in range(rowcols[0])])
 			self.shape = self.get_shape()
 		if values is not None:
 			super().__init__(values)
 			self.shape = self.get_shape()
 
@@ -145,15 +145,15 @@
 
 		raise NotImplementedError("Function Not Implemented")
 
 							
 
 
 	
-	def fill(self, val: Union[int, float]):
+	def fill(self, val: float):
 		"""
 		Fill the Matrix with a specified value.
 
  		Parameters
 	 	----------
 	 	val (Union[int, float]) : The value to fill the Matrix with.
 
@@ -165,15 +165,15 @@
 
  		matrix.fill(1) # Result: [[1, 1, 1], [1, 1, 1], [1, 1, 1]]
  		"""
 		for i in range(len(self)):
 			for j in range(len(self[0])):
 				self.set_value(i, j, val)
 
-	def set_value(self, row: int, col: int, n: Union[int, float]):
+	def set_value(self, row: int, col: int, n: float):
 		"""
     Sets the value at a specified row and column.
 
     Parameters
 		----------
 		row (int) : The row index of the element.
 
@@ -187,15 +187,15 @@
 
  		matrix.set_value(1, 2, 8) # Result: [[0, 8, 0], [0, 0, 0], [0, 0, 0]]
 
 	 	matrix.set_value(3, 1, 5) # Result: [[0, 8, 0], [0, 0, 0], [5, 0, 0]]
     """
 		self[row][col] = n  # Subtracting 1 so if the user inputs 1, the index will be auto set to 0
 
-	def get_value(self, row: int, col: int) -> Union[int, float]:
+	def get_value(self, row: int, col: int) -> float:
 		"""
 		Gets the value at a specified row and column.
 
 		Parameters
 		----------
 		row (int) : The row index of the element.
 
@@ -352,30 +352,30 @@
 				cumsum = 0
 				for j in range(1, self.get_shape()[1] + 1):
 					cumsum += self.get_value(i, j)
 					result.set_value(i, j, cumsum)
 			return result
 		else:
 			raise ValueError("Axis Out Of Bounds")
-		
-	def get_submatrix(self, current_col: int = 0):
+
+	def get_submatrix(self, current_col: int = 0) -> Matrix:
 		if len(self) != len(self[0]):
 			raise ValueError("Matrix Must Be Square")
 		result = Matrix((self.shape[0]-1, self.shape[1]-1))
 		for i in range(1, len(self)):
 			k = 0
 			for j in range(len(self[0])):
 				# print(i, j, self[i][j])
 				if j != current_col:
 					result.set_value(i-1, k, self.get_value(i, j))
 					k += 1
 
 		return result
 
-	def det(self):
+	def det(self) -> int | float:
 		if len(self) != len(self[0]):
 			raise ValueError("Matrix Must Be Square")
 		if self.shape == (1, 1):
 			return self[0][0]
 
 		det = 0
 		sign = 1
@@ -388,18 +388,18 @@
 			det += sign * (self[0][i] * sub_det)
 
 			sign *= -1
 
 		return det
 			
 	
-	def __hash__(self):
+	def __hash__(self) -> int | float:
 		return hash(tuple(map(tuple, self)))
 
-	def __add__(self, other: Union[Matrix, int, float]) -> Matrix:
+	def __add__(self, other: Matrix | float) -> Matrix:
 		if isinstance(other, Matrix):
 			if self.get_shape() != other.get_shape():
 				raise ValueError(
 				 f"Cannot Add Matrix Of Shape {self.get_shape()} To Matrix Of Shape {other.get_shape()}"
 				)
 
 			result = Matrix(self.get_shape())
@@ -412,21 +412,21 @@
 			result = Matrix(self.get_shape())
 			for i in range(len(self)):
 				for j in range(len(self[0])):
 					result.set_value(i, j, self.get_value(i, j) + other)
 
 			return result
 
-	def __radd__(self, other: Union[int, float]) -> Matrix:
+	def __radd__(self, other: Matrix | float) -> Matrix:
 		return self + other
 
-	def __iadd__(self, other: Union[Matrix, int, float]) -> Matrix:
+	def __iadd__(self, other: Matrix | float) -> Matrix:
 		return self + other
 
-	def __sub__(self, other: Union[Matrix, int, float]) -> Matrix:
+	def __sub__(self, other: Matrix | float) -> Matrix:
 		if isinstance(other, Matrix):
 			if self.get_shape() != other.get_shape():
 				raise ValueError(
 				 f"Cannot Subtract Matrix Of Shape {self.get_shape()} From Matrix Of Shape {other.get_shape()}"
 				)
 
 			result = Matrix(self.get_shape())
@@ -440,34 +440,34 @@
 			result = Matrix(self.get_shape())
 			for i in range(len(self)):
 				for j in range(len(self[0])):
 					result.set_value(i, j, self.get_value(i, j) - other)
 
 			return result
 
-	def __isub__(self, other: Union[Matrix, int, float]) -> Matrix:
+	def __isub__(self, other: Matrix | float) -> Matrix:
 		return self - other
 
-	def __rsub__(self, other: Union[Matrix, int, float]) -> Matrix:
+	def __rsub__(self, other: Matrix | float) -> Matrix:
 		return self - other
 
-	def __mul__(self, other: Union[int, float]) -> Matrix:
+	def __mul__(self, other: int, float) -> Matrix:
 		if isinstance(other, Matrix):
 			return self @ other
 		result = Matrix(self.get_shape())
 		for i in range(len(self)):
 			for j in range(len(self[0])):
 				result.set_value(i, j, self.get_value(i, j) * other)
 
 		return result
 
-	def __rmul__(self, other: Union[int, float]) -> Matrix:
+	def __rmul__(self, other: float) -> Matrix:
 		return self * other
 		
-	def __imul__(self, other: Union[int, float]) -> Matrix:
+	def __imul__(self, other: float) -> Matrix:
 		return self * other
 
 	def __matmul__(self, other: Matrix):
 		if isinstance(other, Matrix):
 			if len(self) != len(self[0]):
 				raise ValueError("Not A Square Matrix.")
 			if len(self[0]) != len(other):
@@ -489,16 +489,16 @@
 	def __imatmul__(self, other: Matrix) -> Matrix:
 		return self @ other
 
 	def __rmatmul__(self, other: Matrix) -> Matrix:
 		return self @ other
 
 	def __pow__(self, power: int) -> Matrix:
-		if power < 0:
-			raise ValueError("Power Must Be Greater Than 0")
+		#if power < 0:
+			#raise ValueError("Power Must Be Greater Than 0")
 		if not isinstance(power, int):
 			raise ValueError("Power Must Be An Integer")
 
 		result = Matrix(self.get_shape())
 		if power == 0:
 			result.fill(1)
 		else:
@@ -510,42 +510,42 @@
 
 	def __ipow__(self, power: int) -> Matrix:
 		return self ** power
 
 	def __rpow__(self, power: int) -> Matrix:
 		return self ** power
 	
-	def __truediv__(self, other: Union[int, float]) -> Matrix:
+	def __truediv__(self, other: float) -> Matrix:
 		if isinstance(other, Matrix):
 			raise ValueError("Cannot Divide A Matrix By Another Matrix.")
 		result = Matrix(self.get_shape())
 		for i in range(len(self)):
 			for j in range(len(self[0])):
 				result.set_value(i, j, round(self.get_value(i, j) / other, 2))
 		return result
 
-	def __itruediv__(self, other: Union[int, float]) -> Matrix:
+	def __itruediv__(self, other: float) -> Matrix:
 		return self / other
 
-	def __rtruediv__(self, other: Union[int, float]) -> Matrix:
+	def __rtruediv__(self, other: float) -> Matrix:
 		return self / other
 	
-	def __floordiv__(self, other: Union[int, float]) -> Matrix:
+	def __floordiv__(self, other: float) -> Matrix:
 		if isinstance(other, Matrix):
 			raise ValueError("Cannot Divide A Matrix By Another Matrix.")
 		result = Matrix(self.get_shape())
 		for i in range(len(self)):
 			for j in range(len(self[0])):
 				result.set_value(i, j, self.get_value(i, j) // other)
 		return result
 
-	def __rfloordiv__(self, other: Union[int, float]) -> Matrix:
+	def __rfloordiv__(self, other: float) -> Matrix:
 		return self / other
 
-	def __ifloordiv__(self, other: Union[int, float]) -> Matrix:
+	def __ifloordiv__(self, other: float) -> Matrix:
 		return self / other
 
 	def __neg__(self) -> Matrix:
 		result = Matrix(self.get_shape())
 		for i in range(len(self)):
 			for j in range(len(self[0])):
 				result.set_value(i, j, self.get_value(i, j) * -1)
@@ -555,27 +555,27 @@
 		result = 0
 		for i in range(len(self)):
 			for j in range(len(self[0])):
 				result += self.get_value(i, j)**2
 
 		return math.sqrt(result)
 
-	def __eq__(self, other: Union[Matrix, int, float]) -> bool:
+	def __eq__(self, other: Matrix | float) -> bool:
 		if isinstance(other, Matrix):
 			if self.get_shape() != other.get_shape():
 				return False
 			for i in range(len(self)):
 				for j in range(len(self[0])):
 					if self[i][j] != other[i][j]:
 						return False
 			return True
 		else:
 			return False
 
-	def __neq__(self, other: Union[Matrix, int, float]) -> bool:
+	def __neq__(self, other: Matrix | float) -> bool:
 		if isinstance(other, Matrix):
 			if self.get_shape() != other.get_shape():
 				return True
 			for i in range(len(self)):
 				for j in range(len(self[0])):
 					if self[i][j] == other[i][j]:
 						return False
```

### Comparing `matrixlib_jfj-0.0.81/src/matrixlib_jfj.egg-info/PKG-INFO` & `matrixlib_jfj-0.0.82/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: matrixlib-jfj
-Version: 0.0.81
+Name: matrixlib_jfj
+Version: 0.0.82
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
@@ -110,14 +110,18 @@
 Fixed bug where an external program would run when the user of the package would run their own program.
 <br>
 
 ## Update 0.0.81
 Updated README file to reflect certain information.
 <br>
 
+## Update 0.0.82
+Fixed Type Annotations.
+<br>
+
 # Contributing
 
 ---
 Any and All feedback and help is highly encouraged. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 <br>
```

