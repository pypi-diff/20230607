# Comparing `tmp/monotonic-nn-0.3.1rc1.tar.gz` & `tmp/monotonic-nn-0.3.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic-nn-0.3.1rc1.tar", last modified: Wed Jun  7 07:17:01 2023, max compression
+gzip compressed data, was "monotonic-nn-0.3.1rc2.tar", last modified: Wed Jun  7 07:22:22 2023, max compression
```

## Comparing `monotonic-nn-0.3.1rc1.tar` & `monotonic-nn-0.3.1rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:17:01.923074 monotonic-nn-0.3.1rc1/
--rw-rw-r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc1/LICENSE
--rw-rw-r--   0 davor     (1000) davor     (1000)      111 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc1/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    12016 2023-06-07 07:17:01.923074 monotonic-nn-0.3.1rc1/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)    10872 2023-06-07 07:15:21.000000 monotonic-nn-0.3.1rc1/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:17:01.923074 monotonic-nn-0.3.1rc1/airt/
--rw-rw-r--   0 davor     (1000) davor     (1000)      367 2023-06-07 07:16:41.000000 monotonic-nn-0.3.1rc1/airt/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:17:01.923074 monotonic-nn-0.3.1rc1/airt/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-07 07:16:41.000000 monotonic-nn-0.3.1rc1/airt/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-07 07:16:41.000000 monotonic-nn-0.3.1rc1/airt/_components/helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    31436 2023-06-07 07:16:41.000000 monotonic-nn-0.3.1rc1/airt/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     9935 2023-06-07 07:16:41.000000 monotonic-nn-0.3.1rc1/airt/_modidx.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:17:01.923074 monotonic-nn-0.3.1rc1/airt/keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-07 07:16:41.000000 monotonic-nn-0.3.1rc1/airt/keras/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14089 2023-06-07 07:16:41.000000 monotonic-nn-0.3.1rc1/airt/keras/experiments.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:17:01.923074 monotonic-nn-0.3.1rc1/airt/keras/layers/
--rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-07 07:16:41.000000 monotonic-nn-0.3.1rc1/airt/keras/layers/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:17:01.923074 monotonic-nn-0.3.1rc1/monotonic_nn.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    12016 2023-06-07 07:17:01.000000 monotonic-nn-0.3.1rc1/monotonic_nn.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-07 07:17:01.000000 monotonic-nn-0.3.1rc1/monotonic_nn.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-07 07:17:01.000000 monotonic-nn-0.3.1rc1/monotonic_nn.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-07 07:17:01.000000 monotonic-nn-0.3.1rc1/monotonic_nn.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 18:05:47.000000 monotonic-nn-0.3.1rc1/monotonic_nn.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      268 2023-06-07 07:17:01.000000 monotonic-nn-0.3.1rc1/monotonic_nn.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-07 07:17:01.000000 monotonic-nn-0.3.1rc1/monotonic_nn.egg-info/top_level.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)      919 2023-06-07 07:16:33.000000 monotonic-nn-0.3.1rc1/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-07 07:17:01.923074 monotonic-nn-0.3.1rc1/setup.cfg
--rw-rw-r--   0 davor     (1000) davor     (1000)     3157 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc1/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.625995 monotonic-nn-0.3.1rc2/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    20848 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc2/LICENSE
+-rw-rw-r--   0 davor     (1000) davor     (1000)      111 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc2/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    12019 2023-06-07 07:22:22.625995 monotonic-nn-0.3.1rc2/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10875 2023-06-07 07:21:40.000000 monotonic-nn-0.3.1rc2/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.621995 monotonic-nn-0.3.1rc2/airt/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      367 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.621995 monotonic-nn-0.3.1rc2/airt/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      320 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/_components/helpers.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    31436 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/_components/mono_dense_layer.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9935 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/_modidx.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.621995 monotonic-nn-0.3.1rc2/airt/keras/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/keras/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    14089 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/keras/experiments.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.621995 monotonic-nn-0.3.1rc2/airt/keras/layers/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      344 2023-06-07 07:21:55.000000 monotonic-nn-0.3.1rc2/airt/keras/layers/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-07 07:22:22.625995 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    12019 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)      510 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/SOURCES.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/dependency_links.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)       30 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/entry_points.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-06-05 18:05:47.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/not-zip-safe
+-rw-rw-r--   0 davor     (1000) davor     (1000)      268 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/requires.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        5 2023-06-07 07:22:22.000000 monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/top_level.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)      919 2023-06-07 07:21:45.000000 monotonic-nn-0.3.1rc2/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-07 07:22:22.625995 monotonic-nn-0.3.1rc2/setup.cfg
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3157 2023-06-05 13:19:26.000000 monotonic-nn-0.3.1rc2/setup.py
```

### Comparing `monotonic-nn-0.3.1rc1/LICENSE` & `monotonic-nn-0.3.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.1rc1/PKG-INFO` & `monotonic-nn-0.3.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.3.1rc1
+Version: 0.3.1rc2
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
@@ -274,23 +274,27 @@
 
 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This
 work is licensed under a
 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative
 Commons Attribution-NonCommercial-ShareAlike 4.0 International
 License</a>.
 
