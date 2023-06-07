# Comparing `tmp/jac_vision-1.4.0.9.tar.gz` & `tmp/jac_vision-1.4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_vision-1.4.0.9.tar", last modified: Tue Feb 14 17:26:23 2023, max compression
+gzip compressed data, was "jac_vision-1.4.1.0.tar", last modified: Wed Jun  7 18:25:19 2023, max compression
```

## Comparing `jac_vision-1.4.0.9.tar` & `jac_vision-1.4.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:23.223791 jac_vision-1.4.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-14 17:26:23.223791 jac_vision-1.4.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:23.219791 jac_vision-1.4.0.9/jac_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:23.219791 jac_vision-1.4.0.9/jac_vision/detr/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/detr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/detr/detr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/detr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/detr/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:23.219791 jac_vision-1.4.0.9/jac_vision/dpt/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/dpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/dpt/dpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/dpt/model.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/dpt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:23.219791 jac_vision-1.4.0.9/jac_vision/rftm/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/rftm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/rftm/model.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/rftm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/rftm/rftm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:23.219791 jac_vision-1.4.0.9/jac_vision/yolos/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/yolos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/yolos/model.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/yolos/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/jac_vision/yolos/yolos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:23.219791 jac_vision-1.4.0.9/jac_vision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-14 17:26:23.000000 jac_vision-1.4.0.9/jac_vision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-14 17:26:23.000000 jac_vision-1.4.0.9/jac_vision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 17:26:23.000000 jac_vision-1.4.0.9/jac_vision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-14 17:26:23.000000 jac_vision-1.4.0.9/jac_vision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-14 17:26:23.000000 jac_vision-1.4.0.9/jac_vision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 17:26:23.223791 jac_vision-1.4.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-14 17:25:59.000000 jac_vision-1.4.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:19.866539 jac_vision-1.4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-07 18:25:19.866539 jac_vision-1.4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:19.862539 jac_vision-1.4.1.0/jac_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:19.862539 jac_vision-1.4.1.0/jac_vision/detr/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/detr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/detr/detr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/detr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/detr/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:19.862539 jac_vision-1.4.1.0/jac_vision/dpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/dpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/dpt/dpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/dpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/dpt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:19.862539 jac_vision-1.4.1.0/jac_vision/rftm/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/rftm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/rftm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/rftm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/rftm/rftm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:19.866539 jac_vision-1.4.1.0/jac_vision/yolos/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/yolos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/yolos/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/yolos/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/jac_vision/yolos/yolos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:19.862539 jac_vision-1.4.1.0/jac_vision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-07 18:25:19.000000 jac_vision-1.4.1.0/jac_vision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-07 18:25:19.000000 jac_vision-1.4.1.0/jac_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:25:19.000000 jac_vision-1.4.1.0/jac_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-07 18:25:19.000000 jac_vision-1.4.1.0/jac_vision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 18:25:19.000000 jac_vision-1.4.1.0/jac_vision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:25:19.866539 jac_vision-1.4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-07 18:24:42.000000 jac_vision-1.4.1.0/setup.py
```

### Comparing `jac_vision-1.4.0.9/jac_vision/detr/detr.py` & `jac_vision-1.4.1.0/jac_vision/yolos/yolos.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from .model import DetrDetector
+from .model import YolosDetector
 import torch
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 import traceback
 from fastapi import HTTPException
-from PIL import Image
 import base64
 import io
+from PIL import Image
 
 
-def setup(model: str = "detr-resnet-50", device: str = None):
+@jaseci_action(act_group=["yolos"], allow_remote=True)
+def setup(device: str = None):
     global detector
     if device is None:
         _device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     else:
         _device = torch.device(device)
-    detector = DetrDetector(device=_device, model=model)
-
-
-setup(model="detr-resnet-50", device=None)
+    detector = YolosDetector(device=_device)
 
 
-@jaseci_action(act_group=["detr"], allow_remote=True)
+@jaseci_action(act_group=["yolos"], allow_remote=True)
 def detect(image, b64: bool = False, threshold: float = 0.5) -> list:
     try:
         if threshold > 1 or threshold < 0:
             raise ValueError("Threshold must be between 0 and 1")
         _image = (
             Image.open(io.BytesIO(base64.b64decode(image)))
             if b64
@@ -32,15 +30,15 @@
         )
         return detector.detect(_image, threshold)
     except Exception as e:
         traceback.print_exc()
         raise HTTPException(status_code=500, detail=str(e))
 
 
