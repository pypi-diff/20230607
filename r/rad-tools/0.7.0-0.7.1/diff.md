# Comparing `tmp/rad-tools-0.7.0.tar.gz` & `tmp/rad-tools-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.7.0.tar", last modified: Tue Jun  6 00:13:32 2023, max compression
+gzip compressed data, was "rad-tools-0.7.1.tar", last modified: Wed Jun  7 18:53:52 2023, max compression
```

## Comparing `rad-tools-0.7.0.tar` & `rad-tools-0.7.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.507400 rad-tools-0.7.0/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.0/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-06 00:13:32.506784 rad-tools-0.7.0/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-05 23:32:40.000000 rad-tools-0.7.0/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.455300 rad-tools-0.7.0/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-06 00:13:32.000000 rad-tools-0.7.0/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1203 2023-06-06 00:13:32.000000 rad-tools-0.7.0/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-06 00:13:32.000000 rad-tools-0.7.0/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-06 00:13:32.000000 rad-tools-0.7.0/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-06 00:13:32.000000 rad-tools-0.7.0/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.457785 rad-tools-0.7.0/radtools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      624 2023-06-06 00:13:06.000000 rad-tools-0.7.0/radtools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.467176 rad-tools-0.7.0/radtools/crystal/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      292 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     6865 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/atom.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/atom_types.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    87419 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/bravais_lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     8896 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/crystal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/identify.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/crystal/lattice.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.473734 rad-tools-0.7.0/radtools/dos/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/dos/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    21701 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/dos/dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    22428 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/dos/pdos.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.480558 rad-tools-0.7.0/radtools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-06 00:13:06.000000 rad-tools-0.7.0/radtools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    45538 2023-06-06 00:13:06.000000 rad-tools-0.7.0/radtools/exchange/hamiltonian.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    12326 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/exchange/parameter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.483348 rad-tools-0.7.0/radtools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5458 2023-06-06 00:13:06.000000 rad-tools-0.7.0/radtools/io/tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.485986 rad-tools-0.7.0/radtools/kpoints/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      615 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/kpoints/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4280 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/kpoints/high_symmetry_point.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3625 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/kpoints/kpoints.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-06 00:13:06.000000 rad-tools-0.7.0/radtools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.492839 rad-tools-0.7.0/radtools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/extract_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/identify_wannier_centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4695 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/make_template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    13280 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/plot_dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9920 2023-06-05 23:32:40.000000 rad-tools-0.7.0/radtools/score/plot_tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-06 00:13:32.505099 rad-tools-0.7.0/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.0/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.0/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-05 23:32:40.000000 rad-tools-0.7.0/scripts/rad-extract-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-05 23:32:40.000000 rad-tools-0.7.0/scripts/rad-identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-05 23:32:40.000000 rad-tools-0.7.0/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-05 23:32:40.000000 rad-tools-0.7.0/scripts/rad-plot-dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-05 23:32:40.000000 rad-tools-0.7.0/scripts/rad-plot-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-06 00:13:32.507590 rad-tools-0.7.0/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-05 23:35:15.000000 rad-tools-0.7.0/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.882757 rad-tools-0.7.1/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.1/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-07 18:53:52.882155 rad-tools-0.7.1/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-06 15:39:42.000000 rad-tools-0.7.1/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.837395 rad-tools-0.7.1/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-07 18:53:52.000000 rad-tools-0.7.1/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1203 2023-06-07 18:53:52.000000 rad-tools-0.7.1/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-07 18:53:52.000000 rad-tools-0.7.1/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-07 18:53:52.000000 rad-tools-0.7.1/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-07 18:53:52.000000 rad-tools-0.7.1/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.839613 rad-tools-0.7.1/radtools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      624 2023-06-07 18:48:20.000000 rad-tools-0.7.1/radtools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.854510 rad-tools-0.7.1/radtools/crystal/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      292 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/crystal/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     6862 2023-06-07 15:53:48.000000 rad-tools-0.7.1/radtools/crystal/atom.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/crystal/atom_types.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-07 16:07:49.000000 rad-tools-0.7.1/radtools/crystal/bravais_lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    11380 2023-06-07 16:00:50.000000 rad-tools-0.7.1/radtools/crystal/crystal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/crystal/identify.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/crystal/lattice.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.858186 rad-tools-0.7.1/radtools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    21701 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    22428 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/dos/pdos.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.861572 rad-tools-0.7.1/radtools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    50113 2023-06-07 18:39:47.000000 rad-tools-0.7.1/radtools/exchange/hamiltonian.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-06 17:44:02.000000 rad-tools-0.7.1/radtools/exchange/parameter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.863700 rad-tools-0.7.1/radtools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-07 14:38:12.000000 rad-tools-0.7.1/radtools/io/tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.869382 rad-tools-0.7.1/radtools/kpoints/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      615 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/kpoints/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4280 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/kpoints/high_symmetry_point.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3625 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/kpoints/kpoints.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.873927 rad-tools-0.7.1/radtools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4695 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    13280 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-07 14:19:09.000000 rad-tools-0.7.1/radtools/score/plot_tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.880721 rad-tools-0.7.1/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.1/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.1/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-06 15:39:43.000000 rad-tools-0.7.1/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-06 15:39:43.000000 rad-tools-0.7.1/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-06 15:39:43.000000 rad-tools-0.7.1/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-06 15:39:43.000000 rad-tools-0.7.1/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-06 15:39:43.000000 rad-tools-0.7.1/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-07 18:53:52.883702 rad-tools-0.7.1/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-06 15:39:43.000000 rad-tools-0.7.1/setup.py
```

### Comparing `rad-tools-0.7.0/LICENSE.txt` & `rad-tools-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/PKG-INFO` & `rad-tools-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.0
+Version: 0.7.1
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.0/README.rst` & `rad-tools-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.7.1/rad_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.0
+Version: 0.7.1
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.0/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.7.1/rad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/__init__.py` & `rad-tools-0.7.1/radtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""
 All tools from the package.
 
 
 |version|
 """
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 from . import crystal, dos, exchange, io, kpoints, score
 from .crystal import *
 from .dos import *
 from .exchange import *
 from .io import *
 from .kpoints import *
```

### Comparing `rad-tools-0.7.0/radtools/crystal/atom.py` & `rad-tools-0.7.1/radtools/crystal/atom.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 class Atom:
     r"""
     Atom class.
 
     Notes
     -----
