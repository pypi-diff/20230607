# Comparing `tmp/pycm-3.9.tar.gz` & `tmp/pycm-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycm-3.9.tar", last modified: Mon May  1 17:09:00 2023, max compression
+gzip compressed data, was "pycm-4.0.tar", last modified: Wed Jun  7 14:06:54 2023, max compression
```

## Comparing `pycm-3.9.tar` & `pycm-4.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:09:00.290590 pycm-3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-01 17:08:48.000000 pycm-3.9/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-05-01 17:08:48.000000 pycm-3.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-01 17:08:48.000000 pycm-3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-01 17:08:48.000000 pycm-3.9/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:09:00.286590 pycm-3.9/Otherfiles/
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/PSF.png
--rw-r--r--   0 runner    (1001) docker     (123)    69490 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/block_diagram.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    52087 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/compare_block_diagram.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   116776 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/plot1.png
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/plot2.png
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/plot3.png
--rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/recommendation_block_diagram.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)    68164 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/test.html
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/test.pycm
--rw-r--r--   0 runner    (1001) docker     (123)    49262 2023-05-01 17:09:00.290590 pycm-3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27716 2023-05-01 17:08:48.000000 pycm-3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-01 17:08:48.000000 pycm-3.9/TODO.md
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-01 17:08:48.000000 pycm-3.9/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-01 17:08:48.000000 pycm-3.9/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:09:00.286590 pycm-3.9/paper/
--rw-r--r--   0 runner    (1001) docker     (123)   125670 2023-05-01 17:08:48.000000 pycm-3.9/paper/10.21105.joss.00729.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-01 17:08:48.000000 pycm-3.9/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-01 17:08:48.000000 pycm-3.9/paper/paper.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:09:00.290590 pycm-3.9/pycm/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-01 17:08:48.000000 pycm-3.9/pycm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-01 17:08:48.000000 pycm-3.9/pycm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    21695 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_class_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)    13314 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    30688 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_interpret.py
--rw-r--r--   0 runner    (1001) docker     (123)    39335 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_overall_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    32973 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_param.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21824 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:09:00.290590 pycm-3.9/pycm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49262 2023-05-01 17:09:00.000000 pycm-3.9/pycm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-01 17:09:00.000000 pycm-3.9/pycm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:09:00.000000 pycm-3.9/pycm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 17:09:00.000000 pycm-3.9/pycm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 17:09:00.000000 pycm-3.9/pycm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 17:08:48.000000 pycm-3.9/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 17:08:48.000000 pycm-3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 17:09:00.290590 pycm-3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-01 17:08:48.000000 pycm-3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:06:54.034150 pycm-4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-07 14:06:45.000000 pycm-4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20198 2023-06-07 14:06:45.000000 pycm-4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-07 14:06:45.000000 pycm-4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-07 14:06:45.000000 pycm-4.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:06:54.030150 pycm-4.0/Otherfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-06-07 14:06:45.000000 pycm-4.0/Otherfiles/PSF.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69490 2023-06-07 14:06:45.000000 pycm-4.0/Otherfiles/block_diagram.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    52087 2023-06-07 14:06:45.000000 pycm-4.0/Otherfiles/compare_block_diagram.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   116776 2023-06-07 14:06:45.000000 pycm-4.0/Otherfiles/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-06-07 14:06:45.000000 pycm-4.0/Otherfiles/plot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-07 14:06:45.000000 pycm-4.0/Otherfiles/plot2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-06-07 14:06:45.000000 pycm-4.0/Otherfiles/plot3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-06-07 14:06:45.000000 pycm-4.0/Otherfiles/recommendation_block_diagram.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-07 14:06:45.000000 pycm-4.0/Otherfiles/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    68164 2023-06-07 14:06:45.000000 pycm-4.0/Otherfiles/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-06-07 14:06:45.000000 pycm-4.0/Otherfiles/test.pycm
+-rw-r--r--   0 runner    (1001) docker     (123)    48993 2023-06-07 14:06:54.034150 pycm-4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26995 2023-06-07 14:06:45.000000 pycm-4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-07 14:06:45.000000 pycm-4.0/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-07 14:06:45.000000 pycm-4.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 14:06:45.000000 pycm-4.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:06:54.030150 pycm-4.0/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)   125670 2023-06-07 14:06:45.000000 pycm-4.0/paper/10.21105.joss.00729.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-06-07 14:06:45.000000 pycm-4.0/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-07 14:06:45.000000 pycm-4.0/paper/paper.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:06:54.030150 pycm-4.0/pycm/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-07 14:06:45.000000 pycm-4.0/pycm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-07 14:06:45.000000 pycm-4.0/pycm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21695 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_class_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13314 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30688 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_multilabel_cm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39335 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_overall_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22524 2023-06-07 14:06:45.000000 pycm-4.0/pycm/pycm_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:06:54.034150 pycm-4.0/pycm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48993 2023-06-07 14:06:53.000000 pycm-4.0/pycm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-07 14:06:54.000000 pycm-4.0/pycm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:06:53.000000 pycm-4.0/pycm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 14:06:53.000000 pycm-4.0/pycm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 14:06:53.000000 pycm-4.0/pycm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-07 14:06:45.000000 pycm-4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 14:06:45.000000 pycm-4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:06:54.034150 pycm-4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-07 14:06:45.000000 pycm-4.0/setup.py
```

### Comparing `pycm-3.9/AUTHORS.md` & `pycm-4.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pycm-3.9/CHANGELOG.md` & `pycm-4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [4.0] - 2023-06-07
+### Added
+- `pycmMultiLabelError` class
+- `MultiLabelCM` class
+- `get_cm_by_class` method
+- `get_cm_by_sample` method
+- `__mlcm_vector_handler__` function
+- `__mlcm_assign_classes__` function
+- `__mlcm_vectors_filter__` function
+- `__set_to_multihot__` function
+- `deprecated` function
+### Changed
+- Document modified
+- `README.md` modified
+- Example-4 modified
+- Test system modified
+- Python 3.5 support dropped
 ## [3.9] - 2023-05-01
 ### Added
 - `OVERALL_PARAMS` dictionary
 - `__imbalancement_handler__` function
 - `vector_serializer` function
 - NPV micro/macro
 - `log_loss` method
@@ -688,15 +705,16 @@
 - MK
 - NPV
 - PPV
 - TNR
 - TPR
 - documents and `README.md`
 
