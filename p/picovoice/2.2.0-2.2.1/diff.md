# Comparing `tmp/picovoice-2.2.0.tar.gz` & `tmp/picovoice-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picovoice-2.2.0.tar", last modified: Wed Apr 12 18:05:03 2023, max compression
+gzip compressed data, was "picovoice-2.2.1.tar", last modified: Wed Jun  7 21:28:07 2023, max compression
```

## Comparing `picovoice-2.2.0.tar` & `picovoice-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:05:03.575489 picovoice-2.2.0/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       88 2023-04-12 18:05:02.000000 picovoice-2.2.0/MANIFEST.in
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4412 2023-04-12 18:05:03.575489 picovoice-2.2.0/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     3684 2022-06-13 15:28:43.000000 picovoice-2.2.0/README.md
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:05:03.571489 picovoice-2.2.0/picovoice/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    11344 2023-04-12 18:05:02.000000 picovoice-2.2.0/picovoice/LICENSE
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      534 2023-04-12 18:05:02.000000 picovoice-2.2.0/picovoice/__init__.py
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    12966 2023-04-12 18:05:02.000000 picovoice-2.2.0/picovoice/_picovoice.py
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:05:03.575489 picovoice-2.2.0/picovoice.egg-info/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4412 2023-04-12 18:05:03.000000 picovoice-2.2.0/picovoice.egg-info/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      258 2023-04-12 18:05:03.000000 picovoice-2.2.0/picovoice.egg-info/SOURCES.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-12 18:05:03.000000 picovoice-2.2.0/picovoice.egg-info/dependency_links.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       34 2023-04-12 18:05:03.000000 picovoice-2.2.0/picovoice.egg-info/requires.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       10 2023-04-12 18:05:03.000000 picovoice-2.2.0/picovoice.egg-info/top_level.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-12 18:05:03.575489 picovoice-2.2.0/setup.cfg
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     2284 2023-04-10 19:55:03.000000 picovoice-2.2.0/setup.py
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:28:07.747779 picovoice-2.2.1/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       88 2023-06-07 21:28:07.000000 picovoice-2.2.1/MANIFEST.in
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4449 2023-06-07 21:28:07.747779 picovoice-2.2.1/PKG-INFO
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     3684 2022-09-21 18:37:18.000000 picovoice-2.2.1/README.md
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:28:07.747779 picovoice-2.2.1/picovoice/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)    11344 2023-06-07 21:28:07.000000 picovoice-2.2.1/picovoice/LICENSE
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      534 2023-06-07 21:28:07.000000 picovoice-2.2.1/picovoice/__init__.py
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)    12966 2023-06-07 21:28:07.000000 picovoice-2.2.1/picovoice/_picovoice.py
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:28:07.747779 picovoice-2.2.1/picovoice.egg-info/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4449 2023-06-07 21:28:07.000000 picovoice-2.2.1/picovoice.egg-info/PKG-INFO
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      258 2023-06-07 21:28:07.000000 picovoice-2.2.1/picovoice.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)        1 2023-06-07 21:28:07.000000 picovoice-2.2.1/picovoice.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       34 2023-06-07 21:28:07.000000 picovoice-2.2.1/picovoice.egg-info/requires.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       10 2023-06-07 21:28:07.000000 picovoice-2.2.1/picovoice.egg-info/top_level.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       38 2023-06-07 21:28:07.747779 picovoice-2.2.1/setup.cfg
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     2284 2023-06-07 21:28:01.000000 picovoice-2.2.1/setup.py
```

### Comparing `picovoice-2.2.0/PKG-INFO` & `picovoice-2.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: picovoice
-Version: 2.2.0
+Version: 2.2.1
 Summary: Picovoice is an end-to-end platform for building voice products on your terms.
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
@@ -106,7 +108,9 @@
 
 In order to detect wake words and run inference in other languages you need to use the corresponding model file. The model files for all supported languages are available [here](https://github.com/Picovoice/porcupine/tree/master/lib/common) and [here](https://github.com/Picovoice/rhino/tree/master/lib/common).
 
 ## Demos
 
 [picovoicedemo](https://pypi.org/project/picovoicedemo/) provides command-line utilities for processing real-time
 audio (i.e. microphone) and files using Picovoice platform.
+
+
```

### Comparing `picovoice-2.2.0/README.md` & `picovoice-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `picovoice-2.2.0/picovoice/LICENSE` & `picovoice-2.2.1/picovoice/LICENSE`

 * *Files identical despite different names*

### Comparing `picovoice-2.2.0/picovoice/__init__.py` & `picovoice-2.2.1/picovoice/__init__.py`

 * *Files identical despite different names*

### Comparing `picovoice-2.2.0/picovoice/_picovoice.py` & `picovoice-2.2.1/picovoice/_picovoice.py`

 * *Files identical despite different names*

### Comparing `picovoice-2.2.0/picovoice.egg-info/PKG-INFO` & `picovoice-2.2.1/picovoice.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: picovoice
-Version: 2.2.0
+Version: 2.2.1
 Summary: Picovoice is an end-to-end platform for building voice products on your terms.
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
@@ -106,7 +108,9 @@
 
 In order to detect wake words and run inference in other languages you need to use the corresponding model file. The model files for all supported languages are available [here](https://github.com/Picovoice/porcupine/tree/master/lib/common) and [here](https://github.com/Picovoice/rhino/tree/master/lib/common).
 
 ## Demos
 
 [picovoicedemo](https://pypi.org/project/picovoicedemo/) provides command-line utilities for processing real-time
 audio (i.e. microphone) and files using Picovoice platform.
+
+
```

### Comparing `picovoice-2.2.0/setup.py` & `picovoice-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,23 +29,23 @@
     f.write('include picovoice/_picovoice.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="picovoice",
-    version="2.2.0",
+    version="2.2.1",
     author="Picovoice Inc.",
     author_email="hello@picovoice.ai",
     description="Picovoice is an end-to-end platform for building voice products on your terms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/picovoice",
     packages=["picovoice"],
-    install_requires=["pvporcupine==2.2.0", "pvrhino==2.2.0"],
+    install_requires=["pvporcupine==2.2.1", "pvrhino==2.2.1"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

