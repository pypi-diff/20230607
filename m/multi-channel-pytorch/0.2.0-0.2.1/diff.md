# Comparing `tmp/multi_channel_pytorch-0.2.0.tar.gz` & `tmp/multi_channel_pytorch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_channel_pytorch-0.2.0.tar", max compression
+gzip compressed data, was "multi_channel_pytorch-0.2.1.tar", max compression
```

## Comparing `multi_channel_pytorch-0.2.0.tar` & `multi_channel_pytorch-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35821 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.2.0/multi_channel_pytorch/__init__.py
--rw-r--r--   0        0        0     7807 2023-06-07 10:47:31.805147 multi_channel_pytorch-0.2.0/multi_channel_pytorch/injection.py
--rw-r--r--   0        0        0      807 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.2.0/multi_channel_pytorch/multify.py
--rw-r--r--   0        0        0       89 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.2.0/multi_channel_pytorch/utils.py
--rw-r--r--   0        0        0      527 2023-06-07 10:49:10.100826 multi_channel_pytorch-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2090 2023-06-07 10:36:27.173678 multi_channel_pytorch-0.2.0/README.md
--rw-r--r--   0        0        0     2716 1970-01-01 00:00:00.000000 multi_channel_pytorch-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35821 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.2.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.2.1/multi_channel_pytorch/__init__.py
+-rw-r--r--   0        0        0     7867 2023-06-07 13:23:58.356080 multi_channel_pytorch-0.2.1/multi_channel_pytorch/injection.py
+-rw-r--r--   0        0        0      988 2023-06-07 11:14:47.818135 multi_channel_pytorch-0.2.1/multi_channel_pytorch/multify.py
+-rw-r--r--   0        0        0       89 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.2.1/multi_channel_pytorch/utils.py
+-rw-r--r--   0        0        0      527 2023-06-07 13:24:55.287295 multi_channel_pytorch-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2086 2023-06-07 13:24:22.731944 multi_channel_pytorch-0.2.1/README.md
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 multi_channel_pytorch-0.2.1/PKG-INFO
```

### Comparing `multi_channel_pytorch-0.2.0/LICENSE` & `multi_channel_pytorch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multi_channel_pytorch-0.2.0/multi_channel_pytorch/injection.py` & `multi_channel_pytorch-0.2.1/multi_channel_pytorch/injection.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             padding_mode=model.features[0].padding_mode
         )
 
     with torch.no_grad():
         # https://stackoverflow.com/questions/49433936/how-do-i-initialize-weights-in-pytorch
         # Initialize weight randomly with Gaussian
         # nn.init.normal_(model.conv1.weight[:, 3], 0, 0.001)
-        model.features[0].weight[:, 3].data.normal_(0, 0.001)
+        model.features[0].weight[:, num_channels - 1].data.normal_(0, 0.001)
 
         # Copy weights for rgb channels from pretrained model
         model.features[0].weight[:, :3] = weight
 
         if biased is not None:
             # Set bias from previous state dict
             model.features[0].load_state_dict(state_dict, strict=False)
@@ -85,15 +85,15 @@
             padding_mode=model.features[0][0].padding_mode
         )
 
     with torch.no_grad():
         # https://stackoverflow.com/questions/49433936/how-do-i-initialize-weights-in-pytorch
         # Initialize weight randomly with Gaussian
         # nn.init.normal_(model.conv1.weight[:, 3], 0, 0.001)
-        model.features[0][0].weight[:, 3].data.normal_(0, 0.001)
+        model.features[0][0].weight[:, num_channels - 1].data.normal_(0, 0.001)
 
         # Copy weights for rgb channels from pretrained model
         model.features[0][0].weight[:, :3] = weight
 
         if biased is not None:
             # Set bias from previous state dict
             model.features[0][0].load_state_dict(state_dict, strict=False)
@@ -134,15 +134,15 @@
             padding_mode=model.conv1.padding_mode
         )
 
     with torch.no_grad():
         # https://stackoverflow.com/questions/49433936/how-do-i-initialize-weights-in-pytorch
         # Initialize weight randomly with Gaussian
         # nn.init.normal_(model.conv1.weight[:, 3], 0, 0.001)
-        model.conv1.weight[:, 3].data.normal_(0, 0.001)
+        model.conv1.weight[:, num_channels - 1].data.normal_(0, 0.001)
 
         # Copy weights for rgb channels from pretrained model
         model.conv1.weight[:, :3] = weight
 
         if biased is not None:
             # Set bias from previous state dict
             model.conv1.load_state_dict(state_dict, strict=False)
@@ -182,15 +182,15 @@
             groups=model.conv_proj.groups,
             padding_mode=model.conv_proj.padding_mode
         )
 
     with torch.no_grad():
         # https://stackoverflow.com/questions/49433936/how-do-i-initialize-weights-in-pytorch
         # Initialize weight randomly with Gaussian