-[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v3.9...dev
+[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v4.0...dev
+[4.0]: https://github.com/sepandhaghighi/pycm/compare/v3.9...v4.0
 [3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9
 [3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8
 [3.7]: https://github.com/sepandhaghighi/pycm/compare/v3.6...v3.7
 [3.6]: https://github.com/sepandhaghighi/pycm/compare/v3.5...v3.6
 [3.5]: https://github.com/sepandhaghighi/pycm/compare/v3.4...v3.5
 [3.4]: https://github.com/sepandhaghighi/pycm/compare/v3.3...v3.4
 [3.3]: https://github.com/sepandhaghighi/pycm/compare/v3.2...v3.3
```

### Comparing `pycm-3.9/LICENSE` & `pycm-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycm-3.9/Otherfiles/PSF.png` & `pycm-4.0/Otherfiles/PSF.png`

 * *Files identical despite different names*

### Comparing `pycm-3.9/Otherfiles/block_diagram.jpg` & `pycm-4.0/Otherfiles/block_diagram.jpg`

 * *Files identical despite different names*

### Comparing `pycm-3.9/Otherfiles/compare_block_diagram.jpg` & `pycm-4.0/Otherfiles/compare_block_diagram.jpg`

 * *Files identical despite different names*

### Comparing `pycm-3.9/Otherfiles/logo.png` & `pycm-4.0/Otherfiles/logo.png`

 * *Files identical despite different names*

### Comparing `pycm-3.9/Otherfiles/plot1.png` & `pycm-4.0/Otherfiles/plot1.png`

 * *Files identical despite different names*

### Comparing `pycm-3.9/Otherfiles/plot2.png` & `pycm-4.0/Otherfiles/plot2.png`

 * *Files identical despite different names*

### Comparing `pycm-3.9/Otherfiles/plot3.png` & `pycm-4.0/Otherfiles/plot3.png`

 * *Files identical despite different names*

### Comparing `pycm-3.9/Otherfiles/recommendation_block_diagram.jpg` & `pycm-4.0/Otherfiles/recommendation_block_diagram.jpg`

 * *Files identical despite different names*

### Comparing `pycm-3.9/Otherfiles/test.csv` & `pycm-4.0/Otherfiles/test.csv`

 * *Files identical despite different names*

### Comparing `pycm-3.9/Otherfiles/test.html` & `pycm-4.0/Otherfiles/test.html`

 * *Files 0% similar despite different names*

```diff
@@ -783,10 +783,10 @@
 <td style="border:1px solid black;padding:4px;border-collapse: collapse;background-color:transparent;"><a href="http://www.pycm.io/doc/index.html#sInd-(Similarity-index)" style="text-decoration:None;">sInd</a></td>
 <td style="border:1px solid black;padding:4px;border-collapse: collapse;">0.71716</td>
 <td style="border:1px solid black;padding:4px;border-collapse: collapse;">0.61921</td>
 <td style="border:1px solid black;padding:4px;border-collapse: collapse;">0.58547</td>
 <td style="border:1px solid black;padding:4px;border-collapse: collapse;text-align:left;">Similarity index</td>
 </tr>
 </table>
-<p style="text-align:center;border-top:1px solid black;">Generated By <a href="http://www.pycm.io" style="text-decoration:none;color:red;">PyCM</a> Version 3.9</p>
+<p style="text-align:center;border-top:1px solid black;">Generated By <a href="http://www.pycm.io" style="text-decoration:none;color:red;">PyCM</a> Version 4.0</p>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -160,8 +160,8 @@
 TOP   3         3          6          Test outcome positive
 TP    3         1          3          True positive/hit
 TPR   0.6       0.5        0.6        Sensitivity, recall, hit rate, or true
                                       positive rate
 Y     0.6       0.3        0.17143    Youden index
 dInd  0.4       0.53852    0.58624    Distance index
 sInd  0.71716   0.61921    0.58547    Similarity index
-Generated By PyCM Version 3.9
+Generated By PyCM Version 4.0
```

### Comparing `pycm-3.9/Otherfiles/test.pycm` & `pycm-4.0/Otherfiles/test.pycm`

 * *Files identical despite different names*

### Comparing `pycm-3.9/PKG-INFO` & `pycm-4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: pycm
-Version: 3.9
+Version: 4.0
 Summary: Multi-class confusion matrix library in Python
 Home-page: https://github.com/sepandhaghighi/pycm
-Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.9
+Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v4.0
 Author: PyCM Development Team
 Author-email: info@pycm.io
 License: MIT
 Project-URL: Webpage, https://www.pycm.io
 Project-URL: Source, https://github.com/sepandhaghighi/pycm
 Project-URL: Discord, https://discord.com/invite/zqpU2b3J3f
 Keywords: confusion-matrix python3 python machine_learning ML
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
@@ -31,15 +30,15 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 
 <div align="center">
 <img src="https://github.com/sepandhaghighi/pycm/raw/master/Otherfiles/logo.png" width="550">
@@ -128,42 +127,44 @@
 		<td align="center"><a href="https://www.codefactor.io/repository/github/sepandhaghighi/pycm/overview/dev"><img src="https://www.codefactor.io/repository/github/sepandhaghighi/pycm/badge/dev" alt="CodeFactor" /></a></td>
 		<td align="center"><a href="https://codebeat.co/projects/github-com-sepandhaghighi-pycm-dev"><img alt="codebeat badge" src="https://codebeat.co/badges/f6642af1-c343-48c2-bd3e-eee802facf39" /></a></td>
 	</tr>
 </table>
 
 ## Installation
 
+⚠️  PyCM 3.9 is the last version to support **Python 3.5**
+
 ⚠️  PyCM 2.4 is the last version to support **Python 2.7** & **Python 3.4**
 
 ⚠️  Plotting capability requires **Matplotlib (>= 3.0.0)** or **Seaborn (>= 0.9.1)**
 
 ### Source code
-- Download [Version 3.9](https://github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
+- Download [Version 4.0](https://github.com/sepandhaghighi/pycm/archive/v4.0.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
 - Run `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
 - Run `python3 setup.py install` or `python setup.py install` (Need root access)
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need root access)
+- Run `pip install pycm==4.0` or `pip3 install pycm==4.0` (Need root access)
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io/)
 - Update Conda using `conda update conda` (Need root access)
 - Run `conda install -c sepandhaghighi pycm` (Need root access)
 
 ### Easy install
 
 - Run `easy_install --upgrade pycm` (Need root access)
 
 ### MATLAB
 
 - Download and install [MATLAB](https://www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit)
-- Download and install [Python3.x](https://www.python.org/downloads/) (>=3.5, 64/32 bit)
+- Download and install [Python3.x](https://www.python.org/downloads/) (>=3.6, 64/32 bit)
 	- [x] Select `Add to PATH` option
 	- [x] Select `Install pip` option
 - Run `pip install pycm` or `pip3 install pycm` (Need root access)
 - Configure Python interpreter
 
 ```matlab
 >> pyversion PYTHON_EXECUTABLE_FULL_PATH
@@ -474,77 +475,57 @@
 pycm.ConfusionMatrix(classes: [0, 1, 2])
 >>> cp.sorted
 ['cm2', 'cm3']
 >>> cp.best_name
 'cm2'
 ```
 
+### Multilabel confusion matrix
+
+From `version 4.0`, `MultiLabelCM` has been added to calculate class-wise or sample-wise multilabel confusion matrices. In class-wise mode, confusion matrices are calculated for each class, and in sample-wise mode, they are generated per sample. All generated confusion matrices are binarized with a one-vs-rest transformation.
+
+```pycon
+>>> mlcm = MultiLabelCM(actual_vector=[{"cat", "bird"}, {"dog"}], predict_vector=[{"cat"}, {"dog", "bird"}], classes=["cat", "dog", "bird"])
+>>> mlcm.actual_vector_multihot
+[[1, 0, 1], [0, 1, 0]]
+>>> mlcm.predict_vector_multihot
+[[1, 0, 0], [0, 1, 1]]
+>>> mlcm.get_cm_by_class("cat").print_matrix()
+Predict 0       1       
+Actual
+0       1       0       
+
+1       0       1       
+
+>>> mlcm.get_cm_by_sample(0).print_matrix()
+Predict 0       1       
+Actual
+0       1       0       
+
+1       1       1 
+
+```
+
 ### Online help
 
 `online_help` function is added in `version 1.1` in order to open each statistics definition in web browser
 
 ```pycon
 >>> from pycm import online_help
 >>> online_help("J")
 >>> online_help("SOA1(Landis & Koch)")
 >>> online_help(2)
 ```
 
 * List of items are available by calling `online_help()` (without argument)
 * If PyCM website is not available, set `alt_link = True` (new in `version 2.4`)
 
-### Acceptable data types
-
-**ConfusionMatrix**
-
-1. `actual_vector` : python `list` or numpy `array` of any stringable objects
-2. `predict_vector` : python `list` or numpy `array` of any stringable objects
-3. `matrix` : `dict`
-4. `digit`: `int`
-5. `threshold` : `FunctionType (function or lambda)`
-6. `file` : `File object`
-7. `sample_weight` : python `list` or numpy `array` of numbers
-8. `transpose` : `bool`
-9. `classes` : python `list`
-10. `is_imbalanced` : `bool`
-11. `metrics_off` : `bool`
-
-* Run `help(ConfusionMatrix)` for `ConfusionMatrix` object details
-
-**Compare**
-
-1. `cm_dict` : python `dict` of `ConfusionMatrix` object (`str` : `ConfusionMatrix`)
-2. `by_class` : `bool`
-3. `class_weight` : python `dict` of class weights (`class_name` : `float`)
-4. `class_benchmark_weight`: python `dict` of class benchmark weights (`class_benchmark_name` : `float`)
-5. `overall_benchmark_weight`: python `dict` of overall benchmark weights (`overall_benchmark_name` : `float`)
-6. `digit`: `int`
-
-* Run `help(Compare)` for `Compare` object details
-
-**ROCCurve**
-
-1. `actual_vector` : python `list` or numpy `array` of any stringable objects
-2. `probs` : python `list` or numpy `array`
-3. `classes` : python `list`
-4. `thresholds`: python `list` or numpy `array`
-5. `sample_weight`: python `list` or numpy `array`
-
-**PRCurve**
-
-1. `actual_vector` : python `list` or numpy `array` of any stringable objects
-2. `probs` : python `list` or numpy `array`
-3. `classes` : python `list`
-4. `thresholds`: python `list` or numpy `array`
-5. `sample_weight`: python `list` or numpy `array`
-
-For more information visit [here](https://github.com/sepandhaghighi/pycm/tree/master/Document "Document")
+### Screen record
 
 <div align="center">
-
 <a href="https://asciinema.org/a/171863" target="_blank"><img src="https://asciinema.org/a/171863.png"/></a>
 </div>
 
 ## Try PyCM in your browser!
 
 PyCM can be used online in interactive Jupyter Notebooks via the Binder or Colab services! Try it out now! :
 
@@ -630,14 +611,31 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [4.0] - 2023-06-07
+### Added
+- `pycmMultiLabelError` class
+- `MultiLabelCM` class
+- `get_cm_by_class` method
+- `get_cm_by_sample` method
+- `__mlcm_vector_handler__` function
+- `__mlcm_assign_classes__` function
+- `__mlcm_vectors_filter__` function
+- `__set_to_multihot__` function
+- `deprecated` function
+### Changed
+- Document modified
+- `README.md` modified
+- Example-4 modified
+- Test system modified
+- Python 3.5 support dropped
 ## [3.9] - 2023-05-01
 ### Added
 - `OVERALL_PARAMS` dictionary
 - `__imbalancement_handler__` function
 - `vector_serializer` function
 - NPV micro/macro
 - `log_loss` method
@@ -1317,15 +1315,16 @@
 - MK
 - NPV
 - PPV
 - TNR
 - TPR
 - documents and `README.md`
 
-[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v3.9...dev
+[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v4.0...dev
+[4.0]: https://github.com/sepandhaghighi/pycm/compare/v3.9...v4.0
 [3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9
 [3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8
 [3.7]: https://github.com/sepandhaghighi/pycm/compare/v3.6...v3.7
 [3.6]: https://github.com/sepandhaghighi/pycm/compare/v3.5...v3.6
 [3.5]: https://github.com/sepandhaghighi/pycm/compare/v3.4...v3.5
 [3.4]: https://github.com/sepandhaghighi/pycm/compare/v3.3...v3.4
 [3.3]: https://github.com/sepandhaghighi/pycm/compare/v3.2...v3.3
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: pycm Version: 3.9 Summary: Multi-class confusion
+Metadata-Version: 2.1 Name: pycm Version: 4.0 Summary: Multi-class confusion
 matrix library in Python Home-page: https://github.com/sepandhaghighi/pycm
-Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.9 Author: PyCM
+Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v4.0 Author: PyCM
 Development Team Author-email: info@pycm.io License: MIT Project-URL: Webpage,
 https://www.pycm.io Project-URL: Source, https://github.com/sepandhaghighi/pycm
 Project-URL: Discord, https://discord.com/invite/zqpU2b3J3f Keywords:
 confusion-matrix python3 python machine_learning ML Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: End Users/Desktop Classifier: Intended Audience :: Manufacturing
-Classifier: Intended Audience :: Science/Research Classifier: Topic ::
-Scientific/Engineering :: Information Analysis Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
-Engineering :: Human Machine Interfaces Classifier: Topic :: Scientific/
-Engineering :: Mathematics Classifier: Topic :: Scientific/Engineering ::
-Physics Requires-Python: >=3.5 Description-Content-Type: text/markdown License-
-File: LICENSE License-File: AUTHORS.md
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
+Audience :: Manufacturing Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Information Analysis Classifier:
+Topic :: Education Classifier: Topic :: Scientific/Engineering Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+Scientific/Engineering :: Human Machine Interfaces Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
+Engineering :: Physics Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE License-File: AUTHORS.md
     [https://github.com/sepandhaghighi/pycm/raw/master/Otherfiles/logo.png]
                   ****** PyCM: Python Confusion Matrix ******
 
   [built_with_Python3] [https://img.shields.io/badge/doc-latest-orange.svg]
 [https://codecov.io/gh/sepandhaghighi/pycm/branch/master/graph/badge.svg] [PyPI
     version] [https://anaconda.org/sepandhaghighi/pycm/badges/version.svg]
                          [Document] [Discord_Channel]
@@ -62,30 +61,31 @@
 Branch                      master                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI          pycm/workflows/CI/                  pycm/workflows/CI/
             badge.svg?branch=master]              badge.svg?branch=dev]
              [https://api.codacy.com/project/
 Code Quality           badge/Grade/            [CodeFactor] [codebeat_badge]
              5d9463998a0040d09afc2b80c389365c]
-## Installation â ï¸ PyCM 2.4 is the last version to support **Python 2.7** &
-**Python 3.4** â ï¸ Plotting capability requires **Matplotlib (>= 3.0.0)** or
-**Seaborn (>= 0.9.1)** ### Source code - Download [Version 3.9](https://
-github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://
-github.com/sepandhaghighi/pycm/archive/dev.zip) - Run `pip install -
-r requirements.txt` or `pip3 install -r requirements.txt` (Need root access) -
-Run `python3 setup.py install` or `python setup.py install` (Need root access)
-### PyPI - Check [Python Packaging User Guide](https://packaging.python.org/
-installing/) - Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need
-root access) ### Conda - Check [Conda Managing Package](https://conda.io/) -
-Update Conda using `conda update conda` (Need root access) - Run `conda install
--c sepandhaghighi pycm` (Need root access) ### Easy install - Run `easy_install
---upgrade pycm` (Need root access) ### MATLAB - Download and install [MATLAB]
-(https://www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit) - Download
-and install [Python3.x](https://www.python.org/downloads/) (>=3.5, 64/32 bit) -
-[x] Select `Add to PATH` option - [x] Select `Install pip` option - Run `pip
+## Installation â ï¸ PyCM 3.9 is the last version to support **Python 3.5**
+â ï¸ PyCM 2.4 is the last version to support **Python 2.7** & **Python 3.4**
+â ï¸ Plotting capability requires **Matplotlib (>= 3.0.0)** or **Seaborn (>=
+0.9.1)** ### Source code - Download [Version 4.0](https://github.com/
+sepandhaghighi/pycm/archive/v4.0.zip) or [Latest Source ](https://github.com/
+sepandhaghighi/pycm/archive/dev.zip) - Run `pip install -r requirements.txt` or
+`pip3 install -r requirements.txt` (Need root access) - Run `python3 setup.py
+install` or `python setup.py install` (Need root access) ### PyPI - Check
+[Python Packaging User Guide](https://packaging.python.org/installing/) - Run
+`pip install pycm==4.0` or `pip3 install pycm==4.0` (Need root access) ###
+Conda - Check [Conda Managing Package](https://conda.io/) - Update Conda using
+`conda update conda` (Need root access) - Run `conda install -c sepandhaghighi
+pycm` (Need root access) ### Easy install - Run `easy_install --upgrade pycm`
+(Need root access) ### MATLAB - Download and install [MATLAB](https://
+www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit) - Download and
+install [Python3.x](https://www.python.org/downloads/) (>=3.6, 64/32 bit) - [x]
+Select `Add to PATH` option - [x] Select `Install pip` option - Run `pip
 install pycm` or `pip3 install pycm` (Need root access) - Configure Python
 interpreter ```matlab >> pyversion PYTHON_EXECUTABLE_FULL_PATH ``` - Visit
 [MATLAB Examples](https://github.com/sepandhaghighi/pycm/tree/master/MATLAB) ##
 Usage ### From vector ```pycon >>> from pycm import * >>> y_actu = [2, 0, 2, 2,
 0, 1, 1, 2, 2, 0, 1, 2] >>> y_pred = [0, 0, 2, 1, 0, 2, 1, 0, 2, 0, 2, 2] >>>
 cm = ConfusionMatrix(actual_vector=y_actu, predict_vector=y_pred) >>>
 cm.classes [0, 1, 2] >>> cm.table {0: {0: 3, 1: 0, 2: 0}, 1: {0: 0, 1: 1, 2:
@@ -230,42 +230,31 @@
 any other case, the compared object doesnât select the best confusion matrix.
 ```pycon >>> cm2 = ConfusionMatrix(matrix={0: {0: 2, 1: 50, 2: 6}, 1: {0: 5, 1:
 50, 2: 3}, 2: {0: 1, 1: 7, 2: 50}}) >>> cm3 = ConfusionMatrix(matrix={0: {0:
 50, 1: 2, 2: 6}, 1: {0: 50, 1: 5, 2: 3}, 2: {0: 1, 1: 55, 2: 2}}) >>> cp =
 Compare({"cm2": cm2, "cm3": cm3}) >>> print(cp) Best : cm2 Rank Name Class-
 Score Overall-Score 1 cm2 0.50278 0.58095 2 cm3 0.33611 0.52857 >>> cp.best
 pycm.ConfusionMatrix(classes: [0, 1, 2]) >>> cp.sorted ['cm2', 'cm3'] >>>
-cp.best_name 'cm2' ``` ### Online help `online_help` function is added in
-`version 1.1` in order to open each statistics definition in web browser
-```pycon >>> from pycm import online_help >>> online_help("J") >>> online_help
-("SOA1(Landis & Koch)") >>> online_help(2) ``` * List of items are available by
-calling `online_help()` (without argument) * If PyCM website is not available,
-set `alt_link = True` (new in `version 2.4`) ### Acceptable data types
-**ConfusionMatrix** 1. `actual_vector` : python `list` or numpy `array` of any
-stringable objects 2. `predict_vector` : python `list` or numpy `array` of any
-stringable objects 3. `matrix` : `dict` 4. `digit`: `int` 5. `threshold` :
-`FunctionType (function or lambda)` 6. `file` : `File object` 7.
-`sample_weight` : python `list` or numpy `array` of numbers 8. `transpose` :
-`bool` 9. `classes` : python `list` 10. `is_imbalanced` : `bool` 11.
-`metrics_off` : `bool` * Run `help(ConfusionMatrix)` for `ConfusionMatrix`
-object details **Compare** 1. `cm_dict` : python `dict` of `ConfusionMatrix`
-object (`str` : `ConfusionMatrix`) 2. `by_class` : `bool` 3. `class_weight` :
-python `dict` of class weights (`class_name` : `float`) 4.
-`class_benchmark_weight`: python `dict` of class benchmark weights
-(`class_benchmark_name` : `float`) 5. `overall_benchmark_weight`: python `dict`
-of overall benchmark weights (`overall_benchmark_name` : `float`) 6. `digit`:
-`int` * Run `help(Compare)` for `Compare` object details **ROCCurve** 1.
-`actual_vector` : python `list` or numpy `array` of any stringable objects 2.
-`probs` : python `list` or numpy `array` 3. `classes` : python `list` 4.
-`thresholds`: python `list` or numpy `array` 5. `sample_weight`: python `list`
-or numpy `array` **PRCurve** 1. `actual_vector` : python `list` or numpy
-`array` of any stringable objects 2. `probs` : python `list` or numpy `array`
-3. `classes` : python `list` 4. `thresholds`: python `list` or numpy `array` 5.
-`sample_weight`: python `list` or numpy `array` For more information visit
-[here](https://github.com/sepandhaghighi/pycm/tree/master/Document "Document")
+cp.best_name 'cm2' ``` ### Multilabel confusion matrix From `version 4.0`,
+`MultiLabelCM` has been added to calculate class-wise or sample-wise multilabel
+confusion matrices. In class-wise mode, confusion matrices are calculated for
+each class, and in sample-wise mode, they are generated per sample. All
+generated confusion matrices are binarized with a one-vs-rest transformation.
+```pycon >>> mlcm = MultiLabelCM(actual_vector=[{"cat", "bird"}, {"dog"}],
+predict_vector=[{"cat"}, {"dog", "bird"}], classes=["cat", "dog", "bird"]) >>>
+mlcm.actual_vector_multihot [[1, 0, 1], [0, 1, 0]] >>>
+mlcm.predict_vector_multihot [[1, 0, 0], [0, 1, 1]] >>> mlcm.get_cm_by_class
+("cat").print_matrix() Predict 0 1 Actual 0 1 0 1 0 1 >>> mlcm.get_cm_by_sample
+(0).print_matrix() Predict 0 1 Actual 0 1 0 1 1 1 ``` ### Online help
+`online_help` function is added in `version 1.1` in order to open each
+statistics definition in web browser ```pycon >>> from pycm import online_help
+>>> online_help("J") >>> online_help("SOA1(Landis & Koch)") >>> online_help(2)
+``` * List of items are available by calling `online_help()` (without argument)
+* If PyCM website is not available, set `alt_link = True` (new in `version
+2.4`) ### Screen record
                      [https://asciinema.org/a/171863.png]
 ## Try PyCM in your browser! PyCM can be used online in interactive Jupyter
 Notebooks via the Binder or Colab services! Try it out now! : [![Binder](https:
 //mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sepandhaghighi/pycm/
 master) [![Google Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/sepandhaghighi/pycm/blob/
 master) * Check `Examples` in `Document` folder ## Issues & bug reports 1. Fill
@@ -313,37 +302,42 @@
 ## Show your support ### Star this repo Give a â­ï¸ if this project helped
 you! ### Donate to our project If you do like our project and we hope that you
 do, can you please support us? Our project is not and is never going to be
 working for profit. We need the money just so we can continue doing what we do
 ;-) . [PyCM_Donation] # Changelog All notable changes to this project will be
 documented in this file. The format is based on [Keep a Changelog](http://
 keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning]
-(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ## [3.9] - 2023-05-01 ###
-Added - `OVERALL_PARAMS` dictionary - `__imbalancement_handler__` function -
-`vector_serializer` function - NPV micro/macro - `log_loss` method - 23 new
-distance/similarity 1. Dennis 2. Digby 3. Dispersion 4. Doolittle 5. Eyraud 6.
-Fager & McGowan 7. Faith 8. Fleiss-Levin-Paik 9. Forbes I 10. Forbes II 11.
-Fossum 12. Gilbert & Wells 13. Goodall 14. Goodman & Kruskal's Lambda 15.
-Goodman & Kruskal Lambda-r 16. Guttman's Lambda A 17. Guttman's Lambda B 18.
-Hamann 19. Harris & Lahey 20. Hawkins & Dotson 21. Kendall's Tau 22. Kent &
-Foster I 23. Kent & Foster II ### Changed - `metrics_off` parameter added to
-ConfusionMatrix `__init__` method - `CLASS_PARAMS` changed to a dictionary -
-Code style modified - `sort` parameter added to `relabel` method - Document
-modified - `CONTRIBUTING.md` updated - `codecov` removed from `dev-
-requirements.txt` - Test system modified ## [3.8] - 2023-02-01 ### Added -
-`distance` method - `__contains__` method - `__getitem__` method - Goodman-
-Kruskal's Lambda A benchmark - Goodman-Kruskal's Lambda B benchmark -
-Krippendorff's Alpha benchmark - Pearson's C benchmark - 30 new distance/
-similarity 1. AMPLE 2. Anderberg's D 3. Andres & Marzo's Delta 4. Baroni-Urbani
-& Buser I 5. Baroni-Urbani & Buser II 6. Batagelj & Bren 7. Baulieu I 8.
-Baulieu II 9. Baulieu III 10. Baulieu IV 11. Baulieu V 12. Baulieu VI 13.
-Baulieu VII 14. Baulieu VIII 15. Baulieu IX 16. Baulieu X 17. Baulieu XI 18.
-Baulieu XII 19. Baulieu XIII 20. Baulieu XIV 21. Baulieu XV 22. Benini I 23.
-Benini II 24. Canberra 25. Clement 26. Consonni & Todeschini I 27. Consonni &
-Todeschini II 28. Consonni & Todeschini III 29. Consonni & Todeschini IV 30.
+(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ## [4.0] - 2023-06-07 ###
+Added - `pycmMultiLabelError` class - `MultiLabelCM` class - `get_cm_by_class`
+method - `get_cm_by_sample` method - `__mlcm_vector_handler__` function -
+`__mlcm_assign_classes__` function - `__mlcm_vectors_filter__` function -
+`__set_to_multihot__` function - `deprecated` function ### Changed - Document
+modified - `README.md` modified - Example-4 modified - Test system modified -
+Python 3.5 support dropped ## [3.9] - 2023-05-01 ### Added - `OVERALL_PARAMS`
+dictionary - `__imbalancement_handler__` function - `vector_serializer`
+function - NPV micro/macro - `log_loss` method - 23 new distance/similarity 1.
+Dennis 2. Digby 3. Dispersion 4. Doolittle 5. Eyraud 6. Fager & McGowan 7.
+Faith 8. Fleiss-Levin-Paik 9. Forbes I 10. Forbes II 11. Fossum 12. Gilbert &
+Wells 13. Goodall 14. Goodman & Kruskal's Lambda 15. Goodman & Kruskal Lambda-
+r 16. Guttman's Lambda A 17. Guttman's Lambda B 18. Hamann 19. Harris & Lahey
+20. Hawkins & Dotson 21. Kendall's Tau 22. Kent & Foster I 23. Kent & Foster II
+### Changed - `metrics_off` parameter added to ConfusionMatrix `__init__`
+method - `CLASS_PARAMS` changed to a dictionary - Code style modified - `sort`
+parameter added to `relabel` method - Document modified - `CONTRIBUTING.md`
+updated - `codecov` removed from `dev-requirements.txt` - Test system modified
+## [3.8] - 2023-02-01 ### Added - `distance` method - `__contains__` method -
+`__getitem__` method - Goodman-Kruskal's Lambda A benchmark - Goodman-Kruskal's
+Lambda B benchmark - Krippendorff's Alpha benchmark - Pearson's C benchmark -
+30 new distance/similarity 1. AMPLE 2. Anderberg's D 3. Andres & Marzo's Delta
+4. Baroni-Urbani & Buser I 5. Baroni-Urbani & Buser II 6. Batagelj & Bren 7.
+Baulieu I 8. Baulieu II 9. Baulieu III 10. Baulieu IV 11. Baulieu V 12. Baulieu
+VI 13. Baulieu VII 14. Baulieu VIII 15. Baulieu IX 16. Baulieu X 17. Baulieu XI
+18. Baulieu XII 19. Baulieu XIII 20. Baulieu XIV 21. Baulieu XV 22. Benini I
+23. Benini II 24. Canberra 25. Clement 26. Consonni & Todeschini I 27. Consonni
+& Todeschini II 28. Consonni & Todeschini III 29. Consonni & Todeschini IV 30.
 Consonni & Todeschini V ### Changed - `relabel` method sort bug fixed -
 `README.md` modified - `Compare` overall benchmarks default weights updated -
 Document modified - Test system modified ## [3.7] - 2022-12-15 ### Added -
 `Curve` class - `ROCCurve` class - `PRCurve` class - `pycmCurveError` class ###
 Changed - `CONTRIBUTING.md` updated - `matrix_params_calc` function optimized -
 `README.md` modified - Document modified - Test system modified - `Python 3.11`
 added to `test.yml` ## [3.6] - 2022-08-17 ### Added - Hamming distance - Braun-
@@ -532,17 +526,18 @@
 benchmark - `overall_stat` ## [0.2] - 2018-01-24 ### Added - Population -
 Condition positive - Condition negative - Test outcome positive - Test outcome
 negative - Prevalence - G-measure - Matrix method - Normalized matrix method -
 Params method ### Changed - `statistic_result` to `class_stat` - `params` to
 `stat` ## [0.1] - 2018-01-22 ### Added - ACC - BM - DOR - F1-Score - FDR - FNR
 - FOR - FPR - LR+ - LR- - MCC - MK - NPV - PPV - TNR - TPR - documents and
 `README.md` [Unreleased]: https://github.com/sepandhaghighi/pycm/compare/
-v3.9...dev [3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9
-[3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8 [3.7]: https:
-//github.com/sepandhaghighi/pycm/compare/v3.6...v3.7 [3.6]: https://github.com/
+v4.0...dev [4.0]: https://github.com/sepandhaghighi/pycm/compare/v3.9...v4.0
+[3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9 [3.8]: https:
+//github.com/sepandhaghighi/pycm/compare/v3.7...v3.8 [3.7]: https://github.com/
+sepandhaghighi/pycm/compare/v3.6...v3.7 [3.6]: https://github.com/
 sepandhaghighi/pycm/compare/v3.5...v3.6 [3.5]: https://github.com/
 sepandhaghighi/pycm/compare/v3.4...v3.5 [3.4]: https://github.com/
 sepandhaghighi/pycm/compare/v3.3...v3.4 [3.3]: https://github.com/
 sepandhaghighi/pycm/compare/v3.2...v3.3 [3.2]: https://github.com/
 sepandhaghighi/pycm/compare/v3.1...v3.2 [3.1]: https://github.com/
 sepandhaghighi/pycm/compare/v3.0...v3.1 [3.0]: https://github.com/
 sepandhaghighi/pycm/compare/v2.9...v3.0 [2.9]: https://github.com/
```

### Comparing `pycm-3.9/README.md` & `pycm-4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -85,42 +85,44 @@
 		<td align="center"><a href="https://www.codefactor.io/repository/github/sepandhaghighi/pycm/overview/dev"><img src="https://www.codefactor.io/repository/github/sepandhaghighi/pycm/badge/dev" alt="CodeFactor" /></a></td>
 		<td align="center"><a href="https://codebeat.co/projects/github-com-sepandhaghighi-pycm-dev"><img alt="codebeat badge" src="https://codebeat.co/badges/f6642af1-c343-48c2-bd3e-eee802facf39" /></a></td>
 	</tr>
 </table>
 
 ## Installation
 
+⚠️  PyCM 3.9 is the last version to support **Python 3.5**
+
 ⚠️  PyCM 2.4 is the last version to support **Python 2.7** & **Python 3.4**
 
 ⚠️  Plotting capability requires **Matplotlib (>= 3.0.0)** or **Seaborn (>= 0.9.1)**
 
 ### Source code
-- Download [Version 3.9](https://github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
+- Download [Version 4.0](https://github.com/sepandhaghighi/pycm/archive/v4.0.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
 - Run `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
 - Run `python3 setup.py install` or `python setup.py install` (Need root access)
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need root access)
+- Run `pip install pycm==4.0` or `pip3 install pycm==4.0` (Need root access)
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io/)
 - Update Conda using `conda update conda` (Need root access)
 - Run `conda install -c sepandhaghighi pycm` (Need root access)
 
 ### Easy install
 
 - Run `easy_install --upgrade pycm` (Need root access)
 
 ### MATLAB
 
 - Download and install [MATLAB](https://www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit)
-- Download and install [Python3.x](https://www.python.org/downloads/) (>=3.5, 64/32 bit)
+- Download and install [Python3.x](https://www.python.org/downloads/) (>=3.6, 64/32 bit)
 	- [x] Select `Add to PATH` option
 	- [x] Select `Install pip` option
 - Run `pip install pycm` or `pip3 install pycm` (Need root access)
 - Configure Python interpreter
 
 ```matlab
 >> pyversion PYTHON_EXECUTABLE_FULL_PATH
@@ -431,77 +433,57 @@
 pycm.ConfusionMatrix(classes: [0, 1, 2])
 >>> cp.sorted
 ['cm2', 'cm3']
 >>> cp.best_name
 'cm2'
 ```
 
+### Multilabel confusion matrix
+
+From `version 4.0`, `MultiLabelCM` has been added to calculate class-wise or sample-wise multilabel confusion matrices. In class-wise mode, confusion matrices are calculated for each class, and in sample-wise mode, they are generated per sample. All generated confusion matrices are binarized with a one-vs-rest transformation.
+
+```pycon
+>>> mlcm = MultiLabelCM(actual_vector=[{"cat", "bird"}, {"dog"}], predict_vector=[{"cat"}, {"dog", "bird"}], classes=["cat", "dog", "bird"])
+>>> mlcm.actual_vector_multihot
+[[1, 0, 1], [0, 1, 0]]
+>>> mlcm.predict_vector_multihot
+[[1, 0, 0], [0, 1, 1]]
+>>> mlcm.get_cm_by_class("cat").print_matrix()
+Predict 0       1       
+Actual
+0       1       0       
+
+1       0       1       
+
+>>> mlcm.get_cm_by_sample(0).print_matrix()
+Predict 0       1       
+Actual
+0       1       0       
+
+1       1       1 
+
+```
+
 ### Online help
 
 `online_help` function is added in `version 1.1` in order to open each statistics definition in web browser
 
 ```pycon
 >>> from pycm import online_help
 >>> online_help("J")
 >>> online_help("SOA1(Landis & Koch)")
 >>> online_help(2)
 ```
 
 * List of items are available by calling `online_help()` (without argument)
 * If PyCM website is not available, set `alt_link = True` (new in `version 2.4`)
 
-### Acceptable data types
-
-**ConfusionMatrix**
-
-1. `actual_vector` : python `list` or numpy `array` of any stringable objects
-2. `predict_vector` : python `list` or numpy `array` of any stringable objects
-3. `matrix` : `dict`
-4. `digit`: `int`
-5. `threshold` : `FunctionType (function or lambda)`
-6. `file` : `File object`
-7. `sample_weight` : python `list` or numpy `array` of numbers
-8. `transpose` : `bool`
-9. `classes` : python `list`
-10. `is_imbalanced` : `bool`
-11. `metrics_off` : `bool`
-
-* Run `help(ConfusionMatrix)` for `ConfusionMatrix` object details
-
-**Compare**
-
-1. `cm_dict` : python `dict` of `ConfusionMatrix` object (`str` : `ConfusionMatrix`)
-2. `by_class` : `bool`
-3. `class_weight` : python `dict` of class weights (`class_name` : `float`)
-4. `class_benchmark_weight`: python `dict` of class benchmark weights (`class_benchmark_name` : `float`)
-5. `overall_benchmark_weight`: python `dict` of overall benchmark weights (`overall_benchmark_name` : `float`)
-6. `digit`: `int`
-
-* Run `help(Compare)` for `Compare` object details
-
-**ROCCurve**
-
-1. `actual_vector` : python `list` or numpy `array` of any stringable objects
-2. `probs` : python `list` or numpy `array`
-3. `classes` : python `list`
-4. `thresholds`: python `list` or numpy `array`
-5. `sample_weight`: python `list` or numpy `array`
-
-**PRCurve**
-
-1. `actual_vector` : python `list` or numpy `array` of any stringable objects
-2. `probs` : python `list` or numpy `array`
-3. `classes` : python `list`
-4. `thresholds`: python `list` or numpy `array`
-5. `sample_weight`: python `list` or numpy `array`
-
-For more information visit [here](https://github.com/sepandhaghighi/pycm/tree/master/Document "Document")
+### Screen record
 
 <div align="center">
-
 <a href="https://asciinema.org/a/171863" target="_blank"><img src="https://asciinema.org/a/171863.png"/></a>
 </div>
 
 ## Try PyCM in your browser!
 
 PyCM can be used online in interactive Jupyter Notebooks via the Binder or Colab services! Try it out now! :
```

#### html2text {}

```diff
@@ -37,30 +37,31 @@
 Branch                      master                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI          pycm/workflows/CI/                  pycm/workflows/CI/
             badge.svg?branch=master]              badge.svg?branch=dev]
              [https://api.codacy.com/project/
 Code Quality           badge/Grade/            [CodeFactor] [codebeat_badge]
              5d9463998a0040d09afc2b80c389365c]
-## Installation â ï¸ PyCM 2.4 is the last version to support **Python 2.7** &
-**Python 3.4** â ï¸ Plotting capability requires **Matplotlib (>= 3.0.0)** or
-**Seaborn (>= 0.9.1)** ### Source code - Download [Version 3.9](https://
-github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://
-github.com/sepandhaghighi/pycm/archive/dev.zip) - Run `pip install -
-r requirements.txt` or `pip3 install -r requirements.txt` (Need root access) -
-Run `python3 setup.py install` or `python setup.py install` (Need root access)
-### PyPI - Check [Python Packaging User Guide](https://packaging.python.org/
-installing/) - Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need
-root access) ### Conda - Check [Conda Managing Package](https://conda.io/) -
-Update Conda using `conda update conda` (Need root access) - Run `conda install
--c sepandhaghighi pycm` (Need root access) ### Easy install - Run `easy_install
---upgrade pycm` (Need root access) ### MATLAB - Download and install [MATLAB]
-(https://www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit) - Download
-and install [Python3.x](https://www.python.org/downloads/) (>=3.5, 64/32 bit) -
-[x] Select `Add to PATH` option - [x] Select `Install pip` option - Run `pip
+## Installation â ï¸ PyCM 3.9 is the last version to support **Python 3.5**
+â ï¸ PyCM 2.4 is the last version to support **Python 2.7** & **Python 3.4**
+â ï¸ Plotting capability requires **Matplotlib (>= 3.0.0)** or **Seaborn (>=
+0.9.1)** ### Source code - Download [Version 4.0](https://github.com/
+sepandhaghighi/pycm/archive/v4.0.zip) or [Latest Source ](https://github.com/
+sepandhaghighi/pycm/archive/dev.zip) - Run `pip install -r requirements.txt` or
+`pip3 install -r requirements.txt` (Need root access) - Run `python3 setup.py
+install` or `python setup.py install` (Need root access) ### PyPI - Check
+[Python Packaging User Guide](https://packaging.python.org/installing/) - Run
+`pip install pycm==4.0` or `pip3 install pycm==4.0` (Need root access) ###
+Conda - Check [Conda Managing Package](https://conda.io/) - Update Conda using
+`conda update conda` (Need root access) - Run `conda install -c sepandhaghighi
+pycm` (Need root access) ### Easy install - Run `easy_install --upgrade pycm`
+(Need root access) ### MATLAB - Download and install [MATLAB](https://
+www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit) - Download and
+install [Python3.x](https://www.python.org/downloads/) (>=3.6, 64/32 bit) - [x]
+Select `Add to PATH` option - [x] Select `Install pip` option - Run `pip
 install pycm` or `pip3 install pycm` (Need root access) - Configure Python
 interpreter ```matlab >> pyversion PYTHON_EXECUTABLE_FULL_PATH ``` - Visit
 [MATLAB Examples](https://github.com/sepandhaghighi/pycm/tree/master/MATLAB) ##
 Usage ### From vector ```pycon >>> from pycm import * >>> y_actu = [2, 0, 2, 2,
 0, 1, 1, 2, 2, 0, 1, 2] >>> y_pred = [0, 0, 2, 1, 0, 2, 1, 0, 2, 0, 2, 2] >>>
 cm = ConfusionMatrix(actual_vector=y_actu, predict_vector=y_pred) >>>
 cm.classes [0, 1, 2] >>> cm.table {0: {0: 3, 1: 0, 2: 0}, 1: {0: 0, 1: 1, 2:
@@ -205,42 +206,31 @@
 any other case, the compared object doesnât select the best confusion matrix.
 ```pycon >>> cm2 = ConfusionMatrix(matrix={0: {0: 2, 1: 50, 2: 6}, 1: {0: 5, 1:
 50, 2: 3}, 2: {0: 1, 1: 7, 2: 50}}) >>> cm3 = ConfusionMatrix(matrix={0: {0:
 50, 1: 2, 2: 6}, 1: {0: 50, 1: 5, 2: 3}, 2: {0: 1, 1: 55, 2: 2}}) >>> cp =
 Compare({"cm2": cm2, "cm3": cm3}) >>> print(cp) Best : cm2 Rank Name Class-
 Score Overall-Score 1 cm2 0.50278 0.58095 2 cm3 0.33611 0.52857 >>> cp.best
 pycm.ConfusionMatrix(classes: [0, 1, 2]) >>> cp.sorted ['cm2', 'cm3'] >>>
-cp.best_name 'cm2' ``` ### Online help `online_help` function is added in
-`version 1.1` in order to open each statistics definition in web browser
-```pycon >>> from pycm import online_help >>> online_help("J") >>> online_help
-("SOA1(Landis & Koch)") >>> online_help(2) ``` * List of items are available by
-calling `online_help()` (without argument) * If PyCM website is not available,
-set `alt_link = True` (new in `version 2.4`) ### Acceptable data types
-**ConfusionMatrix** 1. `actual_vector` : python `list` or numpy `array` of any
-stringable objects 2. `predict_vector` : python `list` or numpy `array` of any
-stringable objects 3. `matrix` : `dict` 4. `digit`: `int` 5. `threshold` :
-`FunctionType (function or lambda)` 6. `file` : `File object` 7.
-`sample_weight` : python `list` or numpy `array` of numbers 8. `transpose` :
-`bool` 9. `classes` : python `list` 10. `is_imbalanced` : `bool` 11.
-`metrics_off` : `bool` * Run `help(ConfusionMatrix)` for `ConfusionMatrix`
-object details **Compare** 1. `cm_dict` : python `dict` of `ConfusionMatrix`
-object (`str` : `ConfusionMatrix`) 2. `by_class` : `bool` 3. `class_weight` :
-python `dict` of class weights (`class_name` : `float`) 4.
-`class_benchmark_weight`: python `dict` of class benchmark weights
-(`class_benchmark_name` : `float`) 5. `overall_benchmark_weight`: python `dict`
-of overall benchmark weights (`overall_benchmark_name` : `float`) 6. `digit`:
-`int` * Run `help(Compare)` for `Compare` object details **ROCCurve** 1.
-`actual_vector` : python `list` or numpy `array` of any stringable objects 2.
-`probs` : python `list` or numpy `array` 3. `classes` : python `list` 4.
-`thresholds`: python `list` or numpy `array` 5. `sample_weight`: python `list`
-or numpy `array` **PRCurve** 1. `actual_vector` : python `list` or numpy
-`array` of any stringable objects 2. `probs` : python `list` or numpy `array`
-3. `classes` : python `list` 4. `thresholds`: python `list` or numpy `array` 5.
-`sample_weight`: python `list` or numpy `array` For more information visit
-[here](https://github.com/sepandhaghighi/pycm/tree/master/Document "Document")
+cp.best_name 'cm2' ``` ### Multilabel confusion matrix From `version 4.0`,
+`MultiLabelCM` has been added to calculate class-wise or sample-wise multilabel
+confusion matrices. In class-wise mode, confusion matrices are calculated for
+each class, and in sample-wise mode, they are generated per sample. All
+generated confusion matrices are binarized with a one-vs-rest transformation.
+```pycon >>> mlcm = MultiLabelCM(actual_vector=[{"cat", "bird"}, {"dog"}],
+predict_vector=[{"cat"}, {"dog", "bird"}], classes=["cat", "dog", "bird"]) >>>
+mlcm.actual_vector_multihot [[1, 0, 1], [0, 1, 0]] >>>
+mlcm.predict_vector_multihot [[1, 0, 0], [0, 1, 1]] >>> mlcm.get_cm_by_class
+("cat").print_matrix() Predict 0 1 Actual 0 1 0 1 0 1 >>> mlcm.get_cm_by_sample
+(0).print_matrix() Predict 0 1 Actual 0 1 0 1 1 1 ``` ### Online help
+`online_help` function is added in `version 1.1` in order to open each
+statistics definition in web browser ```pycon >>> from pycm import online_help
+>>> online_help("J") >>> online_help("SOA1(Landis & Koch)") >>> online_help(2)
+``` * List of items are available by calling `online_help()` (without argument)
+* If PyCM website is not available, set `alt_link = True` (new in `version
+2.4`) ### Screen record
                      [https://asciinema.org/a/171863.png]
 ## Try PyCM in your browser! PyCM can be used online in interactive Jupyter
 Notebooks via the Binder or Colab services! Try it out now! : [![Binder](https:
 //mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sepandhaghighi/pycm/
 master) [![Google Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/sepandhaghighi/pycm/blob/
 master) * Check `Examples` in `Document` folder ## Issues & bug reports 1. Fill
```

### Comparing `pycm-3.9/TODO.md` & `pycm-4.0/TODO.md`

 * *Files identical despite different names*

### Comparing `pycm-3.9/paper/10.21105.joss.00729.pdf` & `pycm-4.0/paper/10.21105.joss.00729.pdf`

 * *Files identical despite different names*

### Comparing `pycm-3.9/paper/paper.bib` & `pycm-4.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `pycm-3.9/paper/paper.md` & `pycm-4.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/__main__.py` & `pycm-4.0/pycm/__main__.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_ci.py` & `pycm-4.0/pycm/pycm_ci.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_class_func.py` & `pycm-4.0/pycm/pycm_class_func.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_compare.py` & `pycm-4.0/pycm/pycm_compare.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_curve.py` & `pycm-4.0/pycm/pycm_curve.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_distance.py` & `pycm-4.0/pycm/pycm_distance.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_error.py` & `pycm-4.0/pycm/pycm_error.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,7 +38,13 @@
     pass
 
 
 class pycmCurveError(Exception):
     """Curve error class."""
 
     pass
+
+
+class pycmMultiLabelError(Exception):
+    """Multilabel error class."""
+
+    pass
```

### Comparing `pycm-3.9/pycm/pycm_handler.py` & `pycm-4.0/pycm/pycm_handler.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_interpret.py` & `pycm-4.0/pycm/pycm_interpret.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_obj.py` & `pycm-4.0/pycm/pycm_obj.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_output.py` & `pycm-4.0/pycm/pycm_output.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_overall_func.py` & `pycm-4.0/pycm/pycm_overall_func.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_param.py` & `pycm-4.0/pycm/pycm_param.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """Parameters and constants."""
-PYCM_VERSION = "3.9"
+PYCM_VERSION = "4.0"
 
 
 OVERVIEW = '''
 PyCM is a multi-class confusion matrix library written in Python that
 supports both input data vectors and direct matrix, and a proper tool for
 post-classification model evaluation that supports most classes and overall
 statistics parameters.
@@ -63,21 +63,25 @@
 PLOT_COLORS_CLASS_MISMATCH_ERROR = "Given colors and classes have not the same length."
 PLOT_MARKERS_CLASS_MISMATCH_ERROR = "Given markers and classes have not the same length."
 VECTOR_TYPE_ERROR = "The type of input vectors is assumed to be a list or a NumPy array"
 VECTOR_SIZE_ERROR = "Input vectors must have same length"
 VECTOR_EMPTY_ERROR = "Input vectors are empty"
 VECTOR_ONLY_ERROR = "This option only works in vector mode"
 VECTOR_UNIQUE_CLASS_ERROR = "The classes list isn't unique. It contains duplicated labels."
+NOT_ALL_SET_VECTOR_ERROR = "Class extraction from input failed. Input vectors should be a list of sets with unified types."
 CLASS_NUMBER_ERROR = "Number of the classes is lower than 2"
 METRICS_OFF_ERROR = "This method cannot be executed while 'metrics_off=True'."
 CLASSES_ERROR = "Used classes is not a subset of matrix's classes."
 COMPARE_FORMAT_ERROR = "The input type is supposed to be dictionary but it's not!"
 CLASSES_LENGHT_ERROR = "Classes length is not equal to the array length."
 AREA_METHOD_ERROR = "The numeric integral method can only be selected between 'trapezoidal' and 'midpoint'!"
 
+VECTOR_INDEX_ERROR = "Given index is out of vector's range."
+INVALID_CLASS_NAME_ERROR = "Given class name is not among problem's classes."
+
 COMPARE_TYPE_ERROR = "The input is supposed to consist of pycm.ConfusionMatrix object but it's not!"
 COMPARE_DOMAIN_ERROR = "The domain of all ConfusionMatrix objects must be same! The sample size or the number " \
                        "of classes are different."
 COMPARE_NUMBER_ERROR = "Lower than two confusion matrices is given for comparing. The minimum number of " \
                        "confusion matrix for comparing is 2."
 
 COMPARE_CLASS_WEIGHT_ERROR = "The class_weight type must be dictionary and also must be specified for all of the classes."
@@ -116,14 +120,16 @@
 
 CLASSES_WARNING = "Used classes is not a subset of classes in actual and predict vectors."
 
 CLASSES_TYPE_WARNING = "The classes is neither a list nor None so it'll be ignored."
 
 CURVE_NONE_WARNING = "The curve axes contain non-numerical value(s)."
 
+DEPRECATION_WARNING = "`{}` is deprecated and may be removed in future releases."
+
 DISTANCE_METRIC_TYPE_ERROR = "The metric type must be DistanceType"
 
 CLASS_NUMBER_THRESHOLD = 10
 
 BALANCE_RATIO_THRESHOLD = 3
 
 CLASS_PARAMS = {
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-# -*- coding: utf-8 -*- """Parameters and constants.""" PYCM_VERSION = "3.9"
+# -*- coding: utf-8 -*- """Parameters and constants.""" PYCM_VERSION = "4.0"
 OVERVIEW = ''' PyCM is a multi-class confusion matrix library written in Python
 that supports both input data vectors and direct matrix, and a proper tool for
 post-classification model evaluation that supports most classes and overall
 statistics parameters. PyCM is the swiss-army knife of confusion matrices,
 targeted mainly at data scientists that need a broad array of metrics for
 predictive models and an accurate evaluation of large variety of classifiers.
 If you use PyCM in your research, we would appreciate citations to the
@@ -39,24 +39,28 @@
 install it using this command: pip install matplotlib"
 PLOT_COLORS_CLASS_MISMATCH_ERROR = "Given colors and classes have not the same
 length." PLOT_MARKERS_CLASS_MISMATCH_ERROR = "Given markers and classes have
 not the same length." VECTOR_TYPE_ERROR = "The type of input vectors is assumed
 to be a list or a NumPy array" VECTOR_SIZE_ERROR = "Input vectors must have
 same length" VECTOR_EMPTY_ERROR = "Input vectors are empty" VECTOR_ONLY_ERROR =
 "This option only works in vector mode" VECTOR_UNIQUE_CLASS_ERROR = "The
-classes list isn't unique. It contains duplicated labels." CLASS_NUMBER_ERROR =
-"Number of the classes is lower than 2" METRICS_OFF_ERROR = "This method cannot
-be executed while 'metrics_off=True'." CLASSES_ERROR = "Used classes is not a
+classes list isn't unique. It contains duplicated labels."
+NOT_ALL_SET_VECTOR_ERROR = "Class extraction from input failed. Input vectors
+should be a list of sets with unified types." CLASS_NUMBER_ERROR = "Number of
+the classes is lower than 2" METRICS_OFF_ERROR = "This method cannot be
+executed while 'metrics_off=True'." CLASSES_ERROR = "Used classes is not a
 subset of matrix's classes." COMPARE_FORMAT_ERROR = "The input type is supposed
 to be dictionary but it's not!" CLASSES_LENGHT_ERROR = "Classes length is not
 equal to the array length." AREA_METHOD_ERROR = "The numeric integral method
-can only be selected between 'trapezoidal' and 'midpoint'!" COMPARE_TYPE_ERROR
-= "The input is supposed to consist of pycm.ConfusionMatrix object but it's
-not!" COMPARE_DOMAIN_ERROR = "The domain of all ConfusionMatrix objects must be
-same! The sample size or the number " \ "of classes are different."
+can only be selected between 'trapezoidal' and 'midpoint'!" VECTOR_INDEX_ERROR
+= "Given index is out of vector's range." INVALID_CLASS_NAME_ERROR = "Given
+class name is not among problem's classes." COMPARE_TYPE_ERROR = "The input is
+supposed to consist of pycm.ConfusionMatrix object but it's not!"
+COMPARE_DOMAIN_ERROR = "The domain of all ConfusionMatrix objects must be same!
+The sample size or the number " \ "of classes are different."
 COMPARE_NUMBER_ERROR = "Lower than two confusion matrices is given for
 comparing. The minimum number of " \ "confusion matrix for comparing is 2."
 COMPARE_CLASS_WEIGHT_ERROR = "The class_weight type must be dictionary and also
 must be specified for all of the classes." COMPARE_CLASS_BENCHMARK_WEIGHT_ERROR
 = "The class_benchmark_weight type must be dictionary and also must be
 specified for all of the class benchmarks."
 COMPARE_OVERALL_BENCHMARK_WEIGHT_ERROR = "The overall_benchmark_weight type
@@ -80,21 +84,22 @@
 confusion matrix is a high dimension matrix and won't be demonstrated
 properly.\n" \ "If confusion matrix has too many zeros (sparse matrix) you can
 set `sparse` flag to True in printing functions "\ "otherwise by using save_csv
 method to save the confusion matrix in csv format you'll have better
 demonstration." CLASSES_WARNING = "Used classes is not a subset of classes in
 actual and predict vectors." CLASSES_TYPE_WARNING = "The classes is neither a
 list nor None so it'll be ignored." CURVE_NONE_WARNING = "The curve axes
-contain non-numerical value(s)." DISTANCE_METRIC_TYPE_ERROR = "The metric type
-must be DistanceType" CLASS_NUMBER_THRESHOLD = 10 BALANCE_RATIO_THRESHOLD = 3
-CLASS_PARAMS = { "TPR": "TPR", "TNR": "TNR", "PPV": "PPV", "NPV": "NPV", "FNR":
-"FNR", "FPR": "FPR", "FDR": "FDR", "FOR": "FOR", "ACC": "ACC", "F1": "F1",
-"MCC": "MCC", "BM": "BM", "MK": "MK", "PLR": "PLR", "NLR": "NLR", "DOR": "DOR",
-"TP": "TP", "TN": "TN", "FP": "FP", "FN": "FN", "POP": "POP", "P": "P", "N":
-"N", "TOP": "TOP", "TON": "TON", "PRE": "PRE", "G": "G", "RACC": "RACC",
+contain non-numerical value(s)." DEPRECATION_WARNING = "`{}` is deprecated and
+may be removed in future releases." DISTANCE_METRIC_TYPE_ERROR = "The metric
+type must be DistanceType" CLASS_NUMBER_THRESHOLD = 10 BALANCE_RATIO_THRESHOLD
+= 3 CLASS_PARAMS = { "TPR": "TPR", "TNR": "TNR", "PPV": "PPV", "NPV": "NPV",
+"FNR": "FNR", "FPR": "FPR", "FDR": "FDR", "FOR": "FOR", "ACC": "ACC", "F1":
+"F1", "MCC": "MCC", "BM": "BM", "MK": "MK", "PLR": "PLR", "NLR": "NLR", "DOR":
+"DOR", "TP": "TP", "TN": "TN", "FP": "FP", "FN": "FN", "POP": "POP", "P": "P",
+"N": "N", "TOP": "TOP", "TON": "TON", "PRE": "PRE", "G": "G", "RACC": "RACC",
 "F0.5": "F05", "F2": "F2", "ERR": "ERR", "RACCU": "RACCU", "J": "J", "IS":
 "IS", "CEN": "CEN", "MCEN": "MCEN", "AUC": "AUC", "sInd": "sInd", "dInd":
 "dInd", "DP": "DP", "Y": "Y", "PLRI": "PLRI", "DPI": "DPI", "AUCI": "AUCI",
 "GI": "GI", "LS": "LS", "AM": "AM", "BCD": "BCD", "OP": "OP", "IBA": "IBA",
 "GM": "GM", "Q": "Q", "AGM": "AGM", "NLRI": "NLRI", "MCCI": "MCCI", "AGF":
 "AGF", "OC": "OC", "OOC": "OOC", "AUPR": "AUPR", "ICSI": "ICSI", "QI": "QI",
 "HD": "HD", "BB": "BB", } OVERALL_PARAMS = { 'Overall ACC': 'Overall_ACC',
```

### Comparing `pycm-3.9/pycm/pycm_test.py` & `pycm-4.0/pycm/pycm_test.py`

 * *Files identical despite different names*

### Comparing `pycm-3.9/pycm/pycm_util.py` & `pycm-4.0/pycm/pycm_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -771,13 +771,41 @@
         """
         Inner function.
 
         :param args: non-keyword arguments
         :type args: list
         :param kwargs: keyword arguments
         :type kwargs: dict
-        :return: None
+        :return: modified function result
         """
         if args[0].metrics_off:
             raise pycmMatrixError(METRICS_OFF_ERROR)
         return func(*args, **kwargs)
     return inner_function
+
+
+def deprecated(func):
+    """
+    Send a warning regarding function's deprecation.
+
+    :param func: input function
+    :type func: function
+    :return: inner function
+    """
+    @wraps(func)
+    def inner_function(*args, **kwargs):
+        """
+        Inner function.
+
+        :param args: non-keyword arguments
+        :type args: list
+        :param kwargs: keyword arguments
+        :type kwargs: dict
+        :return: modified function result
+        """
+        warn(
+            DEPRECATION_WARNING.format(
+                func.__name__),
+            category=DeprecationWarning,
+            stacklevel=2)
+        return func(*args, **kwargs)
+    return inner_function
```

### Comparing `pycm-3.9/pycm.egg-info/PKG-INFO` & `pycm-4.0/pycm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: pycm
-Version: 3.9
+Version: 4.0
 Summary: Multi-class confusion matrix library in Python
 Home-page: https://github.com/sepandhaghighi/pycm
-Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.9
+Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v4.0
 Author: PyCM Development Team
 Author-email: info@pycm.io
 License: MIT
 Project-URL: Webpage, https://www.pycm.io
 Project-URL: Source, https://github.com/sepandhaghighi/pycm
 Project-URL: Discord, https://discord.com/invite/zqpU2b3J3f
 Keywords: confusion-matrix python3 python machine_learning ML
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
@@ -31,15 +30,15 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 
 <div align="center">
 <img src="https://github.com/sepandhaghighi/pycm/raw/master/Otherfiles/logo.png" width="550">
@@ -128,42 +127,44 @@
 		<td align="center"><a href="https://www.codefactor.io/repository/github/sepandhaghighi/pycm/overview/dev"><img src="https://www.codefactor.io/repository/github/sepandhaghighi/pycm/badge/dev" alt="CodeFactor" /></a></td>
 		<td align="center"><a href="https://codebeat.co/projects/github-com-sepandhaghighi-pycm-dev"><img alt="codebeat badge" src="https://codebeat.co/badges/f6642af1-c343-48c2-bd3e-eee802facf39" /></a></td>
 	</tr>
 </table>
 
 ## Installation
 
+⚠️  PyCM 3.9 is the last version to support **Python 3.5**
+
 ⚠️  PyCM 2.4 is the last version to support **Python 2.7** & **Python 3.4**
 
 ⚠️  Plotting capability requires **Matplotlib (>= 3.0.0)** or **Seaborn (>= 0.9.1)**
 
 ### Source code
-- Download [Version 3.9](https://github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
+- Download [Version 4.0](https://github.com/sepandhaghighi/pycm/archive/v4.0.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
 - Run `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
 - Run `python3 setup.py install` or `python setup.py install` (Need root access)
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need root access)
+- Run `pip install pycm==4.0` or `pip3 install pycm==4.0` (Need root access)
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io/)
 - Update Conda using `conda update conda` (Need root access)
 - Run `conda install -c sepandhaghighi pycm` (Need root access)
 
 ### Easy install
 
 - Run `easy_install --upgrade pycm` (Need root access)
 
 ### MATLAB
 
 - Download and install [MATLAB](https://www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit)
-- Download and install [Python3.x](https://www.python.org/downloads/) (>=3.5, 64/32 bit)
+- Download and install [Python3.x](https://www.python.org/downloads/) (>=3.6, 64/32 bit)
 	- [x] Select `Add to PATH` option
 	- [x] Select `Install pip` option
 - Run `pip install pycm` or `pip3 install pycm` (Need root access)
 - Configure Python interpreter
 
 ```matlab
 >> pyversion PYTHON_EXECUTABLE_FULL_PATH
@@ -474,77 +475,57 @@
 pycm.ConfusionMatrix(classes: [0, 1, 2])
 >>> cp.sorted
 ['cm2', 'cm3']
 >>> cp.best_name
 'cm2'
 ```
 
+### Multilabel confusion matrix
+
+From `version 4.0`, `MultiLabelCM` has been added to calculate class-wise or sample-wise multilabel confusion matrices. In class-wise mode, confusion matrices are calculated for each class, and in sample-wise mode, they are generated per sample. All generated confusion matrices are binarized with a one-vs-rest transformation.
+
+```pycon
+>>> mlcm = MultiLabelCM(actual_vector=[{"cat", "bird"}, {"dog"}], predict_vector=[{"cat"}, {"dog", "bird"}], classes=["cat", "dog", "bird"])
+>>> mlcm.actual_vector_multihot
+[[1, 0, 1], [0, 1, 0]]
+>>> mlcm.predict_vector_multihot
+[[1, 0, 0], [0, 1, 1]]
+>>> mlcm.get_cm_by_class("cat").print_matrix()
+Predict 0       1       
+Actual
+0       1       0       
+
+1       0       1       
+
+>>> mlcm.get_cm_by_sample(0).print_matrix()
+Predict 0       1       
+Actual
+0       1       0       
+
+1       1       1 
+
+```
+
 ### Online help
 
 `online_help` function is added in `version 1.1` in order to open each statistics definition in web browser
 
 ```pycon
 >>> from pycm import online_help
 >>> online_help("J")
 >>> online_help("SOA1(Landis & Koch)")
 >>> online_help(2)
 ```
 
 * List of items are available by calling `online_help()` (without argument)
 * If PyCM website is not available, set `alt_link = True` (new in `version 2.4`)
 
-### Acceptable data types
-
-**ConfusionMatrix**
-
-1. `actual_vector` : python `list` or numpy `array` of any stringable objects
-2. `predict_vector` : python `list` or numpy `array` of any stringable objects
-3. `matrix` : `dict`
-4. `digit`: `int`
-5. `threshold` : `FunctionType (function or lambda)`
-6. `file` : `File object`
-7. `sample_weight` : python `list` or numpy `array` of numbers
-8. `transpose` : `bool`
-9. `classes` : python `list`
-10. `is_imbalanced` : `bool`
-11. `metrics_off` : `bool`
-
-* Run `help(ConfusionMatrix)` for `ConfusionMatrix` object details
-
-**Compare**
-
-1. `cm_dict` : python `dict` of `ConfusionMatrix` object (`str` : `ConfusionMatrix`)
-2. `by_class` : `bool`
-3. `class_weight` : python `dict` of class weights (`class_name` : `float`)
-4. `class_benchmark_weight`: python `dict` of class benchmark weights (`class_benchmark_name` : `float`)
-5. `overall_benchmark_weight`: python `dict` of overall benchmark weights (`overall_benchmark_name` : `float`)
-6. `digit`: `int`
-
-* Run `help(Compare)` for `Compare` object details
-
-**ROCCurve**
-
-1. `actual_vector` : python `list` or numpy `array` of any stringable objects
-2. `probs` : python `list` or numpy `array`
-3. `classes` : python `list`
-4. `thresholds`: python `list` or numpy `array`
-5. `sample_weight`: python `list` or numpy `array`
-
-**PRCurve**
-
-1. `actual_vector` : python `list` or numpy `array` of any stringable objects
-2. `probs` : python `list` or numpy `array`
-3. `classes` : python `list`
-4. `thresholds`: python `list` or numpy `array`
-5. `sample_weight`: python `list` or numpy `array`
-
-For more information visit [here](https://github.com/sepandhaghighi/pycm/tree/master/Document "Document")
+### Screen record
 
 <div align="center">
-
 <a href="https://asciinema.org/a/171863" target="_blank"><img src="https://asciinema.org/a/171863.png"/></a>
 </div>
 
 ## Try PyCM in your browser!
 
 PyCM can be used online in interactive Jupyter Notebooks via the Binder or Colab services! Try it out now! :
 
@@ -630,14 +611,31 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [4.0] - 2023-06-07
+### Added
+- `pycmMultiLabelError` class
+- `MultiLabelCM` class
+- `get_cm_by_class` method
+- `get_cm_by_sample` method
+- `__mlcm_vector_handler__` function
+- `__mlcm_assign_classes__` function
+- `__mlcm_vectors_filter__` function
+- `__set_to_multihot__` function
+- `deprecated` function
+### Changed
+- Document modified
+- `README.md` modified
+- Example-4 modified
+- Test system modified
+- Python 3.5 support dropped
 ## [3.9] - 2023-05-01
 ### Added
 - `OVERALL_PARAMS` dictionary
 - `__imbalancement_handler__` function
 - `vector_serializer` function
 - NPV micro/macro
 - `log_loss` method
@@ -1317,15 +1315,16 @@
 - MK
 - NPV
 - PPV
 - TNR
 - TPR
 - documents and `README.md`
 
-[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v3.9...dev
+[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v4.0...dev
+[4.0]: https://github.com/sepandhaghighi/pycm/compare/v3.9...v4.0
 [3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9
 [3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8
 [3.7]: https://github.com/sepandhaghighi/pycm/compare/v3.6...v3.7
 [3.6]: https://github.com/sepandhaghighi/pycm/compare/v3.5...v3.6
 [3.5]: https://github.com/sepandhaghighi/pycm/compare/v3.4...v3.5
 [3.4]: https://github.com/sepandhaghighi/pycm/compare/v3.3...v3.4
 [3.3]: https://github.com/sepandhaghighi/pycm/compare/v3.2...v3.3
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: pycm Version: 3.9 Summary: Multi-class confusion
+Metadata-Version: 2.1 Name: pycm Version: 4.0 Summary: Multi-class confusion
 matrix library in Python Home-page: https://github.com/sepandhaghighi/pycm
-Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.9 Author: PyCM
+Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v4.0 Author: PyCM
 Development Team Author-email: info@pycm.io License: MIT Project-URL: Webpage,
 https://www.pycm.io Project-URL: Source, https://github.com/sepandhaghighi/pycm
 Project-URL: Discord, https://discord.com/invite/zqpU2b3J3f Keywords:
 confusion-matrix python3 python machine_learning ML Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: End Users/Desktop Classifier: Intended Audience :: Manufacturing
-Classifier: Intended Audience :: Science/Research Classifier: Topic ::
-Scientific/Engineering :: Information Analysis Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
-Engineering :: Human Machine Interfaces Classifier: Topic :: Scientific/
-Engineering :: Mathematics Classifier: Topic :: Scientific/Engineering ::
-Physics Requires-Python: >=3.5 Description-Content-Type: text/markdown License-
-File: LICENSE License-File: AUTHORS.md
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
+Audience :: Manufacturing Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Information Analysis Classifier:
+Topic :: Education Classifier: Topic :: Scientific/Engineering Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+Scientific/Engineering :: Human Machine Interfaces Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
+Engineering :: Physics Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE License-File: AUTHORS.md
     [https://github.com/sepandhaghighi/pycm/raw/master/Otherfiles/logo.png]
                   ****** PyCM: Python Confusion Matrix ******
 
   [built_with_Python3] [https://img.shields.io/badge/doc-latest-orange.svg]
 [https://codecov.io/gh/sepandhaghighi/pycm/branch/master/graph/badge.svg] [PyPI
     version] [https://anaconda.org/sepandhaghighi/pycm/badges/version.svg]
                          [Document] [Discord_Channel]
@@ -62,30 +61,31 @@
 Branch                      master                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI          pycm/workflows/CI/                  pycm/workflows/CI/
             badge.svg?branch=master]              badge.svg?branch=dev]
              [https://api.codacy.com/project/
 Code Quality           badge/Grade/            [CodeFactor] [codebeat_badge]
              5d9463998a0040d09afc2b80c389365c]
-## Installation â ï¸ PyCM 2.4 is the last version to support **Python 2.7** &
-**Python 3.4** â ï¸ Plotting capability requires **Matplotlib (>= 3.0.0)** or
-**Seaborn (>= 0.9.1)** ### Source code - Download [Version 3.9](https://
-github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://
-github.com/sepandhaghighi/pycm/archive/dev.zip) - Run `pip install -
-r requirements.txt` or `pip3 install -r requirements.txt` (Need root access) -
-Run `python3 setup.py install` or `python setup.py install` (Need root access)
-### PyPI - Check [Python Packaging User Guide](https://packaging.python.org/
-installing/) - Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need
-root access) ### Conda - Check [Conda Managing Package](https://conda.io/) -
-Update Conda using `conda update conda` (Need root access) - Run `conda install
--c sepandhaghighi pycm` (Need root access) ### Easy install - Run `easy_install
---upgrade pycm` (Need root access) ### MATLAB - Download and install [MATLAB]
-(https://www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit) - Download
-and install [Python3.x](https://www.python.org/downloads/) (>=3.5, 64/32 bit) -
-[x] Select `Add to PATH` option - [x] Select `Install pip` option - Run `pip
+## Installation â ï¸ PyCM 3.9 is the last version to support **Python 3.5**
+â ï¸ PyCM 2.4 is the last version to support **Python 2.7** & **Python 3.4**
+â ï¸ Plotting capability requires **Matplotlib (>= 3.0.0)** or **Seaborn (>=
+0.9.1)** ### Source code - Download [Version 4.0](https://github.com/
+sepandhaghighi/pycm/archive/v4.0.zip) or [Latest Source ](https://github.com/
+sepandhaghighi/pycm/archive/dev.zip) - Run `pip install -r requirements.txt` or
+`pip3 install -r requirements.txt` (Need root access) - Run `python3 setup.py
+install` or `python setup.py install` (Need root access) ### PyPI - Check
+[Python Packaging User Guide](https://packaging.python.org/installing/) - Run
+`pip install pycm==4.0` or `pip3 install pycm==4.0` (Need root access) ###
+Conda - Check [Conda Managing Package](https://conda.io/) - Update Conda using
+`conda update conda` (Need root access) - Run `conda install -c sepandhaghighi
+pycm` (Need root access) ### Easy install - Run `easy_install --upgrade pycm`
+(Need root access) ### MATLAB - Download and install [MATLAB](https://
+www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit) - Download and
+install [Python3.x](https://www.python.org/downloads/) (>=3.6, 64/32 bit) - [x]
+Select `Add to PATH` option - [x] Select `Install pip` option - Run `pip
 install pycm` or `pip3 install pycm` (Need root access) - Configure Python
 interpreter ```matlab >> pyversion PYTHON_EXECUTABLE_FULL_PATH ``` - Visit
 [MATLAB Examples](https://github.com/sepandhaghighi/pycm/tree/master/MATLAB) ##
 Usage ### From vector ```pycon >>> from pycm import * >>> y_actu = [2, 0, 2, 2,
 0, 1, 1, 2, 2, 0, 1, 2] >>> y_pred = [0, 0, 2, 1, 0, 2, 1, 0, 2, 0, 2, 2] >>>
 cm = ConfusionMatrix(actual_vector=y_actu, predict_vector=y_pred) >>>
 cm.classes [0, 1, 2] >>> cm.table {0: {0: 3, 1: 0, 2: 0}, 1: {0: 0, 1: 1, 2:
@@ -230,42 +230,31 @@
 any other case, the compared object doesnât select the best confusion matrix.
 ```pycon >>> cm2 = ConfusionMatrix(matrix={0: {0: 2, 1: 50, 2: 6}, 1: {0: 5, 1:
 50, 2: 3}, 2: {0: 1, 1: 7, 2: 50}}) >>> cm3 = ConfusionMatrix(matrix={0: {0:
 50, 1: 2, 2: 6}, 1: {0: 50, 1: 5, 2: 3}, 2: {0: 1, 1: 55, 2: 2}}) >>> cp =
 Compare({"cm2": cm2, "cm3": cm3}) >>> print(cp) Best : cm2 Rank Name Class-
 Score Overall-Score 1 cm2 0.50278 0.58095 2 cm3 0.33611 0.52857 >>> cp.best
 pycm.ConfusionMatrix(classes: [0, 1, 2]) >>> cp.sorted ['cm2', 'cm3'] >>>
-cp.best_name 'cm2' ``` ### Online help `online_help` function is added in
-`version 1.1` in order to open each statistics definition in web browser
-```pycon >>> from pycm import online_help >>> online_help("J") >>> online_help
-("SOA1(Landis & Koch)") >>> online_help(2) ``` * List of items are available by
-calling `online_help()` (without argument) * If PyCM website is not available,
-set `alt_link = True` (new in `version 2.4`) ### Acceptable data types
-**ConfusionMatrix** 1. `actual_vector` : python `list` or numpy `array` of any
-stringable objects 2. `predict_vector` : python `list` or numpy `array` of any
-stringable objects 3. `matrix` : `dict` 4. `digit`: `int` 5. `threshold` :
-`FunctionType (function or lambda)` 6. `file` : `File object` 7.
-`sample_weight` : python `list` or numpy `array` of numbers 8. `transpose` :
-`bool` 9. `classes` : python `list` 10. `is_imbalanced` : `bool` 11.
-`metrics_off` : `bool` * Run `help(ConfusionMatrix)` for `ConfusionMatrix`
-object details **Compare** 1. `cm_dict` : python `dict` of `ConfusionMatrix`
-object (`str` : `ConfusionMatrix`) 2. `by_class` : `bool` 3. `class_weight` :
-python `dict` of class weights (`class_name` : `float`) 4.
-`class_benchmark_weight`: python `dict` of class benchmark weights
-(`class_benchmark_name` : `float`) 5. `overall_benchmark_weight`: python `dict`
-of overall benchmark weights (`overall_benchmark_name` : `float`) 6. `digit`:
-`int` * Run `help(Compare)` for `Compare` object details **ROCCurve** 1.
-`actual_vector` : python `list` or numpy `array` of any stringable objects 2.
-`probs` : python `list` or numpy `array` 3. `classes` : python `list` 4.
-`thresholds`: python `list` or numpy `array` 5. `sample_weight`: python `list`
-or numpy `array` **PRCurve** 1. `actual_vector` : python `list` or numpy
-`array` of any stringable objects 2. `probs` : python `list` or numpy `array`
-3. `classes` : python `list` 4. `thresholds`: python `list` or numpy `array` 5.
-`sample_weight`: python `list` or numpy `array` For more information visit
-[here](https://github.com/sepandhaghighi/pycm/tree/master/Document "Document")
+cp.best_name 'cm2' ``` ### Multilabel confusion matrix From `version 4.0`,
+`MultiLabelCM` has been added to calculate class-wise or sample-wise multilabel
+confusion matrices. In class-wise mode, confusion matrices are calculated for
+each class, and in sample-wise mode, they are generated per sample. All
+generated confusion matrices are binarized with a one-vs-rest transformation.
+```pycon >>> mlcm = MultiLabelCM(actual_vector=[{"cat", "bird"}, {"dog"}],
+predict_vector=[{"cat"}, {"dog", "bird"}], classes=["cat", "dog", "bird"]) >>>
+mlcm.actual_vector_multihot [[1, 0, 1], [0, 1, 0]] >>>
+mlcm.predict_vector_multihot [[1, 0, 0], [0, 1, 1]] >>> mlcm.get_cm_by_class
+("cat").print_matrix() Predict 0 1 Actual 0 1 0 1 0 1 >>> mlcm.get_cm_by_sample
+(0).print_matrix() Predict 0 1 Actual 0 1 0 1 1 1 ``` ### Online help
+`online_help` function is added in `version 1.1` in order to open each
+statistics definition in web browser ```pycon >>> from pycm import online_help
+>>> online_help("J") >>> online_help("SOA1(Landis & Koch)") >>> online_help(2)
+``` * List of items are available by calling `online_help()` (without argument)
+* If PyCM website is not available, set `alt_link = True` (new in `version
+2.4`) ### Screen record
                      [https://asciinema.org/a/171863.png]
 ## Try PyCM in your browser! PyCM can be used online in interactive Jupyter
 Notebooks via the Binder or Colab services! Try it out now! : [![Binder](https:
 //mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sepandhaghighi/pycm/
 master) [![Google Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/sepandhaghighi/pycm/blob/
 master) * Check `Examples` in `Document` folder ## Issues & bug reports 1. Fill
@@ -313,37 +302,42 @@
 ## Show your support ### Star this repo Give a â­ï¸ if this project helped
 you! ### Donate to our project If you do like our project and we hope that you
 do, can you please support us? Our project is not and is never going to be
 working for profit. We need the money just so we can continue doing what we do
 ;-) . [PyCM_Donation] # Changelog All notable changes to this project will be
 documented in this file. The format is based on [Keep a Changelog](http://
 keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning]
-(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ## [3.9] - 2023-05-01 ###
-Added - `OVERALL_PARAMS` dictionary - `__imbalancement_handler__` function -
-`vector_serializer` function - NPV micro/macro - `log_loss` method - 23 new
-distance/similarity 1. Dennis 2. Digby 3. Dispersion 4. Doolittle 5. Eyraud 6.
-Fager & McGowan 7. Faith 8. Fleiss-Levin-Paik 9. Forbes I 10. Forbes II 11.
-Fossum 12. Gilbert & Wells 13. Goodall 14. Goodman & Kruskal's Lambda 15.
-Goodman & Kruskal Lambda-r 16. Guttman's Lambda A 17. Guttman's Lambda B 18.
-Hamann 19. Harris & Lahey 20. Hawkins & Dotson 21. Kendall's Tau 22. Kent &
-Foster I 23. Kent & Foster II ### Changed - `metrics_off` parameter added to
-ConfusionMatrix `__init__` method - `CLASS_PARAMS` changed to a dictionary -
-Code style modified - `sort` parameter added to `relabel` method - Document
-modified - `CONTRIBUTING.md` updated - `codecov` removed from `dev-
-requirements.txt` - Test system modified ## [3.8] - 2023-02-01 ### Added -
-`distance` method - `__contains__` method - `__getitem__` method - Goodman-
-Kruskal's Lambda A benchmark - Goodman-Kruskal's Lambda B benchmark -
-Krippendorff's Alpha benchmark - Pearson's C benchmark - 30 new distance/
-similarity 1. AMPLE 2. Anderberg's D 3. Andres & Marzo's Delta 4. Baroni-Urbani
-& Buser I 5. Baroni-Urbani & Buser II 6. Batagelj & Bren 7. Baulieu I 8.
-Baulieu II 9. Baulieu III 10. Baulieu IV 11. Baulieu V 12. Baulieu VI 13.
-Baulieu VII 14. Baulieu VIII 15. Baulieu IX 16. Baulieu X 17. Baulieu XI 18.
-Baulieu XII 19. Baulieu XIII 20. Baulieu XIV 21. Baulieu XV 22. Benini I 23.
-Benini II 24. Canberra 25. Clement 26. Consonni & Todeschini I 27. Consonni &
-Todeschini II 28. Consonni & Todeschini III 29. Consonni & Todeschini IV 30.
+(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ## [4.0] - 2023-06-07 ###
+Added - `pycmMultiLabelError` class - `MultiLabelCM` class - `get_cm_by_class`
+method - `get_cm_by_sample` method - `__mlcm_vector_handler__` function -
+`__mlcm_assign_classes__` function - `__mlcm_vectors_filter__` function -
+`__set_to_multihot__` function - `deprecated` function ### Changed - Document
+modified - `README.md` modified - Example-4 modified - Test system modified -
+Python 3.5 support dropped ## [3.9] - 2023-05-01 ### Added - `OVERALL_PARAMS`
+dictionary - `__imbalancement_handler__` function - `vector_serializer`
+function - NPV micro/macro - `log_loss` method - 23 new distance/similarity 1.
+Dennis 2. Digby 3. Dispersion 4. Doolittle 5. Eyraud 6. Fager & McGowan 7.
+Faith 8. Fleiss-Levin-Paik 9. Forbes I 10. Forbes II 11. Fossum 12. Gilbert &
+Wells 13. Goodall 14. Goodman & Kruskal's Lambda 15. Goodman & Kruskal Lambda-
+r 16. Guttman's Lambda A 17. Guttman's Lambda B 18. Hamann 19. Harris & Lahey
+20. Hawkins & Dotson 21. Kendall's Tau 22. Kent & Foster I 23. Kent & Foster II
+### Changed - `metrics_off` parameter added to ConfusionMatrix `__init__`
+method - `CLASS_PARAMS` changed to a dictionary - Code style modified - `sort`
+parameter added to `relabel` method - Document modified - `CONTRIBUTING.md`
+updated - `codecov` removed from `dev-requirements.txt` - Test system modified
+## [3.8] - 2023-02-01 ### Added - `distance` method - `__contains__` method -
+`__getitem__` method - Goodman-Kruskal's Lambda A benchmark - Goodman-Kruskal's
+Lambda B benchmark - Krippendorff's Alpha benchmark - Pearson's C benchmark -
+30 new distance/similarity 1. AMPLE 2. Anderberg's D 3. Andres & Marzo's Delta
+4. Baroni-Urbani & Buser I 5. Baroni-Urbani & Buser II 6. Batagelj & Bren 7.
+Baulieu I 8. Baulieu II 9. Baulieu III 10. Baulieu IV 11. Baulieu V 12. Baulieu
+VI 13. Baulieu VII 14. Baulieu VIII 15. Baulieu IX 16. Baulieu X 17. Baulieu XI
+18. Baulieu XII 19. Baulieu XIII 20. Baulieu XIV 21. Baulieu XV 22. Benini I
+23. Benini II 24. Canberra 25. Clement 26. Consonni & Todeschini I 27. Consonni
+& Todeschini II 28. Consonni & Todeschini III 29. Consonni & Todeschini IV 30.
 Consonni & Todeschini V ### Changed - `relabel` method sort bug fixed -
 `README.md` modified - `Compare` overall benchmarks default weights updated -
 Document modified - Test system modified ## [3.7] - 2022-12-15 ### Added -
 `Curve` class - `ROCCurve` class - `PRCurve` class - `pycmCurveError` class ###
 Changed - `CONTRIBUTING.md` updated - `matrix_params_calc` function optimized -
 `README.md` modified - Document modified - Test system modified - `Python 3.11`
 added to `test.yml` ## [3.6] - 2022-08-17 ### Added - Hamming distance - Braun-
@@ -532,17 +526,18 @@
 benchmark - `overall_stat` ## [0.2] - 2018-01-24 ### Added - Population -
 Condition positive - Condition negative - Test outcome positive - Test outcome
 negative - Prevalence - G-measure - Matrix method - Normalized matrix method -
 Params method ### Changed - `statistic_result` to `class_stat` - `params` to
 `stat` ## [0.1] - 2018-01-22 ### Added - ACC - BM - DOR - F1-Score - FDR - FNR
 - FOR - FPR - LR+ - LR- - MCC - MK - NPV - PPV - TNR - TPR - documents and
 `README.md` [Unreleased]: https://github.com/sepandhaghighi/pycm/compare/
-v3.9...dev [3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9
-[3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8 [3.7]: https:
-//github.com/sepandhaghighi/pycm/compare/v3.6...v3.7 [3.6]: https://github.com/
+v4.0...dev [4.0]: https://github.com/sepandhaghighi/pycm/compare/v3.9...v4.0
+[3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9 [3.8]: https:
+//github.com/sepandhaghighi/pycm/compare/v3.7...v3.8 [3.7]: https://github.com/
+sepandhaghighi/pycm/compare/v3.6...v3.7 [3.6]: https://github.com/
 sepandhaghighi/pycm/compare/v3.5...v3.6 [3.5]: https://github.com/
 sepandhaghighi/pycm/compare/v3.4...v3.5 [3.4]: https://github.com/
 sepandhaghighi/pycm/compare/v3.3...v3.4 [3.3]: https://github.com/
 sepandhaghighi/pycm/compare/v3.2...v3.3 [3.2]: https://github.com/
 sepandhaghighi/pycm/compare/v3.1...v3.2 [3.1]: https://github.com/
 sepandhaghighi/pycm/compare/v3.0...v3.1 [3.0]: https://github.com/
 sepandhaghighi/pycm/compare/v2.9...v3.0 [2.9]: https://github.com/
```

### Comparing `pycm-3.9/pycm.egg-info/SOURCES.txt` & `pycm-4.0/pycm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 MANIFEST.in
 README.md
 TODO.md
 codecov.yml
 dev-requirements.txt
 pytest.ini
 requirements.txt
-setup.cfg
 setup.py
 Otherfiles/PSF.png
 Otherfiles/block_diagram.jpg
 Otherfiles/compare_block_diagram.jpg
 Otherfiles/logo.png
 Otherfiles/plot1.png
 Otherfiles/plot2.png
@@ -30,14 +29,15 @@
 pycm/pycm_class_func.py
 pycm/pycm_compare.py
 pycm/pycm_curve.py
 pycm/pycm_distance.py
 pycm/pycm_error.py
 pycm/pycm_handler.py
 pycm/pycm_interpret.py
+pycm/pycm_multilabel_cm.py
 pycm/pycm_obj.py
 pycm/pycm_output.py
 pycm/pycm_overall_func.py
 pycm/pycm_param.py
 pycm/pycm_profile.py
 pycm/pycm_test.py
 pycm/pycm_util.py
```

### Comparing `pycm-3.9/setup.py` & `pycm-4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,37 +32,36 @@
    data scientists that need a broad array of metrics for predictive models
    and an accurate evaluation of large variety of classifiers.'''
 
 
 setup(
     name='pycm',
     packages=['pycm'],
-    version='3.9',
+    version='4.0',
     description='Multi-class confusion matrix library in Python',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     author='PyCM Development Team',
     author_email='info@pycm.io',
     url='https://github.com/sepandhaghighi/pycm',
-    download_url='https://github.com/sepandhaghighi/pycm/tarball/v3.9',
+    download_url='https://github.com/sepandhaghighi/pycm/tarball/v4.0',
     keywords="confusion-matrix python3 python machine_learning ML",
     project_urls={
         'Webpage': 'https://www.pycm.io',
         'Source': 'https://github.com/sepandhaghighi/pycm',
         'Discord': 'https://discord.com/invite/zqpU2b3J3f',
     },
     install_requires=get_requires(),
-    python_requires='>=3.5',
+    python_requires='>=3.6',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Intended Audience :: Developers',
```

