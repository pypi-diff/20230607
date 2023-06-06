# Comparing `tmp/robotransforms-0.5.4.tar.gz` & `tmp/robotransforms-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotransforms-0.5.4.tar", last modified: Tue Jun  6 21:31:17 2023, max compression
+gzip compressed data, was "robotransforms-0.5.5.tar", last modified: Tue Jun  6 23:39:16 2023, max compression
```

## Comparing `robotransforms-0.5.4.tar` & `robotransforms-0.5.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.228878 robotransforms-0.5.4/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1076 2022-12-01 23:55:43.000000 robotransforms-0.5.4/LICENSE
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       37 2022-12-02 15:43:21.000000 robotransforms-0.5.4/MANIFEST.in
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-06-06 21:31:17.224878 robotransforms-0.5.4/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      347 2023-05-03 23:31:19.000000 robotransforms-0.5.4/README.md
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       60 2023-05-03 23:34:03.000000 robotransforms-0.5.4/pyproject.toml
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.220878 robotransforms-0.5.4/robotransforms/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      148 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       22 2023-06-06 21:29:02.000000 robotransforms-0.5.4/robotransforms/_version.py
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.224878 robotransforms-0.5.4/robotransforms/dead_reckon/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/dead_reckon/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11493 2023-06-06 21:25:33.000000 robotransforms-0.5.4/robotransforms/dead_reckon/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      732 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/dead_reckon/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2811 2023-03-07 00:07:47.000000 robotransforms-0.5.4/robotransforms/dead_reckon/dead_reckon.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8728 2023-06-06 21:27:21.000000 robotransforms-0.5.4/robotransforms/dead_reckon/dead_reckon_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    15825 2023-03-07 00:44:08.000000 robotransforms-0.5.4/robotransforms/dead_reckon/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.224878 robotransforms-0.5.4/robotransforms/euclidean/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      120 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/euclidean/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8310 2023-05-03 23:28:26.000000 robotransforms-0.5.4/robotransforms/euclidean/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1566 2023-05-03 23:28:26.000000 robotransforms-0.5.4/robotransforms/euclidean/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11585 2023-05-03 23:28:26.000000 robotransforms-0.5.4/robotransforms/euclidean/euclidean.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14307 2023-05-04 15:04:49.000000 robotransforms-0.5.4/robotransforms/euclidean/euclidean_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6960 2023-05-03 23:28:26.000000 robotransforms-0.5.4/robotransforms/euclidean/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.224878 robotransforms-0.5.4/robotransforms/utils/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       55 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/utils/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     3680 2022-12-02 19:58:46.000000 robotransforms-0.5.4/robotransforms/utils/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      351 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/utils/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      545 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/utils/utils.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1055 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/utils/utils_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6290 2022-12-02 15:43:21.000000 robotransforms-0.5.4/robotransforms/utils/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 21:31:17.220878 robotransforms-0.5.4/robotransforms.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-06-06 21:31:17.000000 robotransforms-0.5.4/robotransforms.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      943 2023-06-06 21:31:17.000000 robotransforms-0.5.4/robotransforms.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-06-06 21:31:17.000000 robotransforms-0.5.4/robotransforms.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       12 2023-06-06 21:31:17.000000 robotransforms-0.5.4/robotransforms.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2023-06-06 21:31:17.000000 robotransforms-0.5.4/robotransforms.egg-info/top_level.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-06-06 21:31:17.228878 robotransforms-0.5.4/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1907 2022-12-02 17:09:02.000000 robotransforms-0.5.4/setup.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 23:39:16.572397 robotransforms-0.5.5/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1076 2022-12-01 23:55:43.000000 robotransforms-0.5.5/LICENSE
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       37 2022-12-02 15:43:21.000000 robotransforms-0.5.5/MANIFEST.in
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-06-06 23:39:16.572397 robotransforms-0.5.5/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      347 2023-05-03 23:31:19.000000 robotransforms-0.5.5/README.md
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       60 2023-05-03 23:34:03.000000 robotransforms-0.5.5/pyproject.toml
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 23:39:16.568397 robotransforms-0.5.5/robotransforms/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      148 2022-12-02 15:43:21.000000 robotransforms-0.5.5/robotransforms/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       22 2023-06-06 23:36:37.000000 robotransforms-0.5.5/robotransforms/_version.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 23:39:16.568397 robotransforms-0.5.5/robotransforms/dead_reckon/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2022-12-02 15:43:21.000000 robotransforms-0.5.5/robotransforms/dead_reckon/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11552 2023-06-06 23:37:59.000000 robotransforms-0.5.5/robotransforms/dead_reckon/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      732 2022-12-02 15:43:21.000000 robotransforms-0.5.5/robotransforms/dead_reckon/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2811 2023-03-07 00:07:47.000000 robotransforms-0.5.5/robotransforms/dead_reckon/dead_reckon.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8769 2023-06-06 23:38:34.000000 robotransforms-0.5.5/robotransforms/dead_reckon/dead_reckon_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    15825 2023-03-07 00:44:08.000000 robotransforms-0.5.5/robotransforms/dead_reckon/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 23:39:16.568397 robotransforms-0.5.5/robotransforms/euclidean/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      120 2022-12-02 15:43:21.000000 robotransforms-0.5.5/robotransforms/euclidean/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8310 2023-05-03 23:28:26.000000 robotransforms-0.5.5/robotransforms/euclidean/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1566 2023-05-03 23:28:26.000000 robotransforms-0.5.5/robotransforms/euclidean/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11585 2023-05-03 23:28:26.000000 robotransforms-0.5.5/robotransforms/euclidean/euclidean.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14307 2023-05-04 15:04:49.000000 robotransforms-0.5.5/robotransforms/euclidean/euclidean_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6960 2023-05-03 23:28:26.000000 robotransforms-0.5.5/robotransforms/euclidean/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 23:39:16.572397 robotransforms-0.5.5/robotransforms/utils/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       55 2022-12-02 15:43:21.000000 robotransforms-0.5.5/robotransforms/utils/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     3680 2022-12-02 19:58:46.000000 robotransforms-0.5.5/robotransforms/utils/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      351 2022-12-02 15:43:21.000000 robotransforms-0.5.5/robotransforms/utils/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      545 2022-12-02 15:43:21.000000 robotransforms-0.5.5/robotransforms/utils/utils.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1055 2022-12-02 15:43:21.000000 robotransforms-0.5.5/robotransforms/utils/utils_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6290 2022-12-02 15:43:21.000000 robotransforms-0.5.5/robotransforms/utils/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-06 23:39:16.568397 robotransforms-0.5.5/robotransforms.egg-info/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-06-06 23:39:16.000000 robotransforms-0.5.5/robotransforms.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      943 2023-06-06 23:39:16.000000 robotransforms-0.5.5/robotransforms.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-06-06 23:39:16.000000 robotransforms-0.5.5/robotransforms.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       12 2023-06-06 23:39:16.000000 robotransforms-0.5.5/robotransforms.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2023-06-06 23:39:16.000000 robotransforms-0.5.5/robotransforms.egg-info/top_level.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-06-06 23:39:16.572397 robotransforms-0.5.5/setup.cfg
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1907 2022-12-02 17:09:02.000000 robotransforms-0.5.5/setup.py
```

### Comparing `robotransforms-0.5.4/LICENSE` & `robotransforms-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/PKG-INFO` & `robotransforms-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotransforms
-Version: 0.5.4
+Version: 0.5.5
 Summary: A transformation library for robot motion
 Home-page: https://github.com/Nova-Dynamics/transforms-python
 Author: Jonathan D. B. Van Schenck
 Author-email: jvschenck@novadynamics.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `robotransforms-0.5.4/robotransforms/dead_reckon/base.cpp` & `robotransforms-0.5.5/robotransforms/dead_reckon/base.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #include <math.h>
 #include <algorithm>
 
 #include "../utils/base.h"
 #include "../euclidean/base.h"
 #include "base.h"
 
+// var_de ~ 4*var_dq = (2 * delta_dq)^2 ~ var_ypr
+constexpr double MAGIC_ROTVEC_ERROR = 1e-6;
+
 constexpr double DR_D_NOM = 0.464;
 constexpr double DR_LO2G = 0.05;
 constexpr double DR_MU = 0.8;
 constexpr double DR_D_EFF_PARAMS[3] = {0.505225138, 4.55440687, 0.00237199585};
 
 // Is this a bad idea?
 constexpr double L_PLUS_LAMBDA = 3;
@@ -65,15 +68,15 @@
         if ( std::abs(vdiff) >= 1e-3 ) {
             rho = std::abs(std::tanh( vave / vdiff ));
         }
 
         // TODO : make this configurable in the future
         // TODO : do we actually need the penalty?
         // the dq has a rotvec representation [ e1, e2, e3 ], these are the errors therein
-        double var_de = 1e-5; // var_de ~ 4*var_dq = (2 * delta_dq)^2 ~ var_ypr
+        double var_de = MAGIC_ROTVEC_ERROR;
         out[0] = ddl*ddl + 1e-8;
         out[1] = rho*ddl*ddr;
         out[2] = ddr*ddr + 1e-8;
         out[3] = var_de;
         out[4] = var_de;
         out[5] = var_de;
     }
```

