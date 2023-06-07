# Comparing `tmp/artus-0.1.0.tar.gz` & `tmp/artus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artus-0.1.0.tar", last modified: Wed Jun  7 10:08:25 2023, max compression
+gzip compressed data, was "artus-0.1.1.tar", last modified: Wed Jun  7 10:19:04 2023, max compression
```

## Comparing `artus-0.1.0.tar` & `artus-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:08:25.324201 artus-0.1.0/
--rw-rw-r--   0 justine   (1000) justine   (1000)     2668 2023-06-07 10:08:25.324201 artus-0.1.0/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)     2169 2023-06-07 08:24:41.000000 artus-0.1.0/README.md
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:08:25.320201 artus-0.1.0/artus/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.1.0/artus/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:08:25.324201 artus-0.1.0/artus/evaluate_model/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.0/artus/evaluate_model/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.1.0/artus/evaluate_model/coco_stats.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.1.0/artus/evaluate_model/evaluate.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-02 10:55:35.000000 artus-0.1.0/artus/evaluate_model/write_eval_results.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:08:25.324201 artus-0.1.0/artus/inference/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.0/artus/inference/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.1.0/artus/inference/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.1.0/artus/inference/deploy_unlabeled_dataset.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)    10522 2023-06-06 07:13:05.000000 artus-0.1.0/artus/inference/predict.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:08:25.324201 artus-0.1.0/artus/prepare/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.0/artus/prepare/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.1.0/artus/prepare/coco_splitting.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.1.0/artus/prepare/crs_settings.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.1.0/artus/prepare/tile.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.1.0/artus/prepare/transform_geoson_to_coco.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:08:25.324201 artus-0.1.0/artus/spatialize/
--rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.1.0/artus/spatialize/GeoCOCOExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     7231 2023-06-06 07:14:53.000000 artus-0.1.0/artus/spatialize/GeoFiftyoneExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.0/artus/spatialize/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:08:25.324201 artus-0.1.0/artus/train/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.0/artus/train/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.1.0/artus/train/build_trainer.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.1.0/artus/train/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.1.0/artus/train/data_augmentation.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.1.0/artus/train/train.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.1.0/artus/train/validation_hook.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:08:25.324201 artus-0.1.0/artus.egg-info/
--rw-rw-r--   0 justine   (1000) justine   (1000)     2668 2023-06-07 10:08:25.000000 artus-0.1.0/artus.egg-info/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)      872 2023-06-07 10:08:25.000000 artus-0.1.0/artus.egg-info/SOURCES.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-07 10:08:25.000000 artus-0.1.0/artus.egg-info/dependency_links.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)      408 2023-06-07 10:08:25.000000 artus-0.1.0/artus.egg-info/requires.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-07 10:08:25.000000 artus-0.1.0/artus.egg-info/top_level.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)     1215 2023-06-06 11:17:59.000000 artus-0.1.0/pyproject.toml
--rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-07 10:08:25.324201 artus-0.1.0/setup.cfg
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.739368 artus-0.1.1/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2821 2023-06-07 10:19:04.735368 artus-0.1.1/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2322 2023-06-07 10:16:33.000000 artus-0.1.1/README.md
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.1.1/artus/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/evaluate_model/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.1/artus/evaluate_model/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.1.1/artus/evaluate_model/coco_stats.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.1.1/artus/evaluate_model/evaluate.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-02 10:55:35.000000 artus-0.1.1/artus/evaluate_model/write_eval_results.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/inference/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.1/artus/inference/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.1.1/artus/inference/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.1.1/artus/inference/deploy_unlabeled_dataset.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)    10522 2023-06-06 07:13:05.000000 artus-0.1.1/artus/inference/predict.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/prepare/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.1/artus/prepare/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.1.1/artus/prepare/coco_splitting.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.1.1/artus/prepare/crs_settings.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.1.1/artus/prepare/tile.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.1.1/artus/prepare/transform_geoson_to_coco.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/spatialize/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.1.1/artus/spatialize/GeoCOCOExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     7231 2023-06-06 07:14:53.000000 artus-0.1.1/artus/spatialize/GeoFiftyoneExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.1/artus/spatialize/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/train/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.1/artus/train/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.1.1/artus/train/build_trainer.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.1.1/artus/train/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.1.1/artus/train/data_augmentation.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.1.1/artus/train/train.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.1.1/artus/train/validation_hook.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus.egg-info/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2821 2023-06-07 10:19:04.000000 artus-0.1.1/artus.egg-info/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)      872 2023-06-07 10:19:04.000000 artus-0.1.1/artus.egg-info/SOURCES.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-07 10:19:04.000000 artus-0.1.1/artus.egg-info/dependency_links.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)      408 2023-06-07 10:19:04.000000 artus-0.1.1/artus.egg-info/requires.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-07 10:19:04.000000 artus-0.1.1/artus.egg-info/top_level.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)     1215 2023-06-07 10:16:48.000000 artus-0.1.1/pyproject.toml
+-rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-07 10:19:04.739368 artus-0.1.1/setup.cfg
```

### Comparing `artus-0.1.0/PKG-INFO` & `artus-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: artus
-Version: 0.1.0
+Version: 0.1.1
 Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
 Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
 Project-URL: Homepage, https://github.com/6tronl/artus
 Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
 
