# Comparing `tmp/PyIntegral-0.0.10.tar.gz` & `tmp/PyIntegral-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyIntegral-0.0.10.tar", last modified: Wed Jun  7 13:12:21 2023, max compression
+gzip compressed data, was "PyIntegral-0.0.11.tar", last modified: Wed Jun  7 13:29:12 2023, max compression
```

## Comparing `PyIntegral-0.0.10.tar` & `PyIntegral-0.0.11.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 13:12:21.877350 PyIntegral-0.0.10/
--rw-r--r--   0 jean      (1000) users      (100)      894 2023-06-07 12:58:56.000000 PyIntegral-0.0.10/LICENSE.txt
--rw-r--r--   0 jean      (1000) users      (100)     8588 2023-06-07 13:12:21.877350 PyIntegral-0.0.10/PKG-INFO
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 13:12:21.873350 PyIntegral-0.0.10/PyIntegral.egg-info/
--rw-r--r--   0 jean      (1000) users      (100)     8588 2023-06-07 13:12:21.000000 PyIntegral-0.0.10/PyIntegral.egg-info/PKG-INFO
--rw-r--r--   0 jean      (1000) users      (100)      384 2023-06-07 13:12:21.000000 PyIntegral-0.0.10/PyIntegral.egg-info/SOURCES.txt
--rw-r--r--   0 jean      (1000) users      (100)        1 2023-06-07 13:12:21.000000 PyIntegral-0.0.10/PyIntegral.egg-info/dependency_links.txt
--rw-r--r--   0 jean      (1000) users      (100)       17 2023-06-07 13:12:21.000000 PyIntegral-0.0.10/PyIntegral.egg-info/requires.txt
--rw-r--r--   0 jean      (1000) users      (100)       11 2023-06-07 13:12:21.000000 PyIntegral-0.0.10/PyIntegral.egg-info/top_level.txt
--rwxr-xr-x   0 jean      (1000) users      (100)     8002 2023-06-07 13:12:03.000000 PyIntegral-0.0.10/README.md
--rw-r--r--   0 jean      (1000) users      (100)       38 2023-06-07 13:12:21.877350 PyIntegral-0.0.10/setup.cfg
--rw-r--r--   0 jean      (1000) users      (100)     1425 2023-06-07 13:10:28.000000 PyIntegral-0.0.10/setup.py
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 13:12:21.873350 PyIntegral-0.0.10/src/
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 13:12:21.877350 PyIntegral-0.0.10/src/fortran/
--rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-06-07 12:58:56.000000 PyIntegral-0.0.10/src/fortran/DataTypes.f90
--rw-r--r--   0 jean      (1000) users      (100)     7359 2023-06-07 12:58:56.000000 PyIntegral-0.0.10/src/fortran/GaussLegendreQuadrature.f90
--rw-r--r--   0 jean      (1000) users      (100)    43798 2023-06-07 12:58:56.000000 PyIntegral-0.0.10/src/fortran/IntegralALL.f90
--rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-06-07 12:58:56.000000 PyIntegral-0.0.10/src/fortran/LINinterpol.f90
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 13:12:21.877350 PyIntegral-0.0.10/src/python/
--rw-r--r--   0 jean      (1000) users      (100)     1784 2023-06-07 12:58:56.000000 PyIntegral-0.0.10/src/python/PyIntegralALL.py
--rwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 12:58:56.000000 PyIntegral-0.0.10/src/python/__init__.py
--rw-r--r--   0 jean      (1000) users      (100)        7 2023-06-07 12:59:53.000000 PyIntegral-0.0.10/version.txt
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 13:29:12.905326 PyIntegral-0.0.11/
+-rw-r--r--   0 jean      (1000) users      (100)      894 2023-06-07 12:58:56.000000 PyIntegral-0.0.11/LICENSE.txt
+-rw-r--r--   0 jean      (1000) users      (100)     8588 2023-06-07 13:29:12.905326 PyIntegral-0.0.11/PKG-INFO
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 13:29:12.905326 PyIntegral-0.0.11/PyIntegral.egg-info/
+-rw-r--r--   0 jean      (1000) users      (100)     8588 2023-06-07 13:29:12.000000 PyIntegral-0.0.11/PyIntegral.egg-info/PKG-INFO
+-rw-r--r--   0 jean      (1000) users      (100)      381 2023-06-07 13:29:12.000000 PyIntegral-0.0.11/PyIntegral.egg-info/SOURCES.txt
+-rw-r--r--   0 jean      (1000) users      (100)        1 2023-06-07 13:29:12.000000 PyIntegral-0.0.11/PyIntegral.egg-info/dependency_links.txt
+-rw-r--r--   0 jean      (1000) users      (100)       17 2023-06-07 13:29:12.000000 PyIntegral-0.0.11/PyIntegral.egg-info/requires.txt
+-rw-r--r--   0 jean      (1000) users      (100)       11 2023-06-07 13:29:12.000000 PyIntegral-0.0.11/PyIntegral.egg-info/top_level.txt
+-rwxr-xr-x   0 jean      (1000) users      (100)     8002 2023-06-07 13:28:42.000000 PyIntegral-0.0.11/README.md
+-rw-r--r--   0 jean      (1000) users      (100)       38 2023-06-07 13:29:12.905326 PyIntegral-0.0.11/setup.cfg
+-rw-r--r--   0 jean      (1000) users      (100)     1425 2023-06-07 13:10:28.000000 PyIntegral-0.0.11/setup.py
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 13:29:12.901327 PyIntegral-0.0.11/src/
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 13:29:12.905326 PyIntegral-0.0.11/src/fortran/
+-rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-06-07 12:58:56.000000 PyIntegral-0.0.11/src/fortran/DataTypes.f90
+-rw-r--r--   0 jean      (1000) users      (100)     7359 2023-06-07 12:58:56.000000 PyIntegral-0.0.11/src/fortran/GaussLegendreQuadrature.f90
+-rw-r--r--   0 jean      (1000) users      (100)    43798 2023-06-07 12:58:56.000000 PyIntegral-0.0.11/src/fortran/IntegralALL.f90
+-rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-06-07 12:58:56.000000 PyIntegral-0.0.11/src/fortran/LINinterpol.f90
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 13:29:12.905326 PyIntegral-0.0.11/src/python/
+-rw-r--r--   0 jean      (1000) users      (100)     1772 2023-06-07 13:28:09.000000 PyIntegral-0.0.11/src/python/PyIntegral.py
+-rwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-07 12:58:56.000000 PyIntegral-0.0.11/src/python/__init__.py
+-rw-r--r--   0 jean      (1000) users      (100)        7 2023-06-07 13:28:28.000000 PyIntegral-0.0.11/version.txt
```

### Comparing `PyIntegral-0.0.10/LICENSE.txt` & `PyIntegral-0.0.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyIntegral-0.0.10/PKG-INFO` & `PyIntegral-0.0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIntegral
-Version: 0.0.10
+Version: 0.0.11
 Summary: Integrate arrays, functions numerically using different methods in Python. Original Fortran 2003+ legacy routines date back to 2003-2004. Read the LICENSE.txt file.
 Home-page: https://github.com/neutrinomuon/PyIntegral
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 ####  A Fortran legacy package to easy integrate numerically
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 © Copyright ®
 
 J.G. - Jean Gomes
 
