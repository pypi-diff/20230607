# Comparing `tmp/artus-0.1.1.tar.gz` & `tmp/artus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artus-0.1.1.tar", last modified: Wed Jun  7 10:19:04 2023, max compression
+gzip compressed data, was "artus-0.1.3.tar", last modified: Wed Jun  7 10:32:17 2023, max compression
```

## Comparing `artus-0.1.1.tar` & `artus-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.739368 artus-0.1.1/
--rw-rw-r--   0 justine   (1000) justine   (1000)     2821 2023-06-07 10:19:04.735368 artus-0.1.1/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)     2322 2023-06-07 10:16:33.000000 artus-0.1.1/README.md
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.1.1/artus/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/evaluate_model/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.1/artus/evaluate_model/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.1.1/artus/evaluate_model/coco_stats.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.1.1/artus/evaluate_model/evaluate.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-02 10:55:35.000000 artus-0.1.1/artus/evaluate_model/write_eval_results.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/inference/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.1/artus/inference/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.1.1/artus/inference/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.1.1/artus/inference/deploy_unlabeled_dataset.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)    10522 2023-06-06 07:13:05.000000 artus-0.1.1/artus/inference/predict.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/prepare/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.1/artus/prepare/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.1.1/artus/prepare/coco_splitting.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.1.1/artus/prepare/crs_settings.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.1.1/artus/prepare/tile.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.1.1/artus/prepare/transform_geoson_to_coco.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/spatialize/
--rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.1.1/artus/spatialize/GeoCOCOExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     7231 2023-06-06 07:14:53.000000 artus-0.1.1/artus/spatialize/GeoFiftyoneExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.1/artus/spatialize/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus/train/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.1/artus/train/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.1.1/artus/train/build_trainer.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.1.1/artus/train/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.1.1/artus/train/data_augmentation.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.1.1/artus/train/train.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.1.1/artus/train/validation_hook.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:19:04.735368 artus-0.1.1/artus.egg-info/
--rw-rw-r--   0 justine   (1000) justine   (1000)     2821 2023-06-07 10:19:04.000000 artus-0.1.1/artus.egg-info/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)      872 2023-06-07 10:19:04.000000 artus-0.1.1/artus.egg-info/SOURCES.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-07 10:19:04.000000 artus-0.1.1/artus.egg-info/dependency_links.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)      408 2023-06-07 10:19:04.000000 artus-0.1.1/artus.egg-info/requires.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-07 10:19:04.000000 artus-0.1.1/artus.egg-info/top_level.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)     1215 2023-06-07 10:16:48.000000 artus-0.1.1/pyproject.toml
--rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-07 10:19:04.739368 artus-0.1.1/setup.cfg
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     3059 2023-06-07 10:32:17.019467 artus-0.1.3/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2427 2023-06-07 10:22:31.000000 artus-0.1.3/README.md
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.1.3/artus/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/evaluate_model/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.3/artus/evaluate_model/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.1.3/artus/evaluate_model/coco_stats.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.1.3/artus/evaluate_model/evaluate.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-02 10:55:35.000000 artus-0.1.3/artus/evaluate_model/write_eval_results.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/inference/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.3/artus/inference/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.1.3/artus/inference/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.1.3/artus/inference/deploy_unlabeled_dataset.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)    10522 2023-06-06 07:13:05.000000 artus-0.1.3/artus/inference/predict.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/prepare/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.3/artus/prepare/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.1.3/artus/prepare/coco_splitting.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.1.3/artus/prepare/crs_settings.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.1.3/artus/prepare/tile.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.1.3/artus/prepare/transform_geoson_to_coco.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/spatialize/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.1.3/artus/spatialize/GeoCOCOExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     7231 2023-06-06 07:14:53.000000 artus-0.1.3/artus/spatialize/GeoFiftyoneExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.3/artus/spatialize/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus/train/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.1.3/artus/train/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.1.3/artus/train/build_trainer.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.1.3/artus/train/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.1.3/artus/train/data_augmentation.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.1.3/artus/train/train.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.1.3/artus/train/validation_hook.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-07 10:32:17.019467 artus-0.1.3/artus.egg-info/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     3059 2023-06-07 10:32:17.000000 artus-0.1.3/artus.egg-info/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)      872 2023-06-07 10:32:17.000000 artus-0.1.3/artus.egg-info/SOURCES.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-07 10:32:17.000000 artus-0.1.3/artus.egg-info/dependency_links.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)      408 2023-06-07 10:32:17.000000 artus-0.1.3/artus.egg-info/requires.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-07 10:32:17.000000 artus-0.1.3/artus.egg-info/top_level.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)     1331 2023-06-07 10:31:36.000000 artus-0.1.3/pyproject.toml
+-rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-07 10:32:17.019467 artus-0.1.3/setup.cfg
```

### Comparing `artus-0.1.1/PKG-INFO` & `artus-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: artus
-Version: 0.1.1
+Version: 0.1.3
 Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
 Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
 Project-URL: Homepage, https://github.com/6tronl/artus
 Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
+Project-URL: Tutorials, https://github.com/6tronl/artus-examples
+Project-URL: Documentation, https://artus.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
 