-    "==" (and "!=") operation compare two atoms based on their literals and indexes.
+    "==" (and "!=") operation compare two atoms based on their names and indexes.
     If index of one atom is not define, then comparison raises ``ValueError``.
     For the check of the atom type use :py:attr:`Atom.type`.
-    In most cases :py:attr:`Atom.literal` = :py:attr:`Atom.type`.
+    In most cases :py:attr:`Atom.name` = :py:attr:`Atom.type`.
 
     Parameters
     ----------
-    literal : str, default X
+    name : str, default X
         Name of the atom.
     position : (3,) |array_like|_, default [0,0,0]
         Position of the atom in absolute coordinates.
     spin : float, optional
         Spin of the atom.
     spin_vector : (3,) |array_like|_, optional
         Classical spin vector of the atom.
@@ -30,102 +30,103 @@
         Only the direction matters, for the value use ``spin``.
     magmom : (3,) |array_like|_, optional
         Magnetic moment of the atom.
     charge : float, optional
         Charge of the atom.
     index : int, optional
         Custom index of an atom, used differently in different scenarios.
-        Meant to be unique, when an atom belongs to some group
+        Combination of :py:attr:`.name` and :py:attr:`.index`
+        is meant to be unique, when an atom belongs to some group
         (i.e. to :py:class:`.Crystal` or :py:class:`.ExchangeHamiltonian`).
 
     Attributes
     ----------
-    literal : str
+    name : str
     type : str
     index : int
     position : (3,) :numpy:`ndarray`
         Position of the atom in absolute coordinates.
     spin : (3,) :numpy:`ndarray`
     magmom : (3,) :numpy:`ndarray`
     charge : float
     """
 
     def __init__(
         self,
-        literal="X",
+        name="X",
         position=None,
         spin=None,
         spin_vector=None,
         magmom=None,
         charge=None,
         index=None,
     ) -> None:
-        self._literal = "X"
+        self._name = "X"
         self._index = None
         self._type = None
         if position is None:
             position = (0, 0, 0)
         self.position = np.array(position)
         self._spin = None
         self._spin_vector = None
         self._magmom = None
         self._charge = None
 
-        self.literal = literal
+        self.name = name
         if spin is not None:
             self.spin = spin
         if spin_vector is not None:
             self.spin_vector = spin_vector
         if magmom is not None:
             self.magmom = magmom
         if charge is not None:
             self.charge = charge
         if index is not None:
             self.index = index
 
     def __str__(self):
-        return self.literal
+        return self.name
 
     def __format__(self, format_spec):
         return format(str(self), format_spec)
 
     # ==
     def __eq__(self, other) -> bool:
         if not isinstance(other, Atom):
             raise TypeError(
                 f"TypeError: unsupported operand type(s) "
-                + f"for =: '{other.__class__.__name__}' and 'Atom'"
+                + f"for ==: '{other.__class__.__name__}' and 'Atom'"
             )
-        return self.literal == other.literal and self.index == other.index
+        return self.name == other.name and self.index == other.index
 
     def __hash__(self):
-        return hash(str(self.literal) + str(self.index))
+        return hash(str(self.name) + str(self.index))
 
     # !=
     def __neq__(self, other):
         return not self == other
 
     @property
-    def literal(self):
-        return self._literal
+    def name(self):
+        return self._name
 
-    @literal.setter
-    def literal(self, new_literal):
-        self._literal = new_literal
+    @name.setter
+    def name(self, new_name):
+        self._name = new_name
         self._type = None
 
     @property
     def type(self):
         r"""
         Type of an atom (i.e. Cr, Ni, ...).
         """
         if self._type is None:
             self._type = "X"
             for i in atom_types:
-                if i in self._literal:
+                if i in self._name:
                     self._type = i
                     break
         return self._type
 
     @property
     def index(self):
         r"""
@@ -242,12 +243,12 @@
 
     @charge.setter
     def charge(self, new_charge):
         self._charge = new_charge
 
     @property
     def fullname(self):
-        r"""Return fullname (literal + index) of an atom."""
+        r"""Return fullname (name + index) of an atom."""
         try:
-            return f"{self.literal}_{self.index}"
+            return f"{self.name}_{self.index}"
         except ValueError:
