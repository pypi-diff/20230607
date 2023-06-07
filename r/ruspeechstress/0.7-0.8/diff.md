# Comparing `tmp/ruspeechstress-0.7.tar.gz` & `tmp/ruspeechstress-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruspeechstress-0.7.tar", last modified: Wed Jun  7 16:14:08 2023, max compression
+gzip compressed data, was "ruspeechstress-0.8.tar", last modified: Wed Jun  7 16:34:16 2023, max compression
```

## Comparing `ruspeechstress-0.7.tar` & `ruspeechstress-0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:14:08.422555 ruspeechstress-0.7/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:14:08.422555 ruspeechstress-0.7/PKG-INFO
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:14:08.422555 ruspeechstress-0.7/ruspeechstress/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      761 2023-06-07 16:13:56.000000 ruspeechstress-0.7/ruspeechstress/__init__.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    13250 2023-06-07 16:12:22.000000 ruspeechstress-0.7/ruspeechstress/dataset.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    31206 2023-06-07 09:32:56.000000 ruspeechstress-0.7/ruspeechstress/sound.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)    18830 2023-06-07 16:12:22.000000 ruspeechstress-0.7/ruspeechstress/stress_detector.py
--rw-rw-r--   0 sivh      (1000) sivh      (1000)     1806 2021-06-01 18:24:40.000000 ruspeechstress-0.7/ruspeechstress/utils.py
-drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:14:08.422555 ruspeechstress-0.7/ruspeechstress.egg-info/
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:14:08.000000 ruspeechstress-0.7/ruspeechstress.egg-info/PKG-INFO
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      295 2023-06-07 16:14:08.000000 ruspeechstress-0.7/ruspeechstress.egg-info/SOURCES.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)        1 2023-06-07 16:14:08.000000 ruspeechstress-0.7/ruspeechstress.egg-info/dependency_links.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)       15 2023-06-07 16:14:08.000000 ruspeechstress-0.7/ruspeechstress.egg-info/top_level.txt
--rw-rw-r--   0 sivh      (1000) sivh      (1000)       38 2023-06-07 16:14:08.422555 ruspeechstress-0.7/setup.cfg
--rw-rw-r--   0 sivh      (1000) sivh      (1000)      377 2023-06-07 16:13:56.000000 ruspeechstress-0.7/setup.py
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:34:16.047209 ruspeechstress-0.8/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:34:16.047209 ruspeechstress-0.8/PKG-INFO
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:34:16.047209 ruspeechstress-0.8/ruspeechstress/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      747 2023-06-07 16:33:38.000000 ruspeechstress-0.8/ruspeechstress/__init__.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    13536 2023-06-07 16:33:38.000000 ruspeechstress-0.8/ruspeechstress/dataset.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    31206 2023-06-07 09:32:56.000000 ruspeechstress-0.8/ruspeechstress/sound.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)    18830 2023-06-07 16:12:22.000000 ruspeechstress-0.8/ruspeechstress/stress_detector.py
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)     1806 2021-06-01 18:24:40.000000 ruspeechstress-0.8/ruspeechstress/utils.py
+drwxrwxr-x   0 sivh      (1000) sivh      (1000)        0 2023-06-07 16:34:16.047209 ruspeechstress-0.8/ruspeechstress.egg-info/
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      303 2023-06-07 16:34:16.000000 ruspeechstress-0.8/ruspeechstress.egg-info/PKG-INFO
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      295 2023-06-07 16:34:16.000000 ruspeechstress-0.8/ruspeechstress.egg-info/SOURCES.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)        1 2023-06-07 16:34:16.000000 ruspeechstress-0.8/ruspeechstress.egg-info/dependency_links.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)       15 2023-06-07 16:34:16.000000 ruspeechstress-0.8/ruspeechstress.egg-info/top_level.txt
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)       38 2023-06-07 16:34:16.047209 ruspeechstress-0.8/setup.cfg
+-rw-rw-r--   0 sivh      (1000) sivh      (1000)      377 2023-06-07 16:33:48.000000 ruspeechstress-0.8/setup.py
```

### Comparing `ruspeechstress-0.7/ruspeechstress/dataset.py` & `ruspeechstress-0.8/ruspeechstress/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,20 @@
 
 
 class NoDictProvided(Exception):
     pass
 
 
 def clear_old_files(working_dir, directory='wav_tg_all'):