### Comparing `robotransforms-0.5.4/robotransforms/dead_reckon/base.h` & `robotransforms-0.5.5/robotransforms/dead_reckon/base.h`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms/dead_reckon/dead_reckon.py` & `robotransforms-0.5.5/robotransforms/dead_reckon/dead_reckon.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms/dead_reckon/dead_reckon_pure.py` & `robotransforms-0.5.5/robotransforms/dead_reckon/dead_reckon_pure.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 L_PLUS_LAMBDA = 3
 
 def sinc(x):
     # Use power series for small x
     if (np.abs(x) < 1e-4): return 1 - (x*x/6) + (x*x*x*x/120)
     return np.sin(x)/x
 
+# var_de ~ 4*var_dq = (2 * delta_dq)^2 ~ var_ypr
+MAGIC_ROTVEC_ERROR = 1e-6
+
 DR_D_NOM = 0.464
 DR_LO2G = 0.05
 DR_MU = 0.8
 DR_D_EFF_PARAMS = [0.505225138, 4.55440687, 0.00237199585]
 
 def dr_calculate_d(v_ave,v_diff):
     _v_diff = v_diff
@@ -50,15 +53,15 @@
     rho = 1-1e-8
     if ( np.abs(vdiff) >= 1e-3 ) :
         rho = np.abs(np.tanh( vave / vdiff ))
 
     # TODO : make this configurable in the future
     # TODO : do we actually need the penalty?
     # the dq has a rotvec representation [ e1, e2, e3 ], these are the errors therein
