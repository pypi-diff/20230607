# Comparing `tmp/numan-1.0.3.tar.gz` & `tmp/numan-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numan-1.0.3.tar", last modified: Sun Sep 25 05:21:14 2022, max compression
+gzip compressed data, was "numan-1.0.4.tar", last modified: Tue Jun  6 23:03:01 2023, max compression
```

## Comparing `numan-1.0.3.tar` & `numan-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-09-25 05:21:14.587791 numan-1.0.3/
--rw-rw-rw-   0        0        0     1094 2022-05-18 18:25:15.000000 numan-1.0.3/LICENSE.md
--rw-rw-rw-   0        0        0     2181 2022-09-25 05:21:14.585827 numan-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2022-05-18 18:25:15.000000 numan-1.0.3/README.md
--rw-rw-rw-   0        0        0     1279 2022-09-25 05:16:35.000000 numan-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-25 05:21:14.587791 numan-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0       53 2022-08-16 05:16:10.000000 numan-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-25 05:21:14.517979 numan-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2022-09-25 05:21:14.566881 numan-1.0.3/src/numan/
--rw-rw-rw-   0        0        0      224 2022-09-25 05:16:00.000000 numan-1.0.3/src/numan/__init__.py
--rw-rw-rw-   0        0        0    30153 2022-09-22 01:15:46.000000 numan-1.0.3/src/numan/analysis.py
--rw-rw-rw-   0        0        0     1382 2022-08-18 08:58:12.000000 numan-1.0.3/src/numan/notifications.py
--rw-rw-rw-   0        0        0    32617 2022-09-25 04:39:18.000000 numan-1.0.3/src/numan/plots.py
--rw-rw-rw-   0        0        0     1097 2022-08-18 04:32:02.000000 numan-1.0.3/src/numan/project.py
--rw-rw-rw-   0        0        0    27110 2022-09-25 04:25:09.000000 numan-1.0.3/src/numan/report.py
--rw-rw-rw-   0        0        0     3396 2022-08-21 22:45:27.000000 numan-1.0.3/src/numan/runner.py
--rw-rw-rw-   0        0        0     5169 2022-09-25 00:13:45.000000 numan-1.0.3/src/numan/utils.py
--rw-rw-rw-   0        0        0    31018 2022-08-22 20:39:52.000000 numan-1.0.3/src/numan/visualization.py
-drwxrwxrwx   0        0        0        0 2022-09-25 05:21:14.584831 numan-1.0.3/src/numan.egg-info/
--rw-rw-rw-   0        0        0     2181 2022-09-25 05:21:14.000000 numan-1.0.3/src/numan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2022-09-25 05:21:14.000000 numan-1.0.3/src/numan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-25 05:21:14.000000 numan-1.0.3/src/numan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2022-09-25 05:21:14.000000 numan-1.0.3/src/numan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-09-25 05:21:14.000000 numan-1.0.3/src/numan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 23:03:01.549703 numan-1.0.4/
+-rw-rw-rw-   0        0        0     1094 2022-05-18 18:25:15.000000 numan-1.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0     2181 2023-06-06 23:03:01.548699 numan-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1558 2022-05-18 18:25:15.000000 numan-1.0.4/README.md
+-rw-rw-rw-   0        0        0     1314 2023-06-06 20:30:59.000000 numan-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 23:03:01.550700 numan-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       53 2022-08-16 05:16:10.000000 numan-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:03:01.390700 numan-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 23:03:01.487699 numan-1.0.4/src/numan/
+-rw-rw-rw-   0        0        0      224 2022-09-25 05:16:00.000000 numan-1.0.4/src/numan/__init__.py
+-rw-rw-rw-   0        0        0    30144 2023-06-06 20:27:40.000000 numan-1.0.4/src/numan/analysis.py
+-rw-rw-rw-   0        0        0     1382 2022-08-18 08:58:12.000000 numan-1.0.4/src/numan/notifications.py
+-rw-rw-rw-   0        0        0    32617 2022-09-25 04:39:18.000000 numan-1.0.4/src/numan/plots.py
+-rw-rw-rw-   0        0        0     1097 2022-08-18 04:32:02.000000 numan-1.0.4/src/numan/project.py
+-rw-rw-rw-   0        0        0    27170 2023-06-06 23:01:44.000000 numan-1.0.4/src/numan/report.py
+-rw-rw-rw-   0        0        0     3396 2022-08-21 22:45:27.000000 numan-1.0.4/src/numan/runner.py
+-rw-rw-rw-   0        0        0     5169 2022-09-25 00:13:45.000000 numan-1.0.4/src/numan/utils.py
+-rw-rw-rw-   0        0        0    31015 2023-06-06 20:27:40.000000 numan-1.0.4/src/numan/visualization.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:03:01.519698 numan-1.0.4/src/numan.egg-info/
+-rw-rw-rw-   0        0        0     2181 2023-06-06 23:03:01.000000 numan-1.0.4/src/numan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-06-06 23:03:01.000000 numan-1.0.4/src/numan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 23:03:01.000000 numan-1.0.4/src/numan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-06-06 23:03:01.000000 numan-1.0.4/src/numan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 23:03:01.000000 numan-1.0.4/src/numan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 23:03:01.546699 numan-1.0.4/tests/
+-rw-rw-rw-   0        0        0    15043 2022-11-29 19:20:20.000000 numan-1.0.4/tests/test_plots.py
+-rw-rw-rw-   0        0        0    15189 2023-06-06 20:27:40.000000 numan-1.0.4/tests/test_plots_cp13.py
+-rw-rw-rw-   0        0        0     1469 2022-09-22 06:17:16.000000 numan-1.0.4/tests/test_utils.py
```

### Comparing `numan-1.0.3/LICENSE.md` & `numan-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `numan-1.0.3/PKG-INFO` & `numan-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numan
-Version: 1.0.3
+Version: 1.0.4
 Summary: numerosity analysis package
 Author-email: Anna Nadtochiy <nadtochi@usc.edu>
 Project-URL: Homepage, https://github.com/LemonJust/numan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `numan-1.0.3/README.md` & `numan-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `numan-1.0.3/pyproject.toml` & `numan-1.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "numan"
-version = "1.0.3"
+version = "1.0.4"
 description='numerosity analysis package'
 readme = "README.md"
 authors = [{ name = "Anna Nadtochiy", email = "nadtochi@usc.edu" }]
 license = { file = "LICENSE" }
 classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering :: Image Processing',
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
 ]
 dependencies = [
-    'vodex >=1.0.3,<2.0.0',
+    'vodex >=1.0.18,<2.0.0',
     'pypdf2',
     'reportlab',
     'scipy',
     'ipykernel',
     'urllib3',
     'nbconvert',
-    'scipy'
+    'scipy',
+    'matplotlib',
+    'pandas'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["bumpver"]
 
 [project.urls] # Read The Docs will also go in here
 Homepage = "https://github.com/LemonJust/numan"
 
 [tool.bumpver]
-current_version = "1.0.3"
+current_version = "1.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `numan-1.0.3/src/numan/analysis.py` & `numan-1.0.4/src/numan/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,17 +103,17 @@
                 diameter = np.array(diameter)
             if units == 'phs':
                 diameter = np.round(diameter / self.resolution)
             d = diameter
 
         r = d / 2  # radius
         # make sure diameter is odd: round to the next odd number