-You are free to: - Share — copy and redistribute the material in any
+You are free to:
+
+- Share — copy and redistribute the material in any
 medium or format
 
 - Adapt — remix, transform, and build upon the material
 
 The licensor cannot revoke these freedoms as long as you follow the
 license terms.
 
-Under the following terms: - Attribution — You must give appropriate
+Under the following terms: 
+
+- Attribution — You must give appropriate
 credit, provide a link to the license, and indicate if changes were
 made. You may do so in any reasonable manner, but not in any way that
 suggests the licensor endorses you or your use.
 
 - NonCommercial — You may not use the material for commercial purposes.
 
 - ShareAlike — If you remix, transform, or build upon the material, you
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.1rc1 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.1rc2 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
 colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
 Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
```

### Comparing `monotonic-nn-0.3.1rc1/README.md` & `monotonic-nn-0.3.1rc2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,23 +247,27 @@
 
 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This
 work is licensed under a
 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative
 Commons Attribution-NonCommercial-ShareAlike 4.0 International
 License</a>.
 
-You are free to: - Share — copy and redistribute the material in any
+You are free to:
+
+- Share — copy and redistribute the material in any
 medium or format
 
 - Adapt — remix, transform, and build upon the material
 
 The licensor cannot revoke these freedoms as long as you follow the
 license terms.
 
-Under the following terms: - Attribution — You must give appropriate
+Under the following terms: 
+
+- Attribution — You must give appropriate
 credit, provide a link to the license, and indicate if changes were
 made. You may do so in any reasonable manner, but not in any way that
 suggests the licensor endorses you or your use.
 
 - NonCommercial — You may not use the material for commercial purposes.
 
 - ShareAlike — If you remix, transform, or build upon the material, you
```

### Comparing `monotonic-nn-0.3.1rc1/airt/_components/mono_dense_layer.py` & `monotonic-nn-0.3.1rc2/airt/_components/mono_dense_layer.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.1rc1/airt/_modidx.py` & `monotonic-nn-0.3.1rc2/airt/_modidx.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.1rc1/airt/keras/experiments.py` & `monotonic-nn-0.3.1rc2/airt/keras/experiments.py`

 * *Files identical despite different names*

### Comparing `monotonic-nn-0.3.1rc1/monotonic_nn.egg-info/PKG-INFO` & `monotonic-nn-0.3.1rc2/monotonic_nn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-nn
-Version: 0.3.1rc1
+Version: 0.3.1rc2
 Summary: Monotonic Neural Networks
 Home-page: https://github.com/airtai/monotonic-nn
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions
@@ -274,23 +274,27 @@
 
 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This
 work is licensed under a
 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative
 Commons Attribution-NonCommercial-ShareAlike 4.0 International
 License</a>.
 
-You are free to: - Share — copy and redistribute the material in any
+You are free to:
+
+- Share — copy and redistribute the material in any
 medium or format
 
 - Adapt — remix, transform, and build upon the material
 
 The licensor cannot revoke these freedoms as long as you follow the
 license terms.
 
-Under the following terms: - Attribution — You must give appropriate
+Under the following terms: 
+
+- Attribution — You must give appropriate
 credit, provide a link to the license, and indicate if changes were
 made. You may do so in any reasonable manner, but not in any way that
 suggests the licensor endorses you or your use.
 
 - NonCommercial — You may not use the material for commercial purposes.
 
 - ShareAlike — If you remix, transform, or build upon the material, you
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.1rc1 Summary: Monotonic
+Metadata-Version: 2.1 Name: monotonic-nn Version: 0.3.1rc2 Summary: Monotonic
 Neural Networks Home-page: https://github.com/airtai/monotonic-nn Author: AIRT
 Technologies d.o.o. Author-email: info@airt.ai License: Creative Commons
 License Project-URL: Bug Tracker, https://github.com/airtai/monotonic-nn/issues
 Project-URL: CI, https://github.com/airtai/monotonic-nn/actions Project-URL:
 Documentation, https://monotonic.airt.ai/ Project-URL: Tutorial, https://
 colab.research.google.com/github/airtai/monotonic-nn/blob/main/nbs/index.ipynb
 Keywords: tensorflow keras monotone "monotonic neural networks" "dense layer"
```

### Comparing `monotonic-nn-0.3.1rc1/settings.ini` & `monotonic-nn-0.3.1rc2/settings.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = monotonic-nn
 lib_name = %(repo)s
-version = 0.3.1rc1
+version = 0.3.1rc2
 min_python = 3.8
 license = cc
 
 ### nbdev ###
 doc_path = _docs
 lib_path = airt
 nbs_path = nbs
```

### Comparing `monotonic-nn-0.3.1rc1/setup.py` & `monotonic-nn-0.3.1rc2/setup.py`

 * *Files identical despite different names*

