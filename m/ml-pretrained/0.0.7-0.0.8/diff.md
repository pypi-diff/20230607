# Comparing `tmp/ml-pretrained-0.0.7.tar.gz` & `tmp/ml-pretrained-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-pretrained-0.0.7.tar", last modified: Wed Jun  7 03:34:58 2023, max compression
+gzip compressed data, was "ml-pretrained-0.0.8.tar", last modified: Wed Jun  7 05:40:04 2023, max compression
```

## Comparing `ml-pretrained-0.0.7.tar` & `ml-pretrained-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/ml_pretrained.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 03:34:58.000000 ml-pretrained-0.0.7/ml_pretrained.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-07 03:34:58.000000 ml-pretrained-0.0.7/ml_pretrained.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:34:58.000000 ml-pretrained-0.0.7/ml_pretrained.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 03:34:58.000000 ml-pretrained-0.0.7/ml_pretrained.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 03:34:58.000000 ml-pretrained-0.0.7/ml_pretrained.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/tacotron2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/pretrained/vocoder/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/vocoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/vocoder/hifigan.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pretrained/vocoder/waveglow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 03:34:58.120495 ml-pretrained-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:34:58.116495 ml-pretrained-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/tests/test_rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 03:34:41.000000 ml-pretrained-0.0.7/tests/test_tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/ml_pretrained.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 05:40:04.000000 ml-pretrained-0.0.8/ml_pretrained.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-07 05:40:04.000000 ml-pretrained-0.0.8/ml_pretrained.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:40:04.000000 ml-pretrained-0.0.8/ml_pretrained.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 05:40:04.000000 ml-pretrained-0.0.8/ml_pretrained.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 05:40:04.000000 ml-pretrained-0.0.8/ml_pretrained.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/pretrained/vocoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/vocoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/vocoder/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/vocoder/waveglow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/tests/test_rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/tests/test_tacotron2.py
```

### Comparing `ml-pretrained-0.0.7/LICENSE` & `ml-pretrained-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/PKG-INFO` & `ml-pretrained-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.7
+Version: 0.0.8
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.7/README.md` & `ml-pretrained-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/ml_pretrained.egg-info/PKG-INFO` & `ml-pretrained-0.0.8/ml_pretrained.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.7
+Version: 0.0.8
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.7/ml_pretrained.egg-info/SOURCES.txt` & `ml-pretrained-0.0.8/ml_pretrained.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/pretrained/blip.py` & `ml-pretrained-0.0.8/pretrained/blip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/pretrained/clip.py` & `ml-pretrained-0.0.8/pretrained/clip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/pretrained/hubert.py` & `ml-pretrained-0.0.8/pretrained/hubert.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/pretrained/llama.py` & `ml-pretrained-0.0.8/pretrained/llama.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/pretrained/rwkv.py` & `ml-pretrained-0.0.8/pretrained/rwkv.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,21 +320,28 @@
 
     def tensor_to(self, x: Tensor) -> Tensor:
         ref_tensor = self.head.weight
         if x.is_floating_point():
             return x.to(ref_tensor)
         return x.to(ref_tensor.device)
 
-    def forward(self, tokens: Tensor, states_in: list[State] | None = None) -> tuple[Tensor, list[State]]:
+    def forward(
+        self,
+        tokens: Tensor,
+        states_in: list[State] | None = None,
+        return_logits: bool = False,
+    ) -> tuple[Tensor, list[State]]:
         x = self.emb(tokens)
         states_out: list[State] = []
         for i, block in enumerate(self.blocks):
             x, state_out = block(x, None if states_in is None else states_in[i])
             states_out.append(state_out)
         x = self.head(self.ln_out(x))
+        if return_logits:
+            return x, states_out
         e_x = torch.exp(x - torch.max(x))
         probs = e_x / e_x.sum()
         return probs, states_out
 
     def predictor(self) -> "RwkvPredictor":
         return RwkvPredictor(self)
 
@@ -359,37 +366,44 @@
         """
         super().__init__()
 
         self.tokenizer = get_tokenizer()
         self.model = rwkv_model
 
     def sample_probs(self, probs: Tensor, temperature: float = 1.0, top_p: float = 0.85) -> Tensor:
-        probs = probs ** (1 / temperature)
-        probs_sort, probs_idx = torch.sort(probs, dim=-1, descending=True)
-        probs_sum = torch.cumsum(probs_sort, dim=-1)
-        mask = probs_sum - probs_sort > top_p
-        probs_sort[mask] = 0.0
-        probs_sort.div_(probs_sort.sum(dim=-1, keepdim=True))
-        next_token = torch.multinomial(probs_sort.squeeze(-3), num_samples=1)
-        next_token = torch.gather(probs_idx, -1, next_token[..., None, :, :]).squeeze(-1)
-        return next_token
+        try:
+            probs = probs ** (1 / temperature)
+            probs_sort, probs_idx = torch.sort(probs, dim=-1, descending=True)
+            probs_sum = torch.cumsum(probs_sort, dim=-1)
+            mask = probs_sum - probs_sort > top_p
+            probs_sort[mask] = 0.0
+            probs_sort.div_(probs_sort.sum(dim=-1, keepdim=True) + 1e-6)
+            next_token = torch.multinomial(probs_sort.squeeze(-3), num_samples=1)
+            next_token = torch.gather(probs_idx, -1, next_token[..., None, :, :]).squeeze(-1)
+            return next_token
+
+        except Exception:
+            logger.exception("Error sampling from probabilities.")
+            return probs.new_zeros(probs.shape[:-1], dtype=torch.long)
 
     @torch.no_grad()
     def generate(
         self,
-        prompt: str,
+        prompt: str | Tensor,
         max_len: int = 256,
         temperature: float = 1.0,
         top_p: float = 0.85,
         end_toks: Sequence[int] | None = None,
         end_strs: Sequence[str] | None = None,
     ) -> Iterator[str]:
-        tokens = self.tokenizer.encode(prompt).ids
+        if isinstance(prompt, str):
+            prompt = torch.tensor([self.tokenizer.encode(prompt).ids])
+        assert prompt.dim() == 2 and prompt.shape[0] == 1
 
-        probs, state = self.model(self.model.tensor_to(torch.tensor([tokens])))
+        probs, state = self.model(self.model.tensor_to(prompt))
         probs = probs[:, -1:]
 
         end_toks_set = set() if end_toks is None else set(end_toks)
         end_strs_set = [] if end_strs is None else list(end_strs)
 
         for i in range(max_len):
             token = self.sample_probs(probs, temperature=temperature, top_p=top_p)
```

### Comparing `ml-pretrained-0.0.7/pretrained/sam.py` & `ml-pretrained-0.0.8/pretrained/sam.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/pretrained/tacotron2.py` & `ml-pretrained-0.0.8/pretrained/tacotron2.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/pretrained/vocoder/__init__.py` & `ml-pretrained-0.0.8/pretrained/vocoder/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/pretrained/vocoder/hifigan.py` & `ml-pretrained-0.0.8/pretrained/vocoder/hifigan.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/pretrained/vocoder/waveglow.py` & `ml-pretrained-0.0.8/pretrained/vocoder/waveglow.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/pyproject.toml` & `ml-pretrained-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/setup.py` & `ml-pretrained-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/tests/test_rwkv.py` & `ml-pretrained-0.0.8/tests/test_rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.7/tests/test_tacotron2.py` & `ml-pretrained-0.0.8/tests/test_tacotron2.py`

 * *Files identical despite different names*