-            return self.literal
+            return self.name
```

### Comparing `rad-tools-0.7.0/radtools/crystal/atom_types.py` & `rad-tools-0.7.1/radtools/crystal/atom_types.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/crystal/bravais_lattice.py` & `rad-tools-0.7.1/radtools/crystal/bravais_lattice.py`

 * *Files 0% similar despite different names*

```diff
@@ -2512,41 +2512,41 @@
     .. [1] Setyawan, W. and Curtarolo, S., 2010.
         High-throughput electronic band structure calculations: Challenges and tools.
         Computational materials science, 49(2), pp.299-312.
     """
 
     lattice_type = lepage(*param_from_cell(cell))
 
-    # if lattice_type == "CUB":
-    #     return CUB(cell=cell)
-    # if lattice_type == "FCC":
-    #     return FCC(cell=cell)
-    # if lattice_type == "BCC":
-    #     return BCC(cell=cell)
-    # if lattice_type == "TET":
-    #     return TET(cell=cell)
-    # if lattice_type == "BCT":
-    #     return BCT(cell=cell)
-    # if lattice_type == "ORC":
-    #     return ORC(cell=cell)
-    # if lattice_type == "ORCF":
-    #     return ORCF(cell=cell)
-    # if lattice_type == "ORCC":
-    #     return ORCC(cell=cell)
-    # if lattice_type == "ORCI":
-    #     return ORCI(cell=cell)
-    # if lattice_type == "HEX":
-    #     return HEX(cell=cell)
-    # if lattice_type == "RHL":
-    #     return RHL(cell=cell)
-    # if lattice_type == "MCL":
-    #     return MCL(cell=cell)
-    # if lattice_type == "MCLC":
-    #     return MCLC(cell=cell)
-    # return TRI(cell=cell)
+    if lattice_type == "CUB":
+        return CUB(cell=cell)
+    if lattice_type == "FCC":
+        return FCC(cell=cell)
+    if lattice_type == "BCC":
+        return BCC(cell=cell)
+    if lattice_type == "TET":
+        return TET(cell=cell)
+    if lattice_type == "BCT":
+        return BCT(cell=cell)
+    if lattice_type == "ORC":
+        return ORC(cell=cell)
+    if lattice_type == "ORCF":
+        return ORCF(cell=cell)
+    if lattice_type == "ORCC":
+        return ORCC(cell=cell)
+    if lattice_type == "ORCI":
+        return ORCI(cell=cell)
+    if lattice_type == "HEX":
+        return HEX(cell=cell)
+    if lattice_type == "RHL":
+        return RHL(cell=cell)
+    if lattice_type == "MCL":
+        return MCL(cell=cell)
+    if lattice_type == "MCLC":
+        return MCLC(cell=cell)
+    return TRI(cell=cell)
     return Lattice(cell)
 
 
 def lattice_example(
     lattice=None,
 ):
     r"""
```

### Comparing `rad-tools-0.7.0/radtools/crystal/crystal.py` & `rad-tools-0.7.1/radtools/crystal/crystal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from math import sqrt
 
+from typing import Union
+
 import numpy as np
 
 from radtools.crystal.atom import Atom
 from radtools.crystal.lattice import Lattice
 from radtools.crystal.bravais_lattice import bravais_lattice_from_cell
 from radtools.routines import absolute_to_relative
 
@@ -103,25 +105,37 @@
         for atom in self:
             relative = absolute_to_relative(old_cell, atom.position)
             atom.position = relative @ self.cell
 
     def __iter__(self):
         return CrystalIterator(self)
 
-    def __contains__(self, atom):
+    def __contains__(self, atom: Union[Atom, str]):
+        if isinstance(atom, str):
+            atom = self.get_atom(atom, return_all=True)
+            if isinstance(atom, list):
+                atom = atom[0]
         return atom in self.atoms
 
     def __getitem__(self, index) -> Atom:
         return self.atoms[index]
 
     def __getattr__(self, name):
         # Fix copy/deepcopy RecursionError
         if name in ["__setstate__"]:
             raise AttributeError(name)
-        return getattr(self.lattice, name)
+        try:
+            index = None
+            if "_" in name:
+                index = int(name.split("_")[1])
+                name = name.split("_")[0]
+            atom = self.get_atom(name=name, index=index)
+            return atom
+        except ValueError:
+            return getattr(self.lattice, name)
 
     @property
     def lattice(self):
         r"""
         Lattice of the crystal.
 
         See :ref:`rad-tools_lattice` for details.
@@ -133,133 +147,179 @@
         if not isinstance(new_lattice, Lattice):
             raise TypeError(
                 "New lattice is not a lattice. " + f"Received {type(new_lattice)}."
             )
         self._lattice = new_lattice
 
     def add_atom(self, new_atom: Atom):
+        r"""
+        Add atom to the crystall.
+
+        If ``new_atom```s literal and index are the same as of some atom of the crystal,
+        then ``new_atom`` is not added.
+
+        If index of ``new_atom`` is not defined, it is set.
+
+        Parameters
+        ----------
+        new_atoms : :py:class:`.Atom`
+            New atom.
+
+        Raises
+        ------
+        TypeError
+            If ``new_atom`` is not an :py:class:`.Atom`.
+        ValueError
+            If the atom is already present in the crystal.
+        """
         if not isinstance(new_atom, Atom):
             raise TypeError("New atom is not an Atom. " + f"Received {type(new_atom)}.")
+        try:
+            i = new_atom.index
+        except ValueError:
+            new_atom.index = len(self.atoms) + 1
         if new_atom not in self.atoms:
-            try:
-                i = new_atom.index
-            except ValueError:
-                new_atom.index = len(self.atoms) + 1
             self.atoms.append(new_atom)
+        else:
+            raise ValueError("Atom is already in the crystal.")
 
-    def remove_atom(self, atom: Atom):
+    def remove_atom(self, atom: Union[Atom, str]):
         r"""
         Remove atom from the crystal.
 
+        If type(``atom``) == ``str``, then all atoms with the name ``atom`` are removed.
+
         Parameters
         ----------
-        atom : :py:class:`.Atom`
-            Atom object.
+        atom : :py:class:`.Atom` or str
+            :py:class`.Atom` object or atom`s name.
+            If name, then it has to be unique among atoms of the crystal.
         """
 
-        self.atoms.remove(atom)
+        if isinstance(atom, str):
+            atoms = self.get_atom(atom, return_all=True)
+        else:
+            atoms = [atom]
+        for atom in atoms:
+            self.atoms.remove(atom)
 
-    def get_atom(self, literal, index=None):
+    def get_atom(self, name, index=None, return_all=False):
         r"""
