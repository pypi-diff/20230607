# Comparing `tmp/petab_MS-0.1.21.tar.gz` & `tmp/petab_MS-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/petab_MS-0.1.21.tar", last modified: Tue Mar 29 12:40:19 2022, max compression
+gzip compressed data, was "petab_MS-0.1.22.tar", last modified: Wed Jun  7 13:47:21 2023, max compression
```

## Comparing `petab_MS-0.1.21.tar` & `petab_MS-0.1.22.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 emad      (1000) emad      (1000)        0 2022-03-29 12:40:19.000000 petab_MS-0.1.21/
--rw-r--r--   0 emad      (1000) emad      (1000)       32 2021-08-26 13:43:23.000000 petab_MS-0.1.21/MANIFEST.in
--rw-r--r--   0 emad      (1000) emad      (1000)     2471 2022-03-29 12:40:19.000000 petab_MS-0.1.21/PKG-INFO
--rw-rw-r--   0 emad      (1000) emad      (1000)     1702 2021-11-15 08:56:51.000000 petab_MS-0.1.21/README.md
-drwxr-xr-x   0 emad      (1000) emad      (1000)        0 2022-03-29 12:40:19.000000 petab_MS-0.1.21/petab_MS/
--rw-r--r--   0 emad      (1000) emad      (1000)     4663 2022-01-19 15:46:13.000000 petab_MS-0.1.21/petab_MS/C.py
--rw-r--r--   0 emad      (1000) emad      (1000)     1143 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/__init__.py
--rw-r--r--   0 emad      (1000) emad      (1000)    12936 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/calculate.py
--rw-r--r--   0 emad      (1000) emad      (1000)     2664 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/composite_problem.py
--rw-r--r--   0 emad      (1000) emad      (1000)     3038 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/conditions.py
--rw-r--r--   0 emad      (1000) emad      (1000)    11853 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/core.py
--rw-r--r--   0 emad      (1000) emad      (1000)       55 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/format_version.py
--rw-r--r--   0 emad      (1000) emad      (1000)    32352 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/lint.py
--rw-r--r--   0 emad      (1000) emad      (1000)    14159 2022-02-15 12:50:20.000000 petab_MS-0.1.21/petab_MS/measurements.py
--rw-r--r--   0 emad      (1000) emad      (1000)     1131 2022-01-19 16:09:24.000000 petab_MS-0.1.21/petab_MS/obcetive_function.py
--rw-r--r--   0 emad      (1000) emad      (1000)     5710 2022-01-19 15:46:13.000000 petab_MS-0.1.21/petab_MS/observables.py
--rw-r--r--   0 emad      (1000) emad      (1000)    25388 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/parameter_mapping.py
--rw-r--r--   0 emad      (1000) emad      (1000)    16558 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/parameters.py
--rwxr-xr-x   0 emad      (1000) emad      (1000)     6194 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/petablint.py
--rw-r--r--   0 emad      (1000) emad      (1000)    27232 2022-01-19 16:14:37.000000 petab_MS-0.1.21/petab_MS/problem.py
--rw-r--r--   0 emad      (1000) emad      (1000)     3466 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/sampling.py
--rw-r--r--   0 emad      (1000) emad      (1000)    14938 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/sbml.py
--rw-r--r--   0 emad      (1000) emad      (1000)     8559 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/simulate.py
--rw-r--r--   0 emad      (1000) emad      (1000)       51 2022-03-29 12:39:06.000000 petab_MS-0.1.21/petab_MS/version.py
-drwxr-xr-x   0 emad      (1000) emad      (1000)        0 2022-03-29 12:40:19.000000 petab_MS-0.1.21/petab_MS/visualize/
--rw-r--r--   0 emad      (1000) emad      (1000)      816 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/visualize/__init__.py
--rw-r--r--   0 emad      (1000) emad      (1000)     3109 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/visualize/data_overview.py
--rw-r--r--   0 emad      (1000) emad      (1000)    40808 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/visualize/helper_functions.py
--rw-r--r--   0 emad      (1000) emad      (1000)    21667 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/visualize/plot_data_and_simulation.py
--rw-r--r--   0 emad      (1000) emad      (1000)    13665 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/visualize/plotter.py
--rw-r--r--   0 emad      (1000) emad      (1000)    35811 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/visualize/plotting.py
--rw-r--r--   0 emad      (1000) emad      (1000)     7040 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/visualize/plotting_config.py
--rw-r--r--   0 emad      (1000) emad      (1000)     7927 2021-11-15 08:56:51.000000 petab_MS-0.1.21/petab_MS/yaml.py
-drwxr-xr-x   0 emad      (1000) emad      (1000)        0 2022-03-29 12:40:19.000000 petab_MS-0.1.21/petab_MS.egg-info/
--rw-r--r--   0 emad      (1000) emad      (1000)     2471 2022-03-29 12:40:19.000000 petab_MS-0.1.21/petab_MS.egg-info/PKG-INFO
--rw-r--r--   0 emad      (1000) emad      (1000)      917 2022-03-29 12:40:19.000000 petab_MS-0.1.21/petab_MS.egg-info/SOURCES.txt
--rw-r--r--   0 emad      (1000) emad      (1000)        1 2022-03-29 12:40:19.000000 petab_MS-0.1.21/petab_MS.egg-info/dependency_links.txt
--rw-r--r--   0 emad      (1000) emad      (1000)       52 2022-03-29 12:40:19.000000 petab_MS-0.1.21/petab_MS.egg-info/entry_points.txt
--rw-r--r--   0 emad      (1000) emad      (1000)      331 2022-03-29 12:40:19.000000 petab_MS-0.1.21/petab_MS.egg-info/requires.txt
--rw-r--r--   0 emad      (1000) emad      (1000)        9 2022-03-29 12:40:19.000000 petab_MS-0.1.21/petab_MS.egg-info/top_level.txt
--rw-r--r--   0 emad      (1000) emad      (1000)       38 2022-03-29 12:40:19.000000 petab_MS-0.1.21/setup.cfg
--rw-rw-r--   0 emad      (1000) emad      (1000)     2744 2021-11-15 08:56:51.000000 petab_MS-0.1.21/setup.py
+drwxrwxr-x   0 emad      (1000) emad      (1000)        0 2023-06-07 13:47:21.186827 petab_MS-0.1.22/
+-rw-rw-r--   0 emad      (1000) emad      (1000)     1081 2022-12-21 16:51:40.000000 petab_MS-0.1.22/LICENSE
+-rw-rw-r--   0 emad      (1000) emad      (1000)       32 2022-12-21 16:51:40.000000 petab_MS-0.1.22/MANIFEST.in
+-rw-rw-r--   0 emad      (1000) emad      (1000)     2878 2023-06-07 13:47:21.186827 petab_MS-0.1.22/PKG-INFO
+-rw-rw-r--   0 emad      (1000) emad      (1000)     1708 2023-06-07 12:47:21.000000 petab_MS-0.1.22/README.md
+drwxrwxr-x   0 emad      (1000) emad      (1000)        0 2023-06-07 13:47:21.186827 petab_MS-0.1.22/petab_MS/
+-rw-rw-r--   0 emad      (1000) emad      (1000)     4663 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/C.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)     1143 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/__init__.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    12936 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/calculate.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)     2664 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/composite_problem.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)     3038 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/conditions.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    11859 2023-06-07 12:39:46.000000 petab_MS-0.1.22/petab_MS/core.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)       55 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/format_version.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    32352 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/lint.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    14159 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/measurements.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)     1131 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/obcetive_function.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)     5710 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/observables.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    25388 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/parameter_mapping.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    16558 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/parameters.py
+-rwxrwxr-x   0 emad      (1000) emad      (1000)     6194 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/petablint.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    27232 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/problem.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)     3466 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/sampling.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    14938 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/sbml.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)     8559 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/simulate.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)       51 2023-06-07 12:42:18.000000 petab_MS-0.1.22/petab_MS/version.py
+drwxrwxr-x   0 emad      (1000) emad      (1000)        0 2023-06-07 13:47:21.186827 petab_MS-0.1.22/petab_MS/visualize/
+-rw-rw-r--   0 emad      (1000) emad      (1000)      816 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/visualize/__init__.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)     3109 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/visualize/data_overview.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    40808 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/visualize/helper_functions.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    21667 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/visualize/plot_data_and_simulation.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    13665 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/visualize/plotter.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)    35811 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/visualize/plotting.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)     7040 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/visualize/plotting_config.py
+-rw-rw-r--   0 emad      (1000) emad      (1000)     7927 2023-06-07 12:38:32.000000 petab_MS-0.1.22/petab_MS/yaml.py
+drwxrwxr-x   0 emad      (1000) emad      (1000)        0 2023-06-07 13:47:21.186827 petab_MS-0.1.22/petab_MS.egg-info/
+-rw-rw-r--   0 emad      (1000) emad      (1000)     2878 2023-06-07 13:47:21.000000 petab_MS-0.1.22/petab_MS.egg-info/PKG-INFO
+-rw-rw-r--   0 emad      (1000) emad      (1000)      950 2023-06-07 13:47:21.000000 petab_MS-0.1.22/petab_MS.egg-info/SOURCES.txt
+-rw-rw-r--   0 emad      (1000) emad      (1000)        1 2023-06-07 13:47:21.000000 petab_MS-0.1.22/petab_MS.egg-info/dependency_links.txt
+-rw-rw-r--   0 emad      (1000) emad      (1000)       51 2023-06-07 13:47:21.000000 petab_MS-0.1.22/petab_MS.egg-info/entry_points.txt
+-rw-rw-r--   0 emad      (1000) emad      (1000)      331 2023-06-07 13:47:21.000000 petab_MS-0.1.22/petab_MS.egg-info/requires.txt
+-rw-rw-r--   0 emad      (1000) emad      (1000)        9 2023-06-07 13:47:21.000000 petab_MS-0.1.22/petab_MS.egg-info/top_level.txt
+-rw-rw-r--   0 emad      (1000) emad      (1000)      386 2023-06-07 13:13:15.000000 petab_MS-0.1.22/pyproject.toml
+-rw-rw-r--   0 emad      (1000) emad      (1000)     1817 2023-06-07 13:47:21.186827 petab_MS-0.1.22/setup.cfg
+-rw-rw-r--   0 emad      (1000) emad      (1000)     2748 2023-06-07 13:02:38.000000 petab_MS-0.1.22/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `petab_MS-0.1.21/README.md` & `petab_MS-0.1.22/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![CI](https://github.com/EmadAlamoudi/libpetab-python-MS/actions/workflows/ci_tests.yml/badge.svg?branch=master)](https://github.com/EmadAlamoudi/libpetab-python-MS/actions/workflows/ci_tests.yml)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/fd7dd5cee68e449983be5c43f230c7f3)](https://www.codacy.com/gh/EmadAlamoudi/libpetab-python-MS)
 [![codecov](https://codecov.io/gh/EmadAlamoudi/libpetab-python-MS/branch/master/graph/badge.svg)](https://codecov.io/gh/EmadAlamoudi/libpetab-python-MS)
-[![PyPI version](https://badge.fury.io/py/petab.svg)](https://badge.fury.io/py/petab)
+[![PyPI version](https://badge.fury.io/py/petab-ms.svg)](https://badge.fury.io/py/petab-ms)
 
 # petab_MS - a Python package for handling PEtab files for multiscale systems
 
 PEtab_MS is an extension of PEtab for multiscale systems. [PEtab](https://petab.readthedocs.io/) is a data format for specifying
 parameter estimation problems in systems biology. This repository provides
 the `petab` Python package for reading, writing and validating PEtab files.
```

