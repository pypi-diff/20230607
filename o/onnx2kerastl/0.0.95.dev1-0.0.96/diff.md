# Comparing `tmp/onnx2kerastl-0.0.95.dev1.tar.gz` & `tmp/onnx2kerastl-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.95.dev1.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.96.tar", max compression
```

## Comparing `onnx2kerastl-0.0.95.dev1.tar` & `onnx2kerastl-0.0.96.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1067 2023-05-17 10:05:24.840017 onnx2kerastl-0.0.95.dev1/LICENSE
--rw-r--r--   0        0        0       66 2023-05-17 10:05:24.840536 onnx2kerastl-0.0.95.dev1/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-05-17 10:05:24.840790 onnx2kerastl-0.0.95.dev1/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2023-05-17 10:05:24.840968 onnx2kerastl-0.0.95.dev1/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2023-05-17 10:05:24.841141 onnx2kerastl-0.0.95.dev1/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    14493 2023-05-30 11:55:43.175666 onnx2kerastl-0.0.95.dev1/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11968 2023-05-17 10:05:24.841507 onnx2kerastl-0.0.95.dev1/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      584 2023-05-23 13:09:48.518074 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2023-05-17 10:05:24.841906 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2023-05-17 10:05:24.842046 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2023-05-17 10:05:24.842190 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1730 2023-05-17 10:05:24.842337 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2023-05-17 10:05:24.842473 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2023-05-17 10:05:24.842602 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9380 2023-05-30 11:55:17.256120 onnx2kerastl-0.0.95.dev1/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2023-05-17 10:05:24.842900 onnx2kerastl-0.0.95.dev1/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3947 2023-05-30 11:43:46.982250 onnx2kerastl-0.0.95.dev1/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-05-30 11:55:17.207286 onnx2kerastl-0.0.95.dev1/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3791 2023-05-17 10:05:24.843376 onnx2kerastl-0.0.95.dev1/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2023-05-17 10:05:24.843508 onnx2kerastl-0.0.95.dev1/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5551 2023-05-17 10:05:24.843673 onnx2kerastl-0.0.95.dev1/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    16027 2023-05-30 11:41:40.091917 onnx2kerastl-0.0.95.dev1/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-05-17 10:05:24.844012 onnx2kerastl-0.0.95.dev1/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-05-17 10:05:24.844205 onnx2kerastl-0.0.95.dev1/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    17737 2023-05-30 11:55:17.264481 onnx2kerastl-0.0.95.dev1/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     5011 2023-05-30 11:38:10.695884 onnx2kerastl-0.0.95.dev1/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-05-17 10:05:24.844792 onnx2kerastl-0.0.95.dev1/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     5629 2023-05-30 11:55:17.248648 onnx2kerastl-0.0.95.dev1/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1035 2023-05-30 12:05:54.899568 onnx2kerastl-0.0.95.dev1/pyproject.toml
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.95.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-17 10:05:24.840017 onnx2kerastl-0.0.96/LICENSE
+-rw-r--r--   0        0        0       66 2023-05-17 10:05:24.840536 onnx2kerastl-0.0.96/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-05-17 10:05:24.840790 onnx2kerastl-0.0.96/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2023-05-17 10:05:24.840968 onnx2kerastl-0.0.96/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2023-06-07 15:57:44.568650 onnx2kerastl-0.0.96/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    14415 2023-06-07 16:25:57.562217 onnx2kerastl-0.0.96/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11968 2023-05-17 10:05:24.841507 onnx2kerastl-0.0.96/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-05-23 13:09:48.518074 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-17 10:05:24.841906 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2023-05-17 10:05:24.842046 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2023-05-17 10:05:24.842190 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1730 2023-05-17 10:05:24.842337 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2023-05-17 10:05:24.842473 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2023-05-17 10:05:24.842602 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9380 2023-06-07 16:25:57.562862 onnx2kerastl-0.0.96/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2023-05-17 10:05:24.842900 onnx2kerastl-0.0.96/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3947 2023-05-30 11:43:46.982250 onnx2kerastl-0.0.96/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-05-30 11:55:17.207286 onnx2kerastl-0.0.96/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3791 2023-05-17 10:05:24.843376 onnx2kerastl-0.0.96/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2023-05-17 10:05:24.843508 onnx2kerastl-0.0.96/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-17 10:05:24.843673 onnx2kerastl-0.0.96/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    16027 2023-06-07 15:57:44.569123 onnx2kerastl-0.0.96/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-05-17 10:05:24.844012 onnx2kerastl-0.0.96/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-05-17 10:05:24.844205 onnx2kerastl-0.0.96/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    17750 2023-06-07 16:25:57.564211 onnx2kerastl-0.0.96/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5006 2023-06-07 10:11:23.748652 onnx2kerastl-0.0.96/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-05-17 10:05:24.844792 onnx2kerastl-0.0.96/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     5822 2023-06-07 16:25:57.564995 onnx2kerastl-0.0.96/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1030 2023-06-07 16:25:57.566693 onnx2kerastl-0.0.96/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.96/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.95.dev1/LICENSE` & `onnx2kerastl-0.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.96/onnx2kerastl/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,16 +109,14 @@
         for onnx_i in onnx_inputs:
             if onnx_i.name == input_name:
                 dtype = None if input_types is None else input_types[i]
                 input_shape = [i.dim_value for i in onnx_i.type.tensor_type.shape.dim]
                 input_shape = [shape if shape != 0 else None for shape in input_shape]
                 batch_size = input_shape[0]
                 input_shape = input_shape[1:]
