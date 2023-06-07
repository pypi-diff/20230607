# Comparing `tmp/rdrobust-1.0.8.tar.gz` & `tmp/rdrobust-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/rmasini/Dropbox/rdrobust/Python/rdrobust/dist/.tmp-q4pa9krl/rdrobust-1.0.8.tar", last modified: Thu Feb  9 14:39:35 2023, max compression
+gzip compressed data, was "/Users/rmasini/Dropbox/rdrobust/Python/rdrobust/dist/.tmp-eh1x9bbg/rdrobust-1.0.9.tar", last modified: Wed Jun  7 15:53:54 2023, max compression
```

## Comparing `rdrobust-1.0.8.tar` & `rdrobust-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-02-09 14:39:35.692487 rdrobust-1.0.8/
--rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-02-09 14:39:35.692717 rdrobust-1.0.8/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)     5912 2021-07-26 21:54:29.000000 rdrobust-1.0.8/README.md
--rw-r--r--   0 rmasini    (501) staff       (20)      108 2022-08-11 22:11:33.000000 rdrobust-1.0.8/pyproject.toml
--rw-r--r--   0 rmasini    (501) staff       (20)      809 2023-02-09 14:39:35.693805 rdrobust-1.0.8/setup.cfg
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-02-09 14:39:35.662095 rdrobust-1.0.8/src/
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-02-09 14:39:35.688251 rdrobust-1.0.8/src/rdrobust/
--rwxr-xr-x   0 rmasini    (501) staff       (20)      118 2021-07-08 00:17:48.000000 rdrobust-1.0.8/src/rdrobust/__init__.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    18083 2023-02-09 14:38:02.000000 rdrobust-1.0.8/src/rdrobust/funs.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    27500 2023-02-09 14:37:48.000000 rdrobust-1.0.8/src/rdrobust/rdbwselect.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    30191 2023-02-09 14:37:56.000000 rdrobust-1.0.8/src/rdrobust/rdplot.py
--rwxr-xr-x   0 rmasini    (501) staff       (20)    30992 2023-02-09 14:37:35.000000 rdrobust-1.0.8/src/rdrobust/rdrobust.py
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-02-09 14:39:35.692056 rdrobust-1.0.8/src/rdrobust.egg-info/
--rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-02-09 14:39:35.000000 rdrobust-1.0.8/src/rdrobust.egg-info/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)      334 2023-02-09 14:39:35.000000 rdrobust-1.0.8/src/rdrobust.egg-info/SOURCES.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        1 2023-02-09 14:39:35.000000 rdrobust-1.0.8/src/rdrobust.egg-info/dependency_links.txt
--rw-r--r--   0 rmasini    (501) staff       (20)       36 2023-02-09 14:39:35.000000 rdrobust-1.0.8/src/rdrobust.egg-info/requires.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        9 2023-02-09 14:39:35.000000 rdrobust-1.0.8/src/rdrobust.egg-info/top_level.txt
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-07 15:53:54.696076 rdrobust-1.0.9/
+-rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-06-07 15:53:54.696326 rdrobust-1.0.9/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)     5912 2021-07-26 21:54:29.000000 rdrobust-1.0.9/README.md
+-rw-r--r--   0 rmasini    (501) staff       (20)      108 2022-08-11 22:11:33.000000 rdrobust-1.0.9/pyproject.toml
+-rw-r--r--   0 rmasini    (501) staff       (20)      828 2023-06-07 15:53:54.697313 rdrobust-1.0.9/setup.cfg
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-07 15:53:54.665420 rdrobust-1.0.9/src/
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-07 15:53:54.690528 rdrobust-1.0.9/src/rdrobust/
+-rwxr-xr-x   0 rmasini    (501) staff       (20)      142 2023-06-07 15:51:19.000000 rdrobust-1.0.9/src/rdrobust/__init__.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    18074 2023-06-07 15:51:02.000000 rdrobust-1.0.9/src/rdrobust/funs.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    27460 2023-06-07 15:50:22.000000 rdrobust-1.0.9/src/rdrobust/rdbwselect.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    30156 2023-06-07 15:50:48.000000 rdrobust-1.0.9/src/rdrobust/rdplot.py
+-rwxr-xr-x   0 rmasini    (501) staff       (20)    30912 2023-06-07 15:50:40.000000 rdrobust-1.0.9/src/rdrobust/rdrobust.py
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-07 15:53:54.695546 rdrobust-1.0.9/src/rdrobust.egg-info/
+-rw-r--r--   0 rmasini    (501) staff       (20)     6513 2023-06-07 15:53:54.000000 rdrobust-1.0.9/src/rdrobust.egg-info/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)      334 2023-06-07 15:53:54.000000 rdrobust-1.0.9/src/rdrobust.egg-info/SOURCES.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        1 2023-06-07 15:53:54.000000 rdrobust-1.0.9/src/rdrobust.egg-info/dependency_links.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)       55 2023-06-07 15:53:54.000000 rdrobust-1.0.9/src/rdrobust.egg-info/requires.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        9 2023-06-07 15:53:54.000000 rdrobust-1.0.9/src/rdrobust.egg-info/top_level.txt
```

### Comparing `rdrobust-1.0.8/PKG-INFO` & `rdrobust-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdrobust
-Version: 1.0.8
+Version: 1.0.9
 Summary: Implements local polynomial Regression Discontinuity (RD) point estimators with robust bias-corrected confidence intervals and inference procedures.
 Home-page: https://github.com/rdpackages/rdrobust
 Author: Ricardo Masini
 Author-email: rmasini@princeton.edu
 Project-URL: Bug Tracker, https://github.com/rdpackages/rdrobust/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rdrobust-1.0.8/README.md` & `rdrobust-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rdrobust-1.0.8/setup.cfg` & `rdrobust-1.0.9/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rdrobust
