# Comparing `tmp/moosez-2.0.2.tar.gz` & `tmp/moosez-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.0.2.tar", last modified: Tue Jun  6 16:03:40 2023, max compression
+gzip compressed data, was "moosez-2.0.3.tar", last modified: Wed Jun  7 12:41:23 2023, max compression
```

## Comparing `moosez-2.0.2.tar` & `moosez-2.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 16:03:40.591980 moosez-2.0.2/
--rw-r--r--   0 lalithsimac   (501) staff       (20)    11357 2023-06-06 13:31:59.000000 moosez-2.0.2/LICENSE
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1404 2023-06-06 16:03:40.591772 moosez-2.0.2/PKG-INFO
--rw-r--r--   0 lalithsimac   (501) staff       (20)    19071 2023-06-06 13:31:59.000000 moosez-2.0.2/README.md
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 16:03:40.590163 moosez-2.0.2/moosez/
--rw-r--r--   0 lalithsimac   (501) staff       (20)      227 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/__init__.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1362 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/constants.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     7161 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/display.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3662 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/download.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4119 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/file_utilities.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4002 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/image_conversion.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3416 2023-06-06 15:07:22.000000 moosez-2.0.2/moosez/image_processing.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4163 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/input_validation.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     7781 2023-06-06 15:53:20.000000 moosez-2.0.2/moosez/moosez.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     5974 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/predict.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3090 2023-06-06 13:31:59.000000 moosez-2.0.2/moosez/resources.py
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-06 16:03:40.591475 moosez-2.0.2/moosez.egg-info/
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1404 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/PKG-INFO
--rw-r--r--   0 lalithsimac   (501) staff       (20)      445 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)        1 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)       47 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/entry_points.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)      234 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/requires.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)        7 2023-06-06 16:03:40.000000 moosez-2.0.2/moosez.egg-info/top_level.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)       38 2023-06-06 16:03:40.592056 moosez-2.0.2/setup.cfg
--rw-r--r--   0 lalithsimac   (501) staff       (20)     2178 2023-06-06 16:03:09.000000 moosez-2.0.2/setup.py
+drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-07 12:41:23.327851 moosez-2.0.3/
+-rw-r--r--   0 lalithsimac   (501) staff       (20)    11357 2023-06-06 13:31:59.000000 moosez-2.0.3/LICENSE
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     1427 2023-06-07 12:41:23.327445 moosez-2.0.3/PKG-INFO
+-rw-r--r--   0 lalithsimac   (501) staff       (20)    19071 2023-06-06 13:31:59.000000 moosez-2.0.3/README.md
+drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-07 12:41:23.324025 moosez-2.0.3/moosez/
+-rw-r--r--   0 lalithsimac   (501) staff       (20)      227 2023-06-06 13:31:59.000000 moosez-2.0.3/moosez/__init__.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     1362 2023-06-06 13:31:59.000000 moosez-2.0.3/moosez/constants.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     5434 2023-06-07 12:38:35.000000 moosez-2.0.3/moosez/display.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     3662 2023-06-06 13:31:59.000000 moosez-2.0.3/moosez/download.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     4119 2023-06-06 13:31:59.000000 moosez-2.0.3/moosez/file_utilities.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     4002 2023-06-06 13:31:59.000000 moosez-2.0.3/moosez/image_conversion.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     3416 2023-06-06 15:07:22.000000 moosez-2.0.3/moosez/image_processing.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     4163 2023-06-06 13:31:59.000000 moosez-2.0.3/moosez/input_validation.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     7392 2023-06-07 12:38:35.000000 moosez-2.0.3/moosez/moosez.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     5974 2023-06-06 13:31:59.000000 moosez-2.0.3/moosez/predict.py
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     3090 2023-06-06 13:31:59.000000 moosez-2.0.3/moosez/resources.py
+drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-07 12:41:23.326854 moosez-2.0.3/moosez.egg-info/
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     1427 2023-06-07 12:41:23.000000 moosez-2.0.3/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 lalithsimac   (501) staff       (20)      445 2023-06-07 12:41:23.000000 moosez-2.0.3/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)        1 2023-06-07 12:41:23.000000 moosez-2.0.3/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)       47 2023-06-07 12:41:23.000000 moosez-2.0.3/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)      234 2023-06-07 12:41:23.000000 moosez-2.0.3/moosez.egg-info/requires.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)        7 2023-06-07 12:41:23.000000 moosez-2.0.3/moosez.egg-info/top_level.txt
+-rw-r--r--   0 lalithsimac   (501) staff       (20)       38 2023-06-07 12:41:23.327991 moosez-2.0.3/setup.cfg
+-rw-r--r--   0 lalithsimac   (501) staff       (20)     2207 2023-06-07 12:40:12.000000 moosez-2.0.3/setup.py
```

### Comparing `moosez-2.0.2/LICENSE` & `moosez-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.0.2/PKG-INFO` & `moosez-2.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.2
+Version: 2.0.3
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Platform: UNKNOWN
@@ -13,11 +13,12 @@
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Requires-Python: >=3.9
 License-File: LICENSE
 
 mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical whole-body segmentation tasks. It serves models tailored towards different modalities such as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a reliable tool for medical imaging applications.