-    files = os.listdir(os.path.join(working_dir, directory))
-    for file in files:
-        os.remove(os.path.join(os.path.join(working_dir, directory), file))
+    if not os.path.exists(os.path.join(working_dir, directory)):
+        pass
+    else:
+        files = os.listdir(os.path.join(working_dir, directory))
+        for file in files:
+            os.remove(os.path.join(os.path.join(working_dir, directory), file))
 
 
 def get_files(working_dir, input_directory='./dataset'):
     file_pairs = {}
     full_path = os.path.join(working_dir, input_directory)
     for file in listdir(full_path):
         text = os.path.join(full_path, file[:-4] + '.txt')
@@ -139,20 +142,22 @@
     for i in range(len(chunks)):
         if "'" in chunks[i]:
             stress_position = i + 1
     if stress_position != 0:
         return stress_position
 
 
-def collect_dataset(working_dir, input_files, dictionary, output_path='./wav_tg_all', mode='collect_dataset'):
+def collect_dataset(working_dir, input_files, dictionary, output_path='wav_tg_all', mode='collect_dataset'):
     n = 0
     all_data = []
     words = []
     words_all = []
     words_in_dict = []
+    if not os.path.exists(os.path.join(working_dir, output_path)):
+        os.mkdir(os.path.join(working_dir, output_path))
     for wav in input_files.keys():
         if os.path.exists(wav[:-4] + '.TextGrid'):
             transcription = textgrid.TextGrid.fromFile(wav[:-4] + '.TextGrid')
             for i in range(len(transcription[0])):
                 word = transcription[0][i]
                 if mode == 'collect_dataset':
                     if word.mark != "" and word.mark in dictionary.keys() and len(
@@ -218,23 +223,24 @@
     for file in os.listdir(os.path.join(working_dir, input_path)):
         wav_file = file.strip('.TextGrid') + '.wav'
         if file.endswith('.TextGrid') and not os.path.exists(
                 os.path.join(os.path.join(working_dir, input_path), wav_file)):
             os.remove(os.path.join(os.path.join(working_dir, input_path), file))
 
 
-def dataset(working_dir, dictionary_path=None, mode=None, model_path='models/classifier_vot.pkl',
+def dataset(dataset_dir, dictionary_path=None, mode=None, model_path='models/classifier_vot.pkl',
             scaler_path='models/scaler.pkl'):
-    clear_old_files(working_dir)
+    working_dir = os.path.dirname(os.path.dirname(dataset_dir))
+    clear_old_files(dataset_dir)
     print("Getting files and preprocessing audio and text...")
-    files = get_files(working_dir)
+    files = get_files(dataset_dir)
     preprocess_audio(files)
     get_size(files)
     transcribe_audio(files)
-    files = get_files(working_dir)
+    files = get_files(dataset_dir)
     preprocess_text(files)
     print("Creating TextGrid files...")
     # webmaus(files, working_dir)
     if dictionary_path is None:
         raise NoDictProvided('No dictionary provided.')
     dictionary = build_dictionary(dictionary_path)
     print("Collecting dataset...")
```

### Comparing `ruspeechstress-0.7/ruspeechstress/sound.py` & `ruspeechstress-0.8/ruspeechstress/sound.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.7/ruspeechstress/stress_detector.py` & `ruspeechstress-0.8/ruspeechstress/stress_detector.py`

 * *Files identical despite different names*

### Comparing `ruspeechstress-0.7/ruspeechstress/utils.py` & `ruspeechstress-0.8/ruspeechstress/utils.py`

 * *Files identical despite different names*

