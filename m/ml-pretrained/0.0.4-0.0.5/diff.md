# Comparing `tmp/ml-pretrained-0.0.4.tar.gz` & `tmp/ml-pretrained-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-pretrained-0.0.4.tar", last modified: Wed Jun  7 02:47:10 2023, max compression
+gzip compressed data, was "ml-pretrained-0.0.5.tar", last modified: Wed Jun  7 03:04:08 2023, max compression
```

## Comparing `ml-pretrained-0.0.4.tar` & `ml-pretrained-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:47:10.512313 ml-pretrained-0.0.4/ml_pretrained.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 02:47:10.000000 ml-pretrained-0.0.4/ml_pretrained.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 02:47:10.000000 ml-pretrained-0.0.4/ml_pretrained.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:47:10.000000 ml-pretrained-0.0.4/ml_pretrained.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 02:47:10.000000 ml-pretrained-0.0.4/ml_pretrained.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 02:47:10.000000 ml-pretrained-0.0.4/ml_pretrained.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/tacotron2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/pretrained/vocoder/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/vocoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/vocoder/hifigan.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/vocoder/waveglow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/tests/test_rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/tests/test_tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:04:08.674118 ml-pretrained-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:04:08.674118 ml-pretrained-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:04:08.670118 ml-pretrained-0.0.5/ml_pretrained.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:04:08.000000 ml-pretrained-0.0.5/ml_pretrained.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-07 03:04:08.000000 ml-pretrained-0.0.5/ml_pretrained.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:04:08.000000 ml-pretrained-0.0.5/ml_pretrained.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 03:04:08.000000 ml-pretrained-0.0.5/ml_pretrained.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 03:04:08.000000 ml-pretrained-0.0.5/ml_pretrained.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:04:08.670118 ml-pretrained-0.0.5/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:04:08.670118 ml-pretrained-0.0.5/pretrained/vocoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/vocoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/vocoder/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/vocoder/waveglow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 03:04:08.674118 ml-pretrained-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:04:08.674118 ml-pretrained-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/tests/test_rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/tests/test_tacotron2.py
```

### Comparing `ml-pretrained-0.0.4/LICENSE` & `ml-pretrained-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/PKG-INFO` & `ml-pretrained-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.4
+Version: 0.0.5
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.4/README.md` & `ml-pretrained-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/ml_pretrained.egg-info/PKG-INFO` & `ml-pretrained-0.0.5/ml_pretrained.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.4
+Version: 0.0.5
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.4/ml_pretrained.egg-info/SOURCES.txt` & `ml-pretrained-0.0.5/ml_pretrained.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ml_pretrained.egg-info/requires.txt
 ml_pretrained.egg-info/top_level.txt
 pretrained/__init__.py
 pretrained/blip.py
 pretrained/clip.py
 pretrained/hubert.py
 pretrained/llama.py
+pretrained/py.typed
 pretrained/rwkv.py
 pretrained/sam.py
 pretrained/tacotron2.py
 pretrained/vocoder/__init__.py
 pretrained/vocoder/hifigan.py
 pretrained/vocoder/waveglow.py
 tests/test_rwkv.py
```

### Comparing `ml-pretrained-0.0.4/pretrained/blip.py` & `ml-pretrained-0.0.5/pretrained/blip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/pretrained/clip.py` & `ml-pretrained-0.0.5/pretrained/clip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/pretrained/hubert.py` & `ml-pretrained-0.0.5/pretrained/hubert.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/pretrained/llama.py` & `ml-pretrained-0.0.5/pretrained/llama.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/pretrained/rwkv.py` & `ml-pretrained-0.0.5/pretrained/rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/pretrained/sam.py` & `ml-pretrained-0.0.5/pretrained/sam.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/pretrained/tacotron2.py` & `ml-pretrained-0.0.5/pretrained/tacotron2.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/pretrained/vocoder/__init__.py` & `ml-pretrained-0.0.5/pretrained/vocoder/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/pretrained/vocoder/hifigan.py` & `ml-pretrained-0.0.5/pretrained/vocoder/hifigan.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/pretrained/vocoder/waveglow.py` & `ml-pretrained-0.0.5/pretrained/vocoder/waveglow.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/pyproject.toml` & `ml-pretrained-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/setup.py` & `ml-pretrained-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/tests/test_rwkv.py` & `ml-pretrained-0.0.5/tests/test_rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.4/tests/test_tacotron2.py` & `ml-pretrained-0.0.5/tests/test_tacotron2.py`

 * *Files identical despite different names*

