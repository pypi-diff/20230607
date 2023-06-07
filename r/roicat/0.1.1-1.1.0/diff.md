# Comparing `tmp/roicat-0.1.1.tar.gz` & `tmp/roicat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roicat-0.1.1.tar", last modified: Wed Jun  7 17:30:16 2023, max compression
+gzip compressed data, was "roicat-1.1.0.tar", last modified: Wed Jun  7 17:40:43 2023, max compression
```

## Comparing `roicat-0.1.1.tar` & `roicat-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 17:30:16.797247 roicat-0.1.1/
--rw-rw-rw-   0        0        0    34895 2023-06-07 16:45:57.000000 roicat-0.1.1/LICENSE.md
--rw-rw-rw-   0        0        0       24 2023-06-07 16:09:48.000000 roicat-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      435 2023-06-07 17:30:16.797247 roicat-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8511 2023-06-07 16:09:48.000000 roicat-0.1.1/README.md
--rw-rw-rw-   0        0        0     8511 2023-06-07 17:09:41.000000 roicat-0.1.1/README.rst
--rw-rw-rw-   0        0        0      406 2023-06-07 16:09:49.000000 roicat-0.1.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 17:30:16.748996 roicat-0.1.1/roicat/
--rw-rw-rw-   0        0        0    38841 2023-06-07 16:09:49.000000 roicat-0.1.1/roicat/ROInet.py
--rw-rw-rw-   0        0        0      252 2023-06-07 17:29:41.000000 roicat-0.1.1/roicat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:30:16.772812 roicat-0.1.1/roicat/classification/
--rw-rw-rw-   0        0        0     5631 2023-06-07 16:09:49.000000 roicat-0.1.1/roicat/classification/crossval.py
--rw-rw-rw-   0        0        0    11175 2023-05-09 14:53:52.000000 roicat-0.1.1/roicat/classification/data.py
--rw-rw-rw-   0        0        0     1454 2023-05-09 14:53:52.000000 roicat-0.1.1/roicat/classification/evaluate.py
--rw-rw-rw-   0        0        0     5478 2023-05-09 14:53:52.000000 roicat-0.1.1/roicat/classification/pipeline.py
--rw-rw-rw-   0        0        0      359 2023-05-09 14:53:52.000000 roicat-0.1.1/roicat/classification/visualization.py
--rw-rw-rw-   0        0        0    68978 2023-06-07 16:09:49.000000 roicat-0.1.1/roicat/data_importing.py
--rw-rw-rw-   0        0        0   107152 2023-06-07 16:09:49.000000 roicat-0.1.1/roicat/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:30:16.772812 roicat-0.1.1/roicat/model_training/
--rw-rw-rw-   0        0        0       92 2023-05-09 14:53:52.000000 roicat-0.1.1/roicat/model_training/__init__.py
--rw-rw-rw-   0        0        0    17479 2023-05-09 14:53:52.000000 roicat-0.1.1/roicat/model_training/augmentation.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:30:16.789007 roicat-0.1.1/roicat/tracking/
--rw-rw-rw-   0        0        0      187 2023-05-09 14:53:52.000000 roicat-0.1.1/roicat/tracking/__init__.py
--rw-rw-rw-   0        0        0    35543 2023-06-07 16:09:49.000000 roicat-0.1.1/roicat/tracking/alignment.py
--rw-rw-rw-   0        0        0     7976 2023-06-07 16:09:49.000000 roicat-0.1.1/roicat/tracking/blurring.py
--rw-rw-rw-   0        0        0    62691 2023-06-07 16:09:49.000000 roicat-0.1.1/roicat/tracking/clustering.py
--rw-rw-rw-   0        0        0     2791 2023-06-07 16:09:49.000000 roicat-0.1.1/roicat/tracking/scatteringWaveletTransformer.py
--rw-rw-rw-   0        0        0    25679 2023-06-07 16:09:49.000000 roicat-0.1.1/roicat/tracking/similarity_graph.py
--rw-rw-rw-   0        0        0    38642 2023-06-07 16:09:49.000000 roicat-0.1.1/roicat/util.py
--rw-rw-rw-   0        0        0    12285 2023-06-07 16:09:49.000000 roicat-0.1.1/roicat/visualization.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:30:16.756504 roicat-0.1.1/roicat.egg-info/
--rw-rw-rw-   0        0        0      435 2023-06-07 17:30:16.000000 roicat-0.1.1/roicat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      788 2023-06-07 17:30:16.000000 roicat-0.1.1/roicat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 17:30:16.000000 roicat-0.1.1/roicat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1577 2023-06-07 17:30:16.000000 roicat-0.1.1/roicat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-07 17:30:16.000000 roicat-0.1.1/roicat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       87 2023-06-07 17:30:16.797247 roicat-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3846 2023-06-07 17:30:07.000000 roicat-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:40:43.103210 roicat-1.1.0/
+-rw-rw-rw-   0        0        0    34895 2023-06-07 16:45:57.000000 roicat-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0       24 2023-06-07 16:09:48.000000 roicat-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8976 2023-06-07 17:40:43.103210 roicat-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8511 2023-06-07 16:09:48.000000 roicat-1.1.0/README.md
+-rw-rw-rw-   0        0        0     8511 2023-06-07 17:09:41.000000 roicat-1.1.0/README.rst
+-rw-rw-rw-   0        0        0      406 2023-06-07 16:09:49.000000 roicat-1.1.0/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 17:40:43.062298 roicat-1.1.0/roicat/
+-rw-rw-rw-   0        0        0    38841 2023-06-07 16:09:49.000000 roicat-1.1.0/roicat/ROInet.py
+-rw-rw-rw-   0        0        0      252 2023-06-07 17:40:38.000000 roicat-1.1.0/roicat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:40:43.078628 roicat-1.1.0/roicat/classification/
+-rw-rw-rw-   0        0        0     5631 2023-06-07 16:09:49.000000 roicat-1.1.0/roicat/classification/crossval.py
+-rw-rw-rw-   0        0        0    11175 2023-05-09 14:53:52.000000 roicat-1.1.0/roicat/classification/data.py
+-rw-rw-rw-   0        0        0     1454 2023-05-09 14:53:52.000000 roicat-1.1.0/roicat/classification/evaluate.py
+-rw-rw-rw-   0        0        0     5478 2023-05-09 14:53:52.000000 roicat-1.1.0/roicat/classification/pipeline.py
+-rw-rw-rw-   0        0        0      359 2023-05-09 14:53:52.000000 roicat-1.1.0/roicat/classification/visualization.py
+-rw-rw-rw-   0        0        0    68978 2023-06-07 16:09:49.000000 roicat-1.1.0/roicat/data_importing.py
+-rw-rw-rw-   0        0        0   107152 2023-06-07 16:09:49.000000 roicat-1.1.0/roicat/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:40:43.087036 roicat-1.1.0/roicat/model_training/
+-rw-rw-rw-   0        0        0       92 2023-05-09 14:53:52.000000 roicat-1.1.0/roicat/model_training/__init__.py
+-rw-rw-rw-   0        0        0    17479 2023-05-09 14:53:52.000000 roicat-1.1.0/roicat/model_training/augmentation.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:40:43.095196 roicat-1.1.0/roicat/tracking/
+-rw-rw-rw-   0        0        0      187 2023-05-09 14:53:52.000000 roicat-1.1.0/roicat/tracking/__init__.py
+-rw-rw-rw-   0        0        0    35543 2023-06-07 16:09:49.000000 roicat-1.1.0/roicat/tracking/alignment.py
+-rw-rw-rw-   0        0        0     7976 2023-06-07 16:09:49.000000 roicat-1.1.0/roicat/tracking/blurring.py
+-rw-rw-rw-   0        0        0    62691 2023-06-07 16:09:49.000000 roicat-1.1.0/roicat/tracking/clustering.py
+-rw-rw-rw-   0        0        0     2791 2023-06-07 16:09:49.000000 roicat-1.1.0/roicat/tracking/scatteringWaveletTransformer.py
+-rw-rw-rw-   0        0        0    25679 2023-06-07 16:09:49.000000 roicat-1.1.0/roicat/tracking/similarity_graph.py
+-rw-rw-rw-   0        0        0    38642 2023-06-07 16:09:49.000000 roicat-1.1.0/roicat/util.py
+-rw-rw-rw-   0        0        0    12285 2023-06-07 16:09:49.000000 roicat-1.1.0/roicat/visualization.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:40:43.070316 roicat-1.1.0/roicat.egg-info/
+-rw-rw-rw-   0        0        0     8976 2023-06-07 17:40:42.000000 roicat-1.1.0/roicat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      788 2023-06-07 17:40:42.000000 roicat-1.1.0/roicat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 17:40:42.000000 roicat-1.1.0/roicat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1577 2023-06-07 17:40:42.000000 roicat-1.1.0/roicat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-07 17:40:42.000000 roicat-1.1.0/roicat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       87 2023-06-07 17:40:43.103210 roicat-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3893 2023-06-07 17:39:37.000000 roicat-1.1.0/setup.py
```

### Comparing `roicat-0.1.1/LICENSE.md` & `roicat-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/README.md` & `roicat-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/README.rst` & `roicat-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/ROInet.py` & `roicat-1.1.0/roicat/ROInet.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/classification/crossval.py` & `roicat-1.1.0/roicat/classification/crossval.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/classification/data.py` & `roicat-1.1.0/roicat/classification/data.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/classification/evaluate.py` & `roicat-1.1.0/roicat/classification/evaluate.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/classification/pipeline.py` & `roicat-1.1.0/roicat/classification/pipeline.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/data_importing.py` & `roicat-1.1.0/roicat/data_importing.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/helpers.py` & `roicat-1.1.0/roicat/helpers.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/model_training/augmentation.py` & `roicat-1.1.0/roicat/model_training/augmentation.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/tracking/alignment.py` & `roicat-1.1.0/roicat/tracking/alignment.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/tracking/blurring.py` & `roicat-1.1.0/roicat/tracking/blurring.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/tracking/clustering.py` & `roicat-1.1.0/roicat/tracking/clustering.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/tracking/scatteringWaveletTransformer.py` & `roicat-1.1.0/roicat/tracking/scatteringWaveletTransformer.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/tracking/similarity_graph.py` & `roicat-1.1.0/roicat/tracking/similarity_graph.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/util.py` & `roicat-1.1.0/roicat/util.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat/visualization.py` & `roicat-1.1.0/roicat/visualization.py`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat.egg-info/SOURCES.txt` & `roicat-1.1.0/roicat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/roicat.egg-info/requires.txt` & `roicat-1.1.0/roicat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `roicat-0.1.1/setup.py` & `roicat-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -112,15 +112,16 @@
 setup(
     name='roicat',
     version=version,
     author='Richard Hakim',
     keywords=['neuroscience', 'neuroimaging', 'machine learning', 'deep learning'],
     license='LICENSE',
     description='A library for classifying and tracking ROIs.',
-    long_description='README.md',
+    long_description=readme,
+    long_description_content_type="text/markdown",
     url='https://github.com/RichieHakim/ROICaT',
 
     packages=[
         'roicat',
         'roicat.tracking',
         'roicat.classification',
         'roicat.model_training',
```