@@ -44,10 +46,13 @@
 All the installation procedures are available here : [install artus](https://artus.readthedocs.io/en/latest/installation.html)
 
 ## Tutorials
 
 If you want to get started with artus you can follow the [notebooks](https://github.com/6tronl/artus-examples). Depending on you requirements, you will find tutorials to train
 a new deep learning model, to predict an unlabeled raster or to convert different annotations files (COCO, geojson...).
 
+## Documentation
+
+Documentation is available on [Read the docs](https://artus.readthedocs.io/en/latest/)
```

### Comparing `artus-0.1.1/README.md` & `artus-0.1.3/artus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: artus
+Version: 0.1.3
+Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
+Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
+Project-URL: Homepage, https://github.com/6tronl/artus
+Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
+Project-URL: Tutorials, https://github.com/6tronl/artus-examples
+Project-URL: Documentation, https://artus.readthedocs.io/en/latest/
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 <div align="center">
 
 <img src="https://github.com/6tronl/artus/blob/main/docs/logo_artus.png?raw=True" height="130px">
 
 # Predict geospatial data with artificial intelligence
 
 </div>
@@ -32,10 +46,13 @@
 All the installation procedures are available here : [install artus](https://artus.readthedocs.io/en/latest/installation.html)
 
 ## Tutorials
 
 If you want to get started with artus you can follow the [notebooks](https://github.com/6tronl/artus-examples). Depending on you requirements, you will find tutorials to train
 a new deep learning model, to predict an unlabeled raster or to convert different annotations files (COCO, geojson...).
 
+## Documentation
+
+Documentation is available on [Read the docs](https://artus.readthedocs.io/en/latest/)
```

### Comparing `artus-0.1.1/artus/evaluate_model/coco_stats.py` & `artus-0.1.3/artus/evaluate_model/coco_stats.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/evaluate_model/evaluate.py` & `artus-0.1.3/artus/evaluate_model/evaluate.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/evaluate_model/write_eval_results.py` & `artus-0.1.3/artus/evaluate_model/write_eval_results.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/inference/config.py` & `artus-0.1.3/artus/inference/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/inference/deploy_unlabeled_dataset.py` & `artus-0.1.3/artus/inference/deploy_unlabeled_dataset.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/inference/predict.py` & `artus-0.1.3/artus/inference/predict.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/prepare/coco_splitting.py` & `artus-0.1.3/artus/prepare/coco_splitting.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/prepare/crs_settings.py` & `artus-0.1.3/artus/prepare/crs_settings.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/prepare/tile.py` & `artus-0.1.3/artus/prepare/tile.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/prepare/transform_geoson_to_coco.py` & `artus-0.1.3/artus/prepare/transform_geoson_to_coco.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/spatialize/GeoCOCOExporter.py` & `artus-0.1.3/artus/spatialize/GeoCOCOExporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/spatialize/GeoFiftyoneExporter.py` & `artus-0.1.3/artus/spatialize/GeoFiftyoneExporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/train/build_trainer.py` & `artus-0.1.3/artus/train/build_trainer.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/train/config.py` & `artus-0.1.3/artus/train/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/train/data_augmentation.py` & `artus-0.1.3/artus/train/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/train/train.py` & `artus-0.1.3/artus/train/train.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus/train/validation_hook.py` & `artus-0.1.3/artus/train/validation_hook.py`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/artus.egg-info/PKG-INFO` & `artus-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: artus
-Version: 0.1.1
-Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
-Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
-Project-URL: Homepage, https://github.com/6tronl/artus
-Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 <div align="center">
 
 <img src="https://github.com/6tronl/artus/blob/main/docs/logo_artus.png?raw=True" height="130px">
 
 # Predict geospatial data with artificial intelligence
 
 </div>
@@ -44,10 +32,13 @@
 All the installation procedures are available here : [install artus](https://artus.readthedocs.io/en/latest/installation.html)
 
 ## Tutorials
 
 If you want to get started with artus you can follow the [notebooks](https://github.com/6tronl/artus-examples). Depending on you requirements, you will find tutorials to train
 a new deep learning model, to predict an unlabeled raster or to convert different annotations files (COCO, geojson...).
 
+## Documentation
+
+Documentation is available on [Read the docs](https://artus.readthedocs.io/en/latest/)
```

### Comparing `artus-0.1.1/artus.egg-info/SOURCES.txt` & `artus-0.1.3/artus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artus-0.1.1/pyproject.toml` & `artus-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "artus"
-version = "0.1.1"
+version = "0.1.3"
 authors = [
   { name="Justine Talpaert Daudon", email="justine.daudon@protonmail.com" },
 ]
 description = "A geoAI package to train and predict spatial occurences on rasters or georeferenced images."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -41,7 +41,9 @@
     "tensorboard>=2.12.0",
     "tqdm>=4.65.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/6tronl/artus"
 "Bug Tracker" = "https://github.com/6tronl/artus/issues"
+"Tutorials" = "https://github.com/6tronl/artus-examples"
+"Documentation" = "https://artus.readthedocs.io/en/latest/"
```