-                if len(input_shape) == 0:
-                    input_shape = 1
                 if batch_size is None:
                     layers[input_name] = keras.layers.InputLayer(
                         input_shape=input_shape, name=input_name, dtype=dtype).output
                 else:
                     layers[input_name] = keras.layers.InputLayer(
                         input_shape=input_shape, name=input_name, dtype=dtype, batch_size=batch_size).output
                 keras_inputs.append(layers[input_name])
```

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/ltsm_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/reshape_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import keras
 import numpy as np
 import tensorflow as tf
 from keras import backend as K
 from keras.layers import SlicingOpLambda
 
-from .utils import is_numpy, ensure_tf_type, ensure_numpy_type, match_tensors_rank
+from .utils import is_numpy, ensure_tf_type, ensure_numpy_type, unsqueeze_tensors_of_rank_one
 
 
 def convert_transpose(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert transpose.
     :param node: current operation node
     :param params: operation attributes
@@ -145,15 +145,15 @@
                 try:
                     layers[node_name] = tf.concat(layer_input, axis=params['axis'], name=keras_name)
                 except Exception as ex:
                     # might be due to type mismatch between different inputs of tf.concat
                     raise
 
             else:
-                layer_input = match_tensors_rank(layer_input)
+                layer_input = unsqueeze_tensors_of_rank_one(layer_input, axis=params['axis'])
                 layers[node_name] = keras.layers.concatenate(inputs=layer_input,
                                                              axis=params['axis'],
                                                              name=keras_name)
         else:
             layers[node_name] = layer_input[0]
 
 
@@ -415,15 +415,15 @@
     :param keras_name: resulting layer name
     :return: None
     """
     if len(node.input) != 2:
         assert AttributeError('More than 2 input for expand layer.')
 
     input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
-    input_1 = ensure_numpy_type(layers[node.input[1]]).astype(np.int32)
+    input_1 = layers[node.input[1]]
     if input_0.dtype.is_bool:
         input_0 = tf.cast(input_0, dtype='int32')
-    layers[node_name] = input_0 * tf.ones(input_1, dtype=input_0.dtype)
+    layers[node_name] = input_0 * tf.ones(shape=input_1, dtype=input_0.dtype)
 
 
 def convert_tile(node, params, layers, lambda_func, node_name, keras_name):
     layers[node_name] = tf.tile(layers[node.input[0]], layers[node.input[1]])
```

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/sampling_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     alphas = []
     floors = []
     ceils = []
     index_order = [0, 1] if indexing == "ij" else [1, 0]
     # unstacked_query_points = tf.unstack(query_points, axis=2, num=2)
 
     for i, dim in enumerate(index_order):