```

### Comparing `moosez-2.0.2/README.md` & `moosez-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.0.2/moosez/constants.py` & `moosez-2.0.3/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.2/moosez/download.py` & `moosez-2.0.3/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.2/moosez/file_utilities.py` & `moosez-2.0.3/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.2/moosez/image_conversion.py` & `moosez-2.0.3/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.2/moosez/image_processing.py` & `moosez-2.0.3/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.2/moosez/input_validation.py` & `moosez-2.0.3/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.2/moosez/moosez.py` & `moosez-2.0.3/moosez/moosez.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,42 +78,28 @@
     logging.info(' ')
     logging.info('- Main directory: ' + parent_folder)
     logging.info('- Model name: ' + model_name)
     logging.info(' ')
     print(' ')
     print(f'{constants.ANSI_VIOLET} NOTE:{constants.ANSI_RESET}')
     print(' ')
-    display.expectations(model_name)
+    modalities = display.expectations(model_name)
 
     # ----------------------------------
     # DOWNLOADING THE MODEL
     # ----------------------------------
 
     print('')
     print(f'{constants.ANSI_VIOLET} MODEL DOWNLOAD:{constants.ANSI_RESET}')
     print('')
     model_path = constants.NNUNET_RESULTS_FOLDER
     file_utilities.create_directory(model_path)
     download.model(model_name, model_path)
 
     # ----------------------------------
-    # CHECKING FOR EXPECTED MODALITIES
-    # ----------------------------------
-
-    with open(os.devnull, "w") as devnull:
-        old_stdout = os.dup(1)
-        os.dup2(devnull.fileno(), 1)
-
-        # Call the function with suppressed output
-        modalities = display.expected_modality(model_name)
-
-        # Restore stdout
-        os.dup2(old_stdout, 1)
-
-    # ----------------------------------
     # INPUT STANDARDIZATION
     # ----------------------------------
 
     print('')
     print(f'{constants.ANSI_VIOLET} STANDARDIZING INPUT DATA TO NIFTI:{constants.ANSI_RESET}')
     print('')
     logging.info(' ')
```

### Comparing `moosez-2.0.2/moosez/predict.py` & `moosez-2.0.3/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.2/moosez/resources.py` & `moosez-2.0.3/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.2/moosez.egg-info/PKG-INFO` & `moosez-2.0.3/moosez.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.2
+Version: 2.0.3
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Platform: UNKNOWN
@@ -13,11 +13,12 @@
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Requires-Python: >=3.9
 License-File: LICENSE
 
 mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical whole-body segmentation tasks. It serves models tailored towards different modalities such as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a reliable tool for medical imaging applications.
```

### Comparing `moosez-2.0.2/setup.py` & `moosez-2.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.0.2',
+    version='2.0.3',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
+    python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
                      'reliable tool for medical imaging applications.',
     url='https://github.com/QIMP-Team/mooseZ',
     license='Apache 2.0',
     classifiers=[
```

