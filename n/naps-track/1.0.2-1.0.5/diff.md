# Comparing `tmp/naps-track-1.0.2.tar.gz` & `tmp/naps-track-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/naps-track-1.0.2.tar", last modified: Tue Jan 10 19:03:28 2023, max compression
+gzip compressed data, was "dist/naps-track-1.0.5.tar", last modified: Wed Jun  7 02:49:04 2023, max compression
```

## Comparing `naps-track-1.0.2.tar` & `naps-track-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 19:03:28.000000 naps-track-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-10 19:03:24.000000 naps-track-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-01-10 19:03:28.000000 naps-track-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-01-10 19:03:24.000000 naps-track-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 19:03:28.000000 naps-track-1.0.2/naps/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-01-10 19:03:24.000000 naps-track-1.0.2/naps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-01-10 19:03:24.000000 naps-track-1.0.2/naps/aruco.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-01-10 19:03:24.000000 naps-track-1.0.2/naps/cost_matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6978 2023-01-10 19:03:24.000000 naps-track-1.0.2/naps/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-01-10 19:03:24.000000 naps-track-1.0.2/naps/naps_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-01-10 19:03:24.000000 naps-track-1.0.2/naps/sleap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 19:03:28.000000 naps-track-1.0.2/naps_track.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-01-10 19:03:27.000000 naps-track-1.0.2/naps_track.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-10 19:03:28.000000 naps-track-1.0.2/naps_track.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 19:03:27.000000 naps-track-1.0.2/naps_track.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-10 19:03:27.000000 naps-track-1.0.2/naps_track.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-10 19:03:27.000000 naps-track-1.0.2/naps_track.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-10 19:03:27.000000 naps-track-1.0.2/naps_track.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-10 19:03:24.000000 naps-track-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-10 19:03:28.000000 naps-track-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-01-10 19:03:24.000000 naps-track-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:49:04.000000 naps-track-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 02:48:56.000000 naps-track-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-07 02:49:04.000000 naps-track-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-07 02:48:56.000000 naps-track-1.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/aruco.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/cost_matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6978 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/matching.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3902 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/naps_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/naps_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/naps_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/sleap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8011 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/utils/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/utils/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 02:48:57.000000 naps-track-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 02:49:04.000000 naps-track-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-07 02:48:57.000000 naps-track-1.0.5/setup.py
```

### Comparing `naps-track-1.0.2/PKG-INFO` & `naps-track-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naps-track
-Version: 1.0.2
+Version: 1.0.5
 Summary: NAPS (NAPS is ArUco Plus SLEAP)
 Home-page: https://github.com/kocherlab/naps
 License: MIT
 Project-URL: Documentation, https://naps.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/kocherlab/naps
 Project-URL: Issue tracker, https://github.com/kocherlab/naps/issues
 Description: |Stable version| |Latest version| |Documentation| |github ci| |Coverage| |conda| |Conda Upload| |PyPI Upload| |LICENSE|
@@ -66,15 +66,14 @@
         
         ========
         Features
         ========
         * Easy, direct installation across platforms
         * Built directly on top of `OpenCV <https://opencv.org/>`_ and `SLEAP <https://sleap.ai/>`_ with a modular, extensible codebase
         * Flexible API that allows drop in of different methods for marker identification
-        * Multiprocessing through `Ray <https://docs.ray.io/>`_
         
         
         ============
         Getting NAPS
         ============
         
         ------------
@@ -152,9 +151,9 @@
         ================
         Acknowledgements
         ================
         
         Much of the structure and content of the README and the documentation is borrowed from the `SLEAP repository <https://github.com/talmolab/sleap>`_.
         
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `naps-track-1.0.2/README.rst` & `naps-track-1.0.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 
 ========
 Features
 ========
 * Easy, direct installation across platforms
 * Built directly on top of `OpenCV <https://opencv.org/>`_ and `SLEAP <https://sleap.ai/>`_ with a modular, extensible codebase
 * Flexible API that allows drop in of different methods for marker identification
-* Multiprocessing through `Ray <https://docs.ray.io/>`_
 
 
 ============
 Getting NAPS
 ============
 
 ------------
```

### Comparing `naps-track-1.0.2/naps/aruco.py` & `naps-track-1.0.5/naps/aruco.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.2/naps/cost_matrix.py` & `naps-track-1.0.5/naps/cost_matrix.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.2/naps/matching.py` & `naps-track-1.0.5/naps/matching.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.2/naps/sleap_utils.py` & `naps-track-1.0.5/naps/sleap_utils.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.2/naps_track.egg-info/PKG-INFO` & `naps-track-1.0.5/naps_track.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naps-track
-Version: 1.0.2
+Version: 1.0.5
 Summary: NAPS (NAPS is ArUco Plus SLEAP)
 Home-page: https://github.com/kocherlab/naps
 License: MIT
 Project-URL: Documentation, https://naps.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/kocherlab/naps
 Project-URL: Issue tracker, https://github.com/kocherlab/naps/issues
 Description: |Stable version| |Latest version| |Documentation| |github ci| |Coverage| |conda| |Conda Upload| |PyPI Upload| |LICENSE|
@@ -66,15 +66,14 @@
         
         ========
         Features
         ========
         * Easy, direct installation across platforms
         * Built directly on top of `OpenCV <https://opencv.org/>`_ and `SLEAP <https://sleap.ai/>`_ with a modular, extensible codebase
         * Flexible API that allows drop in of different methods for marker identification
-        * Multiprocessing through `Ray <https://docs.ray.io/>`_
         
         
         ============
         Getting NAPS
         ============
         
         ------------
@@ -152,9 +151,9 @@
         ================
         Acknowledgements
         ================
         
         Much of the structure and content of the README and the documentation is borrowed from the `SLEAP repository <https://github.com/talmolab/sleap>`_.
         
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `naps-track-1.0.2/setup.py` & `naps-track-1.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,30 +13,34 @@
 requirement_path = lib_folder + "/requirements.txt"
 requirements = []
 if os.path.isfile(requirement_path):
     with open(requirement_path) as f:
         requirements = f.read().splitlines()
 
 # Executable scripts in the package
-tool_scripts = ["naps/naps_track.py"]
+tool_scripts = ["naps/naps_track.py", "naps/naps_plot.py", "naps/naps_interactions.py"]
 
 setup(
     name=naps.__name__,
     version=naps.__version__,
     project_urls={
         "Documentation": naps.__docs__,
         "Code": naps.__code__,
         "Issue tracker": naps.__issue__,
     },
     license=naps.__license__,
     url=naps.__url__,
     description=naps.__summary__,
     long_description_content_type="text/x-rst",
     long_description=readme,
-    packages=["naps"],
+    packages=["naps", "naps.utils"],
     install_requires=requirements,
     scripts=tool_scripts,
     entry_points={
-        "console_scripts": ["naps-track=naps.naps_track:main"],
+        "console_scripts": [
+            "naps-track=naps.naps_track:main",
+            "naps-plot=naps.naps_plot:main",
+            "naps-interactions=naps.naps_interactions:main",
+        ],
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
 )
```

