# Comparing `tmp/lifetimefitting-0.0.24.tar.gz` & `tmp/lifetimefitting-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.24.tar", last modified: Mon Jun  5 06:06:22 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.25.tar", last modified: Tue Jun  6 23:42:51 2023, max compression
```

## Comparing `lifetimefitting-0.0.24.tar` & `lifetimefitting-0.0.25.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:22.080037 lifetimefitting-0.0.24/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-05 06:06:22.080037 lifetimefitting-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:22.076037 lifetimefitting-0.0.24/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:22.076037 lifetimefitting-0.0.24/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:22.080037 lifetimefitting-0.0.24/app/lifetimefitting/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/funcs/expFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/funcs/fittingFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/funcs/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:22.080037 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-05 06:06:22.000000 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 06:06:22.000000 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:06:22.000000 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 06:06:22.000000 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 06:06:22.000000 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 06:06:22.080037 lifetimefitting-0.0.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:42:51.761957 lifetimefitting-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-06 23:42:39.000000 lifetimefitting-0.0.25/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-06 23:42:51.761957 lifetimefitting-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-06 23:42:39.000000 lifetimefitting-0.0.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:42:51.757957 lifetimefitting-0.0.25/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:42:51.757957 lifetimefitting-0.0.25/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 23:42:39.000000 lifetimefitting-0.0.25/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-06 23:42:39.000000 lifetimefitting-0.0.25/app/lifetimefitting/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:42:51.761957 lifetimefitting-0.0.25/app/lifetimefitting/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 23:42:39.000000 lifetimefitting-0.0.25/app/lifetimefitting/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-06 23:42:39.000000 lifetimefitting-0.0.25/app/lifetimefitting/funcs/expFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-06 23:42:39.000000 lifetimefitting-0.0.25/app/lifetimefitting/funcs/fittingFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-06-06 23:42:39.000000 lifetimefitting-0.0.25/app/lifetimefitting/funcs/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:42:51.761957 lifetimefitting-0.0.25/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-06 23:42:51.000000 lifetimefitting-0.0.25/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 23:42:51.000000 lifetimefitting-0.0.25/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:42:51.000000 lifetimefitting-0.0.25/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 23:42:51.000000 lifetimefitting-0.0.25/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 23:42:51.000000 lifetimefitting-0.0.25/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 23:42:51.761957 lifetimefitting-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-06 23:42:39.000000 lifetimefitting-0.0.25/setup.py
```

### Comparing `lifetimefitting-0.0.24/LICENSE.md` & `lifetimefitting-0.0.25/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.24/PKG-INFO` & `lifetimefitting-0.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.24
+Version: 0.0.25
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.24/README.md` & `lifetimefitting-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.24/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.25/app/lifetimefitting/__main__.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.24/app/lifetimefitting/funcs/expFuncs.py` & `lifetimefitting-0.0.25/app/lifetimefitting/funcs/expFuncs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.24/app/lifetimefitting/funcs/fittingFuncs.py` & `lifetimefitting-0.0.25/app/lifetimefitting/funcs/fittingFuncs.py`

 * *Files identical despite different names*

```diff
@@ -48,15 +48,15 @@
 
     for i in range(expCount):
         minbounds += [0, 0]
         maxbounds += [99999999, 1]
 
     popt, pcov = curve_fit(fitFunc, x, y,
                            bounds=(minbounds, maxbounds),
-                           maxfev=maxIter,
+                        #    maxfev=maxIter,
                            max_nfev=999999999999,
                            # verbose=2,
                            )
 
     residual = np.sum(np.subtract(y, FLFuncList[expCount](x, *popt)))
 
     return popt, residual
```

### Comparing `lifetimefitting-0.0.24/app/lifetimefitting/funcs/gui.py` & `lifetimefitting-0.0.25/app/lifetimefitting/funcs/gui.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.24/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.25/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.24
+Version: 0.0.25
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.24/setup.py` & `lifetimefitting-0.0.25/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.24",
+    version = "0.0.25",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
```

