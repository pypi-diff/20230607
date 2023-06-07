# Comparing `tmp/psdist-0.1.5.tar.gz` & `tmp/psdist-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdist-0.1.5.tar", last modified: Fri Jun  2 17:04:59 2023, max compression
+gzip compressed data, was "psdist-0.1.6.tar", last modified: Wed Jun  7 16:49:28 2023, max compression
```

## Comparing `psdist-0.1.5.tar` & `psdist-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-02 17:04:59.648864 psdist-0.1.5/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1070 2022-11-29 16:42:20.000000 psdist-0.1.5/LICENSE
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1245 2023-06-02 17:04:59.648720 psdist-0.1.5/PKG-INFO
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      787 2023-06-02 12:53:27.000000 psdist-0.1.5/README.md
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-02 17:04:59.646177 psdist-0.1.5/psdist/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       95 2023-03-02 16:46:32.000000 psdist-0.1.5/psdist/__init__.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4925 2023-01-17 23:20:27.000000 psdist-0.1.5/psdist/ap.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    12828 2023-06-02 13:20:42.000000 psdist-0.1.5/psdist/cloud.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1247 2023-01-17 19:53:50.000000 psdist-0.1.5/psdist/data.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    18125 2023-06-02 16:02:32.000000 psdist-0.1.5/psdist/image.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       53 2023-05-24 15:51:53.000000 psdist-0.1.5/psdist/sampling.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1344 2023-03-02 16:46:32.000000 psdist-0.1.5/psdist/utils.py
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-02 17:04:59.648361 psdist-0.1.5/psdist/visualization/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      156 2023-03-02 16:46:32.000000 psdist-0.1.5/psdist/visualization/__init__.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    16217 2023-06-02 16:55:39.000000 psdist-0.1.5/psdist/visualization/cloud.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    36316 2023-05-24 15:50:44.000000 psdist-0.1.5/psdist/visualization/grid.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    22591 2023-06-02 17:03:58.000000 psdist-0.1.5/psdist/visualization/image.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4152 2023-03-02 16:46:32.000000 psdist-0.1.5/psdist/visualization/visualization.py
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-02 17:04:59.647091 psdist-0.1.5/psdist.egg-info/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1245 2023-06-02 17:04:59.000000 psdist-0.1.5/psdist.egg-info/PKG-INFO
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      455 2023-06-02 17:04:59.000000 psdist-0.1.5/psdist.egg-info/SOURCES.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        1 2023-06-02 17:04:59.000000 psdist-0.1.5/psdist.egg-info/dependency_links.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      110 2023-06-02 17:04:59.000000 psdist-0.1.5/psdist.egg-info/requires.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        7 2023-06-02 17:04:59.000000 psdist-0.1.5/psdist.egg-info/top_level.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      716 2023-06-02 17:03:41.000000 psdist-0.1.5/pyproject.toml
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       38 2023-06-02 17:04:59.648914 psdist-0.1.5/setup.cfg
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-07 16:49:28.933718 psdist-0.1.6/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1070 2022-11-29 16:42:20.000000 psdist-0.1.6/LICENSE
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1078 2023-06-07 16:49:28.933603 psdist-0.1.6/PKG-INFO
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      619 2023-06-02 22:01:08.000000 psdist-0.1.6/README.md
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-07 16:49:28.932302 psdist-0.1.6/psdist/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       95 2023-03-02 16:46:32.000000 psdist-0.1.6/psdist/__init__.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4925 2023-01-17 23:20:27.000000 psdist-0.1.6/psdist/ap.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    12828 2023-06-02 13:20:42.000000 psdist-0.1.6/psdist/cloud.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1247 2023-01-17 19:53:50.000000 psdist-0.1.6/psdist/data.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    18125 2023-06-07 16:45:05.000000 psdist-0.1.6/psdist/image.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       53 2023-05-24 15:51:53.000000 psdist-0.1.6/psdist/sampling.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1344 2023-03-02 16:46:32.000000 psdist-0.1.6/psdist/utils.py
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-07 16:49:28.933450 psdist-0.1.6/psdist/visualization/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      156 2023-03-02 16:46:32.000000 psdist-0.1.6/psdist/visualization/__init__.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    16087 2023-06-05 16:13:18.000000 psdist-0.1.6/psdist/visualization/cloud.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    36316 2023-05-24 15:50:44.000000 psdist-0.1.6/psdist/visualization/grid.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    22591 2023-06-02 17:03:58.000000 psdist-0.1.6/psdist/visualization/image.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4152 2023-03-02 16:46:32.000000 psdist-0.1.6/psdist/visualization/visualization.py
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-07 16:49:28.932847 psdist-0.1.6/psdist.egg-info/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1078 2023-06-07 16:49:28.000000 psdist-0.1.6/psdist.egg-info/PKG-INFO
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      455 2023-06-07 16:49:28.000000 psdist-0.1.6/psdist.egg-info/SOURCES.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        1 2023-06-07 16:49:28.000000 psdist-0.1.6/psdist.egg-info/dependency_links.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      110 2023-06-07 16:49:28.000000 psdist-0.1.6/psdist.egg-info/requires.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        7 2023-06-07 16:49:28.000000 psdist-0.1.6/psdist.egg-info/top_level.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      716 2023-06-07 16:48:31.000000 psdist-0.1.6/pyproject.toml
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       38 2023-06-07 16:49:28.933756 psdist-0.1.6/setup.cfg
```

### Comparing `psdist-0.1.5/LICENSE` & `psdist-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psdist-0.1.5/PKG-INFO` & `psdist-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: psdist
-Version: 0.1.5
+Version: 0.1.6
 Summary: Analysis/visualization of phase space distributions
 Author-email: Austin Hoover <ahoover1218@gmail.com>
 Project-URL: homepage, https://github.com/austin-hoover/psdist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # psdist
 
