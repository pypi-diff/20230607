# Comparing `tmp/openvino_model_api-0.1.1.tar.gz` & `tmp/openvino_model_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvino_model_api-0.1.1.tar", last modified: Mon Jun  5 10:38:12 2023, max compression
+gzip compressed data, was "openvino_model_api-0.1.2.tar", last modified: Wed Jun  7 12:34:17 2023, max compression
```

## Comparing `openvino_model_api-0.1.1.tar` & `openvino_model_api-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 wov       (1000) wov       (1000)        0 2023-06-05 10:38:12.389157 openvino_model_api-0.1.1/
--rw-rw-r--   0 wov       (1000) wov       (1000)     6935 2023-06-05 10:38:12.389157 openvino_model_api-0.1.1/PKG-INFO
-drwxrwxr-x   0 wov       (1000) wov       (1000)        0 2023-06-05 10:38:12.389157 openvino_model_api-0.1.1/openvino_model_api.egg-info/
--rw-rw-r--   0 wov       (1000) wov       (1000)     6935 2023-06-05 10:38:12.000000 openvino_model_api-0.1.1/openvino_model_api.egg-info/PKG-INFO
--rw-rw-r--   0 wov       (1000) wov       (1000)     2996 2023-06-05 10:38:12.000000 openvino_model_api-0.1.1/openvino_model_api.egg-info/SOURCES.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)        1 2023-06-05 10:38:12.000000 openvino_model_api-0.1.1/openvino_model_api.egg-info/dependency_links.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)      157 2023-06-05 10:38:12.000000 openvino_model_api-0.1.1/openvino_model_api.egg-info/requires.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)        9 2023-06-05 10:38:12.000000 openvino_model_api-0.1.1/openvino_model_api.egg-info/top_level.txt
--rw-rw-r--   0 wov       (1000) wov       (1000)       38 2023-06-05 10:38:12.389157 openvino_model_api-0.1.1/setup.cfg
--rwxrwxr-x   0 wov       (1000) wov       (1000)     1636 2023-06-05 10:34:46.000000 openvino_model_api-0.1.1/setup.py
+drwxrwxr-x   0 wov       (1000) wov       (1000)        0 2023-06-07 12:34:17.423834 openvino_model_api-0.1.2/
+-rw-rw-r--   0 wov       (1000) wov       (1000)     6935 2023-06-07 12:34:17.423834 openvino_model_api-0.1.2/PKG-INFO
+drwxrwxr-x   0 wov       (1000) wov       (1000)        0 2023-06-07 12:34:17.423834 openvino_model_api-0.1.2/openvino_model_api.egg-info/
+-rw-rw-r--   0 wov       (1000) wov       (1000)     6935 2023-06-07 12:34:17.000000 openvino_model_api-0.1.2/openvino_model_api.egg-info/PKG-INFO
+-rw-rw-r--   0 wov       (1000) wov       (1000)     2996 2023-06-07 12:34:17.000000 openvino_model_api-0.1.2/openvino_model_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 wov       (1000) wov       (1000)        1 2023-06-07 12:34:17.000000 openvino_model_api-0.1.2/openvino_model_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 wov       (1000) wov       (1000)      157 2023-06-07 12:34:17.000000 openvino_model_api-0.1.2/openvino_model_api.egg-info/requires.txt
+-rw-rw-r--   0 wov       (1000) wov       (1000)        9 2023-06-07 12:34:17.000000 openvino_model_api-0.1.2/openvino_model_api.egg-info/top_level.txt
+-rw-rw-r--   0 wov       (1000) wov       (1000)       38 2023-06-07 12:34:17.423834 openvino_model_api-0.1.2/setup.cfg
+-rwxrwxr-x   0 wov       (1000) wov       (1000)     1636 2023-06-07 09:20:54.000000 openvino_model_api-0.1.2/setup.py
```

### Comparing `openvino_model_api-0.1.1/PKG-INFO` & `openvino_model_api-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openvino_model_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Model API: model wrappers and pipelines for inference with OpenVINO
 Home-page: https://github.com/openvinotoolkit/model_api
 Author: Intel(R) Corporation
 License: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `openvino_model_api-0.1.1/openvino_model_api.egg-info/PKG-INFO` & `openvino_model_api-0.1.2/openvino_model_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openvino-model-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Model API: model wrappers and pipelines for inference with OpenVINO
 Home-page: https://github.com/openvinotoolkit/model_api
 Author: Intel(R) Corporation
 License: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `openvino_model_api-0.1.1/openvino_model_api.egg-info/SOURCES.txt` & `openvino_model_api-0.1.2/openvino_model_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openvino_model_api-0.1.1/setup.py` & `openvino_model_api-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from setuptools import find_packages, setup
 
 SETUP_DIR = Path(__file__).resolve().parent
 
 setup(
     name="openvino_model_api",
-    version="0.1.1",
+    version="0.1.2",
     description="Model API: model wrappers and pipelines for inference with OpenVINO",
     author="Intel(R) Corporation",
     url="https://github.com/openvinotoolkit/model_api",
     packages=find_packages(SETUP_DIR),
     package_dir={"openvino": str(SETUP_DIR / "openvino")},
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
```

