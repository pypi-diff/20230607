# Comparing `tmp/matrixlib_jfj-0.0.4.tar.gz` & `tmp/matrixlib_jfj-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixlib_jfj-0.0.4.tar", last modified: Wed Jun  7 02:05:45 2023, max compression
+gzip compressed data, was "matrixlib_jfj-0.0.5.tar", last modified: Wed Jun  7 03:18:05 2023, max compression
```

## Comparing `matrixlib_jfj-0.0.4.tar` & `matrixlib_jfj-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 02:05:45.552305 matrixlib_jfj-0.0.4/
--rw-r--r--   0 runner    (1000) runner    (1000)    35148 2023-06-06 20:50:00.000000 matrixlib_jfj-0.0.4/LICENSE.md
--rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 02:05:45.552305 matrixlib_jfj-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-06-06 20:36:36.000000 matrixlib_jfj-0.0.4/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)     1014 2023-06-07 01:46:06.000000 matrixlib_jfj-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      965 2023-06-07 02:05:45.552305 matrixlib_jfj-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)       65 2023-06-07 01:15:59.000000 matrixlib_jfj-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 02:05:45.548305 matrixlib_jfj-0.0.4/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 02:05:45.548305 matrixlib_jfj-0.0.4/src/matrixlib_jfj/
--rw-r--r--   0 runner    (1000) runner    (1000)      960 2023-06-07 02:05:39.000000 matrixlib_jfj-0.0.4/src/matrixlib_jfj/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13662 2023-06-07 02:02:54.000000 matrixlib_jfj-0.0.4/src/matrixlib_jfj/matrix.py
--rw-r--r--   0 runner    (1000) runner    (1000)      270 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.4/src/matrixlib_jfj/utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)      213 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.4/src/matrixlib_jfj/vector.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 02:05:45.552305 matrixlib_jfj-0.0.4/src/matrixlib_jfj.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 02:05:45.000000 matrixlib_jfj-0.0.4/src/matrixlib_jfj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      371 2023-06-07 02:05:45.000000 matrixlib_jfj-0.0.4/src/matrixlib_jfj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-07 02:05:45.000000 matrixlib_jfj-0.0.4/src/matrixlib_jfj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2023-06-07 02:05:45.000000 matrixlib_jfj-0.0.4/src/matrixlib_jfj.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-06-07 02:05:45.000000 matrixlib_jfj-0.0.4/src/matrixlib_jfj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 03:18:05.715081 matrixlib_jfj-0.0.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)    35148 2023-06-06 20:50:00.000000 matrixlib_jfj-0.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 03:18:05.719081 matrixlib_jfj-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-06-06 20:36:36.000000 matrixlib_jfj-0.0.5/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)     1014 2023-06-07 01:46:06.000000 matrixlib_jfj-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      965 2023-06-07 03:18:05.719081 matrixlib_jfj-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)       65 2023-06-07 01:15:59.000000 matrixlib_jfj-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 03:18:05.711081 matrixlib_jfj-0.0.5/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 03:18:05.715081 matrixlib_jfj-0.0.5/src/matrixlib_jfj/
+-rw-r--r--   0 runner    (1000) runner    (1000)      960 2023-06-07 03:17:46.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13699 2023-06-07 03:15:46.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj/matrix.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      270 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj/utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      213 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj/vector.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 03:18:05.715081 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 03:18:05.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      371 2023-06-07 03:18:05.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-07 03:18:05.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2023-06-07 03:18:05.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-06-07 03:18:05.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/top_level.txt
```

### Comparing `matrixlib_jfj-0.0.4/LICENSE.md` & `matrixlib_jfj-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.4/PKG-INFO` & `matrixlib_jfj-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib_jfj
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `matrixlib_jfj-0.0.4/pyproject.toml` & `matrixlib_jfj-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.4/setup.cfg` & `matrixlib_jfj-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.4/src/matrixlib_jfj/__init__.py` & `matrixlib_jfj-0.0.5/src/matrixlib_jfj/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
  	print(transposed) # Output:
 
  	0 0 0\n
 	0 0 0\n
  	6 0 0
 
-Version: 0.0.4
+Version: 0.0.5
 
 Author: Jemma Starecki
 
 Made By <a href="https://github.com/JemmaFromJupiter" target="_blank">JemmaFromJupiter</a> On Github.
 """
 from __future__ import annotations
 from . import matrix
 from . import vector
 from . import utils
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __author__ = "JemmaFromJupiter"
 
 __all__ = [
 	"matrix",
 	"vector",
 	"utils"
 ]
```

### Comparing `matrixlib_jfj-0.0.4/src/matrixlib_jfj/matrix.py` & `matrixlib_jfj-0.0.5/src/matrixlib_jfj/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,17 @@
 		for row in range(rows):
 			result.append("|" + "   ".join(map(lambda el: f"{el:^{max}}", self[row])) + "|\n")
 		center_space = " "*(len(result[1])-5)
 		result.append("+-" + center_space + "-+")
 		result.insert(0, "+-" + center_space + "-+\n")
 		return "".join(result)
 
+	def __repr__(self):
+		return self
+	
 	def fill(self, val: Union[int, float]):
 		"""
 		Fill the Matrix with a specified value.
 
  		Parameters
 	 	----------
 	 	val (Union[int, float]) : The value to fill the Matrix with.
```

### Comparing `matrixlib_jfj-0.0.4/src/matrixlib_jfj.egg-info/PKG-INFO` & `matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib-jfj
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