-This repository is a collection of analysis and visualization methods for six-dimensional position-momentum space (phase space) distributions. Most of the methods should work for point-cloud or image data of any dimensionality.
+This repository is a collection of analysis and visualization methods for six-dimensional position-momentum space (phase space) distributions. Its primary use has been to slice and project high-dimensional data, both in point-cloud and image form.
 
 
 ## Installation
 
 https://pypi.org/project/psdist/
 
 
 ## Examples
 
-Some examples in accelerator physics that use methods from this repository:
-* https://journals.aps.org/prab/abstract/10.1103/PhysRevAccelBeams.23.124201
-* https://arxiv.org/abs/2301.04178
+See `/examples` folder and https://austin-hoover.github.io/psdist/.
 
-Each subplot in the figure below shows the measured $x-p_x$ distribution of a hadron beam within a small box in $y-p_y-p_z$ space; $y$ varies along the columns, $p_y$ varies along the rows, and $p_z$ varies with the animation frame number.
 
-![](examples/figures/view_yyp_slice_xxp_wslice.gif)
+## Related packages
+
+* https://github.com/openPMD/openPMD-viewer
+* https://github.com/bwheelz36/ParticlePhaseSpace
+* https://github.com/ColwynGulliford/distgen
+* https://aplpy.readthedocs.io/en/stable/fitsfigure/slicing.html
```

### Comparing `psdist-0.1.5/psdist/ap.py` & `psdist-0.1.6/psdist/ap.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.5/psdist/cloud.py` & `psdist-0.1.6/psdist/cloud.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.5/psdist/data.py` & `psdist-0.1.6/psdist/data.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.5/psdist/image.py` & `psdist-0.1.6/psdist/image.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.5/psdist/utils.py` & `psdist-0.1.6/psdist/utils.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.5/psdist/visualization/cloud.py` & `psdist-0.1.6/psdist/visualization/cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
     autolim_kws : dict
         Key word arguments passed to `auto_limits`.
     fig_kws : dict
         Key word arguments passed to `proplot.subplots`.
     **plot_kws
         Key word arguments passed to `plot2d`.
     """
-    if np.ndim(data) == 2:
+    if type(data) is not list:
         data = [data]
     n_data = len(data)
     n_dims = data[0].shape[1]
     for i in range(1, n_data):
         if data[i].shape[1] != n_dims:
             raise ValueError("data must have the same number of dimensions.")
 
@@ -335,16 +335,14 @@
 
     if limits is None:
         if autolim_kws is None:
             autolim_kws = dict()
         limits_list = np.array([auto_limits(X, **autolim_kws) for X in data])
         mins = np.min(limits_list[:, :, 0], axis=0)   
         maxs = np.max(limits_list[:, :, 1], axis=0)
-        # mins = np.min([np.min(X, axis=0) for X in data], axis=0)
-        # maxs = np.max([np.max(X, axis=0) for X in data], axis=0)
         limits = [(mins[i], maxs[i]) for i in range(n_dims)]
     if dims is None:
         dims = [f"x{i + 1}" for i in range(n_dims)]
     if units is None:
         units = n_dims * [""]
     dims_units = []
     for dim, unit in zip(dims, units):
```

### Comparing `psdist-0.1.5/psdist/visualization/grid.py` & `psdist-0.1.6/psdist/visualization/grid.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.5/psdist/visualization/image.py` & `psdist-0.1.6/psdist/visualization/image.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.5/psdist/visualization/visualization.py` & `psdist-0.1.6/psdist/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.5/psdist.egg-info/PKG-INFO` & `psdist-0.1.6/psdist.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: psdist
-Version: 0.1.5
+Version: 0.1.6
 Summary: Analysis/visualization of phase space distributions
 Author-email: Austin Hoover <ahoover1218@gmail.com>
 Project-URL: homepage, https://github.com/austin-hoover/psdist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # psdist
 
-This repository is a collection of analysis and visualization methods for six-dimensional position-momentum space (phase space) distributions. Most of the methods should work for point-cloud or image data of any dimensionality.
+This repository is a collection of analysis and visualization methods for six-dimensional position-momentum space (phase space) distributions. Its primary use has been to slice and project high-dimensional data, both in point-cloud and image form.
 
 
 ## Installation
 
 https://pypi.org/project/psdist/
 
 
 ## Examples
 
-Some examples in accelerator physics that use methods from this repository:
-* https://journals.aps.org/prab/abstract/10.1103/PhysRevAccelBeams.23.124201
-* https://arxiv.org/abs/2301.04178
+See `/examples` folder and https://austin-hoover.github.io/psdist/.
 
-Each subplot in the figure below shows the measured $x-p_x$ distribution of a hadron beam within a small box in $y-p_y-p_z$ space; $y$ varies along the columns, $p_y$ varies along the rows, and $p_z$ varies with the animation frame number.
 
-![](examples/figures/view_yyp_slice_xxp_wslice.gif)
+## Related packages
+
+* https://github.com/openPMD/openPMD-viewer
+* https://github.com/bwheelz36/ParticlePhaseSpace
+* https://github.com/ColwynGulliford/distgen
+* https://aplpy.readthedocs.io/en/stable/fitsfigure/slicing.html
```

### Comparing `psdist-0.1.5/pyproject.toml` & `psdist-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psdist"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Austin Hoover", email="ahoover1218@gmail.com" },
 ]
 description = "Analysis/visualization of phase space distributions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

