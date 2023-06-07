# Comparing `tmp/pygem-0.2.1.tar.gz` & `tmp/pygem-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/drounce/Documents/HiMAT/packaging_pygem/PyGEM/dist/.tmp-xknww4bx/pygem-0.2.1.tar", last modified: Wed Jun  7 05:20:28 2023, max compression
+gzip compressed data, was "pygem-0.2.2.tar", last modified: Wed Jun  7 17:21:02 2023, max compression
```

## Comparing `pygem-0.2.1.tar` & `pygem-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.048444 pygem-0.2.1/
--rwxr-xr-x   0 drounce    (501) staff       (20)     1361 2023-06-07 05:19:38.000000 pygem-0.2.1/.gitignore
--rwxr-xr-x   0 drounce    (501) staff       (20)     1069 2023-06-07 05:19:38.000000 pygem-0.2.1/LICENSE
--rw-r--r--   0 drounce    (501) staff       (20)     2386 2023-06-07 05:20:28.047922 pygem-0.2.1/PKG-INFO
--rwxr-xr-x   0 drounce    (501) staff       (20)     1931 2023-06-07 05:19:38.000000 pygem-0.2.1/README.md
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.041858 pygem-0.2.1/pygem/
--rwxr-xr-x   0 drounce    (501) staff       (20)       83 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/__init__.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    48958 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/glacierdynamics.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    60883 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/massbalance.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    12724 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/oggm_compat.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.043723 pygem-0.2.1/pygem/preprocess/
--rwxr-xr-x   0 drounce    (501) staff       (20)     9171 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/preprocess/ecmwf_data.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    22140 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/pygem_input.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    22040 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/pygem_modelsetup.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.044321 pygem-0.2.1/pygem/scraps/
--rwxr-xr-x   0 drounce    (501) staff       (20)      529 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/scraps/dummy_task_module.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     1000 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/scraps/run.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.046029 pygem-0.2.1/pygem/shop/
--rwxr-xr-x   0 drounce    (501) staff       (20)     6736 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/shop/calving.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    21905 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/shop/climate.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     7783 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/shop/debris.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     5063 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/shop/icethickness.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    12429 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/shop/mbdata.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.046903 pygem-0.2.1/pygem/tests/
--rwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/tests/__init__.py
--rwxr-xr-x   0 drounce    (501) staff       (20)      149 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/tests/test_basics.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     2594 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/tests/test_oggm_compat.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.047428 pygem-0.2.1/pygem/utils/
--rwxr-xr-x   0 drounce    (501) staff       (20)     2304 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/utils/_funcs.py
--rw-r--r--   0 drounce    (501) staff       (20)     2651 2023-06-07 05:19:38.000000 pygem-0.2.1/pygem/utils/_funcs_selectglaciers.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 05:20:28.043408 pygem-0.2.1/pygem.egg-info/
--rw-r--r--   0 drounce    (501) staff       (20)     2386 2023-06-07 05:20:27.000000 pygem-0.2.1/pygem.egg-info/PKG-INFO
--rw-r--r--   0 drounce    (501) staff       (20)      631 2023-06-07 05:20:28.000000 pygem-0.2.1/pygem.egg-info/SOURCES.txt
--rw-r--r--   0 drounce    (501) staff       (20)        1 2023-06-07 05:20:27.000000 pygem-0.2.1/pygem.egg-info/dependency_links.txt
--rw-r--r--   0 drounce    (501) staff       (20)        6 2023-06-07 05:20:27.000000 pygem-0.2.1/pygem.egg-info/top_level.txt
--rw-r--r--   0 drounce    (501) staff       (20)      610 2023-06-07 05:19:38.000000 pygem-0.2.1/pyproject.toml
--rw-r--r--   0 drounce    (501) staff       (20)       38 2023-06-07 05:20:28.048543 pygem-0.2.1/setup.cfg
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.137871 pygem-0.2.2/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1361 2020-11-22 15:57:18.000000 pygem-0.2.2/.gitignore
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1069 2020-11-22 15:57:18.000000 pygem-0.2.2/LICENSE
+-rw-r--r--   0 drounce    (501) staff       (20)     2386 2023-06-07 17:21:02.137554 pygem-0.2.2/PKG-INFO
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1931 2023-06-07 04:01:43.000000 pygem-0.2.2/README.md
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.132023 pygem-0.2.2/pygem/
+-rwxr-xr-x   0 drounce    (501) staff       (20)       83 2023-06-07 17:13:35.000000 pygem-0.2.2/pygem/__init__.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    28650 2023-06-07 17:03:36.000000 pygem-0.2.2/pygem/class_climate.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    35877 2023-06-07 17:03:36.000000 pygem-0.2.2/pygem/gcmbiasadj.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    48958 2023-06-07 03:54:10.000000 pygem-0.2.2/pygem/glacierdynamics.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    60883 2023-06-07 04:01:43.000000 pygem-0.2.2/pygem/massbalance.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    12724 2023-06-07 03:54:10.000000 pygem-0.2.2/pygem/oggm_compat.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.133600 pygem-0.2.2/pygem/preprocess/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     9171 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/preprocess/ecmwf_data.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    22140 2023-06-07 05:08:29.000000 pygem-0.2.2/pygem/pygem_input.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    23592 2023-06-07 17:03:36.000000 pygem-0.2.2/pygem/pygem_modelsetup.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.134157 pygem-0.2.2/pygem/scraps/
+-rwxr-xr-x   0 drounce    (501) staff       (20)      529 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/scraps/dummy_task_module.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1000 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/scraps/run.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.135697 pygem-0.2.2/pygem/shop/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     6736 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/shop/calving.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    21905 2021-02-01 14:09:24.000000 pygem-0.2.2/pygem/shop/climate.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     7783 2021-02-01 14:09:24.000000 pygem-0.2.2/pygem/shop/debris.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     5063 2021-09-23 17:13:56.000000 pygem-0.2.2/pygem/shop/icethickness.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    12429 2022-08-11 04:33:58.000000 pygem-0.2.2/pygem/shop/mbdata.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.136664 pygem-0.2.2/pygem/tests/
+-rwxr-xr-x   0 drounce    (501) staff       (20)        0 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/tests/__init__.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)      149 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/tests/test_basics.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     2594 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/tests/test_oggm_compat.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.137152 pygem-0.2.2/pygem/utils/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     2304 2021-01-10 16:41:45.000000 pygem-0.2.2/pygem/utils/_funcs.py
+-rw-r--r--   0 drounce    (501) staff       (20)     2651 2022-06-13 02:59:07.000000 pygem-0.2.2/pygem/utils/_funcs_selectglaciers.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.133151 pygem-0.2.2/pygem.egg-info/
+-rw-r--r--   0 drounce    (501) staff       (20)     2386 2023-06-07 17:21:02.000000 pygem-0.2.2/pygem.egg-info/PKG-INFO
+-rw-r--r--   0 drounce    (501) staff       (20)      674 2023-06-07 17:21:02.000000 pygem-0.2.2/pygem.egg-info/SOURCES.txt
+-rw-r--r--   0 drounce    (501) staff       (20)        1 2023-06-07 17:21:02.000000 pygem-0.2.2/pygem.egg-info/dependency_links.txt
+-rw-r--r--   0 drounce    (501) staff       (20)        6 2023-06-07 17:21:02.000000 pygem-0.2.2/pygem.egg-info/top_level.txt
+-rw-r--r--   0 drounce    (501) staff       (20)      610 2023-06-07 17:13:35.000000 pygem-0.2.2/pyproject.toml
+-rw-r--r--   0 drounce    (501) staff       (20)       38 2023-06-07 17:21:02.137981 pygem-0.2.2/setup.cfg
```

### Comparing `pygem-0.2.1/.gitignore` & `pygem-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/LICENSE` & `pygem-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/PKG-INFO` & `pygem-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygem
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Glacier Evolution Model for large-scale glacier modeling
 Author-email: David Rounce <drounce@cmu.edu>
 Project-URL: Homepage, https://github.com/drounce/PyGEM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygem-0.2.1/README.md` & `pygem-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/glacierdynamics.py` & `pygem-0.2.2/pygem/glacierdynamics.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/massbalance.py` & `pygem-0.2.2/pygem/massbalance.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/oggm_compat.py` & `pygem-0.2.2/pygem/oggm_compat.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/preprocess/ecmwf_data.py` & `pygem-0.2.2/pygem/preprocess/ecmwf_data.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/pygem_input.py` & `pygem-0.2.2/pygem/pygem_input.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/pygem_modelsetup.py` & `pygem-0.2.2/pygem/pygem_modelsetup.py`

 * *Files 7% similar despite different names*

