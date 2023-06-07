# Comparing `tmp/mapreader-0.3.4.tar.gz` & `tmp/mapreader-1.0.1.post0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapreader-0.3.4.tar", last modified: Wed Mar 29 12:31:40 2023, max compression
+gzip compressed data, was "mapreader-1.0.1.post0.dev9.tar", last modified: Wed Jun  7 12:38:11 2023, max compression
```

## Comparing `mapreader-0.3.4.tar` & `mapreader-1.0.1.post0.dev9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-03-29 12:31:40.178989 mapreader-0.3.4/
--rw-r--r--   0 rwood      (504) staff       (20)     1216 2023-03-22 14:17:08.000000 mapreader-0.3.4/LICENSE
--rw-r--r--   0 rwood      (504) staff       (20)     6969 2023-03-29 12:31:40.178869 mapreader-0.3.4/PKG-INFO
--rw-r--r--   0 rwood      (504) staff       (20)     5659 2023-03-24 09:48:14.000000 mapreader-0.3.4/README.md
-drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-03-29 12:31:40.173482 mapreader-0.3.4/mapreader/
--rw-r--r--   0 rwood      (504) staff       (20)      653 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/__init__.py
-drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-03-29 12:31:40.174976 mapreader-0.3.4/mapreader/annotate/
--rw-r--r--   0 rwood      (504) staff       (20)        0 2023-03-29 09:24:14.000000 mapreader-0.3.4/mapreader/annotate/__init__.py
--rw-r--r--   0 rwood      (504) staff       (20)    19453 2023-03-29 10:18:50.000000 mapreader-0.3.4/mapreader/annotate/load_annotate.py
--rw-r--r--   0 rwood      (504) staff       (20)    25245 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/annotate/utils.py
-drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-03-29 12:31:40.175788 mapreader-0.3.4/mapreader/download/
--rw-r--r--   0 rwood      (504) staff       (20)        0 2023-03-29 09:09:12.000000 mapreader-0.3.4/mapreader/download/__init__.py
--rw-r--r--   0 rwood      (504) staff       (20)     7815 2023-03-29 10:18:50.000000 mapreader-0.3.4/mapreader/download/azure_access.py
--rw-r--r--   0 rwood      (504) staff       (20)    46623 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/download/tileserver_access.py
--rw-r--r--   0 rwood      (504) staff       (20)     5338 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/download/tileserver_helpers.py
--rw-r--r--   0 rwood      (504) staff       (20)     7788 2023-03-29 10:18:50.000000 mapreader-0.3.4/mapreader/download/tileserver_scraper.py
--rw-r--r--   0 rwood      (504) staff       (20)     4602 2023-03-29 10:18:50.000000 mapreader-0.3.4/mapreader/download/tileserver_stitcher.py
-drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-03-29 12:31:40.176209 mapreader-0.3.4/mapreader/loader/
--rw-r--r--   0 rwood      (504) staff       (20)      138 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/loader/__init__.py
--rw-r--r--   0 rwood      (504) staff       (20)    81416 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/loader/images.py
--rw-r--r--   0 rwood      (504) staff       (20)     4236 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/loader/loader.py
-drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-03-29 12:31:40.176405 mapreader-0.3.4/mapreader/process/
--rw-r--r--   0 rwood      (504) staff       (20)        0 2023-03-22 14:17:08.000000 mapreader-0.3.4/mapreader/process/__init__.py
--rw-r--r--   0 rwood      (504) staff       (20)     7701 2023-03-29 10:18:50.000000 mapreader-0.3.4/mapreader/process/process.py
-drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-03-29 12:31:40.176753 mapreader-0.3.4/mapreader/slicers/
--rw-r--r--   0 rwood      (504) staff       (20)        0 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/slicers/__init__.py
--rw-r--r--   0 rwood      (504) staff       (20)     2925 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/slicers/slicers.py
-drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-03-29 12:31:40.177373 mapreader-0.3.4/mapreader/train/
--rw-r--r--   0 rwood      (504) staff       (20)        0 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/train/__init__.py
--rw-r--r--   0 rwood      (504) staff       (20)    72492 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/train/classifier.py
--rw-r--r--   0 rwood      (504) staff       (20)    25303 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/train/classifier_context.py
--rw-r--r--   0 rwood      (504) staff       (20)     1991 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/train/custom_models.py
--rw-r--r--   0 rwood      (504) staff       (20)    23378 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/train/datasets.py
-drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-03-29 12:31:40.177895 mapreader-0.3.4/mapreader/utils/
--rw-r--r--   0 rwood      (504) staff       (20)        0 2023-03-22 14:17:08.000000 mapreader-0.3.4/mapreader/utils/__init__.py
--rw-r--r--   0 rwood      (504) staff       (20)      967 2023-03-29 12:22:50.000000 mapreader-0.3.4/mapreader/utils/compute_and_save_stats.py
--rw-r--r--   0 rwood      (504) staff       (20)     3999 2023-03-29 10:18:50.000000 mapreader-0.3.4/mapreader/utils/geo_utils.py
--rw-r--r--   0 rwood      (504) staff       (20)     1654 2023-03-29 12:04:17.000000 mapreader-0.3.4/mapreader/utils/slice_parallel.py
-drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-03-29 12:31:40.174425 mapreader-0.3.4/mapreader.egg-info/
--rw-r--r--   0 rwood      (504) staff       (20)     6969 2023-03-29 12:31:40.000000 mapreader-0.3.4/mapreader.egg-info/PKG-INFO
--rw-r--r--   0 rwood      (504) staff       (20)     1193 2023-03-29 12:31:40.000000 mapreader-0.3.4/mapreader.egg-info/SOURCES.txt
--rw-r--r--   0 rwood      (504) staff       (20)        1 2023-03-29 12:31:40.000000 mapreader-0.3.4/mapreader.egg-info/dependency_links.txt
--rw-r--r--   0 rwood      (504) staff       (20)       55 2023-03-29 12:31:40.000000 mapreader-0.3.4/mapreader.egg-info/entry_points.txt
--rw-r--r--   0 rwood      (504) staff       (20)        1 2023-03-23 14:47:41.000000 mapreader-0.3.4/mapreader.egg-info/not-zip-safe
--rw-r--r--   0 rwood      (504) staff       (20)      562 2023-03-29 12:31:40.000000 mapreader-0.3.4/mapreader.egg-info/requires.txt
--rw-r--r--   0 rwood      (504) staff       (20)       10 2023-03-29 12:31:40.000000 mapreader-0.3.4/mapreader.egg-info/top_level.txt
--rw-r--r--   0 rwood      (504) staff       (20)       38 2023-03-29 12:31:40.179028 mapreader-0.3.4/setup.cfg
--rw-r--r--   0 rwood      (504) staff       (20)     2567 2023-03-29 10:18:50.000000 mapreader-0.3.4/setup.py
-drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-03-29 12:31:40.178693 mapreader-0.3.4/tests/
--rw-r--r--   0 rwood      (504) staff       (20)     1029 2023-03-29 12:01:25.000000 mapreader-0.3.4/tests/test_geo_utils.py
--rw-r--r--   0 rwood      (504) staff       (20)       68 2023-03-22 14:17:08.000000 mapreader-0.3.4/tests/test_import.py
--rw-r--r--   0 rwood      (504) staff       (20)     5618 2023-03-29 12:22:50.000000 mapreader-0.3.4/tests/test_loader.py
--rw-r--r--   0 rwood      (504) staff       (20)     8009 2023-03-29 12:22:50.000000 mapreader-0.3.4/tests/test_non_geo_pipeline.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.913844 mapreader-1.0.1.post0.dev9/
+-rw-r--r--   0 rwood      (504) staff       (20)     1216 2023-03-22 14:17:08.000000 mapreader-1.0.1.post0.dev9/LICENSE
+-rw-r--r--   0 rwood      (504) staff       (20)     7277 2023-06-07 12:38:11.913897 mapreader-1.0.1.post0.dev9/PKG-INFO
+-rw-r--r--   0 rwood      (504) staff       (20)     5949 2023-06-06 16:21:10.000000 mapreader-1.0.1.post0.dev9/README.md
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.914221 mapreader-1.0.1.post0.dev9/mapreader/
+-rw-r--r--   0 rwood      (504) staff       (20)      867 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)      508 2023-06-07 12:38:11.914250 mapreader-1.0.1.post0.dev9/mapreader/_version.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.910724 mapreader-1.0.1.post0.dev9/mapreader/annotate/
+-rw-r--r--   0 rwood      (504) staff       (20)        0 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/annotate/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)    24794 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/annotate/utils.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.911521 mapreader-1.0.1.post0.dev9/mapreader/classify/
+-rw-r--r--   0 rwood      (504) staff       (20)        0 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)    73307 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/classifier.py
+-rw-r--r--   0 rwood      (504) staff       (20)    27268 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/classifier_context.py
+-rw-r--r--   0 rwood      (504) staff       (20)     1991 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/custom_models.py
+-rw-r--r--   0 rwood      (504) staff       (20)    28572 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/datasets.py
+-rw-r--r--   0 rwood      (504) staff       (20)    25048 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/classify/load_annotations.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.912334 mapreader-1.0.1.post0.dev9/mapreader/download/
+-rw-r--r--   0 rwood      (504) staff       (20)        0 2023-05-04 15:10:34.000000 mapreader-1.0.1.post0.dev9/mapreader/download/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)     2285 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/data_structures.py
+-rw-r--r--   0 rwood      (504) staff       (20)     4564 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/downloader.py
+-rw-r--r--   0 rwood      (504) staff       (20)     4553 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/downloader_utils.py
+-rw-r--r--   0 rwood      (504) staff       (20)    38174 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/sheet_downloader.py
+-rw-r--r--   0 rwood      (504) staff       (20)     6430 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/tile_loading.py
+-rw-r--r--   0 rwood      (504) staff       (20)     5832 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/download/tile_merging.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.912820 mapreader-1.0.1.post0.dev9/mapreader/load/
+-rw-r--r--   0 rwood      (504) staff       (20)      132 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/load/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)     3676 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/mapreader/load/geo_utils.py
+-rw-r--r--   0 rwood      (504) staff       (20)    86859 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/load/images.py
+-rw-r--r--   0 rwood      (504) staff       (20)     4846 2023-06-05 15:21:44.000000 mapreader-1.0.1.post0.dev9/mapreader/load/loader.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.913008 mapreader-1.0.1.post0.dev9/mapreader/process/
+-rw-r--r--   0 rwood      (504) staff       (20)        0 2023-03-22 14:17:08.000000 mapreader-1.0.1.post0.dev9/mapreader/process/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)     7669 2023-05-09 12:50:40.000000 mapreader-1.0.1.post0.dev9/mapreader/process/process.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.913318 mapreader-1.0.1.post0.dev9/mapreader/utils/
+-rw-r--r--   0 rwood      (504) staff       (20)        0 2023-03-22 14:17:08.000000 mapreader-1.0.1.post0.dev9/mapreader/utils/__init__.py
+-rw-r--r--   0 rwood      (504) staff       (20)      967 2023-05-09 12:50:40.000000 mapreader-1.0.1.post0.dev9/mapreader/utils/compute_and_save_stats.py
+-rw-r--r--   0 rwood      (504) staff       (20)     1654 2023-04-25 09:23:09.000000 mapreader-1.0.1.post0.dev9/mapreader/utils/slice_parallel.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.910527 mapreader-1.0.1.post0.dev9/mapreader.egg-info/
+-rw-r--r--   0 rwood      (504) staff       (20)     7277 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/PKG-INFO
+-rw-r--r--   0 rwood      (504) staff       (20)     1224 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/SOURCES.txt
+-rw-r--r--   0 rwood      (504) staff       (20)        1 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/dependency_links.txt
+-rw-r--r--   0 rwood      (504) staff       (20)       55 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/entry_points.txt
+-rw-r--r--   0 rwood      (504) staff       (20)        1 2023-03-23 14:47:41.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/not-zip-safe
+-rw-r--r--   0 rwood      (504) staff       (20)      603 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/requires.txt
+-rw-r--r--   0 rwood      (504) staff       (20)       10 2023-06-07 12:38:11.000000 mapreader-1.0.1.post0.dev9/mapreader.egg-info/top_level.txt
+-rw-r--r--   0 rwood      (504) staff       (20)      211 2023-06-07 12:38:11.914097 mapreader-1.0.1.post0.dev9/setup.cfg
+-rw-r--r--   0 rwood      (504) staff       (20)     2764 2023-06-06 16:21:10.000000 mapreader-1.0.1.post0.dev9/setup.py
+drwxr-xr-x   0 rwood      (504) staff       (20)        0 2023-06-07 12:38:11.913750 mapreader-1.0.1.post0.dev9/tests/
+-rw-r--r--   0 rwood      (504) staff       (20)     3993 2023-06-05 15:21:45.000000 mapreader-1.0.1.post0.dev9/tests/test_annotations_loader.py
+-rw-r--r--   0 rwood      (504) staff       (20)     5335 2023-06-05 15:21:45.000000 mapreader-1.0.1.post0.dev9/tests/test_classifier.py
+-rw-r--r--   0 rwood      (504) staff       (20)      577 2023-06-05 15:21:45.000000 mapreader-1.0.1.post0.dev9/tests/test_import.py
+-rw-r--r--   0 rwood      (504) staff       (20)    14024 2023-05-24 14:03:30.000000 mapreader-1.0.1.post0.dev9/tests/test_sheet_downloader.py
+-rw-r--r--   0 rwood      (504) staff       (20)    83607 2023-04-25 09:23:09.000000 mapreader-1.0.1.post0.dev9/versioneer.py
```

### Comparing `mapreader-0.3.4/LICENSE` & `mapreader-1.0.1.post0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `mapreader-0.3.4/PKG-INFO` & `mapreader-1.0.1.post0.dev9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 0.3.4
+Version: 1.0.1.post0.dev9
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
@@ -20,15 +20,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
     <br>
     <p align="center">
     <h1>MapReader</h1>
@@ -48,80 +48,79 @@
     </a>
     <br/>
 </p>
 
 
 ## What is MapReader?
 
-<!--- picture here? --->
-<p align="center">
-  <figure>
-  <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/figs/river_banner_8bit.png"
+<div align="center">
+    <figure>
+    <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/figs/river_banner_8bit.png"
         alt="Annotated Map with Prediction Outputs"
         width="70%">
-  </figure>
-</p>
+    </figure>
+</div>
 
 MapReader is an end-to-end computer vision (CV) pipeline for exploring and analyzing images at scale. 
 
-MapReader was developed in the [Living with Machines](https://livingwithmachines.ac.uk/) project to analyze large collections of historical maps but is a _**generalisable**_ computer vision pipeline which can be applied to _**any images**_ in a wide variety of domains. 
+MapReader was developed in the [Living with Machines](https://livingwithmachines.ac.uk/) project to analyze large collections of historical maps but is a _**generalizable**_ computer vision pipeline which can be applied to _**any images**_ in a wide variety of domains. 
 
 
 ## Overview
 
-MapReader is a groundbreaking interdisciplinary tool that emerged from a specific set of geospatial historical research questions. It was inspired by methods in biomedical imaging and geographic information science, which were adapted for annotation and use by historians, for example in [JVC](https://doi.org/10.1093/jvcult/vcab009) and [MapReader](https://arxiv.org/abs/2111.15592) papers. The success of the tool subsequently generated interest from plant phenotype researchers working with large image datasets, and so MapReader is an example of cross-pollination between the humanities and the sciences made possible by reproducible data science.
+MapReader is a groundbreaking interdisciplinary tool that emerged from a specific set of geospatial historical research questions. It was inspired by methods in biomedical imaging and geographic information science, which were adapted for use by historians, for example in our [Journal of Victorian Culture](https://doi.org/10.1093/jvcult/vcab009) and [Geospatial Humanities 2022 SIGSPATIAL workshop](https://arxiv.org/abs/2111.15592) papers. The success of the tool subsequently generated interest from plant phenotype researchers working with large image datasets, and so MapReader is an example of cross-pollination between the humanities and the sciences made possible by reproducible data science.
 
 ### MapReader pipeline 
 
-The MapReader pipeline consists of two main components:
-1. preprocessing/annotation 
-2. training/inference
-
-<p align="center">
+<div align="center">
   <figure>
-  <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/figs/MapReader_pipeline.png"
+  <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/docs/source/figures/pipeline_explained.png"
         alt="MapReader pipeline"
         width="70%">
   </figure>
-</p>
-
-
-### What is included?
-
-The MapReader package provides a set of tools to:
+</div>
 
-- **download** images/maps and metadata stored on web-servers (e.g. tileserves which can be used to retrieve maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or elsewhere).
-- **load** images/maps and metadata stored locally.
-- **preprocess** images/maps:
-  - patchify (create patches from a parent image), 
-  - resample (use image transformations to alter pixel-dimensions/resolution/orientation/etc.),
-  - remove borders outside the neatline,
-  - reproject between coordinate reference systems (CRS).
-- **annotate** images/maps (or their patches) using an interactive annotation tool.
-- **train, fine-tune, and evaluate** Computer Vision (CV) models and use these to **predict** labels (i.e. model inference) on large sets of images/maps.
+The MapReader pipeline consists of a linear sequence of tasks which, together, can be used to train a computer vision (CV) classifier to recognise visual features within maps and identify patches containing these features across entire map collections.
 
-Various **plotting and analysis** functionalities are also included (based on packages such as *matplotlib*, *cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)).
+See our [About MapReader](https://mapreader.readthedocs.io/en/latest/About.html) page to learn more.
 
-<!--- or mb picture here? --->
 
 ## Documentation 
 
-The MapReader documentation can be found [here](https://mapreader.readthedocs.io/en/latest/index.html).
+The MapReader documentation can be found at https://mapreader.readthedocs.io/en/latest/index.html.
 
-**New users** should refer to the [Installation instructions](https://mapreader.readthedocs.io/en/latest/Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/Input-guidance.html) for guidance on the initial set up of MapReader.
+**New users** should refer to the [Installation instructions](https://mapreader.readthedocs.io/en/latest/Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/Input-guidance.html) for help with the initial set up of MapReader.
 
-**All users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/latest/User-guide.html) for guidance on how to use MapReader. This contains end-to-end instructions on how to use the MapReader pipeline, plus a number of worked examples illustratng use cases such as:
+**All users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/latest/User-guide/User-guide.html) for guidance on how to use MapReader. This contains end-to-end instructions on how to use the MapReader pipeline, plus a number of worked examples illustratng use cases such as:
 - Geospatial images (i.e. maps)
 - Non-geospatial images 
 
  **Developers and contributors** may also want to refer to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how to contribute to the MapReader package.
+ 
+ 
+## What is included in this repo?
+
+The MapReader package provides a set of tools to:
+
+- **Download** images/maps and metadata stored on web-servers (e.g. tileserves which can be used to retrieve maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or elsewhere).
+- **Load** images/maps and metadata stored locally.
+- **Preprocess** images/maps:
+  - patchify (create patches from a parent image), 
+  - resample (use image transformations to alter pixel-dimensions/resolution/orientation/etc.),
+  - remove borders outside the neatline,
+  - reproject between coordinate reference systems (CRS).
+- **Annotate** images/maps (or their patches) using an interactive annotation tool.
+- **Train or fine-tune** Computer Vision (CV) models and use these to **predict** labels (i.e. model inference) on large sets of images/maps.
+
+Various **plotting and analysis** functionalities are also included (based on packages such as *matplotlib*, *cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)).
+
 
 ## How to cite MapReader
 
-If you use MapReader in your work, please consider acknowledging us by citing [our paper](https://dl.acm.org/doi/10.1145/3557919.3565812):
+If you use MapReader in your work, please consider acknowledging us by citing [our SIGSPATIAL paper](https://dl.acm.org/doi/10.1145/3557919.3565812):
 
 - Kasra Hosseini, Daniel C. S. Wilson, Kaspar Beelen, and Katherine McDonough. 2022. MapReader: a computer vision pipeline for the semantic exploration of maps at scale. In Proceedings of the 6th ACM SIGSPATIAL International Workshop on Geospatial Humanities (GeoHumanities '22). Association for Computing Machinery, New York, NY, USA, 8–19. https://doi.org/10.1145/3557919.3565812
 
 
 ## Acknowledgements
 
 This work was supported by Living with Machines (AHRC grant AH/S01179X/1) and The Alan Turing Institute (EPSRC grant EP/N510129/1).
```

#### html2text {}

```diff
@@ -1,79 +1,84 @@
-Metadata-Version: 2.1 Name: mapreader Version: 0.3.4 Summary: A computer vision
-pipeline for the semantic exploration of maps/images at scale Home-page: https:
-//github.com/Living-with-machines/MapReader Download-URL: https://github.com/
-Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
-team License: MIT License Keywords: Computer Vision,Classification,Deep
-Learning,living with machines Platform: OS Independent Classifier: Development
-Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Intended Audience :: End Users/Desktop Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: Science/Research Classifier: Operating System :: Unix Classifier:
-Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
-Classifier: Operating System :: OS Independent Classifier: Topic :: Software
-Development Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: mapreader Version: 1.0.1.post0.dev9 Summary: A
+computer vision pipeline for the semantic exploration of maps/images at scale
+Home-page: https://github.com/Living-with-machines/MapReader Download-URL:
+https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
+Author: MapReader team License: MIT License Keywords: Computer
+Vision,Classification,Deep Learning,living with machines Platform: OS
+Independent Classifier: Development Status :: 3 - Alpha Classifier: License ::
+OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Intended Audience :: End Users/Desktop Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research Classifier: Operating System
+:: Unix Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: MacOS Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Requires-Python: >=3.7, <3.11
+Description-Content-Type: text/markdown License-File: LICENSE
 
                             ****** MapReader ******
  ***** A computer vision pipeline for exploring and analyzing images at scale
                                      *****
                   [PyPI] [License] [Integration_Tests_badge]
 ## What is MapReader?
                     [Annotated Map with Prediction Outputs]
 MapReader is an end-to-end computer vision (CV) pipeline for exploring and
 analyzing images at scale. MapReader was developed in the [Living with
 Machines](https://livingwithmachines.ac.uk/) project to analyze large
-collections of historical maps but is a _**generalisable**_ computer vision
+collections of historical maps but is a _**generalizable**_ computer vision
 pipeline which can be applied to _**any images**_ in a wide variety of domains.
 ## Overview MapReader is a groundbreaking interdisciplinary tool that emerged
 from a specific set of geospatial historical research questions. It was
 inspired by methods in biomedical imaging and geographic information science,
-which were adapted for annotation and use by historians, for example in [JVC]
-(https://doi.org/10.1093/jvcult/vcab009) and [MapReader](https://arxiv.org/abs/
-2111.15592) papers. The success of the tool subsequently generated interest
-from plant phenotype researchers working with large image datasets, and so
-MapReader is an example of cross-pollination between the humanities and the
-sciences made possible by reproducible data science. ### MapReader pipeline The
-MapReader pipeline consists of two main components: 1. preprocessing/annotation
-2. training/inference
+which were adapted for use by historians, for example in our [Journal of
+Victorian Culture](https://doi.org/10.1093/jvcult/vcab009) and [Geospatial
+Humanities 2022 SIGSPATIAL workshop](https://arxiv.org/abs/2111.15592) papers.
+The success of the tool subsequently generated interest from plant phenotype
+researchers working with large image datasets, and so MapReader is an example
+of cross-pollination between the humanities and the sciences made possible by
+reproducible data science. ### MapReader pipeline
                              [MapReader pipeline]
-### What is included? The MapReader package provides a set of tools to: -
-**download** images/maps and metadata stored on web-servers (e.g. tileserves
-which can be used to retrieve maps from OpenStreetMap (OSM), the National
-Library of Scotland (NLS), or elsewhere). - **load** images/maps and metadata
-stored locally. - **preprocess** images/maps: - patchify (create patches from a
-parent image), - resample (use image transformations to alter pixel-dimensions/
-resolution/orientation/etc.), - remove borders outside the neatline, -
-reproject between coordinate reference systems (CRS). - **annotate** images/
-maps (or their patches) using an interactive annotation tool. - **train, fine-
-tune, and evaluate** Computer Vision (CV) models and use these to **predict**
-labels (i.e. model inference) on large sets of images/maps. Various **plotting
-and analysis** functionalities are also included (based on packages such as
-*matplotlib*, *cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)).
-## Documentation The MapReader documentation can be found [here](https://
-mapreader.readthedocs.io/en/latest/index.html). **New users** should refer to
+The MapReader pipeline consists of a linear sequence of tasks which, together,
+can be used to train a computer vision (CV) classifier to recognise visual
+features within maps and identify patches containing these features across
+entire map collections. See our [About MapReader](https://
+mapreader.readthedocs.io/en/latest/About.html) page to learn more. ##
+Documentation The MapReader documentation can be found at https://
+mapreader.readthedocs.io/en/latest/index.html. **New users** should refer to
 the [Installation instructions](https://mapreader.readthedocs.io/en/latest/
 Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/
-Input-guidance.html) for guidance on the initial set up of MapReader. **All
+Input-guidance.html) for help with the initial set up of MapReader. **All
 users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/
-latest/User-guide.html) for guidance on how to use MapReader. This contains
-end-to-end instructions on how to use the MapReader pipeline, plus a number of
-worked examples illustratng use cases such as: - Geospatial images (i.e. maps)
-- Non-geospatial images **Developers and contributors** may also want to refer
-to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/
-index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/
-latest/Contribution-guide.html) for guidance on how to contribute to the
-MapReader package. ## How to cite MapReader If you use MapReader in your work,
-please consider acknowledging us by citing [our paper](https://dl.acm.org/doi/
-10.1145/3557919.3565812): - Kasra Hosseini, Daniel C. S. Wilson, Kaspar Beelen,
-and Katherine McDonough. 2022. MapReader: a computer vision pipeline for the
+latest/User-guide/User-guide.html) for guidance on how to use MapReader. This
+contains end-to-end instructions on how to use the MapReader pipeline, plus a
+number of worked examples illustratng use cases such as: - Geospatial images
+(i.e. maps) - Non-geospatial images **Developers and contributors** may also
+want to refer to the [API documentation](https://mapreader.readthedocs.io/en/
+latest/api/index.html) and [Contribution guide](https://
+mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how
+to contribute to the MapReader package. ## What is included in this repo? The
+MapReader package provides a set of tools to: - **Download** images/maps and
+metadata stored on web-servers (e.g. tileserves which can be used to retrieve
+maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or
+elsewhere). - **Load** images/maps and metadata stored locally. -
+**Preprocess** images/maps: - patchify (create patches from a parent image), -
+resample (use image transformations to alter pixel-dimensions/resolution/
+orientation/etc.), - remove borders outside the neatline, - reproject between
+coordinate reference systems (CRS). - **Annotate** images/maps (or their
+patches) using an interactive annotation tool. - **Train or fine-tune**
+Computer Vision (CV) models and use these to **predict** labels (i.e. model
+inference) on large sets of images/maps. Various **plotting and analysis**
+functionalities are also included (based on packages such as *matplotlib*,
+*cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)). ## How to cite
+MapReader If you use MapReader in your work, please consider acknowledging us
+by citing [our SIGSPATIAL paper](https://dl.acm.org/doi/10.1145/
+3557919.3565812): - Kasra Hosseini, Daniel C. S. Wilson, Kaspar Beelen, and
+Katherine McDonough. 2022. MapReader: a computer vision pipeline for the
 semantic exploration of maps at scale. In Proceedings of the 6th ACM SIGSPATIAL
 International Workshop on Geospatial Humanities (GeoHumanities '22).
 Association for Computing Machinery, New York, NY, USA, 8â19. https://
 doi.org/10.1145/3557919.3565812 ## Acknowledgements This work was supported by
 Living with Machines (AHRC grant AH/S01179X/1) and The Alan Turing Institute
 (EPSRC grant EP/N510129/1). Living with Machines, funded by the UK Research and
 Innovation (UKRI) Strategic Priority Fund, is a multidisciplinary collaboration
```

### Comparing `mapreader-0.3.4/README.md` & `mapreader-1.0.1.post0.dev9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,80 +18,79 @@
     </a>
     <br/>
 </p>
 
 
 ## What is MapReader?
 
-<!--- picture here? --->
-<p align="center">
-  <figure>
-  <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/figs/river_banner_8bit.png"
+<div align="center">
+    <figure>
+    <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/figs/river_banner_8bit.png"
         alt="Annotated Map with Prediction Outputs"
         width="70%">
-  </figure>
-</p>
+    </figure>
+</div>
 
 MapReader is an end-to-end computer vision (CV) pipeline for exploring and analyzing images at scale. 
 
-MapReader was developed in the [Living with Machines](https://livingwithmachines.ac.uk/) project to analyze large collections of historical maps but is a _**generalisable**_ computer vision pipeline which can be applied to _**any images**_ in a wide variety of domains. 
+MapReader was developed in the [Living with Machines](https://livingwithmachines.ac.uk/) project to analyze large collections of historical maps but is a _**generalizable**_ computer vision pipeline which can be applied to _**any images**_ in a wide variety of domains. 
 
 
 ## Overview
 
-MapReader is a groundbreaking interdisciplinary tool that emerged from a specific set of geospatial historical research questions. It was inspired by methods in biomedical imaging and geographic information science, which were adapted for annotation and use by historians, for example in [JVC](https://doi.org/10.1093/jvcult/vcab009) and [MapReader](https://arxiv.org/abs/2111.15592) papers. The success of the tool subsequently generated interest from plant phenotype researchers working with large image datasets, and so MapReader is an example of cross-pollination between the humanities and the sciences made possible by reproducible data science.
+MapReader is a groundbreaking interdisciplinary tool that emerged from a specific set of geospatial historical research questions. It was inspired by methods in biomedical imaging and geographic information science, which were adapted for use by historians, for example in our [Journal of Victorian Culture](https://doi.org/10.1093/jvcult/vcab009) and [Geospatial Humanities 2022 SIGSPATIAL workshop](https://arxiv.org/abs/2111.15592) papers. The success of the tool subsequently generated interest from plant phenotype researchers working with large image datasets, and so MapReader is an example of cross-pollination between the humanities and the sciences made possible by reproducible data science.
 
 ### MapReader pipeline 
 
-The MapReader pipeline consists of two main components:
-1. preprocessing/annotation 
-2. training/inference
-
-<p align="center">
+<div align="center">
   <figure>
-  <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/figs/MapReader_pipeline.png"
+  <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/docs/source/figures/pipeline_explained.png"
         alt="MapReader pipeline"
         width="70%">
   </figure>
-</p>
-
+</div>
 
-### What is included?
-
-The MapReader package provides a set of tools to:
-
-- **download** images/maps and metadata stored on web-servers (e.g. tileserves which can be used to retrieve maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or elsewhere).
-- **load** images/maps and metadata stored locally.
-- **preprocess** images/maps:
-  - patchify (create patches from a parent image), 
-  - resample (use image transformations to alter pixel-dimensions/resolution/orientation/etc.),
-  - remove borders outside the neatline,
-  - reproject between coordinate reference systems (CRS).
-- **annotate** images/maps (or their patches) using an interactive annotation tool.
-- **train, fine-tune, and evaluate** Computer Vision (CV) models and use these to **predict** labels (i.e. model inference) on large sets of images/maps.
+The MapReader pipeline consists of a linear sequence of tasks which, together, can be used to train a computer vision (CV) classifier to recognise visual features within maps and identify patches containing these features across entire map collections.
 
-Various **plotting and analysis** functionalities are also included (based on packages such as *matplotlib*, *cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)).
+See our [About MapReader](https://mapreader.readthedocs.io/en/latest/About.html) page to learn more.
 
-<!--- or mb picture here? --->
 
 ## Documentation 
 
-The MapReader documentation can be found [here](https://mapreader.readthedocs.io/en/latest/index.html).
+The MapReader documentation can be found at https://mapreader.readthedocs.io/en/latest/index.html.
 
-**New users** should refer to the [Installation instructions](https://mapreader.readthedocs.io/en/latest/Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/Input-guidance.html) for guidance on the initial set up of MapReader.
+**New users** should refer to the [Installation instructions](https://mapreader.readthedocs.io/en/latest/Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/Input-guidance.html) for help with the initial set up of MapReader.
 
-**All users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/latest/User-guide.html) for guidance on how to use MapReader. This contains end-to-end instructions on how to use the MapReader pipeline, plus a number of worked examples illustratng use cases such as:
+**All users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/latest/User-guide/User-guide.html) for guidance on how to use MapReader. This contains end-to-end instructions on how to use the MapReader pipeline, plus a number of worked examples illustratng use cases such as:
 - Geospatial images (i.e. maps)
 - Non-geospatial images 
 
  **Developers and contributors** may also want to refer to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how to contribute to the MapReader package.
+ 
+ 
+## What is included in this repo?
+
+The MapReader package provides a set of tools to:
+
+- **Download** images/maps and metadata stored on web-servers (e.g. tileserves which can be used to retrieve maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or elsewhere).
+- **Load** images/maps and metadata stored locally.
+- **Preprocess** images/maps:
+  - patchify (create patches from a parent image), 
+  - resample (use image transformations to alter pixel-dimensions/resolution/orientation/etc.),
+  - remove borders outside the neatline,
+  - reproject between coordinate reference systems (CRS).
+- **Annotate** images/maps (or their patches) using an interactive annotation tool.
+- **Train or fine-tune** Computer Vision (CV) models and use these to **predict** labels (i.e. model inference) on large sets of images/maps.
+
+Various **plotting and analysis** functionalities are also included (based on packages such as *matplotlib*, *cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)).
+
 
 ## How to cite MapReader
 
-If you use MapReader in your work, please consider acknowledging us by citing [our paper](https://dl.acm.org/doi/10.1145/3557919.3565812):
+If you use MapReader in your work, please consider acknowledging us by citing [our SIGSPATIAL paper](https://dl.acm.org/doi/10.1145/3557919.3565812):
 
 - Kasra Hosseini, Daniel C. S. Wilson, Kaspar Beelen, and Katherine McDonough. 2022. MapReader: a computer vision pipeline for the semantic exploration of maps at scale. In Proceedings of the 6th ACM SIGSPATIAL International Workshop on Geospatial Humanities (GeoHumanities '22). Association for Computing Machinery, New York, NY, USA, 8–19. https://doi.org/10.1145/3557919.3565812
 
 
 ## Acknowledgements
 
 This work was supported by Living with Machines (AHRC grant AH/S01179X/1) and The Alan Turing Institute (EPSRC grant EP/N510129/1).
```

#### html2text {}

```diff
@@ -4,58 +4,63 @@
                                      *****
                   [PyPI] [License] [Integration_Tests_badge]
 ## What is MapReader?
                     [Annotated Map with Prediction Outputs]
 MapReader is an end-to-end computer vision (CV) pipeline for exploring and
 analyzing images at scale. MapReader was developed in the [Living with
 Machines](https://livingwithmachines.ac.uk/) project to analyze large
-collections of historical maps but is a _**generalisable**_ computer vision
+collections of historical maps but is a _**generalizable**_ computer vision
 pipeline which can be applied to _**any images**_ in a wide variety of domains.
 ## Overview MapReader is a groundbreaking interdisciplinary tool that emerged
 from a specific set of geospatial historical research questions. It was
 inspired by methods in biomedical imaging and geographic information science,
-which were adapted for annotation and use by historians, for example in [JVC]
-(https://doi.org/10.1093/jvcult/vcab009) and [MapReader](https://arxiv.org/abs/
-2111.15592) papers. The success of the tool subsequently generated interest
-from plant phenotype researchers working with large image datasets, and so
-MapReader is an example of cross-pollination between the humanities and the
-sciences made possible by reproducible data science. ### MapReader pipeline The
-MapReader pipeline consists of two main components: 1. preprocessing/annotation
-2. training/inference
+which were adapted for use by historians, for example in our [Journal of
+Victorian Culture](https://doi.org/10.1093/jvcult/vcab009) and [Geospatial
+Humanities 2022 SIGSPATIAL workshop](https://arxiv.org/abs/2111.15592) papers.
+The success of the tool subsequently generated interest from plant phenotype
+researchers working with large image datasets, and so MapReader is an example
+of cross-pollination between the humanities and the sciences made possible by
+reproducible data science. ### MapReader pipeline
                              [MapReader pipeline]
-### What is included? The MapReader package provides a set of tools to: -
-**download** images/maps and metadata stored on web-servers (e.g. tileserves
-which can be used to retrieve maps from OpenStreetMap (OSM), the National
-Library of Scotland (NLS), or elsewhere). - **load** images/maps and metadata
-stored locally. - **preprocess** images/maps: - patchify (create patches from a
-parent image), - resample (use image transformations to alter pixel-dimensions/
-resolution/orientation/etc.), - remove borders outside the neatline, -
-reproject between coordinate reference systems (CRS). - **annotate** images/
-maps (or their patches) using an interactive annotation tool. - **train, fine-
-tune, and evaluate** Computer Vision (CV) models and use these to **predict**
-labels (i.e. model inference) on large sets of images/maps. Various **plotting
-and analysis** functionalities are also included (based on packages such as
-*matplotlib*, *cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)).
-## Documentation The MapReader documentation can be found [here](https://
-mapreader.readthedocs.io/en/latest/index.html). **New users** should refer to
+The MapReader pipeline consists of a linear sequence of tasks which, together,
+can be used to train a computer vision (CV) classifier to recognise visual
+features within maps and identify patches containing these features across
+entire map collections. See our [About MapReader](https://
+mapreader.readthedocs.io/en/latest/About.html) page to learn more. ##
+Documentation The MapReader documentation can be found at https://
+mapreader.readthedocs.io/en/latest/index.html. **New users** should refer to
 the [Installation instructions](https://mapreader.readthedocs.io/en/latest/
 Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/
-Input-guidance.html) for guidance on the initial set up of MapReader. **All
+Input-guidance.html) for help with the initial set up of MapReader. **All
 users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/
-latest/User-guide.html) for guidance on how to use MapReader. This contains
-end-to-end instructions on how to use the MapReader pipeline, plus a number of
-worked examples illustratng use cases such as: - Geospatial images (i.e. maps)
-- Non-geospatial images **Developers and contributors** may also want to refer
-to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/
-index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/
-latest/Contribution-guide.html) for guidance on how to contribute to the
-MapReader package. ## How to cite MapReader If you use MapReader in your work,
-please consider acknowledging us by citing [our paper](https://dl.acm.org/doi/
-10.1145/3557919.3565812): - Kasra Hosseini, Daniel C. S. Wilson, Kaspar Beelen,
-and Katherine McDonough. 2022. MapReader: a computer vision pipeline for the
+latest/User-guide/User-guide.html) for guidance on how to use MapReader. This
+contains end-to-end instructions on how to use the MapReader pipeline, plus a
+number of worked examples illustratng use cases such as: - Geospatial images
+(i.e. maps) - Non-geospatial images **Developers and contributors** may also
+want to refer to the [API documentation](https://mapreader.readthedocs.io/en/
+latest/api/index.html) and [Contribution guide](https://
+mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how
+to contribute to the MapReader package. ## What is included in this repo? The
+MapReader package provides a set of tools to: - **Download** images/maps and
+metadata stored on web-servers (e.g. tileserves which can be used to retrieve
+maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or
+elsewhere). - **Load** images/maps and metadata stored locally. -
+**Preprocess** images/maps: - patchify (create patches from a parent image), -
+resample (use image transformations to alter pixel-dimensions/resolution/
+orientation/etc.), - remove borders outside the neatline, - reproject between
+coordinate reference systems (CRS). - **Annotate** images/maps (or their
+patches) using an interactive annotation tool. - **Train or fine-tune**
+Computer Vision (CV) models and use these to **predict** labels (i.e. model
+inference) on large sets of images/maps. Various **plotting and analysis**
+functionalities are also included (based on packages such as *matplotlib*,
+*cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)). ## How to cite
+MapReader If you use MapReader in your work, please consider acknowledging us
+by citing [our SIGSPATIAL paper](https://dl.acm.org/doi/10.1145/
+3557919.3565812): - Kasra Hosseini, Daniel C. S. Wilson, Kaspar Beelen, and
+Katherine McDonough. 2022. MapReader: a computer vision pipeline for the
 semantic exploration of maps at scale. In Proceedings of the 6th ACM SIGSPATIAL
 International Workshop on Geospatial Humanities (GeoHumanities '22).
 Association for Computing Machinery, New York, NY, USA, 8â19. https://
 doi.org/10.1145/3557919.3565812 ## Acknowledgements This work was supported by
 Living with Machines (AHRC grant AH/S01179X/1) and The Alan Turing Institute
 (EPSRC grant EP/N510129/1). Living with Machines, funded by the UK Research and
 Innovation (UKRI) Strategic Priority Fund, is a multidisciplinary collaboration
```

### Comparing `mapreader-0.3.4/mapreader/annotate/load_annotate.py` & `mapreader-1.0.1.post0.dev9/mapreader/classify/load_annotations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,245 +1,236 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from glob import glob
-import matplotlib.pyplot as plt
 import os
+from decimal import Decimal
+from typing import Callable, Optional, Union
+
+import matplotlib.pyplot as plt
+import numpy as np
 import pandas as pd
-from skimage import io
+from PIL import Image
 from sklearn.model_selection import train_test_split
-from typing import Union, Optional
+from torch import Tensor
+from torch.utils.data import DataLoader, Sampler, WeightedRandomSampler
+from torchvision.transforms import Compose
 
+from .datasets import PatchDataset
 
-class loadAnnotations:
-    def __init__(self):
-        self.annotations = pd.DataFrame()
-        self.reviewed = pd.DataFrame()
-        self.col_path = None
 
-    def load_all(self, csv_paths: str, **kwds) -> None:
+class AnnotationsLoader:
+    def __init__(self):
         """
-        Load multiple CSV files into the class instance using the ``load``
-        method.
-
-        Parameters
-        ----------
-        csv_paths : str
-            The file path pattern to match CSV files to load.
-        **kwds : dict
-            Additional keyword arguments to pass to the ``load`` method.
-
-        Returns
-        -------
-        None
+        A Class for loading annnotations and preparing datasets and dataloaders for use in training/validation of a model.
         """
-        for csv_path in glob(csv_paths):
-            self.load(csv_path=csv_path, append=True, **kwds)
+        self.annotations = pd.DataFrame()
+        self.reviewed = pd.DataFrame()
+        self.id_col = None
+        self.patch_paths_col = None
+        self.label_col = None
+        self.datasets = None
 
     def load(
         self,
-        csv_path: str,
-        path2dir: Optional[str] = None,
-        col_path: Optional[str] = "image_id",
-        keep_these_cols: Optional[bool] = False,
+        annotations: Union[str, pd.DataFrame],
+        delimiter: Optional[str] = "\t",
+        id_col: Optional[str] = "image_id",
+        patch_paths_col: Optional[str] = "image_path",
+        label_col: Optional[str] = "label",
         append: Optional[bool] = True,
-        col_label: Optional[str] = "label",
-        shuffle_rows: Optional[bool] = True,
-        reset_index: Optional[bool] = True,
-        random_state: Optional[int] = 1234,
-    ) -> None:
-        """
-        Read and append an annotation file to the class instance's annotations
-        DataFrame.
+        scramble_frame: Optional[bool] = False,
+        reset_index: Optional[bool] = False,
+    ):
+        """Loads annotations from a csv file or dataframe and can be used to set the ``id_col``, ``patch_paths_col`` and ``label_col`` attributes.
 
         Parameters
         ----------
-        csv_path : str
-            Path to an annotation file in CSV format.
-        path2dir : str, optional
-            Update the ``col_path`` column by adding ``path2dir/col_path``, by
-            default ``None``.
-        col_path : str, optional
-            Name of the column that contains image paths, by default
-            ``"image_id"``.
-        keep_these_cols : bool, optional
-            Only keep these columns. If ``False`` (default), all columns will
-            be kept.
-        append : bool, optional
-            Append a newly read CSV file to the ``annotations`` property if
-            set to ``True``. By default, ``True``.
-        col_label : str, optional
-            Name of the column that contains labels. Default is ``"label"``.
-        shuffle_rows : bool, optional
-            Shuffle rows after reading annotations. Default is ``True``.
-        reset_index : bool, optional
-            Reset the index of the annotation DataFrame at the end of the
-            method. Default is ``True``.
-        random_state : int, optional
-            Random seed for row shuffling. Default is ``1234``.
+        annotations : Union[str, pd.DataFrame]
+            The annotations.
+            Can either be the path to a csv file or a pandas.DataFrame.
+        delimiter : Optional[str], optional
+            The delimiter to use when loading the csv file as a dataframe, by default "\t".
+        id_col : Optional[str], optional
+            The name of the column which contains the image IDs, by default "image_id".
+        patch_paths_col : Optional[str], optional
+            The name of the column containing the image paths, by default "image_path".
+        label_col : Optional[str], optional
+            The name of the column containing the image labels, by default "label".
+        append : Optional[bool], optional
+            Whether to append the annotations to a pre-existing ``annotations`` dataframe.
+            If False, existing dataframe will be overwritten.
+            By default True.
+        scramble_frame : Optional[bool], optional
+            Whether to shuffle the rows of the dataframe, by default False.
+        reset_index : Optional[bool], optional
+            Whether to reset the index of the dataframe (e.g. after shuffling), by default False.
 
-        Returns
-        -------
-        None
+        Raises
+        ------
+        ValueError
+            If ``annotations`` is passed as something other than a string or pd.DataFrame.
         """
-        if isinstance(csv_path, str):
-            print(f"* reading: {csv_path}")
-            annots_rd = pd.read_csv(csv_path)
-        else:
-            print("* reading dataframe")
-            annots_rd = csv_path.copy()
-        self.col_label = col_label
-        print(f"* #rows: {len(annots_rd)}")
-        print(
-            f"* label column name: {self.col_label} (you can change this later by .set_col_label(new_label) )"  # noqa
-        )
-        if shuffle_rows:
-            annots_rd = annots_rd.sample(frac=1, random_state=random_state)
-            print("* shuffle rows: Yes")
-
-        if keep_these_cols:
-            annots_rd = annots_rd[keep_these_cols]
-
-        if self.col_path is None:
-            self.col_path = col_path
-        elif self.col_path != col_path:
+
+        if not self.id_col:
+            self.id_col = id_col
+        elif self.id_col != id_col:
             print(
-                f"[WARNING] previously, the col_path was set to {self.col_path}. Column '{col_path}' will be renamed."  # noqa
+                f'[WARNING] ID column was previously "{self.id_col}, but will now be set to {id_col}.'
             )
-            annots_rd.rename(columns={col_path: self.col_path}, inplace=True)
 
-        if path2dir:
+        if not self.patch_paths_col:
+            self.patch_paths_col = patch_paths_col
+        elif self.patch_paths_col != patch_paths_col:
             print(
-                f"* update paths in '{self.col_path}' column by inserting '{path2dir}'"  # noqa
+                f'[WARNING] Patch paths column was previously "{self.patch_paths_col}, but will now be set to {patch_paths_col}.'
             )
-            annots_rd[self.col_path] = (
-                os.path.abspath(path2dir)
-                + os.path.sep
-                + annots_rd[self.col_path]
+
+        if not self.label_col:
+            self.label_col = label_col
+        elif self.label_col != label_col:
+            print(
+                f'[WARNING] Label column was previously "{self.label_col}, but will now be set to {label_col}.'
             )
 
-        if (len(self.annotations) == 0) or (append is False):
-            self.annotations = annots_rd.copy()
-        else:
-            self.annotations = pd.concat(
-                [self.annotations, annots_rd.copy()], ignore_index=True
+        if not isinstance(annotations, (str, pd.DataFrame)):
+            raise ValueError(
+                "[ERROR] Please pass ``annotations`` as a string (path to csv file) or pd.DataFrame."
+            )
+        if isinstance(annotations, str):
+            annotations = self._load_annotations_csv(
+                annotations, delimiter, scramble_frame, reset_index
             )
 
-        self.annotations.drop_duplicates(subset=[self.col_path], inplace=True)
-        if reset_index:
-            self.annotations.reset_index(drop=True, inplace=True)
-        print()
+        annotations = annotations.astype(
+            {self.label_col: str}
+        )  # ensure labels are interpreted as strings
+
+        if append:
+            self.annotations = pd.concat([self.annotations, annotations])
+        else:
+            self.annotations = annotations
+
+        unique_labels = self.annotations[self.label_col].unique().tolist()
+        self.unique_labels = unique_labels
+        self.annotations["label_index"] = self.annotations[self.label_col].apply(
+            self._get_label_index
+        )
+
+        labels_map = {i: label for i, label in enumerate(unique_labels)}
+        self.labels_map = labels_map
+
         print(self)
 
-    def set_col_label(self, new_label: str = "label") -> None:
-        """
-        Set a new label for the column that contains the labels.
+    def _load_annotations_csv(
+        self,
+        annotations: str,
+        delimiter: Optional[str] = "\t",
+        scramble_frame: Optional[bool] = False,
+        reset_index: Optional[bool] = False,
+    ) -> pd.DataFrame:
+        """Loads annotations from a csv file.
 
         Parameters
         ----------
-        new_label : str, optional
-            Name of the new label column, by default ``"label"``.
+        annotations : str
+            The path to the annotations csv file.
+        delimiter : Optional[str], optional
+            The delimiter to use when loading the csv file as a dataframe, by default "\t".
+        scramble_frame : Optional[bool], optional
+            Whether to shuffle the rows of the dataframe, by default False.
+        reset_index : Optional[bool], optional
+            Whether to reset the index of the dataframe (e.g. after shuffling), by default False.
 
         Returns
         -------
-        None
+        pd.DataFrame
+            Dataframe containing the annotations.
+
+        Raises
+        ------
+        ValueError
+            If ``annotations`` is passed as something other than a string or pd.DataFrame.
         """
-        self.col_label = new_label
 
-    def show_image(self, indx: int, cmap: Optional[str] = "viridis") -> None:
+        if os.path.isfile(annotations):
+            print(f'[INFO] Reading "{annotations}"')
+            annotations = pd.read_csv(annotations, sep=delimiter, index_col=0)
+        else:
+            raise ValueError(f'[ERROR] "{annotations}" cannot be found.')
+
+        if scramble_frame:
+            annotations = annotations.sample(frac=1)
+        if reset_index:
+            annotations.reset_index(drop=True, inplace=True)
+
+        annotations.drop_duplicates(subset=self.id_col, inplace=True, keep="first")
+        return annotations
+
+    def show_patch(self, patch_id: str) -> None:
         """
-        Display an image specified by its index along with its label.
+        Display a patch and its label.
 
         Parameters
         ----------
-        indx : int
-            Index of the image in the annotations DataFrame to display.
-        cmap : str, optional
-            The colormap to use, by default ``"viridis"``.
-
-            To see available colormaps, see
-            https://matplotlib.org/stable/gallery/color/colormap_reference.html.
+        patch_id : str
+            The image ID of the patch to show.
 
         Returns
         -------
         None
         """
-        if (self.col_path is None) or (len(self.annotations) == 0):
-            print(f"[ERROR] length: {len(self.annotations)}")
-            return
 
-        plt.imshow(
-            io.imread(self.annotations.iloc[indx][self.col_path]), cmap=cmap
-        )
-        plt.title(self.annotations.iloc[indx][self.col_label])
-        plt.xticks([])
-        plt.yticks([])
-        plt.pause(0.001)
+        if len(self.annotations) == 0:
+            raise ValueError("[ERROR] No annotations loaded.")
+
+        patch_row = self.annotations[self.annotations[self.id_col] == patch_id]
+        patch_path = patch_row[self.patch_paths_col].values[0]
+        patch_label = patch_row[self.label_col].values[0]
+        img = Image.open(patch_path)
+
+        plt.imshow(img)
+        plt.axis("off")
+        plt.title(patch_label)
         plt.show()
 
-    def adjust_labels(self, shiftby: int = -1) -> None:
-        """
-        Shift labels in the self.annotations DataFrame by the specified value
-        (``shiftby``).
+    def print_unique_labels(self) -> None:
+        """Prints unique labels
 
-        Parameters
-        ----------
-        shiftby : int, optional
-            The value to shift labels by. Default is ``-1``.
-
-        Returns
-        -------
-        None
+        Raises
+        ------
+        ValueError
+            If no annotations are found.
+        """
+        if len(self.annotations) == 0:
+            raise ValueError("[ERROR] No annotations loaded.")
 
-        Notes
-        -----
-        This function updates the ``self.annotations`` DataFrame by adding the
-        value of ``shiftby`` to the values of the ``self.col_label`` column. It
-        also prints the value counts of the ``self.col_label`` column before
-        and after the shift.
-        """
-        print(20 * "-")
-        print("[INFO] value counts before shift:")
-        print(self.annotations[self.col_label].value_counts())
-
-        self.annotations[self.col_label] += shiftby
-
-        print(20 * "-")
-        print("[INFO] value counts after shift:")
-        print(self.annotations[self.col_label].value_counts())
-        print(20 * "-")
+        print(f"[INFO] Unique labels: {self.unique_labels}")
 
     def review_labels(
         self,
-        tar_label: Optional[int] = None,
-        start_indx: Optional[int] = 1,
-        chunks: Optional[int] = 8 * 6,
+        label_to_review: Optional[str] = None,
+        chunks: Optional[int] = 8 * 3,
         num_cols: Optional[int] = 8,
-        figsize: Union[list, tuple] = (8 * 3, 8 * 2),
         exclude_df: Optional[pd.DataFrame] = None,
         include_df: Optional[pd.DataFrame] = None,
         deduplicate_col: Optional[str] = "image_id",
     ) -> None:
         """
         Perform image review on annotations and update labels for a given
         label or all labels.
 
         Parameters
         ----------
-        tar_label : int, optional
+        label_to_review : str, optional
             The target label to review. If not provided, all labels will be
             reviewed, by default ``None``.
-        start_indx : int, optional
-            The index of the first image to review, by default ``1``.
         chunks : int, optional
-            The number of images to display at a time, by default ``8 * 6``.
+            The number of images to display at a time, by default ``24``.
         num_cols : int, optional
             The number of columns in the display, by default ``8``.
-        figsize : list or tuple, optional
-            The size of the display window, by default ``(8 * 3, 8 * 2)``.
         exclude_df : pandas.DataFrame, optional
             A DataFrame of images to exclude from review, by default ``None``.
         include_df : pandas.DataFrame, optional
             A DataFrame of images to include for review, by default ``None``.
         deduplicate_col : str, optional
             The column to use for deduplicating reviewed images, by default
             ``"image_id"``.
@@ -247,301 +238,429 @@
         Returns
         -------
         None
 
         Notes
         ------
         This method reviews images with their corresponding labels and allows
-        the user to change the label for each image. The updated labels are
-        saved in both the annotations and reviewed DataFrames. If
-        ``exclude_df`` is provided, images with ``image_path`` in
-        ``exclude_df["image_path"]`` are skipped in the review process. If
-        ``include_df`` is provided, only images with ``image_path`` in
-        ``include_df["image_path"]`` are reviewed. The reviewed DataFrame is
-        deduplicated based on the ``deduplicate_col``.
-        """
-        if tar_label is not None:
-            annot2review = self.annotations[
-                self.annotations[self.col_label] == tar_label
+        the user to change the label for each image.
+
+        Updated labels are saved in ``self.annotations`` and in a newly created ``self.reviewed`` DataFrame.
+        If ``exclude_df`` is provided, images found in this df are skipped in the review process.
+        If ``include_df`` is provided, only images found in this df are reviewed.
+        The ``self.reviewed`` DataFrame is deduplicated based on the ``deduplicate_col``.
+        """
+        if len(self.annotations) == 0:
+            raise ValueError("[ERROR] No annotations loaded.")
+
+        if label_to_review:
+            annots2review = self.annotations[
+                self.annotations[self.label_col] == label_to_review
             ]
+            annots2review.reset_index(inplace=True, drop=True)
         else:
-            annot2review = self.annotations
-
-        annot2review.drop_duplicates(inplace=True)
+            annots2review = self.annotations
+            annots2review.reset_index(inplace=True, drop=True)
 
-        indx = start_indx - 1
-        while indx < len(annot2review):
-            plt.figure(figsize=figsize)
-            print("\n" + 30 * "*")
+        if exclude_df is not None:
+            if isinstance(exclude_df, pd.DataFrame):
+                merged_df = pd.merge(
+                    annots2review, exclude_df, how="left", indicator=True
+                )
+                annots2review = merged_df[merged_df["_merge"] == "left_only"].drop(
+                    columns="_merge"
+                )
+                annots2review.reset_index(inplace=True, drop=True)
+            else:
+                raise ValueError("[ERROR] ``exclude_df`` must be a pandas dataframe.")
+
+        if include_df is not None:
+            if isinstance(include_df, pd.DataFrame):
+                annots2review = pd.merge(annots2review, include_df, how="right")
+                annots2review.reset_index(inplace=True, drop=True)
+            else:
+                raise ValueError("[ERROR] ``include_df`` must be a pandas dataframe.")
+
+        image_idx = 0
+        while image_idx < len(annots2review):
+            print('[INFO] Type "exit", "end" or "stop" to exit.')
             print(
-                f"[INFO] review {indx+1}-{indx+chunks}, total: {len(annot2review)}"  # noqa
+                f"[INFO] Showing {image_idx}-{image_idx+chunks} out of {len(annots2review)}."  # noqa
             )
-            print(30 * "*")
-
+            plt.figure(figsize=(num_cols * 3, (chunks // num_cols) * 3))
             counter = 1
             iter_ids = []
-            while (counter <= chunks) and (indx < len(annot2review)):
-                # Skip the image if it is in exclude_df
-                if exclude_df is not None:
-                    if (
-                        annot2review.iloc[indx]["image_path"]
-                        in exclude_df["image_path"].to_list()
-                    ):
-                        indx += 1
-                        continue
-
-                # Skip the image if it is NOT in include_df
-                if include_df is not None:
-                    if (
-                        annot2review.iloc[indx]["image_path"]
-                        not in exclude_df["image_path"].to_list()
-                    ):
-                        indx += 1
-                        continue
-
+            while (counter <= chunks) and (image_idx < len(annots2review)):
                 # The first term is just a ceiling division, equivalent to:
                 # from math import ceil
                 # int(ceil(chunks / num_cols))
-                plt.subplot(-(-chunks // num_cols), num_cols, counter)
-                plt.imshow(io.imread(annot2review.iloc[indx][self.col_path]))
+                plt.subplot((chunks // num_cols), num_cols, counter)
+                patch_path = annots2review.iloc[image_idx][self.patch_paths_col]
+                img = Image.open(patch_path)
+                plt.imshow(img)
                 plt.xticks([])
                 plt.yticks([])
                 plt.title(
-                    f"{annot2review.iloc[indx][self.col_label]} | id: {annot2review.iloc[indx].name}"  # noqa
+                    f"{annots2review.iloc[image_idx][self.label_col]} | id: {annots2review.iloc[image_idx].name}"  # noqa
                 )
-                iter_ids.append(annot2review.iloc[indx].name)
+                iter_ids.append(annots2review.iloc[image_idx].name)
                 # Add to reviewed
-                self.reviewed = self.reviewed.append(annot2review.iloc[indx])
+                self.reviewed = self.reviewed.append(annots2review.iloc[image_idx])
                 try:
                     self.reviewed.drop_duplicates(subset=[deduplicate_col])
                 except Exception:
                     pass
                 counter += 1
-                indx += 1
+                image_idx += 1
             plt.show()
 
-            print(f"list of IDs: {iter_ids}")
-            q = "Enter IDs, comma separated (or press enter to continue): "
+            print(f"[INFO] IDs of current patches: {iter_ids}")
+            q = "\nEnter IDs, comma separated (or press enter to continue): "
             user_input_ids = input(q)
 
             while user_input_ids.strip().lower() not in [
                 "",
                 "exit",
                 "end",
                 "stop",
             ]:
                 list_input_ids = user_input_ids.split(",")
-                input_label = int(input("Enter label  :  "))
+                print(
+                    f"[INFO] Options for labels (or create a new label):{list(self.annotations[self.label_col].unique())}"
+                )
+                input_label = input("Enter new label:  ")
 
-                for one_input_id in list_input_ids:
-                    input_id = int(one_input_id)
+                for input_id in list_input_ids:
+                    input_id = int(input_id)
                     # Change both annotations and reviewed
+                    self.annotations.loc[input_id, self.label_col] = input_label
+                    self.reviewed.loc[input_id, self.label_col] = input_label
+                    # Update label indices
                     self.annotations.loc[
-                        input_id, self.col_label
-                    ] = input_label
-                    self.reviewed.loc[input_id, self.col_label] = input_label
-                    print(f"{input_id} ---> new label: {input_label}")
+                        input_id, "label_index"
+                    ] = self._get_label_index(input_label)
+                    self.reviewed.loc[input_id, "label_index"] = self._get_label_index(
+                        input_label
+                    )
+                    assert (
+                        self.annotations[self.label_col].value_counts().tolist()
+                        == self.annotations["label_index"].value_counts().tolist()
+                    )
+                    print(
+                        f'[INFO] Image {input_id} has been relabelled as "{input_label}"'
+                    )
 
                 user_input_ids = input(q)
 
             if user_input_ids.lower() in ["exit", "end", "stop"]:
                 break
 
-        print("[INFO] Exit...")
+        print("[INFO] Exited.")
 
-    def show_image_labels(
-        self, tar_label: Optional[int] = 1, num_sample: Optional[int] = 10
-    ) -> None:
+    def show_sample(self, label_to_show: str, num_samples: Optional[int] = 9) -> None:
         """Show a random sample of images with the specified label (tar_label).
 
         Parameters
         ----------
-        tar_label : int, optional
-            The label to filter the images by. Default is ``1``.
+        label_to_show : str, optional
+            The label of the images to show.
         num_sample : int, optional
-            The number of images to show. If ``None``, all images with the
-            specified label will be shown. Default is ``10``.
+            The number of images to show.
+            If ``None``, all images with the specified label will be shown. Default is ``9``.
 
         Returns
         -------
         None
         """
-        if (self.col_path is None) or (len(self.annotations) == 0):
-            print(f"[ERROR] length: {len(self.annotations)}")
-            return
-
-        annot2plot = self.annotations[
-            self.annotations[self.col_label] == tar_label
-        ]
-
-        if num_sample is None:
-            num_sample = len(annot2plot)
-
-        plt.figure(figsize=(8, num_sample))
-        for indx in range(num_sample):
-            plt.subplot(int(num_sample / 2.0), 3, indx + 1)
-            plt.imshow(io.imread(annot2plot.iloc[indx][self.col_path]))
-            plt.xticks([])
-            plt.yticks([])
-            plt.title(annot2plot.iloc[indx][self.col_label])
+        if len(self.annotations) == 0:
+            raise ValueError("[ERROR] No annotations loaded.")
+
+        annot2plot = self.annotations[self.annotations[self.label_col] == label_to_show]
+        annot2plot = annot2plot.sample(frac=1)
+        annot2plot.reset_index(drop=True, inplace=True)
+
+        num_samples = min(len(annot2plot), num_samples)
+
+        plt.figure(figsize=(8, num_samples))
+        for i in range(num_samples):
+            plt.subplot(int(num_samples / 2.0), 3, i + 1)
+            patch_path = annot2plot.iloc[i][self.patch_paths_col]
+            img = Image.open(patch_path)
+            plt.imshow(img)
+            plt.axis("off")
+            plt.title(annot2plot.iloc[i][self.label_col])
         plt.show()
 
-    def split_annotations(
+    def create_datasets(
         self,
-        stratify_colname: Optional[str] = "label",
         frac_train: Optional[float] = 0.70,
         frac_val: Optional[float] = 0.15,
         frac_test: Optional[float] = 0.15,
         random_state: Optional[int] = 1364,
+        train_transform: Optional[Union[str, Compose, Callable]] = "train",
+        val_transform: Optional[Union[str, Compose, Callable]] = "val",
+        test_transform: Optional[Union[str, Compose, Callable]] = "test",
     ) -> None:
         """
-        Splits the dataset into three subsets: training, validation, and test
-        sets (DataFrames).
+        Splits the dataset into three subsets: training, validation, and test sets (DataFrames) and saves them as a dictionary in ``self.datasets``.
 
         Parameters
         ----------
-        stratify_colname : str, optional
-            Name of the column on which to stratify the split. The default is
-            ``"label"``.
         frac_train : float, optional
-            Fraction of the dataset to be used for training. The default is
-            ``0.70``.
+            Fraction of the dataset to be used for training.
+            By default ``0.70``.
         frac_val : float, optional
-            Fraction of the dataset to be used for validation. The default is
-            ``0.15``.
+            Fraction of the dataset to be used for validation.
+            By default ``0.15``.
         frac_test : float, optional
-            Fraction of the dataset to be used for testing. The default is
-            ``0.15``.
+            Fraction of the dataset to be used for testing.
+            By default ``0.15``.
         random_state : int, optional
             Random seed to ensure reproducibility. The default is ``1364``.
+        train_transform: str, tochvision.transforms.Compose or Callable, optional
+            The transform to use on the training dataset images.
+            Options are "train", "test" or "val" or, a callable object (e.g. a torchvision transform or torchvision.transforms.Compose).
+            By default "train".
+        val_transform: str, tochvision.transforms.Compose or Callable, optional
+            The transform to use on the validation dataset images.
+            Options are "train", "test" or "val" or, a callable object (e.g. a torchvision transform or torchvision.transforms.Compose).
+            By default "val".
+        test_transform: str, tochvision.transforms.Compose or Callable, optional
+            The transform to use on the test dataset images.
+            Options are "train", "test" or "val" or, a callable object (e.g. a torchvision transform or torchvision.transforms.Compose).
+            By default "test".
+
 
         Raises
         ------
         ValueError
             If the sum of fractions of training, validation and test sets does
             not add up to 1.
 
-        ValueError
-            If ``stratify_colname`` is not a column in the dataframe.
-
         Returns
         -------
         None
-            Sets properties ``df_train``, ``df_val``, ``df_test`` -- three
-            Dataframes containing the three splits on the ``loadAnnotations``
-            instance.
 
         Notes
         -----
+        This method saves the split datasets as a dictionary in ``self.datasets``.
+
         Following fractional ratios provided by the user, where each subset is
         stratified by the values in a specific column (that is, each subset has
         the same relative frequency of the values in the column). It performs
         this splitting by running ``train_test_split()`` twice.
+
+        See ``PatchDataset`` for more information on transforms.
         """
+        if len(self.annotations) == 0:
+            raise ValueError("[ERROR] No annotations loaded.")
 
-        if abs(frac_train + frac_val + frac_test - 1.0) > 1e-4:
-            raise ValueError(
-                f"fractions {frac_train}, {frac_val}, {frac_test} do not add up to 1.0."  # noqa
-                f"Their sum: {frac_train+frac_val+frac_test}"
-            )
+        frac_train = Decimal(str(frac_train))
+        frac_val = Decimal(str(frac_val))
+        frac_test = Decimal(str(frac_test))
 
-        if stratify_colname not in self.annotations.columns:
+        if sum([frac_train + frac_val + frac_test]) != 1:
             raise ValueError(
-                f"{stratify_colname} is not a column in the dataframe"
-            )
+                f"[ERROR] ``frac_train`` ({frac_train}), ``frac_val`` ({frac_val}) and ``frac_test`` ({frac_test}) do not add up to 1."
+            )  # noqa
+
+        labels = self.annotations[self.label_col]
 
-        X = self.annotations  # Contains all columns.
-        y = X[
-            [stratify_colname]
-        ]  # Dataframe of just the column on which to stratify.
-
-        # Split original dataframe into train and temp dataframes.
-        df_train, df_temp, y_train, y_temp = train_test_split(
-            X,
-            y,
-            stratify=y,
-            test_size=(1.0 - frac_train),
+        # Split original dataframe into train and temp (val+test) dataframes.
+        df_train, df_temp, _, labels_temp = train_test_split(
+            self.annotations,
+            labels,
+            stratify=labels,
+            test_size=float(1 - frac_train),
             random_state=random_state,
         )
 
-        if abs(frac_test) < 1e-3:
-            df_val = df_temp
-            df_test = None
-            assert len(self.annotations) == len(df_train) + len(df_val)
-        else:
+        if frac_test != 0:
             # Split the temp dataframe into val and test dataframes.
-            relative_frac_test = frac_test / (frac_val + frac_test)
-            df_val, df_test, y_val, y_test = train_test_split(
+            relative_frac_test = Decimal(frac_test / (frac_val + frac_test))
+            relative_frac_test = relative_frac_test.quantize(Decimal("0.001"))
+            df_val, df_test, _, _ = train_test_split(
                 df_temp,
-                y_temp,
-                stratify=y_temp,
-                test_size=relative_frac_test,
+                labels_temp,
+                stratify=labels_temp,
+                test_size=float(relative_frac_test),
                 random_state=random_state,
             )
-            assert len(self.annotations) == len(df_train) + len(df_val) + len(
-                df_test
+            assert len(self.annotations) == len(df_train) + len(df_val) + len(df_test)
+
+        else:
+            df_val = labels_temp
+            df_test = None
+            assert len(self.annotations) == len(df_train) + len(df_val)
+
+        train_dataset = PatchDataset(
+            df_train,
+            train_transform,
+            patch_paths_col=self.patch_paths_col,
+            label_col=self.label_col,
+            label_index_col="label_index",
+        )
+        val_dataset = PatchDataset(
+            df_val,
+            val_transform,
+            patch_paths_col=self.patch_paths_col,
+            label_col=self.label_col,
+            label_index_col="label_index",
+        )
+        if df_test is not None:
+            test_dataset = PatchDataset(
+                df_test,
+                test_transform,
+                patch_paths_col=self.patch_paths_col,
+                label_col=self.label_col,
+                label_index_col="label_index",
             )
 
-        self.train = df_train
-        self.val = df_val
-        self.test = df_test
-        print("---------------------")
-        print("* Split dataset into:")
-        print(f"    Train: {len(self.train)}")
-        print(f"    Valid: {len(self.val)}")
-        print(f"    Test : {len(self.test) if self.test is not None else 0}")
-        print("---------------------")
+        datasets = {"train": train_dataset, "val": val_dataset, "test": test_dataset}
+        dataset_sizes = {
+            set_name: len(datasets[set_name]) for set_name in datasets.keys()
+        }
+
+        self.datasets = datasets
+        self.dataset_sizes = dataset_sizes
 
-    def sample_labels(
+        print(
+            f'[INFO] Number of annotations in each set:\n\
+        - Train:        {dataset_sizes["train"]}\n\
+        - Validate:     {dataset_sizes["val"]}\n\
+        - Test:         {dataset_sizes["test"]}'
+        )
+
+    def create_dataloaders(
         self,
-        tar_label: Union[int, str],
-        num_samples: int,
-        random_state: Optional[int] = 12345,
+        batch_size: Optional[int] = 16,
+        sampler: Optional[Union[Sampler, str, None]] = "default",
+        shuffle: Optional[bool] = False,
+        num_workers: Optional[int] = 0,
+        **kwargs,
     ) -> None:
-        """
-        Randomly sample a given number of annotations with a given target
-        label and remove all other annotations from the dataframe.
+        """Creates a dictionary containing PyTorch dataloaders
+        saves it to as ``self.dataloaders`` and returns it.
 
         Parameters
         ----------
-        tar_label : int or str
-            The target label for which the annotations will be sampled.
-        num_samples : int
-            The number of annotations to be sampled.
-        random_state : int, optional
-            Seed to ensure reproducibility of the random number generator.
-            Default is ``12345``.
+        batch_size : int, optional
+            The batch size to use for the dataloader. By default ``16``.
+        sampler : Sampler, str or None, optional
+            The sampler to use when creating batches from the training dataset.
+        shuffle : bool, optional
+            Whether to shuffle the dataset during training. By default ``False``.
+        num_workers : int, optional
+            The number of worker threads to use for loading data. By default ``0``.
+        **kwds :
+            Additional keyword arguments to pass to PyTorch's ``DataLoader`` constructor.
+
+        Returns
+        --------
+        Dict
+            Dictionary containing dataloaders.
+
+        Notes
+        -----
+        ``sampler`` will only be applied to the training dataset (datasets["train"]).
+        """
+        if not self.datasets:
+            print(
+                "[INFO] Creating datasets using default train/val/test split of 0.7:0.15:0.15 and default transformations."
+            )
+            self.create_datasets()
+
+        datasets = self.datasets
+
+        if isinstance(sampler, str):
+            if sampler == "default":
+                print("[INFO] Using default sampler.")
+                sampler = self._define_sampler()
+            else:
+                raise ValueError(
+                    '[ERROR] ``sampler`` can only be a PyTorch sampler, ``"default"`` or ``None``.'
+                )
+
+        if sampler and shuffle:
+            print("[INFO] ``sampler`` is defined so train dataset will be unshuffled.")
+
+        dataloaders = {
+            set_name: DataLoader(
+                datasets[set_name],
+                batch_size=batch_size,
+                sampler=sampler if set_name == "train" else None,
+                shuffle=False if set_name == "train" else shuffle,
+                num_workers=num_workers,
+                **kwargs,
+            )
+            for set_name in datasets.keys()
+        }
+
+        self.dataloaders = dataloaders
+
+        return dataloaders
+
+    def _define_sampler(self):
+        """Defines a weighted random sampler for the training dataset.
+        Weighting are proportional to the reciprocal of number of instances of each label.
+
+        Returns
+        -------
+        torch.utils.data.WeightedRandomSampler
+            The sampler
 
         Raises
         ------
         ValueError
-            If ``tar_label`` is not a column in the dataframe.
+            If "train" cannot be found in ``self.datasets.keys()``.
+        """
+        if not self.datasets:
+            self.create_datasets()
+
+        datasets = self.datasets
+
+        if "train" in datasets.keys():
+            value_counts = (
+                datasets["train"].patch_df[self.label_col].value_counts().to_list()
+            )
+            weights = np.reciprocal(Tensor(value_counts))
+            weights = weights.double()
+            sampler = WeightedRandomSampler(
+                weights[datasets["train"].patch_df["label_index"].tolist()],
+                num_samples=len(datasets["train"].patch_df),
+            )
+
+        else:
+            raise ValueError('[ERROR] "train" should be one the dataset names.')
+
+        return sampler
+
+    def _get_label_index(self, label: str) -> int:
+        """Gets the index of a label.
+
+        Parameters
+        ----------
+        label : str
+            A label from the ``label_col`` of the ``patch_df``.
 
         Returns
         -------
-        None
-            The dataframe with remaining annotations is stored in
-            ``self.annotations``.
+        int
+            The index of the label.
+
+        Notes
+        -----
+        Used to generate the ``label_index`` column.
+
         """
-        if (self.col_path is None) or (len(self.annotations) == 0):
-            print(f"[ERROR] length: {len(self.annotations)}")
-            return
-        all_annots = self.annotations.copy()
-        tar_rows = all_annots[all_annots[self.col_label] == tar_label]
-        tar_samples = tar_rows.sample(num_samples, random_state=random_state)
-        new_annots = all_annots[
-            (all_annots[self.col_label] != tar_label)
-            | (all_annots.index.isin(tar_samples.index))
-        ]
-        self.annotations = new_annots
+        return self.unique_labels.index(label)
 
     def __str__(self):
-        print("------------------------")
-        print(f"* Number of annotations: {len(self.annotations)}\n")
+        print(f"[INFO] Number of annotations:   {len(self.annotations)}\n")
         if len(self.annotations) > 0:
-            print("* First few rows:")
-            print(self.annotations.head())
-            print("...\n")
-            print(f"* Value counts (column: {self.col_label}):")
-            print(self.annotations[self.col_label].value_counts())
-        print("------------------------")
+            value_counts = self.annotations[self.label_col].value_counts()
+            print(
+                f'[INFO] Number of instances of each label (from column "{self.label_col}"):'
+            )
+            for label, count in value_counts.items():
+                print(f"        - {label}:      {count}")
         return ""
```

### Comparing `mapreader-0.3.4/mapreader/annotate/utils.py` & `mapreader-1.0.1.post0.dev9/mapreader/annotate/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,24 +55,24 @@
     Refer to ``ipyannotate`` and ``matplotlib`` for more info.
     """
 
     # setup the images
     gridsize = (5, 1)
     plt.clf()
     plt.figure(figsize=(12, 12))
-    if treelevel == "child" and contextimage:
+    if treelevel == "patch" and contextimage:
         plt.subplot2grid(gridsize, (2, 0))
     else:
         plt.subplot2grid(gridsize, (0, 0), rowspan=2)
     plt.imshow(Image.open(record[1]))
     plt.xticks([])
     plt.yticks([])
     plt.title(f"{record[0]}", size=20)
 
-    if treelevel == "child" and contextimage:
+    if treelevel == "patch" and contextimage:
         parent_path = os.path.dirname(
             annotation_tasks["paths"][record[3]]["parent_paths"]
         )
         # Here, we assume that min_x, min_y, max_x and max_y are in the patch
         # name
         split_path = record[0].split("-")
         min_x, min_y, max_x, max_y = (
@@ -92,17 +92,15 @@
         min_x_par = max(0, min_x - x_offset)
         max_x_par = min(max_x + x_offset, np.shape(par_img)[1])
         max_y_par = min(max_y + y_offset, np.shape(par_img)[0])
 
         # par_img = par_img[min_y_par:max_y_par, min_x_par:max_x_par]
         par_img = par_img.crop((min_x_par, min_y_par, max_x_par, max_y_par))
 
-        plt.imshow(
-            par_img, extent=(min_x_par, max_x_par, max_y_par, min_y_par)
-        )
+        plt.imshow(par_img, extent=(min_x_par, max_x_par, max_y_par, min_y_par))
         # ---
 
         plt.xticks([])
         plt.yticks([])
 
         # plot the patch border on the context image
         plt.plot([min_x, min_x], [min_y, max_y], lw=2, zorder=10, color="r")
@@ -221,33 +219,29 @@
         df = df[df[label_col_name].isnull()]
         print(f"Number of images to be annotated (total): {len(df)}")
     else:
         # if redo = True or "label" column does not exist
         # annotate all patches in the pandas dataframe
         pass
 
-    tar_param = "mean_pixel_RGB"
+    tar_param = "mean_pixel_R"
     if tar_param in df.columns:
         try:
             pd.options.mode.chained_assignment = None
             df["pixel_groups"] = pd.qcut(
                 df[tar_param], q=10, precision=2, labels=False
             ).values
             if random_state in ["random"]:
                 df = df.groupby("pixel_groups").sample(
                     n=10, random_state=random.randint(0, 1e6)
                 )
             else:
-                df = df.groupby("pixel_groups").sample(
-                    n=10, random_state=random_state
-                )
+                df = df.groupby("pixel_groups").sample(n=10, random_state=random_state)
         except Exception:
-            print(
-                f"[INFO] len(df) = {len(df)}, .sample method is deactivated."
-            )
+            print(f"[INFO] len(df) = {len(df)}, .sample method is deactivated.")
             df = df.iloc[:num_samples]
     else:
         print(f"[WARNING] could not find {tar_param} in columns.")
         df = df.iloc[:num_samples]
 
     data = []
     row_counter = 0
@@ -378,15 +372,15 @@
     task: str,
     annotation_tasks_file: str,
     custom_labels: List[str] = [],
     annotation_set: Optional[str] = "001",
     redo_annotation: Optional[bool] = False,
     patch_paths: Optional[Union[str, bool]] = False,
     parent_paths: Optional[str] = False,
-    tree_level: Optional[str] = "child",
+    tree_level: Optional[str] = "patch",
     sortby: Optional[str] = None,
     min_alpha_channel: Optional[float] = None,
     min_mean_pixel: Optional[float] = None,
     max_mean_pixel: Optional[float] = None,
     min_std_pixel: Optional[float] = None,
     max_std_pixel: Optional[float] = None,
     context_image: Optional[bool] = False,
@@ -416,49 +410,47 @@
     annotation_set : str, optional
         The ID of the annotation set to use in the YAML file
         (``annotation_tasks_file``). Default is ``"001"``.
     redo_annotation : bool, optional
         If ``True``, allows the user to redo annotations on previously
         annotated images. Default is ``False``.
     patch_paths : str or bool, optional
-        The path to the directory containing image patches for child level
-        annotations, if ``custom_labels`` are provided. Default is ``False``
-        and the information is read from the yaml file.
+        The path to the directory containing patches, if ``custom_labels`` are provided. Default is ``False`` and the information is read from the yaml file.
     parent_paths : str, optional
         The path to parent images, if ``custom_labels`` are provided. Default
         is ``False`` and the information is read from the yaml file.
     tree_level : str, optional
-        The level of annotation to be used, either ``"child"`` or ``"parent"``.
-        Default is ``"child"``.
+        The level of annotation to be used, either ``"patch"`` or ``"parent"``.
+        Default is ``"patch"``.
     sortby : str, optional
         If ``"mean"``, sort images by mean pixel intensity. Default is
         ``None``.
     min_alpha_channel : float, optional
         The minimum alpha channel value for images to be included in the
-        annotation interface. Only applies to child level annotations.
+        annotation interface. Only applies to patch level annotations.
         Default is ``None``.
     min_mean_pixel : float, optional
         The minimum mean pixel intensity value for images to be included in
-        the annotation interface. Only applies to child level annotations.
+        the annotation interface. Only applies to patch level annotations.
         Default is ``None``.
     max_mean_pixel : float, optional
         The maximum mean pixel intensity value for images to be included in
-        the annotation interface. Only applies to child level annotations.
+        the annotation interface. Only applies to patch level annotations.
         Default is ``None``.
     min_std_pixel : float, optional
         The minimum standard deviation of pixel intensity value for images to be included in
-        the annotation interface. Only applies to child level annotations.
+        the annotation interface. Only applies to patch level annotations.
         Default is ``None``.
     max_std_pixel : float, optional
         The maximum standard deviation of pixel intensity value for images to be included in
-        the annotation interface. Only applies to child level annotations.
+        the annotation interface. Only applies to patch level annotations.
         Default is ``None``.
     context_image : bool, optional
         If ``True``, includes a context image with each patch image in the
-        annotation interface. Only applies to child level annotations. Default
+        annotation interface. Only applies to patch level annotations. Default
         is ``False``.
     xoffset : int, optional
         The x-offset in pixels to be used for displaying context images in the
         annotation interface. Default is ``500``.
     yoffset : int, optional
         The y-offset in pixels to be used for displaying context images in the
         annotation interface. Default is ``500``.
@@ -506,18 +498,16 @@
         annotation_tasks = yaml.load(annot_file_fio, Loader=yaml.FullLoader)
 
     if annotation_set not in annotation_tasks["paths"].keys():
         raise ValueError(
             f"{annotation_set} could not be found in {annotation_tasks_file}"
         )
     else:
-        if tree_level == "child":
-            patch_paths = annotation_tasks["paths"][annotation_set][
-                "patch_paths"
-            ]
+        if tree_level == "patch":
+            patch_paths = annotation_tasks["paths"][annotation_set]["patch_paths"]
         parent_paths = os.path.join(
             annotation_tasks["paths"][annotation_set]["parent_paths"]
         )
         annot_file = os.path.join(
             annotation_tasks["paths"][annotation_set]["annot_dir"],
             f"{task}_#{userID}#.csv",
         )
@@ -527,103 +517,87 @@
             raise ValueError(
                 f"Task: {task} could not be found and custom_labels == []."
             )
         list_labels = custom_labels
     else:
         list_labels = annotation_tasks["tasks"][task]["labels"]
 
-    if tree_level == "child":
+    if tree_level == "patch":
         # specify the path of patches and the parent images
-        mymaps = load_patches(
-            patch_paths=patch_paths, parent_paths=parent_paths
-        )
+        mymaps = load_patches(patch_paths=patch_paths, parent_paths=parent_paths)
         if os.path.isfile(annot_file):
             mymaps.add_metadata(
                 metadata=annot_file,
-                index_col=-1,
-                delimiter=",",
+                index_col=0,
+                ignore_mismatch=True,
+                delimiter="\t",
                 tree_level=tree_level,
             )
 
-        calc_mean = calc_std = False
+        calc_mean = True
+        calc_std = False
         # Calculate mean before converting to pandas so the dataframe contains information about mean pixel intensity
-        if (
-            sortby == "mean"
-            or isinstance(min_alpha_channel, float)
-            or isinstance(min_mean_pixel, float)
-            or isinstance(max_mean_pixel, float)
-        ):
-            calc_mean = True
-        
-        if (
-            isinstance(min_std_pixel, float)
-            or isinstance(max_std_pixel, float)
-        ):
+        if isinstance(min_std_pixel, float) or isinstance(max_std_pixel, float):
             calc_std = True
 
         if calc_mean or calc_std:
             mymaps.calc_pixel_stats(calc_mean=calc_mean, calc_std=calc_std)
 
         # convert images to dataframe
-        _, sliced_df = mymaps.convertImages()
+        _, patch_df = mymaps.convert_images()
 
         if sortby == "mean":
-            sliced_df.sort_values("mean_pixel_RGB", inplace=True)
+            patch_df.sort_values("mean_pixel_R", inplace=True)
 
         if isinstance(min_alpha_channel, float):
-            if "mean_pixel_A" in sliced_df.columns:
-                sliced_df = sliced_df[
-                    sliced_df["mean_pixel_A"] >= min_alpha_channel
-                ]
+            if "mean_pixel_A" in patch_df.columns:
+                patch_df = patch_df[patch_df["mean_pixel_A"] >= min_alpha_channel]
 
         if isinstance(min_mean_pixel, float):
-            if "mean_pixel_RGB" in sliced_df.columns:
-                sliced_df = sliced_df[
-                    sliced_df["mean_pixel_RGB"] >= min_mean_pixel
-                ]
+            if "mean_pixel_R" in patch_df.columns:
+                patch_df = patch_df[patch_df["mean_pixel_R"] >= min_mean_pixel]
 
         if isinstance(max_mean_pixel, float):
-            if "mean_pixel_RGB" in sliced_df.columns:
-                sliced_df = sliced_df[
-                    sliced_df["mean_pixel_RGB"] <= max_mean_pixel
-                ]
+            if "mean_pixel_R" in patch_df.columns:
+                patch_df = patch_df[patch_df["mean_pixel_R"] <= max_mean_pixel]
 
         if isinstance(min_std_pixel, float):
-            if "std_pixel_RGB" in sliced_df.columns:
-                sliced_df = sliced_df[sliced_df["std_pixel_RGB"] >= min_std_pixel]
+            if "std_pixel_R" in patch_df.columns:
+                patch_df = patch_df[patch_df["std_pixel_R"] >= min_std_pixel]
 
         if isinstance(max_std_pixel, float):
-            if "std_pixel_RGB" in sliced_df.columns:
-                sliced_df = sliced_df[sliced_df["std_pixel_RGB"] <= max_std_pixel]
+            if "std_pixel_R" in patch_df.columns:
+                patch_df = patch_df[patch_df["std_pixel_R"] <= max_std_pixel]
 
         if isinstance(min_std_pixel, float):
-            if "std_pixel_RGB" in sliced_df.columns:
-                sliced_df = sliced_df[sliced_df["std_pixel_RGB"] >= min_std_pixel]
+            if "std_pixel_R" in patch_df.columns:
+                patch_df = patch_df[patch_df["std_pixel_R"] >= min_std_pixel]
 
         if isinstance(max_std_pixel, float):
-            if "std_pixel_RGB" in sliced_df.columns:
-                sliced_df = sliced_df[sliced_df["std_pixel_RGB"] <= max_std_pixel]
+            if "std_pixel_R" in patch_df.columns:
+                patch_df = patch_df[patch_df["std_pixel_R"] <= max_std_pixel]
 
         col_names = ["image_path", "parent_id"]
     else:
         mymaps = loader(path_images=parent_paths)
         if os.path.isfile(annot_file):
             mymaps.add_metadata(
                 metadata=annot_file,
-                index_col=-1,
-                delimiter=",",
+                index_col=0,
+                ignore_mismatch=True,
+                delimiter="\t",
                 tree_level=tree_level,
             )
         # convert images to dataframe
-        sliced_df, _ = mymaps.convertImages()
+        patch_df, _ = mymaps.convert_images()
         col_names = ["image_path"]
 
     # prepare data for annotation
     data2annotate = prepare_data(
-        sliced_df,
+        patch_df,
         col_names=col_names,
         annotation_set=annotation_set,
         redo=redo_annotation,
         random_state=random_state,
     )
 
     if len(data2annotate) == 0:
@@ -668,52 +642,51 @@
     -------
     None
     """
     with open(annotation_tasks_file) as f:
         annotation_tasks = yaml.load(f, Loader=yaml.FullLoader)
 
     if annotation_set not in annotation_tasks["paths"].keys():
-        print(
-            f"{annotation_set} could not be found in {annotation_tasks_file}"
-        )
+        print(f"{annotation_set} could not be found in {annotation_tasks_file}")
     else:
         annot_file = os.path.join(
             annotation_tasks["paths"][annotation_set]["annot_dir"],
             f"{task}_#{userID}#.csv",
         )
 
     annot_file_par = os.path.dirname(os.path.abspath(annot_file))
     if not os.path.isdir(annot_file_par):
         os.makedirs(annot_file_par)
 
     # Read an existing annotation file (for the same task and userID)
     try:
-        image_df = pd.read_csv(annot_file)
+        image_df = pd.read_csv(annot_file, sep="\t", index_col=0)
     except:
-        image_df = pd.DataFrame(columns=["image_id", "label"])
+        image_df = pd.DataFrame(columns=["image_id", "image_path", "label"])
 
     new_labels = 0
     newly_annotated = 0
     for i in range(len(annotation.tasks)):
         if annotation.tasks[i].value is not None:
             newly_annotated += 1
             if (
-                not annotation.tasks[i].output[0]
-                in image_df["image_id"].values.tolist()
+                annotation.tasks[i].output[0]
+                not in image_df["image_id"].values.tolist()
             ):
                 image_df = image_df.append(
                     {
                         "image_id": annotation.tasks[i].output[0],
+                        "image_path": annotation.tasks[i].output[1],
                         "label": annotation.tasks[i].value,
                     },
                     ignore_index=True,
                 )
                 new_labels += 1
 
     if len(image_df) > 0:
-        image_df = image_df.set_index("image_id")
-        image_df.to_csv(annot_file, mode="w")
+        #image_df = image_df.set_index("image_id")
+        image_df.to_csv(annot_file, mode="w", sep="\t")
         print(f"[INFO] Save {newly_annotated} new annotations to {annot_file}")
         print(f"[INFO] {new_labels} labels were not already stored")
-        print(f"[INFO] Total number of annotations: {len(image_df)}")
+        print(f"[INFO] Total number of saved annotations: {len(image_df)}")
     else:
         print("[INFO] No annotations to save!")
```

### Comparing `mapreader-0.3.4/mapreader/loader/images.py` & `mapreader-1.0.1.post0.dev9/mapreader/load/images.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,529 +1,650 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
 try:
     from geopy.distance import geodesic, great_circle
 except ImportError:
     pass
 
 import rasterio
 from glob import glob
 import matplotlib.pyplot as plt
+import matplotlib.patches as patches
 import matplotlib.image as mpimg
 import numpy as np
 import os
 import pandas as pd
-from PIL import Image
-from pylab import cm as pltcm
+from PIL import Image, ImageStat
+import PIL
 from pyproj import Transformer
 import random
 from typing import Literal, Optional, Union, Dict, Tuple, List, Any
+from tqdm import tqdm
+import rasterio
+from rasterio.plot import reshape_as_raster
+from shapely.geometry import box
 
-from mapreader.slicers.slicers import sliceByPixel
-
-# from ..utils import geo_utils
+os.environ['USE_PYGEOS'] = '0' #see here https://github.com/geopandas/geopandas/issues/2691
+import geopandas as geopd
 
 # Ignore warnings
 import warnings
 
 warnings.filterwarnings("ignore")
 
 
-class mapImages:
+class MapImages:
     """
     Class to manage a collection of image paths and construct image objects.
 
     Parameters
     ----------
     path_images : str or None, optional
         Path to the directory containing images (accepts wildcards). By
         default, ``False``
+    file_ext : str or False, optional
+        The file extension of the image files to be loaded, ignored if file types are specified in ``path_images`` (e.g. with ``"./path/to/dir/*png"``).
+        By default ``False``.
     tree_level : str, optional
         Level of the image hierarchy to construct. The value can be
-        ``"parent"`` (default) and ``"child"``.
+        ``"parent"`` (default) and ``"patch"``.
     parent_path : str, optional
         Path to parent images (if applicable), by default ``None``.
-    **kwds : dict, optional
-        Additional keyword arguments to be passed to the ``imagesConstructor``
+    **kwargs : dict, optional
+        Additional keyword arguments to be passed to the ``_images_constructor``
         method.
 
     Attributes
     ----------
     path_images : list
         List of paths to the image files.
     images : dict
         A dictionary containing the constructed image data. It has two levels
-        of hierarchy, ``"parent"`` and ``"child"``, depending on the value of
+        of hierarchy, ``"parent"`` and ``"patch"``, depending on the value of
         the ``tree_level`` parameter.
     """
 
     def __init__(
         self,
         path_images: Optional[str] = None,
+        file_ext: Optional[Union[str, bool]] = False,
         tree_level: Optional[str] = "parent",
         parent_path: Optional[str] = None,
-        **kwds: Dict,
+        **kwargs: Dict,
     ):
-        """Initializes the mapImages class."""
+        """Initializes the MapImages class."""
 
         if path_images:
-            # List with all paths
-            self.path_images = glob(os.path.abspath(path_images))
+            self.path_images = self._resolve_file_path(path_images, file_ext)
+
         else:
             self.path_images = []
 
         # Create images variable (MAIN object variable)
         # New methods (e.g., reading/loading) should construct images this way
-        self.images = {
-            "parent": {},
-            "child": {},
-        }
-        for image_path in self.path_images:
-            self.imagesConstructor(
+        self.images = {"parent": {}, "patch": {}}
+        self.parents = self.images["parent"]
+        self.patches = self.images["patch"]
+
+        for image_path in tqdm(self.path_images):
+            self._images_constructor(
                 image_path=image_path,
                 parent_path=parent_path,
                 tree_level=tree_level,
-                **kwds,
+                **kwargs,
+            )
+
+    @staticmethod
+    def _resolve_file_path(file_path, file_ext = None):
+        if file_ext:
+            if os.path.isdir(file_path):
+                files = glob(os.path.abspath(f"{file_path}/*.{file_ext}"))
+            else: #if not dir
+                files = glob(os.path.abspath(file_path))
+                files = [file for file in files if file.split(".")[-1] == file_ext] 
+
+        else:
+            if os.path.isdir(file_path):
+                files = glob(os.path.abspath(f"{file_path}/*.*"))
+            else:
+                files = glob(os.path.abspath(file_path))
+
+        #check for issues
+        if len(files) == 0:
+            raise ValueError("[ERROR] No files found!")
+        test_ext = files[0].split(".")[-1]
+        if not all(file.split(".")[-1] == test_ext for file in files):
+            raise ValueError(
+                "[ERROR] Directory with multiple file types detected - please specificy file extension (`patch_file_ext`) or, pass path to specific file types (wildcards accepted)."
             )
+        
+        return files
 
     def __len__(self) -> int:
-        return int(len(self.images["parent"]) + len(self.images["child"]))
+        return int(len(self.parents) + len(self.patches))
 
     def __str__(self) -> Literal[""]:
         print(f"#images: {self.__len__()}")
 
-        print(f"\n#parents: {len(self.images['parent'])}")
-        for i, img in enumerate(self.images["parent"]):
+        print(f"\n#parents: {len(self.parents)}")
+        for i, img in enumerate(self.parents):
             print(os.path.relpath(img))
             if i >= 10:
                 print("...")
                 break
 
-        print(f"\n#children: {len(self.images['child'])}")
-        for i, img in enumerate(self.images["child"]):
+        print(f"\n#patches: {len(self.patches)}")
+        for i, img in enumerate(self.patches):
             print(os.path.relpath(img))
             if i >= 10:
                 print("...")
                 break
         return ""
 
-    def imagesConstructor(
+    def _images_constructor(
         self,
         image_path: str,
         parent_path: Optional[str] = None,
-        tree_level: Optional[str] = "child",
-        **kwds: Dict,
+        tree_level: Optional[str] = "parent",
+        **kwargs: Dict,
     ) -> None:
         """
-        Constructs image data from the given image path and parent path and
-        adds it to the ``mapImages`` instance's ``images`` attribute.
+        Constructs image data from the given image path and parent path and adds it to the ``MapImages`` instance's ``images`` attribute.
 
         Parameters
         ----------
         image_path : str
             Path to the image file.
         parent_path : str, optional
             Path to the parent image (if applicable), by default ``None``.
         tree_level : str, optional
-            Level of the image hierarchy to construct, either ``"child"``
+            Level of the image hierarchy to construct, either ``"parent"``
             (default) or ``"parent"``.
-        **kwds : dict, optional
+        **kwargs : dict, optional
             Additional keyword arguments to be included in the constructed
             image data.
 
         Returns
         -------
         None
 
         Raises
         ------
         ValueError
-            If ``tree_level`` is not set to ``"parent"`` or ``"child"``.
-
-            If ``tree_level`` is set to ``"parent"`` and ``parent_path`` is
-            not ``None``.
+            If ``tree_level`` is not set to ``"parent"`` or ``"patch"``.
 
         Notes
         -----
-        This method assumes that the ``images`` attribute has been initialized
-        on the mapImages instance as a dictionary with two levels of hierarchy,
-        ``"parent"`` and ``"child"``. The image data is added to the
-        corresponding level based on the value of ``tree_level``.
+        This method assumes that the ``images`` attribute has been initialized on the MapImages instance as a dictionary with two levels of hierarchy, ``"parent"`` and ``"patch"``. The image data is added to the corresponding level based on the value of ``tree_level``.
         """
 
-        if tree_level not in ["parent", "child"]:
+        if tree_level not in ["parent", "patch"]:
             raise ValueError(
-                f"[ERROR] tree_level can only be set to parent or child, not: {tree_level}"  # noqa
+                f"[ERROR] tree_level can only be set to parent or patch, not: {tree_level}"  # noqa
             )
 
-        if (parent_path is not None) and (tree_level == "parent"):
-            raise ValueError(
-                "[ERROR] if tree_level=parent, parent_path should be None."
-            )
+        if tree_level == "parent":
+            if parent_path:
+                print(
+                    "[WARNING] Ignoring `parent_path` as `tree_level`  is set to 'parent'."
+                )
+                parent_path = None
+            parent_id = None
 
-        # Convert the image_path to its absolute path
-        image_path = os.path.abspath(image_path)
-        image_id, _ = self.splitImagePath(image_path)
+        abs_image_path, image_id, _ = self._convert_image_path(image_path)
 
+        self._check_image_mode(image_path)
+
+        # if parent_path is defined get absolute parent path and parent id (tree_level = "patch" is implied)
         if parent_path:
-            parent_path = os.path.abspath(parent_path)
-            parent_basename, _ = self.splitImagePath(parent_path)
-        else:
-            parent_basename, _ = None, None
+            abs_parent_path, parent_id, _ = self._convert_image_path(parent_path)
 
-        # --- Add other info to images
+        # add image, coords (if present), shape and other kwargs to dictionary
         self.images[tree_level][image_id] = {
-            "parent_id": parent_basename,
-            "image_path": image_path,
+            "parent_id": parent_id,
+            "image_path": abs_image_path,
         }
-
-        for k, v in kwds.items():
+        if tree_level == "parent":
+            try:
+                self._add_geo_info_id(image_id, verbose=False)
+            except:
+                pass
+        
+        self._add_shape_id(image_id)
+        for k, v in kwargs.items():
             self.images[tree_level][image_id][k] = v
 
-        # --- Make sure parent exists in images["parent"]
-        if tree_level == "child" and parent_basename:
-            # three possible scenarios
-            # 1. parent_basename is not in the parent dictionary
-            if parent_basename not in self.images["parent"].keys():
-                self.images["parent"][parent_basename] = {
+        if parent_id:  # tree_level = 'patch' is implied
+            if parent_id not in self.parents.keys():
+                self.parents[parent_id] = {
                     "parent_id": None,
-                    "image_path": parent_path,
+                    "image_path": abs_parent_path,
+                    "patches": [],
                 }
-            # 2. parent_basename exists but parent_id is not defined
-            if (
-                "parent_id"
-                not in self.images["parent"][parent_basename].keys()
-            ):
-                self.images["parent"][parent_basename]["parent_id"] = None
-            # 3. parent_basename exists but image_path is not defined
-            if (
-                "image_path"
-                not in self.images["parent"][parent_basename].keys()
-            ):
-                self.images["parent"][parent_basename][
-                    "image_path"
-                ] = parent_path
+
+            # add patch to parent
+            self._add_patch_to_parent(image_id)
 
     @staticmethod
-    def splitImagePath(inp_path: str) -> Tuple[str, str]:
+    def _check_image_mode(image_path):
+        try:
+            img = Image.open(image_path)       
+        except PIL.UnidentifiedImageError:
+            raise PIL.UnidentifiedImageError(f"[ERROR] {image_path} is not an image file.\n\n\
+See https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.open for more information."
+                                             )
+       
+        if img.mode not in ["1", "L", "LA", "I", "P", "RGB", "RGBA"]:
+            raise NotImplementedError(f"[ERROR] Image mode '{img.mode}' not currently accepted.\n\n\
+Please save your image(s) as one the following image modes: 1, L, LA, I, P, RGB or RGBA.\n\
+See https://pillow.readthedocs.io/en/stable/handbook/concepts.html#modes for more information."
+                                      )
+
+    @staticmethod
+    def _convert_image_path(inp_path: str) -> Tuple[str, str, str]:
         """
-        Split the input path into basename and dirname.
+        Convert an image path into an absolute path and find basename and directory name.
 
         Parameters
         ----------
         inp_path : str
             Input path to split.
 
         Returns
         -------
         tuple
-            A tuple containing the basename and dirname of the input path.
+            A tuple containing the absolute path, basename and directory name.
         """
-        inp_path = os.path.abspath(inp_path)
-        path_basename = os.path.basename(inp_path)
-        path_dirname = os.path.dirname(inp_path)
-        return path_basename, path_dirname
+        abs_path = os.path.abspath(inp_path)
+        path_basename = os.path.basename(abs_path)
+        path_dirname = os.path.dirname(abs_path)
+        return abs_path, path_basename, path_dirname
 
     def add_metadata(
         self,
         metadata: Union[str, pd.DataFrame],
+        index_col: Optional[Union[int, str]] = 0,
+        delimiter: Optional[str] = "\t",
         columns: Optional[List[str]] = None,
         tree_level: Optional[str] = "parent",
-        index_col: Optional[int] = 0,
-        delimiter: Optional[str] = "|",
+        ignore_mismatch: Optional[bool] = False,
     ) -> None:
         """
         Add metadata information to the images dictionary.
 
         Parameters
         ----------
         metadata : str or pandas.DataFrame
-            A csv file path (normally created from a pandas DataFrame) or a
-            pandas DataFrame that contains the metadata information.
-        columns : list, optional
-            List of columns to use, by default ``None``.
-        tree_level : str, optional
-            Determines which images dictionary (``"parent"`` or ``"child"``)
-            to add the metadata to, by default ``"parent"``.
-        index_col : int, optional
-            Column to use as the index when reading the csv file into a pandas
-            DataFrame, by default ``0``.
+            Path to a ``csv``, ``xls`` or ``xlsx`` file or a pandas DataFrame that contains the metadata information.
+        index_col : int or str, optional
+            Column to use as the index when reading the file and converting into a panda.DataFrame.
+            Accepts column indices or column names.
+            By default ``0`` (first column).
 
-            Needs only be provided if a csv file path is provided as
-            the ``metadata`` parameter.
+            Only used if a file path is provided as the ``metadata`` parameter.
+            Ingored if ``columns`` parameter is passed.
         delimiter : str, optional
-            Delimiter to use for reading the csv file into a pandas DataFrame,
-            by default ``"|"``.
+            Delimiter used in the ``csv`` file, by default ``"\t"``.
 
-            Needs only be provided if a csv file path is provided as
+            Only used if a ``csv`` file path is provided as
             the ``metadata`` parameter.
-
+        columns : list, optional
+            List of columns indices or names to add to MapImages.
+            If ``None`` is passed, all columns will be used.
+            By default ``None``.
+        tree_level : str, optional
+            Determines which images dictionary (``"parent"`` or ``"patch"``)
+            to add the metadata to, by default ``"parent"``.
+        ignore_mismatch : bool, optional
+            Whether to error if metadata with mismatching information is passed. 
+            By default ``False``.
+        
         Raises
         ------
         ValueError
-            If metadata is not a pandas DataFrame or a csv file path.
+            If metadata is not a pandas DataFrame or a ``csv``, ``xls`` or ``xlsx`` file path.
 
             If 'name' or 'image_id' is not one of the columns in the metadata.
 
         Returns
         -------
         None
+
+        Notes
+        ------
+        Your metadata file must contain an column which contains the image IDs (filenames) of your images.
+        This should have a column name of either ``name`` or ``image_id``.
+
+        Existing information in your ``MapImages`` object will be overwritten if there are overlapping column headings in your metadata file/dataframe.
         """
 
         if isinstance(metadata, pd.DataFrame):
-            metadata_df = metadata.copy()
-        elif os.path.isfile(metadata):
-            # read the metadata data
-            if index_col >= 0:
-                metadata_df = pd.read_csv(
-                    metadata, index_col=index_col, delimiter=delimiter
-                )
+            if columns:
+                metadata_df=metadata[columns].copy()
             else:
-                metadata_df = pd.read_csv(
-                    metadata, index_col=False, delimiter=delimiter
+                metadata_df=metadata.copy()
+                columns=list(metadata_df.columns)
+        
+        else: #if not df
+            if os.path.isfile(metadata):
+                if metadata.endswith('csv'):
+                    if columns:
+                        metadata_df = pd.read_csv(
+                            metadata, usecols=columns, delimiter=delimiter
+                            )
+                    else:
+                        metadata_df = pd.read_csv(
+                            metadata, index_col=index_col, delimiter=delimiter
+                            )
+                        columns=list(metadata_df.columns)
+                
+                elif metadata.endswith(('xls', 'xlsx')):
+                    if columns:
+                        metadata_df = pd.read_excel(
+                            metadata, usecols=columns,
+                            )
+                    else:
+                        metadata_df = pd.read_excel(
+                            metadata, index_col=index_col,
+                            )
+                        columns=list(metadata_df.columns)
+
+            else:
+                raise ValueError(
+                    "[ERROR] ``metadata`` should either be the path to a ``csv``, ``xls`` or ``xlsx`` file or a pandas DataFrame."  # noqa
                 )
-        else:
-            raise ValueError(
-                "metadata should either path to a csv file or pandas DataFrame."  # noqa
-            )
 
-        # remove duplicates using "name" column
-        if columns is None:
+        # identify image_id column
+        # what to do if "name" or "image_id" are index col?
+        if metadata_df.index.name in ["name", "image_id"]:
+            metadata_df[metadata_df.index.name] = metadata_df.index
             columns = list(metadata_df.columns)
 
-        if ("name" in columns) and ("image_id" in columns):
-            print(
-                "Both 'name' and 'image_id' columns exist! Use 'name' to index."  # noqa
-            )
-            image_id_col = "name"
         if "name" in columns:
             image_id_col = "name"
+            if "image_id" in columns:
+                print(
+                    "[WARNING] Both 'name' and 'image_id' columns exist! Using 'name' as index"  # noqa
+                )
         elif "image_id" in columns:
             image_id_col = "image_id"
         else:
             raise ValueError(
-                "'name' or 'image_id' should be one of the columns."
+                "[ERROR] 'name' or 'image_id' should be one of the columns."
             )
-        metadata_df.drop_duplicates(subset=[image_id_col])
 
-        for i, one_row in metadata_df.iterrows():
-            if not one_row[image_id_col] in self.images[tree_level].keys():
-                # print(f"[WARNING] {one_row[image_id_col]} does not exist in images, skip!")  # noqa
+        if any(metadata_df.duplicated(subset=image_id_col)):
+            print(
+                "[WARNING] Duplicates found in metadata. Keeping only first instance of each duplicated value"
+            )
+            metadata_df.drop_duplicates(subset=image_id_col, inplace=True, keep="first")
+
+        # look for non-intersecting values
+        missing_metadata = set(self.images[tree_level].keys()) - set(
+            metadata_df[image_id_col]
+        )
+        extra_metadata = set(metadata_df[image_id_col]) - set(
+            self.images[tree_level].keys()
+        )
+
+        if not ignore_mismatch:
+            if len(missing_metadata)!=0 and len(extra_metadata)!=0:
+                raise ValueError(f"[ERROR] Metadata is missing information for: {[*missing_metadata]}. \n\
+[ERROR] Metadata contains information about non-existant images: {[*extra_metadata]}"
+                )
+            elif len(missing_metadata)!=0: 
+                raise ValueError(
+                    f"[ERROR] Metadata is missing information for: {[*missing_metadata]}"
+                )
+            elif len(extra_metadata)!=0:
+                raise ValueError(
+                    f"[ERROR] Metadata contains information about non-existant images: {[*extra_metadata]}"
+                )
+
+        for key in self.images[tree_level].keys():
+            if key in missing_metadata:
                 continue
-            for one_col in columns:
-                if one_col in ["coord", "polygone"]:
-                    # Make sure "coord" is interpreted as a tuple
-                    self.images[tree_level][one_row[image_id_col]][
-                        one_col
-                    ] = eval(one_row[one_col])
-                else:
-                    self.images[tree_level][one_row[image_id_col]][
-                        one_col
-                    ] = one_row[one_col]
+            else:
+                data_series = metadata_df[metadata_df[image_id_col] == key].squeeze()
+                for column, item in data_series.items():
+                    try:
+                        self.images[tree_level][key][column] = eval(item)
+                    except:
+                        self.images[tree_level][key][column]=item
 
     def show_sample(
         self,
         num_samples: int,
-        tree_level: Optional[str] = "parent",
+        tree_level: Optional[str] = "patch",
         random_seed: Optional[int] = 65,
-        **kwds: Dict,
+        **kwargs: Dict,
     ) -> None:
         """
         Display a sample of images from a particular level in the image
         hierarchy.
 
         Parameters
         ----------
         num_samples : int
             The number of images to display.
         tree_level : str, optional
             The level of the hierarchy to display images from, which can be
-            ``"child"`` or ``"parent"`` (default).
+            ``"patch"`` or ``"parent"``. By default "patch".
         random_seed : int, optional
             The random seed to use for reproducibility. Default is ``65``.
-        **kwds : dict, optional
+        **kwargs : dict, optional
             Additional keyword arguments to pass to
             ``matplotlib.pyplot.figure()``.
 
         Returns
         -------
-        None
+        matplotlib.Figure
+            The figure generated
         """
         # set random seed for reproducibility
         random.seed(random_seed)
 
-        img_keys = list(self.images[tree_level].keys())
-        num_samples = min(len(img_keys), num_samples)
-        sample_img_keys = random.sample(img_keys, k=num_samples)
+        image_ids = list(self.images[tree_level].keys())
+        num_samples = min(len(image_ids), num_samples)
+        sample_image_ids = random.sample(image_ids, k=num_samples)
 
-        if not kwds.get("figsize"):
-            plt.figure(figsize=(15, num_samples * 2))
-        else:
-            plt.figure(figsize=kwds["figsize"])
+        figsize = kwargs.get("figsize", (15, num_samples * 2))
+        plt.figure(figsize=figsize)
 
-        for i, image_id in enumerate(sample_img_keys):
+        for i, image_id in enumerate(sample_image_ids):
             plt.subplot(num_samples // 3 + 1, 3, i + 1)
-            myimg = mpimg.imread(
-                self.images[tree_level][image_id]["image_path"]
-            )
+            img = Image.open(self.images[tree_level][image_id]["image_path"])
             plt.title(image_id, size=8)
-            plt.imshow(myimg)
+            plt.imshow(
+                img,
+            )
             plt.xticks([])
             plt.yticks([])
 
         plt.tight_layout()
         plt.show()
 
     def list_parents(self) -> List[str]:
         """Return list of all parents"""
-        return list(self.images["parent"].keys())
+        return list(self.parents.keys())
 
-    def list_children(self) -> List[str]:
-        """Return list of all children"""
-        return list(self.images["child"].keys())
+    def list_patches(self) -> List[str]:
+        """Return list of all patches"""
+        return list(self.patches.keys())
 
     def add_shape(self, tree_level: Optional[str] = "parent") -> None:
         """
         Add a shape to each image in the specified level of the image
         hierarchy.
 
         Parameters
         ----------
         tree_level : str, optional
             The level of the hierarchy to add shapes to, either ``"parent"``
-            (default) or ``"child"``.
+            (default) or ``"patch"``.
 
         Returns
         -------
         None
 
         Notes
         -----
-        The method runs :meth:`mapreader.loader.images.mapImages.add_shape_id`
+        The method runs :meth:`mapreader.load.images.MapImages._add_shape_id`
         for each image present at the ``tree_level`` provided.
         """
         print(f"[INFO] Add shape, tree level: {tree_level}")
 
-        list_items = list(self.images[tree_level].keys())
-        for item in list_items:
-            self.add_shape_id(image_id=item, tree_level=tree_level)
+        image_ids = list(self.images[tree_level].keys())
+        for image_id in image_ids:
+            self._add_shape_id(image_id=image_id)
 
-    def add_coord_increments(self) -> None:
+    def add_coord_increments(self, verbose: Optional[bool] = False) -> None:
         """
         Adds coordinate increments to each image at the parent level.
 
         Parameters
         ----------
-        None
+        verbose : bool, optional
+            Whether to print verbose outputs, by default ``False``.
 
         Returns
         -------
         None
 
         Notes
         -----
         The method runs
-        :meth:`mapreader.loader.images.mapImages.add_coord_increments_id`
+        :meth:`mapreader.load.images.MapImages._add_coord_increments_id`
         for each image present at the parent level, which calculates
         pixel-wise delta longitute (``dlon``) and delta latititude (``dlat``)
         for the image and adds the data to it.
         """
         print("[INFO] Add coord-increments, tree level: parent")
 
         parent_list = self.list_parents()
+
         for parent_id in parent_list:
-            if "coord" not in self.images["parent"][parent_id].keys():
+            if "coordinates" not in self.parents[parent_id].keys():
                 print(
-                    f"[WARNING] No coordinates found for {parent_id}. Suggestion: run add_metadata or addGeoInfo"  # noqa
+                    f"[WARNING] No coordinates found for {parent_id}. Suggestion: run add_metadata or add_geo_info."  # noqa
                 )
                 continue
 
-            self.add_coord_increments_id(image_id=parent_id)
+            self._add_coord_increments_id(image_id=parent_id, verbose=verbose)
 
-    def add_center_coord(self, tree_level: Optional[str] = "child") -> None:
+    def add_patch_coords(self, verbose: bool = False) -> None:
+        """Add coordinates to all patches in patches dictionary.
+
+        Parameters
+        ----------
+        verbose : bool, optional
+            Whether to print verbose outputs.
+            By default, ``False``
+        """
+        patch_list = self.list_patches()
+
+        for patch_id in tqdm(patch_list):
+            self._add_patch_coords_id(patch_id, verbose)
+
+    def add_patch_polygons(self, verbose: bool = False) -> None:
+        """Add polygon to all patches in patches dictionary.
+
+        Parameters
+        ----------
+        verbose : bool, optional
+            Whether to print verbose outputs.
+            By default, ``False``
+        """
+        patch_list = self.list_patches()
+
+        for patch_id in tqdm(patch_list):
+            self._add_patch_polygons_id(patch_id, verbose)
+
+    def add_center_coord(self, tree_level: Optional[str] = "patch", verbose: Optional[bool] = False) -> None:
         """
         Adds center coordinates to each image at the specified tree level.
 
         Parameters
         ----------
         tree_level: str, optional
             The tree level where the center coordinates will be added. It can
-            be either ``"parent"`` or ``"child"`` (default).
+            be either ``"parent"`` or ``"patch"`` (default).
+        verbose: bool, optional
+            Whether to print verbose outputs, by default ``False``.
 
         Returns
         -------
         None
 
         Notes
         -----
         The method runs
-        :meth:`mapreader.loader.images.mapImages.add_center_coord_id`
+        :meth:`mapreader.load.images.MapImages._add_center_coord_id`
         for each image present at the ``tree_level`` provided, which calculates
         central longitude and latitude (``center_lon`` and ``center_lat``) for
         the image and adds the data to it.
         """
         print(f"[INFO] Add center coordinates, tree level: {tree_level}")
 
-        list_items = list(self.images[tree_level].keys())
-        par_id_list = []
-        for item in list_items:
+        image_ids = list(self.images[tree_level].keys())
+
+        already_checked_parent_ids = (
+            []
+        )  # for if tree_level is patch, only print error message once for each parent image
+        for image_id in image_ids:
             if tree_level == "parent":
-                if "coord" not in self.images[tree_level][item].keys():
+                if "coordinates" not in self.parents[image_id].keys():
                     print(
-                        f"[WARNING] 'coord' could not be found in {item}. Suggestion: run add_metadata or addGeoInfo"  # noqa
+                        f"[WARNING] 'coordinates' could not be found in {image_id}. Suggestion: run add_metadata or add_geo_info"  # noqa
                     )
                     continue
 
-            if tree_level == "child":
-                par_id = self.images[tree_level][item]["parent_id"]
+            if tree_level == "patch":
+                parent_id = self.patches[image_id]["parent_id"]
 
-                if "coord" not in self.images["parent"][par_id].keys():
-                    if par_id not in par_id_list:
+                if "coordinates" not in self.parents[parent_id].keys():
+                    if parent_id not in already_checked_parent_ids:
                         print(
-                            f"[WARNING] 'coord' could not be found in {par_id} so center coordinates cannot be calculated for it's patches. Suggestion: run add_metadata or addGeoInfo"  # noqa
+                            f"[WARNING] 'coordinates' could not be found in {parent_id} so center coordinates cannot be calculated for it's patches. Suggestion: run add_metadata or add_geo_info."  # noqa
                         )
-                        par_id_list.append(par_id)
+                        already_checked_parent_ids.append(parent_id)
                     continue
 
-            self.add_center_coord_id(image_id=item, tree_level=tree_level)
+            self._add_center_coord_id(image_id=image_id, verbose=verbose)
 
-    def add_shape_id(
-        self, image_id: Union[int, str], tree_level: Optional[str] = "parent"
+    def _add_shape_id(
+        self,
+        image_id: Union[int, str],
     ) -> None:
         """
         Add shape (image_height, image_width, image_channels) of the image
-        with specified ``image_id`` in the given ``tree_level`` to the
-        metadata.
+        with specified ``image_id`` to the metadata.
 
         Parameters
         ----------
         image_id : int or str
             The ID of the image to add shape metadata to.
-        tree_level : str, optional
-            The tree level where the image is located, which can be
-            ``"parent"`` (default) or ``"child"``.
 
         Returns
         -------
         None
             This method does not return anything. It modifies the metadata of
             the ``images`` property in-place.
 
         Notes
         -----
         The shape of the image is obtained by loading the image from its
         ``image_path`` value and getting its shape.
         """
+        tree_level = self._get_tree_level(image_id)
+
         myimg = mpimg.imread(self.images[tree_level][image_id]["image_path"])
         # shape = (hwc)
         myimg_shape = myimg.shape
         self.images[tree_level][image_id]["shape"] = myimg_shape
 
-    def add_coord_increments_id(
+    def _add_coord_increments_id(
         self, image_id: Union[int, str], verbose: Optional[bool] = False
     ) -> None:
         """
         Add pixel-wise delta longitute (``dlon``) and delta latititude
         (``dlat``) to the metadata of the image with the specified ``image_id``
         in the parent tree level.
 
@@ -544,1236 +665,1084 @@
         Notes
         -----
         Coordinate increments (dlon and dlat) are calculated using the
         following formula:
 
         .. code-block:: python
 
-            dlon = abs(lon_max - lon_min) / image_width
             dlat = abs(lat_max - lat_min) / image_height
+            dlon = abs(lon_max - lon_min) / image_width
 
-        ``lon_max``, ``lon_min``, ``lat_max``, ``lat_min`` are the coordinate
-        bounds of the image, and ``image_width`` and ``image_height`` are the
-        width and height of the image in pixels respectively.
+        ``lon_min``, ``lat_min``, ``lon_max`` and ``lat_max`` are the coordinate
+        bounds of the image, and ``image_height`` and ``image_width`` are the
+        height and width of the image in pixels respectively.
 
         This method assumes that the coordinate and shape metadata of the
         image have already been added to the metadata.
 
         If the coordinate metadata cannot be found, a warning message will be
         printed if ``verbose=True``.
 
         If the shape metadata cannot be found, this method will call the
-        :meth:`mapreader.loader.images.mapImages.add_shape_id` method to add
+        :meth:`mapreader.load.images.MapImages._add_shape_id` method to add
         it.
         """
-        # Check for warnings
-        if "coord" not in self.images["parent"][image_id].keys():
-            if verbose:
-                print(
-                    f"[WARNING]'coord' could not be found in {image_id}. Suggestion: run add_metadata or addGeoInfo"  # noqa
-                )
+
+        if "coordinates" not in self.parents[image_id].keys():
+            self._print_if_verbose(
+                f"[WARNING]'coordinates' could not be found in {image_id}. Suggestion: run add_metadata or add_geo_info.",
+                verbose,
+            )
             return
 
-        # Add shapes if non-existent
-        if "shape" not in self.images["parent"][image_id].keys():
-            self.add_shape_id(image_id)
-
-        # Extract height/width/chan from shape
-        image_height, image_width, _ = self.images["parent"][image_id]["shape"]
-
-        # Extract coordinates from image
-        lon_min, lon_max, lat_min, lat_max = self.images["parent"][image_id][
-            "coord"
-        ]
+        if "shape" not in self.parents[image_id].keys():
+            self._add_shape_id(image_id)
+
+        image_height, image_width, _ = self.parents[image_id]["shape"]
+
+        # Extract coordinates from image (xmin, ymin, xmax, ymax)
+        min_x, min_y, max_x, max_y = self.parents[image_id]["coordinates"]
 
         # Calculate dlon and dlat
-        dlon = abs(lon_max - lon_min) / image_width
-        dlat = abs(lat_max - lat_min) / image_height
+        dlon = abs(max_x - min_x) / image_width
+        dlat = abs(max_y - min_y) / image_height
+
+        self.parents[image_id]["dlon"] = dlon
+        self.parents[image_id]["dlat"] = dlat
+
+    def _add_patch_coords_id(self, image_id: str, verbose: bool = False) -> None:
+        """Get coordinates of a patch
+
+        Parameters
+        ----------
+        image_id : str
+            The ID of the patch
+        verbose : bool, optional
+            Whether to print verbose outputs.
+            By default, ``False``.
+
+        Return
+        -------
+        None
+        """
+        parent_id = self.patches[image_id]["parent_id"]
+
+        if "coordinates" not in self.parents[parent_id].keys():
+            self._print_if_verbose(
+                f"[WARNING] No coordinates found in  {parent_id} (parent of {image_id}). Suggestion: run add_metadata or add_geo_info.",
+                verbose,
+            )
+            return
+
+        else:
+            if not all([k in self.parents[parent_id].keys() for k in ["dlat", "dlon"]]):
+                self._add_coord_increments_id(parent_id)
+
+            # get min_x and min_y and pixel-wise dlon and dlat for parent image
+            parent_min_x = self.parents[parent_id]["coordinates"][0]
+            parent_min_y = self.parents[parent_id]["coordinates"][1]
+            dlon = self.parents[parent_id]["dlon"]
+            dlat = self.parents[parent_id]["dlat"]
+
+            # get patch bounds
+            pixel_bounds = self.patches[image_id]["pixel_bounds"]
+
+            # get patch coords
+            min_x = (pixel_bounds[0] * dlon) + parent_min_x
+            min_y = (pixel_bounds[1] * dlat) + parent_min_y
+            max_x = (pixel_bounds[2] * dlon) + parent_min_x
+            max_y = (pixel_bounds[3] * dlat) + parent_min_y
+
+            self.patches[image_id]["coordinates"] = (min_x, min_y, max_x, max_y)
+            self.patches[image_id]["crs"] = self.parents[parent_id]["crs"]
 
-        # Assign values
-        self.images["parent"][image_id]["dlon"] = dlon
-        self.images["parent"][image_id]["dlat"] = dlat
+    def _add_patch_polygons_id(self, image_id: str, verbose: bool = False) -> None:
+        """Create polygon from a patch and save to patch dictionary.
+
+        Parameters
+        ----------
+        image_id : str
+            The ID of the patch
+        verbose : bool, optional
+            Whether to print verbose outputs.
+            By default, ``False``.
+
+        Return
+        -------
+        None
+        """
+        
+        if "coordinates" not in self.patches[image_id].keys():
+            self._add_patch_coords_id(image_id, verbose)
+        
+        if "coordinates" in self.patches[image_id].keys():
+            coords = self.patches[image_id]["coordinates"]
+            self.patches[image_id]["polygon"] = box(*coords)
 
-    def add_center_coord_id(
+    def _add_center_coord_id(
         self,
         image_id: Union[int, str],
-        tree_level: Optional[str] = "child",
         verbose: Optional[bool] = False,
     ) -> None:
         """
         Calculates and adds center coordinates (longitude as ``center_lon``
-        and latitude as ``center_lat``) to a given image patch.
+        and latitude as ``center_lat``) to a given image_id's dictionary.
 
         Parameters
         ----------
         image_id : int or str
-            The ID of the image patch to add center coordinates to.
-        tree_level : str, optional
-            The level of the image patch in the image hierarchy, either
-            ``"parent"`` or ``"child"`` (default).
+            The ID of the patch to add center coordinates to.
         verbose : bool, optional
             Whether to print warning messages or not. Defaults to ``False``.
 
-        Raises
-        ------
-        NotImplementedError
-            If ``tree_level`` is not set to ``"parent"`` or ``"child"``.
-
         Returns
         -------
         None
         """
-        if tree_level == "child":
-            par_id = self.images[tree_level][image_id]["parent_id"]
-
-            if ("dlon" not in self.images["parent"][par_id].keys()) or (
-                "dlat" not in self.images["parent"][par_id].keys()
-            ):
-                if "coord" not in self.images["parent"][par_id].keys():
-                    if verbose:
-                        print(
-                            f"[WARNING] No coordinates found for {image_id}. Suggestion: run add_metadata or addGeoInfo"  # noqa
-                        )
-                    return
-
-                else:
-                    self.add_coord_increments_id(par_id)
-
-            dlon = self.images["parent"][par_id]["dlon"]
-            dlat = self.images["parent"][par_id]["dlat"]
-            lon_min, lon_max, lat_min, lat_max = self.images["parent"][par_id][
-                "coord"
-            ]
-            min_abs_x = self.images[tree_level][image_id]["min_x"] * dlon
-            max_abs_x = self.images[tree_level][image_id]["max_x"] * dlon
-            min_abs_y = self.images[tree_level][image_id]["min_y"] * dlat
-            max_abs_y = self.images[tree_level][image_id]["max_y"] * dlat
 
-            self.images[tree_level][image_id]["center_lon"] = (
-                lon_min + (min_abs_x + max_abs_x) / 2.0
-            )
-            self.images[tree_level][image_id]["center_lat"] = (
-                lat_max - (min_abs_y + max_abs_y) / 2.0
-            )
+        tree_level = self._get_tree_level(image_id)
 
-        elif tree_level == "parent":
-            if "coord" not in self.images[tree_level][image_id].keys():
-                if verbose:
-                    print(
-                        f"[WARNING] No coordinates found for {image_id}. Suggestion: run add_metadata or addGeoInfo"  # noqa
-                    )
+        if "coordinates" not in self.images[tree_level][image_id].keys():
+            if tree_level == "parent":
+                self._print_if_verbose(
+                    f"[WARNING] No coordinates found for {image_id}. Suggestion: run add_metadata or add_geo_info.",
+                    verbose,
+                )
                 return
 
-            print(f"[INFO] Reading 'coord' from {image_id}")
-            lon_min, lon_max, lat_min, lat_max = self.images[tree_level][
-                image_id
-            ]["coord"]
-            self.images[tree_level][image_id]["center_lon"] = (
-                lon_min + lon_max
-            ) / 2.0
-            self.images[tree_level][image_id]["center_lat"] = (
-                lat_min + lat_max
-            ) / 2.0
-        else:
-            raise NotImplementedError(
-                "Tree level must be set to 'parent' or 'child'."
-            )
+            if tree_level == "patch":
+                self._add_patch_coords_id(image_id, verbose)
+
+        if "coordinates" in self.images[tree_level][image_id].keys():
+            self._print_if_verbose(f"[INFO] Reading 'coordinates' from {image_id}.", verbose)
+            min_x, min_y, max_x, max_y = self.images[tree_level][image_id][
+                "coordinates"
+            ]
+            self.images[tree_level][image_id]["center_lat"] = np.mean([min_y, max_y])
+            self.images[tree_level][image_id]["center_lon"] = np.mean([min_x, max_x])
 
-    def calc_pixel_width_height(
+    def _calc_pixel_height_width(
         self,
         parent_id: Union[int, str],
-        calc_size_in_m: Optional[str] = "great-circle",
+        method: Optional[str] = "great-circle",
         verbose: Optional[bool] = False,
-    ) -> Tuple[float, float, float, float]:
+    ) -> Tuple[Tuple, float, float]:
         """
-        Calculate the width and height of each pixel in a given image in
-        meters.
+        Calculate the height and width of each pixel in a given image in meters.
 
         Parameters
         ----------
         parent_id : int or str
             The ID of the parent image to calculate pixel size.
-        calc_size_in_m : str, optional
+        method : str, optional
             Method to use for calculating image size in meters.
-            Possible values: ``"great-circle"`` (default), ``"gc"`` (alias for
-            ``"great-circle"``), ``"geodesic"``. ``"great-circle"`` and
-            ``"gc"`` compute size using the great-circle distance formula,
-            while ``"geodesic"`` computes size using the geodesic distance
-            formula.
+
+            Possible values: ``"great-circle"`` (default), ``"gc"``, ``"great_circle"``, ``"geodesic"`` or ``"gd"``.
+            ``"great-circle"``, ``"gc"`` and ``"great_circle"`` compute size using the great-circle distance formula,
+            while ``"geodesic"`` and ``"gd"`` computes size using the geodesic distance formula.
         verbose : bool, optional
             If ``True``, print additional information during the calculation.
             Default is ``False``.
 
         Returns
         -------
-        tuple of floats
-            The size of the image in meters as a tuple of bottom, top, left,
-            and right distances (in that order).
+        tuple
+            Tuple containing the size of the image in meters (as a tuple of left, bottom, right and top distances) and the mean pixel height and width in meters.
 
         Notes
         -----
         This method requires the parent image to have location metadata added
-        with either the :meth:`mapreader.loader.images.mapImages.add_metadata`
-        or :meth:`mapreader.loader.images.mapImages.addGeoInfo` methods.
+        with either the :meth:`mapreader.load.images.MapImages.add_metadata`
+        or :meth:`mapreader.load.images.MapImages.add_geo_info` methods.
 
         The calculations are performed using the ``geopy.distance.geodesic``
         and ``geopy.distance.great_circle`` methods. Thus, the method requires
         the ``geopy`` package to be installed.
         """
 
-        if "coord" not in self.images["parent"][parent_id].keys():
+        if "coordinates" not in self.parents[parent_id].keys():
             print(
-                f"[WARNING] 'coord' could not be found in {parent_id}. Suggestion: run add_metadata or addGeoInfo"  # noqa
+                f"[WARNING] 'coordinates' could not be found in {parent_id}. Suggestion: run add_metadata or add_geo_info."  # noqa
             )
             return
 
-        myimg = mpimg.imread(self.images["parent"][parent_id]["image_path"])
-        image_height, image_width, _ = myimg_shape = myimg.shape
+        if "shape" not in self.parents[parent_id].keys():
+            self._add_shape_id(parent_id)
 
-        (xmin, xmax, ymin, ymax) = self.images["parent"][parent_id]["coord"]
-        if verbose:
-            print("[INFO] Using coordinates to compute width/height:")
-            print(f"[INFO] lon min/max: {xmin:.4f}/{xmax:.4f}")
-            print(f"[INFO] lat min/max: {ymin:.4f}/{ymax:.4f}")
-            print(f"[INFO] shape (hwc): {myimg_shape}")
+        height, width, _ = self.parents[parent_id]["shape"]
+        xmin, ymin, xmax, ymax = self.parents[parent_id]["coordinates"]
 
         # Calculate the size of image in meters
-        if calc_size_in_m == "geodesic":
+        if method in ["geodesic", "gd"]:
             bottom = geodesic((ymin, xmin), (ymin, xmax)).meters
             right = geodesic((ymin, xmax), (ymax, xmax)).meters
             top = geodesic((ymax, xmax), (ymax, xmin)).meters
             left = geodesic((ymax, xmin), (ymin, xmin)).meters
-            size_in_m = (bottom, top, left, right)
-            if verbose:
-                print(
-                    f"[INFO] size (in meters) bottom/top/left/right: {bottom:.2f}/{top:.2f}/{left:.2f}/{right:.2f}"  # noqa
-                )
 
-            mean_width = np.mean(
-                [size_in_m[0] / image_width, size_in_m[1] / image_width]
-            )
-            mean_height = np.mean(
-                [size_in_m[2] / image_height, size_in_m[3] / image_height]
-            )
-            if verbose:
-                print(
-                    f"Each pixel is ~{mean_width:.3f} X {mean_height:.3f} meters (width x height)."  # noqa
-                )
-
-        elif calc_size_in_m in ["gc", "great-circle"]:
+        elif method in ["gc", "great-circle", "great_circle"]:
             bottom = great_circle((ymin, xmin), (ymin, xmax)).meters
             right = great_circle((ymin, xmax), (ymax, xmax)).meters
             top = great_circle((ymax, xmax), (ymax, xmin)).meters
             left = great_circle((ymax, xmin), (ymin, xmin)).meters
-            size_in_m = (bottom, top, left, right)
-            if verbose:
-                print(
-                    f"[INFO] size (in meters) bottom/top/left/right: {bottom:.2f}/{top:.2f}/{left:.2f}/{right:.2f}"  # noqa
-                )
 
-            mean_width = np.mean(
-                [size_in_m[0] / image_width, size_in_m[1] / image_width]
-            )
-            mean_height = np.mean(
-                [size_in_m[2] / image_height, size_in_m[3] / image_height]
+        else:
+            raise NotImplementedError(
+                f'[ERROR] Method must be one of "great-circle", "great_cirlce", "gc", "geodesic" or "gd", not: {method}'
             )
-            if verbose:
-                print(
-                    f"Each pixel is ~{mean_width:.3f} x {mean_height:.3f} meters (width x height)."  # noqa
-                )
 
-        return size_in_m
+        size_in_m = (left, bottom, right, top)  # anticlockwise order
 
-    def sliceAll(
+        mean_pixel_height = np.mean([right / height, left / height])
+        mean_pixel_width = np.mean([bottom / width, top / width])
+
+        self._print_if_verbose(
+            f"[INFO] Size in meters of left/bottom/right/top: {left:.2f}/{bottom:.2f}/{right:.2f}/{top:.2f}",
+            verbose,
+        )
+        self._print_if_verbose(
+            f"Each pixel is ~{mean_pixel_height:.3f} X {mean_pixel_width:.3f} meters (height x width).",
+            verbose,
+        )  # noqa
+
+        return size_in_m, mean_pixel_height, mean_pixel_width
+
+    def patchify_all(
         self,
         method: Optional[str] = "pixel",
-        slice_size: Optional[int] = 100,
-        path_save: Optional[str] = "sliced_images",
+        patch_size: Optional[int] = 100,
+        tree_level: Optional[str] = "parent",
+        path_save: Optional[str] = None,
+        add_to_parents: Optional[bool] = True,
         square_cuts: Optional[bool] = False,
         resize_factor: Optional[bool] = False,
         output_format: Optional[str] = "png",
         rewrite: Optional[bool] = False,
         verbose: Optional[bool] = False,
-        tree_level: Optional[str] = "parent",
-        add2child: Optional[bool] = True,
-        id1: Optional[int] = 0,
-        id2: Optional[int] = -1,
     ) -> None:
         """
-        Slice all images in the specified ``tree_level`` and add the sliced
-        images to the mapImages instance's ``images`` dictionary.
+        Patchify all images in the specified ``tree_level`` and (if ``add_to_parents=True``) add the patches to the MapImages instance's ``images`` dictionary.
 
         Parameters
         ----------
         method : str, optional
-            Method used to slice images, choices between ``"pixel"`` (default)
+            Method used to patchify images, choices between ``"pixel"`` (default)
             and ``"meters"`` or ``"meter"``.
-        slice_size : int, optional
+        patch_size : int, optional
             Number of pixels/meters in both x and y to use for slicing, by
             default ``100``.
+        tree_level : str, optional
+            Tree level, choices between ``"parent"`` or ``"patch``, by default
+            ``"parent"``.
         path_save : str, optional
-            Directory to save the sliced images, by default
-            ``"sliced_images"``.
+            Directory to save the patches.
+            If None, will be set as f"patches_{patch_size}_{method}" (e.g. "patches_100_pixel").
+            By default None.
+        add_to_parents : bool, optional
+            If True, patches will be added to the MapImages instance's
+            ``images`` dictionary, by default ``True``.
         square_cuts : bool, optional
-            If True, all sliced images will have the same number of pixels in
+            If True, all patches will have the same number of pixels in
             x and y, by default ``False``.
         resize_factor : bool, optional
-            If True, resize the images before slicing, by default ``False``.
+            If True, resize the images before patchifying, by default ``False``.
         output_format : str, optional
             Format to use when writing image files, by default ``"png"``.
         rewrite : bool, optional
-            If True, existing slices will be rewritten, by default ``False``.
+            If True, existing patches will be rewritten, by default ``False``.
         verbose : bool, optional
             If True, progress updates will be printed throughout, by default
             ``False``.
-        tree_level : str, optional
-            Tree level, choices between ``"parent"`` or ``"child``, by default
-            ``"parent"``.
-        add2child : bool, optional
-            If True, sliced images will be added to the mapImages instance's
-            ``images`` dictionary, by default ``True``.
-        id1 : int, optional
-            The start index of the images to slice. Default is ``0``.
-        id2 : int, optional
-            The end index of the images to slice. Default is ``-1`` (i.e., all
-            images after index ``id1`` will be sliced).
-
-        Raises
-        ------
-        ValueError
-            If ``id2 < id1``.
 
         Returns
         -------
         None
         """
-        if id2 < 0:
-            img_keys = list(self.images[tree_level].keys())[id1:]
-        elif id2 < id1:
-            raise ValueError("id2 should be > id1.")
-        else:
-            img_keys = list(self.images[tree_level].keys())[id1:id2]
 
-        for image_id in img_keys:
+        image_ids = self.images[tree_level].keys()
+        original_patch_size = patch_size
+
+        if path_save is None:
+            path_save = f"patches_{patch_size}_{method}"
+        
+        print(f'[INFO] Saving patches in directory named "{path_save}".')
+
+        for image_id in tqdm(image_ids):
             image_path = self.images[tree_level][image_id]["image_path"]
 
-            sliced_images_info = self._slice(
-                image_path=image_path,
-                method=method,
-                slice_size=slice_size,
+            self._print_if_verbose(f"[INFO] Patchifying {os.path.relpath(image_path)}", verbose)
+
+            # make sure the dir exists
+            self._make_dir(path_save)
+
+            if method in ["meters", "meter"]:
+                if "coordinates" not in self.images[tree_level][image_id].keys():
+                    raise ValueError(
+                        "[ERROR] Please add coordinate information first. Suggestion: Run add_metadata or add_geo_info."  # noqa
+                    )
+
+                mean_pixel_height = self._calc_pixel_height_width(image_id)[1]
+                patch_size = int(
+                    original_patch_size / mean_pixel_height
+                )  ## check this is correct - should patch be different size in x and y?
+
+            self._patchify_by_pixel(
+                image_id=image_id,
+                patch_size=patch_size,
                 path_save=path_save,
+                add_to_parents=add_to_parents,
                 square_cuts=square_cuts,
                 resize_factor=resize_factor,
                 output_format=output_format,
                 rewrite=rewrite,
                 verbose=verbose,
-                image_id=image_id,
-                tree_level=tree_level,
             )
 
-            if add2child:
-                for i in range(len(sliced_images_info)):
-                    # Add sliced images to the .images["child"]
-                    self.imagesConstructor(
-                        image_path=sliced_images_info[i][0],
-                        parent_path=image_path,
-                        tree_level="child",
-                        min_x=sliced_images_info[i][1][0],
-                        min_y=sliced_images_info[i][1][1],
-                        max_x=sliced_images_info[i][1][2],
-                        max_y=sliced_images_info[i][1][3],
-                    )
-
-        if add2child:
-            # add children to the parent dictionary
-            self.addChildren()
-
-    def _slice(
+    def _patchify_by_pixel(
         self,
-        image_path: str,
-        method: Optional[str] = "pixel",
-        slice_size: Optional[int] = 100,
-        path_save: Optional[str] = "sliced_images",
+        image_id: str,
+        patch_size: int,
+        path_save: str,
+        add_to_parents: Optional[bool] = True,
         square_cuts: Optional[bool] = False,
         resize_factor: Optional[bool] = False,
         output_format: Optional[str] = "png",
         rewrite: Optional[bool] = False,
-        verbose: Optional[bool] = True,
-        image_id: Optional[Union[int, str]] = None,
-        tree_level: Optional[str] = None,
-    ) -> List:
-        """
-        Slice one image
-
-        ..
-            Private method.
+        verbose: Optional[bool] = False,
+    ):
+        """Patchify one image and (if ``add_to_parents=True``) add the patch to the MapImages instance's ``images`` dictionary.
 
         Parameters
         ----------
-        image_path : str
-            Path to image.
-        method : str, optional
-            Method used to slice images, choices between ``"pixel"`` and
-            ``"meters"`` or ``"meter"``, by default ``"pixel"``.
-        slice_size : int, optional
-            Number of pixels/meters in both x and y to use for slicing, by
-            default ``100``.
-        path_save : str, optional
-            Directory to save the sliced images, by default
-            ``"sliced_images"``.
+        image_id : str
+            The ID of the image to patchify
+        patch_size : int
+            Number of pixels in both x and y to use for slicing
+        path_save : str
+            Directory to save the patches.
+        add_to_parents : bool, optional
+            If True, patches will be added to the MapImages instance's
+            ``images`` dictionary, by default ``True``.
         square_cuts : bool, optional
-            If ``True``, all sliced images will have the same number of pixels
-            in x and y, by default ``False``.
+            If True, all patches will have the same number of pixels in
+            x and y, by default ``False``.
         resize_factor : bool, optional
-            If ``True``, resize the images before slicing, by
-            ``False``.
+            If True, resize the images before patchifying, by default ``False``.
         output_format : str, optional
-            Format to use when writing image files, by default
-            ``"png"``.
+            Format to use when writing image files, by default ``"png"``.
         rewrite : bool, optional
-            If ``True``, existing slices will be rewritten, by default
-            ``False``.
+            If True, existing patches will be rewritten, by default ``False``.
         verbose : bool, optional
-            If ``True``, progress updates will be printed throughout, by
-            default ``False``.
-        tree_level : str, optional
-            Tree level, choices between ``"parent"`` or ``"child"``, by
-            default ``"parent"``.
-
-        Returns
-        -------
-        list
-            sliced_images_info
+            If True, progress updates will be printed throughout, by default
+            ``False``.
         """
+        tree_level = self._get_tree_level(image_id)
 
-        print(40 * "=")
-        print(f"Slicing {os.path.relpath(image_path)}")
-        print(40 * "-")
-
-        # make sure the dir exists
-        self._makeDir(path_save)
-
-        # which image should be sliced
-        image_path = os.path.abspath(image_path)
-        sliced_images_info = None
-        if method == "pixel":
-            sliced_images_info = sliceByPixel(
-                image_path=image_path,
-                slice_size=slice_size,
-                path_save=path_save,
-                square_cuts=square_cuts,
-                resize_factor=resize_factor,
-                output_format=output_format,
-                rewrite=rewrite,
-                verbose=verbose,
-            )
-
-        elif method in ["meters", "meter"]:
-            keys = self.images[tree_level][image_id].keys()
+        parent_path = self.images[tree_level][image_id]["image_path"]
+        img = Image.open(parent_path)
 
-            if "coord" not in keys:
-                raise ValueError(
-                    "Please add coordinate information first. Suggestion: Run add_metadata or addGeoInfo"  # noqa
+        if resize_factor:
+            original_height, original_width = img.height, img.width
+            img = img.resize(
+                (
+                    int(original_width / resize_factor),
+                    int(original_height / resize_factor),
                 )
+            )
 
-            if "shape" not in keys:
-                self.add_shape_id(image_id=image_id, tree_level=tree_level)
+        height, width = img.height, img.width
 
-            image_height, _, _ = self.images[tree_level][image_id]["shape"]
+        for x in range(0, width, patch_size):
+            for y in range(0, height, patch_size):
+                max_x = min(x + patch_size, width)
+                max_y = min(y + patch_size, height)
+
+                if (
+                    square_cuts
+                ):  # move min_x and min_y back a bit so the patch is square
+                    min_x = x - (patch_size - (max_x - x))
+                    min_y = y - (patch_size - (max_y - y))
 
-            # size in meter contains: (bottom, top, left, right)
-            size_in_m = self.calc_pixel_width_height(image_id)
+                else:
+                    min_x = x
+                    min_y = y
 
-            # pixel height in m per pixel
-            pixel_height = size_in_m[2] / image_height
-            number_pixels4slice = int(slice_size / pixel_height)
+                patch_id = f"patch-{min_x}-{min_y}-{max_x}-{max_y}-#{image_id}#.{output_format}"
+                patch_path = os.path.join(path_save, patch_id)
+                patch_path = os.path.abspath(patch_path)
+
+                if os.path.isfile(patch_path) and not rewrite:
+                    self._print_if_verbose(
+                        f"[INFO] File already exists: {patch_path}.", verbose
+                    )
+                
+                else:
+                    self._print_if_verbose(
+                        f'[INFO] Creating "{patch_id}". Number of pixels in x,y: {max_x - min_x},{max_y - min_y}.',
+                        verbose,
+                    )
 
-            sliced_images_info = sliceByPixel(
-                image_path=image_path,
-                slice_size=number_pixels4slice,
-                path_save=path_save,
-                square_cuts=square_cuts,
-                resize_factor=resize_factor,
-                output_format=output_format,
-                rewrite=rewrite,
-                verbose=verbose,
-            )
+                    patch = img.crop((min_x, min_y, max_x, max_y))
+                    patch.save(patch_path, output_format)
 
-        return sliced_images_info
+                if add_to_parents:
+                    self._images_constructor(
+                        image_path=patch_path,
+                        parent_path=parent_path,
+                        tree_level="patch",
+                        pixel_bounds=(min_x, min_y, max_x, max_y),
+                    )
+                    self._add_patch_coords_id(patch_id)
+                    self._add_patch_polygons_id(patch_id)
 
-    def addChildren(self) -> None:
+    def _add_patch_to_parent(self, patch_id: str) -> None:
         """
-        Add children to parent.
+        Add patch to parent.
+
+        Parameters
+        ----------
+        patch_id : str
+            The ID of the patch to be added
 
         Returns
         -------
         None
 
         Notes
         -----
-        This method adds children to their corresponding parent image. It
-        checks if the parent image has any child image, and if not, it creates
-        a list of children and assigns it to the parent. If the parent image
-        already has a list of children, the method checks if the current child
-        is already in the list. If not, the child is added to the list.
-        """
-        for child in self.images["child"].keys():
-            my_parent = self.images["child"][child]["parent_id"]
-            if not self.images["parent"][my_parent].get("children", False):
-                self.images["parent"][my_parent]["children"] = [child]
-            else:
-                if child not in self.images["parent"][my_parent]["children"]:
-                    self.images["parent"][my_parent]["children"].append(child)
+        This method adds patches to their corresponding parent image.
 
-    def _makeDir(
-        self, path_make: str, exists_ok: Optional[bool] = True
-    ) -> None:
+        It checks if the parent image has any patches, and if not, it creates
+        a list of patches and assigns it to the parent. If the parent image
+        already has a list of patches, the method checks if the current patch
+        is already in the list. If not, the patch is added to the list.
+        """
+        patch_parent = self.patches[patch_id]["parent_id"]
+
+        if patch_parent not in self.parents.keys():
+            self.load_parents(parent_ids=patch_parent)
+        
+        if "patches" not in self.parents[patch_parent].keys():
+            self.parents[patch_parent]["patches"] = [patch_id]
+        else:
+            if patch_id not in self.parents[patch_parent]["patches"]:
+                self.parents[patch_parent]["patches"].append(patch_id)
+
+    def _make_dir(self, path_make: str, exists_ok: Optional[bool] = True) -> None:
         """
         Helper method to make directories.
 
         ..
             Private method.
         """
         os.makedirs(path_make, exist_ok=exists_ok)
 
     def calc_pixel_stats(
         self,
-        parent_id: Optional[Union[str, int]] = None,
+        parent_id: Optional[str] = None,
         calc_mean: Optional[bool] = True,
         calc_std: Optional[bool] = True,
+        verbose: Optional[bool] = False,
     ) -> None:
         """
         Calculate the mean and standard deviation of pixel values for all
-        channels (R, G, B, RGB and, if present, Alpha) of all child images of
-        a given parent image. Store the results in the mapImages instance's
+        channels of all patches of
+        a given parent image. Store the results in the MapImages instance's
         ``images`` dictionary.
 
         Parameters
         ----------
-        parent_id : str, int, or None, optional
-            The ID of the parent image to calculate pixel stats for. If
-            ``None``, calculate pixel stats for all parent images.
+        parent_id : str or None, optional
+            The ID of the parent image to calculate pixel stats for.
+            If ``None``, calculate pixel stats for all parent images.
+            By default, None
         calc_mean : bool, optional
-            Whether to calculate mean pixel values. Default is ``True``.
+            Whether to calculate mean pixel values. By default, ``True``.
         calc_std : bool, optional
-            Whether to calculate standard deviation of pixel values. Default
-            is ``True``.
+            Whether to calculate standard deviation of pixel values.
+            By default, ``True``.
+        verbose : bool, optional
+            Whether to print verbose outputs. By default, ``False``.
 
         Returns
         -------
         None
 
         Notes
         -----
-        - Pixel stats are calculated for child images of the parent image
+        - Pixel stats are calculated for patches of the parent image
           specified by ``parent_id``.
         - If ``parent_id`` is ``None``, pixel stats are calculated for all
           parent images in the object.
         - If mean or standard deviation of pixel values has already been
-          calculated for a child image, the calculation is skipped.
+          calculated for a patch, the calculation is skipped.
         - Pixel stats are stored in the ``images`` attribute of the
-          ``mapImages`` instance, under the ``child`` key for each child image.
-        - If no children are found for a parent image, a warning message is
+          ``MapImages`` instance, under the ``patch`` key for each patch.
+        - If no patches are found for a parent image, a warning message is
           displayed and the method moves on to the next parent image.
         """
         # Get correct parent ID
         if parent_id is None:
             parent_ids = self.list_parents()
         else:
             parent_ids = [parent_id]
 
-        for parent_id in parent_ids:
-            print(10 * "-")
-            print(f"[INFO] calculate pixel stats for image: {parent_id}")
+        for parent_id in tqdm(parent_ids):
+            self._print_if_verbose(
+                f"\n[INFO] Calculating pixel stats for patches of image: {parent_id}", verbose
+            )
 
-            if "children" not in self.images["parent"][parent_id]:
-                print(f"[WARNING] No child found for: {parent_id}")
+            if "patches" not in self.parents[parent_id]:
+                print(f"[WARNING] No patches found for: {parent_id}")
                 continue
 
-            list_children = self.images["parent"][parent_id]["children"]
+            list_patches = self.parents[parent_id]["patches"]
 
-            for child in list_children:
-                child_data = self.images["child"][child]
+            for patch in list_patches:
+                patch_data = self.patches[patch]
+                patch_keys = patch_data.keys()
+                img = Image.open(patch_data["image_path"])
+                bands = img.getbands()
 
-                # Check whether calculation has already been run
-                child_keys = child_data.keys()
-                if all(
-                    [
-                        "mean_pixel_RGB" in child_keys,
-                        "std_pixel_RGB" in child_keys,
-                    ]
-                ):
-                    continue
+                if calc_mean:
+                    if all(f"mean_pixel_{band}" in patch_keys for band in bands):
+                        calc_mean = False
+                if calc_std:
+                    if all(f"std_pixel_{band}" in patch_keys for band in bands):
+                        calc_std = False
 
-                # Load image
-                child_img = mpimg.imread(child_data["image_path"])
+                img_stat = ImageStat.Stat(img)
 
                 if calc_mean:
-                    # Calculate mean pixel values
-                    self.images["child"][child]["mean_pixel_R"] = np.mean(
-                        child_img[:, :, 0]
-                    )
-                    self.images["child"][child]["mean_pixel_G"] = np.mean(
-                        child_img[:, :, 1]
-                    )
-                    self.images["child"][child]["mean_pixel_B"] = np.mean(
-                        child_img[:, :, 2]
-                    )
-                    self.images["child"][child]["mean_pixel_RGB"] = np.mean(
-                        child_img[:, :, 0:3]
-                    )
-                    # check whether alpha is present
-                    if child_img.shape[2] > 3:
-                        self.images["child"][child]["mean_pixel_A"] = np.mean(
-                            child_img[:, :, 3]
-                        )
+                    img_mean = img_stat.mean
+                    for i, band in enumerate(bands):
+                        # Calculate mean pixel values
+                        self.patches[patch][f"mean_pixel_{band}"] = img_mean[i] / 255
+
                 if calc_std:
-                    # Calculate standard deviation for pixel values
-                    self.images["child"][child]["std_pixel_R"] = np.std(
-                        child_img[:, :, 0]
-                    )
-                    self.images["child"][child]["std_pixel_G"] = np.std(
-                        child_img[:, :, 1]
-                    )
-                    self.images["child"][child]["std_pixel_B"] = np.std(
-                        child_img[:, :, 2]
-                    )
-                    self.images["child"][child]["std_pixel_RGB"] = np.std(
-                        child_img[:, :, 0:3]
-                    )
-                    # check whether alpha is present
-                    if child_img.shape[2] > 3:
-                        self.images["child"][child]["std_pixel_A"] = np.std(
-                            child_img[:, :, 3]
-                        )
+                    img_std = img_stat.stddev
+                    for i, band in enumerate(bands):
+                        # Calculate std pixel values
+                        self.patches[patch][f"std_pixel_{band}"] = img_std[i] / 255
 
-    def convertImages(self) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    def convert_images(self, save: Optional[bool] = False, save_format: Optional[str] ="csv") -> Tuple[pd.DataFrame, pd.DataFrame]:
         """
-        Convert the ``mapImages`` instance's ``images`` dictionary into pandas
+        Convert the ``MapImages`` instance's ``images`` dictionary into pandas
         DataFrames for easy manipulation.
 
+        Parameters
+        ----------
+
+        save : bool, optional
+            Whether to save the dataframes as files. By default ``False``.
+        save_format : str, optional
+            If ``save = True``, the file format to use when saving the dataframes.
+            Options of csv ("csv") or excel ("excel" or "xlsx"). 
+            By default, "csv".
+
         Returns
         -------
         tuple of two pandas DataFrames
             The method returns a tuple of two DataFrames: One for the
-            ``parent`` images and one for the ``child`` images.
+            ``parent`` images and one for the ``patch`` images.
         """
-        parents = pd.DataFrame.from_dict(self.images["parent"], orient="index")
-        children = pd.DataFrame.from_dict(self.images["child"], orient="index")
+        parent_df = pd.DataFrame.from_dict(self.parents, orient="index")
+        patch_df = pd.DataFrame.from_dict(self.patches, orient="index")
 
-        return parents, children
+        parent_df.index.set_names("image_id", inplace=True)
+        patch_df.index.set_names("image_id", inplace=True)
 
-    def show_par(
+        if save:
+
+            if save_format == "csv":
+                parent_df.to_csv("parent_df.csv", sep="\t")
+                print('[INFO] Saved parent dataframe as "parent_df.csv"')
+                patch_df.to_csv("patch_df.csv", sep="\t")
+                print('[INFO] Saved patch dataframe as "patch_df.csv"')
+            elif save_format in ["excel", "xlsx"]:
+                parent_df.to_excel("parent_df.xlsx")
+                print('[INFO] Saved parent dataframe as "parent_df.xlsx"')
+                patch_df.to_excel("patch_df.xlsx")
+                print('[INFO] Saved patch dataframe as "patch_df.xslx"')
+
+            else:
+                raise ValueError(f'[ERROR] ``save_format`` should be one of "csv", "excel" or "xlsx". Not {save_format}.')
+
+        return parent_df, patch_df
+
+    def show_parent(
         self,
-        parent_id: Union[int, str],
-        value: Optional[Union[List[str], bool]] = False,
-        **kwds,
+        parent_id: str,
+        column_to_plot: Optional[str] = None,
+        **kwargs: Dict,
     ) -> None:
         """
-        A wrapper method for `.show()` which plots all children of a
+        A wrapper method for `.show()` which plots all patches of a
         specified parent (`parent_id`).
 
         Parameters
         ----------
-        parent_id : int or str
+        parent_id : str
             ID of the parent image to be plotted.
-        value : list or bool, optional
-            Value to be plotted on each child image, by default False.
+        column_to_plot : str, optional
+            Column whose values will be plotted on patches, by default ``None``.
+        **kwargs: Dict
+            Key words to pass to ``show`` method.
+            See help text for ``show`` for more information.
 
         Returns
         -------
-        None
-
-        Raises
-        ------
-        KeyError
-            If the parent_id is not found in the image dictionary.
+        list
+            A list of figures created by the method.
 
         Notes
         -----
         This is a wrapper method. See the documentation of the
-        :meth:`mapreader.loader.images.mapImages.show` method for more detail.
+        :meth:`mapreader.load.images.MapImages.show` method for more detail.
         """
-        image_ids = self.images["parent"][parent_id]["children"]
-        self.show(image_ids, value=value, **kwds)
+        patch_ids = self.parents[parent_id]["patches"]
+        figures = self.show(patch_ids, column_to_plot=column_to_plot, **kwargs)
+        
+        return figures
 
     def show(
         self,
         image_ids: Union[str, List[str]],
-        value: Optional[Union[str, List[str], bool]] = False,
+        column_to_plot: Optional[str] = None,
+        figsize: Optional[tuple] = (10,10),
         plot_parent: Optional[bool] = True,
-        border: Optional[bool] = True,
+        patch_border: Optional[bool] = True,
         border_color: Optional[str] = "r",
-        vmin: Optional[Union[float, List[float]]] = 0.5,
-        vmax: Optional[Union[float, List[float]]] = 2.5,
-        colorbar: Optional[Union[str, List[str]]] = "viridis",
-        alpha: Optional[Union[float, List[float]]] = 1.0,
-        discrete_colorbar: Optional[Union[int, List[int]]] = 256,
-        tree_level: Optional[str] = "child",
-        grid_plot: Optional[Tuple[int, int]] = (20000, 20000),
-        plot_histogram: Optional[bool] = True,
+        vmin: Optional[float] = None,
+        vmax: Optional[float] = None,
+        alpha: Optional[float] = 1.0,
+        cmap: Optional[str] = "viridis",
+        discrete_cmap: Optional[int] = 256,
+        plot_histogram: Optional[bool] = False,
         save_kml_dir: Optional[Union[bool, str]] = False,
         image_width_resolution: Optional[int] = None,
         kml_dpi_image: Optional[int] = None,
-        **kwds: Dict,
     ) -> None:
         """
         Plot images from a list of `image_ids`.
 
         Parameters
         ----------
         image_ids : str or list
             Image ID or list of image IDs to be plotted.
-        value : str, list or bool, optional
-            Value to plot on child images, by default ``False``.
+        column_to_plot : str, optional
+            Column whose values will be plotted on patches, by default ``None``.
         plot_parent : bool, optional
             If ``True``, parent image will be plotted in background, by
             default ``True``.
-        border : bool, optional
-            If ``True``, a border will be placed around each child image, by
+        figsize : tuple, optional
+            The size of the figure to be plotted. By default, ``(10,10)``.
+        patch_border : bool, optional
+            If ``True``, a border will be placed around each patch, by
             default ``True``.
         border_color : str, optional
             The color of the border. Default is ``"r"``.
-        vmin : float or list, optional
-            The minimum value for the colormap. By default ``0.5``.
-
-            If a list is provided, it must be the same length as ``image_ids``.
-        vmax : float or list, optional
-            The maximum value for the colormap. By default ``2.5``.
-
-            If a list is provided, it must be the same length as ``image_ids``.
-        colorbar : str or list, optional
-            Colorbar used to visualise chosen ``value``, by default
-            ``"viridis"``.
-
-            If a list is provided, it must be the same length as ``image_ids``.
-        alpha : float or list, optional
+        vmin : float, optional
+            The minimum value for the colormap.
+            If ``None``, will be set to minimum value in ``column_to_plot``, by default ``None``.
+        vmax : float, optional
+            The maximum value for the colormap.
+            If ``None``, will be set to the maximum value in ``column_to_plot``, by default ``None``.
+        alpha : float, optional
             Transparency level for plotting ``value`` with floating point
-            values ranging from 0.0 (transparent) to 1 (opaque). By default,
-            ``1.0``.
-
-            If a list is provided, it must be the same length as ``image_ids``.
-        discrete_colorbar : int or list, optional
-            Number of discrete colurs to use in colorbar, by default ``256``.
-
-            If a list is provided, it must be the same length as ``image_ids``.
-        tree_level : str, optional
-            The level of the image tree to be plotted. Must be either
-            ``"child"`` (default) or ``"parent"``.
-        grid_plot : tuple, optional
-            The size of the grid (number of rows and columns) to be used to
-            plot images. Later adjusted to the true min/max of all subplots.
-            By default ``(20000, 20000)``.
+            values ranging from 0.0 (transparent) to 1 (opaque), by default ``1.0``.
+        cmap : str, optional
+            Colour map used to visualise chosen ``column_to_plot`` values, by default ``"viridis"``.
+        discrete_cmap : int, optional
+            Number of discrete colours to use in colour map, by default ``256``.
         plot_histogram : bool, optional
-            If ``True``, plot histograms of the ``value`` of images. By
-            default ``True``.
+            If ``True``, plot histograms of the ``value`` of images. By default ``False``.
         save_kml_dir : str or bool, optional
             If ``True``, save KML files of the images. If a string is provided,
             it is the path to the directory in which to save the KML files. If
             set to ``False``, no files are saved. By default ``False``.
         image_width_resolution : int or None, optional
             The pixel width to be used for plotting. If ``None``, the
             resolution is not changed. Default is ``None``.
 
             Note: Only relevant when ``tree_level="parent"``.
         kml_dpi_image : int or None, optional
             The resolution, in dots per inch, to create KML images when
             ``save_kml_dir`` is specified (as either ``True`` or with path).
             By default ``None``.
-
+        
         Returns
         -------
-        None
+        list
+            A list of figures created by the method.
         """
         # create list, if not already a list
-        if not (isinstance(image_ids, list) or isinstance(image_ids, tuple)):
+        if isinstance(image_ids, str):
             image_ids = [image_ids]
-        values = [value] if not (isinstance(value, list)) else value[:]
-        vmins = [vmin] if not (isinstance(vmin, list)) else vmin[:]
-        vmaxs = [vmax] if not (isinstance(vmax, list)) else vmax[:]
-        colorbars = (
-            [colorbar] if not (isinstance(colorbar, list)) else colorbar[:]
-        )
-        alphas = [alpha] if not (isinstance(alpha, list)) else alpha[:]
-        discrete_colorbars = (
-            [discrete_colorbar]
-            if not (isinstance(discrete_colorbar, list))
-            else discrete_colorbar[:]
-        )
 
-        if tree_level == "parent":
-            for one_image_id in image_ids:
-                figsize = self._get_kwds(kwds, "figsize")
-                plt.figure(figsize=figsize)
-
-                par_path = self.images["parent"][one_image_id]["image_path"]
-                par_image = Image.open(par_path)
-
-                # Change the resolution of the image if image_width_resolution
-                # is specified
-                if image_width_resolution is not None:
-                    basewidth = int(image_width_resolution)
-                    wpercent = basewidth / float(par_image.size[0])
-                    hsize = int((float(par_image.size[1]) * float(wpercent)))
-                    par_image = par_image.resize(
-                        (basewidth, hsize), Image.ANTIALIAS
-                    )
+        if not isinstance(image_ids, list):
+            raise ValueError(
+                f"[ERROR] Please pass image_ids as str or list of strings."
+            )
 
-                # remove the borders
-                plt.gca().set_axis_off()
-                plt.subplots_adjust(
-                    top=1, bottom=0, right=1, left=0, hspace=0, wspace=0
-                )
+        if all(self._get_tree_level(image_id) == "parent" for image_id in image_ids):
+            tree_level = "parent"
+        elif all(self._get_tree_level(image_id) == "patch" for image_id in image_ids):
+            tree_level = "patch"
+        else:
+            raise ValueError("[ERROR] Image IDs must all be at the same tree level")
 
-                plt.imshow(
-                    par_image,
-                    zorder=1,
-                    interpolation="nearest",
-                    extent=(0, par_image.size[0], par_image.size[1], 0),
-                )
+        figures = []
+        if tree_level == "parent":
+            for image_id in tqdm(image_ids):
+                image_path = self.parents[image_id]["image_path"]
+                img = Image.open(image_path)
+
+                # if image_width_resolution is specified, resize the image
+                if image_width_resolution:
+                    new_width = int(image_width_resolution)
+                    rescale_factor = new_width / img.width
+                    new_height = int(img.height * rescale_factor)
+                    img = img.resize((new_width, new_height), Image.LANCZOS)
+
+                fig = plt.figure(figsize=figsize)
+                plt.axis("off")
+                plt.imshow(img, zorder=1)
+
+                if column_to_plot:
+                    print(
+                        "[WARNING] Values are only plotted on patches. If you'd like to plot values on all patches of a parent image, use ``show_parent`` instead."
+                    )
 
                 if save_kml_dir:
-                    if (
-                        "coord"
-                        not in self.images["parent"][one_image_id].keys()
-                    ):
+                    if "coordinates" not in self.parents[image_id].keys():
                         print(
-                            "[WARNING] 'coord' could not be found. This is needed when save_kml_dir is set...continue"  # noqa
+                            f"[WARNING] 'coordinates' could not be found in {image_id} so no KML file can be created/saved."  # noqa
                         )
                         continue
+                    else:
+                        os.makedirs(save_kml_dir, exist_ok=True)
+                        kml_out_path = os.path.join(save_kml_dir, image_id)
+
+                        plt.savefig(
+                            kml_out_path,
+                            bbox_inches="tight",
+                            pad_inches=0,
+                            dpi=kml_dpi_image,
+                        )
 
-                    # remove x/y ticks when creating KML out of images
-                    plt.xticks([])
-                    plt.yticks([])
+                        self._create_kml(
+                            kml_out_path=kml_out_path,
+                            column_to_plot=column_to_plot,
+                            coords=self.parents[image_id]["coordinates"],
+                            counter=-1,
+                        )
 
-                    os.makedirs(save_kml_dir, exist_ok=True)
-                    path2kml = os.path.join(save_kml_dir, f"{one_image_id}")
-                    plt.savefig(
-                        f"{path2kml}",
-                        bbox_inches="tight",
-                        pad_inches=0,
-                        dpi=kml_dpi_image,
-                    )
+                plt.title(image_id)
+                figures.append(fig)
 
-                    self._createKML(
-                        path2kml=path2kml,
-                        value=one_image_id,
-                        coords=self.images["parent"][one_image_id]["coord"],
-                        counter=-1,
-                    )
-                else:
-                    plt.title(one_image_id)
-                    plt.show()
+            return figures
 
-        elif tree_level == "child":
+        elif tree_level == "patch":
             # Collect parents information
-            parents = {}
-            for i in range(len(image_ids)):
-                try:
-                    parent_id = self.images[tree_level][image_ids[i]][
-                        "parent_id"
-                    ]
-                except Exception as err:
-                    print(err)
+            parent_images = {}
+            for image_id in image_ids:
+                parent_id = self.patches[image_id].get("parent_id", None)
+
+                if parent_id is None:
+                    print(f"[WARNING] {image_id} has no parent. Skipping.")
                     continue
 
-                if parent_id not in parents:
-                    parents[parent_id] = {
-                        "path": self.images["parent"][parent_id]["image_path"],
-                        "child": [],
+                if parent_id not in parent_images.keys():
+                    parent_images[parent_id] = {
+                        "image_path": self.parents[parent_id]["image_path"],
+                        "patches": [image_id],
                     }
+                else:
+                    parent_images[parent_id]["patches"].append(image_id)
 
-                parents[parent_id]["child"].append(image_ids[i])
-
-            for i in parents.keys():
-                figsize = self._get_kwds(kwds, "figsize")
-                plt.figure(figsize=figsize)
-
-                for i_value, value in enumerate(values):
-                    # initialize image2plot
-                    # will be filled with values of 'value'
-                    image2plot = np.empty(grid_plot)
-                    image2plot[:] = np.nan
-                    min_x, min_y, max_x, max_y = (
-                        grid_plot[1],
-                        grid_plot[0],
-                        0,
-                        0,
-                    )
-                    for child_id in parents[i]["child"]:
-                        one_image = self.images[tree_level][child_id]
-
-                        # Set the values for each child
-                        if not value:
-                            pass
-
-                        elif value == "const":
-                            # Assign values to image2plot, update min_x,
-                            # min_y, ...
-                            image2plot[
-                                one_image["min_y"] : one_image["max_y"],
-                                one_image["min_x"] : one_image["max_x"],
-                            ] = 1.0
-
-                        elif value == "random":
-                            import random
-
-                            # assign values to image2plot, update min_x,
-                            # min_y, ...
-                            image2plot[
-                                one_image["min_y"] : one_image["max_y"],
-                                one_image["min_x"] : one_image["max_x"],
-                            ] = random.random()
-
-                        elif value:
-                            if value not in one_image:
-                                assign_value = None
-                            else:
-                                assign_value = one_image[value]
-                            # assign values to image2plot, update min_x,
-                            # min_y, ...
-                            image2plot[
-                                one_image["min_y"] : one_image["max_y"],
-                                one_image["min_x"] : one_image["max_x"],
-                            ] = assign_value
-
-                        # reset min/max of x and y
-                        min_x = min(min_x, one_image["min_x"])
-                        min_y = min(min_y, one_image["min_y"])
-                        max_x = max(max_x, one_image["max_x"])
-                        max_y = max(max_y, one_image["max_y"])
-
-                        if border:
-                            self._plotBorder(
-                                one_image, plt, color=border_color
-                            )
-
-                    if value:
-                        vmin = vmins[i_value]
-                        vmax = vmaxs[i_value]
-                        alpha = alphas[i_value]
-                        colorbar = colorbars[i_value]
-                        discrete_colorbar = discrete_colorbars[i_value]
-
-                        # set discrete colorbar
-                        colorbar = pltcm.get_cmap(colorbar, discrete_colorbar)
-
-                        # Adjust image2plot to global min/max in x and y
-                        # directions
-                        image2plot = image2plot[min_y:max_y, min_x:max_x]
-                        plt.imshow(
-                            image2plot,
-                            zorder=10 + i_value,
-                            interpolation="nearest",
-                            cmap=colorbar,
-                            vmin=vmin,
-                            vmax=vmax,
-                            alpha=alpha,
-                            extent=(min_x, max_x, max_y, min_y),
+            # plot each parent
+            for parent_id in tqdm(parent_images.keys()):
+                fig, ax = plt.subplots(figsize=figsize)
+                ax.axis("off")
+
+                # initialize values_array - will be filled with values of 'value'
+                parent_height, parent_width, _ = self.parents[parent_id]["shape"]
+                values_array = np.full((parent_height, parent_width), np.nan)
+
+                for patch_id in self.parents[parent_id]["patches"]:
+                    patch_dic = self.patches[patch_id]
+                    pixel_bounds = patch_dic[
+                        "pixel_bounds"
+                    ]  # min_x, min_y, max_x, max_y
+
+                    # Set the values for each patch
+                    if column_to_plot:
+                        patch_value = patch_dic.get(column_to_plot, None)
+
+                        # assign values to values_array
+                        values_array[
+                            pixel_bounds[1] : pixel_bounds[3],
+                            pixel_bounds[0] : pixel_bounds[2],
+                        ] = patch_value
+
+                    if patch_border:
+                        patch_xy = (pixel_bounds[0], pixel_bounds[1])
+                        patch_width = pixel_bounds[2] - pixel_bounds[0]  # max_x - min_x
+                        patch_height = (
+                            pixel_bounds[3] - pixel_bounds[1]
+                        )  # max_y - min_y
+                        rect = patches.Rectangle(
+                            patch_xy,
+                            patch_width,
+                            patch_height,
+                            fc="none",
+                            ec=border_color,
+                            lw=1,
+                            zorder=20,
                         )
+                        ax.add_patch(rect)
 
-                        if save_kml_dir:
-                            plt.xticks([])
-                            plt.yticks([])
-                        else:
-                            plt.colorbar(fraction=0.03)
+                if column_to_plot:
+                    vmin = vmin if vmin else np.min(values_array)
+                    vmax = vmax if vmax else np.max(values_array)
+
+                    # set discrete colorbar
+                    cmap = plt.get_cmap(cmap, discrete_cmap)
+
+                    values_plot = ax.imshow(
+                        values_array,
+                        zorder=10,
+                        cmap=cmap,
+                        vmin=vmin,
+                        vmax=vmax,
+                        alpha=alpha,
+                    )
+                    
+                    fig.colorbar(values_plot, shrink=0.8)
 
                 if plot_parent:
-                    par_path = os.path.join(parents[i]["path"])
-                    par_image = mpimg.imread(par_path)
-                    plt.imshow(
-                        par_image,
-                        zorder=1,
-                        interpolation="nearest",
-                        extent=(0, par_image.shape[1], par_image.shape[0], 0),
-                    )
-                    if not save_kml_dir:
-                        plt.title(i)
+                    parent_path = parent_images[parent_id]["image_path"]
+                    parent_image = Image.open(parent_path)
 
-                if not save_kml_dir:
-                    plt.show()
-                else:
+                    ax.imshow(parent_image)
+
+                if save_kml_dir:
                     os.makedirs(save_kml_dir, exist_ok=True)
-                    path2kml = os.path.join(save_kml_dir, f"{value}_{i}")
+                    kml_out_path = os.path.join(save_kml_dir, parent_id)
                     plt.savefig(
-                        f"{path2kml}",
+                        f"{kml_out_path}",
                         bbox_inches="tight",
                         pad_inches=0,
                         dpi=kml_dpi_image,
                     )
-
-                    self._createKML(
-                        path2kml=path2kml,
-                        value=value,
-                        coords=self.images["parent"][i]["coord"],
-                        counter=i,
+                    self._create_kml(
+                        kml_out_path=kml_out_path,
+                        column_to_plot=column_to_plot,
+                        coords=self.parents[image_id]["coordinates"],
+                        counter=-1,
                     )
 
-                if value and plot_histogram:
-                    histogram_range = self._get_kwds(kwds, "histogram_range")
-                    plt.figure(figsize=(7, 5))
-                    plt.hist(
-                        image2plot.flatten(),
-                        color="k",
-                        bins=np.arange(
-                            histogram_range[0] - histogram_range[2] / 2.0,
-                            histogram_range[1] + histogram_range[2],
-                            histogram_range[2],
-                        ),
-                    )
-                    plt.xlabel(value, size=20)
-                    plt.ylabel("Freq.", size=20)
-                    plt.xticks(size=18)
-                    plt.yticks(size=18)
-                    plt.grid()
-                    plt.show()
+                ax.set_title(image_id)
+                figures.append(fig)
+
+                if column_to_plot and plot_histogram:
+                    self._hist_values_array(column_to_plot, values_array)
 
-    def _createKML(
+            return figures
+
+    def _create_kml(
         self,
-        path2kml: str,
-        value: str,
+        kml_out_path: str,
+        column_to_plot: str,
         coords: Union[List, Tuple],
         counter: Optional[int] = -1,
     ) -> None:
         """Create a KML file.
 
         ..
             Private method.
 
         Parameters
         ----------
         path2kml : str
             Directory to save KML file.
         value : _type_
-            Value to be plotted on the underlying image.
-            See `.show()` for detail.
+            Column to plot on underlying image.
         coords : list or tuple
             Coordinates of the bounding box.
         counter : int, optional
             Counter to be used for HREF, by default `-1`.
         """
 
         try:
             import simplekml
         except ImportError:
-            raise ImportError(
-                "[ERROR] simplekml is needed to create KML outputs."
-            )
+            raise ImportError("[ERROR] simplekml is needed to create KML outputs.")
 
-        (lon_min, lon_max, lat_min, lat_max) = coords
+        (lon_min, lat_min, lon_max, lat_max) = coords  # (xmin, ymin, xmax, ymax)
 
         # -----> create KML
         kml = simplekml.Kml()
         ground = kml.newgroundoverlay(name=str(counter))
         if counter == -1:
-            ground.icon.href = f"./{value}"
+            ground.icon.href = f"./{column_to_plot}"
         else:
-            ground.icon.href = f"./{value}_{counter}"
+            ground.icon.href = f"./{column_to_plot}_{counter}"
 
         ground.latlonbox.north = lat_max
         ground.latlonbox.south = lat_min
         ground.latlonbox.east = lon_max
         ground.latlonbox.west = lon_min
         # ground.latlonbox.rotation = -14
 
-        kml.save(f"{path2kml}.kml")
+        kml.save(f"{kml_out_path}.kml")
 
-    def _plotBorder(
+    def _hist_values_array(
         self,
-        image_dict: Dict,
-        plt: plt,
-        linewidth: Optional[int] = 0.5,
-        zorder: Optional[int] = 20,
-        color: Optional[str] = "r",
-    ) -> None:
-        """Plot border for an image
-
-        ..
-            Private method.
-
-        Arguments:
-            image_dict : dict
-                image dictionary, e.g., one item in ``self.images["child"]``
-            plt : matplotlib.pyplot object
-                a matplotlib.pyplot object
-
-        Keyword Arguments:
-            linewidth : int
-                line-width (default: ``2``)
-            zorder : int
-                z-order for the border (default: ``5``)
-            color : str
-                color of the border (default: ``"r"``)
-        """
-        plt.plot(
-            [image_dict["min_x"], image_dict["min_x"]],
-            [image_dict["min_y"], image_dict["max_y"]],
-            lw=linewidth,
-            zorder=zorder,
-            color=color,
-        )
-        plt.plot(
-            [image_dict["min_x"], image_dict["max_x"]],
-            [image_dict["max_y"], image_dict["max_y"]],
-            lw=linewidth,
-            zorder=zorder,
-            color=color,
-        )
-        plt.plot(
-            [image_dict["max_x"], image_dict["max_x"]],
-            [image_dict["max_y"], image_dict["min_y"]],
-            lw=linewidth,
-            zorder=zorder,
-            color=color,
-        )
-        plt.plot(
-            [image_dict["max_x"], image_dict["min_x"]],
-            [image_dict["min_y"], image_dict["min_y"]],
-            lw=linewidth,
-            zorder=zorder,
-            color=color,
+        column_to_plot,
+        values_array,
+    ):
+        plt.figure(figsize=(7, 5))
+        plt.hist(
+            values_array.flatten(),
+            color="k",
+            bins=20,
         )
 
-    @staticmethod
-    def _get_kwds(
-        kwds: Dict, key: str
-    ) -> Union[Tuple[int, int], int, List[Union[int, float]], Any]:
-        """
-        If ``kwds`` dictionary has the ``key``, return value; otherwise, use
-        default for ``key`` provided.
-
-        ..
-            Private method.
-        """
-        if key in kwds:
-            return kwds[key]
-        else:
-            if key == "figsize":
-                return (10, 10)
-            elif key in ["vmin"]:
-                return 0
-            elif key in ["vmax", "alpha"]:
-                return 1
-            elif key in ["colorbar"]:
-                return "binary"
-            elif key in ["histogram_range"]:
-                return [0, 1, 0.01]
-            elif key in ["discrete_colorbar"]:
-                return 100
+        plt.xlabel(column_to_plot, size=20)
+        plt.ylabel("Freq.", size=20)
+        plt.xticks(size=18)
+        plt.yticks(size=18)
+        plt.grid()
+        plt.show()
 
-    def loadPatches(
+    def load_patches(
         self,
         patch_paths: str,
+        patch_file_ext: Optional[Union[str, bool]] = False,
         parent_paths: Optional[Union[str, bool]] = False,
-        add_geo_par: Optional[bool] = False,
+        parent_file_ext: Optional[Union[str, bool]] = False,
+        add_geo_info: Optional[bool] = False,
         clear_images: Optional[bool] = False,
     ) -> None:
         """
         Loads patch images from the given paths and adds them to the ``images``
-        dictionary in the ``mapImages`` instance.
+        dictionary in the ``MapImages`` instance.
 
         Parameters
         ----------
         patch_paths : str
             The file path of the patches to be loaded.
 
             *Note: The ``patch_paths`` parameter accepts wildcards.*
+        patch_file_ext : str or bool, optional
+            The file extension of the patches to be loaded, ignored if file extensions are specified in ``patch_paths`` (e.g. with ``"./path/to/dir/*png"``)
+            By default ``False``.
         parent_paths : str or bool, optional
             The file path of the parent images to be loaded. If set to
             ``False``, no parents are loaded. Default is ``False``.
 
             *Note: The ``parent_paths`` parameter accepts wildcards.*
-        add_geo_par : bool, optional
+        parent_file_ext : str or bool, optional
+            The file extension of the parent images, ignored if file extensions are specified in ``parent_paths`` (e.g. with ``"./path/to/dir/*png"``)
+            By default ``False``.
+        add_geo_info : bool, optional
             If ``True``, adds geographic information to the parent image.
             Default is ``False``.
         clear_images : bool, optional
             If ``True``, clears the images from the ``images`` dictionary
             before loading. Default is ``False``.
 
         Returns
         -------
         None
         """
-
-        patch_paths = glob(os.path.abspath(patch_paths))
+        patch_files = self._resolve_file_path(patch_paths, patch_file_ext)
 
         if clear_images:
-            self.images = {}
-            self.images["parent"] = {}
-            self.images["child"] = {}
+            self.images = {"parent": {}, "patch": {}}
+            self.parents = {} #are these needed?
+            self.patches = {} #are these needed?
 
-        for file_path in patch_paths:
-            if not os.path.isfile(file_path):
-                print(f"[WARNING] file does not exist: {file_path}")
+        if parent_paths:
+            # Add parents
+            self.load_parents(
+                parent_paths=parent_paths,
+                parent_file_ext=parent_file_ext,
+                overwrite=False,
+                add_geo_info=add_geo_info,
+            )
+        
+        for patch_file in tqdm(patch_files):
+            if not os.path.isfile(patch_file):
+                print(f"[WARNING] File does not exist: {patch_file}")
                 continue
 
+            self._check_image_mode(patch_file)
+
             # patch ID is set to the basename
-            patch_id = os.path.basename(file_path)
+            patch_id = os.path.basename(patch_file)
 
             # Parent ID and border can be detected using patch_id
-            parent_id = self.detectParIDfromPath(patch_id)
-            min_x, min_y, max_x, max_y = self.detectBorderFromPath(patch_id)
+            try:
+                parent_id = self.detect_parent_id_from_path(patch_id)
+                pixel_bounds = self.detect_pixel_bounds_from_path(patch_id)
+            except:
+                parent_id = None
+                pixel_bounds = None
+
+            # Add patch
+            if not self.patches.get(patch_id, False):
+                self.patches[patch_id] = {}
+            self.patches[patch_id]["parent_id"] = parent_id
+            self.patches[patch_id]["image_path"] = patch_file
+            self.patches[patch_id]["pixel_bounds"] = pixel_bounds
 
-            # Add child
-            if not self.images["child"].get(patch_id, False):
-                self.images["child"][patch_id] = {}
-            self.images["child"][patch_id]["parent_id"] = parent_id
-            self.images["child"][patch_id]["image_path"] = file_path
-            self.images["child"][patch_id]["min_x"] = min_x
-            self.images["child"][patch_id]["min_y"] = min_y
-            self.images["child"][patch_id]["max_x"] = max_x
-            self.images["child"][patch_id]["max_y"] = max_y
-
-        if parent_paths:
-            # Add parents
-            self.loadParents(
-                parent_paths=parent_paths, update=False, add_geo=add_geo_par
-            )
-            # Add children to the parent
-            self.addChildren()
+            # Add patches to the parent
+            self._add_patch_to_parent(patch_id)
 
     @staticmethod
-    def detectParIDfromPath(
+    def detect_parent_id_from_path(
         image_id: Union[int, str], parent_delimiter: Optional[str] = "#"
     ) -> str:
         """
         Detect parent IDs from ``image_id``.
 
         Parameters
         ----------
         image_id : int or str
-            ID of child image.
+            ID of patch.
         parent_delimiter : str, optional
-            Delimiter used to separate parent ID when naming child image, by
+            Delimiter used to separate parent ID when naming patch, by
             default ``"#"``.
 
         Returns
         -------
         str
             Parent ID.
         """
         return image_id.split(parent_delimiter)[1]
 
     @staticmethod
-    def detectBorderFromPath(
+    def detect_pixel_bounds_from_path(
         image_id: Union[int, str],
         # border_delimiter="-" # <-- not in use in this method
     ) -> Tuple[int, int, int, int]:
         """
-        Detects borders from the path assuming child image is named using the
+        Detects borders from the path assuming patch is named using the
         following format: ``...-min_x-min_y-max_x-max_y-...``
 
         Parameters
         ----------
         image_id : int or str
             ID of image
 
         ..
             border_delimiter : str, optional
-                Delimiter used to separate border values when naming child
+                Delimiter used to separate border values when naming patch
                 image, by default ``"-"``.
 
         Returns
         -------
         tuple of min_x, min_y, max_x, max_y
             Border (min_x, min_y, max_x, max_y) of image
         """
@@ -1782,291 +1751,445 @@
         return (
             int(split_path[1]),
             int(split_path[2]),
             int(split_path[3]),
             int(split_path[4]),
         )
 
-    def loadParents(
+    def load_parents(
         self,
         parent_paths: Optional[Union[str, bool]] = False,
         parent_ids: Optional[Union[List[str], str, bool]] = False,
-        update: Optional[bool] = False,
-        add_geo: Optional[bool] = False,
+        parent_file_ext: Optional[Union[str, bool]] = False,
+        overwrite: Optional[bool] = False,
+        add_geo_info: Optional[bool] = False,
     ) -> None:
         """
         Load parent images from file paths (``parent_paths``).
 
         If ``parent_paths`` is not given, only ``parent_ids``, no image path
         will be added to the images.
 
         Parameters
         ----------
         parent_paths : str or bool, optional
             Path to parent images, by default ``False``.
         parent_ids : list, str or bool, optional
             ID(s) of parent images. Ignored if ``parent_paths`` are specified.
             By default ``False``.
-        update : bool, optional
+        parent_file_ext : str or bool, optional
+            The file extension of the parent images, ignored if file extensions are specified in ``parent_paths`` (e.g. with ``"./path/to/dir/*png"``)
+            By default ``False``.
+        overwrite : bool, optional
             If ``True``, current parents will be overwritten, by default
             ``False``.
-        add_geo : bool, optional
+        add_geo_info : bool, optional
             If ``True``, geographical info will be added to parents, by
             default ``False``.
 
         Returns
         -------
         None
         """
-
+        
         if parent_paths:
-            if not isinstance(parent_paths, list):
-                parent_paths = glob(os.path.abspath(parent_paths))
-            if update:
-                self.images["parent"] = {}
-
-            for parent_path in parent_paths:
-                parent_id = os.path.basename(parent_path)
-                self.images["parent"][parent_id] = {"parent_id": None}
-                if os.path.isfile(parent_path):
-                    self.images["parent"][parent_id][
-                        "image_path"
-                    ] = os.path.abspath(parent_path)
-                else:
-                    self.images["parent"][parent_id]["image_path"] = None
+            files = self._resolve_file_path(parent_paths, parent_file_ext)
+
+            if overwrite:
+                self.parents = {}
+
+            for file in tqdm(files):
+                if not os.path.isfile(file):
+                    print(f"[WARNING] File does not exist: {file}")
+                    continue
+
+                self._check_image_mode(file)
 
-                if add_geo:
-                    self.addGeoInfo()
+                parent_id = os.path.basename(file)
+                
+                if not self.parents.get(parent_id, False):
+                    self.parents[parent_id] = {}
+                self.parents[parent_id]["parent_id"] = None 
+                self.parents[parent_id]["image_path"] = os.path.abspath(file) if os.path.isfile(file) else None
+                if add_geo_info:
+                    self.add_geo_info()
 
         elif parent_ids:
             if not isinstance(parent_ids, list):
                 parent_ids = [parent_ids]
+            
             for parent_id in parent_ids:
-                self.images["parent"][parent_id] = {"parent_id": None}
-                self.images["parent"][parent_id]["image_path"] = None
+                if not self.parents.get(parent_id, False):
+                    self.parents[parent_id] = {}
+                self.parents[parent_id]["parent_id"] = None
+                self.parents[parent_id]["image_path"] = None
+        
+        else:
+            raise ValueError("[ERROR] Please pass one of ``parent_paths`` or ``parent_ids``.")
 
-    def loadDataframe(
+    def load_df(
         self,
-        parents: Optional[Union[pd.DataFrame, str]] = None,
-        children_df: Optional[Union[pd.DataFrame, str]] = None,
+        parent_df: Optional[pd.DataFrame] = None,
+        patch_df: Optional[pd.DataFrame] = None,
         clear_images: Optional[bool] = True,
     ) -> None:
         """
-        Form images variable from pandas DataFrame(s).
+        Create ``MapImages`` instance by loading data from pandas DataFrame(s).
 
         Parameters
         ----------
-        parents : pandas.DataFrame, str or None, optional
+        parent_df : pandas.DataFrame, optional
             DataFrame containing parents or path to parents, by default
             ``None``.
-        children_df : pandas.DataFrame or None, optional
-            DataFrame containing children (patches), by default ``None``.
+        patch_df : pandas.DataFrame, optional
+            DataFrame containing patches, by default ``None``.
         clear_images : bool, optional
             If ``True``, clear images before reading the dataframes, by
             default ``True``.
 
         Returns
         -------
         None
         """
 
         if clear_images:
-            self.images = {"parent": {}, "child": {}}
+            self.images = {"parent": {}, "patch": {}}
 
-        if not isinstance(children_df, type(None)):
-            self.images["child"] = children_df.to_dict(orient="index")
+        if isinstance(parent_df, pd.DataFrame):
+            self.parents.update(parent_df.to_dict(orient="index"))
 
-        if not isinstance(parents, type(None)):
-            if isinstance(parents, str):
-                self.loadParents(parents)
-            else:
-                self.images["parent"] = parents.to_dict(orient="index")
-
-            for parent_id in self.images["parent"].keys():
-                # Do we need this?
-                # k2change = "children"
-                # if k2change in self.images["parent"][parent_id]:
-                #    try:
-                #        self.images["parent"][parent_id][k2change] = self.images["parent"][parent_id][k2change]  # noqa
-                #    except Exception as err:
-                #        print(err)
-
-                k2change = "coord"
-                if k2change in self.images["parent"][parent_id]:
-                    try:
-                        self.images["parent"][parent_id][
-                            k2change
-                        ] = self.images["parent"][parent_id][k2change]
-                    except Exception as err:
-                        print(err)
+        if isinstance(patch_df, pd.DataFrame):
+            self.patches.update(patch_df.to_dict(orient="index"))
 
-            self.addChildren()
+        for patch_id in self.list_patches():
+            self._add_patch_to_parent(patch_id)
 
-    def load_csv_file(
+    def load_csv(
         self,
         parent_path: Optional[str] = None,
-        child_path: Optional[str] = None,
+        patch_path: Optional[str] = None,
         clear_images: Optional[bool] = False,
-        index_col_child: Optional[int] = 0,
+        index_col_patch: Optional[int] = 0,
         index_col_parent: Optional[int] = 0,
     ) -> None:
         """
-        Load CSV files containing information about parent and child images,
-        and update the ``images`` attribute of the ``mapImages`` instance with
+        Load CSV files containing information about parent and patches,
+        and update the ``images`` attribute of the ``MapImages`` instance with
         the loaded data.
 
         Parameters
         ----------
         parent_path : str, optional
             Path to the CSV file containing parent image information.
-        child_path : str, optional
-            Path to the CSV file containing child image information.
+        patch_path : str, optional
+            Path to the CSV file containing patch information.
         clear_images : bool, optional
             If True, clear all previously loaded image information before
             loading new information. Default is ``False``.
-        index_col_child : int, optional
-            Column to set as index for the child DataFrame, by default ``0``.
+        index_col_patch : int, optional
+            Column to set as index for the patch DataFrame, by default ``0``.
         index_col_parent : int, optional
             Column to set as index for the parent DataFrame, by default ``0``.
 
         Returns
         -------
         None
         """
         if clear_images:
-            self.images = {"parent": {}, "child": {}}
+            self.images = {"parent": {}, "patch": {}}
 
-        if isinstance(child_path, str) and os.path.isfile(child_path):
-            self.images["child"].update(
-                pd.read_csv(child_path, index_col=index_col_child).to_dict(
-                    orient="index"
-                )
-            )
-
-        if isinstance(parent_path, str) and os.path.isfile(parent_path):
-            self.images["parent"].update(
-                pd.read_csv(parent_path, index_col=index_col_parent).to_dict(
-                    orient="index"
-                )
-            )
+        if not isinstance(parent_path, str):
+            raise ValueError("[ERROR] Please pass ``parent_path`` as string.")
+        if not isinstance(patch_path, str):
+            raise ValueError("[ERROR] Please pass ``patch_path`` as string.")
 
-            self.addChildren()
+        if os.path.isfile(parent_path):
+            parent_df = pd.read_csv(parent_path, index_col=index_col_parent)
+        else:
+            raise ValueError(f"[ERROR] {parent_path} cannot be found.")
+                    
+        if os.path.isfile(patch_path):
+            patch_df = pd.read_csv(patch_path, index_col=index_col_patch)
+        else:
+            raise ValueError(f"[ERROR] {patch_path} cannot be found.")
 
-            for parent_id in self.images["parent"].keys():
-                k2change = "children"
-                if k2change in self.images["parent"][parent_id]:
-                    self.images["parent"][parent_id][k2change] = eval(
-                        self.images["parent"][parent_id][k2change]
-                    )
+        self.load_df(parent_df=parent_df, patch_df=patch_df, clear_images=clear_images)
 
-                k2change = "coord"
-                if k2change in self.images["parent"][parent_id]:
-                    self.images["parent"][parent_id][k2change] = eval(
-                        self.images["parent"][parent_id][k2change]
-                    )
 
-    def addGeoInfo(
+    def add_geo_info(
         self,
-        proj2convert: Optional[str] = "EPSG:4326",
-        calc_method: Optional[str] = "great-circle",
-        verbose: Optional[bool] = False,
+        target_crs: Optional[str] = "EPSG:4326",
+        verbose: Optional[bool] = True,
     ) -> None:
         """
-        Add geographic information (shape, coords, reprojected to EPSG:4326,
-        and size in meters) to the ``images`` attribute of the ``mapImages``
-        instance from image metadata.
+        Add coordinates (reprojected to EPSG:4326) to all parents images using image metadata.
 
         Parameters
         ----------
-        proj2convert : str, optional
+        target_crs : str, optional
             Projection to convert coordinates into, by default ``"EPSG:4326"``.
-        calc_method : str, optional
-            Method to use for calculating image size in meters. Possible
-            values: ``"great-circle"`` (default), ``"gc"`` (alias for
-            ``"great-circle"``), ``"geodesic"``. ``"great-circle"`` and
-            ``"gc"`` compute size using the great-circle distance formula,
-            while ``"geodesic"`` computes size using the geodesic distance
-            formula.
         verbose : bool, optional
-            Whether to print progress messages or not. The default is
-            ``False``.
+            Whether to print verbose output, by default ``True``
 
         Returns
         -------
         None
 
         Notes
         -----
+        For each image in the parents dictionary, this method calls ``_add_geo_info_id`` and coordinates (if present) to the image in the ``parent`` dictionary.
+        """
+        image_ids = list(self.parents.keys())
+
+        for image_id in image_ids:
+            self._add_geo_info_id(image_id, target_crs)
+
+    def _add_geo_info_id(
+        self,
+        image_id: str,
+        target_crs: Optional[str] = "EPSG:4326",
+        verbose: Optional[bool] = True,
+    ) -> None:
+        """
+        Add coordinates (reprojected to EPSG:4326) to an image.
+
+        Parameters
+        ----------
+        image_id : str
+            The ID of the image to add geographic information to
+        target_crs : str, optional
+            Projection to convert coordinates into, by default ``"EPSG:4326"``.
+        verbose : bool, optional
+            Whether to print verbose output, by default ``True``
+
+        Returns
+        -------
+        None
+
+        Notes
+        ------
         This method reads the image files specified in the ``image_path`` key
         of each dictionary in the ``parent`` dictionary.
 
         It then checks if the image has geographic coordinates in its metadata,
         if not it prints a warning message and skips to the next image.
 
         If coordinates are present, this method converts them to the specified
-        projection ``proj2convert`` and calculates the size of each pixel
-        based on the method specified in ``calc_method``.
+        projection ``target_crs``.
+
+        These are then added to the dictionary in the ``parent`` dictionary corresponding to each image.
+        """
+
+        image_path = self.parents[image_id]["image_path"]
 
-        The resulting information is then added to the dictionary in the
-        ``parent`` dictionary corresponding to each image.
+        # Read the image using rasterio
+        tiff_src = rasterio.open(image_path)
+
+        # Check whether coordinates are present
+        if isinstance(tiff_src.crs, type(None)):
+            self._print_if_verbose(
+                f"No coordinates found in {image_id}. Try add_metadata instead.",
+                verbose,
+            )  # noqa
+            return
+
+        else:
+            # Get coordinates as string
+            tiff_proj = tiff_src.crs.to_string()
+            # Coordinate transformation: proj1 ---> proj2
+            # tiff is "lat, lon" instead of "x, y"
+            transformer = Transformer.from_crs(tiff_proj, target_crs)
+            ymin, xmin = transformer.transform(
+                tiff_src.bounds.left, tiff_src.bounds.bottom
+            )
+            ymax, xmax = transformer.transform(
+                tiff_src.bounds.right, tiff_src.bounds.top
+            )
+            # New projected coordinates
+            coords = (xmin, ymin, xmax, ymax)
+            self.parents[image_id]["coordinates"] = coords
+            self.parents[image_id]["crs"] = target_crs
 
-        Note that the calculations are performed using the
-        ``geopy.distance.geodesic`` and ``geopy.distance.great_circle``
-        methods. Thus, the method requires the ``geopy`` package to be
-        installed.
+    @staticmethod
+    def _print_if_verbose(msg: str, verbose: bool) -> None:
+        """
+        Print message if verbose is True.
         """
-        image_ids = list(self.images["parent"].keys())
+        if verbose:
+            print(msg)
 
-        for image_id in image_ids:
-            image_path = self.images["parent"][image_id]["image_path"]
+    def _get_tree_level(self, image_id: str) -> str:
+        """Identify tree level of an image from image_id.
 
-            # Read the image using rasterio
-            tiff_src = rasterio.open(image_path)
+        Parameters
+        ----------
+        image_id : str
+            The ID of the image to identify tree level for.
 
-            # Get height and width for image
-            image_height, image_width = tiff_src.shape
+        Returns
+        -------
+        str
+            The tree level of the image.
+        """
+        tree_level = "parent" if bool(self.parents.get(image_id)) else "patch"
+        return tree_level
+    
+    def save_patches_as_geotiffs(
+        self, 
+        rewrite: Optional[bool] = False, 
+        verbose: Optional[bool] = False,
+        crs: Optional[str] = None,
+    ) -> None:
+        """Save all patches in MapImages instance as geotiffs.
 
-            # Extract channels
-            image_channels = tiff_src.count
+        Parameters
+        ----------
+        rewrite : bool, optional
+            Whether to rewrite files if they already exist, by default False
+        verbose : bool, optional
+            Whether to print verbose outputs, by default False
+        crs : str, optional
+            The CRS of the coordinates.
+            If None, the method will first look for ``crs`` in the patches dictionary and use those. If ``crs`` cannot be found in the dictionary, the method will use "EPSG:4326".
+            By default None.
+        """
 
-            # Set shape
-            shape = (image_height, image_width, image_channels)
-            self.images["parent"][image_id]["shape"] = shape
+        patches_list = self.list_patches()
+        
+        for patch_id in tqdm(patches_list):
+            self._save_patch_as_geotiff(patch_id, rewrite, verbose, crs)
 
-            # Check whether coordinates are present
-            if isinstance(tiff_src.crs, type(None)):
-                print(
-                    f"No coordinates found in {image_id}. Try add_metadata instead"  # noqa
-                )
-                continue
+    def _save_patch_as_geotiff(
+        self, 
+        patch_id: str, 
+        rewrite: Optional[bool] = False, 
+        verbose: Optional[bool] = False,
+        crs: Optional[str] = None,
+    ) -> None:
+        """Save a patch as a geotiff.
 
-            else:
-                # Get coordinates as string
-                tiff_proj = tiff_src.crs.to_string()
+        Parameters
+        ----------
+        patch_id : str
+            The ID of the patch to write.
+        rewrite : bool, optional
+            Whether to rewrite files if they already exist, by default False
+        verbose : bool, optional
+            Whether to print verbose outputs, by default False
+        crs : Optional[str], optional
+            The CRS of the coordinates.
+            If None, the method will first look for ``crs`` in the patches dictionary and use those. If ``crs`` cannot be found in the dictionary, the method will use "EPSG:4326".
+            By default None.
 
-                # Coordinate transformation: proj1 ---> proj2
-                transformer = Transformer.from_crs(tiff_proj, proj2convert)
-                ymax, xmin = transformer.transform(
-                    tiff_src.bounds.left, tiff_src.bounds.top
-                )
-                ymin, xmax = transformer.transform(
-                    tiff_src.bounds.right, tiff_src.bounds.bottom
-                )
+        Raises
+        ------
+        ValueError
+            If patch directory does not exist.
+        """
 
-                # New projected coordinates
-                coords = (xmin, xmax, ymin, ymax)
-                self.images["parent"][image_id]["coord"] = coords
-
-                # Calculate pixel size in meters
-                size_in_m = self.calc_pixel_width_height(
-                    parent_id=image_id,
-                    calc_size_in_m=calc_method,
-                    verbose=verbose,
-                )
-                self.images["parent"][image_id]["size_in_m"] = size_in_m
+        patch_path = self.patches[patch_id]["image_path"]
+        patch_dir = os.path.dirname(patch_path)
+
+        if not os.path.exists(patch_dir):
+            raise ValueError(f'[ERROR] Patch directory "{patch_dir}" does not exist.')
+        
+        patch_id_no_ext = os.path.splitext(patch_id)[0]
+        geotiff_path = f"{patch_dir}/{patch_id_no_ext}.tif"
+        
+        self.patches[patch_id]["geotiff_path"] = geotiff_path
+        
+        if os.path.isfile(f"{geotiff_path}"):
+            if not rewrite:
+                self._print_if_verbose(
+                    f'[INFO] File already exists: {geotiff_path}.', verbose
+                    )
+                return
+            
+        self._print_if_verbose(
+            f"[INFO] Creating: {geotiff_path}.",
+            verbose,
+        )
+
+        if "shape" not in self.patches[patch_id].keys():
+            self._add_shape_id(patch_id)
+        height, width, channels = self.patches[patch_id]["shape"]
+
+        if "coordinates" not in self.patches[patch_id].keys():
+            self._add_patch_coords_id(patch_id)
+        coords = self.patches[patch_id]["coordinates"]
+        
+        if not crs:
+            crs = self.patches[patch_id].get("crs", "EPSG:4326")
+
+        patch_affine = rasterio.transform.from_bounds(*coords, width, height)
+        patch = Image.open(patch_path)
+        patch_array = reshape_as_raster(patch)
+
+        with rasterio.open(
+            f"{geotiff_path}",
+            'w',
+            driver="GTiff",
+            height=patch.height,
+            width=patch.width,
+            count=channels,
+            transform=patch_affine,
+            dtype='uint8',
+            nodata=0,
+            crs=crs,
+        ) as dst:
+            dst.write(patch_array)    
+
+    def save_patches_to_geojson(
+        self, 
+        geojson_fname: Optional[str] = "patches.geojson",
+        rewrite: Optional[bool] = False, 
+        crs: Optional[str] = None,
+    ) -> None:
+        """Saves patches to a geojson file.
+
+        Parameters
+        ----------
+        geojson_fname : Optional[str], optional
+            The name of the geojson file, by default "patches.geojson"
+        rewrite : Optional[bool], optional
+            Whether to overwrite an existing file, by default False.
+        crs : Optional[str], optional
+            The CRS to use when writing the geojson.
+            If None, the method will look for "crs" in the patches dictionary and, if found, will use that. Otherwise it will set the crs to the default value of "EPSG:4326".
+            By default None
+        """
+        if os.path.isfile(geojson_fname):
+            if not rewrite:
+                print(f'[WARNING] File already exists: {geojson_fname}. Use ``rewrite=True`` to overwrite.')
+                return
+    
+        _, patch_df = self.convert_images()
+
+        if "polygon" not in patch_df.columns:
+            self.add_patch_polygons()
+            _, patch_df = self.convert_images()
+
+        if not crs:
+            if "crs" in patch_df.columns:
+                if len(patch_df["crs"].unique()) == 1:
+                    crs = patch_df["crs"].unique()[0]
+            else:
+                crs = "EPSG:4326"
+
+        patch_df.reset_index(names="image_id", inplace=True)
+        
+        #drop pixel stats columns
+        patch_df.drop(columns=patch_df.filter(like="pixel", axis=1), inplace=True)
+        #drop tuple columns - cause errors
+        for col in patch_df.columns:
+            if isinstance(patch_df[col][0], tuple):
+                patch_df.drop(columns=col, inplace=True)
+        
+        geo_patch_df = geopd.GeoDataFrame(patch_df, geometry="polygon", crs=crs)
+        geo_patch_df.to_file(geojson_fname, driver="GeoJSON")
 
     '''
     def readPatches(self,
                   patch_paths,
                   parent_paths,
                   metadata=None,
                   metadata_fmt="dataframe",
@@ -2082,16 +2205,16 @@
             clear_images {bool} -- clear images variable before reading
                     patches (default: {False})
         """
         patch_paths = glob(os.path.abspath(patch_paths))
 
         if clear_images:
             self.images = {}
-            self.images["parent"] = {}
-            self.images["child"] = {}
+            self.parents = {}
+            self.patches = {}
             # XXX check
         if not isinstance(metadata, type(None)):
             include_metadata = True
             if metadata_fmt in ["dataframe"]:
                 metadata_df = metadata
             elif metadata_fmt.lower() in ["csv"]:
                 try:
@@ -2111,46 +2234,46 @@
                 raise ValueError(f"patch_paths should point to actual files. Current patch_paths: {patch_paths}")
             # patch ID is set to the basename
             patch_id = os.path.basename(tpath)
             # XXXX
             if include_metadata and (not patch_id in list(metadata['rd_index_id'])):
                 continue
             # Parent ID and border can be detected using patch_id
-            parent_id = self.detectParIDfromPath(patch_id)
-            min_x, min_y, max_x, max_y = self.detectBorderFromPath(patch_id)
+            parent_id = self.detect_parent_id_from_path(patch_id)
+            min_x, min_y, max_x, max_y = self.detect_border_from_path(patch_id)
 
-            # Add child
-            if not self.images["child"].get(patch_id, False):
-                self.images["child"][patch_id] = {}
-            self.images["child"][patch_id]["parent_id"] = parent_id
-            self.images["child"][patch_id]["image_path"] = tpath
-            self.images["child"][patch_id]["min_x"] = min_x
-            self.images["child"][patch_id]["min_y"] = min_y
-            self.images["child"][patch_id]["max_x"] = max_x
-            self.images["child"][patch_id]["max_y"] = max_y
+            # Add patch
+            if not self.patches.get(patch_id, False):
+                self.patches[patch_id] = {}
+            self.patches[patch_id]["parent_id"] = parent_id
+            self.patches[patch_id]["image_path"] = tpath
+            self.patches[patch_id]["min_x"] = min_x
+            self.patches[patch_id]["min_y"] = min_y
+            self.patches[patch_id]["max_x"] = max_x
+            self.patches[patch_id]["max_y"] = max_y
 
         # XXX check
         if include_metadata:
             # metadata_cols = set(metadata_df.columns) - set(['rd_index_id'])
             for one_row in metadata_df.iterrows():
                 for one_col in list(metadata_cols2add):
-                    self.images["child"][one_row[1]['rd_index_id']][one_col] = one_row[1][one_col]
+                    self.patches[one_row[1]['rd_index_id']][one_col] = one_row[1][one_col]
 
         if parent_paths:
             # Add parents
             self.readParents(parent_paths=parent_paths)
-            # Add children to the parent
-            self.addChildren()
+            # Add patches to the parent
+            self._add_patch_to_parent()
 
     def process(self, tree_level="parent", update_paths=True,
                 save_preproc_dir="./test_preproc"):
         """Process images using process.py module
 
         Args:
-            tree_level (str, optional): "parent" or "child" paths will be used. Defaults to "parent".
+            tree_level (str, optional): "parent" or "patch" paths will be used. Defaults to "parent".
             update_paths (bool, optional): XXX. Defaults to True.
             save_preproc_dir (str, optional): Path to store preprocessed images. Defaults to "./test_preproc".
         """
             from mapreader import process
         # Collect paths and store them self.process_paths
         self.getProcessPaths(tree_level=tree_level)
 
@@ -2159,38 +2282,38 @@
         if update_paths:
             self.readParents(saved_paths, update=True)
 
     def getProcessPaths(self, tree_level="parent"):
         """Create a list of paths to be processed
 
         Args:
-            tree_level (str, optional): "parent" or "child" paths will be used. Defaults to "parent".
+            tree_level (str, optional): "parent" or "patch" paths will be used. Defaults to "parent".
         """
         process_paths = []
         for one_img in self.images[tree_level].keys():
             process_paths.append(self.images[tree_level][one_img]["image_path"])
         self.process_paths = process_paths
         
     def prepare4inference(self, fmt="dataframe"):
         """Convert images to the specified format (fmt)
             Keyword Arguments:
             fmt {str} -- convert images variable to this format (default: {"dataframe"})
         """
         if fmt in ["pandas", "dataframe"]:
-            children = pd.DataFrame.from_dict(self.images["child"], orient="index")
-            children.reset_index(inplace=True)
-            if len(children) > 0:
-                children.rename(columns={"image_path": "image_id"}, inplace=True)
-                children.drop(columns=["index", "parent_id"], inplace=True)
-                children["label"] = -1
+            patches = pd.DataFrame.from_dict(self.patches, orient="index")
+            patches.reset_index(inplace=True)
+            if len(patches) > 0:
+                patches.rename(columns={"image_path": "image_id"}, inplace=True)
+                patches.drop(columns=["index", "parent_id"], inplace=True)
+                patches["label"] = -1
 
-            parents = pd.DataFrame.from_dict(self.images["parent"], orient="index")
+            parents = pd.DataFrame.from_dict(self.parents, orient="index")
             parents.reset_index(inplace=True)
             if len(parents) > 0:
                 parents.rename(columns={"image_path": "image_id"}, inplace=True)
                 parents.drop(columns=["index", "parent_id"], inplace=True)
                 parents["label"] = -1
 
-            return parents, children
+            return parents, patches
         else:
             raise ValueError(f"Format {fmt} is not supported!")
     '''
```

### Comparing `mapreader-0.3.4/mapreader/loader/loader.py` & `mapreader-1.0.1.post0.dev9/mapreader/load/loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,131 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from mapreader.loader.images import mapImages
+from mapreader.load.images import MapImages
 from typing import Optional, Union, Dict
 
 
 def loader(
     path_images: Optional[str] = None,
     tree_level: Optional[str] = "parent",
     parent_path: Optional[str] = None,
-    **kwds: Dict
-) -> mapImages:
+    **kwargs: dict
+) -> MapImages:
     """
-    Creates a ``mapImages`` class to manage a collection of image paths and
+    Creates a ``MapImages`` class to manage a collection of image paths and
     construct image objects.
 
     Parameters
     ----------
     path_images : str or None, optional
         Path to the directory containing images (accepts wildcards). By
         default, ``None``
     tree_level : str, optional
         Level of the image hierarchy to construct. The value can be
-        ``"parent"`` (default) and ``"child"``.
+        ``"parent"`` (default) and ``"patch"``.
     parent_path : str, optional
         Path to parent images (if applicable), by default ``None``.
-    **kwds : dict, optional
-        Additional keyword arguments to be passed to the ``imagesConstructor``
+    **kwargs : dict, optional
+        Additional keyword arguments to be passed to the ``_images_constructor()``
         method.
 
     Returns
     -------
-    mapImages
-        The ``mapImages`` class which can manage a collection of image paths
+    MapImages
+        The ``MapImages`` class which can manage a collection of image paths
         and construct image objects.
 
     Notes
     -----
     This is a wrapper method. See the documentation of the
-    :class:`mapreader.loader.images.mapImages` class for more detail.
+    :class:`mapreader.load.images.MapImages` class for more detail.
     """
-    img = mapImages(
-        path_images=path_images,
-        tree_level=tree_level,
-        parent_path=parent_path,
-        **kwds
+    img = MapImages(
+        path_images=path_images, tree_level=tree_level, parent_path=parent_path, **kwargs
     )
     return img
 
 
 def load_patches(
     patch_paths: str,
+    patch_file_ext: Optional[Union[str, bool]] = False,
     parent_paths: Optional[Union[str, bool]] = False,
-    add_geo_par: Optional[bool] = False,
+    parent_file_ext: Optional[Union[str, bool]] = False,
+    add_geo_info: Optional[bool] = False,
     clear_images: Optional[bool] = False,
-) -> mapImages:
+) -> MapImages:
     """
-    Creates a ``mapImages`` class to manage a collection of image paths and
+    Creates a ``MapImages`` class to manage a collection of image paths and
     construct image objects. Then loads patch images from the given paths and
-    adds them to the ``images`` dictionary in the ``mapImages`` instance.
+    adds them to the ``images`` dictionary in the ``MapImages`` instance.
 
     Parameters
     ----------
     patch_paths : str
         The file path of the patches to be loaded.
 
         *Note: The ``patch_paths`` parameter accepts wildcards.*
+    patch_file_ext : str or bool, optional
+        The file extension of the patches, ignored if file extensions are specified in ``patch_paths`` (e.g. with ``"./path/to/dir/*png"``)
+        By default ``False``.
     parent_paths : str or bool, optional
         The file path of the parent images to be loaded. If set to
         ``False``, no parents are loaded. Default is ``False``.
 
         *Note: The ``parent_paths`` parameter accepts wildcards.*
-    add_geo_par : bool, optional
+    parent_file_ext : str or bool, optional
+        The file extension of the parent images, ignored if file extensions are specified in ``parent_paths`` (e.g. with ``"./path/to/dir/*png"``)
+        By default ``False``.
+    add_geo_info : bool, optional
         If ``True``, adds geographic information to the parent image.
         Default is ``False``.
     clear_images : bool, optional
         If ``True``, clears the images from the ``images`` dictionary
         before loading. Default is ``False``.
 
     Returns
     -------
-    mapImages
-        The ``mapImages`` class which can manage a collection of image paths
+    MapImages
+        The ``MapImages`` class which can manage a collection of image paths
         and construct image objects.
 
     Notes
     -----
     This is a wrapper method. See the documentation of the
-    :class:`mapreader.loader.images.mapImages` class for more detail.
+    :class:`mapreader.load.images.MapImages` class for more detail.
 
     This function in particular, also calls the
-    :meth:`mapreader.loader.images.mapImages.loadPatches` method. Please see
+    :meth:`mapreader.load.images.MapImages.loadPatches` method. Please see
     the documentation for that method for more information as well.
     """
-    img = mapImages()
-    img.loadPatches(
+    img = MapImages()
+    img.load_patches(
         patch_paths=patch_paths,
+        patch_file_ext=patch_file_ext,
         parent_paths=parent_paths,
-        add_geo_par=add_geo_par,
+        parent_file_ext=parent_file_ext,
+        add_geo_info=add_geo_info,
         clear_images=clear_images,
     )
     return img
 
 
 '''
 def read_patches(patch_paths, parent_paths, metadata=None,
                metadata_fmt="dataframe", metadata_cols2add=[], metadata_index_column="image_id",  # noqa
                clear_images=False):
-    """Construct mapImages object by calling readPatches method
+    """Construct MapImages object by calling readPatches method
        This method reads patches from files (patch_paths) and add parents if parent_paths is provided  # noqa
 
     Arguments:
         patch_paths {str, wildcard accepted} -- path to patches
         parent_paths {False or str, wildcard accepted} -- path to parents
         metadata_path -- path to metadata
         metadata_fmt -- format of the metadata file (default: csv)
         metadata_index_column -- column to be used as index
         clear_images {bool} -- clear images variable before reading patches (default: {False})  # noqa
     """
-    img = mapImages()
+    img = MapImages()
     img.readPatches(patch_paths, parent_paths, metadata, metadata_fmt, metadata_cols2add, metadata_index_column, clear_images)  # noqa
     return img
 '''
```

### Comparing `mapreader-0.3.4/mapreader/process/process.py` & `mapreader-1.0.1.post0.dev9/mapreader/process/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,15 @@
 
     # make sure that the file is resampled correctly before proceeding to the
     # next step
     resampled = False
     try:
         gdal_exec = distutils.spawn.find_executable("gdal_translate")
         if not gdal_exec:
-            err_msg = (
-                "gdal_translate could not be found. Refer to https://gdal.org/"
-            )
+            err_msg = "gdal_translate could not be found. Refer to https://gdal.org/"
             raise ImportError(err_msg)
 
         # Run gdal using subprocess, in our experiments, this was faster than
         # using the library
         gdal_command = f"{gdal_exec} -of GTiff -strict -outsize {resize_percent}% {resize_percent}% {path2save_crop} {path2save_resample}"  # noqa
         # gdalwarp -t_srs EPSG:3857 -crop_to_cutline -overwrite 126517601.27.tif ./preproc/resize_126517601.27.tif # noqa
         subprocess.run(gdal_command, shell=True)
```

### Comparing `mapreader-0.3.4/mapreader/train/classifier.py` & `mapreader-1.0.1.post0.dev9/mapreader/classify/classifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,391 +1,292 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import copy
-import joblib
-import matplotlib.pyplot as plt
-import numpy as np
 import os
 import random
 import socket
 import sys
 import time
-
 from datetime import datetime
-from typing import Union, List, Optional, Tuple, Dict, Any, Hashable
-
-from sklearn.metrics import precision_recall_fscore_support
-from sklearn.metrics import roc_auc_score
+from typing import Any, Dict, Hashable, Iterable, List, Optional, Tuple, Union
 
+import joblib
+import matplotlib.pyplot as plt
+import numpy as np
 import torch
-from torch import optim
 import torch.nn as nn
-
-from torch.utils.data import DataLoader
-
 import torchvision
+from sklearn.metrics import precision_recall_fscore_support, roc_auc_score
+from torch import optim
+from torch.utils.data import DataLoader, Sampler
+from torchinfo import summary
 from torchvision import models
 
+from .datasets import PatchDataset
+
 # import pickle
 # from tqdm.autonotebook import tqdm
 # from torch.nn.modules.module import _addindent
 
 
-class classifier:
-    def __init__(self, device: Optional[str] = "default"):
+class ClassifierContainer:
+    def __init__(
+        self,
+        model: Union[str, nn.Module, None],
+        dataloaders: Union[Dict[str, DataLoader], None],
+        labels_map: Union[Dict[int, str], None],
+        device: Optional[str] = "default",
+        input_size: Optional[int] = (224, 224),
+        is_inception: Optional[bool] = False,
+        load_path: Optional[str] = None,
+        force_device: Optional[bool] = False,
+        **kwargs,
+    ):
         """
-        Initialize a classifier object.
+        Initialize an ClassifierContainer object.
 
         Parameters
         ----------
+        model : str, nn.Module or None
+            The PyTorch model to add to the object.
+
+            - If passed as a string, will run ``_initialize_model(model, **kwargs)``\. See https://pytorch.org/vision/0.8/models.html for options.
+            - Must be ``None`` if ``load_path`` is specified as model will be loaded from file.
+
+        dataloaders: Dict or None
+            A dictionary containing set names as keys and dataloaders as values (i.e. set_name: dataloader).
+            Can only be ``None`` if ``load_path`` is specified as dataloaders will be loaded from file.
+        labels_map: Dict or None
+            A dictionary containing the mapping of each label index to its label, with indices as keys and labels as values (i.e. idx: label).
+            Can only be ``None`` if ``load_path`` is specified as labels_map will be loaded from file.
         device : str, optional
-            The device to be used for training and storing models. Can be set
-            to ``"default"``, ``"cpu"``, ``"cuda:0"``, etc. By default
-            ``"default"``.
+            The device to be used for training and storing models.
+            Can be set to "default", "cpu", "cuda:0", etc. By default, "default".
+        input_size : int, optional
+            The expected input size of the model. Default is ``(224,224)``\.
+        is_inception : bool, optional
+            Whether the model is an Inception-style model.
+            Default is ``False``\.
+        load_path : str, optional
+            The path to an ``\.obj`` file containing a
+        force_device : bool, optional
+            Whether to force the use of a specific device.
+            If set to ``True``\, the default device is used.
+            Defaults to ``False``\.
+        kwargs : Dict
+            Keyword arguments to pass to the ``_initialize_model()`` method (if passing ``model`` as a string).
 
         Attributes
         ----------
         device : torch.device
             The device being used for training and storing models.
-        dataloader : dict
+        dataloaders : dict
             A dictionary to store dataloaders for the model.
+        labels_map : dict
+            A dictionary mapping label indices to their labels.
         dataset_sizes : dict
             A dictionary to store sizes of datasets for the model.
-        class_names : None or list of str
-            A list of class names for the model.
-        model : None or torch.nn.Module
-            The model being trained.
-        optimizer : None or torch.optim.Optimizer
-            The optimizer being used for training the model.
-        scheduler : None or torch.optim.lr_scheduler._LRScheduler
-            The learning rate scheduler being used for training the model.
+        model : torch.nn.Module
+            The model.
         input_size : None or tuple of int
             The size of the input to the model.
         is_inception : None or bool
             A flag indicating if the model is an Inception model.
+        optimizer : None or torch.optim.Optimizer
+            The optimizer being used for training the model.
+        scheduler : None or torch.optim.lr_scheduler._LRScheduler
+            The learning rate scheduler being used for training the model.
+        criterion : None or nn.modules.loss._Loss
+            The criterion to use for training the model.
         metrics : dict
             A dictionary to store the metrics computed during training.
         last_epoch : int
             The last epoch number completed during training.
         best_loss : torch.Tensor
             The best validation loss achieved during training.
         best_epoch : int
             The epoch in which the best validation loss was achieved during
             training.
         tmp_save_filename : str
             A temporary file name to save checkpoints during training and
             validation.
         """
 
+        # set up device
         if device in ["default", None]:
-            self.device = torch.device(
-                "cuda:0" if torch.cuda.is_available() else "cpu"
-            )
+            self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
         else:
             self.device = device
         print(f"[INFO] Device is set to {self.device}")
 
-        self.dataloader = {}
-        self.dataset_sizes = {}
-        self.class_names = None
-        self.model = None
-        self.optimizer = None
-        self.scheduler = None
-        self.input_size = None
-        self.is_inception = None
-        self.metrics = {}
-        self.last_epoch = 0
-        self.best_loss = torch.tensor(np.inf)
-        self.best_epoch = 0
-        # temp file to save checkpoints during training/validation
-        self.tmp_save_filename = (
-            f"tmp_{random.randint(0, 1e10)}_checkpoint.pkl"
-        )
-
-        # add colors for printing/logging
-        self._print_colors()
-
-    def set_classnames(self, classname_dict: dict) -> None:
-        """
-        Set the class names and the number of classes in the object detection
-        model.
-
-        Parameters
-        ----------
-        classname_dict : dict
-            A dictionary containing the class IDs (as keys) and their
-            corresponding names (as values). E.g.
-            ``{0: "rail space", 1: "No rail space"}``
-
-        Returns
-        -------
-        None
-        """
-        self.class_names = classname_dict
-        self.num_classes = len(self.class_names)
-
-    def add2dataloader(
-        self,
-        dataset: torch.utils.data.Dataset,
-        set_name: Optional[Union[str, None]] = None,
-        batch_size: Optional[int] = 16,
-        shuffle: Optional[bool] = True,
-        num_workers: Optional[int] = 0,
-        **kwds,
-    ) -> torch.utils.data.DataLoader:
-        """
-        Adds a PyTorch dataloader to the object's ``dataloader`` dictionary
-        property and returns it.
-
-        Parameters
-        ----------
-        dataset : torch.utils.data.Dataset
-            The PyTorch dataset to use for the dataloader.
-        set_name : str or None, optional
-            The name to use when adding the dataloader to the object's
-            ``dataloader`` dictionary property (e.g., ``"train"``, ``"val"``
-            or ``"test"``).
-
-            If ``None`` (default), the dataloader is returned without being
-            added to the dictionary.
-        batch_size : int, optional
-            The batch size to use for the dataloader. Default is ``16``.
-        shuffle : bool, optional
-            Whether to shuffle the dataset during training. Default is
-            ``True``.
-        num_workers : int, optional
-            The number of worker threads to use for loading data. Default is
-            ``0``.
-        **kwds :
-            Additional keyword arguments to pass to PyTorch's ``DataLoader``
-            constructor.
-
-        Returns
-        -------
-        dl : torch.utils.data.DataLoader
-            The dataloader that was created.
-        """
-
-        dl = DataLoader(
-            dataset,
-            batch_size=batch_size,
-            shuffle=shuffle,
-            num_workers=num_workers,
-            **kwds,
-        )
-
-        if set_name is None:
-            return dl
-        else:
-            self.dataloader[set_name] = dl
-            self.dataset_sizes[set_name] = len(
-                self.dataloader[set_name].dataset
+        # check if loading an pre-existing object
+        if model and load_path:
+            raise ValueError(
+                "[ERROR] ``model`` and ``load_path`` cannot be used together - please set one to ``None``\."
             )
-            print(
-                f"[INFO] added '{set_name}' dataloader with {self.dataset_sizes[set_name]} elements."  # noqa
+        if (
+            any(val is None for val in [model, dataloaders, labels_map])
+            and not load_path
+        ):
+            raise ValueError(
+                "[ERROR] Unless passing ``load_path``\, ``model``\, ``dataloaders`` and ``labels_map`` must be defined."
             )
 
-    def print_classes_dl(self, set_name: Optional[str] = "train"):
-        """
-        Prints information about the labels and class names (if available)
-        associated with a dataloader.
+        if load_path:
+            self.load(load_path=load_path, force_device=force_device)
 
-        Parameters
-        ----------
-        set_name : str, optional
-            The name of the dataloader to print information about, normally
-            specified in ``self.add2dataloader``. Default is ``"train"``.
-
-        Returns
-        -------
-        None
-        """
-        print(
-            f"[INFO] labels:   {self.dataloader[set_name].dataset.uniq_labels}"
-        )
-        if self.class_names is not None:
-            print(f"[INFO] class-names: {self.class_names}")
-
-    def add_model(
-        self,
-        model: nn.Module,
-        input_size: Optional[int] = 224,
-        is_inception: Optional[bool] = False,
-    ) -> None:
-        """
-        Add a PyTorch model to the classifier object.
+        # add dataloaders
+        if dataloaders:
+            self.dataloaders = dataloaders
+            for set_name, dataloader in dataloaders.items():
+                print(
+                    f'[INFO] Loaded "{set_name}" with {len(dataloader.dataset)} items.'
+                )
 
-        Parameters
-        ----------
-        model : nn.Module
-            The PyTorch model to add to the object. See: ``torchvision.models``
-        input_size : int, optional
-            The expected input size of the model. Default is ``224``.
-        is_inception : bool, optional
-            Whether the model is an Inception-style model. Default is
-            ``False``.
+        if labels_map:
+            self.labels_map = labels_map
 
-        Raises
-        ------
-        ValueError
-            If the object's ``class_names`` attribute is ``None``. They should
-            be specified with the ``set_classnames`` method.
+        if model:
+            print("[INFO] Initializing model.")
 
-        Returns
-        -------
-        None
-        """
-        if self.class_names is None:
-            raise ValueError(
-                "[ERROR] specify class names using set_classnames method."
+            # set up model and move to device
+            if isinstance(model, nn.Module):
+                self.model = model.to(self.device)
+                self.input_size = input_size
+                self.is_inception = is_inception
+            elif isinstance(model, str):
+                self._initialize_model(model, **kwargs)
+
+            self.optimizer = None
+            self.scheduler = None
+            self.criterion = None
+
+            self.metrics = {}
+            self.last_epoch = 0
+            self.best_loss = torch.tensor(np.inf)
+            self.best_epoch = 0
+
+            # temp file to save checkpoints during training/validation
+            if not os.path.exists("./tmp_checkpoints"):
+                os.makedirs("./tmp_checkpoints")
+            self.tmp_save_filename = (
+                f"./tmp_checkpoints/tmp_{random.randint(0, 1e10)}_checkpoint.pkl"
             )
-        else:
-            self.print_classes_dl()
 
-        self.model = model.to(self.device)
-        self.input_size = input_size
-        self.is_inception = is_inception
+            # add colors for printing/logging
+            self._print_colors()
 
-    def del_model(self) -> None:
-        """
-        Deletes the PyTorch model from the classifier object.
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        None
-
-        Notes
-        -----
-        This function deletes the PyTorch model from the object and resets any
-        associated metadata, such as the expected input size and whether the
-        model is an Inception-style model. It also resets any associated
-        metrics and best epoch/loss values.
-        """
-        self.model = None
-        self.input_size = None
-        self.is_inception = None
-        self.metrics = {}
-        self.last_epoch = 0
-        self.best_loss = torch.tensor(np.inf)
-        self.best_epoch = 0
-
-    def layerwise_lr(
+    def generate_layerwise_lrs(
         self,
         min_lr: float,
         max_lr: float,
-        ltype: Optional[str] = "linspace",
+        spacing: Optional[str] = "linspace",
     ) -> List[Dict]:
         """
         Calculates layer-wise learning rates for a given set of model
         parameters.
 
         Parameters
         ----------
         min_lr : float
             The minimum learning rate to be used.
         max_lr : float
             The maximum learning rate to be used.
-        ltype : str, optional
+        spacing : str, optional
             The type of sequence to use for spacing the specified interval
-            learning rates. Can be either ``"linspace"`` or ``"geomspace"``,
+            learning rates. Can be either ``"linspace"`` or ``"geomspace"``\,
             where `"linspace"` uses evenly spaced learning rates over a
             specified interval and `"geomspace"` uses learning rates spaced
-            evenly on a log scale (a geometric progression). Defaults to
-            ``"linspace"``.
+            evenly on a log scale (a geometric progression). By default ``"linspace"``\.
 
         Returns
         -------
         list of dicts
             A list of dictionaries containing the parameters and learning
             rates for each layer.
         """
-        if ltype.lower() in ["line", "linear", "linspace"]:
-            list_lrs = np.linspace(
-                min_lr, max_lr, len(list(self.model.named_parameters()))
-            )
-        elif ltype.lower() in ["log", "geomspace"]:
-            list_lrs = np.geomspace(
-                min_lr, max_lr, len(list(self.model.named_parameters()))
-            )
+        if spacing.lower() == "linspace":
+            lrs = np.linspace(min_lr, max_lr, len(list(self.model.named_parameters())))
+        elif spacing.lower() in ["log", "geomspace"]:
+            lrs = np.geomspace(min_lr, max_lr, len(list(self.model.named_parameters())))
         else:
             raise NotImplementedError(
-                "Implemented methods are: linspace and geomspace"
+                '[ERROR] ``spacing`` must be one of "linspace" or "geomspace"'
             )
 
-        list2optim = []
-        for i, (name, params) in enumerate(self.model.named_parameters()):
-            list2optim.append({"params": params, "lr": list_lrs[i]})
+        params2optimise = [
+            {"params": params, "learning rate": lrs[i]}
+            for i, (_, params) in enumerate(self.model.named_parameters())
+        ]
 
-        return list2optim
+        return params2optimise
 
     def initialize_optimizer(
         self,
         optim_type: Optional[str] = "adam",
-        params2optim: Optional[str] = "infer",
+        params2optimise: Optional[Union[str, Iterable]] = "infer",
         optim_param_dict: Optional[dict] = {"lr": 1e-3},
         add_optim: Optional[bool] = True,
     ) -> Union[torch.optim.Optimizer, None]:
         """
         Initializes an optimizer for the model and adds it to the classifier
         object.
 
         Parameters
         ----------
         optim_type : str, optional
             The type of optimizer to use. Can be set to ``"adam"`` (default),
-            ``"adamw"``, or ``"sgd"``.
-        params2optim : str or iterable, optional
-            The parameters to optimize. If set to ``"infer"``, all model
+            ``"adamw"``\, or ``"sgd"``\.
+        params2optimise : str or iterable, optional
+            The parameters to optimize. If set to ``"infer"``\, all model
             parameters that require gradients will be optimized, by default
-            ``"infer"``.
+            ``"infer"``\.
         optim_param_dict : dict, optional
             The parameters to pass to the optimizer constructor as a
-            dictionary, by default ``{"lr": 1e-3}``.
+            dictionary, by default ``{"lr": 1e-3}``\.
         add_optim : bool, optional
-            If ``True``, adds the optimizer to the classifier object, by
-            default ``True``.
+            If ``True``\, adds the optimizer to the classifier object, by
+            default ``True``\.
 
         Returns
         -------
         optimizer : torch.optim.Optimizer
             The initialized optimizer. Only returned if ``add_optim`` is set to
-            ``False``.
+            ``False``\.
 
         Notes
         -----
         If ``add_optim`` is True, the optimizer will be added to object.
 
         Note that the first argument of an optimizer is parameters to optimize,
         e.g. ``params2optimize = model_ft.parameters()``:
 
-        - ``model_ft.parameters()``: all parameters are being optimized
-        - ``model_ft.fc.parameters()``: only parameters of final layer are being optimized
+        - ``model_ft.parameters()``\: all parameters are being optimized
+        - ``model_ft.fc.parameters()``\: only parameters of final layer are being optimized
 
         Here, we use:
 
         .. code-block:: python
 
             filter(lambda p: p.requires_grad, self.model.parameters())
         """
-        if params2optim == "infer":
-            params2optim = filter(
-                lambda p: p.requires_grad, self.model.parameters()
-            )
+        if params2optimise == "infer":
+            params2optimise = filter(lambda p: p.requires_grad, self.model.parameters())
 
         if optim_type.lower() in ["adam"]:
-            optimizer = optim.Adam(params2optim, **optim_param_dict)
+            optimizer = optim.Adam(params2optimise, **optim_param_dict)
         elif optim_type.lower() in ["adamw"]:
-            optimizer = optim.AdamW(params2optim, **optim_param_dict)
+            optimizer = optim.AdamW(params2optimise, **optim_param_dict)
         elif optim_type.lower() in ["sgd"]:
-            optimizer = optim.SGD(params2optim, **optim_param_dict)
+            optimizer = optim.SGD(params2optimise, **optim_param_dict)
+        else:
+            raise NotImplementedError(
+                '[ERROR] At present, only Adam ("adam"), AdamW ("adamw") and SGD ("sgd") are options for ``optim_type``\.'
+            )
 
         if add_optim:
             self.add_optimizer(optimizer)
         else:
             return optimizer
 
     def add_optimizer(self, optimizer: torch.optim.Optimizer) -> None:
@@ -413,54 +314,59 @@
         Initializes a learning rate scheduler for the optimizer and adds it to
         the classifier object.
 
         Parameters
         ----------
         scheduler_type : str, optional
             The type of learning rate scheduler to use. Can be either
-            ``"steplr"`` (default) or ``"onecyclelr"``.
+            ``"steplr"`` (default) or ``"onecyclelr"``\.
         scheduler_param_dict : dict, optional
             The parameters to pass to the scheduler constructor, by default
-            ``{"step_size": 10, "gamma": 0.1}``.
+            ``{"step_size": 10, "gamma": 0.1}``\.
         add_scheduler : bool, optional
-            If ``True``, adds the scheduler to the classifier object, by
-            default ``True``.
+            If ``True``\, adds the scheduler to the classifier object, by
+            default ``True``\.
 
         Raises
         ------
         ValueError
             If the specified ``scheduler_type`` is not implemented.
 
         Returns
         -------
         scheduler : torch.optim.lr_scheduler._LRScheduler
             The initialized learning rate scheduler. Only returned if
             ``add_scheduler`` is set to False.
         """
-        if scheduler_type.lower() in ["steplr"]:
+        if self.optimizer is None:
+            raise ValueError(
+                "[ERROR] Optimizer is not yet defined. \n\n\
+Use ``initialize_optimizer`` or ``add_optimizer`` to define one."  # noqa
+            )
+
+        if scheduler_type.lower() == "steplr":
             scheduler = optim.lr_scheduler.StepLR(
                 self.optimizer, **scheduler_param_dict
             )
-        elif scheduler_type.lower() in ["onecyclelr"]:
+        elif scheduler_type.lower() == "onecyclelr":
             scheduler = optim.lr_scheduler.OneCycleLR(
-                self.optimizer, **scheduler_param_dict
+                self.optimizer,
+                **scheduler_param_dict,  # TODO: RW - Cannot use this with default scheduler_param_dict - need to update
             )
         else:
             raise NotImplementedError(
-                f"[ERROR] scheduler of type: {scheduler_type} is not implemented."  # noqa
+                f'[ERROR] At present, ``scheduler_type`` can only be "steplr" or "onecyclelr". Not {scheduler_type}.'  # noqa
             )
 
         if add_scheduler:
             self.add_scheduler(scheduler)
         else:
             return scheduler
 
-    def add_scheduler(
-        self, scheduler: torch.optim.lr_scheduler._LRScheduler
-    ) -> None:
+    def add_scheduler(self, scheduler: torch.optim.lr_scheduler._LRScheduler) -> None:
         """
         Add a scheduler to the classifier object.
 
         Parameters
         ----------
         scheduler : torch.optim.lr_scheduler._LRScheduler
             The scheduler to add to the classifier object.
@@ -473,47 +379,90 @@
 
         Returns
         -------
         None
         """
         if self.optimizer is None:
             raise ValueError(
-                "[ERROR] optimizer is needed. Use initialize_optimizer or add_optimizer"  # noqa
+                "[ERROR] Optimizer is needed. Use initialize_optimizer or add_optimizer"  # noqa
             )
 
         self.scheduler = scheduler
 
-    def add_criterion(self, criterion: torch.nn.modules.loss._Loss) -> None:
+    def add_criterion(
+        self, criterion: Optional[Union[str, nn.modules.loss._Loss]] = "cross entropy"
+    ) -> None:
         """
         Add a loss criterion to the classifier object.
 
         Parameters
         ----------
-        criterion : torch.nn.modules.loss._Loss
+        criterion : str or torch.nn.modules.loss._Loss
             The loss criterion to add to the classifier object.
+            Accepted string values are "cross entropy" or "ce" (cross-entropy), "bce" (binary cross-entropy) and "mse" (mean squared error).
 
         Returns
         -------
         None
             The function only modifies the ``criterion`` attribute of the
             classifier and does not return anything.
         """
+        if isinstance(criterion, str):
+            if criterion in ["cross entropy", "ce", "cross_entropy", "cross-entropy"]:
+                criterion = nn.CrossEntropyLoss()
+            elif criterion in [
+                "bce",
+                "binary_cross_entropy",
+                "binary cross entropy",
+                "binary cross-entropy",
+            ]:
+                criterion = nn.BCELoss()
+            elif criterion in [
+                "mse",
+                "mean_square_error",
+                "mean_squared_error",
+                "mean squared error",
+            ]:
+                criterion = nn.MSELoss()
+            else:
+                raise NotImplementedError(
+                    '[ERROR] At present, if passing ``criterion`` as a string, criterion can only be "cross entropy" or "ce" (cross-entropy), "bce" (binary cross-entropy) or "mse" (mean squared error).'
+                )
+
+            print(f'[INFO] Using "{criterion}" as criterion.')
+
+        elif not isinstance(criterion, nn.modules.loss._Loss):
+            raise ValueError(
+                '[ERROR] Please pass ``criterion`` as a string ("cross entropy", "bce" or "mse") or torch.nn loss function (see https://pytorch.org/docs/stable/nn.html).'
+            )
+
         self.criterion = criterion
 
     def model_summary(
         self,
-        only_trainable: Optional[bool] = False,
-        print_space: Optional[List[int]] = [40, 20, 20],
+        input_size: Optional[Union[tuple, list]] = None,
+        trainable_col: Optional[bool] = False,
+        **kwargs,
     ) -> None:
         """
-        Print a summary of the model including the modules, the number of
-        parameters in each module, and the dimension of the output tensor of
-        each module. If ``only_trainable`` is ``True``, it only prints the
-        trainable parameters.
+        Print a summary of the model.
+
+        Parameters
+        ----------
+        input_size : tuple or list, optional
+            The size of the input data.
+            If None, input size is taken from "train" dataloader (``self.dataloaders["train"]``\).
+        trainable_col : bool, optional
+            If ``True``\, adds a column showing which parameters are trainable.
+            Defaults to ``False``\.
+        **kwargs : Dict
+            Keyword arguments to pass to ``torchinfo.summary()`` (see https://github.com/TylerYep/torchinfo).
 
+        Notes
+        -----
         Other ways to check params:
 
         .. code-block:: python
 
             sum(p.numel() for p in myclassifier.model.parameters())
 
         .. code-block:: python
@@ -524,104 +473,43 @@
         And:
 
         .. code-block:: python
 
             for name, param in self.model.named_parameters():
                 n = name.split(".")[0].split("_")[0]
                 print(name, param.requires_grad)
-
-        Parameters
-        ----------
-        only_trainable : bool, optional
-            If ``True``, only the trainable parameters will be printed.
-            Defaults to ``False``.
-        print_space : list, optional
-            A list with three integers defining the width of each column in
-            the printed table. By default, ``[40, 20, 20]``.
-
-        Returns
-        -------
-        None
-
-        Notes
-        -----
-        Credit: this function is the modified version of
-        https://stackoverflow.com/a/62508086.
         """
+        if not input_size:
+            batch_size = self.dataloaders["train"].batch_size
+            channels = len(self.dataloaders["train"].dataset.image_mode)
+            input_size = (batch_size, channels, *self.input_size)
 
-        if self.model is None:
-            raise ValueError("[ERROR] no model is added. Use .add_model")
-
-        # header
-        col1, col2, col3 = "modules", "parameters", "dim"
-        line_divider = sum(print_space) * "-" + "----------"
-        print(line_divider)
-        print(
-            f"| {col1:>{print_space[0]}} | {col2:>{print_space[1]}} | {col3:>{print_space[2]}}"  # noqa
-        )
-        print(line_divider)
-
-        # body
-        total_params = 0
-        total_trainable_params = 0
-        for name, parameter in self.model.named_parameters():
-            if (not parameter.requires_grad) and only_trainable:
-                continue
-            elif not parameter.requires_grad:
-                cbeg, cend = self.color_red, self.color_reset
-            else:
-                cbeg = cend = ""
-
-            param = parameter.numel()
-
-            print(
-                f"{cbeg}| {name:>{print_space[0]}} | {param:>{print_space[1]}} | {str(list(parameter.shape)):>{print_space[2]}} |{cend}"  # noqa
-            )
-
-            total_params += param
-            if parameter.requires_grad:
-                total_trainable_params += param
-
-        # footer
-        print(line_divider)
-        if not only_trainable:
-            print(
-                f"| {'Total params':>{print_space[0]}} | {total_params:>{print_space[1]}} | {'':>{print_space[2]}} |"  # noqa
-            )
-        print(
-            f"| {'Total trainable params':>{print_space[0]}} | {total_trainable_params:>{print_space[1]}} | {'':>{print_space[2]}} |"  # noqa
-        )
-        print(line_divider)
+        if trainable_col:
+            col_names = ["num_params", "output_size", "trainable"]
+        else:
+            col_names = ["output_size", "output_size", "num_params"]
 
-        # add 6 to sum(print_space) as we have two times: " | " with size 3 in
-        # the other/above prints
-        print(f"| {'Other parameters:':<{sum(print_space) + 6}} |")
-        print(
-            f"| {'* input size:   '+str(self.input_size):<{sum(print_space) + 6}} |"  # noqa
+        model_summary = summary(
+            self.model, input_size=input_size, col_names=col_names, **kwargs
         )
-        print(
-            f"| {'* is_inception: '+str(self.is_inception):<{sum(print_space) + 6}} |"  # noqa
-        )
-        print(line_divider)
+        print(model_summary)
 
-    def freeze_layers(
-        self, layers_to_freeze: Optional[List[str]] = []
-    ) -> None:
+    def freeze_layers(self, layers_to_freeze: Optional[List[str]] = []) -> None:
         """
         Freezes the specified layers in the neural network by setting
         ``requires_grad`` attribute to False for their parameters.
 
         Parameters
         ----------
         layers_to_freeze : list of str, optional
             List of names of the layers to freeze. If a layer name ends with
             an asterisk (``"*"``), then all parameters whose name contains the
             layer name (excluding the asterisk) are frozen. Otherwise,
             only the parameters with an exact match to the layer name
-            are frozen. By default, ``[]``.
+            are frozen. By default, ``[]``\.
 
         Returns
         -------
         None
             The function only modifies the ``requires_grad`` attribute of the
             specified parameters and does not return anything.
 
@@ -645,15 +533,15 @@
         Parameters
         ----------
         layers_to_unfreeze : list of str, optional
             List of names of the layers to unfreeze. If a layer name ends with
             an asterisk (``"*"``), then all parameters whose name contains the
             layer name (excluding the asterisk) are unfrozen. Otherwise,
             only the parameters with an exact match to the layer name
-            are unfrozen. By default, ``[]``.
+            are unfrozen. By default, ``[]``\.
 
         Returns
         -------
         None
             The function only modifies the ``requires_grad`` attribute of the
             specified parameters and does not return anything.
 
@@ -665,26 +553,24 @@
         for layer in layers_to_unfreeze:
             for name, param in self.model.named_parameters():
                 if (layer[-1] == "*") and (layer.replace("*", "") in name):
                     param.requires_grad = True
                 elif (layer[-1] != "*") and (layer == name):
                     param.requires_grad = True
 
-    def only_keep_layers(
-        self, only_keep_layers_list: Optional[List[str]] = []
-    ) -> None:
+    def only_keep_layers(self, only_keep_layers_list: Optional[List[str]] = []) -> None:
         """
         Only keep the specified layers (``only_keep_layers_list``) for
         gradient computation during the backpropagation.
 
         Parameters
         ----------
         only_keep_layers_list : list, optional
             List of layer names to keep. All other layers will have their
-            gradient computation turned off. Default is ``[]``.
+            gradient computation turned off. Default is ``[]``\.
 
         Returns
         -------
         None
             The function only modifies the ``requires_grad`` attribute of the
             specified parameters and does not return anything.
         """
@@ -693,29 +579,29 @@
                 param.requires_grad = True
             else:
                 param.requires_grad = False
 
     def inference(
         self,
         set_name: Optional[str] = "infer",
-        verbosity_level: Optional[int] = 0,
+        verbose: Optional[bool] = False,
         print_info_batch_freq: Optional[int] = 5,
     ):
         """
         Run inference on a specified dataset (``set_name``).
 
         Parameters
         ----------
         set_name : str, optional
             The name of the dataset to run inference on, by default
-            ``"infer"``.
-        verbosity_level : int, optional
-            The verbosity level of the output messages, by default ``0``.
+            ``"infer"``\.
+        verbose : bool, optional
+           Whether to print verbose outputs, by default False.
         print_info_batch_freq : int, optional
-            The frequency of printouts, by default ``5``.
+            The frequency of printouts, by default ``5``\.
 
         Returns
         -------
         None
 
         Notes
         -----
@@ -724,15 +610,15 @@
         ``num_epochs`` set to ``1`` and all the other parameters specified in
         the function arguments.
         """
         self.train(
             phases=[set_name],
             num_epochs=1,
             save_model_dir=None,
-            verbosity_level=verbosity_level,
+            verbose=verbose,
             tensorboard_path=None,
             tmp_file_save_freq=2,
             remove_after_load=False,
             print_info_batch_freq=print_info_batch_freq,
         )
 
     def train_component_summary(self) -> None:
@@ -756,15 +642,15 @@
         self.model_summary(only_trainable=True)
 
     def train(
         self,
         phases: Optional[List[str]] = ["train", "val"],
         num_epochs: Optional[int] = 25,
         save_model_dir: Optional[Union[str, None]] = "models",
-        verbosity_level: Optional[int] = 1,
+        verbose: Optional[bool] = False,
         tensorboard_path: Optional[Union[str, None]] = None,
         tmp_file_save_freq: Optional[Union[int, None]] = 2,
         remove_after_load: Optional[bool] = True,
         print_info_batch_freq: Optional[Union[int, None]] = 5,
     ) -> None:
         """
         Train the model on the specified phases for a given number of epochs.
@@ -773,381 +659,384 @@
         :meth:`mapreader.train.classifier.classifier.train_core` method to
         capture exceptions (``KeyboardInterrupt`` is the only supported
         exception currently).
 
         Parameters
         ----------
         phases : list of str, optional
-            The phases to train the model on for each epoch. Default is
-            ``["train", "val"]``.
+            The phases to run through during each training iteration. Default is
+            ``["train", "val"]``\.
         num_epochs : int, optional
-            The number of epochs to train the model for. Default is ``25``.
+            The number of epochs to train the model for. Default is ``25``\.
         save_model_dir : str or None, optional
-            The directory to save the model in. Default is ``"models"``. If
-            set to ``None``, the model is not saved.
-        verbosity_level : int, optional
-            The level of verbosity during training:
-
-            - ``0`` is silent,
-            - ``1`` is progress bar and metrics,
-            - ``2`` is detailed information.
-
-            Default is ``1``.
+            The directory to save the model in. Default is ``"models"``\. If
+            set to ``None``\, the model is not saved.
+        verbose : int, optional
+            Whether to print verbose outputs, by default ``False``\.
         tensorboard_path : str or None, optional
             The path to the directory to save TensorBoard logs in. If set to
-            ``None``, no TensorBoard logs are saved. Default is ``None``.
+            ``None``\, no TensorBoard logs are saved. Default is ``None``\.
         tmp_file_save_freq : int, optional
             The frequency (in epochs) to save a temporary file of the model.
-            Default is ``2``. If set to ``0`` or ``None``, no temporary file
+            Default is ``2``\. If set to ``0`` or ``None``\, no temporary file
             is saved.
         remove_after_load : bool, optional
             Whether to remove the temporary file after loading it. Default is
-            ``True``.
+            ``True``\.
         print_info_batch_freq : int, optional
             The frequency (in batches) to print training information. Default
-            is ``5``. If set to ``0`` or ``None``, no training information is
+            is ``5``\. If set to ``0`` or ``None``\, no training information is
             printed.
 
         Returns
         -------
         None
             The function saves the model to the ``save_model_dir`` directory,
             and optionally to a temporary file. If interrupted with a
-            ``KeyboardInterrupt``, the function tries to load the temporary
+            ``KeyboardInterrupt``\, the function tries to load the temporary
             file. If no temporary file is found, it continues without loading.
 
         Notes
         -----
         Refer to the documentation of
         :meth:`mapreader.train.classifier.classifier.train_core` for more
         information.
         """
 
         try:
             self.train_core(
                 phases,
                 num_epochs,
                 save_model_dir,
-                verbosity_level,
+                verbose,
                 tensorboard_path,
                 tmp_file_save_freq,
                 print_info_batch_freq=print_info_batch_freq,
             )
         except KeyboardInterrupt:
-            print("KeyboardInterrupted...Exiting...")
+            print("[INFO] Exiting...")
             if os.path.isfile(self.tmp_save_filename):
-                print(f"File found: {self.tmp_save_filename}...load...")
-                self.load(
-                    self.tmp_save_filename, remove_after_load=remove_after_load
-                )
+                print(f'[INFO] Loading "{self.tmp_save_filename}" as model.')
+                self.load(self.tmp_save_filename, remove_after_load=remove_after_load)
             else:
-                print("No temporary file was found.")
+                print("[INFO] No checkpoint file found - model has not been updated.")
 
     def train_core(
         self,
         phases: Optional[List[str]] = ["train", "val"],
         num_epochs: Optional[int] = 25,
         save_model_dir: Optional[Union[str, None]] = "models",
-        verbosity_level: Optional[int] = 1,
+        verbose: Optional[bool] = False,
         tensorboard_path: Optional[Union[str, None]] = None,
         tmp_file_save_freq: Optional[Union[int, None]] = 2,
         print_info_batch_freq: Optional[Union[int, None]] = 5,
     ) -> None:
         """
         Trains/fine-tunes a classifier for the specified number of epochs on
         the given phases using the specified hyperparameters.
 
         Parameters
         ----------
         phases : list of str, optional
-            The phases to train the model on for each epoch. Default is
-            ``["train", "val"]``.
+            The phases to run through during each training iteration. Default is
+            ``["train", "val"]``\.
         num_epochs : int, optional
-            The number of epochs to train the model for. Default is ``25``.
+            The number of epochs to train the model for. Default is ``25``\.
         save_model_dir : str or None, optional
-            The directory to save the model in. Default is ``"models"``. If
-            set to ``None``, the model is not saved.
-        verbosity_level : int, optional
-            The level of verbosity during training:
-
-            - ``0`` is silent,
-            - ``1`` is progress bar and metrics,
-            - ``2`` is detailed information.
-
-            Default is ``1``.
+            The directory to save the model in. Default is ``"models"``\. If
+            set to ``None``\, the model is not saved.
+        verbose : bool, optional
+            Whether to print verbose outputs, by default ``False``\.
         tensorboard_path : str or None, optional
             The path to the directory to save TensorBoard logs in. If set to
-            ``None``, no TensorBoard logs are saved. Default is ``None``.
+            ``None``\, no TensorBoard logs are saved. Default is ``None``\.
         tmp_file_save_freq : int, optional
             The frequency (in epochs) to save a temporary file of the model.
-            Default is ``2``. If set to ``0`` or ``None``, no temporary file
+            Default is ``2``\. If set to ``0`` or ``None``\, no temporary file
             is saved.
         print_info_batch_freq : int, optional
             The frequency (in batches) to print training information. Default
-            is ``5``. If set to ``0`` or ``None``, no training information is
+            is ``5``\. If set to ``0`` or ``None``\, no training information is
             printed.
 
         Raises
         ------
         ValueError
             If the criterion is not set. Use the ``add_criterion`` method to
             set the criterion.
 
             If the optimizer is not set and the phase is "train". Use the
             ``initialize_optimizer`` or ``add_optimizer`` method to set the
             optimizer.
 
         KeyError
             If the specified phase cannot be found in the keys of the object's
-            ``dataloader`` dictionary property.
+            ``dataloaders`` dictionary property.
 
         Returns
         -------
         None
         """
 
         if self.criterion is None:
             raise ValueError(
-                "[ERROR] criterion is needed. Use add_criterion method"
+                "[ERROR] Criterion is not yet defined.\n\n\
+Use ``add_criterion`` to define one."
             )
 
+        print(f"[INFO] Each training step will pass: {phases}.")
+
         for phase in phases:
-            if phase not in self.dataloader.keys():
+            if phase not in self.dataloaders.keys():
                 raise KeyError(
-                    f"[ERROR] specified phase: {phase} cannot be find in object's dataloader with keys: {self.dataloader.keys()}"  # noqa
+                    f'[ERROR] "{phase}" dataloader cannot be found in dataloaders.\n\
+    Valid options for ``phases`` argument are: {self.dataloaders.keys()}'  # noqa
                 )
 
-        if verbosity_level >= 1:
+        if verbose:
             self.train_component_summary()
 
         since = time.time()
 
         # initialize variables
         train_phase_names = ["train", "training"]
         valid_phase_names = ["val", "validation", "eval", "evaluation"]
         best_model_wts = copy.deepcopy(self.model.state_dict())
         self.pred_conf = []
-        self.pred_label = []
-        self.orig_label = []
+        self.pred_label_indices = []
+        self.orig_label_indices = []
         if save_model_dir is not None:
             save_model_dir = os.path.abspath(save_model_dir)
 
         # Check if SummaryWriter (for tensorboard) can be imported
         tboard_writer = None
         if tensorboard_path is not None:
             try:
                 from torch.utils.tensorboard import SummaryWriter
 
                 tboard_writer = SummaryWriter(tensorboard_path)
             except ImportError:
                 print(
-                    "[WARNING] could not import SummaryWriter from torch.utils.tensorboard"  # noqa
+                    "[WARNING] Could not import ``SummaryWriter`` from torch.utils.tensorboard"  # noqa
                 )
-                print("[WARNING] continue without tensorboard.")
+                print("[WARNING] Continuing without tensorboard.")
                 tensorboard_path = None
 
         start_epoch = self.last_epoch + 1
         end_epoch = self.last_epoch + num_epochs
+
         # --- Main train loop
         for epoch in range(start_epoch, end_epoch + 1):
             # --- loop, phases
             for phase in phases:
                 if phase.lower() in train_phase_names:
                     self.model.train()
                 else:
                     self.model.eval()
 
                 # initialize vars with one epoch lifetime
                 running_loss = 0.0
                 running_pred_conf = []
-                running_pred_label = []
-                running_orig_label = []
+                running_pred_label_indices = []
+                running_orig_label_indices = []
 
                 # TQDM
-                # batch_loop = tqdm(iter(self.dataloader[phase]), total=len(self.dataloader[phase]), leave=False) # noqa
+                # batch_loop = tqdm(iter(self.dataloaders[phase]), total=len(self.dataloaders[phase]), leave=False) # noqa
                 # if phase.lower() in train_phase_names+valid_phase_names:
                 #     batch_loop.set_description(f"Epoch {epoch}/{end_epoch}")
 
-                phase_batch_size = self.dataloader[phase].batch_size
-                total_inp_counts = len(self.dataloader[phase].dataset)
+                phase_batch_size = self.dataloaders[phase].batch_size
+                total_inp_counts = len(self.dataloaders[phase].dataset)
 
                 # --- loop, batches
-                for batch_idx, (inputs, labels) in enumerate(
-                    self.dataloader[phase]
+                for batch_idx, (inputs, labels, label_indices) in enumerate(
+                    self.dataloaders[phase]
                 ):
                     inputs = inputs.to(self.device)
-                    labels = labels.to(self.device)
+                    label_indices = label_indices.to(self.device)
 
                     if self.optimizer is None:
                         if phase.lower() in train_phase_names:
                             raise ValueError(
-                                f"[ERROR] optimizer should be set when phase is {phase}. Use initialize_optimizer or add_optimizer."  # noqa
+                                f"[ERROR] An optimizer should be defined for {phase} phase.\n\
+Use ``initialize_optimizer`` or ``add_optimizer`` to add one."  # noqa
                             )
                     else:
                         self.optimizer.zero_grad()
 
                     if phase.lower() in train_phase_names + valid_phase_names:
                         # forward, track history if only in train
-                        with torch.set_grad_enabled(
-                            phase.lower() in train_phase_names
-                        ):
+                        with torch.set_grad_enabled(phase.lower() in train_phase_names):
                             # Get model outputs and calculate loss
                             # Special case for inception because in training,
                             # it has an auxiliary output.
                             #     In train mode we calculate the loss by
                             #     summing the final output and the auxiliary
                             #     output but in testing we only consider the
                             #     final output.
                             if self.is_inception and (
                                 phase.lower() in train_phase_names
                             ):
                                 outputs, aux_outputs = self.model(inputs)
-                                loss1 = self.criterion(outputs, labels)
-                                loss2 = self.criterion(aux_outputs, labels)
+
+                                if not all(
+                                    isinstance(out, torch.Tensor)
+                                    for out in [outputs, aux_outputs]
+                                ):
+                                    try:
+                                        outputs = outputs.logits
+                                        aux_outputs = aux_outputs.logits
+                                    except AttributeError as err:
+                                        raise AttributeError(err.message)
+
+                                loss1 = self.criterion(outputs, label_indices)
+                                loss2 = self.criterion(aux_outputs, label_indices)
                                 # XXX From https://discuss.pytorch.org/t/how-to-optimize-inception-model-with-auxiliary-classifiers/7958 # noqa
                                 loss = loss1 + 0.4 * loss2
+
                             else:
                                 outputs = self.model(inputs)
-                                # labels = labels.long().squeeze_()
-                                loss = self.criterion(outputs, labels)
 
-                            _, pred_label = torch.max(outputs, dim=1)
+                                if not isinstance(outputs, torch.Tensor):
+                                    try:
+                                        outputs = outputs.logits
+                                    except AttributeError as err:
+                                        raise AttributeError(err.message)
+                                loss = self.criterion(outputs, label_indices)
+
+                            _, pred_label_indices = torch.max(outputs, dim=1)
 
                             # backward + optimize only if in training phase
                             if phase.lower() in train_phase_names:
                                 loss.backward()
                                 self.optimizer.step()
 
                         # XXX (why multiply?)
                         running_loss += loss.item() * inputs.size(0)
 
                         # TQDM
                         # batch_loop.set_postfix(loss=loss.data)
                         # batch_loop.refresh()
                     else:
                         outputs = self.model(inputs)
-                        _, pred_label = torch.max(outputs, dim=1)
+
+                        if not isinstance(outputs, torch.Tensor):
+                            try:
+                                outputs = outputs.logits
+                            except AttributeError as err:
+                                raise AttributeError(err.message)
+
+                        _, pred_label_indices = torch.max(outputs, dim=1)
 
                     running_pred_conf.extend(
-                        torch.nn.functional.softmax(outputs, dim=1)
-                        .cpu()
-                        .tolist()
+                        torch.nn.functional.softmax(outputs, dim=1).cpu().tolist()
                     )
-                    running_pred_label.extend(pred_label.cpu().tolist())
-                    running_orig_label.extend(labels.cpu().tolist())
+                    running_pred_label_indices.extend(pred_label_indices.cpu().tolist())
+                    running_orig_label_indices.extend(label_indices.cpu().tolist())
 
                     if batch_idx % print_info_batch_freq == 0:
                         curr_inp_counts = min(
                             total_inp_counts,
                             (batch_idx + 1) * phase_batch_size,
                         )
-                        progress_perc = (
-                            curr_inp_counts / total_inp_counts * 100.0
-                        )
-                        tmp_str = f"{curr_inp_counts}/{total_inp_counts} ({progress_perc:5.1f}%)"  # noqa
+                        progress_perc = curr_inp_counts / total_inp_counts * 100.0
+                        tmp_str = f"{curr_inp_counts}/{total_inp_counts} ({progress_perc:5.1f}% )"  # noqa
 
                         epoch_msg = f"{phase: <8} -- {epoch}/{end_epoch} -- "
                         epoch_msg += f"{tmp_str: >20} -- "
 
                         if phase.lower() in valid_phase_names:
                             epoch_msg += f"Loss: {loss.data:.3f}"
-                            self.cprint("[INFO]", self.color_dred, epoch_msg)
+                            self.cprint("[INFO]", self.__color_dred, epoch_msg)
                         elif phase.lower() in train_phase_names:
                             epoch_msg += f"Loss: {loss.data:.3f}"
-                            self.cprint("[INFO]", self.color_dgreen, epoch_msg)
+                            self.cprint("[INFO]", self.__color_dgreen, epoch_msg)
                         else:
-                            self.cprint("[INFO]", self.color_dgreen, epoch_msg)
+                            self.cprint("[INFO]", self.__color_dgreen, epoch_msg)
                     # --- END: one batch
 
                 # scheduler
-                if phase.lower() in train_phase_names and (
-                    self.scheduler is not None
-                ):
+                if phase.lower() in train_phase_names and (self.scheduler is not None):
                     self.scheduler.step()
 
                 if phase.lower() in train_phase_names + valid_phase_names:
                     # --- collect statistics
-                    epoch_loss = running_loss / self.dataset_sizes[phase]
+                    epoch_loss = running_loss / len(self.dataloaders[phase].dataset)
                     self._add_metrics(f"epoch_loss_{phase}", epoch_loss)
 
                     if tboard_writer is not None:
                         tboard_writer.add_scalar(
                             f"loss/{phase}",
                             self.metrics[f"epoch_loss_{phase}"][-1],
                             epoch,
                         )
 
                     # other metrics (precision/recall/F1)
                     self.calculate_add_metrics(
-                        running_orig_label,
-                        running_pred_label,
+                        running_orig_label_indices,
+                        running_pred_label_indices,
                         running_pred_conf,
                         phase,
                         epoch,
                         tboard_writer,
                     )
 
                     epoch_msg = f"{phase: <8} -- {epoch}/{end_epoch} -- "
-                    epoch_msg = self.gen_epoch_msg(phase, epoch_msg)
+                    epoch_msg = self._gen_epoch_msg(phase, epoch_msg)
 
                     if phase.lower() in valid_phase_names:
-                        self.cprint(
-                            "[INFO]", self.color_dred, epoch_msg + "\n"
-                        )
+                        self.cprint("[INFO]", self.__color_dred, epoch_msg + "\n")
                     else:
-                        self.cprint("[INFO]", self.color_dgreen, epoch_msg)
+                        self.cprint("[INFO]", self.__color_dgreen, epoch_msg)
 
                 # labels/confidence
                 self.pred_conf.extend(running_pred_conf)
-                self.pred_label.extend(running_pred_label)
-                self.orig_label.extend(running_orig_label)
+                self.pred_label_indices.extend(running_pred_label_indices)
+                self.orig_label_indices.extend(running_orig_label_indices)
 
                 # Update best_loss and _epoch?
-                if (
-                    phase.lower() in valid_phase_names
-                    and epoch_loss < self.best_loss
-                ):
+                if phase.lower() in valid_phase_names and epoch_loss < self.best_loss:
                     self.best_loss = epoch_loss
                     self.best_epoch = epoch
                     best_model_wts = copy.deepcopy(self.model.state_dict())
 
                 if phase.lower() in valid_phase_names:
                     if epoch % tmp_file_save_freq == 0:
-                        print(
-                            f"SAVE temp file: {self.tmp_save_filename} | set .last_epoch: {epoch}"  # noqa
-                        )
-                        tmp_str = f"[INFO] SAVE temp file: {self.tmp_save_filename} | set .last_epoch: {epoch}\n"  # noqa
-                        print(self.color_lgrey + tmp_str + self.color_reset)
+                        tmp_str = f'[INFO] Checkpoint file saved to "{self.tmp_save_filename}".'  # noqa
+                        print(self.__color_lgrey + tmp_str + self.__color_reset)
                         self.last_epoch = epoch
                         self.save(self.tmp_save_filename, force=True)
 
+        self.pred_label = [
+            self.labels_map.get(i, None) for i in self.pred_label_indices
+        ]
+        self.orig_label = [
+            self.labels_map.get(i, None) for i in self.orig_label_indices
+        ]
+
         time_elapsed = time.time() - since
-        print(
-            f"Total time: {time_elapsed // 60:.0f}m {time_elapsed % 60:.0f}s"
-        )
+        print(f"[INFO] Total time: {time_elapsed // 60:.0f}m {time_elapsed % 60:.0f}s")
 
         # load best model weights
         self.model.load_state_dict(best_model_wts)
 
         # --- SAVE model/object
         if phase.lower() in train_phase_names + valid_phase_names:
             self.last_epoch = epoch
             if save_model_dir is not None:
                 save_filename = f"checkpoint_{self.best_epoch}.pkl"
                 save_model_path = os.path.join(save_model_dir, save_filename)
                 self.save(save_model_path, force=True)
-                with open(
-                    os.path.join(save_model_dir, "info.txt"), "a+"
-                ) as fio:
+                with open(os.path.join(save_model_dir, "info.txt"), "a+") as fio:
                     fio.writelines(f"{save_filename},{self.best_loss:.5f}\n")
 
                 print(
-                    f"[INFO] Save model epoch: {self.best_epoch} with least valid loss: {self.best_loss:.4f}"  # noqa
-                )
-                print(f"[INFO] Path: {save_model_path}")
+                    f"[INFO] Model at epoch {self.best_epoch} has least valid loss ({self.best_loss:.4f}) so will be saved.\n\
+[INFO] Path: {save_model_path}"
+                )  # noqa
 
     def calculate_add_metrics(
         self,
         y_true,
         y_pred,
         y_score,
         phase: str,
@@ -1168,34 +1057,34 @@
             targets as returned by a classifier.
 
         y_score : array-like of shape (n_samples, n_classes)
             Predicted probabilities for each class. Only required when
             ``y_pred`` is not binary.
 
         phase : str
-            Name of the current phase, typically ``"train"`` or ``"val"``. See
+            Name of the current phase, typically ``"train"`` or ``"val"``\. See
             ``train`` function.
 
         epoch : int, optional
-            Current epoch number. Default is ``-1``.
+            Current epoch number. Default is ``-1``\.
 
         tboard_writer : object, optional
             TensorBoard SummaryWriter object to write the metrics. Default is
-            ``None``.
+            ``None``\.
 
         Returns
         -------
         None
 
         Notes
         -----
         This method uses both the
         ``sklearn.metrics.precision_recall_fscore_support`` and
         ``sklearn.metrics.roc_auc_score`` functions from ``scikit-learn`` to
-        calculate the metrics for each average type (``"micro"``, ``"macro"``
+        calculate the metrics for each average type (``"micro"``\, ``"macro"``
         and ``"weighted"``). The results are then added to the ``metrics``
         dictionary. It also writes the metrics to the TensorBoard
         SummaryWriter, if ``tboard_writer`` is not None.
         """
         # convert y_score to a numpy array:
         y_score = np.array(y_score)
 
@@ -1269,24 +1158,24 @@
                 )
                 tboard_writer.add_scalar(
                     f"Fscore/{phase}/binary_{i}",
                     self.metrics[f"epoch_fscore_{i}_{phase}"][-1],
                     epoch,
                 )
 
-    def gen_epoch_msg(self, phase: str, epoch_msg: str) -> str:
+    def _gen_epoch_msg(self, phase: str, epoch_msg: str) -> str:
         """
         Generates a log message for an epoch during training or validation.
         The message includes information about the loss, F-score, and recall
         for a given phase (training or validation).
 
         Parameters
         ----------
         phase : str
-            The training phase, either ``"train"`` or ``"val"``.
+            The training phase, either ``"train"`` or ``"val"``\.
         epoch_msg : str
             The message string to be modified with the epoch metrics.
 
         Returns
         -------
         epoch_msg : str
             The updated message string with the epoch metrics.
@@ -1321,15 +1210,15 @@
 
         Notes
         -----
         If the key ``k`` does not exist in the dictionary of metrics, a new
         key-value pair is created with ``k`` as the key and a new list
         containing the value ``v`` as the value. If the key ``k`` already
         exists in the dictionary of metrics, the value `v` is appended to the
-        list associated with the key ``k``.
+        list associated with the key ``k``\.
         """
         if k not in self.metrics.keys():
             self.metrics[k] = [v]
         else:
             self.metrics[k].append(v)
 
     def plot_metric(
@@ -1357,32 +1246,32 @@
             The label for the y-axis.
         legends : list of str
             The legend labels for each metric.
         x_axis : str, optional
             The metric to be used as the x-axis. Can be ``"epoch"`` (default)
             or any other metric name present in the dataset.
         x_label : str, optional
-            The label for the x-axis. Defaults to ``"epoch"``.
+            The label for the x-axis. Defaults to ``"epoch"``\.
         colors : list of str, optional
             The colors to be used for the lines of each metric. It must be at
-            least the same size as ``y_axis``. Defaults to
-            ``5 * ["k", "tab:red"]``.
+            least the same size as ``y_axis``\. Defaults to
+            ``5 * ["k", "tab:red"]``\.
         styles : list of str, optional
             The line styles to be used for the lines of each metric. It must
-            be at least the same size as ``y_axis``. Defaults to
-            ``10 * ["-"]``.
+            be at least the same size as ``y_axis``\. Defaults to
+            ``10 * ["-"]``\.
         markers : list of str, optional
             The markers to be used for the lines of each metric. It must be at
-            least the same size as ``y_axis``. Defaults to ``10 * ["o"]``.
+            least the same size as ``y_axis``\. Defaults to ``10 * ["o"]``\.
         figsize : tuple of int, optional
-            The size of the figure in inches. Defaults to ``(10, 5)``.
+            The size of the figure in inches. Defaults to ``(10, 5)``\.
         plt_yrange : tuple of float, optional
-            The range of values for the y-axis. Defaults to ``None``.
+            The range of values for the y-axis. Defaults to ``None``\.
         plt_xrange : tuple of float, optional
-            The range of values for the x-axis. Defaults to ``None``.
+            The range of values for the x-axis. Defaults to ``None``\.
 
         Returns
         -------
         None
 
         Notes
         -----
@@ -1447,41 +1336,33 @@
             plt.xlim(plt_xrange[0], plt_xrange[1])
         if plt_yrange is not None:
             plt.ylim(plt_yrange[0], plt_yrange[1])
 
         plt.grid()
         plt.show()
 
-    def initialize_model(
+    def _initialize_model(
         self,
         model_name: str,
         pretrained: Optional[bool] = True,
         last_layer_num_classes: Optional[Union[str, int]] = "default",
-        add_model: Optional[bool] = True,
     ) -> Tuple[Any, int, bool]:
         """
         Initializes a PyTorch model with the option to change the number of
         classes in the last layer (``last_layer_num_classes``).
 
-        The function handles six PyTorch models: ResNet, AlexNet, VGG,
-        SqueezeNet, DenseNet, and Inception v3.
-
         Parameters
         ----------
         model_name : str
-            Name of a PyTorch model. See
-            https://pytorch.org/vision/0.8/models.html
+            Name of a PyTorch model. See https://pytorch.org/vision/0.8/models.html for options.
         pretrained : bool, optional
             Use pretrained version, by default ``True``
         last_layer_num_classes : str or int, optional
-            Number of elements in the last layer. If ``"default"``, sets it to
-            the number of classes. By default, ``"default"``.
-        add_model : bool, optional
-            If ``True`` (default), adds the initialized model to the instance
-            of the class.
+            Number of elements in the last layer. If ``"default"``\, sets it to
+            the number of classes. By default, ``"default"``\.
 
         Returns
         -------
         model : PyTorch model
             The initialized PyTorch model with the changed last layer.
         input_size : int
             Input size of the model.
@@ -1491,48 +1372,44 @@
         Raises
         ------
         ValueError
             If an invalid model name is passed.
 
         Notes
         -----
-        Inception v3 requires the input size to be ``(299, 299)``, whereas all
-        of the other models expect ``(224, 224)``.
+        Inception v3 requires the input size to be ``(299, 299)``\, whereas all
+        of the other models expect ``(224, 224)``\.
 
-        See https://pytorch.org/vision/0.8/models.html for available models.
+        See https://pytorch.org/vision/0.8/models.html.
         """
 
         # Initialize these variables which will be set in this if statement.
         # Each of these variables is model specific.
         model_dw = models.__getattribute__(model_name)
         model_dw = model_dw(pretrained)
-        input_size = 224
+        input_size = (224, 224)
         is_inception = False
 
         if last_layer_num_classes in ["default"]:
-            last_layer_num_classes = self.num_classes
+            last_layer_num_classes = len(self.labels_map)
         else:
             last_layer_num_classes = int(last_layer_num_classes)
 
         if "resnet" in model_name:
             num_ftrs = model_dw.fc.in_features
             model_dw.fc = nn.Linear(num_ftrs, last_layer_num_classes)
 
         elif "alexnet" in model_name:
             num_ftrs = model_dw.classifier[6].in_features
-            model_dw.classifier[6] = nn.Linear(
-                num_ftrs, last_layer_num_classes
-            )
+            model_dw.classifier[6] = nn.Linear(num_ftrs, last_layer_num_classes)
 
         elif "vgg" in model_name:
             # vgg11_bn
             num_ftrs = model_dw.classifier[6].in_features
-            model_dw.classifier[6] = nn.Linear(
-                num_ftrs, last_layer_num_classes
-            )
+            model_dw.classifier[6] = nn.Linear(num_ftrs, last_layer_num_classes)
 
         elif "squeezenet" in model_name:
             model_dw.classifier[1] = nn.Conv2d(
                 512, last_layer_num_classes, kernel_size=(1, 1), stride=(1, 1)
             )
             model_dw.num_classes = last_layer_num_classes
 
@@ -1550,23 +1427,19 @@
             # Handle the primary net
             num_ftrs = model_dw.fc.in_features
             model_dw.fc = nn.Linear(num_ftrs, last_layer_num_classes)
             is_inception = True
             input_size = 299
 
         else:
-            raise ValueError("Invalid model name, exiting...")
+            raise NotImplementedError("[ERROR] Invalid model name.")
 
-        if add_model:
-            self.del_model()
-            self.add_model(
-                model_dw, input_size=input_size, is_inception=is_inception
-            )
-        else:
-            return model_dw, input_size, is_inception
+        self.model = model_dw.to(self.device)
+        self.input_size = input_size
+        self.is_inception = is_inception
 
     def show_sample(
         self,
         set_name: Optional[str] = "train",
         batch_number: Optional[int] = 1,
         print_batch_info: Optional[bool] = True,
         figsize: Optional[Tuple[int, int]] = (15, 10),
@@ -1575,22 +1448,22 @@
         Displays a sample of training or validation data in a grid format with
         their corresponding class labels.
 
         Parameters
         ----------
         set_name : str, optional
             Name of the dataset (``"train"``/``"validation"``) to display the
-            sample from, by default ``"train"``.
+            sample from, by default ``"train"``\.
         batch_number : int, optional
-            Number of batches to display, by default ``1``.
+            Which batch to display, by default ``1``\.
         print_batch_info : bool, optional
             Whether to print information about the batch size, by default
-            ``True``.
+            ``True``\.
         figsize : tuple, optional
-            Figure size (width, height) in inches, by default ``(15, 10)``.
+            Figure size (width, height) in inches, by default ``(15, 10)``\.
 
         Returns
         -------
         None
             Displays the sample images with their corresponding class labels.
 
         Raises
@@ -1602,54 +1475,75 @@
         Notes
         -----
         This method uses the dataloader of the ``ImageClassifierData`` class
         and the ``torchvision.utils.make_grid`` function to display the sample
         data in a grid format. It also calls the ``_imshow`` method of the
         ``ImageClassifierData`` class to show the sample data.
         """
+        if set_name not in self.dataloaders.keys():
+            raise ValueError(
+                f"[ERROR] ``set_name`` must be one of {list(self.dataloaders.keys())}."
+            )
+
         if print_batch_info:
             # print info about batch size
-            self.batch_info(set_name)
+            self.print_batch_info(set_name)
 
-        dl_iter = iter(self.dataloader[set_name])
+        dataloader = self.dataloaders[set_name]
+
+        num_batches = int(np.ceil(len(dataloader.dataset) / dataloader.batch_size))
+        if min(num_batches, batch_number) != batch_number:
+            print(
+                f'[INFO] "{set_name}" only contains {num_batches}.\n\
+Output will show batch number {num_batches}.'
+            )
+            batch_number = num_batches
+
+        dl_iter = iter(dataloader)
         for _ in range(batch_number):
             # Get a batch of training data
-            inputs, classes = next(dl_iter)
+            inputs, labels, label_indices = next(dl_iter)
 
         # Make a grid from batch
         out = torchvision.utils.make_grid(inputs)
         self._imshow(
             out,
-            title=str([self.class_names[int(x)] for x in classes]),
+            title=f"{labels}\n{label_indices.tolist()}",
             figsize=figsize,
         )
 
-    def batch_info(self, set_name: Optional[str] = "train") -> None:
+    def print_batch_info(self, set_name: Optional[str] = "train") -> None:
         """
         Print information about a dataset's batches, samples, and batch-size.
 
         Parameters
         ----------
         set_name : str, optional
             Name of the dataset to display batch information for (default is
             ``"train"``).
 
         Returns
         -------
         None
         """
+        if set_name not in self.dataloaders.keys():
+            raise ValueError(
+                f"[ERROR] ``set_name`` must be one of {list(self.dataloaders.keys())}."
+            )
 
-        batch_size = self.dataloader[set_name].batch_size
-        num_samples = len(self.dataloader[set_name].dataset)
+        batch_size = self.dataloaders[set_name].batch_size
+        num_samples = len(self.dataloaders[set_name].dataset)
         num_batches = int(np.ceil(num_samples / batch_size))
 
-        print(f"[INFO] dataset: {set_name}")
-        print(f"#samples:    {num_samples}")
-        print(f"#batch size: {batch_size}")
-        print(f"#batches:    {num_batches}")
+        print(
+            f"[INFO] dataset: {set_name}\n\
+        - items:        {num_samples}\n\
+        - batch size:   {batch_size}\n\
+        - batches:      {num_batches}"
+        )
 
     @staticmethod
     def _imshow(
         inp: np.ndarray,
         title: Optional[str] = None,
         figsize: Optional[Tuple[int, int]] = (15, 10),
     ) -> None:
@@ -1657,18 +1551,18 @@
         Displays an image of a tensor using matplotlib.pyplot.
 
         Parameters
         ----------
         inp : numpy.ndarray
             Input image to be displayed.
         title : str, optional
-            Title of the plot, default is ``None``.
+            Title of the plot, default is ``None``\.
         figsize : tuple, optional
             Figure size in inches as a tuple of (width, height), default is
-            ``(15, 10)``.
+            ``(15, 10)``\.
 
         Returns
         -------
         None
             Displays the image of the provided tensor.
         """
 
@@ -1679,141 +1573,150 @@
         # inp = std * inp + mean
 
         inp = np.clip(inp, 0, 1)
         plt.figure(figsize=figsize)
         plt.imshow(inp)
         if title is not None:
             plt.title(title)
+        plt.axis("off")
         plt.pause(0.001)  # pause a bit so that plots are updated
         plt.show()
 
-    def inference_sample_results(
+    def show_inference_sample_results(
         self,
+        label: str,
         num_samples: Optional[int] = 6,
-        class_index: Optional[int] = 0,
-        set_name: Optional[str] = "train",
+        set_name: Optional[str] = "test",
         min_conf: Optional[Union[None, float]] = None,
         max_conf: Optional[Union[None, float]] = None,
         figsize: Optional[Tuple[int, int]] = (15, 15),
     ) -> None:
         """
-        Performs inference on a given dataset and displays results for a
-        specified class.
+        Shows a sample of the results of the inference.
 
         Parameters
         ----------
+        label : str, optional
+            The label for which to display results.
         num_samples : int, optional
-            The number of sample results to display. Defaults to ``6``.
-        class_index : int, optional
-            The index of the class for which to display results. Defaults to
-            ``0``.
+            The number of sample results to display. Defaults to ``6``\.
         set_name : str, optional
             The name of the dataset split to use for inference. Defaults to
-            ``"train"``.
+            ``"test"``\.
         min_conf : float, optional
             The minimum confidence score for a sample result to be displayed.
             Samples with lower confidence scores will be skipped. Defaults to
-            ``None``.
+            ``None``\.
         max_conf : float, optional
             The maximum confidence score for a sample result to be displayed.
             Samples with higher confidence scores will be skipped. Defaults to
-            ``None``.
+            ``None``\.
         figsize : tuple[int, int], optional
             Figure size (width, height) in inches, displaying the sample
-            results. Defaults to ``(15, 15)``.
+            results. Defaults to ``(15, 15)``\.
 
         Returns
         -------
         None
         """
 
         # eval mode, keep track of the current mode
         was_training = self.model.training
         self.model.eval()
 
         counter = 0
         fig = plt.figure(figsize=figsize)
         with torch.no_grad():
-            for inputs, labels in iter(self.dataloader[set_name]):
+            for inputs, labels, label_indices in iter(self.dataloaders[set_name]):
                 inputs = inputs.to(self.device)
-                labels = labels.to(self.device)
+                label_indices = label_indices.to(self.device)
 
                 outputs = self.model(inputs)
+
+                if not isinstance(outputs, torch.Tensor):
+                    try:
+                        outputs = outputs.logits
+                    except AttributeError as err:
+                        raise AttributeError(err.message)
+
                 pred_conf = torch.nn.functional.softmax(outputs, dim=1) * 100.0
                 _, preds = torch.max(outputs, 1)
 
+                # reverse the labels_map dict
+                label_index_dict = {v: k for k, v in self.labels_map.items()}
+
                 # go through images in batch
                 for j in range(len(preds)):
-                    pred_ind = int(preds[j])
-                    if pred_ind != class_index:
+                    predicted_index = int(preds[j])
+                    if predicted_index != label_index_dict[label]:
                         continue
                     if (min_conf is not None) and (
-                        pred_conf[j][pred_ind] < min_conf
+                        pred_conf[j][predicted_index] < min_conf
                     ):
                         continue
                     if (max_conf is not None) and (
-                        pred_conf[j][pred_ind] > max_conf
+                        pred_conf[j][predicted_index] > max_conf
                     ):
                         continue
 
                     counter += 1
 
-                    class_name = self.class_names[pred_ind]
-                    conf_score = pred_conf[j][pred_ind]
+                    conf_score = pred_conf[j][predicted_index]
                     ax = plt.subplot(int(num_samples / 2.0), 3, counter)
                     ax.axis("off")
-                    ax.set_title(f"{class_name} | {conf_score:.3f}")
+                    ax.set_title(f"{label} | {conf_score:.3f}")
 
                     inp = inputs.cpu().data[j].numpy().transpose((1, 2, 0))
                     inp = np.clip(inp, 0, 1)
                     plt.imshow(inp)
 
                     if counter == num_samples:
                         self.model.train(mode=was_training)
                         plt.show()
                         return
+
             self.model.train(mode=was_training)
             plt.show()
 
     def save(
         self,
         save_path: Optional[str] = "default.obj",
         force: Optional[bool] = False,
     ) -> None:
         """
         Save the object to a file.
 
         Parameters
         ----------
         save_path : str, optional
-            The path to the file to write. If the file already exists and
-            ``force`` is not ``True``, a ``FileExistsError`` is raised.
-            Defaults to ``"default.obj"``.
+            The path to the file to write.
+            If the file already exists and ``force`` is not ``True``\, a ``FileExistsError`` is raised.
+            Defaults to ``"default.obj"``\.
         force : bool, optional
             Whether to overwrite the file if it already exists. Defaults to
-            ``False``.
+            ``False``\.
 
         Raises
         ------
         FileExistsError
-            If the file already exists and ``force`` is not ``True``.
+            If the file already exists and ``force`` is not ``True``\.
 
         Notes
         -----
         The object is saved in two parts. First, a serialized copy of the
         object's dictionary is written to the specified file using the
         ``joblib.dump`` function. The object's ``model`` attribute is excluded
         from this dictionary and saved separately using the ``torch.save``
-        function, with a filename derived from the original ``save_path``.
+        function, with a filename derived from the original ``save_path``\.
         """
         if os.path.isfile(save_path):
             if force:
                 os.remove(save_path)
             else:
-                raise FileExistsError(f"file already exists: {save_path}")
+                raise FileExistsError(f"[INFO] File already exists: {save_path}")
 
         # parent/base-names
         par_name = os.path.dirname(os.path.abspath(save_path))
         base_name = os.path.basename(os.path.abspath(save_path))
 
         # Extract model, write it separately using torch.save
         obj2write = copy.deepcopy(self.__dict__)
@@ -1823,70 +1726,97 @@
         os.makedirs(par_name, exist_ok=True)
         with open(save_path, "wb") as myfile:
             # pickle.dump(self.__dict__, myfile)
             joblib.dump(obj2write, myfile)
 
         torch.save(mymodel, os.path.join(par_name, f"model_{base_name}"))
 
+    def load_dataset(
+        self,
+        dataset: PatchDataset,
+        set_name: str,
+        batch_size: Optional[int] = 16,
+        sampler: Optional[Union[Sampler, None]] = None,
+        shuffle: Optional[bool] = False,
+        num_workers: Optional[int] = 0,
+        **kwargs,
+    ) -> None:
+        """Creates a DataLoader from a PatchDataset and adds it to the ``dataloaders`` dictionary.
+
+        Parameters
+        ----------
+        dataset : PatchDataset
+            The dataset to add
+        set_name : str
+            The name to use for the dataset
+        batch_size : Optional[int], optional
+            The batch size to use when creating the DataLoader, by default 16
+        sampler : Optional[Union[Sampler, None]], optional
+            The sampler to use when creating the DataLoader, by default None
+        shuffle : Optional[bool], optional
+            Whether to shuffle the PatchDataset, by default False
+        num_workers : Optional[int], optional
+            The number of worker threads to use for loading data, by default 0.
+        """
+        if sampler and shuffle:
+            print("[INFO] ``sampler`` is defined so train dataset will be unshuffled.")
+
+        dataloader = DataLoader(
+            dataset,
+            batch_size=batch_size,
+            sampler=sampler,
+            shuffle=shuffle,
+            num_workers=num_workers,
+            **kwargs,
+        )
+
+        self.dataloaders[set_name] = dataloader
+
     def load(
         self,
         load_path: str,
-        remove_after_load: Optional[bool] = False,
         force_device: Optional[bool] = False,
     ) -> None:
         """
         This function loads the state of a class instance from a saved file
         using the joblib library. It also loads a PyTorch model from a
         separate file and maps it to the device used to load the class
         instance.
 
         Parameters
         ----------
         load_path : str
             Path to the saved file to load.
-        remove_after_load : bool, optional
-            Whether to remove the saved file after loading. Defaults to
-            ``False``.
         force_device : bool or str, optional
             Whether to force the use of a specific device, or the name of the
-            device to use. If set to ``True``, the default device is used.
-            Defaults to ``False``.
+            device to use. If set to ``True``\, the default device is used.
+            Defaults to ``False``\.
 
         Raises
         ------
         FileNotFoundError
             If the specified file does not exist.
 
-        Modifies
-        ----------
-        self.__dict__ : dict
-            The state of the class instance is updated with the contents of
-            the saved file.
-        os.environ["CUDA_VISIBLE_DEVICES"] : str
-            The CUDA_VISIBLE_DEVICES environment variable is updated if the
-            ``force_device`` argument is specified.
-
         Returns
         -------
         None
         """
 
         load_path = os.path.abspath(load_path)
         mydevice = self.device
 
         if not os.path.isfile(load_path):
-            raise FileNotFoundError(f"file not found: {load_path}")
+            raise FileNotFoundError(f'[ERROR] "{load_path}" cannot be found.')
+
+        print(f'[INFO] Loading "{load_path}".')
 
         with open(load_path, "rb") as myfile:
             # objPickle = pickle.load(myfile)
             objPickle = joblib.load(myfile)
 
-        if remove_after_load:
-            os.remove(load_path)
-
         self.__dict__ = objPickle
 
         if force_device:
             if not isinstance(force_device, str):
                 force_device = str(force_device)
             os.environ["CUDA_VISIBLE_DEVICES"] = force_device
 
@@ -1900,55 +1830,55 @@
             self.model = self.model.to(mydevice)
         except:
             pass
 
     def _print_colors(self):
         """Private function, setting color attributes on the object."""
         # color
-        self.color_lgrey = "\033[1;90m"
-        self.color_grey = "\033[90m"  # broing information
-        self.color_yellow = "\033[93m"  # FYI
-        self.color_orange = "\033[0;33m"  # Warning
+        self.__color_lgrey = "\033[1;90m"
+        self.__color_grey = "\033[90m"  # boring information
+        self.__color_yellow = "\033[93m"  # FYI
+        self.__color_orange = "\033[0;33m"  # Warning
 
-        self.color_lred = "\033[1;31m"  # there is smoke
-        self.color_red = "\033[91m"  # fire!
-        self.color_dred = "\033[2;31m"  # Everything is on fire
+        self.__color_lred = "\033[1;31m"  # there is smoke
+        self.__color_red = "\033[91m"  # fire!
+        self.__color_dred = "\033[2;31m"  # Everything is on fire
 
-        self.color_lblue = "\033[1;34m"
-        self.color_blue = "\033[94m"
-        self.color_dblue = "\033[2;34m"
+        self.__color_lblue = "\033[1;34m"
+        self.__color_blue = "\033[94m"
+        self.__color_dblue = "\033[2;34m"
 
-        self.color_lgreen = "\033[1;32m"  # all is normal
-        self.color_green = "\033[92m"  # something else
-        self.color_dgreen = "\033[2;32m"  # even more interesting
+        self.__color_lgreen = "\033[1;32m"  # all is normal
+        self.__color_green = "\033[92m"  # something else
+        self.__color_dgreen = "\033[2;32m"  # even more interesting
 
-        self.color_lmagenta = "\033[1;35m"
-        self.color_magenta = "\033[95m"  # for title
-        self.color_dmagenta = "\033[2;35m"
+        self.__color_lmagenta = "\033[1;35m"
+        self.__color_magenta = "\033[95m"  # for title
+        self.__color_dmagenta = "\033[2;35m"
 
-        self.color_cyan = "\033[96m"  # system time
-        self.color_white = "\033[97m"  # final time
+        self.__color_cyan = "\033[96m"  # system time
+        self.__color_white = "\033[97m"  # final time
 
-        self.color_black = "\033[0;30m"
+        self.__color_black = "\033[0;30m"
 
-        self.color_reset = "\033[0m"
-        self.color_bold = "\033[1m"
-        self.color_under = "\033[4m"
+        self.__color_reset = "\033[0m"
+        self.__color_bold = "\033[1m"
+        self.__color_under = "\033[4m"
 
-    def get_time(self) -> str:
+    def _get_dtime(self) -> str:
         """
         Get the current date and time as a formatted string.
 
         Returns
         -------
         str
             A string representing the current date and time.
         """
-        time = datetime.strftime(datetime.now(), "%Y-%m-%d %H:%M:%S")
-        return time
+        dtime = datetime.strftime(datetime.now(), "%Y-%m-%d %H:%M:%S")
+        return dtime
 
     def cprint(self, type_info: str, bc_color: str, text: str) -> None:
         """
         Print colored text with additional information.
 
         Parameters
         ----------
@@ -1960,43 +1890,43 @@
             The text to display.
 
         Returns
         -------
         None
             The colored message is displayed on the standard output stream.
         """
-        ho_nam = socket.gethostname().split(".")[0][:10]
+        host_name = socket.gethostname().split(".")[0][:10]
 
         print(
-            self.color_green + self.get_time() + self.color_reset,
-            self.color_magenta + ho_nam + self.color_reset,
-            self.color_bold + self.color_grey + type_info + self.color_reset,
-            bc_color + text + self.color_reset,
+            self.__color_green + self._get_dtime() + self.__color_reset,
+            self.__color_magenta + host_name + self.__color_reset,
+            self.__color_bold + self.__color_grey + type_info + self.__color_reset,
+            bc_color + text + self.__color_reset,
         )
 
     def update_progress(
         self,
         progress: Union[float, int],
         text: Optional[str] = "",
         barLength: Optional[int] = 30,
     ) -> None:
         """Update the progress bar.
 
         Parameters
         ----------
         progress : float or int
-            The progress value to display, between ``0`` and ``1``.
+            The progress value to display, between ``0`` and ``1``\.
             If an integer is provided, it will be converted to a float.
             If a value outside the range ``[0, 1]`` is provided, it will be
             clamped to the nearest valid value.
         text : str, optional
             Additional text to display after the progress bar, defaults to
-            ``""``.
+            ``""``\.
         barLength : int, optional
-            The length of the progress bar in characters, defaults to ``30``.
+            The length of the progress bar in characters, defaults to ``30``\.
 
         Raises
         ------
         TypeError
             If progress is not a floating point value or an integer.
 
         Returns
```

### Comparing `mapreader-0.3.4/mapreader/train/classifier_context.py` & `mapreader-1.0.1.post0.dev9/mapreader/classify/classifier_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from .classifier import classifier
-
 import copy
-import matplotlib.pyplot as plt
-import numpy as np
 import os
 import time
-import torchvision
 
 # from tqdm.autonotebook import tqdm
-from typing import Union, List, Optional, Tuple, Dict
+from typing import Dict, List, Optional, Tuple, Union
 
+import matplotlib.pyplot as plt
+import numpy as np
 import torch
+import torchvision
 
+from .classifier import ClassifierContainer
 
-class classifierContext(classifier):
+
+class ClassifierContextContainer(ClassifierContainer):
     def train(
         self,
         phases: Optional[List[str]] = ["train", "val"],
         num_epochs: Optional[int] = 25,
         save_model_dir: Optional[Union[str, None]] = "models",
         verbosity_level: Optional[int] = 1,
         tensorboard_path: Optional[Union[str, None]] = None,
@@ -83,22 +83,20 @@
                 save_model_dir,
                 verbosity_level,
                 tensorboard_path,
                 tmp_file_save_freq,
                 print_info_batch_freq=print_info_batch_freq,
             )
         except KeyboardInterrupt:
-            print("KeyboardInterrupted... Exiting...")
+            print("[INFO] Exiting...")
             if os.path.isfile(self.tmp_save_filename):
-                print(f"File found: {self.tmp_save_filename}... Loading...")
-                self.load(
-                    self.tmp_save_filename, remove_after_load=remove_after_load
-                )
+                print(f'[INFO] Loading "{self.tmp_save_filename}" as model.')
+                self.load(self.tmp_save_filename, remove_after_load=remove_after_load)
             else:
-                print("No temporary file was found.")
+                print("[INFO] No checkpoint file found - model has not been updated.")
 
     def train_core(
         self,
         phases: Optional[List[str]] = ["train", "val"],
         num_epochs: Optional[int] = 25,
         save_model_dir: Optional[Union[str, None]] = "models",
         verbosity_level: Optional[int] = 1,
@@ -157,21 +155,25 @@
         Returns
         -------
         None
         """
 
         if self.criterion is None:
             raise ValueError(
-                "[ERROR] criterion is needed. Use add_criterion method"
+                "[ERROR] Criterion is not yet defined.\n\n\
+Use ``add_criterion`` to define one."
             )
 
+        print(f"[INFO] Each epoch will pass: {phases}.")
+
         for phase in phases:
-            if phase not in self.dataloader.keys():
+            if phase not in self.dataloaders.keys():
                 raise KeyError(
-                    f"[ERROR] specified phase: {phase} cannot be find in object's dataloader with keys: {self.dataloader.keys()}"  # noqa
+                    f'[ERROR] "{phase}" dataloader cannot be found in dataloaders.\n\
+    Valid options for ``phases`` argument are: {self.dataloaders.keys()}'  # noqa
                 )
 
         if verbosity_level >= 1:
             self.train_component_summary()
 
         since = time.time()
 
@@ -210,101 +212,118 @@
                     self.model.train()
                 else:
                     self.model.eval()
 
                 # initialize vars with one epoch lifetime
                 running_loss = 0.0
                 running_pred_conf = []
-                running_pred_label = []
-                running_orig_label = []
+                running_pred_label_indices = []
+                running_orig_label_indices = []
 
                 # TQDM
-                # batch_loop = tqdm(iter(self.dataloader[phase]), total=len(self.dataloader[phase]), leave=False) # noqa
+                # batch_loop = tqdm(iter(self.dataloaders[phase]), total=len(self.dataloaders[phase]), leave=False) # noqa
                 # if phase.lower() in train_phase_names+valid_phase_names:
                 #     batch_loop.set_description(f"Epoch {epoch}/{end_epoch}")
 
-                phase_batch_size = self.dataloader[phase].batch_size
-                total_inp_counts = len(self.dataloader[phase].dataset)
+                phase_batch_size = self.dataloaders[phase].batch_size
+                total_inp_counts = len(self.dataloaders[phase].dataset)
 
                 # --- loop, batches
-                for batch_idx, (inputs1, inputs2, labels) in enumerate(
-                    self.dataloader[phase]
+                for batch_idx, (inputs1, inputs2, labels, label_indices) in enumerate(
+                    self.dataloaders[phase]
                 ):
                     inputs1 = inputs1.to(self.device)
                     inputs2 = inputs2.to(self.device)
-                    labels = labels.to(self.device)
+                    label_indices = label_indices.to(self.device)
 
                     if self.optimizer is None:
                         if phase.lower() in train_phase_names:
                             raise ValueError(
-                                f"[ERROR] optimizer should be set when phase is {phase}. Use initialize_optimizer or add_optimizer."  # noqa
+                                f"[ERROR] An optimizer should be defined for {phase} phase.\n\
+Use ``initialize_optimizer`` or ``add_optimizer`` to add one."  # noqa
                             )
                     else:
                         self.optimizer.zero_grad()
 
                     if phase.lower() in train_phase_names + valid_phase_names:
                         # forward, track history if only in train
-                        with torch.set_grad_enabled(
-                            phase.lower() in train_phase_names
-                        ):
+                        with torch.set_grad_enabled(phase.lower() in train_phase_names):
                             # Get model outputs and calculate loss
                             # Special case for inception because in training
                             # it has an auxiliary output.
                             #     In train mode we calculate the loss by
                             #     summing the final output and the auxiliary
                             #     output but in testing we only consider the
                             #     final output.
                             if self.is_inception and (
                                 phase.lower() in train_phase_names
                             ):
-                                outputs, aux_outputs = self.model(
-                                    inputs1, inputs2
-                                )
-                                loss1 = self.criterion(outputs, labels)
-                                loss2 = self.criterion(aux_outputs, labels)
+                                outputs, aux_outputs = self.model(inputs1, inputs2)
+
+                                if not all(
+                                    isinstance(out, torch.Tensor)
+                                    for out in [outputs, aux_outputs]
+                                ):
+                                    try:
+                                        outputs = outputs.logits
+                                        aux_outputs = aux_outputs.logits
+                                    except AttributeError as err:
+                                        raise AttributeError(err.message)
+
+                                loss1 = self.criterion(outputs, label_indices)
+                                loss2 = self.criterion(aux_outputs, label_indices)
                                 # XXX From https://discuss.pytorch.org/t/how-to-optimize-inception-model-with-auxiliary-classifiers/7958 # noqa
                                 loss = loss1 + 0.4 * loss2
                             else:
                                 outputs = self.model(inputs1, inputs2)
                                 # labels = labels.long().squeeze_()
-                                loss = self.criterion(outputs, labels)
+                                if not isinstance(outputs, torch.Tensor):
+                                    try:
+                                        outputs = outputs.logits
+                                    except AttributeError as err:
+                                        raise AttributeError(err.message)
+
+                                loss = self.criterion(outputs, label_indices)
 
-                            _, pred_label = torch.max(outputs, dim=1)
+                            _, pred_label_indices = torch.max(outputs, dim=1)
 
                             # backward + optimize only if in training phase
                             if phase.lower() in train_phase_names:
                                 loss.backward()
                                 self.optimizer.step()
 
                         # XXX (why multiply?)
                         running_loss += loss.item() * inputs1.size(0)
 
                         # TQDM
                         # batch_loop.set_postfix(loss=loss.data)
                         # batch_loop.refresh()
                     else:
                         outputs = self.model(inputs1, inputs2)
-                        _, pred_label = torch.max(outputs, dim=1)
+
+                        if not isinstance(outputs, torch.Tensor):
+                            try:
+                                outputs = outputs.logits
+                            except AttributeError as err:
+                                raise AttributeError(err.message)
+
+                        _, pred_label_indices = torch.max(outputs, dim=1)
 
                     running_pred_conf.extend(
-                        torch.nn.functional.softmax(outputs, dim=1)
-                        .cpu()
-                        .tolist()
+                        torch.nn.functional.softmax(outputs, dim=1).cpu().tolist()
                     )
-                    running_pred_label.extend(pred_label.cpu().tolist())
-                    running_orig_label.extend(labels.cpu().tolist())
+                    running_pred_label_indices.extend(pred_label_indices.cpu().tolist())
+                    running_orig_label_indices.extend(label_indices.cpu().tolist())
 
                     if batch_idx % print_info_batch_freq == 0:
                         curr_inp_counts = min(
                             total_inp_counts,
                             (batch_idx + 1) * phase_batch_size,
                         )
-                        progress_perc = (
-                            curr_inp_counts / total_inp_counts * 100.0
-                        )
+                        progress_perc = curr_inp_counts / total_inp_counts * 100.0
                         tmp_str = f"{curr_inp_counts}/{total_inp_counts} ({progress_perc:5.1f}%)"  # noqa
 
                         epoch_msg = f"{phase: <8} -- {epoch}/{end_epoch} -- "
                         epoch_msg += f"{tmp_str: >20} -- "
 
                         if phase.lower() in valid_phase_names:
                             epoch_msg += f"Loss: {loss.data:.3f}"
@@ -313,79 +332,74 @@
                             epoch_msg += f"Loss: {loss.data:.3f}"
                             self.cprint("[INFO]", self.color_dgreen, epoch_msg)
                         else:
                             self.cprint("[INFO]", self.color_dgreen, epoch_msg)
                     # --- END: one batch
 
                 # scheduler
-                if phase.lower() in train_phase_names and (
-                    self.scheduler is not None
-                ):
+                if phase.lower() in train_phase_names and (self.scheduler is not None):
                     self.scheduler.step()
 
                 if phase.lower() in train_phase_names + valid_phase_names:
                     # --- collect statistics
-                    epoch_loss = running_loss / self.dataset_sizes[phase]
+                    epoch_loss = running_loss / len(self.dataloaders[phase].dataset)
                     self._add_metrics(f"epoch_loss_{phase}", epoch_loss)
 
                     if tboard_writer is not None:
                         tboard_writer.add_scalar(
                             f"loss/{phase}",
                             self.metrics[f"epoch_loss_{phase}"][-1],
                             epoch,
                         )
 
                     # other metrics (precision/recall/F1)
                     self.calculate_add_metrics(
-                        running_orig_label,
-                        running_pred_label,
+                        running_orig_label_indices,
+                        running_pred_label_indices,
                         running_pred_conf,
                         phase,
                         epoch,
                         tboard_writer,
                     )
 
                     epoch_msg = f"{phase: <8} -- {epoch}/{end_epoch} -- "
                     epoch_msg = self.gen_epoch_msg(phase, epoch_msg)
 
                     if phase.lower() in valid_phase_names:
-                        self.cprint(
-                            "[INFO]", self.color_dred, epoch_msg + "\n"
-                        )
+                        self.cprint("[INFO]", self.color_dred, epoch_msg + "\n")
                     else:
                         self.cprint("[INFO]", self.color_dgreen, epoch_msg)
 
                 # labels/confidence
                 self.pred_conf.extend(running_pred_conf)
-                self.pred_label.extend(running_pred_label)
-                self.orig_label.extend(running_orig_label)
+                self.pred_label_indices.extend(running_pred_label_indices)
+                self.orig_label_indices.extend(running_orig_label_indices)
 
                 # Update best_loss and _epoch?
-                if (
-                    phase.lower() in valid_phase_names
-                    and epoch_loss < self.best_loss
-                ):
+                if phase.lower() in valid_phase_names and epoch_loss < self.best_loss:
                     self.best_loss = epoch_loss
                     self.best_epoch = epoch
                     best_model_wts = copy.deepcopy(self.model.state_dict())
 
                 if phase.lower() in valid_phase_names:
                     if epoch % tmp_file_save_freq == 0:
-                        print(
-                            f"SAVE temp file: {self.tmp_save_filename} | set .last_epoch: {epoch}"  # noqa
-                        )
-                        tmp_str = f"[INFO] SAVE temp file: {self.tmp_save_filename} | set .last_epoch: {epoch}\n"  # noqa
+                        tmp_str = f'[INFO] Checkpoint file saved to "{self.tmp_save_filename}".'  # noqa
                         print(self.color_lgrey + tmp_str + self.color_reset)
                         self.last_epoch = epoch
                         self.save(self.tmp_save_filename, force=True)
 
+        self.pred_label = [
+            self.labels_map.get(i, None) for i in self.pred_label_indices
+        ]
+        self.orig_label = [
+            self.labels_map.get(i, None) for i in self.orig_label_indices
+        ]
+
         time_elapsed = time.time() - since
-        print(
-            f"Total time: {time_elapsed // 60:.0f}m {time_elapsed % 60:.0f}s"
-        )
+        print(f"[INFO] Total time: {time_elapsed // 60:.0f}m {time_elapsed % 60:.0f}s")
 
         # load best model weights
         self.model.load_state_dict(best_model_wts)
 
         # --- SAVE model/object
         if phase.lower() in train_phase_names + valid_phase_names:
             self.last_epoch = epoch
@@ -394,17 +408,17 @@
                 save_model_path = os.path.join(save_model_dir, save_filename)
                 self.save(save_model_path, force=True)
                 info_path = os.path.join(save_model_dir, "info.txt")
                 with open(info_path, "a+") as f:
                     f.writelines(f"{save_filename},{self.best_loss:.5f}\n")
 
                 print(
-                    f"[INFO] Save model epoch: {self.best_epoch} with least valid loss: {self.best_loss:.4f}"  # noqa
-                )
-                print(f"[INFO] Path: {save_model_path}")
+                    f"[INFO] Model at epoch {self.best_epoch} has least valid loss ({self.best_loss:.4f}) so will be saved.\n\
+[INFO] Path: {save_model_path}"
+                )  # noqa
 
     def show_sample(
         self,
         set_name: Optional[str] = "train",
         batch_number: Optional[int] = 1,
         print_batch_info: Optional[bool] = True,
         figsize: Optional[Tuple[int, int]] = (15, 10),
@@ -440,121 +454,134 @@
         Notes
         -----
         This method uses the dataloader of the ``ImageClassifierData`` class
         and the ``torchvision.utils.make_grid`` function to display the sample
         data in a grid format. It also calls the ``_imshow`` method of the
         ``ImageClassifierData`` class to show the sample data.
         """
+        if set_name not in self.dataloaders.keys():
+            raise ValueError(
+                f"[ERROR] ``set_name`` must be one of {list(self.dataloaders.keys())}."
+            )
+
         if print_batch_info:
             # print info about batch size
             self.batch_info()
 
-        dl_iter = iter(self.dataloader[set_name])
+        dataloader = self.dataloaders[set_name]
+
+        num_batches = int(np.ceil(len(dataloader.dataset) / dataloader.batch_size))
+        if min(num_batches, batch_number) != batch_number:
+            print(
+                f'[INFO] "{set_name}" only contains {num_batches}.\n\
+Output will show batch number {num_batches}.'
+            )
+            batch_number = num_batches
+
+        dl_iter = iter(dataloader)
         for _ in range(batch_number):
             # Get a batch of training data
-            inputs1, inputs2, classes = next(dl_iter)
+            inputs1, inputs2, labels, label_indices = next(dl_iter)
 
         # Make a grid from batch
         out = torchvision.utils.make_grid(inputs1)
         self._imshow(
             out,
-            title=str([self.class_names[int(x)] for x in classes]),
+            title=f"{labels}\n{label_indices.tolist()}",
             figsize=figsize,
         )
 
         out = torchvision.utils.make_grid(inputs2)
         self._imshow(
             out,
-            title=str([self.class_names[int(x)] for x in classes]),
+            title=f"{labels}\n{label_indices.tolist()}",
             figsize=figsize,
         )
 
-    def layerwise_lr(
+    def generate_layerwise_lrs(
         self,
         min_lr: float,
         max_lr: float,
-        ltype: Optional[str] = "linspace",
+        spacing: Optional[str] = "linspace",
         sep_group_names: List[str] = ["features1", "features2"],
     ) -> List[Dict]:
         """
         Calculates layer-wise learning rates for a given set of model
         parameters.
 
         Parameters
         ----------
         min_lr : float
             The minimum learning rate to be used.
         max_lr : float
             The maximum learning rate to be used.
-        ltype : str, optional
+        spacing : str, optional
             The type of sequence to use for spacing the specified interval
             learning rates. Can be either ``"linspace"`` or ``"geomspace"``,
             where `"linspace"` uses evenly spaced learning rates over a
             specified interval and `"geomspace"` uses learning rates spaced
-            evenly on a log scale (a geometric progression). Defaults to
-            ``"linspace"``.
+            evenly on a log scale (a geometric progression). By default ``"linspace"``.
         sep_group_names : list, optional
             A list of strings containing the names of parameter groups. Layers
             belonging to each group will be assigned the same learning rate.
             Defaults to ``["features1", "features2"]``.
 
         Returns
         -------
         list of dicts
             A list of dictionaries containing the parameters and learning
             rates for each layer.
         """
-        list2optim = []
+        params2optimise = []
+
         for group in range(len(sep_group_names)):
             # count number of layers in this group
             num_grp_layers = 0
             for i, (name, params) in enumerate(self.model.named_parameters()):
                 if sep_group_names[group] in name:
                     num_grp_layers += 1
 
             # define layer-wise learning rates
-            if ltype.lower() in ["line", "linear", "linspace"]:
+            if spacing.lower() == "linspace":
                 list_lrs = np.linspace(min_lr, max_lr, num_grp_layers)
-            elif ltype.lower() in ["log", "geomspace"]:
+            elif spacing.lower() in ["log", "geomspace"]:
                 list_lrs = np.geomspace(min_lr, max_lr, num_grp_layers)
             else:
                 raise NotImplementedError(
-                    "Implemented methods are: linspace and geomspace"
+                    '[ERROR] ``spacing`` must be one of "linspace" or "geomspace"'
                 )
 
             # assign learning rates
             i_count = 0
             for _, (name, params) in enumerate(self.model.named_parameters()):
-                if not sep_group_names[group] in name:
+                if sep_group_names[group] not in name:
                     continue
-                list2optim.append({"params": params, "lr": list_lrs[i_count]})
+                params2optimise.append({"params": params, "lr": list_lrs[i_count]})
                 i_count += 1
 
-        return list2optim
+        return params2optimise
 
-    def inference_sample_results(
+    def show_inference_sample_results(
         self,
+        label: str,
         num_samples: Optional[int] = 6,
-        class_index: Optional[int] = 0,
         set_name: Optional[str] = "train",
         min_conf: Optional[Union[None, float]] = None,
         max_conf: Optional[Union[None, float]] = None,
         figsize: Optional[Tuple[int, int]] = (15, 15),
     ) -> None:
         """
-        Performs inference on a given dataset and displays results for a
-        specified class.
+        Shows a sample of the results of the inference.
 
         Parameters
         ----------
+        label : str, optional
+            The label for which to display results.
         num_samples : int, optional
             The number of sample results to display. Defaults to ``6``.
-        class_index : int, optional
-            The index of the class for which to display results. Defaults to
-            ``0``.
         set_name : str, optional
             The name of the dataset split to use for inference. Defaults to
             ``"train"``.
         min_conf : float, optional
             The minimum confidence score for a sample result to be displayed.
             Samples with lower confidence scores will be skipped. Defaults to
             ``None``.
@@ -571,48 +598,59 @@
         None
         """
 
         # eval mode, keep track of the current mode
         was_training = self.model.training
         self.model.eval()
 
-        fig = plt.figure(figsize=figsize)
-
         counter = 0
+        plt.figure(figsize=figsize)
         with torch.no_grad():
-            for inputs1, inputs2, labels in iter(self.dataloader[set_name]):
+            for inputs1, inputs2, labels, label_indices in iter(
+                self.dataloaders[set_name]
+            ):
                 inputs1 = inputs1.to(self.device)
-                labels = labels.to(self.device)
                 inputs2 = inputs2.to(self.device)
+                label_indices = label_indices.to(self.device)
 
                 outputs = self.model(inputs1, inputs2)
+
+                if not isinstance(outputs, torch.Tensor):
+                    try:
+                        outputs = outputs.logits
+                    except AttributeError as err:
+                        raise AttributeError(err.message)
+
                 pred_conf = torch.nn.functional.softmax(outputs, dim=1) * 100.0
                 _, preds = torch.max(outputs, 1)
 
+                label_index_dict = {
+                    label: index for label, index in zip(labels, label_indices)
+                }
+
                 # go through images in batch
                 for j in range(len(preds)):
-                    pred_ind = int(preds[j])
-                    if pred_ind != class_index:
+                    predicted_index = int(preds[j])
+                    if predicted_index != label_index_dict[label]:
                         continue
                     if (min_conf is not None) and (
-                        pred_conf[j][pred_ind] < min_conf
+                        pred_conf[j][predicted_index] < min_conf
                     ):
                         continue
                     if (max_conf is not None) and (
-                        pred_conf[j][pred_ind] > max_conf
+                        pred_conf[j][predicted_index] > max_conf
                     ):
                         continue
 
                     counter += 1
 
-                    class_name = self.class_names[pred_ind]
-                    conf_score = pred_conf[j][pred_ind]
+                    conf_score = pred_conf[j][predicted_index]
                     ax = plt.subplot(int(num_samples / 2.0), 3, counter)
                     ax.axis("off")
-                    ax.set_title(f"{class_name} | {conf_score:.3f}")
+                    ax.set_title(f"{label} | {conf_score:.3f}")
 
                     inp = inputs1.cpu().data[j].numpy().transpose((1, 2, 0))
                     inp = np.clip(inp, 0, 1)
                     plt.imshow(inp)
 
                     if counter == num_samples:
                         self.model.train(mode=was_training)
```

### Comparing `mapreader-0.3.4/mapreader/train/custom_models.py` & `mapreader-1.0.1.post0.dev9/mapreader/classify/custom_models.py`

 * *Files identical despite different names*

### Comparing `mapreader-0.3.4/mapreader/utils/compute_and_save_stats.py` & `mapreader-1.0.1.post0.dev9/mapreader/utils/compute_and_save_stats.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 from mapreader import load_patches
 from parhugin import multiFunc
 
 
 def save_stats(one_dir):
     mymaps = load_patches(
-        os.path.join(one_dir, "slice_50_50", "*png"),
+        os.path.join(one_dir, "patch_50_50", "*png"),
         parent_paths=os.path.join(one_dir, "*png"),
     )
 
     path2metadata = os.path.join(one_dir, "metadata.csv")
     mymaps.add_metadata(metadata=path2metadata)
     mymaps.add_center_coord()
     mymaps.calc_pixel_stats()
-    pd_parent, pd_child = mymaps.convertImages()
-    pd_parent.to_csv(os.path.join(one_dir, "pd_parent.csv"), mode="w", header=True)
-    pd_child.to_csv(os.path.join(one_dir, "pd_child.csv"), mode="w", header=True)
+    parent_df, patch_df = mymaps.convertImages()
+    parent_df.to_csv(os.path.join(one_dir, "parent_df.csv"), mode="w", header=True)
+    patch_df.to_csv(os.path.join(one_dir, "patch_df.csv"), mode="w", header=True)
 
 
 list_dirs = glob("/maps_large/2021_experiments_1inch/chunks_*")
 
 myproc = multiFunc(num_req_p=10)
 
 list_jobs = []
```

### Comparing `mapreader-0.3.4/mapreader/utils/geo_utils.py` & `mapreader-1.0.1.post0.dev9/mapreader/load/geo_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Returns
     -------
     list
         shape, CRS, coord
     """
     # read the image using rasterio
     tiff_src = rasterio.open(image_path)
-    image_height, image_width = tiff_src.shape
+    image_height, image_width = tiff_src.height, tiff_src.width
     image_channels = tiff_src.count
     tiff_shape = (image_height, image_width, image_channels)
 
     # check coordinates are present
     if isinstance(tiff_src.crs, type(None)):
         raise ValueError(f"No coordinates found in {image_path}")
     else:
@@ -35,78 +35,71 @@
 
     print(f"[INFO] Shape: {tiff_shape}. \n[INFO] CRS: {tiff_proj}.")
     print("[INFO] Coordinates: %.4f %.4f %.4f %.4f" % tiff_coord)
 
     return tiff_shape, tiff_proj, tiff_coord
 
 
-def reprojectGeoInfo(image_path, proj2convert="EPSG:4326", calc_size_in_m=False):
-    """Extract geographic information from GeoTiff files and reproject to specified CRS (`proj2convert`).
+def reproject_geo_info(image_path, target_crs="EPSG:4326", calc_size_in_m=False):
+    """Extract geographic information from GeoTiff files and reproject to specified CRS (`target_crs`).
 
     Parameters
     ----------
     image_path : str
         Path to image
-    proj2convert : str, optional
+    target_crs : str, optional
         Projection to convert coordinates into, by default "EPSG:4326"
     calc_size_in_m : str or bool, optional
         Method to compute pixel widths and heights, choices between "geodesic" and "great-circle" or "gc", by default "great-circle", by default False
 
     Returns
     -------
     list
         shape, old CRS, new CRS, reprojected coord, size in meters
     """
     tiff_shape, tiff_proj, tiff_coord = extractGeoInfo(image_path)
 
     # Coordinate transformation: proj1 ---> proj2
-    transformer = Transformer.from_crs(tiff_proj, proj2convert)
-    ymax, xmin = transformer.transform(tiff_coord[0], tiff_coord[3])
-    ymin, xmax = transformer.transform(tiff_coord[2], tiff_coord[1])
-    coord = (xmin, xmax, ymin, ymax)
+    transformer = Transformer.from_crs(tiff_proj, target_crs)
+    ymin, xmin = transformer.transform(
+        tiff_coord[0], tiff_coord[1]
+    )
+    ymax, xmax = transformer.transform(
+        tiff_coord[2], tiff_coord[3]
+    )
+    coord = (xmin, ymin, xmax, ymax)
 
-    print(f"[INFO] New CRS: {proj2convert}")
+    print(f"[INFO] New CRS: {target_crs}")
     print("[INFO] Reprojected coordinates: %.4f %.4f %.4f %.4f" % coord)
 
+    height, width, _ = tiff_shape
+
     # Calculate the size of image in meters
-    if calc_size_in_m == "geodesic":
+    if calc_size_in_m in ["geodesic", "gd"]:
         bottom = geodesic((ymin, xmin), (ymin, xmax)).meters
         right = geodesic((ymin, xmax), (ymax, xmax)).meters
         top = geodesic((ymax, xmax), (ymax, xmin)).meters
         left = geodesic((ymax, xmin), (ymin, xmin)).meters
-        size_in_m = (bottom, top, left, right)
-        print(
-            f"[INFO] size (in meters) bottom/top/left/right: {bottom:.2f}/{top:.2f}/{left:.2f}/{right:.2f}"
-        )
 
-        mean_width = np.mean(
-            [size_in_m[0] / tiff_shape[2], size_in_m[1] / tiff_shape[2]]
-        )
-        mean_height = np.mean(
-            [size_in_m[2] / tiff_shape[1], size_in_m[3] / tiff_shape[1]]
-        )
-        print(
-            f"Each pixel is ~{mean_width:.3f} X {mean_height:.3f} meters (width x height)."
-        )
-    elif calc_size_in_m in ["gc", "great-circle"]:
+    elif calc_size_in_m in ["gc", "great-circle", "great_circle"]:
         bottom = great_circle((ymin, xmin), (ymin, xmax)).meters
         right = great_circle((ymin, xmax), (ymax, xmax)).meters
         top = great_circle((ymax, xmax), (ymax, xmin)).meters
         left = great_circle((ymax, xmin), (ymin, xmin)).meters
-        size_in_m = (bottom, top, left, right)
-        print(
-            f"[INFO] size (in meters) bottom/top/left/right: {bottom:.2f}/{top:.2f}/{left:.2f}/{right:.2f}"
-        )
 
-        mean_width = np.mean(
-            [size_in_m[0] / tiff_shape[2], size_in_m[1] / tiff_shape[2]]
-        )
-        mean_height = np.mean(
-            [size_in_m[2] / tiff_shape[1], size_in_m[3] / tiff_shape[1]]
-        )
-        print(
-            f"Each pixel is ~{mean_width:.3f} x {mean_height:.3f} meters (width x height)."
-        )
-    else:
+    elif not calc_size_in_m:
         size_in_m = False
+    
+    else:
+        raise NotImplementedError(
+            f'[ERROR] ``calc_size_in_m`` must be one of "great-circle", "great_cirlce", "gc", "geodesic" or "gd", not: {calc_size_in_m}'
+        )
+
+    size_in_m = (left, bottom, right, top)  # anticlockwise order
+
+    mean_pixel_height = np.mean([right / height, left / height])
+    mean_pixel_width = np.mean([bottom / width, top / width])
+
+    print(f"[INFO] Size in meters of left/bottom/right/top: {left:.2f}/{bottom:.2f}/{right:.2f}/{top:.2f}")
+    print(f"Each pixel is ~{mean_pixel_height:.3f} X {mean_pixel_width:.3f} meters (height x width).")  # noqa
 
-    return tiff_shape, tiff_proj, proj2convert, coord, size_in_m
+    return tiff_shape, tiff_proj, target_crs, coord, size_in_m
```

### Comparing `mapreader-0.3.4/mapreader/utils/slice_parallel.py` & `mapreader-1.0.1.post0.dev9/mapreader/utils/slice_parallel.py`

 * *Files identical despite different names*

### Comparing `mapreader-0.3.4/mapreader.egg-info/PKG-INFO` & `mapreader-1.0.1.post0.dev9/mapreader.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 0.3.4
+Version: 1.0.1.post0.dev9
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
@@ -20,15 +20,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
     <br>
     <p align="center">
     <h1>MapReader</h1>
@@ -48,80 +48,79 @@
     </a>
     <br/>
 </p>
 
 
 ## What is MapReader?
 
-<!--- picture here? --->
-<p align="center">
-  <figure>
-  <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/figs/river_banner_8bit.png"
+<div align="center">
+    <figure>
+    <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/figs/river_banner_8bit.png"
         alt="Annotated Map with Prediction Outputs"
         width="70%">
-  </figure>
-</p>
+    </figure>
+</div>
 
 MapReader is an end-to-end computer vision (CV) pipeline for exploring and analyzing images at scale. 
 
-MapReader was developed in the [Living with Machines](https://livingwithmachines.ac.uk/) project to analyze large collections of historical maps but is a _**generalisable**_ computer vision pipeline which can be applied to _**any images**_ in a wide variety of domains. 
+MapReader was developed in the [Living with Machines](https://livingwithmachines.ac.uk/) project to analyze large collections of historical maps but is a _**generalizable**_ computer vision pipeline which can be applied to _**any images**_ in a wide variety of domains. 
 
 
 ## Overview
 
-MapReader is a groundbreaking interdisciplinary tool that emerged from a specific set of geospatial historical research questions. It was inspired by methods in biomedical imaging and geographic information science, which were adapted for annotation and use by historians, for example in [JVC](https://doi.org/10.1093/jvcult/vcab009) and [MapReader](https://arxiv.org/abs/2111.15592) papers. The success of the tool subsequently generated interest from plant phenotype researchers working with large image datasets, and so MapReader is an example of cross-pollination between the humanities and the sciences made possible by reproducible data science.
+MapReader is a groundbreaking interdisciplinary tool that emerged from a specific set of geospatial historical research questions. It was inspired by methods in biomedical imaging and geographic information science, which were adapted for use by historians, for example in our [Journal of Victorian Culture](https://doi.org/10.1093/jvcult/vcab009) and [Geospatial Humanities 2022 SIGSPATIAL workshop](https://arxiv.org/abs/2111.15592) papers. The success of the tool subsequently generated interest from plant phenotype researchers working with large image datasets, and so MapReader is an example of cross-pollination between the humanities and the sciences made possible by reproducible data science.
 
 ### MapReader pipeline 
 
-The MapReader pipeline consists of two main components:
-1. preprocessing/annotation 
-2. training/inference
-
-<p align="center">
+<div align="center">
   <figure>
-  <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/figs/MapReader_pipeline.png"
+  <img src="https://raw.githubusercontent.com/Living-with-machines/MapReader/main/docs/source/figures/pipeline_explained.png"
         alt="MapReader pipeline"
         width="70%">
   </figure>
-</p>
-
-
-### What is included?
-
-The MapReader package provides a set of tools to:
+</div>
 
-- **download** images/maps and metadata stored on web-servers (e.g. tileserves which can be used to retrieve maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or elsewhere).
-- **load** images/maps and metadata stored locally.
-- **preprocess** images/maps:
-  - patchify (create patches from a parent image), 
-  - resample (use image transformations to alter pixel-dimensions/resolution/orientation/etc.),
-  - remove borders outside the neatline,
-  - reproject between coordinate reference systems (CRS).
-- **annotate** images/maps (or their patches) using an interactive annotation tool.
-- **train, fine-tune, and evaluate** Computer Vision (CV) models and use these to **predict** labels (i.e. model inference) on large sets of images/maps.
+The MapReader pipeline consists of a linear sequence of tasks which, together, can be used to train a computer vision (CV) classifier to recognise visual features within maps and identify patches containing these features across entire map collections.
 
-Various **plotting and analysis** functionalities are also included (based on packages such as *matplotlib*, *cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)).
+See our [About MapReader](https://mapreader.readthedocs.io/en/latest/About.html) page to learn more.
 
-<!--- or mb picture here? --->
 
 ## Documentation 
 
-The MapReader documentation can be found [here](https://mapreader.readthedocs.io/en/latest/index.html).
+The MapReader documentation can be found at https://mapreader.readthedocs.io/en/latest/index.html.
 
-**New users** should refer to the [Installation instructions](https://mapreader.readthedocs.io/en/latest/Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/Input-guidance.html) for guidance on the initial set up of MapReader.
+**New users** should refer to the [Installation instructions](https://mapreader.readthedocs.io/en/latest/Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/Input-guidance.html) for help with the initial set up of MapReader.
 
-**All users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/latest/User-guide.html) for guidance on how to use MapReader. This contains end-to-end instructions on how to use the MapReader pipeline, plus a number of worked examples illustratng use cases such as:
+**All users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/latest/User-guide/User-guide.html) for guidance on how to use MapReader. This contains end-to-end instructions on how to use the MapReader pipeline, plus a number of worked examples illustratng use cases such as:
 - Geospatial images (i.e. maps)
 - Non-geospatial images 
 
  **Developers and contributors** may also want to refer to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how to contribute to the MapReader package.
+ 
+ 
+## What is included in this repo?
+
+The MapReader package provides a set of tools to:
+
+- **Download** images/maps and metadata stored on web-servers (e.g. tileserves which can be used to retrieve maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or elsewhere).
+- **Load** images/maps and metadata stored locally.
+- **Preprocess** images/maps:
+  - patchify (create patches from a parent image), 
+  - resample (use image transformations to alter pixel-dimensions/resolution/orientation/etc.),
+  - remove borders outside the neatline,
+  - reproject between coordinate reference systems (CRS).
+- **Annotate** images/maps (or their patches) using an interactive annotation tool.
+- **Train or fine-tune** Computer Vision (CV) models and use these to **predict** labels (i.e. model inference) on large sets of images/maps.
+
+Various **plotting and analysis** functionalities are also included (based on packages such as *matplotlib*, *cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)).
+
 
 ## How to cite MapReader
 
-If you use MapReader in your work, please consider acknowledging us by citing [our paper](https://dl.acm.org/doi/10.1145/3557919.3565812):
+If you use MapReader in your work, please consider acknowledging us by citing [our SIGSPATIAL paper](https://dl.acm.org/doi/10.1145/3557919.3565812):
 
 - Kasra Hosseini, Daniel C. S. Wilson, Kaspar Beelen, and Katherine McDonough. 2022. MapReader: a computer vision pipeline for the semantic exploration of maps at scale. In Proceedings of the 6th ACM SIGSPATIAL International Workshop on Geospatial Humanities (GeoHumanities '22). Association for Computing Machinery, New York, NY, USA, 8–19. https://doi.org/10.1145/3557919.3565812
 
 
 ## Acknowledgements
 
 This work was supported by Living with Machines (AHRC grant AH/S01179X/1) and The Alan Turing Institute (EPSRC grant EP/N510129/1).
```

#### html2text {}

```diff
@@ -1,79 +1,84 @@
-Metadata-Version: 2.1 Name: mapreader Version: 0.3.4 Summary: A computer vision
-pipeline for the semantic exploration of maps/images at scale Home-page: https:
-//github.com/Living-with-machines/MapReader Download-URL: https://github.com/
-Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
-team License: MIT License Keywords: Computer Vision,Classification,Deep
-Learning,living with machines Platform: OS Independent Classifier: Development
-Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Intended Audience :: End Users/Desktop Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: Science/Research Classifier: Operating System :: Unix Classifier:
-Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
-Classifier: Operating System :: OS Independent Classifier: Topic :: Software
-Development Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: mapreader Version: 1.0.1.post0.dev9 Summary: A
+computer vision pipeline for the semantic exploration of maps/images at scale
+Home-page: https://github.com/Living-with-machines/MapReader Download-URL:
+https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
+Author: MapReader team License: MIT License Keywords: Computer
+Vision,Classification,Deep Learning,living with machines Platform: OS
+Independent Classifier: Development Status :: 3 - Alpha Classifier: License ::
+OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Intended Audience :: End Users/Desktop Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research Classifier: Operating System
+:: Unix Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: MacOS Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Requires-Python: >=3.7, <3.11
+Description-Content-Type: text/markdown License-File: LICENSE
 
                             ****** MapReader ******
  ***** A computer vision pipeline for exploring and analyzing images at scale
                                      *****
                   [PyPI] [License] [Integration_Tests_badge]
 ## What is MapReader?
                     [Annotated Map with Prediction Outputs]
 MapReader is an end-to-end computer vision (CV) pipeline for exploring and
 analyzing images at scale. MapReader was developed in the [Living with
 Machines](https://livingwithmachines.ac.uk/) project to analyze large
-collections of historical maps but is a _**generalisable**_ computer vision
+collections of historical maps but is a _**generalizable**_ computer vision
 pipeline which can be applied to _**any images**_ in a wide variety of domains.
 ## Overview MapReader is a groundbreaking interdisciplinary tool that emerged
 from a specific set of geospatial historical research questions. It was
 inspired by methods in biomedical imaging and geographic information science,
-which were adapted for annotation and use by historians, for example in [JVC]
-(https://doi.org/10.1093/jvcult/vcab009) and [MapReader](https://arxiv.org/abs/
-2111.15592) papers. The success of the tool subsequently generated interest
-from plant phenotype researchers working with large image datasets, and so
-MapReader is an example of cross-pollination between the humanities and the
-sciences made possible by reproducible data science. ### MapReader pipeline The
-MapReader pipeline consists of two main components: 1. preprocessing/annotation
-2. training/inference
+which were adapted for use by historians, for example in our [Journal of
+Victorian Culture](https://doi.org/10.1093/jvcult/vcab009) and [Geospatial
+Humanities 2022 SIGSPATIAL workshop](https://arxiv.org/abs/2111.15592) papers.
+The success of the tool subsequently generated interest from plant phenotype
+researchers working with large image datasets, and so MapReader is an example
+of cross-pollination between the humanities and the sciences made possible by
+reproducible data science. ### MapReader pipeline
                              [MapReader pipeline]
-### What is included? The MapReader package provides a set of tools to: -
-**download** images/maps and metadata stored on web-servers (e.g. tileserves
-which can be used to retrieve maps from OpenStreetMap (OSM), the National
-Library of Scotland (NLS), or elsewhere). - **load** images/maps and metadata
-stored locally. - **preprocess** images/maps: - patchify (create patches from a
-parent image), - resample (use image transformations to alter pixel-dimensions/
-resolution/orientation/etc.), - remove borders outside the neatline, -
-reproject between coordinate reference systems (CRS). - **annotate** images/
-maps (or their patches) using an interactive annotation tool. - **train, fine-
-tune, and evaluate** Computer Vision (CV) models and use these to **predict**
-labels (i.e. model inference) on large sets of images/maps. Various **plotting
-and analysis** functionalities are also included (based on packages such as
-*matplotlib*, *cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)).
-## Documentation The MapReader documentation can be found [here](https://
-mapreader.readthedocs.io/en/latest/index.html). **New users** should refer to
+The MapReader pipeline consists of a linear sequence of tasks which, together,
+can be used to train a computer vision (CV) classifier to recognise visual
+features within maps and identify patches containing these features across
+entire map collections. See our [About MapReader](https://
+mapreader.readthedocs.io/en/latest/About.html) page to learn more. ##
+Documentation The MapReader documentation can be found at https://
+mapreader.readthedocs.io/en/latest/index.html. **New users** should refer to
 the [Installation instructions](https://mapreader.readthedocs.io/en/latest/
 Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/
-Input-guidance.html) for guidance on the initial set up of MapReader. **All
+Input-guidance.html) for help with the initial set up of MapReader. **All
 users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/
-latest/User-guide.html) for guidance on how to use MapReader. This contains
-end-to-end instructions on how to use the MapReader pipeline, plus a number of
-worked examples illustratng use cases such as: - Geospatial images (i.e. maps)
-- Non-geospatial images **Developers and contributors** may also want to refer
-to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/
-index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/
-latest/Contribution-guide.html) for guidance on how to contribute to the
-MapReader package. ## How to cite MapReader If you use MapReader in your work,
-please consider acknowledging us by citing [our paper](https://dl.acm.org/doi/
-10.1145/3557919.3565812): - Kasra Hosseini, Daniel C. S. Wilson, Kaspar Beelen,
-and Katherine McDonough. 2022. MapReader: a computer vision pipeline for the
+latest/User-guide/User-guide.html) for guidance on how to use MapReader. This
+contains end-to-end instructions on how to use the MapReader pipeline, plus a
+number of worked examples illustratng use cases such as: - Geospatial images
+(i.e. maps) - Non-geospatial images **Developers and contributors** may also
+want to refer to the [API documentation](https://mapreader.readthedocs.io/en/
+latest/api/index.html) and [Contribution guide](https://
+mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how
+to contribute to the MapReader package. ## What is included in this repo? The
+MapReader package provides a set of tools to: - **Download** images/maps and
+metadata stored on web-servers (e.g. tileserves which can be used to retrieve
+maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or
+elsewhere). - **Load** images/maps and metadata stored locally. -
+**Preprocess** images/maps: - patchify (create patches from a parent image), -
+resample (use image transformations to alter pixel-dimensions/resolution/
+orientation/etc.), - remove borders outside the neatline, - reproject between
+coordinate reference systems (CRS). - **Annotate** images/maps (or their
+patches) using an interactive annotation tool. - **Train or fine-tune**
+Computer Vision (CV) models and use these to **predict** labels (i.e. model
+inference) on large sets of images/maps. Various **plotting and analysis**
+functionalities are also included (based on packages such as *matplotlib*,
+*cartopy*, *Google Earth*, and [kepler.gl](https://kepler.gl/)). ## How to cite
+MapReader If you use MapReader in your work, please consider acknowledging us
+by citing [our SIGSPATIAL paper](https://dl.acm.org/doi/10.1145/
+3557919.3565812): - Kasra Hosseini, Daniel C. S. Wilson, Kaspar Beelen, and
+Katherine McDonough. 2022. MapReader: a computer vision pipeline for the
 semantic exploration of maps at scale. In Proceedings of the 6th ACM SIGSPATIAL
 International Workshop on Geospatial Humanities (GeoHumanities '22).
 Association for Computing Machinery, New York, NY, USA, 8â19. https://
 doi.org/10.1145/3557919.3565812 ## Acknowledgements This work was supported by
 Living with Machines (AHRC grant AH/S01179X/1) and The Alan Turing Institute
 (EPSRC grant EP/N510129/1). Living with Machines, funded by the UK Research and
 Innovation (UKRI) Strategic Priority Fund, is a multidisciplinary collaboration
```

### Comparing `mapreader-0.3.4/mapreader.egg-info/SOURCES.txt` & `mapreader-1.0.1.post0.dev9/mapreader.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
+versioneer.py
 mapreader/__init__.py
+mapreader/_version.py
 mapreader.egg-info/PKG-INFO
 mapreader.egg-info/SOURCES.txt
 mapreader.egg-info/dependency_links.txt
 mapreader.egg-info/entry_points.txt
 mapreader.egg-info/not-zip-safe
 mapreader.egg-info/requires.txt
 mapreader.egg-info/top_level.txt
 mapreader/annotate/__init__.py
-mapreader/annotate/load_annotate.py
 mapreader/annotate/utils.py
+mapreader/classify/__init__.py
+mapreader/classify/classifier.py
+mapreader/classify/classifier_context.py
+mapreader/classify/custom_models.py
+mapreader/classify/datasets.py
+mapreader/classify/load_annotations.py
 mapreader/download/__init__.py
-mapreader/download/azure_access.py
-mapreader/download/tileserver_access.py
-mapreader/download/tileserver_helpers.py
-mapreader/download/tileserver_scraper.py
-mapreader/download/tileserver_stitcher.py
-mapreader/loader/__init__.py
-mapreader/loader/images.py
-mapreader/loader/loader.py
+mapreader/download/data_structures.py
+mapreader/download/downloader.py
+mapreader/download/downloader_utils.py
+mapreader/download/sheet_downloader.py
+mapreader/download/tile_loading.py
+mapreader/download/tile_merging.py
+mapreader/load/__init__.py
+mapreader/load/geo_utils.py
+mapreader/load/images.py
+mapreader/load/loader.py
 mapreader/process/__init__.py
 mapreader/process/process.py
-mapreader/slicers/__init__.py
-mapreader/slicers/slicers.py
-mapreader/train/__init__.py
-mapreader/train/classifier.py
-mapreader/train/classifier_context.py
-mapreader/train/custom_models.py
-mapreader/train/datasets.py
 mapreader/utils/__init__.py
 mapreader/utils/compute_and_save_stats.py
-mapreader/utils/geo_utils.py
 mapreader/utils/slice_parallel.py
-tests/test_geo_utils.py
+tests/test_annotations_loader.py
+tests/test_classifier.py
 tests/test_import.py
-tests/test_loader.py
-tests/test_non_geo_pipeline.py
+tests/test_sheet_downloader.py
```

### Comparing `mapreader-0.3.4/mapreader.egg-info/requires.txt` & `mapreader-1.0.1.post0.dev9/mapreader.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 matplotlib<4.0.0,>=3.5.0
 numpy<2.0.0,>=1.21.5
 pandas<2.0.0,>=1.3.4
 pyproj<4.0.0,>=3.2.0
 azure-storage-blob<13.0.0,>=12.9.0
 aiohttp<4.0.0,>=3.8.1
-Shapely<2.0.0,>=1.8.0
+Shapely<3.0.0,>=2.0.0
 nest-asyncio<2.0.0,>=1.5.1
 scikit-image>=0.18.3
 scikit-learn<2.0.0,>=1.0.1
 torch<2.0.0,>=1.10.0
 torchvision<0.12.1,>=0.11.1
 jupyter<2.0.0,>=1.0.0
 ipykernel<7.0.0,>=6.5.1
@@ -18,7 +18,11 @@
 PyYAML<7.0,>=6.0
 tensorboard<3.0.0,>=2.7.0
 parhugin<0.0.4,>=0.0.3
 geopy==2.1.0
 rasterio<2.0.0,>=1.2.10
 keplergl<0.4.0,>=0.3.2
 simplekml<2.0.0,>=1.3.6
+versioneer>=0.28
+tqdm
+torchinfo
+openpyxl
```

### Comparing `mapreader-0.3.4/setup.py` & `mapreader-1.0.1.post0.dev9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 import setuptools
+import versioneer
+
 
 setuptools.setup(
     name="mapreader",
-    version="0.3.4",
+    version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
     description="A computer vision pipeline for the semantic exploration of maps/images at scale",
     author=u"MapReader team",
     #author_email="",
     license="MIT License",
     keywords=["Computer Vision", "Classification", "Deep Learning", "living with machines"],
     long_description = open('README.md', encoding="utf8").read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
     url="https://github.com/Living-with-machines/MapReader",
     download_url="https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip",
     packages = setuptools.find_packages(),
     include_package_data = True,
     platforms="OS Independent",
-    python_requires='>=3.7',
+    python_requires='>=3.7, <3.11',
     install_requires=[
         "matplotlib>=3.5.0,<4.0.0",
         "numpy>=1.21.5,<2.0.0",
         "pandas>=1.3.4,<2.0.0",
         "pyproj>=3.2.0,<4.0.0",
         "azure-storage-blob>=12.9.0,<13.0.0",
         "aiohttp>=3.8.1,<4.0.0",
-        "Shapely>=1.8.0,<2.0.0",
+        "Shapely>=2.0.0,<3.0.0",
         "nest-asyncio>=1.5.1,<2.0.0",
         "scikit-image>=0.18.3",
         "scikit-learn>=1.0.1,<2.0.0",
         "torch>=1.10.0,<2.0.0",
         "torchvision>=0.11.1,<0.12.1",
         "jupyter>=1.0.0,<2.0.0",
         "ipykernel>=6.5.1,<7.0.0",
         "ipywidgets>=7.7.3,<8.0.0",
         "ipyannotate==0.1.0-beta.0",
         "Cython>=0.29.24,<0.30.0",
+        # "proj>=0.2.0,<0.3.0",
         "PyYAML>=6.0,<7.0",
         "tensorboard>=2.7.0,<3.0.0",
         "parhugin>=0.0.3,<0.0.4",
         "geopy==2.1.0",
         "rasterio>=1.2.10,<2.0.0",
         "keplergl>=0.3.2,<0.4.0",
         "simplekml>=1.3.6,<2.0.0",
+        "versioneer>=0.28",
+        "tqdm",
+        "torchinfo",
+	    "openpyxl",
     ],
     
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
```

