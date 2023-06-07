# Comparing `tmp/ruspeechstress-0.6.tar.gz` & `tmp/ruspeechstress-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruspeechstress-0.6.tar", last modified: Wed Jun  7 16:12:24 2023, max compression
+gzip compressed data, was "ruspeechstress-0.7.tar", last modified: Wed Jun  7 16:14:08 2023, max compression
```

## Comparing `ruspeechstress-0.6.tar` & `ruspeechstress-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:12:24.395391 ruspeechstress-0.6/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:12:24.395391 ruspeechstress-0.6/PKG-INFO
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:12:24.391391 ruspeechstress-0.6/ruspeechstress/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      760 2023-06-07 16:12:22.000000 ruspeechstress-0.6/ruspeechstress/__init__.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    13250 2023-06-07 16:12:22.000000 ruspeechstress-0.6/ruspeechstress/dataset.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    31206 2023-06-07 09:32:56.000000 ruspeechstress-0.6/ruspeechstress/sound.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    18830 2023-06-07 16:12:22.000000 ruspeechstress-0.6/ruspeechstress/stress_detector.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)     1806 2021-06-01 18:24:40.000000 ruspeechstress-0.6/ruspeechstress/utils.py
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:12:24.391391 ruspeechstress-0.6/ruspeechstress.egg-info/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:12:24.000000 ruspeechstress-0.6/ruspeechstress.egg-info/PKG-INFO
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      295 2023-06-07 16:12:24.000000 ruspeechstress-0.6/ruspeechstress.egg-info/SOURCES.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)        1 2023-06-07 16:12:24.000000 ruspeechstress-0.6/ruspeechstress.egg-info/dependency_links.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)       15 2023-06-07 16:12:24.000000 ruspeechstress-0.6/ruspeechstress.egg-info/top_level.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)       38 2023-06-07 16:12:24.395391 ruspeechstress-0.6/setup.cfg
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      377 2023-06-07 16:12:22.000000 ruspeechstress-0.6/setup.py
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:14:08.422555 ruspeechstress-0.7/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:14:08.422555 ruspeechstress-0.7/PKG-INFO
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:14:08.422555 ruspeechstress-0.7/ruspeechstress/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      761 2023-06-07 16:13:56.000000 ruspeechstress-0.7/ruspeechstress/__init__.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    13250 2023-06-07 16:12:22.000000 ruspeechstress-0.7/ruspeechstress/dataset.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    31206 2023-06-07 09:32:56.000000 ruspeechstress-0.7/ruspeechstress/sound.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    18830 2023-06-07 16:12:22.000000 ruspeechstress-0.7/ruspeechstress/stress_detector.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)     1806 2021-06-01 18:24:40.000000 ruspeechstress-0.7/ruspeechstress/utils.py
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:14:08.422555 ruspeechstress-0.7/ruspeechstress.egg-info/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:14:08.000000 ruspeechstress-0.7/ruspeechstress.egg-info/PKG-INFO
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      295 2023-06-07 16:14:08.000000 ruspeechstress-0.7/ruspeechstress.egg-info/SOURCES.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)        1 2023-06-07 16:14:08.000000 ruspeechstress-0.7/ruspeechstress.egg-info/dependency_links.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)       15 2023-06-07 16:14:08.000000 ruspeechstress-0.7/ruspeechstress.egg-info/top_level.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)       38 2023-06-07 16:14:08.422555 ruspeechstress-0.7/setup.cfg
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      377 2023-06-07 16:13:56.000000 ruspeechstress-0.7/setup.py
```

### Comparing `ruspeechstress-0.6/ruspeechstress/__init__.py` & `ruspeechstress-0.7/ruspeechstress/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from .stress_detector import StressDetector, FEATURES
-from dataset import dataset
+from .dataset import dataset
 import numpy as np
 
 
 def create_dataset(working_dir=os.getcwd(), dictionary_path=None):
     dataset(working_dir=working_dir, dictionary_path=dictionary_path, mode='collect_dataset')
```

### Comparing `ruspeechstress-0.6/ruspeechstress/dataset.py` & `ruspeechstress-0.7/ruspeechstress/dataset.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.6/ruspeechstress/sound.py` & `ruspeechstress-0.7/ruspeechstress/sound.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.6/ruspeechstress/stress_detector.py` & `ruspeechstress-0.7/ruspeechstress/stress_detector.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.6/ruspeechstress/utils.py` & `ruspeechstress-0.7/ruspeechstress/utils.py`

 * *Files identical despite different names*

