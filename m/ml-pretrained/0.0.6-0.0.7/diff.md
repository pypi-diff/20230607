# Comparing `tmp/ml-pretrained-0.0.6.tar.gz` & `tmp/ml-pretrained-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-pretrained-0.0.6.tar", last modified: Wed Jun  7 03:11:50 2023, max compression
+gzip compressed data, was "ml-pretrained-0.0.7.tar", last modified: Wed Jun  7 03:34:58 2023, max compression
```

## Comparing `ml-pretrained-0.0.6.tar` & `ml-pretrained-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:50.579413 ml-pretrained-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:11:50.579413 ml-pretrained-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:50.575413 ml-pretrained-0.0.6/ml_pretrained.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:11:50.000000 ml-pretrained-0.0.6/ml_pretrained.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-07 03:11:50.000000 ml-pretrained-0.0.6/ml_pretrained.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:11:50.000000 ml-pretrained-0.0.6/ml_pretrained.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 03:11:50.000000 ml-pretrained-0.0.6/ml_pretrained.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 03:11:50.000000 ml-pretrained-0.0.6/ml_pretrained.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:50.575413 ml-pretrained-0.0.6/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/tacotron2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:50.575413 ml-pretrained-0.0.6/pretrained/vocoder/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/vocoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/vocoder/hifigan.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/vocoder/waveglow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 03:11:50.579413 ml-pretrained-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:50.579413 ml-pretrained-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/tests/test_rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/tests/test_tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/ml_pretrained.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:34:58.000000 ml-pretrained-0.0.7/ml_pretrained.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-07 03:34:58.000000 ml-pretrained-0.0.7/ml_pretrained.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:34:58.000000 ml-pretrained-0.0.7/ml_pretrained.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 03:34:58.000000 ml-pretrained-0.0.7/ml_pretrained.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 03:34:58.000000 ml-pretrained-0.0.7/ml_pretrained.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/pretrained/vocoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/vocoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/vocoder/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/vocoder/waveglow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 03:34:58.120495 ml-pretrained-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/tests/test_rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/tests/test_tacotron2.py
```

### Comparing `ml-pretrained-0.0.6/LICENSE` & `ml-pretrained-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/PKG-INFO` & `ml-pretrained-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.6
+Version: 0.0.7
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.6/README.md` & `ml-pretrained-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/ml_pretrained.egg-info/PKG-INFO` & `ml-pretrained-0.0.7/ml_pretrained.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.6
+Version: 0.0.7
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.6/ml_pretrained.egg-info/SOURCES.txt` & `ml-pretrained-0.0.7/ml_pretrained.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/pretrained/blip.py` & `ml-pretrained-0.0.7/pretrained/blip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/pretrained/clip.py` & `ml-pretrained-0.0.7/pretrained/clip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/pretrained/hubert.py` & `ml-pretrained-0.0.7/pretrained/hubert.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/pretrained/llama.py` & `ml-pretrained-0.0.7/pretrained/llama.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/pretrained/rwkv.py` & `ml-pretrained-0.0.7/pretrained/rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/pretrained/sam.py` & `ml-pretrained-0.0.7/pretrained/sam.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/pretrained/tacotron2.py` & `ml-pretrained-0.0.7/pretrained/tacotron2.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/pretrained/vocoder/__init__.py` & `ml-pretrained-0.0.7/pretrained/vocoder/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/pretrained/vocoder/hifigan.py` & `ml-pretrained-0.0.7/pretrained/vocoder/hifigan.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/pretrained/vocoder/waveglow.py` & `ml-pretrained-0.0.7/pretrained/vocoder/waveglow.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/pyproject.toml` & `ml-pretrained-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/setup.py` & `ml-pretrained-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,9 +30,9 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
     python_requires=">=3.10",
     install_requires=["ml-starter"],
     tests_require=["ml-starter[dev]"],
     extras_require={"dev": ["ml-starter[dev]"], "docs": ["ml-starter[docs]"]},
-    package_data={"ml": ["py.typed"]},
+    package_data={"pretrained": ["py.typed"]},
 )
```

### Comparing `ml-pretrained-0.0.6/tests/test_rwkv.py` & `ml-pretrained-0.0.7/tests/test_rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.6/tests/test_tacotron2.py` & `ml-pretrained-0.0.7/tests/test_tacotron2.py`

 * *Files identical despite different names*

