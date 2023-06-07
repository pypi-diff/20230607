# Comparing `tmp/worldvocoder-0.0.0.tar.gz` & `tmp/worldvocoder-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worldvocoder-0.0.0.tar", last modified: Wed Jun  7 19:27:06 2023, max compression
+gzip compressed data, was "worldvocoder-0.0.1.tar", last modified: Wed Jun  7 18:59:46 2023, max compression
```

## Comparing `worldvocoder-0.0.0.tar` & `worldvocoder-0.0.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-06-07 19:27:06.259956 worldvocoder-0.0.0/
--rw-r--r--   0 julianvanasse   (501) staff       (20)     1119 2023-05-27 21:20:51.000000 worldvocoder-0.0.0/LICENSE.txt
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3528 2023-06-07 19:27:06.260008 worldvocoder-0.0.0/PKG-INFO
--rw-r--r--   0 julianvanasse   (501) staff       (20)     2909 2023-06-07 14:24:45.000000 worldvocoder-0.0.0/README.md
--rw-r--r--   0 julianvanasse   (501) staff       (20)      443 2023-06-07 19:26:45.000000 worldvocoder-0.0.0/pyproject.toml
--rw-r--r--   0 julianvanasse   (501) staff       (20)      539 2023-06-07 19:27:06.260235 worldvocoder-0.0.0/setup.cfg
--rw-r--r--   0 julianvanasse   (501) staff       (20)      261 2023-06-07 18:55:58.000000 worldvocoder-0.0.0/setup.py
-drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-06-07 19:27:06.259281 worldvocoder-0.0.0/worldvocoder/
--rw-r--r--   0 julianvanasse   (501) staff       (20)       36 2023-06-07 18:23:35.000000 worldvocoder-0.0.0/worldvocoder/__init__.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     8151 2023-06-07 18:37:40.000000 worldvocoder-0.0.0/worldvocoder/cheaptrick.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    12049 2023-06-07 18:37:53.000000 worldvocoder-0.0.0/worldvocoder/d4c.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    11035 2023-06-04 21:55:46.000000 worldvocoder-0.0.0/worldvocoder/d4cRequiem.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    19600 2023-06-07 18:36:09.000000 worldvocoder-0.0.0/worldvocoder/dio.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3109 2023-06-07 18:38:11.000000 worldvocoder-0.0.0/worldvocoder/get_seeds_signals.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    27287 2023-06-07 13:21:08.000000 worldvocoder-0.0.0/worldvocoder/harvest.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    16426 2023-06-04 21:59:46.000000 worldvocoder-0.0.0/worldvocoder/main.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3371 2023-06-07 18:36:47.000000 worldvocoder-0.0.0/worldvocoder/stonemask.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     5949 2023-05-27 21:20:51.000000 worldvocoder-0.0.0/worldvocoder/swipe.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    10737 2023-05-27 21:20:51.000000 worldvocoder-0.0.0/worldvocoder/synthesis.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     7101 2023-06-07 18:39:12.000000 worldvocoder-0.0.0/worldvocoder/synthesisRequiem.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     9535 2023-05-27 21:20:51.000000 worldvocoder-0.0.0/worldvocoder/synthesis_a.py
-drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-06-07 19:27:06.259847 worldvocoder-0.0.0/worldvocoder.egg-info/
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3528 2023-06-07 19:27:06.000000 worldvocoder-0.0.0/worldvocoder.egg-info/PKG-INFO
--rw-r--r--   0 julianvanasse   (501) staff       (20)      532 2023-06-07 19:27:06.000000 worldvocoder-0.0.0/worldvocoder.egg-info/SOURCES.txt
--rw-r--r--   0 julianvanasse   (501) staff       (20)        1 2023-06-07 19:27:06.000000 worldvocoder-0.0.0/worldvocoder.egg-info/dependency_links.txt
--rw-r--r--   0 julianvanasse   (501) staff       (20)       13 2023-06-07 19:27:06.000000 worldvocoder-0.0.0/worldvocoder.egg-info/top_level.txt
+drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-06-07 18:59:46.919585 worldvocoder-0.0.1/
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     1119 2023-05-27 21:20:51.000000 worldvocoder-0.0.1/LICENSE.txt
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3484 2023-06-07 18:59:46.919679 worldvocoder-0.0.1/PKG-INFO
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     2909 2023-06-07 14:24:45.000000 worldvocoder-0.0.1/README.md
+-rw-r--r--   0 julianvanasse   (501) staff       (20)      539 2023-06-07 18:59:46.920096 worldvocoder-0.0.1/setup.cfg
+-rw-r--r--   0 julianvanasse   (501) staff       (20)      261 2023-06-07 18:55:58.000000 worldvocoder-0.0.1/setup.py
+drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-06-07 18:59:46.918978 worldvocoder-0.0.1/worldvocoder/
+-rw-r--r--   0 julianvanasse   (501) staff       (20)       36 2023-06-07 18:23:35.000000 worldvocoder-0.0.1/worldvocoder/__init__.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     8151 2023-06-07 18:37:40.000000 worldvocoder-0.0.1/worldvocoder/cheaptrick.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    12049 2023-06-07 18:37:53.000000 worldvocoder-0.0.1/worldvocoder/d4c.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    11035 2023-06-04 21:55:46.000000 worldvocoder-0.0.1/worldvocoder/d4cRequiem.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    19600 2023-06-07 18:36:09.000000 worldvocoder-0.0.1/worldvocoder/dio.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3109 2023-06-07 18:38:11.000000 worldvocoder-0.0.1/worldvocoder/get_seeds_signals.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    27287 2023-06-07 13:21:08.000000 worldvocoder-0.0.1/worldvocoder/harvest.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    16426 2023-06-04 21:59:46.000000 worldvocoder-0.0.1/worldvocoder/main.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3371 2023-06-07 18:36:47.000000 worldvocoder-0.0.1/worldvocoder/stonemask.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     5949 2023-05-27 21:20:51.000000 worldvocoder-0.0.1/worldvocoder/swipe.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    10737 2023-05-27 21:20:51.000000 worldvocoder-0.0.1/worldvocoder/synthesis.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     7101 2023-06-07 18:39:12.000000 worldvocoder-0.0.1/worldvocoder/synthesisRequiem.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     9535 2023-05-27 21:20:51.000000 worldvocoder-0.0.1/worldvocoder/synthesis_a.py
+drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-06-07 18:59:46.919484 worldvocoder-0.0.1/worldvocoder.egg-info/
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3484 2023-06-07 18:59:46.000000 worldvocoder-0.0.1/worldvocoder.egg-info/PKG-INFO
+-rw-r--r--   0 julianvanasse   (501) staff       (20)      517 2023-06-07 18:59:46.000000 worldvocoder-0.0.1/worldvocoder.egg-info/SOURCES.txt
+-rw-r--r--   0 julianvanasse   (501) staff       (20)        1 2023-06-07 18:59:46.000000 worldvocoder-0.0.1/worldvocoder.egg-info/dependency_links.txt
+-rw-r--r--   0 julianvanasse   (501) staff       (20)       13 2023-06-07 18:59:46.000000 worldvocoder-0.0.1/worldvocoder.egg-info/top_level.txt
```

### Comparing `worldvocoder-0.0.0/LICENSE.txt` & `worldvocoder-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/PKG-INFO` & `worldvocoder-0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: worldvocoder
-Version: 0.0.0
-Summary: Python implementation of WORLD vocoder.
+Version: 0.0.1
+Summary: Python package for WORLD vocoder
 Home-page: https://github.com/javanasse/Python-WORLD
 Download-URL: https://github.com/javanasse/Python-WORLD/archive/refs/tags/v0.tar.gz
 Author: JulianArmandVanasse