-        Return atom of the crystal.
-
-        Return all atoms with the same literal. If index is provided,
-        then return all atoms with literal and index.
+        Return atom object of the crystal.
 
         Notes
         -----
-        ``index`` is supposed to be a unique value,
+        :py:attr:`.index` in combination with :py:attr:`.name` is supposed to be a unique value,
         however it uniqueness is not strictly checked,
         pay attention in custom cases.
 
         Parameters
         ----------
-        literal : str
+        name : str
             Name of the atom. In general not unique.
         index : any, optional
             Index of the atom.
+        return_all : bool, default False
+            Whether to return the list of non-unique matches or raise an ``ValueError``.
 
         Returns
         -------
-        atom : :py:class:`.Atom` or list or None
-            If there is no atom in the crystal then return ``None``.
+        atom : :py:class:`.Atom` or list
             If only one atom is found, then :py:class:`.Atom` object is returned.
-            If several atoms are found then list of :py:class:`.Atom` objects is returned.
+            If several atoms are found and ``return_all`` is ``True``,
+            then list of :py:class:`.Atom` objects is returned.
+
+        Raises
+        ------
+        ValueError
+            If no match is found or the match is not unique and ``return_all`` is False.
         """
 
         atoms = []
 
         for atom in self:
-            if atom.literal == literal:
-                if index is None:
-                    atoms.append(atom)
-                elif atom.index == index:
+            if atom.name == name:
+                if index is None or atom.index == index:
                     atoms.append(atom)
         if len(atoms) == 0:
-            return None
+            raise ValueError(f"No match found for name = {name}, index = {index}")
         elif len(atoms) == 1:
             return atoms[0]
+        elif not return_all:
+            raise ValueError(
+                f"Multiple matches found for name = {name}, index = {index}"
+            )
         return atoms
 
-    def get_atom_coordinates(self, atom: Atom, R=(0, 0, 0)):
+    def get_atom_coordinates(self, atom: Union[Atom, str], R=(0, 0, 0)):
         r"""
         Getter for the atom coordinates.
 
         Parameters
         ----------
-        atom : :py:class:`.Atom`
-            Atom object.
+        atom : :py:class:`.Atom` or str
+            :py:class`.Atom` object or atom`s name.
+            If name, then it has to be unique among atoms of the crystal.
         R : (3,) |array_like|_, default (0, 0, 0)
             Radius vector of the unit cell for atom2 (i,j,k).
 
         Returns
         -------
         coordinates : 1 x 3 array
             Coordinates of atom in the cell R in absolute coordinates.
         """
 
+        if isinstance(atom, str):
+            atom = self.get_atom(atom)
+
         if atom not in self.atoms:
             raise ValueError(f"There is no {atom} in the crystal.")
 
         return np.array(R) @ self.lattice.cell + atom.position
 
-    def get_vector(self, atom1, atom2, R=(0, 0, 0)):
+    def get_vector(self, atom1: Union[Atom, str], atom2: Union[Atom, str], R=(0, 0, 0)):
         r"""
         Getter for vector between the atom1 and atom2.
 
         Parameters
         ----------
-        atom1 : :py:class:`.Atom`
-            Atom object in (0, 0, 0) unit cell.
-        atom2 : :py:class:`.Atom`
-            Atom object in R unit cell.
+        atom1 : :py:class:`.Atom` or str
+            :py:class`.Atom` object or atom`s name in (0, 0, 0) unit cell.
+            If name, then it has to be unique among atoms of the crystal.
+        atom2 : :py:class:`.Atom` or str
+            :py:class`.Atom` object or atom`s name in ``R`` unit cell.
+            If name, then it has to be unique among atoms of the crystal.
         R : (3,) |array_like|_, default (0, 0, 0)
             Radius vector of the unit cell for atom2 (i,j,k).
 
         Returns
         -------
         v : (3,) :numpy:`ndarray`
             Vector from atom1 in (0,0,0) cell to atom2 in R cell.
         """
 
-        atom1 = self.get_atom_coordinates(atom1)
-        atom2 = self.get_atom_coordinates(atom2, R)
+        coord1 = self.get_atom_coordinates(atom1)
+        coord2 = self.get_atom_coordinates(atom2, R)
 
-        return atom2 - atom1
+        return coord2 - coord1
 
-    def get_distance(self, atom1, atom2, R=(0, 0, 0)):
+    def get_distance(
+        self, atom1: Union[Atom, str], atom2: Union[Atom, str], R=(0, 0, 0)
+    ):
         r"""
         Getter for distance between the atom1 and atom2.
 
         Parameters
         ----------
-        atom1 : :py:class:`.Atom`
-            Atom object in (0, 0, 0) unit cell.
-        atom2 : :py:class:`.Atom`
-            Atom object in R unit cell.
+        atom1 : :py:class:`.Atom` or str
+            :py:class`.Atom` object or atom`s name in (0, 0, 0) unit cell.
+            If name, then it has to be unique among atoms of the crystal.
+        atom2 : :py:class:`.Atom` or str
+            :py:class`.Atom` object or atom`s name in ``R`` unit cell.
+            If name, then it has to be unique among atoms of the crystal.
         R : (3,) |array_like|_, default (0, 0, 0)
             Radius vector of the unit cell for atom2 (i,j,k).
 
         Returns
         -------
         distance : floats
             Distance between atom1 in (0,0,0) cell and atom2 in R cell.
```

