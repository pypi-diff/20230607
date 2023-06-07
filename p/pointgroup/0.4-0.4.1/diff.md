# Comparing `tmp/pointgroup-0.4.tar.gz` & `tmp/pointgroup-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointgroup-0.4.tar", last modified: Mon Mar 20 21:52:14 2023, max compression
+gzip compressed data, was "pointgroup-0.4.1.tar", last modified: Wed Jun  7 11:56:44 2023, max compression
```

## Comparing `pointgroup-0.4.tar` & `pointgroup-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:52:14.896621 pointgroup-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-20 21:52:03.000000 pointgroup-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-20 21:52:14.896621 pointgroup-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-20 21:52:03.000000 pointgroup-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:52:14.892620 pointgroup-0.4/pointgroup/
--rw-r--r--   0 runner    (1001) docker     (123)    14468 2023-03-20 21:52:03.000000 pointgroup-0.4/pointgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-03-20 21:52:03.000000 pointgroup-0.4/pointgroup/element_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-20 21:52:03.000000 pointgroup-0.4/pointgroup/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-20 21:52:03.000000 pointgroup-0.4/pointgroup/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-03-20 21:52:03.000000 pointgroup-0.4/pointgroup/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:52:14.896621 pointgroup-0.4/pointgroup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-20 21:52:14.000000 pointgroup-0.4/pointgroup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-20 21:52:14.000000 pointgroup-0.4/pointgroup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 21:52:14.000000 pointgroup-0.4/pointgroup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-20 21:52:14.000000 pointgroup-0.4/pointgroup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-20 21:52:14.000000 pointgroup-0.4/pointgroup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 21:52:14.896621 pointgroup-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-20 21:52:03.000000 pointgroup-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:56:44.185116 pointgroup-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-07 11:56:34.000000 pointgroup-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-07 11:56:44.185116 pointgroup-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-07 11:56:34.000000 pointgroup-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:56:44.185116 pointgroup-0.4.1/pointgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-06-07 11:56:34.000000 pointgroup-0.4.1/pointgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-07 11:56:34.000000 pointgroup-0.4.1/pointgroup/element_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-07 11:56:34.000000 pointgroup-0.4.1/pointgroup/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-07 11:56:34.000000 pointgroup-0.4.1/pointgroup/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-07 11:56:34.000000 pointgroup-0.4.1/pointgroup/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:56:44.185116 pointgroup-0.4.1/pointgroup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-07 11:56:44.000000 pointgroup-0.4.1/pointgroup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-07 11:56:44.000000 pointgroup-0.4.1/pointgroup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:56:44.000000 pointgroup-0.4.1/pointgroup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 11:56:44.000000 pointgroup-0.4.1/pointgroup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 11:56:44.000000 pointgroup-0.4.1/pointgroup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 11:56:44.185116 pointgroup-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-07 11:56:34.000000 pointgroup-0.4.1/setup.py
```

### Comparing `pointgroup-0.4/LICENSE` & `pointgroup-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pointgroup-0.4/PKG-INFO` & `pointgroup-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointgroup
-Version: 0.4
+Version: 0.4.1
 Summary: pointgroup module
 Home-page: https://github.com/abelcarreras/pointgroup
 Author: Abel Carreras
 Author-email: abelcarreras83@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pointgroup-0.4/README.md` & `pointgroup-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pointgroup-0.4/pointgroup/__init__.py` & `pointgroup-0.4.1/pointgroup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.4'
+__version__ = '0.4.1'
 import numpy as np
 from pointgroup.operations import Inversion, Rotation, ImproperRotation, Reflection, rotation_matrix
 from pointgroup import tools
 
 
 def abs_to_rad(error, coord):
     coord = np.array(coord)
@@ -320,15 +320,19 @@
             return
 
         p_axis = tools.get_perpendicular(main_axis)
         self._set_orientation(main_axis, p_axis)
 
     def _dihedral(self, main_axis):
 
-        self._schoenflies_symbol = "D{}".format(self._max_order)
+        if self._max_order == 1:
+            # D1 is equivalent to C2
+            self._schoenflies_symbol = "C2"
+        else:
+            self._schoenflies_symbol = "D{}".format(self._max_order)
 
         if self._check_op(Reflection(main_axis), tol_factor=0.0):
             self._schoenflies_symbol += 'h'
             return
 
         p_axis = tools.get_perpendicular(main_axis)
         for angle in np.arange(0, np.pi/self._max_order+self._tolerance_ang, self._tolerance_ang):
```

### Comparing `pointgroup-0.4/pointgroup/element_data.py` & `pointgroup-0.4.1/pointgroup/element_data.py`

 * *Files identical despite different names*

### Comparing `pointgroup-0.4/pointgroup/grid.py` & `pointgroup-0.4.1/pointgroup/grid.py`

 * *Files identical despite different names*

### Comparing `pointgroup-0.4/pointgroup/operations.py` & `pointgroup-0.4.1/pointgroup/operations.py`

 * *Files identical despite different names*

### Comparing `pointgroup-0.4/pointgroup/tools.py` & `pointgroup-0.4.1/pointgroup/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def get_mass(symbols):
     mass_vector = []
     for symbol in symbols:
         try:
             mass_vector.append(element_mass(symbol))
         except KeyError as e:
-            warnings.warn('Atomic mass of element {} not found, using 1 u'.format(e))
+            warnings.warn('Atomic element {} not recognized, using mass 1'.format(symbol))
             mass_vector.append(1.0)
     return mass_vector
 
 
 def get_center_mass(symbols, coordinates):
     mass_vector = get_mass(symbols)
     cbye = [np.dot(mass_vector[i], coordinates[i]) for i in range(len(symbols))]
```

### Comparing `pointgroup-0.4/pointgroup.egg-info/PKG-INFO` & `pointgroup-0.4.1/pointgroup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointgroup
-Version: 0.4
+Version: 0.4.1
 Summary: pointgroup module
 Home-page: https://github.com/abelcarreras/pointgroup
 Author: Abel Carreras
 Author-email: abelcarreras83@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pointgroup-0.4/setup.py` & `pointgroup-0.4.1/setup.py`

 * *Files identical despite different names*

