# Comparing `tmp/pvporcupinedemo-2.2.0.tar.gz` & `tmp/pvporcupinedemo-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvporcupinedemo-2.2.0.tar", last modified: Wed Apr 12 17:54:05 2023, max compression
+gzip compressed data, was "pvporcupinedemo-2.2.1.tar", last modified: Wed Jun  7 17:53:53 2023, max compression
```

## Comparing `pvporcupinedemo-2.2.0.tar` & `pvporcupinedemo-2.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 17:54:05.004299 pvporcupinedemo-2.2.0/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      125 2023-04-12 17:54:03.000000 pvporcupinedemo-2.2.0/MANIFEST.in
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6460 2023-04-12 17:54:05.004299 pvporcupinedemo-2.2.0/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5782 2023-04-06 17:23:16.000000 pvporcupinedemo-2.2.0/README.md
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 17:54:05.004299 pvporcupinedemo-2.2.0/pvporcupinedemo/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    11344 2023-04-12 17:54:03.000000 pvporcupinedemo-2.2.0/pvporcupinedemo/LICENSE
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5453 2023-04-12 17:54:03.000000 pvporcupinedemo-2.2.0/pvporcupinedemo/porcupine_demo_file.py
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5572 2023-04-12 17:54:03.000000 pvporcupinedemo-2.2.0/pvporcupinedemo/porcupine_demo_mic.py
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 17:54:05.004299 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6460 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      367 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/SOURCES.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/dependency_links.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      142 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/entry_points.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       37 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/requires.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       16 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/top_level.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-12 17:54:05.004299 pvporcupinedemo-2.2.0/setup.cfg
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     2053 2023-04-06 17:23:16.000000 pvporcupinedemo-2.2.0/setup.py
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 17:53:53.106758 pvporcupinedemo-2.2.1/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      125 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/MANIFEST.in
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6497 2023-06-07 17:53:53.106758 pvporcupinedemo-2.2.1/PKG-INFO
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     5782 2023-06-07 17:44:48.000000 pvporcupinedemo-2.2.1/README.md
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 17:53:53.106758 pvporcupinedemo-2.2.1/pvporcupinedemo/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)    11344 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo/LICENSE
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     5453 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo/porcupine_demo_file.py
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     5572 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo/porcupine_demo_mic.py
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 17:53:53.106758 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6497 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/PKG-INFO
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      367 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)        1 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      143 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/entry_points.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       37 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/requires.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       16 2023-06-07 17:53:53.000000 pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/top_level.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       38 2023-06-07 17:53:53.110758 pvporcupinedemo-2.2.1/setup.cfg
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     2053 2023-06-07 17:53:21.000000 pvporcupinedemo-2.2.1/setup.py
```

### Comparing `pvporcupinedemo-2.2.0/PKG-INFO` & `pvporcupinedemo-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pvporcupinedemo
-Version: 2.2.0
+Version: 2.2.1
 Summary: Porcupine wake word engine demos
 Home-page: https://github.com/Picovoice/porcupine
 Author: Picovoice
 Author-email: hello@picovoice.ai
+License: UNKNOWN
 Keywords: wake word engine,hotword detection,keyword spotting,wake word detection,voice commands
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -169,7 +171,9 @@
 porcupine_demo_file --access_key ${ACCESS_KEY} \
 --wav_path ${AUDIO_PATH} \
 --keywords grasshopper porcupine --sensitivities 0.3 0.6
 ```
 
 Sensitivity is the parameter that enables trading miss rate for the false alarm rate. It is a floating point number within
 `[0, 1]`. A higher sensitivity reduces the miss rate at the cost of increased false alarm rate.
+
+
```

### Comparing `pvporcupinedemo-2.2.0/README.md` & `pvporcupinedemo-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pvporcupinedemo-2.2.0/pvporcupinedemo/LICENSE` & `pvporcupinedemo-2.2.1/pvporcupinedemo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvporcupinedemo-2.2.0/pvporcupinedemo/porcupine_demo_file.py` & `pvporcupinedemo-2.2.1/pvporcupinedemo/porcupine_demo_file.py`

 * *Files identical despite different names*

### Comparing `pvporcupinedemo-2.2.0/pvporcupinedemo/porcupine_demo_mic.py` & `pvporcupinedemo-2.2.1/pvporcupinedemo/porcupine_demo_mic.py`

 * *Files identical despite different names*

### Comparing `pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/PKG-INFO` & `pvporcupinedemo-2.2.1/pvporcupinedemo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pvporcupinedemo
-Version: 2.2.0
+Version: 2.2.1
 Summary: Porcupine wake word engine demos
 Home-page: https://github.com/Picovoice/porcupine
 Author: Picovoice
 Author-email: hello@picovoice.ai
+License: UNKNOWN
 Keywords: wake word engine,hotword detection,keyword spotting,wake word detection,voice commands
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -169,7 +171,9 @@
 porcupine_demo_file --access_key ${ACCESS_KEY} \
 --wav_path ${AUDIO_PATH} \
 --keywords grasshopper porcupine --sensitivities 0.3 0.6
 ```
 
 Sensitivity is the parameter that enables trading miss rate for the false alarm rate. It is a floating point number within
 `[0, 1]`. A higher sensitivity reduces the miss rate at the cost of increased false alarm rate.
+
+
```

### Comparing `pvporcupinedemo-2.2.0/setup.py` & `pvporcupinedemo-2.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     f.write('include pvporcupinedemo/porcupine_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvporcupinedemo",
-    version="2.2.0",
+    version="2.2.1",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Porcupine wake word engine demos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/porcupine",
     packages=["pvporcupinedemo"],
-    install_requires=["pvporcupine==2.2.0", "pvrecorder==1.1.1"],
+    install_requires=["pvporcupine==2.2.1", "pvrecorder==1.1.1"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

