# Comparing `tmp/pygem-0.2.0.tar.gz` & `tmp/pygem-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/drounce/Documents/HiMAT/packaging_pygem/PyGEM/dist/.tmp-gz_mpe4v/pygem-0.2.0.tar", last modified: Wed Jun  7 04:41:03 2023, max compression
+gzip compressed data, was "/Users/drounce/Documents/HiMAT/packaging_pygem/PyGEM/dist/.tmp-xknww4bx/pygem-0.2.1.tar", last modified: Wed Jun  7 05:20:28 2023, max compression
```

## Comparing `pygem-0.2.0.tar` & `pygem-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 04:41:03.746639 pygem-0.2.0/
--rwxr-xr-x   0 drounce    (501) staff       (20)     1361 2023-06-07 04:39:34.000000 pygem-0.2.0/.gitignore
--rwxr-xr-x   0 drounce    (501) staff       (20)     1069 2023-06-07 04:39:34.000000 pygem-0.2.0/LICENSE
--rw-r--r--   0 drounce    (501) staff       (20)     2386 2023-06-07 04:41:03.746303 pygem-0.2.0/PKG-INFO
--rwxr-xr-x   0 drounce    (501) staff       (20)     1931 2023-06-07 04:39:34.000000 pygem-0.2.0/README.md
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 04:41:03.740062 pygem-0.2.0/pygem/
--rwxr-xr-x   0 drounce    (501) staff       (20)       83 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/__init__.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    48958 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/glacierdynamics.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    60883 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/massbalance.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    12724 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/oggm_compat.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 04:41:03.742204 pygem-0.2.0/pygem/preprocess/
--rwxr-xr-x   0 drounce    (501) staff       (20)     9171 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/preprocess/ecmwf_data.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    22284 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/pygem_input.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    22040 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/pygem_modelsetup.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 04:41:03.742905 pygem-0.2.0/pygem/scraps/
--rwxr-xr-x   0 drounce    (501) staff       (20)      529 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/scraps/dummy_task_module.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     1000 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/scraps/run.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 04:41:03.744370 pygem-0.2.0/pygem/shop/
--rwxr-xr-x   0 drounce    (501) staff       (20)     6736 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/shop/calving.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    21905 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/shop/climate.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     7783 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/shop/debris.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     5063 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/shop/icethickness.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    12429 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/shop/mbdata.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 04:41:03.745235 pygem-0.2.0/pygem/tests/
--rwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/tests/__init__.py
--rwxr-xr-x   0 drounce    (501) staff       (20)      149 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/tests/test_basics.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     2594 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/tests/test_oggm_compat.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 04:41:03.745843 pygem-0.2.0/pygem/utils/
--rwxr-xr-x   0 drounce    (501) staff       (20)     2304 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/utils/_funcs.py
--rw-r--r--   0 drounce    (501) staff       (20)     2651 2023-06-07 04:39:34.000000 pygem-0.2.0/pygem/utils/_funcs_selectglaciers.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 04:41:03.741860 pygem-0.2.0/pygem.egg-info/
--rw-r--r--   0 drounce    (501) staff       (20)     2386 2023-06-07 04:41:03.000000 pygem-0.2.0/pygem.egg-info/PKG-INFO
--rw-r--r--   0 drounce    (501) staff       (20)      631 2023-06-07 04:41:03.000000 pygem-0.2.0/pygem.egg-info/SOURCES.txt
--rw-r--r--   0 drounce    (501) staff       (20)        1 2023-06-07 04:41:03.000000 pygem-0.2.0/pygem.egg-info/dependency_links.txt
--rw-r--r--   0 drounce    (501) staff       (20)        6 2023-06-07 04:41:03.000000 pygem-0.2.0/pygem.egg-info/top_level.txt
--rw-r--r--   0 drounce    (501) staff       (20)      610 2023-06-07 04:39:34.000000 pygem-0.2.0/pyproject.toml
--rw-r--r--   0 drounce    (501) staff       (20)       38 2023-06-07 04:41:03.746720 pygem-0.2.0/setup.cfg
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.048444 pygem-0.2.1/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1361 2023-06-07 05:19:38.000000 pygem-0.2.1/.gitignore
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1069 2023-06-07 05:19:38.000000 pygem-0.2.1/LICENSE
+-rw-r--r--   0 drounce    (501) staff       (20)     2386 2023-06-07 05:20:28.047922 pygem-0.2.1/PKG-INFO
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1931 2023-06-07 05:19:38.000000 pygem-0.2.1/README.md
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.041858 pygem-0.2.1/pygem/
+-rwxr-xr-x   0 drounce    (501) staff       (20)       83 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/__init__.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    48958 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/glacierdynamics.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    60883 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/massbalance.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    12724 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/oggm_compat.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.043723 pygem-0.2.1/pygem/preprocess/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     9171 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/preprocess/ecmwf_data.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    22140 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/pygem_input.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    22040 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/pygem_modelsetup.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.044321 pygem-0.2.1/pygem/scraps/
+-rwxr-xr-x   0 drounce    (501) staff       (20)      529 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/scraps/dummy_task_module.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1000 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/scraps/run.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.046029 pygem-0.2.1/pygem/shop/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     6736 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/shop/calving.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    21905 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/shop/climate.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     7783 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/shop/debris.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     5063 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/shop/icethickness.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    12429 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/shop/mbdata.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.046903 pygem-0.2.1/pygem/tests/
+-rwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/tests/__init__.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)      149 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/tests/test_basics.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     2594 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/tests/test_oggm_compat.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.047428 pygem-0.2.1/pygem/utils/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     2304 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/utils/_funcs.py
+-rw-r--r--   0 drounce    (501) staff       (20)     2651 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/utils/_funcs_selectglaciers.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.043408 pygem-0.2.1/pygem.egg-info/
+-rw-r--r--   0 drounce    (501) staff       (20)     2386 2023-06-07 05:20:27.000000 pygem-0.2.1/pygem.egg-info/PKG-INFO
+-rw-r--r--   0 drounce    (501) staff       (20)      631 2023-06-07 05:20:28.000000 pygem-0.2.1/pygem.egg-info/SOURCES.txt
+-rw-r--r--   0 drounce    (501) staff       (20)        1 2023-06-07 05:20:27.000000 pygem-0.2.1/pygem.egg-info/dependency_links.txt
+-rw-r--r--   0 drounce    (501) staff       (20)        6 2023-06-07 05:20:27.000000 pygem-0.2.1/pygem.egg-info/top_level.txt
+-rw-r--r--   0 drounce    (501) staff       (20)      610 2023-06-07 05:19:38.000000 pygem-0.2.1/pyproject.toml
+-rw-r--r--   0 drounce    (501) staff       (20)       38 2023-06-07 05:20:28.048543 pygem-0.2.1/setup.cfg
```

### Comparing `pygem-0.2.0/.gitignore` & `pygem-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/LICENSE` & `pygem-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/PKG-INFO` & `pygem-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygem
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python Glacier Evolution Model for large-scale glacier modeling
 Author-email: David Rounce <drounce@cmu.edu>
 Project-URL: Homepage, https://github.com/drounce/PyGEM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygem-0.2.0/README.md` & `pygem-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/glacierdynamics.py` & `pygem-0.2.1/pygem/glacierdynamics.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/massbalance.py` & `pygem-0.2.1/pygem/massbalance.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/oggm_compat.py` & `pygem-0.2.1/pygem/oggm_compat.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/preprocess/ecmwf_data.py` & `pygem-0.2.1/pygem/preprocess/ecmwf_data.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/pygem_input.py` & `pygem-0.2.1/pygem/pygem_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,22 +35,17 @@
 
 # Types of glaciers to include (True) or exclude (False)
 include_landterm = True                # Switch to include land-terminating glaciers
 include_laketerm = True                # Switch to include lake-terminating glaciers
 include_tidewater = True               # Switch to include tidewater glaciers
 ignore_calving = False                 # Switch to ignore calving and treat tidewater glaciers as land-terminating
 