### Comparing `rad-tools-0.7.0/radtools/crystal/identify.py` & `rad-tools-0.7.1/radtools/crystal/identify.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/crystal/lattice.py` & `rad-tools-0.7.1/radtools/crystal/lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/dos/dos.py` & `rad-tools-0.7.1/radtools/dos/dos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/dos/pdos.py` & `rad-tools-0.7.1/radtools/dos/pdos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/exchange/hamiltonian.py` & `rad-tools-0.7.1/radtools/exchange/hamiltonian.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import numpy as np
 
 from radtools.crystal.atom import Atom
 from radtools.crystal.crystal import Crystal
 from radtools.exchange.parameter import ExchangeParameter
 from radtools.exchange.template import ExchangeTemplate
+from radtools.routines import _toradians
 
 
 class NotationError(ValueError):
     r"""
     Class for the errors with the exchange Hamiltonian notation.
 
     Parameters
@@ -45,15 +46,14 @@
             + f"    ExchangeHamiltonian.set_interpretation({name} = False)\n"
         )
 
     def __str__(self):
         return self.message
 
 
-# TODO Write symmetry constrains
 class ExchangeHamiltonian:
     r"""
     Exchange Hamiltonian.
 
     By default the notation of the exchange Hamiltonian is not defined
     and could be different in different context.
     However, in could always be checked via :py:attr:`.notation`.
@@ -78,15 +78,14 @@
     bonds : dict
         Dictionary of bonds.
 
         .. code-block:: python
 
             {(Atom_1, Atom_2, R): J, ...}
     magnetic_atoms : list
-        List of magnetic atoms.
     cell_list : list
     number_spins_in_unit_cell : int
     notation : str
     space_dimensions : tuple of floats
     double_counting : bool
     spin_normalized : bool
     factor_one_half : bool
@@ -101,15 +100,14 @@
             "spinw": (True, False, False, False, False),
         }
         self._crystal = None
         if crystal is None:
             crystal = Crystal()
         self.crystal = crystal
 
-        self.magnetic_atoms = []
         self.bonds = {}
 
         # Notation settings
         self._double_counting = None
         self._spin_normalized = None
         self._factor_one_half = None
         self._factor_two = None
@@ -423,26 +421,76 @@
             without the modification of the parameters.
         """
 
         if self._double_counting is None:
             raise NotationError("double_counting", "double counting")
         return self._double_counting
 
+    def _ensure_double_counting(self):
+        r"""
+        Ensure double counting.
+
+        Check and fix if needed, that for each (atom1, atom2, R)
+        (atom2, atom1, -R) is present in the Hamiltonian.
+        """
+
+        bonds = list(self)
+        for atom1, atom2, (i, j, k), J in bonds:
+            if (atom2, atom1, (-i, -j, -k)) not in self:
+                self.add_bond(J.T, atom2, atom1, (-i, -j, -k))
+
+    def _ensure_no_double_counting(self):
+        r"""
+        Ensure that there is no double counting in the model.
+
+        If the bond is (atom1, atom2, (i,j,k)), then the bond is kept in the model
+        if one of the conditions is true:
+
+        * i > 0
+        * i = 0 and j > 0
+        * i = 0, j = 0 and k > 0
+        * i = 0, j = 0, k = 0 and atom1.index <= atom2.index
+        """
+
+        bonds = list(self)
+
+        for atom1, atom2, (i, j, k), J in bonds:
+            if (
+                i > 0
+                or (i == 0 and j > 0)
+                or (i == 0 and j == 0 and k > 0)
+                or (i == 0 and j == 0 and k == 0 and atom1.index <= atom2.index)
+            ):
+                if (atom2, atom1, (-i, -j, -k)) in self:
+                    self.remove_bond(atom2, atom1, (-i, -j, -k))
+            else:
+                if (atom2, atom1, (-i, -j, -k)) not in self:
+                    self.add_bond(J.T, atom2, atom1, (-i, -j, -k))
+                    self.remove_bond(atom1, atom2, (i, j, k))
+
     @double_counting.setter
     def double_counting(self, new_value: bool):
         if self._double_counting is not None:
             factor = 1
             if self._double_counting and not new_value:
                 factor = 2
             elif not self._double_counting and new_value:
                 factor = 0.5
             if factor != 1:
-                # TODO Think about bond`s filtering/addition
+                if new_value:
+                    self._ensure_double_counting()
+                else:
+                    self._ensure_no_double_counting()
                 for atom1, atom2, R, J in self:
                     self[atom1, atom2, R] = J * factor
+        else:
+            if new_value:
+                self._ensure_double_counting()
+            else:
+                self._ensure_no_double_counting()
         self._double_counting = bool(new_value)
 
     @property
     def spin_normalized(self) -> bool:
         r"""
         Whether spin is normalized.
 
@@ -588,19 +636,37 @@
                     self[atom1, atom2, R] = J * factor
         self._minus_sign = bool(new_value)
 
     def __iter__(self):
         return ExchangeHamiltonianIterator(self)
 
     def __contains__(self, key):
+        atom1, atom2, R = key
+        if isinstance(atom1, str):
+            atom1 = self.crystal.get_atom(atom1)
+        if isinstance(atom2, str):
+            atom2 = self.crystal.get_atom(atom2)
+        key = (atom1, atom2, R)
         return key in self.bonds
 
     def __getitem__(self, key) -> ExchangeParameter:
+        atom1, atom2, R = key
+        if isinstance(atom1, str):
+            atom1 = self.crystal.get_atom(atom1)
+        if isinstance(atom2, str):
+            atom2 = self.crystal.get_atom(atom2)
+        key = (atom1, atom2, R)
         return self.bonds[key]
 
