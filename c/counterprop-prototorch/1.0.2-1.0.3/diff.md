# Comparing `tmp/counterprop_prototorch-1.0.2.tar.gz` & `tmp/counterprop_prototorch-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "counterprop_prototorch-1.0.2.tar", last modified: Wed Jun  7 13:01:25 2023, max compression
+gzip compressed data, was "counterprop_prototorch-1.0.3.tar", last modified: Wed Jun  7 13:16:31 2023, max compression
```

## Comparing `counterprop_prototorch-1.0.2.tar` & `counterprop_prototorch-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/counterpropagation/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/counterpropagation/core/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/core/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/core/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/core/response_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/counterpropagation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/utils/evalmeasure.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/utils/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:16:31.010283 counterprop_prototorch-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-07 13:16:31.010283 counterprop_prototorch-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:16:31.010283 counterprop_prototorch-1.0.3/counterprop_prototorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-07 13:16:30.000000 counterprop_prototorch-1.0.3/counterprop_prototorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-07 13:16:30.000000 counterprop_prototorch-1.0.3/counterprop_prototorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:16:30.000000 counterprop_prototorch-1.0.3/counterprop_prototorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:16:30.000000 counterprop_prototorch-1.0.3/counterprop_prototorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 13:16:30.000000 counterprop_prototorch-1.0.3/counterprop_prototorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 13:16:30.000000 counterprop_prototorch-1.0.3/counterprop_prototorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:16:31.010283 counterprop_prototorch-1.0.3/counterpropagation/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/counterpropagation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:16:31.010283 counterprop_prototorch-1.0.3/counterpropagation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/counterpropagation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/counterpropagation/core/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/counterpropagation/core/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/counterpropagation/core/response_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:16:31.010283 counterprop_prototorch-1.0.3/counterpropagation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/counterpropagation/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/counterpropagation/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/counterpropagation/utils/evalmeasure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/counterpropagation/utils/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:16:31.010283 counterprop_prototorch-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-07 13:16:23.000000 counterprop_prototorch-1.0.3/setup.py
```

### Comparing `counterprop_prototorch-1.0.2/LICENSE` & `counterprop_prototorch-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.2/PKG-INFO` & `counterprop_prototorch-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: counterprop_prototorch
-Version: 1.0.2
+Version: 1.0.3
 Summary: Counter Propagation based on Prototorch. 
 Home-page: https://github.com/rmschubert/Counterpropagation-Prototorch
 Download-URL: https://github.com/rmschubert/Counterpropagation-Prototorch.git
 Author: Ronny Schubert
 Author-email: trebuhcsynnor@gmail.com
 License: MIT
 Classifier: Environment :: Console
```

### Comparing `counterprop_prototorch-1.0.2/README.md` & `counterprop_prototorch-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/PKG-INFO` & `counterprop_prototorch-1.0.3/counterprop_prototorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: counterprop-prototorch
-Version: 1.0.2
+Version: 1.0.3
 Summary: Counter Propagation based on Prototorch. 
 Home-page: https://github.com/rmschubert/Counterpropagation-Prototorch
 Download-URL: https://github.com/rmschubert/Counterpropagation-Prototorch.git
 Author: Ronny Schubert
 Author-email: trebuhcsynnor@gmail.com
 License: MIT
 Classifier: Environment :: Console
```

### Comparing `counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/SOURCES.txt` & `counterprop_prototorch-1.0.3/counterprop_prototorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.2/counterpropagation/core/cp.py` & `counterprop_prototorch-1.0.3/counterpropagation/core/cp.py`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.2/counterpropagation/core/initializer.py` & `counterprop_prototorch-1.0.3/counterpropagation/core/initializer.py`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.2/counterpropagation/core/response_layer.py` & `counterprop_prototorch-1.0.3/counterpropagation/core/response_layer.py`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.2/counterpropagation/utils/callbacks.py` & `counterprop_prototorch-1.0.3/counterpropagation/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.2/counterpropagation/utils/visualization.py` & `counterprop_prototorch-1.0.3/counterpropagation/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.2/setup.py` & `counterprop_prototorch-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 DOWNLOAD_URL = "https://github.com/rmschubert/Counterpropagation-Prototorch.git"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 INSTALL_REQUIRES = [
     "prototorch>=0.7.4",
+    "prototorch_models>=0.5.4",
+    "pytorch-lightning",
     "scipy",
     "torch-kmeans"
 ]
 
 
 setup(
     name="counterprop_prototorch",
-    version="1.0.2",
+    version="1.0.3",
     description="Counter Propagation based on "
     "Prototorch. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ronny Schubert",
     author_email="trebuhcsynnor@gmail.com",
     url=PROJECT_URL,
```