-@jaseci_action(act_group=["detr"], allow_remote=True)
+@jaseci_action(act_group=["yolos"], allow_remote=True)
 def detect_batch(images, b64: bool = False, threshold: float = 0.5) -> list:
     try:
         if threshold > 1 or threshold < 0:
             raise ValueError("Threshold must be between 0 and 1")
         _images = (
             [Image.open(io.BytesIO(base64.b64decode(image))) for image in images]
             if b64
@@ -48,16 +46,16 @@
         )
         return detector.detect_batch(_images, threshold)
     except Exception as e:
         traceback.print_exc()
         raise HTTPException(status_code=500, detail=str(e))
 
 
-@jaseci_action(act_group=["detr"], allow_remote=True)
+@jaseci_action(act_group=["yolos"], allow_remote=True)
 def get_labels() -> list:
     return detector.get_labels()
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_vision-1.4.0.9/jac_vision/detr/model.py` & `jac_vision-1.4.1.0/jac_vision/detr/model.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.0.9/jac_vision/dpt/dpt.py` & `jac_vision-1.4.1.0/jac_vision/dpt/dpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from .model import DPTLarge
 import torch
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 import traceback
 from fastapi import HTTPException
 from PIL import Image
 import base64
 import io
 
 
+@jaseci_action(act_group=["dpt"], allow_remote=True)
 def setup(model: str = "dpt-large", device: str = None):
     global detector
     if device is None:
         _device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     else:
         _device = torch.device(device)
     detector = DPTLarge(device=_device, model=model)
 
 
-setup(model="dpt-large", device=None)
-
-
 @jaseci_action(act_group=["dpt"], allow_remote=True)
 def estimate(image: str, b64: bool = False) -> str:
     try:
         _image = (
             Image.open(io.BytesIO(base64.b64decode(image)))
             if b64
             else Image.open(image)
@@ -50,10 +48,10 @@
         ]
     except Exception as e:
         traceback.print_exc()
         raise HTTPException(status_code=500, detail=str(e))
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_vision-1.4.0.9/jac_vision/dpt/model.py` & `jac_vision-1.4.1.0/jac_vision/dpt/model.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.0.9/jac_vision/rftm/model.py` & `jac_vision-1.4.1.0/jac_vision/rftm/model.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.0.9/jac_vision/rftm/rftm.py` & `jac_vision-1.4.1.0/jac_vision/rftm/rftm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import torch
 from PIL import Image
 import torch
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 import traceback
 from fastapi import HTTPException
 import base64
 import io
 import os
 import requests
 from .model import RFTM, ToTensor
 
-RTFM_CLASSIFIER_WEIGHTS = "https://huggingface.co/spaces/jaseci/video-anomaly-detection/resolve/main/rftm_classifier.pth"
-RTFM_RESNET_101_WEIGHTS = "https://huggingface.co/spaces/jaseci/video-anomaly-detection/resolve/main/rftm_resnet101.pth"
+RTFM_CLASSIFIER_WEIGHTS = (
+    "https://huggingface.co/jaseci/rtfm/resolve/main/rtfm_classifier.pth"
+)
+RTFM_RESNET_101_WEIGHTS = (
+    "https://huggingface.co/jaseci/rtfm/resolve/main/rtfm_resnet101.pth"
+)
 
 
+@jaseci_action(act_group=["rftm"], allow_remote=True)
 def setup(device: str = None):
     global detector, _device
     os.makedirs("weights", exist_ok=True)
     if not os.path.exists(os.path.join("weights", "rftm_classifier.pth")):
         with open("weights/rftm_classifier.pth", "wb") as f:
             f.write(requests.get(RTFM_CLASSIFIER_WEIGHTS).content)
     if not os.path.exists(os.path.join("weights", "rftm_resnet101.pth")):