+    def __getattr__(self, name):
+        # Fix copy/deepcopy RecursionError
+        if name in ["__setstate__"]:
+            raise AttributeError(name)
+        return getattr(self.crystal, name)
+
     @property
     def crystal(self) -> Crystal:
         r"""
         Crystal of the Hamiltonian.
 
         Crystal, which define the structure.
         See :py:class:`.Crystal`.
@@ -631,14 +697,28 @@
 
         cells = set()
         for atom1, atom2, R, J in self:
             cells.add(R)
         return np.array(list(cells))
 
     @property
+    def magnetic_atoms(self):
+        r"""
+        Magnetic atoms of the model.
+
+        Atoms with at least bond starting or finishing in it.
+        """
+        result = set()
+        for atom1, atom2, R, J in self:
+            result.add(atom1)
+            result.add(atom2)
+
+        return list(result)
+
+    @property
     def number_spins_in_unit_cell(self):
         r"""
         Number of spins (or magnetic atoms) in the unit cell.
         """
 
         return len(self.magnetic_atoms)
 
@@ -713,26 +793,33 @@
             >>> (Cr, Cr, (1,0,0)) in model
             True
 
         Parameters
         ----------
         J : :py:class:`.ExchangeParameter`
             An instance of :py:class:`ExchangeParameter`.
-        atom1 : :py:class:`Atom`
+        atom1 : :py:class:`Atom` or str
             Atom object in (0, 0, 0) unit cell.
-        atom2 : :py:class:`Atom`
+            str works only if atom is already in the Hamiltonian.
+        atom2 : :py:class:`Atom` or str
             Atom object in R unit cell.
+            str works only if atom is already in the Hamiltonian.
         R : tuple of ints
             Vector of the unit cell for atom2.
             In the relative coordinates (i,j,k).
         """
 
-        if atom1 not in self.magnetic_atoms:
+        if isinstance(atom1, str):
+            atom1 = self.crystal.get_atom(atom1)
+        elif atom1 not in self.crystal:
             self.add_atom(atom1)
-        if atom2 not in self.magnetic_atoms:
+
+        if isinstance(atom2, str):
+            atom2 = self.crystal.get_atom(atom2)
+        elif atom2 not in self.crystal:
             self.add_atom(atom2)
 
         self.bonds[(atom1, atom2, R)] = J
 
     def __delitem__(self, key):
         self.remove_bond(*key)
 
@@ -777,30 +864,39 @@
             Atom object in (0, 0, 0) unit cell.
         atom2 : py:class:`.Atom`
             Atom object in R unit cell.
         R : tuple of ints
             Radius vector of the unit cell for atom2 (i,j,k).
         """
 
+        if isinstance(atom1, str):
+            atom1 = self.crystal.get_atom(atom1)
+
+        if isinstance(atom2, str):
+            atom2 = self.crystal.get_atom(atom2)
+
         try:
             del self.bonds[(atom1, atom2, R)]
         except KeyError:
-            pass
+            raise KeyError(
+                f"Bond ({atom2.fullname}, {atom2.fullname}, {R}) is not present in the model."
+            )
 
     def add_atom(self, atom: Atom):
         r"""
         Add atom to the Hamiltonian.
 
+        see :py:meth:`.Crystal.add_atom`
+
         Parameters
         ----------
         atom : :py:class:`.Atom`
             Atom object.
         """
 
-        self.magnetic_atoms.append(atom)
         self.crystal.add_atom(atom)
 
     def remove_atom(self, atom):
         r"""
         Remove magnetic atom from the Hamiltonian.
 
         Note: this method will remove atom itself and all the
@@ -808,17 +904,17 @@
 
         Parameters
         ----------
         atom : :py:class:`.Atom`
             Atom object.
         """
 
+        if isinstance(atom, str):
+            atom = self.crystal.get_atom(atom)
         bonds_for_removal = []
-        if atom in self.magnetic_atoms:
-            self.magnetic_atoms.remove(atom)
         for atom1, atom2, R, J in self:
             if atom1 == atom or atom2 == atom:
                 bonds_for_removal.append((atom1, atom2, R))
 
         for bond in bonds_for_removal:
             del self[bond]
 
@@ -879,19 +975,20 @@
                 bonds_for_removal.add((atom1, atom2, R))
 
             if min_distance is not None and dis < min_distance:
                 bonds_for_removal.add((atom1, atom2, R))
 
             if R_vector is not None and R not in R_vector:
                 bonds_for_removal.add((atom1, atom2, R))
-            # Here literals, not objects are compared, because in general
-            # template only has information about literals and R.
+            # Here names, not objects are compared, because in general
+            # template only has information about names (or fullnames) and R.
             if (
                 template is not None
-                and (atom1.literal, atom2.literal, R) not in template
+                and (atom1.name, atom2.name, R) not in template
+                and (atom1.fullname, atom2.fullname, R) not in template
             ):
                 bonds_for_removal.add((atom1, atom2, R))
 
         for atom1, atom2, R in bonds_for_removal:
             del self[atom1, atom2, R]
 
     def filtered(
@@ -943,14 +1040,15 @@
             max_distance=max_distance,
             min_distance=min_distance,
             template=template,
             R_vector=R_vector,
         )
         return filtered_model
 
+    # TODO rewrite with new template logic (J1 through getattr)
     def force_symmetry(self, template):
         r"""
         Force the Hamiltonian to have the symmetries of the template.
 
         Takes mean values of the parameters.
         For DMI interaction directions are kept the same,
         but the length of the DMI vector is scaled.
@@ -973,16 +1071,16 @@
         self.filter(template=template)
 
         for name in template.names:
             bonds = template.names[name]
             symm_matrix = np.zeros((3, 3), dtype=float)
             dmi_module = 0
             for atom1, atom2, R in bonds:
