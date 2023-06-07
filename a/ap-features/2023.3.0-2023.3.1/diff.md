# Comparing `tmp/ap_features-2023.3.0.tar.gz` & `tmp/ap_features-2023.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ap_features-2023.3.0.tar", last modified: Wed Jun  7 07:49:18 2023, max compression
+gzip compressed data, was "ap_features-2023.3.1.tar", last modified: Wed Jun  7 07:49:21 2023, max compression
```

## Comparing `ap_features-2023.3.0.tar` & `ap_features-2023.3.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:18.641005 ap_features-2023.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-07 07:48:45.000000 ap_features-2023.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-07 07:48:45.000000 ap_features-2023.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-07 07:48:45.000000 ap_features-2023.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 07:48:45.000000 ap_features-2023.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-07 07:49:18.641005 ap_features-2023.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-07 07:48:45.000000 ap_features-2023.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:18.633005 ap_features-2023.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-07 07:48:45.000000 ap_features-2023.3.0/docs/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-06-07 07:48:45.000000 ap_features-2023.3.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-07 07:48:45.000000 ap_features-2023.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 07:49:18.641005 ap_features-2023.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:18.633005 ap_features-2023.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:18.637005 ap_features-2023.3.0/src/c/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/c/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/c/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/c/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:18.637005 ap_features-2023.3.0/src/c/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/c/cmake/BuildType.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/c/common.h
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/c/cost_terms.c
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/c/cost_terms.h
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/c/cost_terms_main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:18.633005 ap_features-2023.3.0/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:18.637005 ap_features-2023.3.0/src/python/ap_features/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/python/ap_features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/python/ap_features/_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/python/ap_features/average.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/python/ap_features/background.py
--rw-r--r--   0 runner    (1001) docker     (123)    37483 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/python/ap_features/beat.py
--rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/python/ap_features/chopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    28479 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/python/ap_features/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/python/ap_features/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/python/ap_features/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/python/ap_features/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-07 07:48:45.000000 ap_features-2023.3.0/src/python/ap_features/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:18.637005 ap_features-2023.3.0/src/python/ap_features.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-07 07:49:18.000000 ap_features-2023.3.0/src/python/ap_features.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-07 07:49:18.000000 ap_features-2023.3.0/src/python/ap_features.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:49:18.000000 ap_features-2023.3.0/src/python/ap_features.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-07 07:49:18.000000 ap_features-2023.3.0/src/python/ap_features.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 07:49:18.000000 ap_features-2023.3.0/src/python/ap_features.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:18.637005 ap_features-2023.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:18.633005 ap_features-2023.3.0/tests/baseline_images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:18.641005 ap_features-2023.3.0/tests/baseline_images/test_plot/
--rw-r--r--   0 runner    (1001) docker     (123)    61987 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/baseline_images/test_plot/beats.png
--rw-r--r--   0 runner    (1001) docker     (123)    79471 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/baseline_images/test_plot/beats_aligned.png
--rw-r--r--   0 runner    (1001) docker     (123)    47169 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/baseline_images/test_plot/poincare.png
--rw-r--r--   0 runner    (1001) docker     (123)    52868 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/baseline_images/test_plot/simple_beat.png
--rw-r--r--   0 runner    (1001) docker     (123)    61269 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/baseline_images/test_plot/simple_beat_with_background.png
--rw-r--r--   0 runner    (1001) docker     (123)    66463 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/baseline_images/test_plot/simple_beat_with_pacing.png
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/cost_terms.npy
--rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/data.npy
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/real_data.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/test_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/test_background.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/test_beat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/test_chopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-07 07:48:45.000000 ap_features-2023.3.0/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.358227 ap_features-2023.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-07 07:48:47.000000 ap_features-2023.3.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-07 07:48:47.000000 ap_features-2023.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-07 07:48:47.000000 ap_features-2023.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 07:48:47.000000 ap_features-2023.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-07 07:49:21.358227 ap_features-2023.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-07 07:48:47.000000 ap_features-2023.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.350227 ap_features-2023.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-07 07:48:47.000000 ap_features-2023.3.1/docs/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-06-07 07:48:47.000000 ap_features-2023.3.1/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-07 07:48:47.000000 ap_features-2023.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 07:49:21.358227 ap_features-2023.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.350227 ap_features-2023.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.354227 ap_features-2023.3.1/src/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.354227 ap_features-2023.3.1/src/c/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/cmake/BuildType.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/cost_terms.c
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/cost_terms.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/cost_terms_main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.350227 ap_features-2023.3.1/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.354227 ap_features-2023.3.1/src/python/ap_features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39251 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/beat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/chopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28479 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.354227 ap_features-2023.3.1/src/python/ap_features.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-07 07:49:21.000000 ap_features-2023.3.1/src/python/ap_features.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-07 07:49:21.000000 ap_features-2023.3.1/src/python/ap_features.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:49:21.000000 ap_features-2023.3.1/src/python/ap_features.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-07 07:49:21.000000 ap_features-2023.3.1/src/python/ap_features.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 07:49:21.000000 ap_features-2023.3.1/src/python/ap_features.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.354227 ap_features-2023.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.350227 ap_features-2023.3.1/tests/baseline_images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.358227 ap_features-2023.3.1/tests/baseline_images/test_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)    61987 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/beats.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79471 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/beats_aligned.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47169 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/poincare.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52868 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61269 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat_with_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66463 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat_with_pacing.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/cost_terms.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/data.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/real_data.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_beat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_chopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_plot.py
```

### Comparing `ap_features-2023.3.0/CONTRIBUTING.md` & `ap_features-2023.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/LICENSE` & `ap_features-2023.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/PKG-INFO` & `ap_features-2023.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ap_features
-Version: 2023.3.0
+Version: 2023.3.1
 Summary: Package to compute features of traces from action potential models
 Author-email: Henrik Finsberg <henriknf@simula.no>, "Kristian G. Hustad" <kghustad@simula.no>
 License: LGPL-2.1
 Project-URL: Homepage, https://computationalphysiology.github.io/ap_features
 Project-URL: Documentation, https://computationalphysiology.github.io/ap_features
 Project-URL: Source, https://github.com/ComputationalPhysiology/ap_features
 Project-URL: Tracker, https://github.com/ComputationalPhysiology/ap_features/issues
