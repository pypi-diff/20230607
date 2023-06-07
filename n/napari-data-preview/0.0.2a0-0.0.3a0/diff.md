# Comparing `tmp/napari_data_preview-0.0.2a0-py3-none-any.whl.zip` & `tmp/napari_data_preview-0.0.3a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 24368 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      193 b- defN 23-Feb-17 08:32 napari_data_preview/__init__.py
--rw-rw-rw-  2.0 fat    31866 b- defN 23-Feb-17 08:32 napari_data_preview/_dock_widget.py
--rw-rw-rw-  2.0 fat    81679 b- defN 23-Feb-17 10:48 napari_data_preview/_reader.py
--rw-rw-rw-  2.0 fat      572 b- defN 23-Feb-21 08:44 napari_data_preview/napari.yaml
--rw-rw-rw-  2.0 fat     1104 b- defN 23-Feb-21 08:44 napari_data_preview-0.0.2a0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1895 b- defN 23-Feb-21 08:44 napari_data_preview-0.0.2a0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-21 08:44 napari_data_preview-0.0.2a0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       72 b- defN 23-Feb-21 08:44 napari_data_preview-0.0.2a0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       20 b- defN 23-Feb-21 08:44 napari_data_preview-0.0.2a0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      920 b- defN 23-Feb-21 08:44 napari_data_preview-0.0.2a0.dist-info/RECORD
-10 files, 118413 bytes uncompressed, 22766 bytes compressed:  80.8%
+Zip file size: 24608 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      193 b- defN 23-Jun-07 14:35 napari_data_preview/__init__.py
+-rw-rw-rw-  2.0 fat    31763 b- defN 23-Jun-07 14:11 napari_data_preview/_dock_widget.py
+-rw-rw-rw-  2.0 fat    81598 b- defN 23-Jun-07 14:29 napari_data_preview/_reader.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-Jun-07 14:37 napari_data_preview/_version.py
+-rw-rw-rw-  2.0 fat      572 b- defN 23-Jun-07 14:43 napari_data_preview/napari.yaml
+-rw-rw-rw-  2.0 fat     1104 b- defN 23-Jun-07 14:56 napari_data_preview-0.0.3a0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1868 b- defN 23-Jun-07 14:56 napari_data_preview-0.0.3a0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 14:56 napari_data_preview-0.0.3a0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       72 b- defN 23-Jun-07 14:56 napari_data_preview-0.0.3a0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jun-07 14:56 napari_data_preview-0.0.3a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1007 b- defN 23-Jun-07 14:56 napari_data_preview-0.0.3a0.dist-info/RECORD
+11 files, 118504 bytes uncompressed, 22868 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -3,29 +3,32 @@
 
 Filename: napari_data_preview/_dock_widget.py
 Comment: 
 
 Filename: napari_data_preview/_reader.py
 Comment: 
 
+Filename: napari_data_preview/_version.py
+Comment: 
+
 Filename: napari_data_preview/napari.yaml
 Comment: 
 
-Filename: napari_data_preview-0.0.2a0.dist-info/LICENSE
+Filename: napari_data_preview-0.0.3a0.dist-info/LICENSE
 Comment: 
 
-Filename: napari_data_preview-0.0.2a0.dist-info/METADATA
+Filename: napari_data_preview-0.0.3a0.dist-info/METADATA
 Comment: 
 
-Filename: napari_data_preview-0.0.2a0.dist-info/WHEEL
+Filename: napari_data_preview-0.0.3a0.dist-info/WHEEL
 Comment: 
 
-Filename: napari_data_preview-0.0.2a0.dist-info/entry_points.txt
+Filename: napari_data_preview-0.0.3a0.dist-info/entry_points.txt
 Comment: 
 
-Filename: napari_data_preview-0.0.2a0.dist-info/top_level.txt
+Filename: napari_data_preview-0.0.3a0.dist-info/top_level.txt
 Comment: 
 
-Filename: napari_data_preview-0.0.2a0.dist-info/RECORD
+Filename: napari_data_preview-0.0.3a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## napari_data_preview/__init__.py

```diff
@@ -1,7 +1,7 @@
 try:
     from ._version import version as __version__
 except ImportError:
     __version__ = "not-installed"
 
-from ._reader import microscope_reader
+from ._reader import napari_get_reader
 from ._dock_widget import DataPreview
```

## napari_data_preview/_dock_widget.py

```diff
@@ -3,20 +3,17 @@
 
 It implements the ``napari_experimental_provide_dock_widget`` hook specification.
 see: https://napari.org/docs/dev/plugins/hook_specifications.html
 
 Replace code below according to your needs.
 """
 
-from ._reader import range_overlap, MyMesoSpimData_2D
+from ._reader import range_overlap
 
 import numpy as np
-from magicgui import magic_factory
-import napari
-from napari.layers import Layer
 from qtpy.QtWidgets import QWidget, QVBoxLayout, QPushButton, QSlider, QLabel
 from PyQt5.QtCore import Qt
 
 
 def test_if_inside_rect(x, y, rect):
     '''
     This function test if a point (pair of x and y coordinates) is inside a rectangle
```