-                # Here literals, not objects are obtained, because in general
-                # template only has information about literals and R.
+                # Here names, not objects are obtained, because in general
+                # template only has information about names and R.
                 J = self[self.crystal.get_atom(atom1), self.crystal.get_atom(atom2), R]
                 symm_matrix = symm_matrix + J.symm_matrix
                 dmi_module = dmi_module + J.dmi_module
 
             symm_matrix = symm_matrix / len(bonds)
             dmi_module = dmi_module / len(bonds)
 
@@ -1163,15 +1261,30 @@
                             + f"{R[0]:2.0f} {R[1]:2.0f} {R[2]:2.0f})\n"
                         )
             if force_symmetry:
                 summary += "\n"
 
         return summary
 
-    # TODO Fix notation
+    def energy_matrix(self):
+        energy = np.zeros((3, 3), dtype=float)
+        factor = 1
+        if self.minus_sign:
+            factor *= -1
+        if self.factor_one_half:
+            factor /= 2
+        if self.factor_two:
+            factor *= 2
+        for atom1, atom2, R, J in self:
+            if self.spin_normalized:
+                energy += factor * J.matrix
+            else:
+                energy += factor * J.matrix * atom1.spin * atom2.spin
+        return energy
+
     def ferromagnetic_energy(self, theta=0, phi=0):
         r"""
         Compute energy of the Hamiltonian assuming ferromagnetic state.
 
         With Hamiltonian of the form:
 
         .. math::
@@ -1179,38 +1292,41 @@
             \hat{H} = - \sum_{i,j} \vec{S}_i J_{ij} \vec{S}_j
 
         where spin vectors are normalized to 1 and :math:`J_{ij}` is the
         exchange matrix.
 
         Parameters
         ----------
-        theta : float, default 0
-            Angle between z axis an direction of the magnetization.
-            :math:`0 < \theta < 180`
-        phi : float, default 0
-            angle between x axis an projection of direction of the
-            magnetization on xy plane.
-            :math:`0 < \phi < 360`
+        theta : float or (N,) |array_like|_, default 0
+            Angle between z axis and direction of the magnetization.
+            :math:`0^{\circ} \le \theta \le 180^{\circ}`.
+        phi : float or (N,) |array_like|_, default 0
+            angle between x axis and projection of
+            magnetization`s direction on xy plane.
+            :math:`0^{\circ} \le \phi < 360^{\circ}`.
 
         Returns
         -------
-        energy : float
+        energy : float or (N,) :numpy:`ndarray`
             Energy of ferromagnetic Hamiltonian with magnetization direction defined
             by ``theta`` and ``phi``. In the units of J values.
         """
 
-        theta = theta / 180 * pi
-        phi = phi / 180 * pi
-        energy = np.zeros((3, 3), dtype=float)
-        for atom1, atom2, R, J in self:
-            energy -= J.matrix
+        theta = np.array(theta) * _toradians
+        phi = np.array(phi) * _toradians
+        if theta.shape == ():
+            theta = np.array([theta])
+        if phi.shape == ():
+            phi = np.array([phi])
         spin_vector = np.array(
-            [cos(phi) * sin(theta), sin(phi) * sin(theta), cos(theta)]
+            [np.cos(phi) * np.sin(theta), np.sin(phi) * np.sin(theta), np.cos(theta)]
+        )
+        energy = np.einsum(
+            "ni,ij,jn->n", spin_vector.T, self.energy_matrix(), spin_vector
         )
-        energy = spin_vector @ energy @ spin_vector
         return energy
 
     # OLD METHODS AND ATTRIBUTES, KEPT FOR BACKWARD COMPATIBILITY
 
     @property
     def cell(self):
         r"""
@@ -1356,7 +1472,25 @@
             result = self._bonds[self._index]
             self._index += 1
             return result
         raise StopIteration
 
     def __iter__(self):
         return self
+
+
+if __name__ == "__main__":
+    model = ExchangeHamiltonian()
+    Cr = Atom("Cr", (0, 0, 0), spin=3 / 2)
+    model[Cr, Cr, (1, 0, 0)] = ExchangeParameter(iso=1)
+    assert model[Cr, Cr, (1, 0, 0)].iso == 1
+
+    model.notation = "standard"
+    assert model[Cr, Cr, (1, 0, 0)].iso == 1
+    model.notation = "standard"
+    assert model[Cr, Cr, (1, 0, 0)].iso == 1
+
+    assert model.double_counting
+    model.double_counting = False
+    assert model[Cr, Cr, (1, 0, 0)].iso == 2
+    model.double_counting = True
+    assert model[Cr, Cr, (1, 0, 0)].iso == 1
```

### Comparing `rad-tools-0.7.0/radtools/exchange/parameter.py` & `rad-tools-0.7.1/radtools/exchange/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,27 +120,27 @@
         if new_matrix.shape != (3, 3):
             raise ValueError("Matrix shape has to be equal to (3, 3)")
         self._matrix = new_matrix
 
     @property
     def symm_matrix(self) -> np.ndarray:
         r"""
-        Symmetric part of exchange :py:attr:`matrix`.
+        Symmetric part of exchange :py:attr:`.matrix`.
 
         .. math::
 
             J_{symm} = \dfrac{J + J^T}{2}
         """
 
         return (self.matrix + self.matrix.T) / 2
 
     @property
     def asymm_matrix(self) -> np.ndarray:
         """