```

### Comparing `ap_features-2023.3.0/README.md` & `ap_features-2023.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/docs/INSTALL.md` & `ap_features-2023.3.1/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/docs/logo.png` & `ap_features-2023.3.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/pyproject.toml` & `ap_features-2023.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "oldest-supported-numpy; python_version>='3.5'",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "ap_features"
-version = "2023.3.0"
+version = "2023.3.1"
 description = "Package to compute features of traces from action potential models"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}, {name = "Kristian G. Hustad", email = "kghustad@simula.no" }]
 license = {text = "LGPL-2.1"}
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["action potential", "cell", "models", "features"]
 dependencies = [
```

### Comparing `ap_features-2023.3.0/src/c/.clang-format` & `ap_features-2023.3.1/src/c/.clang-format`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/c/CMakeLists.txt` & `ap_features-2023.3.1/src/c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/c/cmake/BuildType.cmake` & `ap_features-2023.3.1/src/c/cmake/BuildType.cmake`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/c/cost_terms.c` & `ap_features-2023.3.1/src/c/cost_terms.c`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/c/cost_terms_main.c` & `ap_features-2023.3.1/src/c/cost_terms_main.c`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/python/ap_features/__init__.py` & `ap_features-2023.3.1/src/python/ap_features/__init__.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/python/ap_features/_numba.py` & `ap_features-2023.3.1/src/python/ap_features/_numba.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/python/ap_features/average.py` & `ap_features-2023.3.1/src/python/ap_features/average.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/python/ap_features/background.py` & `ap_features-2023.3.1/src/python/ap_features/background.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/python/ap_features/beat.py` & `ap_features-2023.3.1/src/python/ap_features/beat.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,19 @@
         return f"{self.__class__.__name__}(t={self.t.shape}, y={self.y.shape})"
 
     @property
     def time_unit(self) -> str:
         """The time unit 'ms' or 's'"""
         return utils.time_unit(self.t)
 
+    @property
+    def duration(self) -> float:
+        """The duration of the trace, i.e last time point minus the first"""
+        return self.t[-1] - self.t[0]
+
     def ensure_time_unit(self, unit: str) -> None:
         """Convert time to milliseconds or seconds
 
         Parameters
         ----------
         unit : str
             A string with 'ms' or 's'
@@ -86,18 +91,20 @@
 
         if self.time_unit != unit:
             unitfactor = 1 / 1000.0 if unit == "s" else 1000.0
             self.t[:] *= unitfactor
 
     @property
     def t(self) -> np.ndarray:
+        """The time stamps"""
         return self._t
 
     @property
     def y(self) -> np.ndarray:
+        """The trace"""
         return self._y
 
     def max(self) -> float:
         """Return the maximum value of the trace"""
         return self.y.max()
 
     def min(self) -> float:
@@ -106,14 +113,16 @@
 
     def amp(self) -> float:
         """Return the difference between the maximum and minimum value"""
         return self.max() - self.min()
 
     @property
     def pacing(self) -> np.ndarray:
+        """Array of pacing amplitudes. If no pacing info is available,
+        then this will be an array of zeros with same length as the trace"""
         return self._pacing
 
     def __len__(self):
         return len(self.y)
 
     def __eq__(self, other) -> bool:
         try:
@@ -122,48 +131,87 @@
                 and (self.y == other.y).all()
                 and (self.pacing == other.pacing).all()
             )
         except Exception:
             return False
 
     def slice(self, start: float, end: float, copy: bool = True) -> "Trace":
+        """Create a slice of the original trace
+
+        Parameters
+        ----------
+        start : float
+            Start time of slice
+        end : float
+            End time of slice
+        copy : bool, optional
+            If true create a copy of the original array otherwise return a slice
+            of the original array, by default True
+
+        Returns
+        -------
+        Trace
+            A sliced trace
+        """
         f = copy_function(copy)
         start_index, end_index = chopping.find_start_end_index(self.t, start, end)
         return self.__class__(
             y=f(self.y)[start_index:end_index],
             t=f(self.t)[start_index:end_index],
             pacing=f(self.pacing)[start_index:end_index],
             backend=self._backend,
         )
 
     def copy(self):
+        """Create a copy of the trace"""
         return self.__class__(
             y=np.copy(self.y),
             t=np.copy(self.t),
             pacing=np.copy(self.pacing),
             backend=self._backend,
         )
 
     def plot(
         self,
         fname: str = "",
         include_pacing: bool = False,
         include_background: bool = False,
         ylabel: str = "",
     ):
+        """Plot the trace with matplotlib
+
+        Parameters
+        ----------
+        fname : str, optional
+            Name of the figure to be saved. If not provided the
+            figure will note be saved, but you can show by calling
+            `plt.show`
+        include_pacing : bool, optional
+            Whether to include pacing in the plot, by default False
+        include_background : bool, optional
+            Whether to include the background, by default False
+        ylabel : str, optional
+            Label on the y-axis, by default ""
+
+        Returns
+        -------
+        Tuple[plt.Figure, plt.Axes] | None
+            If matplotlib is installed it will return a tuple containing
+            the figure and the axes.
+        """
         return plot.plot_beat(
             self,
             include_pacing=include_pacing,
             include_background=include_background,
             ylabel=ylabel,
             fname=fname,
         )
 
     def as_spline(self, k: int = 3, s: Optional[int] = None) -> UnivariateSpline:
-        """[summary]
+        """Convert trace to spline
 
         Parameters
         ----------
         k : int, optional
             Degree of the smoothing spline.  Must be 1 <= `k` <= 5.
             Default is `k` = 3, a cubic spline, by default 3.
         s : float or None, optional
@@ -197,19 +245,21 @@
         )
         assert self._t.shape == self._y.shape, msg
         self._y_rest = y_rest
         self._parent = parent
         self._beat_number = beat_number
 
     @property
-    def y_normalized(self):
+    def y_normalized(self) -> np.ndarray:
+        """Return normalized signal"""
         return utils.normalize_signal(self.y, self.y_rest)
 
     @property
-    def y_rest(self):
+    def y_rest(self) -> Optional[float]:
+        """Return resting value if specified, otherwise None"""
         return self._y_rest
 
     def as_beats(self) -> "Beats":
         """Convert trace from Beat to Beats"""
         return Beats(y=self.y, t=self.y, pacing=self.pacing)
 
     def is_valid(self):
@@ -441,15 +491,15 @@
             If true normalize signal first, so that max value is 1.0,
             and min value is zero before performing the computation,
             by default False
 
         Returns
         -------
         float
-            [description]
+            Integral above the APD p line
         """
         return features.integrate_apd(
             t=self.t,
             y=self.y,
             factor=factor,
             use_spline=use_spline,
             normalize=normalize,
```

### Comparing `ap_features-2023.3.0/src/python/ap_features/chopping.py` & `ap_features-2023.3.1/src/python/ap_features/chopping.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/python/ap_features/features.py` & `ap_features-2023.3.1/src/python/ap_features/features.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/python/ap_features/filters.py` & `ap_features-2023.3.1/src/python/ap_features/filters.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/python/ap_features/plot.py` & `ap_features-2023.3.1/src/python/ap_features/plot.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/python/ap_features/testing.py` & `ap_features-2023.3.1/src/python/ap_features/testing.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/python/ap_features/utils.py` & `ap_features-2023.3.1/src/python/ap_features/utils.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/src/python/ap_features.egg-info/PKG-INFO` & `ap_features-2023.3.1/src/python/ap_features.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ap-features
-Version: 2023.3.0
+Version: 2023.3.1
 Summary: Package to compute features of traces from action potential models
 Author-email: Henrik Finsberg <henriknf@simula.no>, "Kristian G. Hustad" <kghustad@simula.no>
 License: LGPL-2.1
 Project-URL: Homepage, https://computationalphysiology.github.io/ap_features
 Project-URL: Documentation, https://computationalphysiology.github.io/ap_features
 Project-URL: Source, https://github.com/ComputationalPhysiology/ap_features
 Project-URL: Tracker, https://github.com/ComputationalPhysiology/ap_features/issues
```

### Comparing `ap_features-2023.3.0/src/python/ap_features.egg-info/SOURCES.txt` & `ap_features-2023.3.1/src/python/ap_features.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/baseline_images/test_plot/beats.png` & `ap_features-2023.3.1/tests/baseline_images/test_plot/beats.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/baseline_images/test_plot/beats_aligned.png` & `ap_features-2023.3.1/tests/baseline_images/test_plot/beats_aligned.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/baseline_images/test_plot/poincare.png` & `ap_features-2023.3.1/tests/baseline_images/test_plot/poincare.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/baseline_images/test_plot/simple_beat.png` & `ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/baseline_images/test_plot/simple_beat_with_background.png` & `ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat_with_background.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/baseline_images/test_plot/simple_beat_with_pacing.png` & `ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat_with_pacing.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/conftest.py` & `ap_features-2023.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/cost_terms.npy` & `ap_features-2023.3.1/tests/cost_terms.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/data.npy` & `ap_features-2023.3.1/tests/data.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/real_data.npy` & `ap_features-2023.3.1/tests/real_data.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/test_average.py` & `ap_features-2023.3.1/tests/test_average.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/test_background.py` & `ap_features-2023.3.1/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/test_beat.py` & `ap_features-2023.3.1/tests/test_beat.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/test_chopping.py` & `ap_features-2023.3.1/tests/test_chopping.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/test_features.py` & `ap_features-2023.3.1/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/test_filters.py` & `ap_features-2023.3.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.0/tests/test_plot.py` & `ap_features-2023.3.1/tests/test_plot.py`

 * *Files identical despite different names*