## napari_data_preview/_reader.py

```diff
@@ -15,15 +15,14 @@
 import dask
 import dask_image.imread
 import dask.array as da
 import tifffile
 
 from PIL import Image
 from skimage import io
-import matplotlib.pyplot as plt
 
 import PySimpleGUI as sg
 
 
 def get_num_values_text(path_text, target_values_string):
 
     '''
@@ -767,16 +766,15 @@
         target = "CHN"
         n = last_file_name.find(target) + len(target)
         n_chans = int(last_file_name[n:n + 2]) + 1
         n_planes = int(n_files / n_chans)
 
         #
         temp_path = os.path.join(temp_path, "VW0_LOC000D_CM0_CHN00_PLN0000.tif")
-        im = plt.imread(temp_path)
-        im = np.array(im)
+        im = io.imread(temp_path)
         size_tile = im.shape
         size_tile = int(size_tile[0])
 
         meta_data_values = get_num_values_text(
             path_text,["Horizontal = ", "Vertical = ", "Actual Vertical Overlap", "Actual Horizontal Overlap"])
 
         dim_x = int(meta_data_values[0])
@@ -1849,24 +1847,24 @@
 
         wd = os.getcwd()
         current_path_xml = os.path.join(wd, name_xml + ".xml")
         target_path_xml = os.path.join(target_path_xml, name_xml + ".xml")
         tree.write(target_path_xml)
 
 
-# def napari_get_reader(path: Union[str, List[str]]): # -> Optional[ReaderFunction]:
-#     """
-#     Return a function named microscope_reader capable of reading different light-sheet microscope data into napari layer data.
-#     Parameters
-#     -------
-#     function:
-#         Return a function that accepts the
-#         same path or list of paths, and returns a list of layer data tuples.
-#     """
-#     return microscope_reader
+def napari_get_reader(path: Union[str, List[str]]): # -> Optional[ReaderFunction]:
+    """
+    Return a function named microscope_reader capable of reading different light-sheet microscope data into napari layer data.
+    Parameters
+    -------
+    function:
+        Return a function that accepts the
+        same path or list of paths, and returns a list of layer data tuples.
+    """
+    return microscope_reader
 
 
 def microscope_reader(path: Union[str, List[str]]) -> List[Tuple[Any, Dict, str]]:
 
     # First test to determine the type of microscope. Than instanciate an object from the corresponding subclass
     type_microscope = get_type_microscope(path)
     if type_microscope == "Clear Scope":
```

## napari_data_preview/napari.yaml

```diff
@@ -1,21 +1,21 @@
 name: napari-data-preview
-schema_version: 0.0.2-alpha
+schema_version: 0.0.3-alpha
 contributions:
 
   readers:
-  - command: napari-data-preview.microscope_reader
+  - command: napari-data-preview.napari_get_reader
     filename_patterns:
     - '*'
     accepts_directories: true
 
   commands:
   - id: napari-data-preview.DataPreview
     title: Open my widget
     python_name: napari_data_preview:DataPreview
-  - id: napari-data-preview.microscope_reader
+  - id: napari-data-preview.napari_get_reader
     title: Get Reader
-    python_name: napari_data_preview._reader:microscope_reader
+    python_name: napari_data_preview._reader:napari_get_reader
 
   widgets:
   - command: napari-data-preview.DataPreview
     display_name: Lightsheet data preview
```

## Comparing `napari_data_preview-0.0.2a0.dist-info/LICENSE` & `napari_data_preview-0.0.3a0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `napari_data_preview-0.0.2a0.dist-info/METADATA` & `napari_data_preview-0.0.3a0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-data-preview
-Version: 0.0.2a0
+Version: 0.0.3a0
 Summary: Preview lightsheet microscopes acquisition, and allow the creation of an XML for importing the data into TeraStitcher.
 Home-page: https://github.com/WyssCenter/napari-data-preview
 Author: Vivien Gaillet, Jules Scholler
 Author-email: jules.scholler@wysscenter.ch
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -25,15 +25,14 @@
 Requires-Dist: lxml
 Requires-Dist: napari-tools-menu
 Requires-Dist: magic-class
 Requires-Dist: napari-plugin-engine (>=0.1.4)
 Requires-Dist: dask
 Requires-Dist: tifffile
 Requires-Dist: dask-image
-Requires-Dist: matplotlib
 Requires-Dist: elementpath
 Requires-Dist: tk (>=0.1.0)
 Requires-Dist: zarr
 Requires-Dist: scikit-image
 Requires-Dist: PySimpleGUI
 Requires-Dist: pytest-shutil
```

