# Comparing `tmp/ezkl-0.0.2.tar.gz` & `tmp/ezkl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "ezkl-0.0.3.tar", max compression
```

## Comparing `ezkl-0.0.2.tar` & `ezkl-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,6 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ezkl-0.0.2/leakyrelu.py~
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 ezkl-0.0.2/examples/export/leakyrelu.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 ezkl-0.0.2/examples/mlp/mlp_relu.py
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 ezkl-0.0.2/examples/tutorial/README.md
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 ezkl-0.0.2/examples/tutorial/tutorial.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ezkl-0.0.2/ezkl/__init__.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 ezkl-0.0.2/ezkl/export.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 ezkl-0.0.2/ezkl/export.py~
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 ezkl-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ezkl-0.0.2/LICENSE
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ezkl-0.0.2/README.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ezkl-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 ezkl-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-07 12:54:22.645108 ezkl-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2307 2023-06-07 12:54:22.645108 ezkl-0.0.3/README.md
+-rw-r--r--   0        0        0      272 2023-06-07 12:54:22.645108 ezkl-0.0.3/ezkl/__init__.py
+-rw-r--r--   0        0        0     3232 2023-06-07 12:54:22.645108 ezkl-0.0.3/ezkl/export.py
+-rw-r--r--   0        0        0      879 2023-06-07 12:54:22.645108 ezkl-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 ezkl-0.0.3/PKG-INFO
```

### Comparing `ezkl-0.0.2/examples/mlp/mlp_relu.py` & `ezkl-0.0.3/ezkl/export.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,72 @@
 import io
 import numpy as np
-from torch import nn
 import torch.onnx
-import torch.nn as nn
-import torch.nn.init as init
+import torch
 import json
+import ezkl_lib
+
+def export(torch_model, input_shape=None, input_array=None, onnx_filename="network.onnx", input_filename="input.json"):
+    """Export a PyTorch model.
+    Arguments:
+    torch_model: a PyTorch model class, such as Network(torch.nn.Module)
+    Optional Keyword Arguments:
+    - input_shape: e.g. [3,2,3], a random input with these dimensions will be generated.
+    - input_array: the given input will be used for the model
+    Note: Exactly one of input_shape and input_array should be specified.
+    - onnx_filename: Default "network.onnx", the name of the onnx file to be generated
+    - input_filename: Defualt "input.json", the name of the json input file to be generated for ezkl
+
+    """
+    if input_array is None:
+        x = 0.1*torch.rand(1,*input_shape, requires_grad=True)
+    else:
+        x = torch.tensor(input_array)
+        if input_shape is not None:
+            assert tuple(input_shape) == x.shape
+        new_shape = tuple([1]+list(x.shape))
+        x = torch.reshape(x,new_shape)
+
 
-class Model(nn.Module):
-    def __init__(self, inplace=False):
-        super(Model, self).__init__()
-
-        self.aff1 = nn.Linear(3,4)
-        self.relu1 = nn.ReLU()
-        self.aff2 = nn.Linear(4,4)
-        self.relu2 = nn.ReLU()
-        self.aff3 = nn.Linear(4,2)
-        self.relu3 = nn.ReLU()
-        self._initialize_weights()
-
-    def forward(self, x):
-        x =  self.aff1(x)
-        x =  self.relu1(x)
-        x =  self.aff2(x)
-        x =  self.relu2(x)
-        x =  self.aff3(x)
-        x =  self.relu3(x)
-        return (x)
-
-
-    def _initialize_weights(self):
-        init.orthogonal_(self.aff1.weight)
-        init.orthogonal_(self.aff2.weight)
-        init.orthogonal_(self.aff3.weight)
-
-def main():
-    torch_model = Model()
-    # Input to the model
-    shape = [3]
-    x = 0.1*torch.rand(1,*shape, requires_grad=True)
     torch_out = torch_model(x)
+
     # Export the model
     torch.onnx.export(torch_model,               # model being run
-                      (x,),                   # model input (or a tuple for multiple inputs)
-                      "mlp.onnx",            # where to save the model (can be a file or file-like object)
+                      x,                   # model input (or a tuple for multiple inputs)
+                      onnx_filename,            # where to save the model (can be a file or file-like object)
                       export_params=True,        # store the trained parameter weights inside the model file
                       opset_version=10,          # the ONNX version to export the model to
                       do_constant_folding=True,  # whether to execute constant folding for optimization
                       input_names = ['input'],   # the model's input names
                       output_names = ['output'], # the model's output names
                       dynamic_axes={'input' : {0 : 'batch_size'},    # variable length axes
                                     'output' : {0 : 'batch_size'}})
 
-    d = ((x).detach().numpy()).reshape([-1]).tolist()
+    data_array = ((x).detach().numpy()).reshape([-1]).tolist()
 
-    data = dict(input_shapes = [shape],
-                input_data = [d],
-                public_inputs = [((o).detach().numpy()).reshape([-1]).tolist() for o in torch_out])
+    data = dict(input_shapes = [input_shape],
+                input_data = [data_array],
+                output_data = [((o).detach().numpy()).reshape([-1]).tolist() for o in torch_out])
 
     # Serialize data into file:
-    json.dump( data, open( "input.json", 'w' ) )
+    json.dump( data, open( input_filename, 'w' ) )
+
+    # Runs a forward operation to quantize inputs
+    ezkl_lib.forward(input_filename, onnx_filename, input_filename)
 
 if __name__ == "__main__":
-    main()
+    from torch import nn
+
+    class MyModel(nn.Module):
+        def __init__(self):
+            super(MyModel, self).__init__()
+            self.flatten = nn.Flatten()
+
+        def forward(self, x):
+            return self.flatten(x)
+
+    circuit = MyModel()
+
+    export(circuit, input_shape = [9,2], input_array= [[0.06980138272047043, 0.09594511240720749], [0.09435884654521942, 0.08530371636152267], [0.059045590460300446, 0.06503964960575104], [0.005533689167350531, 0.08425236493349075], [0.08761995285749435, 0.012599778361618519], [0.014501023106276989, 0.0011647045612335205], [0.007388335652649403, 0.09860159456729889], [0.0525859072804451, 0.0077858567237854], [0.09905613213777542, 0.04969405755400658]])
+
 
 
-
```

### Comparing `ezkl-0.0.2/LICENSE` & `ezkl-0.0.3/LICENSE`

 * *Files identical despite different names*

