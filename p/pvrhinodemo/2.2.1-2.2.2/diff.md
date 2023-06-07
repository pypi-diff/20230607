# Comparing `tmp/pvrhinodemo-2.2.1.tar.gz` & `tmp/pvrhinodemo-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvrhinodemo-2.2.1.tar", last modified: Wed Apr 19 17:44:58 2023, max compression
+gzip compressed data, was "pvrhinodemo-2.2.2.tar", last modified: Wed Jun  7 20:59:02 2023, max compression
```

## Comparing `pvrhinodemo-2.2.1.tar` & `pvrhinodemo-2.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:44:58.731333 pvrhinodemo-2.2.1/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      102 2023-04-19 17:44:57.000000 pvrhinodemo-2.2.1/MANIFEST.in
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4042 2023-04-19 17:44:58.731333 pvrhinodemo-2.2.1/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     3359 2023-04-19 17:34:19.000000 pvrhinodemo-2.2.1/README.md
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:44:58.731333 pvrhinodemo-2.2.1/pvrhinodemo/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5697 2023-04-19 17:44:57.000000 pvrhinodemo-2.2.1/pvrhinodemo/rhino_demo_file.py
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6010 2023-04-19 17:44:57.000000 pvrhinodemo-2.2.1/pvrhinodemo/rhino_demo_mic.py
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:44:58.731333 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4042 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      303 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/SOURCES.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/dependency_links.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      118 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/entry_points.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       33 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/requires.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       12 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/top_level.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-19 17:44:58.731333 pvrhinodemo-2.2.1/setup.cfg
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     1979 2023-04-19 17:41:52.000000 pvrhinodemo-2.2.1/setup.py
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 20:59:02.448870 pvrhinodemo-2.2.2/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      102 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/MANIFEST.in
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4079 2023-06-07 20:59:02.448870 pvrhinodemo-2.2.2/PKG-INFO
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     3359 2023-06-07 20:37:59.000000 pvrhinodemo-2.2.2/README.md
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 20:59:02.448870 pvrhinodemo-2.2.2/pvrhinodemo/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     5697 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo/rhino_demo_file.py
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6010 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo/rhino_demo_mic.py
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 20:59:02.448870 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4079 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/PKG-INFO
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      303 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)        1 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      119 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/entry_points.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       33 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/requires.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       12 2023-06-07 20:59:02.000000 pvrhinodemo-2.2.2/pvrhinodemo.egg-info/top_level.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       38 2023-06-07 20:59:02.448870 pvrhinodemo-2.2.2/setup.cfg
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     1979 2023-06-07 20:58:47.000000 pvrhinodemo-2.2.2/setup.py
```

### Comparing `pvrhinodemo-2.2.1/PKG-INFO` & `pvrhinodemo-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pvrhinodemo
-Version: 2.2.1
+Version: 2.2.2
 Summary: Rhino Speech-to-Intent engine demos.
 Home-page: https://github.com/Picovoice/rhino
 Author: Picovoice
 Author-email: hello@picovoice.ai
+License: UNKNOWN
 Keywords: Speech-to-Intent,voice commands,voice control,speech recognition,natural language understanding
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -109,7 +111,9 @@
 ```
 
 If a problem occurs, we suggest storing the recorded audio into a file for inspection. This can be achieved by:
 
 ```console
 rhino_demo_mic --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} --audio_device_index 0 --output_path ~/test.wav
 ```
+
+
```

### Comparing `pvrhinodemo-2.2.1/README.md` & `pvrhinodemo-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pvrhinodemo-2.2.1/pvrhinodemo/rhino_demo_file.py` & `pvrhinodemo-2.2.2/pvrhinodemo/rhino_demo_file.py`

 * *Files identical despite different names*

### Comparing `pvrhinodemo-2.2.1/pvrhinodemo/rhino_demo_mic.py` & `pvrhinodemo-2.2.2/pvrhinodemo/rhino_demo_mic.py`

 * *Files identical despite different names*

### Comparing `pvrhinodemo-2.2.1/pvrhinodemo.egg-info/PKG-INFO` & `pvrhinodemo-2.2.2/pvrhinodemo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pvrhinodemo
-Version: 2.2.1
+Version: 2.2.2
 Summary: Rhino Speech-to-Intent engine demos.
 Home-page: https://github.com/Picovoice/rhino
 Author: Picovoice
 Author-email: hello@picovoice.ai
+License: UNKNOWN
 Keywords: Speech-to-Intent,voice commands,voice control,speech recognition,natural language understanding
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -109,7 +111,9 @@
 ```
 
 If a problem occurs, we suggest storing the recorded audio into a file for inspection. This can be achieved by:
 
 ```console
 rhino_demo_mic --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} --audio_device_index 0 --output_path ~/test.wav
 ```
+
+
```

### Comparing `pvrhinodemo-2.2.1/setup.py` & `pvrhinodemo-2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     f.write('include pvrhinodemo/rhino_demo_mic.py')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvrhinodemo",
-    version="2.2.1",
+    version="2.2.2",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Rhino Speech-to-Intent engine demos.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/rhino",
     packages=["pvrhinodemo"],
-    install_requires=["pvrhino==2.2.0", "pvrecorder==1.1.1"],
+    install_requires=["pvrhino==2.2.2", "pvrecorder==1.1.1"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

