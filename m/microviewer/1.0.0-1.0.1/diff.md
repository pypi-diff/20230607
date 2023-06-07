# Comparing `tmp/microviewer-1.0.0.tar.gz` & `tmp/microviewer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microviewer-1.0.0.tar", last modified: Tue Jun  6 07:24:44 2023, max compression
+gzip compressed data, was "microviewer-1.0.1.tar", last modified: Wed Jun  7 02:03:41 2023, max compression
```

## Comparing `microviewer-1.0.0.tar` & `microviewer-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-06 07:24:44.556935 microviewer-1.0.0/
--rw-r--r--   0 wms        (501) staff       (20)       52 2023-06-06 07:24:44.000000 microviewer-1.0.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)      280 2023-06-06 07:24:44.000000 microviewer-1.0.0/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.0.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)     2126 2023-06-06 07:24:44.557106 microviewer-1.0.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1112 2023-06-06 05:23:07.000000 microviewer-1.0.0/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-06 07:24:44.554851 microviewer-1.0.0/microviewer/
--rw-r--r--   0 wms        (501) staff       (20)     5037 2023-06-06 05:31:02.000000 microviewer-1.0.0/microviewer/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    34695 2023-06-05 21:09:00.000000 microviewer-1.0.0/microviewer/datacube.js
--rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.0.0/microviewer/favicon.ico
--rw-r--r--   0 wms        (501) staff       (20)    18823 2023-06-06 07:21:48.000000 microviewer-1.0.0/microviewer/index.html
--rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.0.0/microviewer/jquery-3.7.0.min.js
--rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.0.0/microviewer/requirements.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-06 07:24:44.556336 microviewer-1.0.0/microviewer.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     2126 2023-06-06 07:24:44.000000 microviewer-1.0.0/microviewer.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      503 2023-06-06 07:24:44.000000 microviewer-1.0.0/microviewer.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 07:24:44.000000 microviewer-1.0.0/microviewer.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       47 2023-06-06 07:24:44.000000 microviewer-1.0.0/microviewer.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.0.0/microviewer.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-06 07:24:44.000000 microviewer-1.0.0/microviewer.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       12 2023-06-06 07:24:44.000000 microviewer-1.0.0/microviewer.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-06 07:24:44.556749 microviewer-1.0.0/microviewer_cli/
--rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.0.0/microviewer_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     1088 2023-06-06 05:02:43.000000 microviewer-1.0.0/microviewer_cli/cli.py
--rw-r--r--   0 wms        (501) staff       (20)     1015 2023-06-06 07:24:44.557722 microviewer-1.0.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      225 2023-06-06 04:44:08.000000 microviewer-1.0.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-07 02:03:41.140790 microviewer-1.0.1/
+-rw-r--r--   0 wms        (501) staff       (20)       52 2023-06-07 02:03:41.000000 microviewer-1.0.1/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)      495 2023-06-07 02:03:41.000000 microviewer-1.0.1/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.0.1/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)     2372 2023-06-07 02:03:41.140973 microviewer-1.0.1/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1358 2023-06-06 15:00:16.000000 microviewer-1.0.1/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-07 02:03:41.138120 microviewer-1.0.1/microviewer/
+-rw-r--r--   0 wms        (501) staff       (20)     5037 2023-06-06 05:31:02.000000 microviewer-1.0.1/microviewer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    34702 2023-06-06 19:11:19.000000 microviewer-1.0.1/microviewer/datacube.js
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.0.1/microviewer/favicon.ico
+-rw-r--r--   0 wms        (501) staff       (20)    18826 2023-06-06 15:06:58.000000 microviewer-1.0.1/microviewer/index.html
+-rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.0.1/microviewer/jquery-3.7.0.min.js
+-rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.0.1/microviewer/requirements.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-07 02:03:41.139957 microviewer-1.0.1/microviewer.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     2372 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      516 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       47 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.0.1/microviewer.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       28 2023-06-07 02:03:41.000000 microviewer-1.0.1/microviewer.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-07 02:03:41.140493 microviewer-1.0.1/microviewer_cli/
+-rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.0.1/microviewer_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     1088 2023-06-06 05:02:43.000000 microviewer-1.0.1/microviewer_cli/cli.py
+-rw-r--r--   0 wms        (501) staff       (20)   220312 2023-06-06 07:35:34.000000 microviewer-1.0.1/seg-demo.png
+-rw-r--r--   0 wms        (501) staff       (20)     1032 2023-06-07 02:03:41.141623 microviewer-1.0.1/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      225 2023-06-06 04:44:08.000000 microviewer-1.0.1/setup.py
```

### Comparing `microviewer-1.0.0/LICENSE` & `microviewer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.0/PKG-INFO` & `microviewer-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
+[![PyPI version](https://badge.fury.io/py/microviewer.svg)](https://badge.fury.io/py/microviewer)
+
 # microviewer
 Multiplatform 3D numpy image browser based viewer.
 
 ```python
 from microviewer import view, hyperview
 
 view(numpy_image) # for gray and color images
@@ -36,21 +38,29 @@
 ```
 
 ```bash
 uview image.npy.gz # view as image
 uview labels.npy.gz --seg # view as segmentation
 ```
 
+![Segmentation display in microviewer](seg-demo.png "Segmentation display in microviewer.")
+
 Visualize 3D numpy arrays in your browser without difficult installation procedures or reformatting your data.  The code is CPU based and the image is uncompressed in memory. You're limited to images that are at most 2^31 bytes large (~2.1 GB) due to browser limitations.
 
 ## Supports
 
 - 8-bit grayscale 3D images
 - color images (including 3 channel 3D images)
 - floating point images
 - boolean images
 - segmentation labels
 
+## Installation
+
+```bash
+pip install microviewer
+```
+
 ## History
 
 This microviewer package has been a part of CloudVolume since 2018, but is now broken out into its own package for more flexible wider use. Microviewer uses a modified version of https://github.com/seung-lab/data-cube-x/ (2016) to represent the array in Javascript.
```

### Comparing `microviewer-1.0.0/README.md` & `microviewer-1.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI version](https://badge.fury.io/py/microviewer.svg)](https://badge.fury.io/py/microviewer)
+
 # microviewer
 Multiplatform 3D numpy image browser based viewer.
 
 ```python
 from microviewer import view, hyperview
 
 view(numpy_image) # for gray and color images
@@ -12,23 +14,31 @@
 ```
 
 ```bash
 uview image.npy.gz # view as image
 uview labels.npy.gz --seg # view as segmentation
 ```
 
+![Segmentation display in microviewer](seg-demo.png "Segmentation display in microviewer.")
+
 Visualize 3D numpy arrays in your browser without difficult installation procedures or reformatting your data.  The code is CPU based and the image is uncompressed in memory. You're limited to images that are at most 2^31 bytes large (~2.1 GB) due to browser limitations.
 
 ## Supports
 
 - 8-bit grayscale 3D images
 - color images (including 3 channel 3D images)
 - floating point images
 - boolean images
 - segmentation labels
 
+## Installation
+
+```bash
+pip install microviewer
+```
+
 ## History
 
 This microviewer package has been a part of CloudVolume since 2018, but is now broken out into its own package for more flexible wider use. Microviewer uses a modified version of https://github.com/seung-lab/data-cube-x/ (2016) to represent the array in Javascript.
```

### Comparing `microviewer-1.0.0/microviewer/__init__.py` & `microviewer-1.0.1/microviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.0/microviewer/datacube.js` & `microviewer-1.0.1/microviewer/datacube.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -246,20 +246,21 @@
             r: 10,
             g: 10,
             b: 10,
             a: 0
         });
 
         let segments = this.segments;