-version = 1.0.8
+version = 1.0.9
 author = Ricardo Masini
 author_email = rmasini@princeton.edu
 description = Implements local polynomial Regression Discontinuity (RD) point estimators with robust bias-corrected confidence intervals and inference procedures.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rdpackages/rdrobust
 project_urls = 
@@ -17,17 +17,17 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy
-	pandas
+	pandas>=2.0.0
 	scipy
-	sklearn
+	scikit-learn>=1.2.0
 	plotnine
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `rdrobust-1.0.8/src/rdrobust/funs.py` & `rdrobust-1.0.9/src/rdrobust/funs.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,36 +97,35 @@
         print('-'*73)
         
         if self.all is None: method_id = (0,2)
         else: method_id = (0,1,2)
         for j in method_id:
             if j==0:
                 print(self.coef.index[j].ljust(fw_l),
-                      str(round(float(self.coef.iloc[j]),n_dec)).rjust(fw_c),
-                      str(round(float(self.se.iloc[j]),n_dec)).rjust(fw_c),
-                      str(round(float(self.t.iloc[j]),n_dec)).rjust(fw_c),
-                      ("{:.3e}".format(float(self.pv.iloc[j]))).rjust(fw_c+3),
-                      ('[' + str(round(float(self.ci.iloc[j,0]),n_dec)) + ', ' + str(round(float(self.ci.iloc[j,1]),n_dec)) + ']').rjust(fw_ci))
+                      str(round(self.coef.iloc[j].item(),n_dec)).rjust(fw_c),
+                      str(round(self.se.iloc[j].item(),n_dec)).rjust(fw_c),
+                      str(round(self.t.iloc[j].item(),n_dec)).rjust(fw_c),
+                      ("{:.3e}".format(self.pv.iloc[j].item())).rjust(fw_c+3),
+                      ('[' + str(round(self.ci.iloc[j,0].item(),n_dec)) + ', ' + str(round(self.ci.iloc[j,1].item(),n_dec)) + ']').rjust(fw_ci))
             else:
                 if self.all:
                     print(self.coef.index[j].ljust(fw_l),
-                      str(round(float(self.coef.iloc[j]),n_dec)).rjust(fw_c),
-                      str(round(float(self.se.iloc[j]),n_dec)).rjust(fw_c),
-                      str(round(float(self.t.iloc[j]),n_dec)).rjust(fw_c),
-                      ("{:.3e}".format(float(self.pv.iloc[j]))).rjust(fw_c+3),
-                      ('[' + str(round(float(self.ci.iloc[j,0]),n_dec)) + ', ' + str(round(float(self.ci.iloc[j,1]),n_dec)) + ']').rjust(fw_ci))
+                      str(round(self.coef.iloc[j].item(),n_dec)).rjust(fw_c),
+                      str(round(self.se.iloc[j].item(),n_dec)).rjust(fw_c),
+                      str(round(self.t.iloc[j].item(),n_dec)).rjust(fw_c),
+                      ("{:.3e}".format(self.pv.iloc[j].item())).rjust(fw_c+3),
+                      ('[' + str(round(self.ci.iloc[j,0].item(),n_dec)) + ', ' + str(round(self.ci.iloc[j,1].item(),n_dec)) + ']').rjust(fw_ci))
                 else:
                     print(self.coef.index[j].ljust(fw_l),
                       '-'.rjust(fw_c),
                       '-'.rjust(fw_c),
-                      str(round(float(self.t.iloc[j]),n_dec)).rjust(fw_c),
-                      ("{:.3e}".format(float(self.pv.iloc[j]))).rjust(fw_c+3),
-                      ('[' + str(round(float(self.ci.iloc[j,0]),n_dec)) + ', ' + str(round(float(self.ci.iloc[j,1]),n_dec)) + ']').rjust(fw_ci))
-
-                
+                      str(round(self.t.iloc[j].item(),n_dec)).rjust(fw_c),
+                      ("{:.3e}".format(self.pv.iloc[j].item())).rjust(fw_c+3),
+                      ('[' + str(round(self.ci.iloc[j,0].item(),n_dec)) + ', ' + str(round(self.ci.iloc[j,1].item(),n_dec)) + ']').rjust(fw_ci))
+        
         return ''
 
 class rdplot_output:
     def __init__(self, coef, rdplot, vars_bins, vars_poly, J, J_IMSE, J_MV, 
                  scale, rscale, bin_avg, bin_med, p, c, h, N, N_h,
                  binselect, kernel):
         self.coef = coef
```

