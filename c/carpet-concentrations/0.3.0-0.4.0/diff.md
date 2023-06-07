# Comparing `tmp/carpet_concentrations-0.3.0.tar.gz` & `tmp/carpet_concentrations-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carpet_concentrations-0.3.0.tar", max compression
+gzip compressed data, was "carpet_concentrations-0.4.0.tar", max compression
```

## Comparing `carpet_concentrations-0.3.0.tar` & `carpet_concentrations-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1524 2023-05-22 05:41:30.506818 carpet_concentrations-0.3.0/LICENSE
--rw-r--r--   0        0        0     2096 2023-05-27 04:14:21.821420 carpet_concentrations-0.3.0/README.md
--rw-r--r--   0        0        0     3800 2023-05-27 05:21:26.824196 carpet_concentrations-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      199 2023-05-27 02:26:43.018245 carpet_concentrations-0.3.0/src/carpet_concentrations/__init__.py
--rw-r--r--   0        0        0     2975 2023-05-27 02:26:43.018245 carpet_concentrations-0.3.0/src/carpet_concentrations/attrs_utils.py
--rw-r--r--   0        0        0     2812 2023-05-27 02:26:43.018245 carpet_concentrations-0.3.0/src/carpet_concentrations/exceptions.py
--rw-r--r--   0        0        0      139 2023-05-27 02:26:43.018245 carpet_concentrations-0.3.0/src/carpet_concentrations/gridders/__init__.py
--rw-r--r--   0        0        0     6629 2023-05-27 02:26:43.022245 carpet_concentrations-0.3.0/src/carpet_concentrations/gridders/latitude_seasonality_gridder.py
--rw-r--r--   0        0        0       94 2023-05-27 02:26:43.022245 carpet_concentrations-0.3.0/src/carpet_concentrations/input4MIPs/__init__.py
--rw-r--r--   0        0        0    18464 2023-05-27 05:15:41.263121 carpet_concentrations-0.3.0/src/carpet_concentrations/input4MIPs/dataset.py
--rw-r--r--   0        0        0     1592 2023-05-27 02:26:43.022245 carpet_concentrations-0.3.0/src/carpet_concentrations/input4MIPs/metadata_options.py
--rw-r--r--   0        0        0        0 2023-05-22 05:41:30.510818 carpet_concentrations-0.3.0/src/carpet_concentrations/py.typed
--rw-r--r--   0        0        0     1429 2023-05-27 02:26:43.022245 carpet_concentrations-0.3.0/src/carpet_concentrations/testing.py
--rw-r--r--   0        0        0     4948 2023-05-27 02:26:43.022245 carpet_concentrations-0.3.0/src/carpet_concentrations/time.py
--rw-r--r--   0        0        0     1334 2023-05-27 05:15:41.263121 carpet_concentrations-0.3.0/src/carpet_concentrations/xarray_pint_utils.py
--rw-r--r--   0        0        0     3554 2023-05-27 05:15:41.263121 carpet_concentrations-0.3.0/src/carpet_concentrations/xarray_utils.py
--rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 carpet_concentrations-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2023-06-07 05:02:12.405315 carpet_concentrations-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2093 2023-06-07 05:02:12.405315 carpet_concentrations-0.4.0/README.md
+-rw-r--r--   0        0        0     4466 2023-06-07 05:50:26.459595 carpet_concentrations-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/__init__.py
+-rw-r--r--   0        0        0     2975 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/attrs_utils.py
+-rw-r--r--   0        0        0     2812 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/exceptions.py
+-rw-r--r--   0        0        0      139 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/gridders/__init__.py
+-rw-r--r--   0        0        0     6629 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/gridders/latitude_seasonality_gridder.py
+-rw-r--r--   0        0        0       94 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/input4MIPs/__init__.py
+-rw-r--r--   0        0        0    18464 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/input4MIPs/dataset.py
+-rw-r--r--   0        0        0     1592 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/input4MIPs/metadata_options.py
+-rw-r--r--   0        0        0        0 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/py.typed
+-rw-r--r--   0        0        0     1429 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/testing.py
+-rw-r--r--   0        0        0     4948 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/time.py
+-rw-r--r--   0        0        0     1334 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/xarray_pint_utils.py
+-rw-r--r--   0        0        0     3554 2023-06-07 05:02:12.409315 carpet_concentrations-0.4.0/src/carpet_concentrations/xarray_utils.py
+-rw-r--r--   0        0        0     3438 1970-01-01 00:00:00.000000 carpet_concentrations-0.4.0/PKG-INFO
```

### Comparing `carpet_concentrations-0.3.0/LICENSE` & `carpet_concentrations-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.3.0/README.md` & `carpet_concentrations-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,12 +55,12 @@
 You can read the instructions out and run the commands by hand if you wish,
 but we generally discourage this because it can be error prone.
 In order to create your environment, run `make virtual-environment`.
 
 If there are any issues, the messages from the `Makefile` should guide you
 through. If not, please raise an issue in the [issue tracker][issue_tracker].
 
-For the rest of our developer docs, please see {ref}`development-reference`.
+For the rest of our developer docs, please see [](development-reference).
 
 [issue_tracker]: https://gitlab.com/climate-resource/carpet-concentrations/issues
 
 <!--- sec-end-installation-dev -->
```

### Comparing `carpet_concentrations-0.3.0/pyproject.toml` & `carpet_concentrations-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.coverage.run]
 source = ["src"]
 branch = true
 
 [tool.poetry]
 name = "carpet-concentrations"
