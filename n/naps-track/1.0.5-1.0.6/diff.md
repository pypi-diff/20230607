# Comparing `tmp/naps-track-1.0.5.tar.gz` & `tmp/naps-track-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/naps-track-1.0.5.tar", last modified: Wed Jun  7 02:49:04 2023, max compression
+gzip compressed data, was "dist/naps-track-1.0.6.tar", last modified: Wed Jun  7 16:10:40 2023, max compression
```

## Comparing `naps-track-1.0.5.tar` & `naps-track-1.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:49:04.000000 naps-track-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 02:48:56.000000 naps-track-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-07 02:49:04.000000 naps-track-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-07 02:48:56.000000 naps-track-1.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/aruco.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/cost_matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6978 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/matching.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3902 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/naps_interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/naps_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/naps_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/sleap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8011 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/utils/interactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-06-07 02:48:57.000000 naps-track-1.0.5/naps/utils/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 02:49:04.000000 naps-track-1.0.5/naps_track.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 02:48:57.000000 naps-track-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 02:49:04.000000 naps-track-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-07 02:48:57.000000 naps-track-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:40.000000 naps-track-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 16:10:34.000000 naps-track-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-07 16:10:40.000000 naps-track-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-07 16:10:34.000000 naps-track-1.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:40.000000 naps-track-1.0.6/naps/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/aruco.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/cost_matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6978 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/matching.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3902 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/naps_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/naps_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/naps_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/sleap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:40.000000 naps-track-1.0.6/naps/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8011 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/utils/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-06-07 16:10:34.000000 naps-track-1.0.6/naps/utils/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:40.000000 naps-track-1.0.6/naps_track.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-07 16:10:39.000000 naps-track-1.0.6/naps_track.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-07 16:10:40.000000 naps-track-1.0.6/naps_track.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:10:39.000000 naps-track-1.0.6/naps_track.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 16:10:39.000000 naps-track-1.0.6/naps_track.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 16:10:39.000000 naps-track-1.0.6/naps_track.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 16:10:39.000000 naps-track-1.0.6/naps_track.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 16:10:34.000000 naps-track-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:10:40.000000 naps-track-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-07 16:10:34.000000 naps-track-1.0.6/setup.py
```

### Comparing `naps-track-1.0.5/PKG-INFO` & `naps-track-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naps-track
-Version: 1.0.5
+Version: 1.0.6
 Summary: NAPS (NAPS is ArUco Plus SLEAP)
 Home-page: https://github.com/kocherlab/naps
 License: MIT
 Project-URL: Documentation, https://naps.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/kocherlab/naps
 Project-URL: Issue tracker, https://github.com/kocherlab/naps/issues
 Description: |Stable version| |Latest version| |Documentation| |github ci| |Coverage| |conda| |Conda Upload| |PyPI Upload| |LICENSE|
```

### Comparing `naps-track-1.0.5/README.rst` & `naps-track-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.5/naps/__init__.py` & `naps-track-1.0.6/naps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 # from naps import utils
 # import naps.utils
 
 # Basic Information
 __name__ = "naps-track"
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 __summary__ = "NAPS (NAPS is ArUco Plus SLEAP)"
 __url__ = "https://github.com/kocherlab/naps"
 __code__ = "https://github.com/kocherlab/naps"
 __issue__ = "https://github.com/kocherlab/naps/issues"
 __docs__ = "https://naps.readthedocs.io/en/latest/"
 __license__ = "MIT"
 __copyright__ = "2022"
```

### Comparing `naps-track-1.0.5/naps/aruco.py` & `naps-track-1.0.6/naps/aruco.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.5/naps/cost_matrix.py` & `naps-track-1.0.6/naps/cost_matrix.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.5/naps/matching.py` & `naps-track-1.0.6/naps/matching.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.5/naps/naps_interactions.py` & `naps-track-1.0.6/naps/naps_interactions.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.5/naps/naps_plot.py` & `naps-track-1.0.6/naps/naps_plot.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.5/naps/naps_track.py` & `naps-track-1.0.6/naps/naps_track.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,21 @@
         "--end-frame",
         help="The zero-based fully-closed frame to stop NAPS assignment. This allows you to specify at which frame to end the processing.",
         type=int,
         required=True,
     )
 
     parser.add_argument(
+        "--aruco-marker-set",
+        help="The ArUco markers used in the video. This must match the specific set of ArUco markers used in the video for accurate detection and tracking. An example would be DICT_5X5_50, which is a set of 50 5x5 markers. More information can be found in the OpenCV documentation.",
+        type=str,
+        required=True,
+    )
+
+    parser.add_argument(
         "--half-rolling-window-size",
         help="Specifies the number of flanking frames (prior and subsequent) required in the rolling window for Hungarian matching a frame. The larger this window, the more frames will be used for matching. This can result in more robust tracks but in the event of an identity swap, it may take longer to correct the identity. The default is set to 5, resulting in an 11 frame window. You should change this depending on your intended use and your recording setup. ",
         type=int,
         default=5,
     )
 
     parser.add_argument(
@@ -77,21 +84,14 @@
     parser.add_argument(
         "--aruco-crop-size",
         help="The number of pixels horizontally and vertically around the ArUco SLEAP node to identify the marker. The cropping area should be large enough to include the whole marker for accurate detection, but not much larger, to keep the processing efficient and avoid capturing multiple tags. This is data set specific.",
         type=int,
     )
 
     parser.add_argument(
-        "--aruco-marker-set",
-        help="The ArUco markers used in the video. This must match the specific set of ArUco markers used in the video for accurate detection and tracking. An example would be DICT_5X5_50, which is a set of 50 5x5 markers. More information can be found in the OpenCV documentation.",
-        type=str,
-        required=True,
-    )
-
-    parser.add_argument(
         "--aruco-adaptive-thresh-win-size-min",
         dest="adaptiveThreshWinSizeMin",
         help="Specifies the value for adaptiveThreshWinSizeMin used in adaptive thresholding. This parameter affects the adaptive thresholding in the ArUco marker detection, which can impact the robustness of marker detection. The default value is 10, a commonly used value. More information can be found in the OpenCV documentation.",
         type=int,
         default=10,
     )
```

### Comparing `naps-track-1.0.5/naps/sleap_utils.py` & `naps-track-1.0.6/naps/sleap_utils.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.5/naps/utils/interactor.py` & `naps-track-1.0.6/naps/utils/interactor.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.5/naps/utils/tracking.py` & `naps-track-1.0.6/naps/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `naps-track-1.0.5/naps_track.egg-info/PKG-INFO` & `naps-track-1.0.6/naps_track.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naps-track
-Version: 1.0.5
+Version: 1.0.6
 Summary: NAPS (NAPS is ArUco Plus SLEAP)
 Home-page: https://github.com/kocherlab/naps
 License: MIT
 Project-URL: Documentation, https://naps.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/kocherlab/naps
 Project-URL: Issue tracker, https://github.com/kocherlab/naps/issues
 Description: |Stable version| |Latest version| |Documentation| |github ci| |Coverage| |conda| |Conda Upload| |PyPI Upload| |LICENSE|
```

### Comparing `naps-track-1.0.5/setup.py` & `naps-track-1.0.6/setup.py`

 * *Files identical despite different names*

