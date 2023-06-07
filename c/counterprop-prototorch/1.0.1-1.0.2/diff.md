# Comparing `tmp/counterprop_prototorch-1.0.1.tar.gz` & `tmp/counterprop_prototorch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "counterprop_prototorch-1.0.1.tar", last modified: Tue Jun  6 11:55:09 2023, max compression
+gzip compressed data, was "counterprop_prototorch-1.0.2.tar", last modified: Wed Jun  7 13:01:25 2023, max compression
```

## Comparing `counterprop_prototorch-1.0.1.tar` & `counterprop_prototorch-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ronny     (1000) ronny     (1000)        0 2023-06-06 11:55:09.914834 counterprop_prototorch-1.0.1/
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     1132 2023-05-15 11:52:15.000000 counterprop_prototorch-1.0.1/LICENSE
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     2400 2023-06-06 11:55:09.914834 counterprop_prototorch-1.0.1/PKG-INFO
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     1392 2023-03-06 13:45:12.000000 counterprop_prototorch-1.0.1/README.md
-drwxrwxr-x   0 ronny     (1000) ronny     (1000)        0 2023-06-06 11:55:09.914834 counterprop_prototorch-1.0.1/counterprop_prototorch.egg-info/
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     2400 2023-06-06 11:55:09.000000 counterprop_prototorch-1.0.1/counterprop_prototorch.egg-info/PKG-INFO
--rw-rw-r--   0 ronny     (1000) ronny     (1000)      635 2023-06-06 11:55:09.000000 counterprop_prototorch-1.0.1/counterprop_prototorch.egg-info/SOURCES.txt
--rw-rw-r--   0 ronny     (1000) ronny     (1000)        1 2023-06-06 11:55:09.000000 counterprop_prototorch-1.0.1/counterprop_prototorch.egg-info/dependency_links.txt
--rw-rw-r--   0 ronny     (1000) ronny     (1000)        1 2023-05-26 11:44:45.000000 counterprop_prototorch-1.0.1/counterprop_prototorch.egg-info/not-zip-safe
--rw-rw-r--   0 ronny     (1000) ronny     (1000)       57 2023-06-06 11:55:09.000000 counterprop_prototorch-1.0.1/counterprop_prototorch.egg-info/requires.txt
--rw-rw-r--   0 ronny     (1000) ronny     (1000)       19 2023-06-06 11:55:09.000000 counterprop_prototorch-1.0.1/counterprop_prototorch.egg-info/top_level.txt
-drwxrwxr-x   0 ronny     (1000) ronny     (1000)        0 2023-06-06 11:55:09.914834 counterprop_prototorch-1.0.1/counterpropagation/
--rw-rw-r--   0 ronny     (1000) ronny     (1000)      416 2023-06-06 11:39:37.000000 counterprop_prototorch-1.0.1/counterpropagation/__init__.py
-drwxrwxr-x   0 ronny     (1000) ronny     (1000)        0 2023-06-06 11:55:09.914834 counterprop_prototorch-1.0.1/counterpropagation/core/
--rw-rw-r--   0 ronny     (1000) ronny     (1000)       71 2023-05-26 11:51:07.000000 counterprop_prototorch-1.0.1/counterpropagation/core/__init__.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     9927 2023-06-06 11:01:30.000000 counterprop_prototorch-1.0.1/counterpropagation/core/cp.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     2754 2023-06-06 11:49:26.000000 counterprop_prototorch-1.0.1/counterpropagation/core/initializer.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     2198 2023-05-26 10:33:04.000000 counterprop_prototorch-1.0.1/counterpropagation/core/response_layer.py
-drwxrwxr-x   0 ronny     (1000) ronny     (1000)        0 2023-06-06 11:55:09.914834 counterprop_prototorch-1.0.1/counterpropagation/utils/
--rw-rw-r--   0 ronny     (1000) ronny     (1000)      256 2023-03-06 11:38:40.000000 counterprop_prototorch-1.0.1/counterpropagation/utils/__init__.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     1575 2023-05-15 12:55:38.000000 counterprop_prototorch-1.0.1/counterpropagation/utils/callbacks.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)      361 2023-02-06 14:44:01.000000 counterprop_prototorch-1.0.1/counterpropagation/utils/evalmeasure.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)      915 2023-06-06 11:04:22.000000 counterprop_prototorch-1.0.1/counterpropagation/utils/visualization.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)       38 2023-06-06 11:55:09.914834 counterprop_prototorch-1.0.1/setup.cfg
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     1475 2023-06-06 11:42:15.000000 counterprop_prototorch-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 13:01:25.000000 counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/counterpropagation/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/counterpropagation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/core/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/core/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/core/response_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/counterpropagation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/utils/evalmeasure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/counterpropagation/utils/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:01:25.148101 counterprop_prototorch-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-07 13:01:20.000000 counterprop_prototorch-1.0.2/setup.py
```

### Comparing `counterprop_prototorch-1.0.1/LICENSE` & `counterprop_prototorch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.1/counterprop_prototorch.egg-info/SOURCES.txt` & `counterprop_prototorch-1.0.2/counterprop_prototorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.1/counterpropagation/core/cp.py` & `counterprop_prototorch-1.0.2/counterpropagation/core/cp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from typing import Any, Callable, Optional
 