-        Asymmetric part of exchange :py:attr:`matrix`.
+        Asymmetric part of exchange :py:attr:`.matrix`.
 
         .. math::
 
             J_{asymm} = \dfrac{J - J^T}{2}
         """
 
         return (self.matrix - self.matrix.T) / 2
@@ -162,15 +162,15 @@
     def iso(self, new_iso):
         new_iso = new_iso - self.iso
         self.matrix = self.matrix + (new_iso) * np.identity(3, dtype=float)
 
     @property
     def iso_matrix(self) -> np.ndarray:
         r"""
-        Isotropic part of the exchange :py:attr:`matrix`.
+        Isotropic part of the exchange :py:attr:`.matrix`.
 
         Matrix form:
 
         .. code-block:: python
 
             [[J, 0, 0],
              [0, J, 0],
@@ -272,15 +272,15 @@
             dtype=float,
         )
         self.matrix = self.matrix + dmi_matrix
 
     @property
     def dmi_matrix(self) -> np.ndarray:
         r"""
-        Asymmetric part of the exchange :py:attr:`matrix`.
+        Asymmetric part of the exchange :py:attr:`.matrix`.
 
         .. code-block:: python
 
             [[0, D_z, -D_y],
              [-D_z, 0, D_x],
              [D_y, -D_x, 0]]
         """
```

### Comparing `rad-tools-0.7.0/radtools/exchange/template.py` & `rad-tools-0.7.1/radtools/exchange/template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/io/internal.py` & `rad-tools-0.7.1/radtools/io/internal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/io/tb2j.py` & `rad-tools-0.7.1/radtools/io/tb2j.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,17 @@
                     magmom = tuple(map(float, [line[5], line[6], line[7]]))
                 except IndexError:
                     magmom = None
                 try:
                     charge = float(line[4])
                 except IndexError:
                     charge = None
-                model.crystal.add_atom(
+                model.add_atom(
                     Atom(
-                        literal=line[0],
+                        name=line[0],
                         position=tuple(map(float, line[1:4])),
                         index=i,
                         magmom=magmom,
                         charge=charge,
                     )
                 )
                 line = file.readline().split()
@@ -111,16 +111,18 @@
     model.crystal.identify()
 
     # Read exchange
     while line:
         while line and minor_sep not in line:
             line = file.readline()
         line = file.readline().translate(garbage).split()
-        atom1 = model.crystal.get_atom(line[0])
-        atom2 = model.crystal.get_atom(line[1])
+        # atom1 = model.crystal.get_atom(line[0])
+        # atom2 = model.crystal.get_atom(line[1])
+        atom1 = line[0]
+        atom2 = line[1]
         R = tuple(map(int, line[2:5]))
         distance = float(line[-1])
         iso = None
         aniso = None
         dmi = None
         while line and minor_sep not in line:
             line = file.readline()
@@ -140,17 +142,17 @@
                 )
 
             # Read DMI
             if line and dmi_flag in line:
                 dmi = tuple(map(float, line.translate(garbage).split()[-3:]))
 
         # Adding info from the exchange block to the ExchangeHamiltonian structure
-        bond = ExchangeParameter(iso=iso, aniso=aniso, dmi=dmi)
-        model.add_bond(bond, atom1, atom2, R)
-        computed_distance = model.crystal.get_distance(atom1, atom2, R)
+        J = ExchangeParameter(iso=iso, aniso=aniso, dmi=dmi)
+        model.add_bond(J, atom1, atom2, R)
+        computed_distance = model.get_distance(atom1, atom2, R)
         if abs(computed_distance - distance) > 0.001 and not quiet:
             print(
                 f"\nComputed distance is a different from the read one:\n"
                 + f"  Computed: {computed_distance:.4f}\n  "
                 + f"Read: {distance:.4f}\n"
             )
```

### Comparing `rad-tools-0.7.0/radtools/kpoints/__init__.py` & `rad-tools-0.7.1/radtools/kpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/kpoints/high_symmetry_point.py` & `rad-tools-0.7.1/radtools/kpoints/high_symmetry_point.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/kpoints/kpoints.py` & `rad-tools-0.7.1/radtools/kpoints/kpoints.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/map.py` & `rad-tools-0.7.1/radtools/map.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/routines.py` & `rad-tools-0.7.1/radtools/routines.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/score/__init__.py` & `rad-tools-0.7.1/radtools/score/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/score/extract_tb2j.py` & `rad-tools-0.7.1/radtools/score/extract_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/score/identify_wannier_centres.py` & `rad-tools-0.7.1/radtools/score/identify_wannier_centres.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/score/make_template.py` & `rad-tools-0.7.1/radtools/score/make_template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/score/plot_dos.py` & `rad-tools-0.7.1/radtools/score/plot_dos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/radtools/score/plot_tb2j.py` & `rad-tools-0.7.1/radtools/score/plot_tb2j.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,23 +105,23 @@
 
             ax.scatter(x1, y1, s=100 * fig.dpi / 72.0, c="white")
             ax.scatter(x2, y2, s=100 * fig.dpi / 72.0, c="white")
 
             ax.text(
                 x2,
                 y2,
-                atom_mark_to_latex(atom2.literal),
+                atom_mark_to_latex(atom2.name),
                 va="center",
                 ha="center",
                 fontsize=1.5 * fontsize * scale_atoms,
             )
             ax.text(
                 x1,
                 y1,
-                atom_mark_to_latex(atom1.literal),
+                atom_mark_to_latex(atom1.name),
                 va="center",
                 ha="center",
                 fontsize=1.5 * fontsize * scale_atoms,
                 color="#A04F4D",
             )
             if wtp == "iso":
                 ax.text(
```

### Comparing `rad-tools-0.7.0/scripts/compute-energies.py` & `rad-tools-0.7.1/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/scripts/phonopy-plotter.py` & `rad-tools-0.7.1/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.0/setup.py` & `rad-tools-0.7.1/setup.py`

 * *Files identical despite different names*