-    var_de = 1e-5 # var_de ~ 4*var_dq = (2 * delta_dq)^2 ~ var_ypr
+    var_de = MAGIC_ROTVEC_ERROR
     #  [ var_dl, cov_dldr, var_dr, var_dqb, var_dqc, var_dqd ]
     return [ ddl*ddl + 1e-8, rho*ddl*ddr, ddr*ddr + 1e-8, var_de, var_de, var_de ] # TODO : these are estimates, based on gps's 1Hz
 
 def dead_reckon_apply(x_hat, P_hat, step):
     SS = 7 # Full state size
     ESS = 7 + 2 + 4 # dl/dr and then dq
     SM = 6 # Manifold state size
```

### Comparing `robotransforms-0.5.4/robotransforms/dead_reckon/wrapper.cpp` & `robotransforms-0.5.5/robotransforms/dead_reckon/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms/euclidean/base.cpp` & `robotransforms-0.5.5/robotransforms/euclidean/base.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms/euclidean/base.h` & `robotransforms-0.5.5/robotransforms/euclidean/base.h`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms/euclidean/euclidean.py` & `robotransforms-0.5.5/robotransforms/euclidean/euclidean.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms/euclidean/euclidean_pure.py` & `robotransforms-0.5.5/robotransforms/euclidean/euclidean_pure.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms/euclidean/wrapper.cpp` & `robotransforms-0.5.5/robotransforms/euclidean/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms/utils/base.cpp` & `robotransforms-0.5.5/robotransforms/utils/base.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms/utils/utils.py` & `robotransforms-0.5.5/robotransforms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms/utils/utils_pure.py` & `robotransforms-0.5.5/robotransforms/utils/utils_pure.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms/utils/wrapper.cpp` & `robotransforms-0.5.5/robotransforms/utils/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/robotransforms.egg-info/PKG-INFO` & `robotransforms-0.5.5/robotransforms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotransforms
-Version: 0.5.4
+Version: 0.5.5
 Summary: A transformation library for robot motion
 Home-page: https://github.com/Nova-Dynamics/transforms-python
 Author: Jonathan D. B. Van Schenck
 Author-email: jvschenck@novadynamics.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `robotransforms-0.5.4/robotransforms.egg-info/SOURCES.txt` & `robotransforms-0.5.5/robotransforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.4/setup.py` & `robotransforms-0.5.5/setup.py`

 * *Files identical despite different names*

