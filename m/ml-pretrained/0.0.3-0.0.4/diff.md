# Comparing `tmp/ml-pretrained-0.0.3.tar.gz` & `tmp/ml-pretrained-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-pretrained-0.0.3.tar", last modified: Wed Jun  7 00:31:48 2023, max compression
+gzip compressed data, was "ml-pretrained-0.0.4.tar", last modified: Wed Jun  7 02:47:10 2023, max compression
```

## Comparing `ml-pretrained-0.0.3.tar` & `ml-pretrained-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:31:48.589548 ml-pretrained-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 00:31:48.589548 ml-pretrained-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:31:48.585548 ml-pretrained-0.0.3/ml_pretrained.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 00:31:48.000000 ml-pretrained-0.0.3/ml_pretrained.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 00:31:48.000000 ml-pretrained-0.0.3/ml_pretrained.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:31:48.000000 ml-pretrained-0.0.3/ml_pretrained.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 00:31:48.000000 ml-pretrained-0.0.3/ml_pretrained.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 00:31:48.000000 ml-pretrained-0.0.3/ml_pretrained.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:31:48.585548 ml-pretrained-0.0.3/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/tacotron2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:31:48.589548 ml-pretrained-0.0.3/pretrained/vocoder/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/vocoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/vocoder/hifigan.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/vocoder/waveglow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 00:31:48.589548 ml-pretrained-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:31:48.589548 ml-pretrained-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/tests/test_rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/tests/test_tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:47:10.512313 ml-pretrained-0.0.4/ml_pretrained.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 02:47:10.000000 ml-pretrained-0.0.4/ml_pretrained.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 02:47:10.000000 ml-pretrained-0.0.4/ml_pretrained.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:47:10.000000 ml-pretrained-0.0.4/ml_pretrained.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 02:47:10.000000 ml-pretrained-0.0.4/ml_pretrained.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 02:47:10.000000 ml-pretrained-0.0.4/ml_pretrained.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/pretrained/vocoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/vocoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/vocoder/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pretrained/vocoder/waveglow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:47:10.516313 ml-pretrained-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/tests/test_rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 02:46:55.000000 ml-pretrained-0.0.4/tests/test_tacotron2.py
```

### Comparing `ml-pretrained-0.0.3/LICENSE` & `ml-pretrained-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/PKG-INFO` & `ml-pretrained-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.3
+Version: 0.0.4
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.3/README.md` & `ml-pretrained-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/ml_pretrained.egg-info/PKG-INFO` & `ml-pretrained-0.0.4/ml_pretrained.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.3
+Version: 0.0.4
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.3/ml_pretrained.egg-info/SOURCES.txt` & `ml-pretrained-0.0.4/ml_pretrained.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/pretrained/blip.py` & `ml-pretrained-0.0.4/pretrained/blip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/pretrained/clip.py` & `ml-pretrained-0.0.4/pretrained/clip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/pretrained/hubert.py` & `ml-pretrained-0.0.4/pretrained/hubert.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/pretrained/llama.py` & `ml-pretrained-0.0.4/pretrained/llama.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/pretrained/rwkv.py` & `ml-pretrained-0.0.4/pretrained/rwkv.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,18 @@
         self.head = maybe_lora(nn.Linear(emb_dim, num_tokens, bias=False), lora_rank)
 
         # Disables updating the layer norm parameters if using LoRA.
         if lora_rank is not None:
             self.ln_out.requires_grad_(False)
 
     def tensor_to(self, x: Tensor) -> Tensor:
-        return x.to(self.head.weight)
+        ref_tensor = self.head.weight
+        if x.is_floating_point():
+            return x.to(ref_tensor)
+        return x.to(ref_tensor.device)
 
     def forward(self, tokens: Tensor, states_in: list[State] | None = None) -> tuple[Tensor, list[State]]:
         x = self.emb(tokens)
         states_out: list[State] = []
         for i, block in enumerate(self.blocks):
             x, state_out = block(x, None if states_in is None else states_in[i])
             states_out.append(state_out)
```

### Comparing `ml-pretrained-0.0.3/pretrained/sam.py` & `ml-pretrained-0.0.4/pretrained/sam.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/pretrained/tacotron2.py` & `ml-pretrained-0.0.4/pretrained/tacotron2.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/pretrained/vocoder/__init__.py` & `ml-pretrained-0.0.4/pretrained/vocoder/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/pretrained/vocoder/hifigan.py` & `ml-pretrained-0.0.4/pretrained/vocoder/hifigan.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/pretrained/vocoder/waveglow.py` & `ml-pretrained-0.0.4/pretrained/vocoder/waveglow.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/pyproject.toml` & `ml-pretrained-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/setup.py` & `ml-pretrained-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/tests/test_rwkv.py` & `ml-pretrained-0.0.4/tests/test_rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.3/tests/test_tacotron2.py` & `ml-pretrained-0.0.4/tests/test_tacotron2.py`

 * *Files identical despite different names*