### Comparing `petab_MS-0.1.21/petab_MS/C.py` & `petab_MS-0.1.22/petab_MS/C.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/__init__.py` & `petab_MS-0.1.22/petab_MS/__init__.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/calculate.py` & `petab_MS-0.1.22/petab_MS/calculate.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/composite_problem.py` & `petab_MS-0.1.22/petab_MS/composite_problem.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/conditions.py` & `petab_MS-0.1.22/petab_MS/conditions.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/core.py` & `petab_MS-0.1.22/petab_MS/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
     df = pd.DataFrame()
 
     for tmp_df in tables:
         # load from file, if necessary
         if isinstance(tmp_df, str):
             tmp_df = file_parser(tmp_df)
         if not isinstance(tmp_df, dict):
-            df = df.append(tmp_df, sort=False, ignore_index=isinstance(
+            df = pd.concat([df, tmp_df], sort=False, ignore_index=isinstance(
                 tmp_df.index, pd.RangeIndex))
         else:
             df = tmp_df
     return df
 
 
 def to_float_if_float(x: Any) -> Any:
```

### Comparing `petab_MS-0.1.21/petab_MS/lint.py` & `petab_MS-0.1.22/petab_MS/lint.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/measurements.py` & `petab_MS-0.1.22/petab_MS/measurements.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/obcetive_function.py` & `petab_MS-0.1.22/petab_MS/obcetive_function.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/observables.py` & `petab_MS-0.1.22/petab_MS/observables.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/parameter_mapping.py` & `petab_MS-0.1.22/petab_MS/parameter_mapping.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/parameters.py` & `petab_MS-0.1.22/petab_MS/parameters.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/petablint.py` & `petab_MS-0.1.22/petab_MS/petablint.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/problem.py` & `petab_MS-0.1.22/petab_MS/problem.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/sampling.py` & `petab_MS-0.1.22/petab_MS/sampling.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/sbml.py` & `petab_MS-0.1.22/petab_MS/sbml.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/simulate.py` & `petab_MS-0.1.22/petab_MS/simulate.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/visualize/__init__.py` & `petab_MS-0.1.22/petab_MS/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/visualize/data_overview.py` & `petab_MS-0.1.22/petab_MS/visualize/data_overview.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/visualize/helper_functions.py` & `petab_MS-0.1.22/petab_MS/visualize/helper_functions.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/visualize/plot_data_and_simulation.py` & `petab_MS-0.1.22/petab_MS/visualize/plot_data_and_simulation.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/visualize/plotter.py` & `petab_MS-0.1.22/petab_MS/visualize/plotter.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/visualize/plotting.py` & `petab_MS-0.1.22/petab_MS/visualize/plotting.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/visualize/plotting_config.py` & `petab_MS-0.1.22/petab_MS/visualize/plotting_config.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS/yaml.py` & `petab_MS-0.1.22/petab_MS/yaml.py`

 * *Files identical despite different names*

### Comparing `petab_MS-0.1.21/petab_MS.egg-info/SOURCES.txt` & `petab_MS-0.1.22/petab_MS.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
+setup.cfg
 setup.py
 petab_MS/C.py
 petab_MS/__init__.py
 petab_MS/calculate.py
 petab_MS/composite_problem.py
 petab_MS/conditions.py
 petab_MS/core.py
```

### Comparing `petab_MS-0.1.21/setup.py` & `petab_MS-0.1.22/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 def read(fname):
     """Read a file."""
     return open(fname).read()
 
 
 def absolute_links(txt):
-    """Replace relative petab github links by absolute links."""
+    """Replace relative petab-MS github links by absolute links."""
 
     raw_base = "(https://raw.githubusercontent.com/"\
-               "EmadAlamoudi/libpetab-python-MS/master/"
-    embedded_base = "(https://github.com/EmadAlamoudi/libpetab-python-MS/"\
+               "fitmulticell/libpetab-python-MS/"
+    embedded_base = "(https://gitlab.com/fitmulticell/libpetab-python-MS/"\
                     "tree/master/"
     # iterate over links
     for var in re.findall(r'\[.*?\]\((?!http).*?\)', txt):
         if re.match(r'.*?.(png|svg)\)', var):
             # link to raw file
             rep = var.replace("(", raw_base)
         else:
@@ -44,23 +44,23 @@
     ]
 }
 
 # project metadata
 # noinspection PyUnresolvedReferences
 setup(name='petab_MS',
       version=__version__,
-      description='Parameter estimation tabular data for MS',
+      description='Parameter estimation tabular data for multi-scale models',
       long_description=absolute_links(read('README.md')),
       long_description_content_type="text/markdown",
-      author='The PEtab developers',
-      author_email='daniel.weindl@helmholtz-muenchen.de',
-      url='https://github.com/EmadAlamoudi/libpetab-python-MS',
+      author='The PEtab-MS developers',
+      author_email='EmadAlamoudi@uni-bonn.de',
+      url='https://gitlab.com/fitmulticell/libpetab-python-MS',
       packages=find_packages(exclude=['doc*', 'test*']),
       install_requires=['numpy>=1.15.1',
-                        'pandas>=1.2.0',
+                        'pandas>=2.0.1',
                         'matplotlib>=2.2.3',
                         'python-libsbml>=5.17.0',
                         'sympy',
                         'colorama',
                         'seaborn',
                         'pyyaml',
                         'jsonschema',
```

