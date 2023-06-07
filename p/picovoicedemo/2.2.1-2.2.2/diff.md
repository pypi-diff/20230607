# Comparing `tmp/picovoicedemo-2.2.1.tar.gz` & `tmp/picovoicedemo-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picovoicedemo-2.2.1.tar", last modified: Wed Apr 19 17:57:19 2023, max compression
+gzip compressed data, was "picovoicedemo-2.2.2.tar", last modified: Wed Jun  7 21:32:04 2023, max compression
```

## Comparing `picovoicedemo-2.2.1.tar` & `picovoicedemo-2.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:57:19.188887 picovoicedemo-2.2.1/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      119 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/MANIFEST.in
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4906 2023-04-19 17:57:19.188887 picovoicedemo-2.2.1/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4236 2023-04-18 21:24:31.000000 picovoicedemo-2.2.1/README.md
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:57:19.188887 picovoicedemo-2.2.1/picovoicedemo/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    11344 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo/LICENSE
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6568 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo/picovoice_demo_file.py
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6876 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo/picovoice_demo_mic.py
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:57:19.188887 picovoicedemo-2.2.1/picovoicedemo.egg-info/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4906 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      349 2023-04-19 17:57:19.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/SOURCES.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/dependency_links.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      138 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/entry_points.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       35 2023-04-19 17:57:19.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/requires.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       14 2023-04-19 17:57:19.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/top_level.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-19 17:57:19.188887 picovoicedemo-2.2.1/setup.cfg
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     2537 2023-04-19 17:54:51.000000 picovoicedemo-2.2.1/setup.py
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:32:04.317071 picovoicedemo-2.2.2/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      119 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/MANIFEST.in
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4943 2023-06-07 21:32:04.317071 picovoicedemo-2.2.2/PKG-INFO
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4236 2023-06-07 20:45:36.000000 picovoicedemo-2.2.2/README.md
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:32:04.317071 picovoicedemo-2.2.2/picovoicedemo/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)    11344 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo/LICENSE
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6568 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo/picovoice_demo_file.py
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6876 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo/picovoice_demo_mic.py
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:32:04.317071 picovoicedemo-2.2.2/picovoicedemo.egg-info/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4943 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/PKG-INFO
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      349 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)        1 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      139 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/entry_points.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       35 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/requires.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       14 2023-06-07 21:32:04.000000 picovoicedemo-2.2.2/picovoicedemo.egg-info/top_level.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       38 2023-06-07 21:32:04.317071 picovoicedemo-2.2.2/setup.cfg
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     2537 2023-06-07 21:31:44.000000 picovoicedemo-2.2.2/setup.py
```

### Comparing `picovoicedemo-2.2.1/PKG-INFO` & `picovoicedemo-2.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: picovoicedemo
-Version: 2.2.1
+Version: 2.2.2
 Summary: Picovoice demos.
 Home-page: https://github.com/Picovoice/picovoice
 Author: Picovoice Inc.
 Author-email: hello@picovoice.ai
+License: UNKNOWN
 Keywords: wake word,voice control,speech recognition,voice recognition,natural language understanding
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -117,7 +119,9 @@
 --keyword_path ${PATH_TO_PORCUPINE_KEYWORD_FILE} \
 --context_path ${PATH_TO_RHINO_CONTEXT_FILE)} \
 --audio_device_index 0 \
 --output_path ~/test.wav
 ```
 
 If after listening to stored file there is no apparent problem detected please open an issue.
+
+
```

### Comparing `picovoicedemo-2.2.1/README.md` & `picovoicedemo-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `picovoicedemo-2.2.1/picovoicedemo/LICENSE` & `picovoicedemo-2.2.2/picovoicedemo/LICENSE`

 * *Files identical despite different names*

### Comparing `picovoicedemo-2.2.1/picovoicedemo/picovoice_demo_file.py` & `picovoicedemo-2.2.2/picovoicedemo/picovoice_demo_file.py`

 * *Files identical despite different names*

### Comparing `picovoicedemo-2.2.1/picovoicedemo/picovoice_demo_mic.py` & `picovoicedemo-2.2.2/picovoicedemo/picovoice_demo_mic.py`

 * *Files identical despite different names*

### Comparing `picovoicedemo-2.2.1/picovoicedemo.egg-info/PKG-INFO` & `picovoicedemo-2.2.2/picovoicedemo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: picovoicedemo
-Version: 2.2.1
+Version: 2.2.2
 Summary: Picovoice demos.
 Home-page: https://github.com/Picovoice/picovoice
 Author: Picovoice Inc.
 Author-email: hello@picovoice.ai
+License: UNKNOWN
 Keywords: wake word,voice control,speech recognition,voice recognition,natural language understanding
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -117,7 +119,9 @@
 --keyword_path ${PATH_TO_PORCUPINE_KEYWORD_FILE} \
 --context_path ${PATH_TO_RHINO_CONTEXT_FILE)} \
 --audio_device_index 0 \
 --output_path ~/test.wav
 ```
 
 If after listening to stored file there is no apparent problem detected please open an issue.
+
+
```

### Comparing `picovoicedemo-2.2.1/setup.py` & `picovoicedemo-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,23 +35,23 @@
     f.write('include picovoicedemo/picovoice_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="picovoicedemo",
-    version="2.2.1",
+    version="2.2.2",
     author="Picovoice Inc.",
     author_email="hello@picovoice.ai",
     description="Picovoice demos.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/picovoice",
     packages=["picovoicedemo"],
-    install_requires=["picovoice==2.2.0", "pvrecorder==1.1.1"],
+    install_requires=["picovoice==2.2.1", "pvrecorder==1.1.1"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

