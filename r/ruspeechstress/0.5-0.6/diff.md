# Comparing `tmp/ruspeechstress-0.5.tar.gz` & `tmp/ruspeechstress-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruspeechstress-0.5.tar", last modified: Wed Jun  7 16:09:13 2023, max compression
+gzip compressed data, was "ruspeechstress-0.6.tar", last modified: Wed Jun  7 16:12:24 2023, max compression
```

## Comparing `ruspeechstress-0.5.tar` & `ruspeechstress-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:09:13.356905 ruspeechstress-0.5/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:09:13.356905 ruspeechstress-0.5/PKG-INFO
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:09:13.352905 ruspeechstress-0.5/ruspeechstress/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      774 2023-06-07 16:08:57.000000 ruspeechstress-0.5/ruspeechstress/__init__.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    13249 2023-06-07 14:55:17.000000 ruspeechstress-0.5/ruspeechstress/dataset.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    31206 2023-06-07 09:32:56.000000 ruspeechstress-0.5/ruspeechstress/sound.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    18828 2023-06-07 09:27:32.000000 ruspeechstress-0.5/ruspeechstress/stress_detector.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)     1806 2021-06-01 18:24:40.000000 ruspeechstress-0.5/ruspeechstress/utils.py
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:09:13.356905 ruspeechstress-0.5/ruspeechstress.egg-info/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:09:13.000000 ruspeechstress-0.5/ruspeechstress.egg-info/PKG-INFO
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      295 2023-06-07 16:09:13.000000 ruspeechstress-0.5/ruspeechstress.egg-info/SOURCES.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)        1 2023-06-07 16:09:13.000000 ruspeechstress-0.5/ruspeechstress.egg-info/dependency_links.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)       15 2023-06-07 16:09:13.000000 ruspeechstress-0.5/ruspeechstress.egg-info/top_level.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)       38 2023-06-07 16:09:13.356905 ruspeechstress-0.5/setup.cfg
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      377 2023-06-07 16:09:09.000000 ruspeechstress-0.5/setup.py
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:12:24.395391 ruspeechstress-0.6/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:12:24.395391 ruspeechstress-0.6/PKG-INFO
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:12:24.391391 ruspeechstress-0.6/ruspeechstress/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      760 2023-06-07 16:12:22.000000 ruspeechstress-0.6/ruspeechstress/__init__.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    13250 2023-06-07 16:12:22.000000 ruspeechstress-0.6/ruspeechstress/dataset.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    31206 2023-06-07 09:32:56.000000 ruspeechstress-0.6/ruspeechstress/sound.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    18830 2023-06-07 16:12:22.000000 ruspeechstress-0.6/ruspeechstress/stress_detector.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)     1806 2021-06-01 18:24:40.000000 ruspeechstress-0.6/ruspeechstress/utils.py
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:12:24.391391 ruspeechstress-0.6/ruspeechstress.egg-info/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:12:24.000000 ruspeechstress-0.6/ruspeechstress.egg-info/PKG-INFO
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      295 2023-06-07 16:12:24.000000 ruspeechstress-0.6/ruspeechstress.egg-info/SOURCES.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)        1 2023-06-07 16:12:24.000000 ruspeechstress-0.6/ruspeechstress.egg-info/dependency_links.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)       15 2023-06-07 16:12:24.000000 ruspeechstress-0.6/ruspeechstress.egg-info/top_level.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)       38 2023-06-07 16:12:24.395391 ruspeechstress-0.6/setup.cfg
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      377 2023-06-07 16:12:22.000000 ruspeechstress-0.6/setup.py
```

### Comparing `ruspeechstress-0.5/ruspeechstress/__init__.py` & `ruspeechstress-0.6/ruspeechstress/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
-# from .stress_detector import StressDetector, FEATURES
+from .stress_detector import StressDetector, FEATURES
 from dataset import dataset
 import numpy as np
 
 
 def create_dataset(working_dir=os.getcwd(), dictionary_path=None):
     dataset(working_dir=working_dir, dictionary_path=dictionary_path, mode='collect_dataset')
 
 
-# def train_model(working_dir=os.getcwd(), clf=None):
-#     wav_path = os.path.join(working_dir, 'wav_tg_all')
-#     sd = StressDetector(wav_path, FEATURES)
-#     sd.get_features('./data/complete_features.tsv')
-#     evaluation = sd.train(clf())
-#     print(f'F1 Score: {np.mean(evaluation["f1"])}')
+def train_model(working_dir=os.getcwd(), clf=None):
+    wav_path = os.path.join(working_dir, 'wav_tg_all')
+    sd = StressDetector(wav_path, FEATURES)
+    sd.get_features('./data/complete_features.tsv')
+    evaluation = sd.train(clf())
+    print(f'F1 Score: {np.mean(evaluation["f1"])}')
 
 
 def extend_dictionary(working_dir=os.getcwd(), dictionary_path='/home/sivh/thesis/zaliznyak.txt'):
     dataset(working_dir=working_dir, dictionary_path=dictionary_path, mode='extend_dictionary')
```

### Comparing `ruspeechstress-0.5/ruspeechstress/dataset.py` & `ruspeechstress-0.6/ruspeechstress/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pydub import AudioSegment
 import wave
 import requests
 import xml.etree.ElementTree as Et
 import csv
 import textgrid
 import rusyllab
-from stress_detector import StressDetector, FEATURES
+from .stress_detector import StressDetector, FEATURES
 
 
 class FileSizeError(Exception):
     pass
 
 
 class NoDictProvided(Exception):
```

### Comparing `ruspeechstress-0.5/ruspeechstress/sound.py` & `ruspeechstress-0.6/ruspeechstress/sound.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.5/ruspeechstress/stress_detector.py` & `ruspeechstress-0.6/ruspeechstress/stress_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 from sklearn.metrics import accuracy_score, precision_recall_fscore_support, f1_score
 from sklearn.model_selection import ShuffleSplit, GridSearchCV
 from sklearn.preprocessing import StandardScaler
 
 from typing import Tuple, Dict, List
 
-from utils import plot_confusion_matrix
+from .utils import plot_confusion_matrix
 from tqdm import tqdm
-from sound import Sound, LANG_SAMPA_VOWELS
+from .sound import Sound, LANG_SAMPA_VOWELS
 
 # selected features after feature engineering
 FEATURES = ['pos', 'nr_syll', 'nucl_dur', 'syll_dur', 'syll_dur_norm',  'nucl_dur_left', 'nucl_dur_right', 'rms',
             'int_peak', 'rms_norm', 'int_peak_norm', 'rms_left', 'rms_right', 'int_peak_left', 'int_peak_right',
             'spect_b1', 'spect_b2', 'spect_b3', 'spect_b1_left', 'spect_b2_left', 'spect_b3_left', 'spect_b1_right',
             'spect_b2_right', 'spect_b3_right', 'trajectory', 'f0_max', 'f0_mean', 'f0_meanST', 'f0_max_styl',
             'f0_max_norm', 'f0_mean_norm', 'f0_max_styl_norm', 'f0_meanST_norm', 'intersyllab', 'f0_max_left',
```

### Comparing `ruspeechstress-0.5/ruspeechstress/utils.py` & `ruspeechstress-0.6/ruspeechstress/utils.py`

 * *Files identical despite different names*

