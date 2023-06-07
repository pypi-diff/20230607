# Comparing `tmp/ml-pretrained-0.0.5.tar.gz` & `tmp/ml-pretrained-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-pretrained-0.0.5.tar", last modified: Wed Jun  7 03:04:08 2023, max compression
+gzip compressed data, was "ml-pretrained-0.0.6.tar", last modified: Wed Jun  7 03:11:50 2023, max compression
```

## Comparing `ml-pretrained-0.0.5.tar` & `ml-pretrained-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:04:08.674118 ml-pretrained-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:04:08.674118 ml-pretrained-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:04:08.670118 ml-pretrained-0.0.5/ml_pretrained.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:04:08.000000 ml-pretrained-0.0.5/ml_pretrained.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-07 03:04:08.000000 ml-pretrained-0.0.5/ml_pretrained.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:04:08.000000 ml-pretrained-0.0.5/ml_pretrained.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 03:04:08.000000 ml-pretrained-0.0.5/ml_pretrained.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 03:04:08.000000 ml-pretrained-0.0.5/ml_pretrained.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:04:08.670118 ml-pretrained-0.0.5/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/tacotron2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:04:08.670118 ml-pretrained-0.0.5/pretrained/vocoder/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/vocoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/vocoder/hifigan.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pretrained/vocoder/waveglow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 03:04:08.674118 ml-pretrained-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:04:08.674118 ml-pretrained-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/tests/test_rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 03:03:57.000000 ml-pretrained-0.0.5/tests/test_tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:50.579413 ml-pretrained-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:11:50.579413 ml-pretrained-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:50.575413 ml-pretrained-0.0.6/ml_pretrained.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:11:50.000000 ml-pretrained-0.0.6/ml_pretrained.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-07 03:11:50.000000 ml-pretrained-0.0.6/ml_pretrained.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:11:50.000000 ml-pretrained-0.0.6/ml_pretrained.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 03:11:50.000000 ml-pretrained-0.0.6/ml_pretrained.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 03:11:50.000000 ml-pretrained-0.0.6/ml_pretrained.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:50.575413 ml-pretrained-0.0.6/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:50.575413 ml-pretrained-0.0.6/pretrained/vocoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/vocoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/vocoder/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pretrained/vocoder/waveglow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 03:11:50.579413 ml-pretrained-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:11:50.579413 ml-pretrained-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/tests/test_rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 03:11:37.000000 ml-pretrained-0.0.6/tests/test_tacotron2.py
```

### Comparing `ml-pretrained-0.0.5/LICENSE` & `ml-pretrained-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/PKG-INFO` & `ml-pretrained-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.5
+Version: 0.0.6
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.5/README.md` & `ml-pretrained-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/ml_pretrained.egg-info/PKG-INFO` & `ml-pretrained-0.0.6/ml_pretrained.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.5
+Version: 0.0.6
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.5/ml_pretrained.egg-info/SOURCES.txt` & `ml-pretrained-0.0.6/ml_pretrained.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/pretrained/blip.py` & `ml-pretrained-0.0.6/pretrained/blip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/pretrained/clip.py` & `ml-pretrained-0.0.6/pretrained/clip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/pretrained/hubert.py` & `ml-pretrained-0.0.6/pretrained/hubert.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/pretrained/llama.py` & `ml-pretrained-0.0.6/pretrained/llama.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/pretrained/rwkv.py` & `ml-pretrained-0.0.6/pretrained/rwkv.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,17 +214,22 @@
     def time_shift(self, last_x: Tensor, x: Tensor) -> Tensor:
         _, tsz, _ = x.shape
         if tsz > 1:
             last_x = torch.cat((last_x, x[..., :-1, :]), dim=-2)
         return last_x
 
     def forward(self, x: Tensor, state: AttentionState) -> tuple[Tensor, AttentionState]:
-        _, tsz, _ = x.shape
+        bsz, tsz, _ = x.shape
 
-        last_x, last_num, last_den = (self.init_x, self.init_num, self.init_den) if state is None else state
+        if state is None:
+            last_x = self.init_x.repeat(bsz, 1, 1)
+            last_num = self.init_num.repeat(bsz, 1, 1)
+            last_den = self.init_den.repeat(bsz, 1, 1)
+        else:
+            last_x, last_num, last_den = state
         last_x = self.time_shift(last_x, x)
 
         k = self.key(x * self.time_mix_k + last_x * (1 - self.time_mix_k))
         v = self.value(x * self.time_mix_v + last_x * (1 - self.time_mix_v))
         r = self.receptance(x * self.time_mix_r + last_x * (1 - self.time_mix_r))
         sr = torch.sigmoid(r)
 
@@ -258,15 +263,17 @@
     def time_shift(self, last_x: Tensor, x: Tensor) -> Tensor:
         _, tsz, _ = x.shape
         if tsz > 1:
             last_x = torch.cat((last_x, x[..., :-1, :]), dim=-2)
         return last_x
 
     def forward(self, x: Tensor, state: FeedForwardState | None = None) -> tuple[Tensor, FeedForwardState]:
-        last_x = self.time_shift(self.init_state if state is None else state, x)
+        bsz = x.shape[0]
+
+        last_x = self.time_shift(self.init_state.repeat(bsz, 1, 1) if state is None else state, x)
 
         k = self.key(x * self.time_mix_k + last_x * (1 - self.time_mix_k))
         r = self.receptance(x * self.time_mix_r + last_x * (1 - self.time_mix_r))
         vk = self.value(F.relu(k) ** 2)
 
         return torch.sigmoid(r) * vk, x[..., -1:, :]
```

### Comparing `ml-pretrained-0.0.5/pretrained/sam.py` & `ml-pretrained-0.0.6/pretrained/sam.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/pretrained/tacotron2.py` & `ml-pretrained-0.0.6/pretrained/tacotron2.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/pretrained/vocoder/__init__.py` & `ml-pretrained-0.0.6/pretrained/vocoder/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/pretrained/vocoder/hifigan.py` & `ml-pretrained-0.0.6/pretrained/vocoder/hifigan.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/pretrained/vocoder/waveglow.py` & `ml-pretrained-0.0.6/pretrained/vocoder/waveglow.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/pyproject.toml` & `ml-pretrained-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/setup.py` & `ml-pretrained-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/tests/test_rwkv.py` & `ml-pretrained-0.0.6/tests/test_rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.5/tests/test_tacotron2.py` & `ml-pretrained-0.0.6/tests/test_tacotron2.py`

 * *Files identical despite different names*