```diff
@@ -420,7 +420,60 @@
     #   representative of regional processes/climate
     #   Note: this is really only important for calibration purposes and
     #         post-processing when you want to show results over specific
     #         regions.
     # Development Note: if create another method for selecting glaciers,
     #                   make sure that update way to select glacier
     #                   hypsometry as well.
+
+
+def split_list(lst, n=1, option_ordered=1):
+    """
+    Split list into batches for the supercomputer.
+    
+    Parameters
+    ----------
+    lst : list
+        List that you want to split into separate batches
+    n : int
+        Number of batches to split glaciers into.
+    
+    Returns
+    -------
+    lst_batches : list
+        list of n lists that have sequential values in each list
+    """
+    # If batches is more than list, then there will be one glacier in each batch
+    if option_ordered == 1:
+        if n > len(lst):
+            n = len(lst)
+        n_perlist_low = int(len(lst)/n)
+        n_perlist_high = int(np.ceil(len(lst)/n))
+        lst_copy = lst.copy()
+        count = 0
+        lst_batches = []
+        for x in np.arange(n):
+            count += 1
+            if count <= len(lst) % n:
+                lst_subset = lst_copy[0:n_perlist_high]
+                lst_batches.append(lst_subset)
+                [lst_copy.remove(i) for i in lst_subset]
+            else:
+                lst_subset = lst_copy[0:n_perlist_low]
+                lst_batches.append(lst_subset)
+                [lst_copy.remove(i) for i in lst_subset]
+        
+    else:
+        if n > len(lst):
+            n = len(lst)
+    
+        lst_batches = [[] for x in np.arange(n)]
+        nbatch = 0
+        for count, x in enumerate(lst):
+            if count%n == 0:
+                nbatch = 0
+    
+            lst_batches[nbatch].append(x)
+            
+            nbatch += 1
+
+    return lst_batches
```

