# Comparing `tmp/pvcobrademo-1.2.2.tar.gz` & `tmp/pvcobrademo-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvcobrademo-1.2.2.tar", last modified: Tue Apr 11 00:49:22 2023, max compression
+gzip compressed data, was "pvcobrademo-1.2.3.tar", last modified: Wed Jun  7 21:45:13 2023, max compression
```

## Comparing `pvcobrademo-1.2.2.tar` & `pvcobrademo-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:22.449528 pvcobrademo-1.2.2/
--rw-rw-r--   0 eric      (1000) eric      (1000)      105 2023-04-11 00:49:22.000000 pvcobrademo-1.2.2/MANIFEST.in
--rw-rw-r--   0 eric      (1000) eric      (1000)     6091 2023-04-11 00:49:22.449528 pvcobrademo-1.2.2/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     5417 2022-06-07 19:58:39.000000 pvcobrademo-1.2.2/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:22.445528 pvcobrademo-1.2.2/pvcobrademo/
--rw-rw-r--   0 eric      (1000) eric      (1000)    11344 2023-04-11 00:49:22.000000 pvcobrademo-1.2.2/pvcobrademo/LICENSE
--rw-rw-r--   0 eric      (1000) eric      (1000)     2469 2023-04-11 00:49:22.000000 pvcobrademo-1.2.2/pvcobrademo/cobra_demo_file.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4568 2023-04-11 00:49:22.000000 pvcobrademo-1.2.2/pvcobrademo/cobra_demo_mic.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:22.445528 pvcobrademo-1.2.2/pvcobrademo.egg-info/
--rw-rw-r--   0 eric      (1000) eric      (1000)     6091 2023-04-11 00:49:22.000000 pvcobrademo-1.2.2/pvcobrademo.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)      323 2023-04-11 00:49:22.000000 pvcobrademo-1.2.2/pvcobrademo.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-04-11 00:49:22.000000 pvcobrademo-1.2.2/pvcobrademo.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      119 2023-04-11 00:49:22.000000 pvcobrademo-1.2.2/pvcobrademo.egg-info/entry_points.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       33 2023-04-11 00:49:22.000000 pvcobrademo-1.2.2/pvcobrademo.egg-info/requires.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       12 2023-04-11 00:49:22.000000 pvcobrademo-1.2.2/pvcobrademo.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-04-11 00:49:22.449528 pvcobrademo-1.2.2/setup.cfg
--rw-rw-r--   0 eric      (1000) eric      (1000)     1937 2023-04-11 00:48:54.000000 pvcobrademo-1.2.2/setup.py
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:45:13.859469 pvcobrademo-1.2.3/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      105 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/MANIFEST.in
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6091 2023-06-07 21:45:13.859469 pvcobrademo-1.2.3/PKG-INFO
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     5417 2023-06-07 20:46:18.000000 pvcobrademo-1.2.3/README.md
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:45:13.859469 pvcobrademo-1.2.3/pvcobrademo/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)    11344 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo/LICENSE
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     2469 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo/cobra_demo_file.py
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     4556 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo/cobra_demo_mic.py
+drwxrwxr-x   0 kyeo      (1000) kyeo      (1000)        0 2023-06-07 21:45:13.859469 pvcobrademo-1.2.3/pvcobrademo.egg-info/
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     6091 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/PKG-INFO
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      323 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)        1 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)      119 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/entry_points.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       33 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/requires.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       12 2023-06-07 21:45:13.000000 pvcobrademo-1.2.3/pvcobrademo.egg-info/top_level.txt
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)       38 2023-06-07 21:45:13.859469 pvcobrademo-1.2.3/setup.cfg
+-rw-rw-r--   0 kyeo      (1000) kyeo      (1000)     1937 2023-06-07 21:44:56.000000 pvcobrademo-1.2.3/setup.py
```

### Comparing `pvcobrademo-1.2.2/PKG-INFO` & `pvcobrademo-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvcobrademo
-Version: 1.2.2
+Version: 1.2.3
 Summary: Cobra voice activity detection (VAD) engine demos.
 Home-page: https://github.com/Picovoice/cobra
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
 Keywords: voice activity detection engine,VAD
 Platform: UNKNOWN
```

### Comparing `pvcobrademo-1.2.2/README.md` & `pvcobrademo-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pvcobrademo-1.2.2/pvcobrademo/LICENSE` & `pvcobrademo-1.2.3/pvcobrademo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvcobrademo-1.2.2/pvcobrademo/cobra_demo_file.py` & `pvcobrademo-1.2.3/pvcobrademo/cobra_demo_file.py`

 * *Files identical despite different names*

### Comparing `pvcobrademo-1.2.2/pvcobrademo/cobra_demo_mic.py` & `pvcobrademo-1.2.3/pvcobrademo/cobra_demo_mic.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             print('Stopping ...')
         finally:
             if cobra is not None:
                 cobra.delete()
 
             if wav_file is not None:
                 wav_file.close()
-            
+
             if recorder is not None:
                 recorder.delete()
 
     @classmethod
     def show_audio_devices(cls):
         devices = PvRecorder.get_audio_devices()
         for i in range(len(devices)):
```

### Comparing `pvcobrademo-1.2.2/pvcobrademo.egg-info/PKG-INFO` & `pvcobrademo-1.2.3/pvcobrademo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvcobrademo
-Version: 1.2.2
+Version: 1.2.3
 Summary: Cobra voice activity detection (VAD) engine demos.
 Home-page: https://github.com/Picovoice/cobra
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
 Keywords: voice activity detection engine,VAD
 Platform: UNKNOWN
```

### Comparing `pvcobrademo-1.2.2/setup.py` & `pvcobrademo-1.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     f.write('include pvcobrademo/cobra_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvcobrademo",
-    version="1.2.2",
+    version="1.2.3",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Cobra voice activity detection (VAD) engine demos.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/cobra",
     packages=["pvcobrademo"],
-    install_requires=["pvcobra==1.2.1", "pvrecorder==1.1.1"],
+    install_requires=["pvcobra==1.2.2", "pvrecorder==1.1.1"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