-version = "0.3.0"
+version = "0.4.0"
 description = "Core tools for the development of greenhouse gas concentration input files (i.e. flying carpets)."
 authors = ["Zebedee Nicholls <zebedee.nicholls@climate-resource.com>"]
 readme = "README.md"
 packages = [{include = "carpet_concentrations", from = "src"}]
+license = "BSD-3-Clause"
 
 [tool.commitizen]
-version = "0.3.0"
+version = "0.4.0"
 version_files = ["pyproject.toml:^version"]
 tag_format = "v$version"
 major_version_zero = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
@@ -56,14 +57,15 @@
 coverage = "^7.2.0"
 black = "23.3.0"
 blackdoc = "0.3.8"
 commitizen = "^3.1.1"
 mypy = "^1.2.0"
 ruff = "0.0.264"
 pre-commit = "^3.3.1"
+liccheck = "^0.9.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.report]
 fail_under = 95
@@ -104,15 +106,14 @@
     "F",  # pyflakes
     "I",  # isort
     "D",  # pydocstyle
     "PL",  # pylint
     "TRY",  # tryceratops
     "NPY",  # numpy rules
     "RUF",  # ruff specifics
-    "ERA",  # eradicate old commented out code
     "UP",  # pyupgrade
     "S",  # flake8-bandit
     # xarray repo, no PD
 ]
 unfixable = [
     "PD002",  # Disable autofix for inplace as this often introduces bugs
 ]
@@ -128,20 +129,50 @@
     "D",  # Documentation not needed in tests
     "S101",  # S101 Use of `assert` detected
     "PLR2004" # Magic value used in comparison
 ]
 "docs/source/notebooks/*" = [
     "D100",  # Missing docstring at the top of file
     "E402",  # Module level import not at top of file
-    "ERA001",  # False positive while parsing jupytext header
     "S101",  # Use of `assert` detected
 ]
 "scripts/*" = [
     "S101" # S101 Use of `assert` detected
 ]
 "*.pyi" = ["D100", "D101", "D102", "PL"]
 
 [tool.ruff.isort]
 known-first-party = ["src"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
+
+[tool.liccheck]
+authorized_licenses = [
+    "bsd",
+    "bsd license",
+    "BSD 3-Clause",
+    "CC0",
+    "apache",
+    "apache 2.0",
+    "apache software",
+    "apache software license",
+    "Apache License, Version 2.0",
+    "gnu lgpl",
+    "lgpl with exceptions or zpl",
+    "LGPLv2+",
+    "GNU Lesser General Public License v2 (LGPLv2)",
+    "GNU Lesser General Public License v2 or later (LGPLv2+)",
+    "gpl v3",
+    "gplv3",
+    "Historical Permission Notice and Disclaimer (HPND)",
+    "isc license",
+    "isc license (iscl)",
+    "mit",
+    "mit license",
+    "Mozilla Public License 2.0 (MPL 2.0)",
+    "python software foundation",
+    "python software foundation license",
+    "zpl 2.1",
+]
+unauthorized_licenses = [
+]
```

### Comparing `carpet_concentrations-0.3.0/src/carpet_concentrations/attrs_utils.py` & `carpet_concentrations-0.4.0/src/carpet_concentrations/attrs_utils.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.3.0/src/carpet_concentrations/exceptions.py` & `carpet_concentrations-0.4.0/src/carpet_concentrations/exceptions.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.3.0/src/carpet_concentrations/gridders/latitude_seasonality_gridder.py` & `carpet_concentrations-0.4.0/src/carpet_concentrations/gridders/latitude_seasonality_gridder.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.3.0/src/carpet_concentrations/input4MIPs/dataset.py` & `carpet_concentrations-0.4.0/src/carpet_concentrations/input4MIPs/dataset.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.3.0/src/carpet_concentrations/input4MIPs/metadata_options.py` & `carpet_concentrations-0.4.0/src/carpet_concentrations/input4MIPs/metadata_options.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.3.0/src/carpet_concentrations/testing.py` & `carpet_concentrations-0.4.0/src/carpet_concentrations/testing.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.3.0/src/carpet_concentrations/time.py` & `carpet_concentrations-0.4.0/src/carpet_concentrations/time.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.3.0/src/carpet_concentrations/xarray_pint_utils.py` & `carpet_concentrations-0.4.0/src/carpet_concentrations/xarray_pint_utils.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.3.0/src/carpet_concentrations/xarray_utils.py` & `carpet_concentrations-0.4.0/src/carpet_concentrations/xarray_utils.py`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.3.0/PKG-INFO` & `carpet_concentrations-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: carpet-concentrations
-Version: 0.3.0
+Version: 0.4.0
 Summary: Core tools for the development of greenhouse gas concentration input files (i.e. flying carpets).
+License: BSD-3-Clause
 Author: Zebedee Nicholls
 Author-email: zebedee.nicholls@climate-resource.com
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cfxarray
 Provides-Extra: netcdf
 Provides-Extra: notebooks
@@ -85,13 +87,13 @@
 You can read the instructions out and run the commands by hand if you wish,
 but we generally discourage this because it can be error prone.
 In order to create your environment, run `make virtual-environment`.
 
 If there are any issues, the messages from the `Makefile` should guide you
 through. If not, please raise an issue in the [issue tracker][issue_tracker].
 
-For the rest of our developer docs, please see {ref}`development-reference`.
+For the rest of our developer docs, please see [](development-reference).
 
 [issue_tracker]: https://gitlab.com/climate-resource/carpet-concentrations/issues
 
 <!--- sec-end-installation-dev -->
```

