# Comparing `tmp/uintel-0.4.2.tar.gz` & `tmp/uintel-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uintel-0.4.2.tar", last modified: Mon May  8 03:59:51 2023, max compression
+gzip compressed data, was "uintel-0.4.3.tar", last modified: Wed Jun  7 03:51:07 2023, max compression
```

## Comparing `uintel-0.4.2.tar` & `uintel-0.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.147077 uintel-0.4.2/
--rw-rw-r--   0 sam       (1000) sam       (1000)     1075 2023-04-03 04:47:18.000000 uintel-0.4.2/LICENSE
--rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-05-08 03:59:51.147077 uintel-0.4.2/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)     3274 2023-04-03 04:47:18.000000 uintel-0.4.2/README.md
--rw-rw-r--   0 sam       (1000) sam       (1000)       95 2023-04-03 04:47:18.000000 uintel-0.4.2/pyproject.toml
--rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-05-08 03:59:51.147077 uintel-0.4.2/setup.cfg
--rw-rw-r--   0 sam       (1000) sam       (1000)     1560 2023-05-08 03:59:33.000000 uintel-0.4.2/setup.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.139077 uintel-0.4.2/src/
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.143077 uintel-0.4.2/src/uintel/
--rw-rw-r--   0 sam       (1000) sam       (1000)     3030 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     7978 2023-05-05 02:33:43.000000 uintel-0.4.2/src/uintel/aws.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     4657 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/colours.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    10626 2023-05-05 02:33:43.000000 uintel-0.4.2/src/uintel/esri.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.143077 uintel-0.4.2/src/uintel/fonts/
--rw-rw-r--   0 sam       (1000) sam       (1000)    94884 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/fonts/Myriad Pro (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)   208636 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/fonts/Rubik (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)   202424 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/fonts/Rubik Italic (TrueType).ttf
--rw-rw-r--   0 sam       (1000) sam       (1000)    20290 2023-05-05 02:33:43.000000 uintel-0.4.2/src/uintel/geometry.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    23184 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/install.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2308 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/ogc.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3808 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/query.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     7934 2023-05-05 02:33:43.000000 uintel-0.4.2/src/uintel/server.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    13281 2023-05-05 02:33:43.000000 uintel-0.4.2/src/uintel/slack.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     6374 2023-05-08 03:59:28.000000 uintel-0.4.2/src/uintel/sql.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.147077 uintel-0.4.2/src/uintel/styles/
--rw-rw-r--   0 sam       (1000) sam       (1000)     1046 2023-04-03 04:47:18.000000 uintel-0.4.2/src/uintel/styles/ui.mplstyle
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-08 03:59:51.143077 uintel-0.4.2/src/uintel.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-05-08 03:59:51.000000 uintel-0.4.2/src/uintel.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      590 2023-05-08 03:59:51.000000 uintel-0.4.2/src/uintel.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-05-08 03:59:51.000000 uintel-0.4.2/src/uintel.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)      158 2023-05-08 03:59:51.000000 uintel-0.4.2/src/uintel.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        7 2023-05-08 03:59:51.000000 uintel-0.4.2/src/uintel.egg-info/top_level.txt
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 03:51:07.655203 uintel-0.4.3/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1075 2023-04-03 04:47:18.000000 uintel-0.4.3/LICENSE
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-06-07 03:51:07.655203 uintel-0.4.3/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3274 2023-04-03 04:47:18.000000 uintel-0.4.3/README.md
+-rw-rw-r--   0 sam       (1000) sam       (1000)       95 2023-04-03 04:47:18.000000 uintel-0.4.3/pyproject.toml
+-rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-06-07 03:51:07.655203 uintel-0.4.3/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1560 2023-06-07 03:50:39.000000 uintel-0.4.3/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 03:51:07.651203 uintel-0.4.3/src/
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 03:51:07.651203 uintel-0.4.3/src/uintel/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3030 2023-04-03 04:47:18.000000 uintel-0.4.3/src/uintel/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7978 2023-05-05 02:33:43.000000 uintel-0.4.3/src/uintel/aws.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4657 2023-04-03 04:47:18.000000 uintel-0.4.3/src/uintel/colours.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    10626 2023-05-05 02:33:43.000000 uintel-0.4.3/src/uintel/esri.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 03:51:07.651203 uintel-0.4.3/src/uintel/fonts/
+-rw-rw-r--   0 sam       (1000) sam       (1000)    94884 2023-04-03 04:47:18.000000 uintel-0.4.3/src/uintel/fonts/Myriad Pro (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)   208636 2023-04-03 04:47:18.000000 uintel-0.4.3/src/uintel/fonts/Rubik (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)   202424 2023-04-03 04:47:18.000000 uintel-0.4.3/src/uintel/fonts/Rubik Italic (TrueType).ttf
+-rw-rw-r--   0 sam       (1000) sam       (1000)    20898 2023-06-07 03:50:04.000000 uintel-0.4.3/src/uintel/geometry.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    23184 2023-04-03 04:47:18.000000 uintel-0.4.3/src/uintel/install.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2308 2023-04-03 04:47:18.000000 uintel-0.4.3/src/uintel/ogc.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3808 2023-04-03 04:47:18.000000 uintel-0.4.3/src/uintel/query.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7934 2023-05-05 02:33:43.000000 uintel-0.4.3/src/uintel/server.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    13281 2023-05-05 02:33:43.000000 uintel-0.4.3/src/uintel/slack.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6374 2023-05-08 03:59:28.000000 uintel-0.4.3/src/uintel/sql.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 03:51:07.655203 uintel-0.4.3/src/uintel/styles/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1046 2023-04-03 04:47:18.000000 uintel-0.4.3/src/uintel/styles/ui.mplstyle
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-07 03:51:07.651203 uintel-0.4.3/src/uintel.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4036 2023-06-07 03:51:07.000000 uintel-0.4.3/src/uintel.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      590 2023-06-07 03:51:07.000000 uintel-0.4.3/src/uintel.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-06-07 03:51:07.000000 uintel-0.4.3/src/uintel.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)      158 2023-06-07 03:51:07.000000 uintel-0.4.3/src/uintel.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        7 2023-06-07 03:51:07.000000 uintel-0.4.3/src/uintel.egg-info/top_level.txt
```

### Comparing `uintel-0.4.2/LICENSE` & `uintel-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/PKG-INFO` & `uintel-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uintel
-Version: 0.4.2
+Version: 0.4.3
 Summary: Urban Intelligence's unified Python data analysis toolkit
 Home-page: https://uintel.github.io/pyui/
 Author: Sam Archie
 Author-email: sam.archie@urbanintelligence.co.nz
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `uintel-0.4.2/README.md` & `uintel-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/setup.py` & `uintel-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 setuptools.setup(
     # State the generic information about the package
     name='uintel',
-    version='0.4.2',
+    version='0.4.3',
     author="Sam Archie",
     author_email="sam.archie@urbanintelligence.co.nz",
     description="Urban Intelligence's unified Python data analysis toolkit",
     long_description=open('README.md').read().replace("docs/images/blue_logo.svg", "https://urbanintelligence.co.nz/wp-content/uploads/2022/05/Artboard-1-copy-23.svg"),
     long_description_content_type='text/markdown',
     license="MIT",
     url="https://uintel.github.io/pyui/",
```

