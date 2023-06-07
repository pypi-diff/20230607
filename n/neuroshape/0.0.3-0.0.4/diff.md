# Comparing `tmp/neuroshape-0.0.3.tar.gz` & `tmp/neuroshape-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.3.tar", last modified: Wed Jun  7 05:01:54 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.tar", last modified: Wed Jun  7 05:26:30 2023, max compression
```

## Comparing `neuroshape-0.0.3.tar` & `neuroshape-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,48 @@
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:01:54.123643 neuroshape-0.0.3/
--rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.406848 neuroshape-0.0.3/LICENSE
--rw-r--r--   0 nik        (502) admin       (80)      455 2023-06-07 05:01:54.123818 neuroshape-0.0.3/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     5334 2023-06-07 03:43:39.096525 neuroshape-0.0.3/README.rst
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:01:54.051734 neuroshape-0.0.3/neuroshape/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.500598 neuroshape-0.0.3/neuroshape/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    20918 2023-06-07 04:43:27.677208 neuroshape-0.0.3/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 nik        (502) admin       (80)     5054 2023-06-04 23:43:38.501113 neuroshape-0.0.3/neuroshape/eigenmaps.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:01:54.053991 neuroshape-0.0.3/neuroshape/nulls/
--rw-r--r--   0 nik        (502) admin       (80)      347 2023-06-04 23:43:38.505161 neuroshape-0.0.3/neuroshape/nulls/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.505357 neuroshape-0.0.3/neuroshape/nulls/burt.py
--rw-r--r--   0 nik        (502) admin       (80)    14902 2023-06-04 23:43:38.505546 neuroshape-0.0.3/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.505759 neuroshape-0.0.3/neuroshape/nulls/nulls.py
--rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.506010 neuroshape-0.0.3/neuroshape/nulls/spins.py
--rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.506789 neuroshape-0.0.3/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.506923 neuroshape-0.0.3/neuroshape/permutation.py
--rw-r--r--   0 nik        (502) admin       (80)     5145 2023-06-04 23:43:38.507037 neuroshape-0.0.3/neuroshape/poly_eigenmaps.py
--rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.507316 neuroshape-0.0.3/neuroshape/stats.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:01:54.079141 neuroshape-0.0.3/neuroshape/utils/
--rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.761094 neuroshape-0.0.3/neuroshape/utils/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.507794 neuroshape-0.0.3/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.507917 neuroshape-0.0.3/neuroshape/utils/check_map.py
--rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.508050 neuroshape-0.0.3/neuroshape/utils/checks.py
--rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.508168 neuroshape-0.0.3/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.508308 neuroshape-0.0.3/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.508443 neuroshape-0.0.3/neuroshape/utils/concavehull.py
--rw-r--r--   0 nik        (502) admin       (80)     3428 2023-06-04 23:43:38.508580 neuroshape-0.0.3/neuroshape/utils/eigen.py
--rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.508823 neuroshape-0.0.3/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 nik        (502) admin       (80)     9310 2023-06-07 04:41:54.865227 neuroshape-0.0.3/neuroshape/utils/geometry.py
--rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.509143 neuroshape-0.0.3/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.509278 neuroshape-0.0.3/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.509397 neuroshape-0.0.3/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.509518 neuroshape-0.0.3/neuroshape/utils/tmpname.py
--rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.509765 neuroshape-0.0.3/neuroshape/utils/zscore_avg_method.py
--rw-r--r--   0 nik        (502) admin       (80)    15295 2023-06-07 02:28:43.701667 neuroshape-0.0.3/neuroshape/volume_eigenmodes.py
--rw-r--r--   0 nik        (502) admin       (80)      106 2023-06-04 23:43:38.510265 neuroshape-0.0.3/requirements.txt
--rw-r--r--   0 nik        (502) admin       (80)     1063 2023-06-07 00:29:10.039913 neuroshape-0.0.3/setup.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:01:54.123255 neuroshape-0.0.3/src/
--rw-r--r--   0 nik        (502) admin       (80)     4664 2023-06-06 23:21:17.671198 neuroshape-0.0.3/src/eta_squared.c
--rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.852948 neuroshape-0.0.3/src/euler_threshold.c
--rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.185901 neuroshape-0.0.3/src/glmfit.c
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.846755 neuroshape-0.0.4/
+-rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4/LICENSE
+-rw-r--r--   0 nik        (502) admin       (80)       70 2023-06-04 23:43:38.000000 neuroshape-0.0.4/MANIFEST.in
+-rw-r--r--   0 nik        (502) admin       (80)      466 2023-06-07 05:26:30.846418 neuroshape-0.0.4/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     5334 2023-06-07 03:43:39.000000 neuroshape-0.0.4/README.rst
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.836193 neuroshape-0.0.4/neuroshape/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    20918 2023-06-07 04:43:27.000000 neuroshape-0.0.4/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 nik        (502) admin       (80)     5054 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/eigenmaps.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.839752 neuroshape-0.0.4/neuroshape/nulls/
+-rw-r--r--   0 nik        (502) admin       (80)      347 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/burt.py
+-rw-r--r--   0 nik        (502) admin       (80)    14902 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/spins.py
+-rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/permutation.py
+-rw-r--r--   0 nik        (502) admin       (80)     5145 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/poly_eigenmaps.py
+-rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/stats.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.845023 neuroshape-0.0.4/neuroshape/utils/
+-rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4/neuroshape/utils/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/check_map.py
+-rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/checks.py
+-rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/concavehull.py
+-rw-r--r--   0 nik        (502) admin       (80)     3428 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/eigen.py
+-rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 nik        (502) admin       (80)     9310 2023-06-07 04:41:54.000000 neuroshape-0.0.4/neuroshape/utils/geometry.py
+-rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/tmpname.py
+-rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4/neuroshape/utils/zscore_avg_method.py
+-rw-r--r--   0 nik        (502) admin       (80)    15295 2023-06-07 02:28:43.000000 neuroshape-0.0.4/neuroshape/volume_eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.837508 neuroshape-0.0.4/neuroshape.egg-info/
+-rw-r--r--   0 nik        (502) admin       (80)      466 2023-06-07 05:26:30.000000 neuroshape-0.0.4/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     1102 2023-06-07 05:26:30.000000 neuroshape-0.0.4/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-07 05:26:30.000000 neuroshape-0.0.4/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-07 05:26:30.000000 neuroshape-0.0.4/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 nik        (502) admin       (80)      106 2023-06-04 23:43:38.000000 neuroshape-0.0.4/requirements.txt
+-rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-07 05:26:30.846849 neuroshape-0.0.4/setup.cfg
+-rw-r--r--   0 nik        (502) admin       (80)     1021 2023-06-07 05:26:25.000000 neuroshape-0.0.4/setup.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-07 05:26:30.846010 neuroshape-0.0.4/src/
+-rw-r--r--   0 nik        (502) admin       (80)     4664 2023-06-06 23:21:17.000000 neuroshape-0.0.4/src/eta_squared.c
+-rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4/src/euler_threshold.c
+-rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4/src/glmfit.c
```

### Comparing `neuroshape-0.0.3/LICENSE` & `neuroshape-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/README.rst` & `neuroshape-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4/neuroshape/connectopic_laplacian.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/eigenmaps.py` & `neuroshape-0.0.4/neuroshape/eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/nulls/burt.py` & `neuroshape-0.0.4/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/nulls/spins.py` & `neuroshape-0.0.4/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/permutation.py` & `neuroshape-0.0.4/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/poly_eigenmaps.py` & `neuroshape-0.0.4/neuroshape/poly_eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/stats.py` & `neuroshape-0.0.4/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/utils/check_map.py` & `neuroshape-0.0.4/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/utils/checks.py` & `neuroshape-0.0.4/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/utils/eigen.py` & `neuroshape-0.0.4/neuroshape/utils/eigen.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/utils/geometry.py` & `neuroshape-0.0.4/neuroshape/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/neuroshape/volume_eigenmodes.py` & `neuroshape-0.0.4/neuroshape/volume_eigenmodes.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/setup.py` & `neuroshape-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 '''
     setup.py file for neuroshape module
 '''
 
-from distutils.core import setup, Extension
+from setuptools import setup, Extension
 import numpy
 
 # define the extension module
 eta = Extension('neuroshape.eta', sources=['src/eta_squared.c'],
                           include_dirs=[numpy.get_include()])
 
 glmfit = Extension('neuroshape._stats', sources=['src/glmfit.c'],
                    include_dirs=[numpy.get_include()])
 
 euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
                   include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.3',
+      version='0.0.4',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
-      packages=['neuroshape','neuroshape.utils','neuroshape.nulls'],
+      packages=['neuroshape'],
       ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.3/src/eta_squared.c` & `neuroshape-0.0.4/src/eta_squared.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/src/euler_threshold.c` & `neuroshape-0.0.4/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.3/src/glmfit.c` & `neuroshape-0.0.4/src/glmfit.c`

 * *Files identical despite different names*