-last stable version: 0.0.10
+last stable version: 0.0.11
 
 <hr>
 
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)<br>
 [![python3](https://img.shields.io/pypi/pyversions/PyIntegral)](https://img.shields.io/pypi/pyversions/PyIntegral)
 [![badgetlicense](https://anaconda.org/neutrinomuon/PyIntegral/badges/license.svg)](https://anaconda.org/neutrinomuon/PyIntegral/badges/license.svg)
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: PyIntegral Version: 0.0.10 Summary: Integrate
+Metadata-Version: 2.1 Name: PyIntegral Version: 0.0.11 Summary: Integrate
 arrays, functions numerically using different methods in Python. Original
 Fortran 2003+ legacy routines date back to 2003-2004. Read the LICENSE.txt
 file. Home-page: https://github.com/neutrinomuon/PyIntegral Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Fortran Classifier: Operating System :: OS Independent Description-
 Content-Type: text/markdown License-File: LICENSE.txt ### PyIntegral #### A
 Fortran legacy package to easy integrate numerically email:
 [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
 [jean@astro.up.pt](mailto:jean@astro.up.pt) Â© Copyright Â® J.G. - Jean Gomes
-last stable version: 0.0.10
+last stable version: 0.0.11
 ===============================================================================
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)
 [![python3](https://img.shields.io/pypi/pyversions/PyIntegral)](https://
 img.shields.io/pypi/pyversions/PyIntegral) [![badgetlicense](https://
 anaconda.org/neutrinomuon/PyIntegral/badges/license.svg)](https://anaconda.org/
 neutrinomuon/PyIntegral/badges/license.svg)
 ===============================================================================
```

### Comparing `PyIntegral-0.0.10/PyIntegral.egg-info/PKG-INFO` & `PyIntegral-0.0.11/PyIntegral.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIntegral
-Version: 0.0.10
+Version: 0.0.11
 Summary: Integrate arrays, functions numerically using different methods in Python. Original Fortran 2003+ legacy routines date back to 2003-2004. Read the LICENSE.txt file.
 Home-page: https://github.com/neutrinomuon/PyIntegral
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 ####  A Fortran legacy package to easy integrate numerically
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 © Copyright ®
 
 J.G. - Jean Gomes
 
-last stable version: 0.0.10
+last stable version: 0.0.11
 
 <hr>
 
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)<br>
 [![python3](https://img.shields.io/pypi/pyversions/PyIntegral)](https://img.shields.io/pypi/pyversions/PyIntegral)
 [![badgetlicense](https://anaconda.org/neutrinomuon/PyIntegral/badges/license.svg)](https://anaconda.org/neutrinomuon/PyIntegral/badges/license.svg)
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: PyIntegral Version: 0.0.10 Summary: Integrate
+Metadata-Version: 2.1 Name: PyIntegral Version: 0.0.11 Summary: Integrate
 arrays, functions numerically using different methods in Python. Original
 Fortran 2003+ legacy routines date back to 2003-2004. Read the LICENSE.txt
 file. Home-page: https://github.com/neutrinomuon/PyIntegral Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Fortran Classifier: Operating System :: OS Independent Description-
 Content-Type: text/markdown License-File: LICENSE.txt ### PyIntegral #### A
 Fortran legacy package to easy integrate numerically email:
 [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
 [jean@astro.up.pt](mailto:jean@astro.up.pt) Â© Copyright Â® J.G. - Jean Gomes
-last stable version: 0.0.10
+last stable version: 0.0.11
 ===============================================================================
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)
 [![python3](https://img.shields.io/pypi/pyversions/PyIntegral)](https://
 img.shields.io/pypi/pyversions/PyIntegral) [![badgetlicense](https://
 anaconda.org/neutrinomuon/PyIntegral/badges/license.svg)](https://anaconda.org/
 neutrinomuon/PyIntegral/badges/license.svg)
 ===============================================================================
```

### Comparing `PyIntegral-0.0.10/README.md` & `PyIntegral-0.0.11/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ####  A Fortran legacy package to easy integrate numerically
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 © Copyright ®
 
 J.G. - Jean Gomes
 
-last stable version: 0.0.10
+last stable version: 0.0.11
 
 <hr>
 
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)<br>
 [![python3](https://img.shields.io/pypi/pyversions/PyIntegral)](https://img.shields.io/pypi/pyversions/PyIntegral)
 [![badgetlicense](https://anaconda.org/neutrinomuon/PyIntegral/badges/license.svg)](https://anaconda.org/neutrinomuon/PyIntegral/badges/license.svg)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 ### PyIntegral #### A Fortran legacy package to easy integrate numerically
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
 [jean@astro.up.pt](mailto:jean@astro.up.pt) Â© Copyright Â® J.G. - Jean Gomes
-last stable version: 0.0.10
+last stable version: 0.0.11
 ===============================================================================
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)
 [![python3](https://img.shields.io/pypi/pyversions/PyIntegral)](https://
 img.shields.io/pypi/pyversions/PyIntegral) [![badgetlicense](https://
 anaconda.org/neutrinomuon/PyIntegral/badges/license.svg)](https://anaconda.org/
 neutrinomuon/PyIntegral/badges/license.svg)
 ===============================================================================
```

### Comparing `PyIntegral-0.0.10/setup.py` & `PyIntegral-0.0.11/setup.py`

 * *Files identical despite different names*

### Comparing `PyIntegral-0.0.10/src/fortran/DataTypes.f90` & `PyIntegral-0.0.11/src/fortran/DataTypes.f90`

 * *Files identical despite different names*

### Comparing `PyIntegral-0.0.10/src/fortran/GaussLegendreQuadrature.f90` & `PyIntegral-0.0.11/src/fortran/GaussLegendreQuadrature.f90`

 * *Files identical despite different names*

### Comparing `PyIntegral-0.0.10/src/fortran/IntegralALL.f90` & `PyIntegral-0.0.11/src/fortran/IntegralALL.f90`

 * *Files identical despite different names*

### Comparing `PyIntegral-0.0.10/src/fortran/LINinterpol.f90` & `PyIntegral-0.0.11/src/fortran/LINinterpol.f90`

 * *Files identical despite different names*

### Comparing `PyIntegral-0.0.10/src/python/PyIntegralALL.py` & `PyIntegral-0.0.11/src/python/PyIntegral.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 @author: Jean Gomes Copyright (c)
 
 @email: antineutrinomuon@gmail.com
 
 Written: Jean Michel Gomes © Copyright
 """
 
-from pyintegralall import flib
+from PyIntegral import flib
 import numpy as np
 import matplotlib.pyplot as plt
 
-# Class PyIntegralALL
-class PyIntegralALL_class( object ):
+# Class PyIntegral
+class PyIntegral_class( object ):
     ''''Created on 
 Last version on Wed Sep 23 14:33:51 2020
 
 @author: Jean Gomes Copyright (c)
 '''
     def __init__( self, x, y, lambda_i=np.nan, lambda_f=np.nan, int_type=2, verbosity=0 ):
         
@@ -58,15 +58,15 @@
 
 # plt.plot( x,y )
 # plt.plot( x,y*0 )
 
 # plt.step(x, y)
  
 # print(x[0])
-# i_object=PyIntegralALL_class( x,y,lambda_i=-10,lambda_f=-32 )
+# i_object=PyIntegral_class( x,y,lambda_i=-10,lambda_f=-32 )
 
 # print( i_object.integralall )
 
 def main():
     print("")
```