-        d = ((d // 2) * 2 + 1).astype(np.int)
+        d = ((d // 2) * 2 + 1).astype(int)
         # center at zero
-        c = (d // 2).astype(np.int)
+        c = (d // 2).astype(int)
         z = np.arange(d[0]) - c[0]
         y = np.arange(d[1]) - c[1]
         x = np.arange(d[2]) - c[2]
 
         # find what pixels are inside the ellipsoid
         zz, yy, xx = np.meshgrid(z, y, x, indexing='ij')
         inside_ellipsoid = np.sqrt((zz / r[0]) ** 2 + (yy / r[1]) ** 2 + (xx / r[2]) ** 2) <= 1
@@ -153,15 +153,15 @@
         shift = self.center['pix']
         # because of the rounding when going from phs to pix, some extreme spots can be outside the image
         # so make sure they are inside
         border = np.array([zmax - 1, ymax - 1, xmax - 1])
         shift = np.min(np.c_[shift, border], axis=1)
 
         # get the indices
-        idx = idx + shift.astype(np.int)
+        idx = idx + shift.astype(int)
 
         # remove the ones outside the boundary
         idx = idx[np.all(idx >= 0, axis=1), :]
         is_inside = np.logical_and(idx[:, 0] < zmax, np.logical_and(idx[:, 1] < ymax, idx[:, 2] < xmax))
         idx = idx[is_inside, :]
 
         mask[idx[:, 0], idx[:, 1], idx[:, 2]] = 1
```

### Comparing `numan-1.0.3/src/numan/notifications.py` & `numan-1.0.4/src/numan/notifications.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.3/src/numan/plots.py` & `numan-1.0.4/src/numan/plots.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.3/src/numan/project.py` & `numan-1.0.4/src/numan/project.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.3/src/numan/report.py` & `numan-1.0.4/src/numan/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 from .analysis import Spots
 
 
 def merge_pdfs(pdfs, filename):
     """
     Turns a bunch of separate figures (pdfs) into one pdf.
     """
-    mergeFile = PyPDF2.PdfFileMerger()
+    mergeFile = PyPDF2.PdfMerger()
     for pdf in pdfs:
-        mergeFile.append(PyPDF2.PdfFileReader(pdf, 'rb'))
+        mergeFile.append(PyPDF2.PdfReader(pdf, 'rb'))
         os.remove(pdf)
     mergeFile.write(filename)
 
 
 def place_cb(can, x, y, name):
     form = can.acroForm
     can.setFont("Courier", 12)
@@ -308,14 +308,16 @@
         main_title = f"Average DFF per stimuli, pairwise comparison."
 
         # figure out figure layout
         if len(labels) == 3:
             figure_layout = [1, 3]
         elif len(labels) == 4:
             figure_layout = [2, 3]
+        elif len(labels) == 5:
+            figure_layout = [2, 5]
         else:
             raise Exception(f"Don't know how to plot when the number of labels is {len(labels)}")
 
         s_plotter.make_avg_act_scat_figure(labels, main_title,
                                            cell_numbers=cells_idx,
                                            # what grid to use to show the points
                                            figure_layout=figure_layout,
```

### Comparing `numan-1.0.3/src/numan/runner.py` & `numan-1.0.4/src/numan/runner.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.3/src/numan/utils.py` & `numan-1.0.4/src/numan/utils.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.3/src/numan/visualization.py` & `numan-1.0.4/src/numan/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         :type time_points:
         :param front_to_tail:
         :type front_to_tail:
         :return:
         :rtype:
         """
         # timing in volumes, since one volume is one time point of the signal
-        timing = (self.experiment.cycle.timing / self.experiment.volume_manager.fpv).astype(np.int)
+        timing = (self.experiment.cycle.timing / self.experiment.volume_manager.fpv).astype(int)
         # get condition name for each time point of the signal
         conditions = [cond for t, condition in zip(timing, self.experiment.cycle.conditions) for cond in
                       [condition.name] * t]
 
         # encode unique names into intengers, return_inverse gives the integer encoding
         names, values = np.unique(conditions, return_inverse=True)
```

### Comparing `numan-1.0.3/src/numan.egg-info/PKG-INFO` & `numan-1.0.4/src/numan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numan
-Version: 1.0.3
+Version: 1.0.4
 Summary: numerosity analysis package
 Author-email: Anna Nadtochiy <nadtochi@usc.edu>
 Project-URL: Homepage, https://github.com/LemonJust/numan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3
```