@@ -28,17 +33,14 @@
         torch.device("cuda" if torch.cuda.is_available() else "cpu")
         if device is None
         else torch.device(device)
     )
     detector = RFTM(device=_device)
 
 
-setup(device=None)
-
-
 @jaseci_action(act_group=["rftm"], allow_remote=True)
 def predict(frames: list, b64: bool = False) -> float:
     try:
         if b64:
             frames = [io.BytesIO(base64.b64decode(frame)) for frame in frames]
         if len(frames) != 16:
             raise ValueError("Must have 16 frames")
@@ -50,10 +52,10 @@
         return out.item()
     except Exception as e:
         traceback.print_exc()
         raise HTTPException(status_code=500, detail=str(e))
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_vision-1.4.0.9/jac_vision/yolos/model.py` & `jac_vision-1.4.1.0/jac_vision/yolos/model.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.0.9/jac_vision/yolos/yolos.py` & `jac_vision-1.4.1.0/jac_vision/detr/detr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from .model import YolosDetector
+from .model import DetrDetector
 import torch
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 import traceback
 from fastapi import HTTPException
+from PIL import Image
 import base64
 import io
-from PIL import Image
 
 
-def setup(device: str = None):
+@jaseci_action(act_group=["detr"], allow_remote=True)
+def setup(model: str = "detr-resnet-50", device: str = None):
     global detector
     if device is None:
         _device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     else:
         _device = torch.device(device)
-    detector = YolosDetector(device=_device)
-
-
-setup(device=None)
+    detector = DetrDetector(device=_device, model=model)
 
 
-@jaseci_action(act_group=["yolos"], allow_remote=True)
+@jaseci_action(act_group=["detr"], allow_remote=True)
 def detect(image, b64: bool = False, threshold: float = 0.5) -> list:
     try:
         if threshold > 1 or threshold < 0:
             raise ValueError("Threshold must be between 0 and 1")
         _image = (
             Image.open(io.BytesIO(base64.b64decode(image)))
             if b64
@@ -32,15 +30,15 @@
         )
         return detector.detect(_image, threshold)
     except Exception as e:
         traceback.print_exc()
         raise HTTPException(status_code=500, detail=str(e))
 
 
-@jaseci_action(act_group=["yolos"], allow_remote=True)
+@jaseci_action(act_group=["detr"], allow_remote=True)
 def detect_batch(images, b64: bool = False, threshold: float = 0.5) -> list:
     try:
         if threshold > 1 or threshold < 0:
             raise ValueError("Threshold must be between 0 and 1")
         _images = (
             [Image.open(io.BytesIO(base64.b64decode(image))) for image in images]
             if b64
@@ -48,16 +46,16 @@
         )
         return detector.detect_batch(_images, threshold)
     except Exception as e:
         traceback.print_exc()
         raise HTTPException(status_code=500, detail=str(e))
 
 
-@jaseci_action(act_group=["yolos"], allow_remote=True)
+@jaseci_action(act_group=["detr"], allow_remote=True)
 def get_labels() -> list:
     return detector.get_labels()
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_vision-1.4.0.9/jac_vision.egg-info/SOURCES.txt` & `jac_vision-1.4.1.0/jac_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.0.9/setup.py` & `jac_vision-1.4.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,16 +18,20 @@
     return extras_requires
 
 
 setup(
     name="jac_vision",
     version=get_ver(),
     packages=find_packages(include=["jac_vision", "jac_vision.*"]),
-    install_requires=["jaseci", "pytest>=7.0.1,<7.1", "pytest-order>=1.0.1,<1.1"],
+    install_requires=[
+        f"jaseci=={get_ver()}",
+        "pytest>=7.0.1,<7.1",
+        "pytest-order>=1.0.1,<1.1",
+    ],
     extras_require=get_extras_requires(),
     package_data={
-        "": ["*.json", "*.cfg", "VERSION", "*.yaml", "requirements.txt"],
+        "": ["*.json", "*.cfg", "VERSION", "*.yaml", "requirements.txt", "*.jac"],
     },
     author="Jason Mars",
     author_email="jason@jaseci.org",
     url="https://github.com/Jaseci-Labs/jaseci",
 )
```