-<img src="docs/logo_artus.png" height="130px">
+<img src="https://github.com/6tronl/artus/blob/main/docs/logo_artus.png?raw=True" height="130px">
 
 # Predict geospatial data with artificial intelligence
 
 </div>
 
 [![Documentation Status](https://readthedocs.org/projects/artus/badge/?version=latest)](https://artus.readthedocs.io/en/latest/?badge=latest)
 [![Python package](https://github.com/6tronl/artus/actions/workflows/main.yml/badge.svg)](https://github.com/6tronl/artus/actions/workflows/main.yml)
@@ -29,19 +29,19 @@
 To handle large raster file, artus provides a way to tile raster into smaller tiles according to different cutting grids.
 
 Artus has already been implemented in three use cases using 3 differents inputs data : satellite images to detect gillnets vessels, orthomosaics to detect corals
 species and under water images marked with a georeferenced point to detect marine species.
 
 For example, the following map is generated by automatically detecting dead corals on images associated with a single GPS point:
 <div align="center">
-<img src="docs/heatmap_study_area.png" height="500px">
+<img src="https://github.com/6tronl/artus/blob/main/docs/heatmap_study_area.png?raw=True" height="500px">
 </div>
 
 This project is being developed as part of the G2OI project, cofinanced by the European union, the Reunion region, and the French Republic.
-<img src="docs/logos_partenaires.png" height="40px">
+<img src="https://github.com/6tronl/artus/blob/main/docs/logos_partenaires.png?raw=True" height="40px">
 
 ## Installation
 
 All the installation procedures are available here : [install artus](https://artus.readthedocs.io/en/latest/installation.html)
 
 ## Tutorials
```

### Comparing `artus-0.1.0/README.md` & `artus-0.1.1/artus.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,22 @@
+Metadata-Version: 2.1
+Name: artus
+Version: 0.1.1
+Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
+Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
+Project-URL: Homepage, https://github.com/6tronl/artus
+Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 <div align="center">
 
-<img src="docs/logo_artus.png" height="130px">
+<img src="https://github.com/6tronl/artus/blob/main/docs/logo_artus.png?raw=True" height="130px">
 
 # Predict geospatial data with artificial intelligence
 
 </div>
 
 [![Documentation Status](https://readthedocs.org/projects/artus/badge/?version=latest)](https://artus.readthedocs.io/en/latest/?badge=latest)
 [![Python package](https://github.com/6tronl/artus/actions/workflows/main.yml/badge.svg)](https://github.com/6tronl/artus/actions/workflows/main.yml)
@@ -17,19 +29,19 @@
 To handle large raster file, artus provides a way to tile raster into smaller tiles according to different cutting grids.
 
 Artus has already been implemented in three use cases using 3 differents inputs data : satellite images to detect gillnets vessels, orthomosaics to detect corals
 species and under water images marked with a georeferenced point to detect marine species.
 
 For example, the following map is generated by automatically detecting dead corals on images associated with a single GPS point:
 <div align="center">
-<img src="docs/heatmap_study_area.png" height="500px">
+<img src="https://github.com/6tronl/artus/blob/main/docs/heatmap_study_area.png?raw=True" height="500px">
 </div>
 
 This project is being developed as part of the G2OI project, cofinanced by the European union, the Reunion region, and the French Republic.
-<img src="docs/logos_partenaires.png" height="40px">
+<img src="https://github.com/6tronl/artus/blob/main/docs/logos_partenaires.png?raw=True" height="40px">
 
 ## Installation
 
 All the installation procedures are available here : [install artus](https://artus.readthedocs.io/en/latest/installation.html)
 
 ## Tutorials
```

### Comparing `artus-0.1.0/artus/evaluate_model/coco_stats.py` & `artus-0.1.1/artus/evaluate_model/coco_stats.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/evaluate_model/evaluate.py` & `artus-0.1.1/artus/evaluate_model/evaluate.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/evaluate_model/write_eval_results.py` & `artus-0.1.1/artus/evaluate_model/write_eval_results.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/inference/config.py` & `artus-0.1.1/artus/inference/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/inference/deploy_unlabeled_dataset.py` & `artus-0.1.1/artus/inference/deploy_unlabeled_dataset.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/inference/predict.py` & `artus-0.1.1/artus/inference/predict.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/prepare/coco_splitting.py` & `artus-0.1.1/artus/prepare/coco_splitting.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/prepare/crs_settings.py` & `artus-0.1.1/artus/prepare/crs_settings.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/prepare/tile.py` & `artus-0.1.1/artus/prepare/tile.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/prepare/transform_geoson_to_coco.py` & `artus-0.1.1/artus/prepare/transform_geoson_to_coco.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/spatialize/GeoCOCOExporter.py` & `artus-0.1.1/artus/spatialize/GeoCOCOExporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/spatialize/GeoFiftyoneExporter.py` & `artus-0.1.1/artus/spatialize/GeoFiftyoneExporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/train/build_trainer.py` & `artus-0.1.1/artus/train/build_trainer.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/train/config.py` & `artus-0.1.1/artus/train/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/train/data_augmentation.py` & `artus-0.1.1/artus/train/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/train/train.py` & `artus-0.1.1/artus/train/train.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus/train/validation_hook.py` & `artus-0.1.1/artus/train/validation_hook.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/artus.egg-info/SOURCES.txt` & `artus-0.1.1/artus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artus-0.1.0/pyproject.toml` & `artus-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "artus"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Justine Talpaert Daudon", email="justine.daudon@protonmail.com" },
 ]
 description = "A geoAI package to train and predict spatial occurences on rasters or georeferenced images."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

