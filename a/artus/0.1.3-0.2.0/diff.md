# Comparing `tmp/artus-0.1.3.tar.gz` & `tmp/artus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artus-0.1.3.tar", last modified: Wed Jun  7 10:32:17 2023, max compression
+gzip compressed data, was "artus-0.2.0.tar", last modified: Wed Jun  7 12:13:28 2023, max compression
```

## Comparing `artus-0.1.3.tar` & `artus-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/
--rw-rw-r--   0 justine   (1000) justine   (1000)     3059 2023-06-07 10:32:17.019467 artus-0.1.3/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)     2427 2023-06-07 10:22:31.000000 artus-0.1.3/README.md
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.1.3/artus/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/evaluate_model/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.3/artus/evaluate_model/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.1.3/artus/evaluate_model/coco_stats.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.1.3/artus/evaluate_model/evaluate.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-02 10:55:35.000000 artus-0.1.3/artus/evaluate_model/write_eval_results.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/inference/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.3/artus/inference/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.1.3/artus/inference/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.1.3/artus/inference/deploy_unlabeled_dataset.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)    10522 2023-06-06 07:13:05.000000 artus-0.1.3/artus/inference/predict.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/prepare/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.3/artus/prepare/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.1.3/artus/prepare/coco_splitting.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.1.3/artus/prepare/crs_settings.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.1.3/artus/prepare/tile.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.1.3/artus/prepare/transform_geoson_to_coco.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/spatialize/
--rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.1.3/artus/spatialize/GeoCOCOExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     7231 2023-06-06 07:14:53.000000 artus-0.1.3/artus/spatialize/GeoFiftyoneExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.3/artus/spatialize/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/train/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.3/artus/train/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.1.3/artus/train/build_trainer.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.1.3/artus/train/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.1.3/artus/train/data_augmentation.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.1.3/artus/train/train.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.1.3/artus/train/validation_hook.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus.egg-info/
--rw-rw-r--   0 justine   (1000) justine   (1000)     3059 2023-06-07 10:32:17.000000 artus-0.1.3/artus.egg-info/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)      872 2023-06-07 10:32:17.000000 artus-0.1.3/artus.egg-info/SOURCES.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-07 10:32:17.000000 artus-0.1.3/artus.egg-info/dependency_links.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)      408 2023-06-07 10:32:17.000000 artus-0.1.3/artus.egg-info/requires.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-07 10:32:17.000000 artus-0.1.3/artus.egg-info/top_level.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)     1331 2023-06-07 10:31:36.000000 artus-0.1.3/pyproject.toml
--rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-07 10:32:17.019467 artus-0.1.3/setup.cfg
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.291770 artus-0.2.0/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     3059 2023-06-07 12:13:28.291770 artus-0.2.0/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2427 2023-06-07 10:43:24.000000 artus-0.2.0/README.md
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.287770 artus-0.2.0/artus/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.2.0/artus/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.287770 artus-0.2.0/artus/evaluate_model/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.0/artus/evaluate_model/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.2.0/artus/evaluate_model/coco_stats.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.2.0/artus/evaluate_model/evaluate.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-02 10:55:35.000000 artus-0.2.0/artus/evaluate_model/write_eval_results.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.287770 artus-0.2.0/artus/inference/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.0/artus/inference/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.2.0/artus/inference/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.2.0/artus/inference/deploy_unlabeled_dataset.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)    10522 2023-06-06 07:13:05.000000 artus-0.2.0/artus/inference/predict.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.287770 artus-0.2.0/artus/prepare/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.0/artus/prepare/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.2.0/artus/prepare/coco_splitting.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.2.0/artus/prepare/crs_settings.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.2.0/artus/prepare/tile.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.2.0/artus/prepare/transform_geoson_to_coco.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.291770 artus-0.2.0/artus/spatialize/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.2.0/artus/spatialize/GeoCOCOExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     7851 2023-06-07 12:07:22.000000 artus-0.2.0/artus/spatialize/GeoFiftyoneExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     1218 2023-06-07 12:07:12.000000 artus-0.2.0/artus/spatialize/LocationImporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.0/artus/spatialize/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.291770 artus-0.2.0/artus/train/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.0/artus/train/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.2.0/artus/train/build_trainer.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.2.0/artus/train/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.2.0/artus/train/data_augmentation.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.2.0/artus/train/train.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.2.0/artus/train/validation_hook.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 12:13:28.287770 artus-0.2.0/artus.egg-info/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     3059 2023-06-07 12:13:28.000000 artus-0.2.0/artus.egg-info/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)      909 2023-06-07 12:13:28.000000 artus-0.2.0/artus.egg-info/SOURCES.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-07 12:13:28.000000 artus-0.2.0/artus.egg-info/dependency_links.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)      408 2023-06-07 12:13:28.000000 artus-0.2.0/artus.egg-info/requires.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-07 12:13:28.000000 artus-0.2.0/artus.egg-info/top_level.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)     1331 2023-06-07 12:06:56.000000 artus-0.2.0/pyproject.toml
+-rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-07 12:13:28.291770 artus-0.2.0/setup.cfg
```

### Comparing `artus-0.1.3/PKG-INFO` & `artus-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artus
-Version: 0.1.3
+Version: 0.2.0
 Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
 Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
 Project-URL: Homepage, https://github.com/6tronl/artus
 Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
 Project-URL: Tutorials, https://github.com/6tronl/artus-examples
 Project-URL: Documentation, https://artus.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