### Comparing `rdrobust-1.0.8/src/rdrobust/rdbwselect.py` & `rdrobust-1.0.9/src/rdrobust/rdbwselect.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Created on Wed Jul  7 18:57:15 2021
 
 @author: rmasini
 """
 
 import numpy as np
 import pandas as pd
-from .funs import *  # relative path here .funs to make the package
+from rdrobust.funs import *
 
 def rdbwselect(y, x, c = None, fuzzy = None, deriv = None, p = None, q = None,
                covs = None, covs_drop = True, kernel = "tri", weights = None, 
                bwselect = "mserd", vce = "nn", cluster = None, nnmatch = 3,
                scaleregul = 1, sharpbw = False, all = None, subset = None,
                masspoints = "adjust", bwcheck = None, bwrestrict = True,
                stdvars = False, prchk = True):
```

### Comparing `rdrobust-1.0.8/src/rdrobust/rdplot.py` & `rdrobust-1.0.9/src/rdrobust/rdplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import numpy as np
 import scipy.stats as sct
 import pandas  as pd
 from sklearn.linear_model import LinearRegression as LR
 from plotnine import *
-from .funs import *  # relative path here .fun to make package
+from rdrobust.funs import *
 
 
 def rdplot(y, x, c = 0, p = 4, nbins = None, binselect = "esmv", scale = None, 
                   kernel = "uni", weights = None, h = None, 
                   covs = None,  covs_eval = "mean", covs_drop = True,
                   support = None, subset = None, masspoints = "adjust",
                   hide = False, ci = None, shade = False,
```

### Comparing `rdrobust-1.0.8/src/rdrobust/rdrobust.py` & `rdrobust-1.0.9/src/rdrobust/rdrobust.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 @author: rmasini
 """
 
 import numpy as np
 import pandas  as pd
 import scipy.stats as sct
-from .rdbwselect import rdbwselect    # relative path here .rdbwselect to make package
-from .funs import *  # relative path here .funs to make package
+from rdrobust.rdbwselect import rdbwselect
+from rdrobust.funs import *
      
 def rdrobust(y, x, c = None, fuzzy = None, deriv = None,
              p = None, q = None, h = None, b = None, rho = None, 
              covs = None, covs_drop = True,
              kernel = "tri", weights = None, bwselect = "mserd",
              vce = "nn", cluster = None, nnmatch = 3, level = 95, 
              scalepar = 1, scaleregul = 1, sharpbw = False,
```

### Comparing `rdrobust-1.0.8/src/rdrobust.egg-info/PKG-INFO` & `rdrobust-1.0.9/src/rdrobust.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdrobust
-Version: 1.0.8
+Version: 1.0.9
 Summary: Implements local polynomial Regression Discontinuity (RD) point estimators with robust bias-corrected confidence intervals and inference procedures.
 Home-page: https://github.com/rdpackages/rdrobust
 Author: Ricardo Masini
 Author-email: rmasini@princeton.edu
 Project-URL: Bug Tracker, https://github.com/rdpackages/rdrobust/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