### Comparing `uintel-0.4.2/src/uintel/__init__.py` & `uintel-0.4.3/src/uintel/__init__.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/aws.py` & `uintel-0.4.3/src/uintel/aws.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/colours.py` & `uintel-0.4.3/src/uintel/colours.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/esri.py` & `uintel-0.4.3/src/uintel/esri.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/fonts/Myriad Pro (TrueType).ttf` & `uintel-0.4.3/src/uintel/fonts/Myriad Pro (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/fonts/Rubik (TrueType).ttf` & `uintel-0.4.3/src/uintel/fonts/Rubik (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/fonts/Rubik Italic (TrueType).ttf` & `uintel-0.4.3/src/uintel/fonts/Rubik Italic (TrueType).ttf`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/geometry.py` & `uintel-0.4.3/src/uintel/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     """
 
     # Grab the "normal" parameters to pass to ReadAsArray  
     y_top, y_bottom, x_left, x_right = offsets         
     width, height = x_right-x_left, y_bottom-y_top
    
     if width == 0 or height == 0:
-        # The  the requested raster has a zero dimension which is invalid
+        # Then the requested raster has a zero dimension which is invalid
         return None
     if x_left > raster_x_size or y_top > raster_y_size:
         # Then the starting point (top left of the polygon) is outside of the bottom right raster extent
         return None
     elif x_right < 0 or y_bottom < 0:
         # Then the finishing point (bottom right of the polygon) is outside of the top left raster extent
         return None