@@ -21,16 +21,15 @@
 </div>
 
 [![Documentation Status](https://readthedocs.org/projects/artus/badge/?version=latest)](https://artus.readthedocs.io/en/latest/?badge=latest)
 [![Python package](https://github.com/6tronl/artus/actions/workflows/main.yml/badge.svg)](https://github.com/6tronl/artus/actions/workflows/main.yml)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7852855.svg)](https://doi.org/10.5281/zenodo.7852855)
 
 Artus is a python package to automatically produce maps thanks to deep learning models. With artus, you can train deep learning learning models (neural network)
-on raster images annotated with vector files. You can then use the trained model to predict spatial occurrences on new unlabeled rasters. Predictions can be exported
-to a GeoJson format and uploaded in your favourite GIS software.
+on raster images annotated with vector files. You can then use the trained model to predict spatial occurrences on new unlabeled rasters. Predictions can be exported to a GeoJson format and uploaded in your favourite GIS software.
 
 To handle large raster file, artus provides a way to tile raster into smaller tiles according to different cutting grids.
 
 Artus has already been implemented in three use cases using 3 differents inputs data : satellite images to detect gillnets vessels, orthomosaics to detect corals
 species and under water images marked with a georeferenced point to detect marine species.
 
 For example, the following map is generated by automatically detecting dead corals on images associated with a single GPS point:
```

### Comparing `artus-0.1.3/README.md` & `artus-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 </div>
 
 [![Documentation Status](https://readthedocs.org/projects/artus/badge/?version=latest)](https://artus.readthedocs.io/en/latest/?badge=latest)
 [![Python package](https://github.com/6tronl/artus/actions/workflows/main.yml/badge.svg)](https://github.com/6tronl/artus/actions/workflows/main.yml)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7852855.svg)](https://doi.org/10.5281/zenodo.7852855)
 
 Artus is a python package to automatically produce maps thanks to deep learning models. With artus, you can train deep learning learning models (neural network)
-on raster images annotated with vector files. You can then use the trained model to predict spatial occurrences on new unlabeled rasters. Predictions can be exported
-to a GeoJson format and uploaded in your favourite GIS software.
+on raster images annotated with vector files. You can then use the trained model to predict spatial occurrences on new unlabeled rasters. Predictions can be exported to a GeoJson format and uploaded in your favourite GIS software.
 
 To handle large raster file, artus provides a way to tile raster into smaller tiles according to different cutting grids.
 
 Artus has already been implemented in three use cases using 3 differents inputs data : satellite images to detect gillnets vessels, orthomosaics to detect corals
 species and under water images marked with a georeferenced point to detect marine species.
 
 For example, the following map is generated by automatically detecting dead corals on images associated with a single GPS point:
```

### Comparing `artus-0.1.3/artus/evaluate_model/coco_stats.py` & `artus-0.2.0/artus/evaluate_model/coco_stats.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/evaluate_model/evaluate.py` & `artus-0.2.0/artus/evaluate_model/evaluate.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/evaluate_model/write_eval_results.py` & `artus-0.2.0/artus/evaluate_model/write_eval_results.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/inference/config.py` & `artus-0.2.0/artus/inference/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/inference/deploy_unlabeled_dataset.py` & `artus-0.2.0/artus/inference/deploy_unlabeled_dataset.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/inference/predict.py` & `artus-0.2.0/artus/inference/predict.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/prepare/coco_splitting.py` & `artus-0.2.0/artus/prepare/coco_splitting.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/prepare/crs_settings.py` & `artus-0.2.0/artus/prepare/crs_settings.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/prepare/tile.py` & `artus-0.2.0/artus/prepare/tile.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/prepare/transform_geoson_to_coco.py` & `artus-0.2.0/artus/prepare/transform_geoson_to_coco.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/spatialize/GeoCOCOExporter.py` & `artus-0.2.0/artus/spatialize/GeoCOCOExporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/spatialize/GeoFiftyoneExporter.py` & `artus-0.2.0/artus/spatialize/GeoFiftyoneExporter.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     )
 
 """
 
 import pandas as pd
 import fiftyone as fo
 import fiftyone.utils.data as foud
+from shapely import Point
 import geopandas
 import os
 from artus.spatialize.GeoCOCOExporter import GeoCOCOExporter
 
 class GeoFiftyoneExporter(foud.LabeledImageDatasetExporter, GeoCOCOExporter): 
     """Export a fiftyone dataset to a geospatial format (geojson).
 
@@ -128,14 +129,18 @@
             polygon = label.to_shapely(frame_size=(imw,imh))
         elif self.label_type=='polylines':
             polygon = label.to_shapely(frame_size=(imw,imh))
         return polygon
 
     def export_sample(self, image_or_path, label, metadata=None):
         """Exports the given sample to the dataset.
+            
+        If images in the dataset are tif then it will convert use the world coordinates for the masks or bbox...
+        Otherwise, if images are simply georeferenced it will assigned every label on the image to a single GPS point
+        GPS point must have been added to the dataset using :func:`artus.spatialize.LocationImporter.import_csv_locations`
 
         Args:
             image_or_path: an image or the path to the image on disk
             label: an instance of :meth:`label_cls`, or a dictionary mapping
                  field names to :class:`fiftyone.core.labels.Label` instances,
                  or ``None`` if the sample is unlabeled
             metadata (None): a :class:`fiftyone.core.metadata.ImageMetadata`
@@ -148,15 +153,20 @@
 
         # Get field values
         for n_label in getattr(label, self.label_type):
 
             img_filename = sample.filepath
             label = n_label.label
             confidence = n_label.confidence
-            geometry = self.shapely_polygons(n_label, metadata)                
+            
+            if metadata.mime_type == "image/tiff":
+                geometry = self.shapely_polygons(n_label, metadata) 
+                   
+            elif metadata.mime_type == "image/tiff" and self.sample_collection.has_field('location'):
+                geometry = Point(sample.location.point)
 
             gdf_row = (img_filename , label , confidence, geometry)
 
             self._labels.append(gdf_row)
         
         
     def close(self, *args):
@@ -175,11 +185,13 @@
             os.makedirs(self.export_dir)
             
         #convert _labels into gdf
         df = pd.DataFrame(data=self._labels, columns=self.columns_names)
         gdf = geopandas.GeoDataFrame(df, geometry='geometry')
 
         #convert pixel-values coordinates into geospatial coordinates
-        gdf['transform'] =  [self.get_transform(sample) for sample in gdf['img_filename']]
-        affine_transformed_gdf = self.affine_transform(gdf)
-        affine_transformed_gdf = affine_transformed_gdf.filter(items=['img_filename', 'label', 'confidence', 'geometry'])
-        affine_transformed_gdf.to_file(os.path.join(self.export_dir, self.dest_name), driver='GeoJSON')
+        if gdf['geometry'].geom_type.all() != 'Point':
+            gdf['transform'] =  [self.get_transform(sample) for sample in gdf['img_filename']]
+            gdf = self.affine_transform(gdf)        
+
+        gdf = gdf.filter(items=['img_filename', 'label', 'confidence', 'geometry'])
+        gdf.to_file(os.path.join(self.export_dir, self.dest_name), driver='GeoJSON')
```

### Comparing `artus-0.1.3/artus/train/build_trainer.py` & `artus-0.2.0/artus/train/build_trainer.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/train/config.py` & `artus-0.2.0/artus/train/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/train/data_augmentation.py` & `artus-0.2.0/artus/train/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/train/train.py` & `artus-0.2.0/artus/train/train.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus/train/validation_hook.py` & `artus-0.2.0/artus/train/validation_hook.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.3/artus.egg-info/PKG-INFO` & `artus-0.2.0/artus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artus
-Version: 0.1.3
+Version: 0.2.0
 Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
 Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
 Project-URL: Homepage, https://github.com/6tronl/artus
 Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
 Project-URL: Tutorials, https://github.com/6tronl/artus-examples
 Project-URL: Documentation, https://artus.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
@@ -21,16 +21,15 @@
 </div>
 
 [![Documentation Status](https://readthedocs.org/projects/artus/badge/?version=latest)](https://artus.readthedocs.io/en/latest/?badge=latest)
 [![Python package](https://github.com/6tronl/artus/actions/workflows/main.yml/badge.svg)](https://github.com/6tronl/artus/actions/workflows/main.yml)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7852855.svg)](https://doi.org/10.5281/zenodo.7852855)
 
 Artus is a python package to automatically produce maps thanks to deep learning models. With artus, you can train deep learning learning models (neural network)
-on raster images annotated with vector files. You can then use the trained model to predict spatial occurrences on new unlabeled rasters. Predictions can be exported
-to a GeoJson format and uploaded in your favourite GIS software.
+on raster images annotated with vector files. You can then use the trained model to predict spatial occurrences on new unlabeled rasters. Predictions can be exported to a GeoJson format and uploaded in your favourite GIS software.
 
 To handle large raster file, artus provides a way to tile raster into smaller tiles according to different cutting grids.
 
 Artus has already been implemented in three use cases using 3 differents inputs data : satellite images to detect gillnets vessels, orthomosaics to detect corals
 species and under water images marked with a georeferenced point to detect marine species.
 
 For example, the following map is generated by automatically detecting dead corals on images associated with a single GPS point:
```

### Comparing `artus-0.1.3/artus.egg-info/SOURCES.txt` & `artus-0.2.0/artus.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 artus/prepare/__init__.py
 artus/prepare/coco_splitting.py
 artus/prepare/crs_settings.py
 artus/prepare/tile.py
 artus/prepare/transform_geoson_to_coco.py
 artus/spatialize/GeoCOCOExporter.py
 artus/spatialize/GeoFiftyoneExporter.py
+artus/spatialize/LocationImporter.py
 artus/spatialize/__init__.py
 artus/train/__init__.py
 artus/train/build_trainer.py
 artus/train/config.py
 artus/train/data_augmentation.py
 artus/train/train.py
 artus/train/validation_hook.py
```

### Comparing `artus-0.1.3/pyproject.toml` & `artus-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "artus"
-version = "0.1.3"
+version = "0.2.0"
 authors = [
   { name="Justine Talpaert Daudon", email="justine.daudon@protonmail.com" },
 ]
 description = "A geoAI package to train and predict spatial occurences on rasters or georeferenced images."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

