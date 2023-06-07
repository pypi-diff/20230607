# Comparing `tmp/ruspeechstress-0.4.tar.gz` & `tmp/ruspeechstress-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruspeechstress-0.4.tar", last modified: Wed Jun  7 16:07:46 2023, max compression
+gzip compressed data, was "ruspeechstress-0.5.tar", last modified: Wed Jun  7 16:09:13 2023, max compression
```

## Comparing `ruspeechstress-0.4.tar` & `ruspeechstress-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:07:46.621579 ruspeechstress-0.4/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:07:46.621579 ruspeechstress-0.4/PKG-INFO
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:07:46.617579 ruspeechstress-0.4/ruspeechstress/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      760 2023-06-07 16:07:40.000000 ruspeechstress-0.4/ruspeechstress/__init__.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    13249 2023-06-07 14:55:17.000000 ruspeechstress-0.4/ruspeechstress/dataset.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    31206 2023-06-07 09:32:56.000000 ruspeechstress-0.4/ruspeechstress/sound.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    18828 2023-06-07 09:27:32.000000 ruspeechstress-0.4/ruspeechstress/stress_detector.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)     1806 2021-06-01 18:24:40.000000 ruspeechstress-0.4/ruspeechstress/utils.py
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:07:46.621579 ruspeechstress-0.4/ruspeechstress.egg-info/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:07:46.000000 ruspeechstress-0.4/ruspeechstress.egg-info/PKG-INFO
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      295 2023-06-07 16:07:46.000000 ruspeechstress-0.4/ruspeechstress.egg-info/SOURCES.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)        1 2023-06-07 16:07:46.000000 ruspeechstress-0.4/ruspeechstress.egg-info/dependency_links.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)       15 2023-06-07 16:07:46.000000 ruspeechstress-0.4/ruspeechstress.egg-info/top_level.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)       38 2023-06-07 16:07:46.621579 ruspeechstress-0.4/setup.cfg
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      377 2023-06-07 16:07:40.000000 ruspeechstress-0.4/setup.py
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:09:13.356905 ruspeechstress-0.5/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:09:13.356905 ruspeechstress-0.5/PKG-INFO
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:09:13.352905 ruspeechstress-0.5/ruspeechstress/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      774 2023-06-07 16:08:57.000000 ruspeechstress-0.5/ruspeechstress/__init__.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    13249 2023-06-07 14:55:17.000000 ruspeechstress-0.5/ruspeechstress/dataset.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    31206 2023-06-07 09:32:56.000000 ruspeechstress-0.5/ruspeechstress/sound.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    18828 2023-06-07 09:27:32.000000 ruspeechstress-0.5/ruspeechstress/stress_detector.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)     1806 2021-06-01 18:24:40.000000 ruspeechstress-0.5/ruspeechstress/utils.py
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:09:13.356905 ruspeechstress-0.5/ruspeechstress.egg-info/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:09:13.000000 ruspeechstress-0.5/ruspeechstress.egg-info/PKG-INFO
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      295 2023-06-07 16:09:13.000000 ruspeechstress-0.5/ruspeechstress.egg-info/SOURCES.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)        1 2023-06-07 16:09:13.000000 ruspeechstress-0.5/ruspeechstress.egg-info/dependency_links.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)       15 2023-06-07 16:09:13.000000 ruspeechstress-0.5/ruspeechstress.egg-info/top_level.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)       38 2023-06-07 16:09:13.356905 ruspeechstress-0.5/setup.cfg
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      377 2023-06-07 16:09:09.000000 ruspeechstress-0.5/setup.py
```

### Comparing `ruspeechstress-0.4/ruspeechstress/__init__.py` & `ruspeechstress-0.5/ruspeechstress/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
-from .stress_detector import StressDetector, FEATURES
+# from .stress_detector import StressDetector, FEATURES
 from dataset import dataset
 import numpy as np
 
 
 def create_dataset(working_dir=os.getcwd(), dictionary_path=None):
     dataset(working_dir=working_dir, dictionary_path=dictionary_path, mode='collect_dataset')
 
 
-def train_model(working_dir=os.getcwd(), clf=None):
-    wav_path = os.path.join(working_dir, 'wav_tg_all')
-    sd = StressDetector(wav_path, FEATURES)
-    sd.get_features('./data/complete_features.tsv')
-    evaluation = sd.train(clf())
-    print(f'F1 Score: {np.mean(evaluation["f1"])}')
+# def train_model(working_dir=os.getcwd(), clf=None):
+#     wav_path = os.path.join(working_dir, 'wav_tg_all')
+#     sd = StressDetector(wav_path, FEATURES)
+#     sd.get_features('./data/complete_features.tsv')
+#     evaluation = sd.train(clf())
+#     print(f'F1 Score: {np.mean(evaluation["f1"])}')
 
 
 def extend_dictionary(working_dir=os.getcwd(), dictionary_path='/home/sivh/thesis/zaliznyak.txt'):
     dataset(working_dir=working_dir, dictionary_path=dictionary_path, mode='extend_dictionary')
```

### Comparing `ruspeechstress-0.4/ruspeechstress/dataset.py` & `ruspeechstress-0.5/ruspeechstress/dataset.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.4/ruspeechstress/sound.py` & `ruspeechstress-0.5/ruspeechstress/sound.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.4/ruspeechstress/stress_detector.py` & `ruspeechstress-0.5/ruspeechstress/stress_detector.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.4/ruspeechstress/utils.py` & `ruspeechstress-0.5/ruspeechstress/utils.py`

 * *Files identical despite different names*