-Author-email: Julian <julian.vanasse@gmail.com>
-Project-URL: Homepage, https://github.com/javanasse/worldvocoder
+Author-email: julian.vanasse@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -102,7 +103,9 @@
 When you want to specify your own ```fft_size```, you have to use ```f0_floor = 3.0 * fs / fft_size```. 
 If you decrease ```fft_size```, the ```f0_floor``` increases. But, a high ```f0_floor``` might be not good for the analysis of male voices.
 
 
 # CITATION:
 
 Dinh, T., Kain, A., & Tjaden, K. (2019). Using a manifold vocoder for spectral voice and style conversion. Proceedings of the Annual Conference of the International Speech Communication Association, INTERSPEECH, 2019-September, 1388-1392.
+
+
```

### Comparing `worldvocoder-0.0.0/README.md` & `worldvocoder-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/setup.cfg` & `worldvocoder-0.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/cheaptrick.py` & `worldvocoder-0.0.1/worldvocoder/cheaptrick.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/d4c.py` & `worldvocoder-0.0.1/worldvocoder/d4c.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/d4cRequiem.py` & `worldvocoder-0.0.1/worldvocoder/d4cRequiem.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/dio.py` & `worldvocoder-0.0.1/worldvocoder/dio.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/get_seeds_signals.py` & `worldvocoder-0.0.1/worldvocoder/get_seeds_signals.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/harvest.py` & `worldvocoder-0.0.1/worldvocoder/harvest.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/main.py` & `worldvocoder-0.0.1/worldvocoder/main.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/stonemask.py` & `worldvocoder-0.0.1/worldvocoder/stonemask.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/swipe.py` & `worldvocoder-0.0.1/worldvocoder/swipe.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/synthesis.py` & `worldvocoder-0.0.1/worldvocoder/synthesis.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/synthesisRequiem.py` & `worldvocoder-0.0.1/worldvocoder/synthesisRequiem.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder/synthesis_a.py` & `worldvocoder-0.0.1/worldvocoder/synthesis_a.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.0/worldvocoder.egg-info/PKG-INFO` & `worldvocoder-0.0.1/worldvocoder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: worldvocoder
-Version: 0.0.0
-Summary: Python implementation of WORLD vocoder.
+Version: 0.0.1
+Summary: Python package for WORLD vocoder
 Home-page: https://github.com/javanasse/Python-WORLD
 Download-URL: https://github.com/javanasse/Python-WORLD/archive/refs/tags/v0.tar.gz
 Author: JulianArmandVanasse
-Author-email: Julian <julian.vanasse@gmail.com>
-Project-URL: Homepage, https://github.com/javanasse/worldvocoder
+Author-email: julian.vanasse@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -102,7 +103,9 @@
 When you want to specify your own ```fft_size```, you have to use ```f0_floor = 3.0 * fs / fft_size```. 
 If you decrease ```fft_size```, the ```f0_floor``` increases. But, a high ```f0_floor``` might be not good for the analysis of male voices.
 
 
 # CITATION:
 
 Dinh, T., Kain, A., & Tjaden, K. (2019). Using a manifold vocoder for spectral voice and style conversion. Proceedings of the Annual Conference of the International Speech Communication Association, INTERSPEECH, 2019-September, 1388-1392.
+
+
```

### Comparing `worldvocoder-0.0.0/worldvocoder.egg-info/SOURCES.txt` & `worldvocoder-0.0.1/worldvocoder.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE.txt
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 worldvocoder/__init__.py
 worldvocoder/cheaptrick.py
 worldvocoder/d4c.py
 worldvocoder/d4cRequiem.py
 worldvocoder/dio.py
```