-        queries = query_points[:, :, dim, ...]
+        queries = query_points[:, :, dim]
         # queries = unstacked_query_points[dim]
 
         size_in_indexing_dimension = grid_shape[i + 1]
 
         # max_floor is size_in_indexing_dimension - 2 so that max_floor + 1
         # is still a valid index into the grid.
         max_floor = tf.cast(size_in_indexing_dimension - 2, query_type)
```

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.96/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95.dev1/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.96/onnx2kerastl/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,16 @@
     """
     Raise exception if it's not a numpy
     :param obj: object to check
     :return: numpy object
     """
     if is_numpy(obj):
         return obj
-    elif isinstance(obj, tf.Tensor):
-        return obj.numpy()
     else:
-        raise AttributeError('Not a numpy or tf.Tensor type.')
+        raise AttributeError('Not a numpy type.')
 
 
 def ensure_tf_type(obj, name="Const"):
     import numpy as np
     import tensorflow as tf
     """
     Convert to Keras Constant if needed
@@ -132,37 +130,40 @@
         np.testing.assert_allclose(p, k, atol=epsilon, rtol=0.0)
         if error > max_error:
             max_error = error
 
     return max_error
 
 
-def match_tensors_rank(tensor_list):
+def unsqueeze_tensors_of_rank_one(tensor_list, axis: int):
     """
-    Adjusts the ranks of tensors in a given list to match the maximum rank by adding dummy dimensions
+    Adjusts the ranks of tensors of rank 1 in a given list to match the maximum rank by adding dummy dimensions
     e.g., for input tensors shapes [(2,), (1, 4)] the unsqueezed tensors are [(1, 2), (1, 4)]
 
     Args:
         tensor_list (list): A list of tensors.
 
     Returns:
         list: A new list of tensors with adjusted ranks to match the maximum rank.
               If all tensors in the input list already have the same rank, the original list is returned.
     """
     ranks = [tensor.shape.rank for tensor in tensor_list]
     max_rank = max(ranks)
 
     if len(set(ranks)) == 1:
         return tensor_list
+    elif len(set(ranks)) > 2:
+        raise ValueError(f"More than 2 different ranks detected, broadcasting is ambiguous.\n"
+                         f"Check the outputs of layers: \n" + '\n'.join([tensor.name for tensor in tensor_list]))
 
     unsqueezed_tensors = []
     for tensor in tensor_list:
         tensor_rank = tensor.shape.rank
-        if tensor_rank < max_rank:
-            diff_rank = max_rank - tensor_rank
-            diff_shape = [1] * diff_rank + list(tensor.shape)
-            unsqueezed_tensor = tf.broadcast_to(tensor, diff_shape)
+        if tensor_rank == 1:
+            rank_diff = max_rank - 1
+            new_shape = [1] * axis + list(tensor.shape) + [1] * (rank_diff - axis)
+            unsqueezed_tensor = tf.reshape(tensor, new_shape)
             unsqueezed_tensors.append(unsqueezed_tensor)
         else:
             unsqueezed_tensors.append(tensor)
 
     return unsqueezed_tensors
```

### Comparing `onnx2kerastl-0.0.95.dev1/pyproject.toml` & `onnx2kerastl-0.0.96/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.95.dev1"
+version = "0.0.96"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.95.dev1/PKG-INFO` & `onnx2kerastl-0.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.95.dev1
+Version: 0.0.96
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