-import pytorch_lightning as pl
 import torch
 from prototorch.models.abstract import ProtoTorchBolt
-from prototorch.nn.wrappers import LambdaLayer
 from torch.nn import Linear, MSELoss
 from torch.nn.parameter import Parameter
 
-from counterpropagation.utils import accuracy, err10, r_squared
+from counterpropagation.utils import accuracy
 
 
 class CounterPropagation(ProtoTorchBolt):
 
     """
 
     Counterpropagation Model - Base Class
@@ -27,15 +25,16 @@
                             |    
                             |
         Loss(SupervisedModel)
                             |                            
                             |
                             |----> SupervisedModel(Response)
 
-    Thus, ResponseModel must be differentiable.
+    Thus, ResponseModel must be differentiable by Version 1.0.1, however future updates 
+    may include non-trainable Response Models.
 
     """
 
     def __init__( 
         self, 
         hparams,
         resmodel: Any,
@@ -54,36 +53,35 @@
             
             resmodel (Any): 
             Response Model
             
             opsmodel (Optional[Any], None): 
             Supervised (Operation) Model (Layer), can be None for regression,
             in which case an perceptron like layer is created.
-            Defaults to None.
+             Defaults to None.
             
             train_metrics (dict): 
-            Metrics being used to monitor training performance. Defaults to accuracy.
+            Metrics being used to monitor training performance in shape like:
+            train_metrics = {"name_of_metric": callable_metric} 
+             Defaults to accuracy.
             
             test_metrics (Optional[dict], None): 
-            Metrics being used to monitor test performance. Defaults to None.
+            Metrics being used to monitor test performance. 
+             Defaults to None.
             
             same_metrics (bool): 
-            If True, test_metrics will equal train_metrics. If False, an dict needs to be
-            given to test_metrics with the corresponding metrics. Defaults to True.
-
-        Raises:
-            ValueError: When resmodel is None.
+            If True, test_metrics will equal train_metrics. If False a dict needs to be
+            given to test_metrics with the corresponding metrics. 
+             Defaults to True.
 
         """
 
         super(CounterPropagation, self).__init__(hparams, **kwargs)
 
-        if resmodel is None:
-            raise ValueError("Response Model cannot be None")
-        elif opsmodel is None:
+        if opsmodel is None:
             self.res_layer = resmodel(hparams, prototypes_initializer=self.hparams.response_initializer, **kwargs)
             self.ops_layer = opsmodel
         else:
             self.res_layer = resmodel(hparams, prototypes_initializer=self.hparams.response_initializer, **kwargs)
             self.ops_layer = opsmodel(hparams, prototypes_initializer=self.hparams.operation_initializer, **kwargs)
         
         ## allow for customizable metrics
@@ -174,15 +172,15 @@
         return test_loss
 
 class CounterPropagationProtoModel(CounterPropagation):
 
     """
 
     Prototype-based Classification CP-Model, i.e. opsmodel is a
-    prototype-based Model
+    prototype-based / distance-based Model
 
     """
 
     def __init__(self, hparams, **kwargs):
         """
 
         Args:
```

### Comparing `counterprop_prototorch-1.0.1/counterpropagation/core/initializer.py` & `counterprop_prototorch-1.0.2/counterpropagation/core/initializer.py`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.1/counterpropagation/core/response_layer.py` & `counterprop_prototorch-1.0.2/counterpropagation/core/response_layer.py`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.1/counterpropagation/utils/callbacks.py` & `counterprop_prototorch-1.0.2/counterpropagation/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.1/counterpropagation/utils/visualization.py` & `counterprop_prototorch-1.0.2/counterpropagation/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `counterprop_prototorch-1.0.1/setup.py` & `counterprop_prototorch-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "scipy",
     "torch-kmeans"
 ]
 
 
 setup(
     name="counterprop_prototorch",
-    version="1.0.1",
+    version="1.0.2",
     description="Counter Propagation based on "
     "Prototorch. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ronny Schubert",
     author_email="trebuhcsynnor@gmail.com",
     url=PROJECT_URL,
```