-        let show_all = Object.keys(segments).length === 0;
+        let show_all = true;
 
         let ArrayType = this.channel.arrayType();
         let segarray = new Uint8Array(this.renumbering.length);
         Object.keys(segments).forEach((label) => {
             segarray[label] = !!segments[label];
+            show_all &&= !segments[label];
         });
 
         // We sometimes disable the hover highlight to get more performance
         if (hover_enabled) {
             for (let i = pixels32.length - 1; i >= 0; i--) {
                 if (seg_slice[i]) {
                     if (show_all | segarray[seg_slice[i]] | seg_slice[i] === hover_id) {
```

### Comparing `microviewer-1.0.0/microviewer/favicon.ico` & `microviewer-1.0.1/microviewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.0/microviewer/index.html` & `microviewer-1.0.1/microviewer/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -631,15 +631,15 @@
       <p>CONTROLS</p>
       <ul>
         <li>W/S ,/. or scroll - advance selected images</li>
         <li>A/D - switch slicing plane</li>
         <li>Space - zoom in to point</li>
         <li class='segmentation'>L - recolor segmentation labels</li>
         <li>Left Click - freeze info about current pixel</li>
-        <li class="hyperview">X - clear selected segments</li>
+        <li class="segmentation">X - clear selected segments</li>
         <li class="hyperview">+/- increase, decrease opacity</li>
         <li class='segmentation'>H - toggle hover highlight</li>
         <li>1/2 - zoom out/in</li>
       </ul>
 
       <input class="segmentation" type="checkbox" id="show_hover" name="show_hover" checked="checked"/> <label class="segmentation" for="show_hover">Highlight Hover?</label>
       <p class="segmentation">SELECTED SEGMENTS</p>
```

### Comparing `microviewer-1.0.0/microviewer/jquery-3.7.0.min.js` & `microviewer-1.0.1/microviewer/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.0/microviewer.egg-info/PKG-INFO` & `microviewer-1.0.1/microviewer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
+[![PyPI version](https://badge.fury.io/py/microviewer.svg)](https://badge.fury.io/py/microviewer)
+
 # microviewer
 Multiplatform 3D numpy image browser based viewer.
 
 ```python
 from microviewer import view, hyperview
 
 view(numpy_image) # for gray and color images
@@ -36,21 +38,29 @@
 ```
 
 ```bash
 uview image.npy.gz # view as image
 uview labels.npy.gz --seg # view as segmentation
 ```
 
+![Segmentation display in microviewer](seg-demo.png "Segmentation display in microviewer.")
+
 Visualize 3D numpy arrays in your browser without difficult installation procedures or reformatting your data.  The code is CPU based and the image is uncompressed in memory. You're limited to images that are at most 2^31 bytes large (~2.1 GB) due to browser limitations.
 
 ## Supports
 
 - 8-bit grayscale 3D images
 - color images (including 3 channel 3D images)
 - floating point images
 - boolean images
 - segmentation labels
 
+## Installation
+
+```bash
+pip install microviewer
+```
+
 ## History
 
 This microviewer package has been a part of CloudVolume since 2018, but is now broken out into its own package for more flexible wider use. Microviewer uses a modified version of https://github.com/seung-lab/data-cube-x/ (2016) to represent the array in Javascript.
```

### Comparing `microviewer-1.0.0/microviewer_cli/cli.py` & `microviewer-1.0.1/microviewer_cli/cli.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.0.0/setup.cfg` & `microviewer-1.0.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 [global]
 setup-hooks = 
 	pbr.hooks.setup_hook
 
 [files]
 packages = 
 	microviewer
+	microviewer_cli
 
 [wheel]
 universal = 0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