-<<<<<<< HEAD
-#oggm_base_url = 'https://cluster.klima.uni-bremen.de/~oggm/gdirs/oggm_v1.4/L1-L2_files/elev_bands/'
 oggm_base_url = 'https://cluster.klima.uni-bremen.de/~fmaussion/gdirs/prepro_l2_202010/elevbands_fl_with_consensus'
-
-=======
-oggm_base_url = 'https://cluster.klima.uni-bremen.de/~oggm/gdirs/oggm_v1.4/L1-L2_files/elev_bands/'
+#oggm_base_url = 'https://cluster.klima.uni-bremen.de/~oggm/gdirs/oggm_v1.4/L1-L2_files/elev_bands/'
 logging_level = 'DEBUG' # DEBUG, INFO, WARNING, ERROR, WORKFLOW, CRITICAL (recommended WORKFLOW)
->>>>>>> origin/master
 
 #%% ===== CLIMATE DATA ===== 
 # Reference period runs (reference period refers to the calibration period)
 ref_gcm_name = 'ERA5'               # reference climate dataset
 ref_startyear = 2000                # first year of model run (reference dataset)
 ref_endyear = 2019                  # last year of model run (reference dataset)
 ref_wateryear = 'calendar'          # options for years: 'calendar', 'hydro', 'custom'
```

### Comparing `pygem-0.2.0/pygem/pygem_modelsetup.py` & `pygem-0.2.1/pygem/pygem_modelsetup.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/scraps/dummy_task_module.py` & `pygem-0.2.1/pygem/scraps/dummy_task_module.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/scraps/run.py` & `pygem-0.2.1/pygem/scraps/run.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/shop/calving.py` & `pygem-0.2.1/pygem/shop/calving.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/shop/climate.py` & `pygem-0.2.1/pygem/shop/climate.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/shop/debris.py` & `pygem-0.2.1/pygem/shop/debris.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/shop/icethickness.py` & `pygem-0.2.1/pygem/shop/icethickness.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/shop/mbdata.py` & `pygem-0.2.1/pygem/shop/mbdata.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/tests/test_oggm_compat.py` & `pygem-0.2.1/pygem/tests/test_oggm_compat.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/utils/_funcs.py` & `pygem-0.2.1/pygem/utils/_funcs.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem/utils/_funcs_selectglaciers.py` & `pygem-0.2.1/pygem/utils/_funcs_selectglaciers.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pygem.egg-info/PKG-INFO` & `pygem-0.2.1/pygem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygem
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python Glacier Evolution Model for large-scale glacier modeling
 Author-email: David Rounce <drounce@cmu.edu>
 Project-URL: Homepage, https://github.com/drounce/PyGEM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygem-0.2.0/pygem.egg-info/SOURCES.txt` & `pygem-0.2.1/pygem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygem-0.2.0/pyproject.toml` & `pygem-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "wheel",
 ]
 
 [tool.setuptools_scm]
 
 [project]
 name = "pygem"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="David Rounce", email="drounce@cmu.edu" },
 ]
 description = "Python Glacier Evolution Model for large-scale glacier modeling"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