-        model.conv_proj.weight[:, 3].data.normal_(0, 0.001)
+        model.conv_proj.weight[:, num_channels - 1].data.normal_(0, 0.001)
 
         # Copy weights for rgb channels from pretrained model
         model.conv_proj.weight[:, :3] = weight
 
         if biased is not None:
             # Set bias from previous state dict
             model.conv_proj.load_state_dict(state_dict, strict=False)
```

### Comparing `multi_channel_pytorch-0.2.0/multi_channel_pytorch/multify.py` & `multi_channel_pytorch-0.2.1/multi_channel_pytorch/multify.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from torch.nn import Module
 
 from multi_channel_pytorch.injection import *
 
 
 def multify(model: Module, num_channels: int = 3):
+    if num_channels < 3:
+        raise ValueError("3 is the minimum number of channels to support RBG images.")
+
+    # TODO: add copy_weights flag to either copy weights or not
     architecture: str = model.__class__.__name__.lower()
 
     if architecture == 'densenet' or architecture == 'alexnet':
         model = features_0(model=model, num_channels=num_channels)
     elif architecture == 'convnext' or architecture == 'swintransformer' or architecture == 'efficientnet':
         model = features_0_0(model=model, num_channels=num_channels)
     elif architecture == 'resnet':
```

### Comparing `multi_channel_pytorch-0.2.0/pyproject.toml` & `multi_channel_pytorch-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multi-channel-pytorch"
-version = "0.2.0"
+version = "0.2.1"
 description = "Library for adding multi channel functionality to PyTorch models."
 license = "GPL-3.0-only"
 authors = ["Timo Michel <timo.michel1996@outlook.de>"]
 readme = "README.md"
 repository = "https://github.com/Timom1996/multi-channel-pytorch"
 packages = [{include = "multi_channel_pytorch"}]
```

### Comparing `multi_channel_pytorch-0.2.0/README.md` & `multi_channel_pytorch-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Multi-Channel-Pytorch
 > torch, torchvision, multi-channel-input
 
 This library allows to modify known network architectures (e.g. ResNet or EfficientNet) with only one line 
 of code to support additional channels to the already given RGB channels. Even pre-trained neural networks 
-like ResNet50 can be used.
+can be used.
 
 ## Installing / Getting started
 
 Installation works with pypi.
 
 ```shell
 pip install multi-channel-pytorch
@@ -29,15 +29,15 @@
 
 You can add multi channel functionality to one of the previous mentioned architectures with just one line of
 code. 
 
 The following is an example of adding multi-channel support to a pre-trained ResNet50 model:
 
 ```python
-from multi_channel_pytorch import multify
+from multi_channel_pytorch.multify import multify
 from torchvision.models import resnet50
 
 # Create a ResNet50 model with pretrained weights.
 model = resnet50(weights='DEFAULT')
 
 # Add a fourth channel to the previously created model.
 model = multify(model=model, num_channels=4)
@@ -65,8 +65,8 @@
 
 # Copying weights for the first three channels.
 model.conv1.weight[:, :3] = weight
 ```
 
 ## Licensing
 
-The code in this project is licensed under GNU General Public License v3.0.
+The code in this project is licensed under GNU General Public License v3.0.
```

### Comparing `multi_channel_pytorch-0.2.0/PKG-INFO` & `multi_channel_pytorch-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-channel-pytorch
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library for adding multi channel functionality to PyTorch models.
 Home-page: https://github.com/Timom1996/multi-channel-pytorch
 License: GPL-3.0-only
 Author: Timo Michel
 Author-email: timo.michel1996@outlook.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 
 # Multi-Channel-Pytorch
 > torch, torchvision, multi-channel-input
 
 This library allows to modify known network architectures (e.g. ResNet or EfficientNet) with only one line 
 of code to support additional channels to the already given RGB channels. Even pre-trained neural networks 
-like ResNet50 can be used.
+can be used.
 
 ## Installing / Getting started
 
 Installation works with pypi.
 
 ```shell
 pip install multi-channel-pytorch
@@ -46,15 +46,15 @@
 
 You can add multi channel functionality to one of the previous mentioned architectures with just one line of
 code. 
 
 The following is an example of adding multi-channel support to a pre-trained ResNet50 model:
 
 ```python
-from multi_channel_pytorch import multify
+from multi_channel_pytorch.multify import multify
 from torchvision.models import resnet50
 
 # Create a ResNet50 model with pretrained weights.
 model = resnet50(weights='DEFAULT')
 
 # Add a fourth channel to the previously created model.
 model = multify(model=model, num_channels=4)
@@ -83,7 +83,8 @@
 # Copying weights for the first three channels.
 model.conv1.weight[:, :3] = weight
 ```
 
 ## Licensing
 
 The code in this project is licensed under GNU General Public License v3.0.
+
```