@@ -224,20 +224,20 @@
     else:
         warnings.warn(f"Uncaught case in zonal statistics get_raster_array! Details below:\n bounds = {offsets} with raster extends of {raster_x_size} x {raster_y_size}.")
 
 
 def calculate_zonal_statistics(raster_path: str, vector_path: str, raster_band: int = 1, allow_touching_pixels: bool = True, show_progress: bool = True) -> dict:
     """Calculate statistics of a raster over a vector geometry.
 
-    Collect stats (min, max, mean, median, std, sum, 10th percentile, 90th percentile and count) on pixel values (raster) which lie within polygons (vector). If allow_touching_pixels is set to True, then any pixel that touches the exterior of the vector geometry is included in the statistics calculation. The returned dictionary has the vector FID as the key, where the values is a dictionary mapping the statistic's name to value.
+    Collect stats (min, max, mean, median, std, sum, n_pixels, 10th percentile, 90th percentile, count and overlap) on pixel values (raster) which lie within polygons (vector). If allow_touching_pixels is set to True, then any pixel that touches the exterior of the vector geometry is included in the statistics calculation. The returned dictionary has the vector FID as the key, where the values is a dictionary mapping the statistic's name to value.
     
     Examples:
         >>> zonal_statistics = calculate_zonal_statistics("raster.tiff", "vector.shp")
         >>> zonal_statistics[67] # To get the statistics of the raster over the vector shape with an FID of 67
-        {"min": 0, "max": 10.6, "mean": 2.5, "median": 2.8, "std": 0.6, "sum": 180.8, "count": 72, "90th_percentile": 28,"10th_percentile": 0.2}      
+        {"min": 0, "max": 10.6, "mean": 2.5, "median": 2.8, "std": 0.6, "sum": 180.8, "count": 72, "n_pixels": 300, "90th_percentile": 28, "10th_percentile": 0.2, "overlap": 0.24}      
 
     Args:
         raster_path: Filepath of where the raster is stored.
         vector_path: Filepath of where the vector geometry (typically a shapefile) is stored.
         raster_band: Band of the raster to analyse.
         allow_touching_pixels: If True, any pixel that touches the exterior of the vector geometry is included in the statistics calculation. Otherwise, the statistics is using pixels within the vector geometry.
         show_progress: If True, show the progress of calculating the statistics for each vector feature.
@@ -250,15 +250,20 @@
     except ModuleNotFoundError:
         raise ModuleNotFoundError("GDAL could not be located. Please install GDAL seperately into this Python environment, or run 'pip install uintel[full]'")
     try:
         import rasterio as rio
     except ModuleNotFoundError:
         raise ModuleNotFoundError("RasterIO could not be located. Please install rasterio seperately into this Python environment, or run 'pip install uintel[full]'")
 
-    
+    raster_path = "hazard.tif"
+    vector_path = "parks.geojson"
+    raster_band = 1
+    allow_touching_pixels = True
+    show_progress = True
+
     epsg = _check_inputted_datasets(raster_path, vector_path)
 
     # Get GDAL driver
     mem_driver = osgeo.ogr.GetDriverByName("Memory")
     mem_driver_gdal = osgeo.gdal.GetDriverByName("MEM")
 
     # Open datasets
@@ -319,23 +324,25 @@
                         "min": raster_values_over_vector_feature.min(),
                         "max": raster_values_over_vector_feature.max(),
                         "mean": raster_values_over_vector_feature.mean(),
                         "median": np.median(raster_values_over_vector_feature),
                         "std": raster_values_over_vector_feature.std(),
                         "sum": raster_values_over_vector_feature.sum(),
                         "count": len(raster_values_over_vector_feature),
+                        "n_pixels": transformed_array.sum(), # A boolean array where 1 is a pixel, so the sum is how many pixels make up this polygon
                         "90th_percentile": np.percentile(raster_values_over_vector_feature, 90),
                         "10th_percentile": np.percentile(raster_values_over_vector_feature, 10)
-                        }      
+                    }
+                    zonal_statistics[id]["overlap"] = zonal_statistics[id]["count"] / zonal_statistics[id]["n_pixels"] # number of non zero pixels in cell divided by how many cells are in the polygon 
                 else:
                     # There are no raster cells overlapping the vector feature
-                    zonal_statistics[id] = {"min": None, "max": None, "mean": None, "median": None, "std": None, "sum": None, "count": None, "90th_percentile": None, "10th_percentile": None}     
+                    zonal_statistics[id] = {"min": None, "max": None, "mean": None, "median": None, "std": None, "sum": None, "count": 0, "n_pixels": transformed_array.sum(), "90th_percentile": None, "10th_percentile": None, "overlap": 0}     
             else:
                 # There is no raster?
-                zonal_statistics[id] = {"min": None, "max": None, "mean": None, "median": None, "std": None, "sum": None, "count": None, "90th_percentile": None, "10th_percentile": None}
+                zonal_statistics[id] = {"min": None, "max": None, "mean": None, "median": None, "std": None, "sum": None, "count": 0, "n_pixels": 0, "90th_percentile": None, "10th_percentile": None, "overlap": 0}
             
             # Clear some memory
             temporary_dataset = None
             temporary_layer = None
             transformed_dataset = None
             # Repeat with the next polygon geometry
             vector_feature = vector_layer.GetNextFeature()
```

### Comparing `uintel-0.4.2/src/uintel/install.py` & `uintel-0.4.3/src/uintel/install.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/ogc.py` & `uintel-0.4.3/src/uintel/ogc.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/query.py` & `uintel-0.4.3/src/uintel/query.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/server.py` & `uintel-0.4.3/src/uintel/server.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/slack.py` & `uintel-0.4.3/src/uintel/slack.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/sql.py` & `uintel-0.4.3/src/uintel/sql.py`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel/styles/ui.mplstyle` & `uintel-0.4.3/src/uintel/styles/ui.mplstyle`

 * *Files identical despite different names*

### Comparing `uintel-0.4.2/src/uintel.egg-info/PKG-INFO` & `uintel-0.4.3/src/uintel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uintel
-Version: 0.4.2
+Version: 0.4.3
 Summary: Urban Intelligence's unified Python data analysis toolkit
 Home-page: https://uintel.github.io/pyui/
 Author: Sam Archie
 Author-email: sam.archie@urbanintelligence.co.nz
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `uintel-0.4.2/src/uintel.egg-info/SOURCES.txt` & `uintel-0.4.3/src/uintel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