### Comparing `pygem-0.2.1/pygem/scraps/dummy_task_module.py` & `pygem-0.2.2/pygem/scraps/dummy_task_module.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/scraps/run.py` & `pygem-0.2.2/pygem/scraps/run.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/shop/calving.py` & `pygem-0.2.2/pygem/shop/calving.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/shop/climate.py` & `pygem-0.2.2/pygem/shop/climate.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/shop/debris.py` & `pygem-0.2.2/pygem/shop/debris.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/shop/icethickness.py` & `pygem-0.2.2/pygem/shop/icethickness.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/shop/mbdata.py` & `pygem-0.2.2/pygem/shop/mbdata.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/tests/test_oggm_compat.py` & `pygem-0.2.2/pygem/tests/test_oggm_compat.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/utils/_funcs.py` & `pygem-0.2.2/pygem/utils/_funcs.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem/utils/_funcs_selectglaciers.py` & `pygem-0.2.2/pygem/utils/_funcs_selectglaciers.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.1/pygem.egg-info/PKG-INFO` & `pygem-0.2.2/pygem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygem
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Glacier Evolution Model for large-scale glacier modeling
 Author-email: David Rounce <drounce@cmu.edu>
 Project-URL: Homepage, https://github.com/drounce/PyGEM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygem-0.2.1/pygem.egg-info/SOURCES.txt` & `pygem-0.2.2/pygem.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 pygem/__init__.py
+pygem/class_climate.py
+pygem/gcmbiasadj.py
 pygem/glacierdynamics.py
 pygem/massbalance.py
 pygem/oggm_compat.py
 pygem/pygem_input.py
 pygem/pygem_modelsetup.py
 pygem.egg-info/PKG-INFO
 pygem.egg-info/SOURCES.txt
```

### Comparing `pygem-0.2.1/pyproject.toml` & `pygem-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "wheel",
 ]
 
 [tool.setuptools_scm]
 
 [project]
 name = "pygem"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="David Rounce", email="drounce@cmu.edu" },
 ]
 description = "Python Glacier Evolution Model for large-scale glacier modeling"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

