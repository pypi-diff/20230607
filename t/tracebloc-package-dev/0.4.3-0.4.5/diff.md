# Comparing `tmp/tracebloc_package-dev-0.4.3.tar.gz` & `tmp/tracebloc_package-dev-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.4.3.tar", last modified: Thu Jun  1 11:57:12 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.4.5.tar", last modified: Wed Jun  7 07:45:33 2023, max compression
```

## Comparing `tracebloc_package-dev-0.4.3.tar` & `tracebloc_package-dev-0.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 11:57:12.089361 tracebloc_package-dev-0.4.3/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.3/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-01 11:57:12.089499 tracebloc_package-dev-0.4.3/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.3/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-01 11:57:12.089872 tracebloc_package-dev-0.4.3/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-01 11:56:26.000000 tracebloc_package-dev-0.4.3/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 11:57:12.087909 tracebloc_package-dev-0.4.3/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-03-15 10:59:39.000000 tracebloc_package-dev-0.4.3/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-05-18 09:32:19.000000 tracebloc_package-dev-0.4.3/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    20998 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.3/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    60056 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.3/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.4.3/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)     9821 2023-06-01 11:56:14.000000 tracebloc_package-dev-0.4.3/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10203 2023-06-01 06:15:22.000000 tracebloc_package-dev-0.4.3/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     5840 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.3/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3203 2022-06-09 05:22:24.000000 tracebloc_package-dev-0.4.3/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-01 11:57:12.089143 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-01 11:57:12.000000 tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-07 07:45:33.619424 tracebloc_package-dev-0.4.5/
+-rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.5/LICENSE.txt
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-07 07:45:33.619510 tracebloc_package-dev-0.4.5/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.5/README.md
+-rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-07 07:45:33.619821 tracebloc_package-dev-0.4.5/setup.cfg
+-rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-07 07:43:59.000000 tracebloc_package-dev-0.4.5/setup.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-07 07:45:33.618034 tracebloc_package-dev-0.4.5/tracebloc_package/
+-rw-r--r--   0 hasan      (501) staff       (20)       67 2023-03-15 10:59:39.000000 tracebloc_package-dev-0.4.5/tracebloc_package/__init__.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-05-18 09:32:19.000000 tracebloc_package-dev-0.4.5/tracebloc_package/check_parameters.py
+-rw-r--r--   0 hasan      (501) staff       (20)    20998 2023-06-07 07:44:09.000000 tracebloc_package-dev-0.4.5/tracebloc_package/functional_test.py
+-rw-r--r--   0 hasan      (501) staff       (20)    60286 2023-06-07 07:44:09.000000 tracebloc_package-dev-0.4.5/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.4.5/tracebloc_package/messages.py
+-rw-r--r--   0 hasan      (501) staff       (20)     9821 2023-06-07 07:44:08.000000 tracebloc_package-dev-0.4.5/tracebloc_package/upload.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10203 2023-06-07 07:44:08.000000 tracebloc_package-dev-0.4.5/tracebloc_package/user.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5840 2023-06-01 09:06:49.000000 tracebloc_package-dev-0.4.5/tracebloc_package/utils.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3203 2022-06-09 05:22:24.000000 tracebloc_package-dev-0.4.5/tracebloc_package/weights.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-07 07:45:33.619221 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-07 07:45:33.000000 tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.4.3/LICENSE.txt` & `tracebloc_package-dev-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.3/PKG-INFO` & `tracebloc_package-dev-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.4.3
+Version: 0.4.5
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.4.3/setup.py` & `tracebloc_package-dev-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.4.3",
+    version="0.4.5",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.4.3/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.4.5/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.3/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.4.5/tracebloc_package/functional_test.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.3/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.4.5/tracebloc_package/linkModelDataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,17 @@
                 data=data,
             )
             body_unicode = re.content.decode("utf-8")
             content = json.loads(body_unicode)
             if re.status_code == 200:
                 self.__total_images = content["total_images_per_edge"]
                 self.__validation_split = self.__default_validation_split()
+                self.__images_per_class = json.dumps(
+                    training_dataset
+                )  # assign images count for sub-dataset
             # else:
             #     self.__print_error(content['message'])
 
     def __update_image_model(self):
         """
         change image type and size data as user choice in model file provided by user
         """
@@ -656,43 +659,46 @@
                 except:
                     error_msg = f"Please provide tensorflow supported default loss functions losses: {l}\n"
                     self.__print_error(error_msg)
             else:
                 error_msg = "Custom loss function"
                 self.__not_supported_parameters(error_msg)
 
-    def __getlayers(self):
+    def __check_layers(self, layersFreeze):
         """
         load model and get all layers avaiable in model
         """
-        isvalidlayers, model_layers = layer_instance_check(self.__model)
-        return model_layers
+        try:
+            for layer_to_freeze in layersFreeze:
+                layer = self.__model.get_layer(layer_to_freeze)
+        except Exception as e:
+            return False, e
+        return True, ""
 
     def layersFreeze(self, layersFreeze: list):
         """
         Provide name of layers in a list to be frozen before training a model.
         Get layers name in a model provided with the summary shown above.
         example: trainingObject.layersFreeze(['layer_name','layer_name', ...])
         default: None
         """
         if self.__framework == TENSORFLOW_FRAMEWORK:
-            all_layers = self.__getlayers()
             if type(layersFreeze) == list and all(
                 isinstance(sub, str) for sub in layersFreeze
             ):
                 layers_eligible = True
-                for layer in layersFreeze:
-                    if layer not in all_layers:
-                        layers_eligible = False
+                status, _error = self.__check_layers(layersFreeze)
+                if not status:
+                    layers_eligible = False
                 if layers_eligible:
                     layersFreeze = str(layersFreeze)
                     self.__layers_non_trainable = layersFreeze
                     self.__remove_error_method()
                 else:
-                    error_msg = f"Provide layers only which model contains for layersFreeze : {all_layers}\n"
+                    error_msg = f"Provide layers only which model contains for layersFreeze : \n{_error}\n"
                     self.__print_error(error_msg)
             else:
                 error_msg = "Provide values as list of strings for layersFreeze\n"
                 self.__print_error(error_msg)
         else:
             self.__not_supported_parameters("layersFreeze")
```

### Comparing `tracebloc_package-dev-0.4.3/tracebloc_package/messages.py` & `tracebloc_package-dev-0.4.5/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.3/tracebloc_package/upload.py` & `tracebloc_package-dev-0.4.5/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.3/tracebloc_package/user.py` & `tracebloc_package-dev-0.4.5/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.3/tracebloc_package/utils.py` & `tracebloc_package-dev-0.4.5/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.3/tracebloc_package/weights.py` & `tracebloc_package-dev-0.4.5/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.4.3
+Version: 0.4.5
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.4.3/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.4.5/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

