# Comparing `tmp/datasieve-0.1.3.tar.gz` & `tmp/datasieve-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.1.3.tar", max compression
+gzip compressed data, was "datasieve-0.1.4.tar", max compression
```

## Comparing `datasieve-0.1.3.tar` & `datasieve-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1059 2023-06-07 16:31:26.108443 datasieve-0.1.3/LICENSE
--rw-r--r--   0        0        0    11780 2023-06-07 16:31:26.108443 datasieve-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/__init__.py
--rw-r--r--   0        0        0     8427 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/pipeline.py
--rw-r--r--   0        0        0      567 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0     3228 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/base_transform.py
--rw-r--r--   0        0        0     5683 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     2748 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1357 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/noise.py
--rw-r--r--   0        0        0     1432 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1191 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/sklearn_wrapper.py
--rw-r--r--   0        0        0     1621 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1453 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     3275 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/utils.py
--rw-r--r--   0        0        0      544 2023-06-07 16:31:26.112444 datasieve-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    12406 1970-01-01 00:00:00.000000 datasieve-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-06-07 17:23:26.771074 datasieve-0.1.4/LICENSE
+-rw-r--r--   0        0        0    11780 2023-06-07 17:23:26.771074 datasieve-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/__init__.py
+-rw-r--r--   0        0        0     8427 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/pipeline.py
+-rw-r--r--   0        0        0      567 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0     3228 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/base_transform.py
+-rw-r--r--   0        0        0     5683 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     2748 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1357 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/noise.py
+-rw-r--r--   0        0        0     1432 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1191 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/sklearn_wrapper.py
+-rw-r--r--   0        0        0     1621 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1453 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     3275 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/utils.py
+-rw-r--r--   0        0        0      544 2023-06-07 17:23:26.771074 datasieve-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    12406 1970-01-01 00:00:00.000000 datasieve-0.1.4/PKG-INFO
```

### Comparing `datasieve-0.1.3/LICENSE` & `datasieve-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/README.md` & `datasieve-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/datasieve/pipeline.py` & `datasieve-0.1.4/datasieve/pipeline.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/datasieve/transforms/__init__.py` & `datasieve-0.1.4/datasieve/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/datasieve/transforms/base_transform.py` & `datasieve-0.1.4/datasieve/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/datasieve/transforms/dbscan.py` & `datasieve-0.1.4/datasieve/transforms/dbscan.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.1.4/datasieve/transforms/dissimilarity_index.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/datasieve/transforms/noise.py` & `datasieve-0.1.4/datasieve/transforms/noise.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/datasieve/transforms/pca.py` & `datasieve-0.1.4/datasieve/transforms/pca.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/datasieve/transforms/sklearn_wrapper.py` & `datasieve-0.1.4/datasieve/transforms/sklearn_wrapper.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/datasieve/transforms/svm_outlier_extractor.py` & `datasieve-0.1.4/datasieve/transforms/svm_outlier_extractor.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/datasieve/transforms/variance_threshold.py` & `datasieve-0.1.4/datasieve/transforms/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/datasieve/utils.py` & `datasieve-0.1.4/datasieve/utils.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.3/pyproject.toml` & `datasieve-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "datasieve"
-version = "0.1.3"
+version = "0.1.4"
 description = "This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)"
 authors = ['Robert Caulk']
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 scikit-learn = ">=1.1.3"
-pandas = ">=1.3.3"
+pandas = "==2.0.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 autopep8 = "1.6.0"
 flake8 = "^6.0.0"
```

### Comparing `datasieve-0.1.3/PKG-INFO` & `datasieve-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: datasieve
-Version: 0.1.3
+Version: 0.1.4
 Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
 License: MIT
 Author: Robert Caulk
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=1.3.3)
+Requires-Dist: pandas (==2.0.2)
 Requires-Dist: scikit-learn (>=1.1.3)
 Description-Content-Type: text/markdown
 
 # DataSieve
 
 DataSieve is very similar to the SKlearn Pipeline in that it:
```

