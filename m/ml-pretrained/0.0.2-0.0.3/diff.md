# Comparing `tmp/ml-pretrained-0.0.2.tar.gz` & `tmp/ml-pretrained-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-pretrained-0.0.2.tar", last modified: Fri Jun  2 05:13:27 2023, max compression
+gzip compressed data, was "ml-pretrained-0.0.3.tar", last modified: Wed Jun  7 00:31:48 2023, max compression
```

## Comparing `ml-pretrained-0.0.2.tar` & `ml-pretrained-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:13:27.887265 ml-pretrained-0.0.2/ml_pretrained.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-02 05:13:27.000000 ml-pretrained-0.0.2/ml_pretrained.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-02 05:13:27.000000 ml-pretrained-0.0.2/ml_pretrained.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 05:13:27.000000 ml-pretrained-0.0.2/ml_pretrained.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-02 05:13:27.000000 ml-pretrained-0.0.2/ml_pretrained.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 05:13:27.000000 ml-pretrained-0.0.2/ml_pretrained.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/tacotron2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/pretrained/vocoder/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/vocoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/vocoder/hifigan.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/vocoder/waveglow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/tests/test_rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/tests/test_tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:31:48.589548 ml-pretrained-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 00:31:48.589548 ml-pretrained-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:31:48.585548 ml-pretrained-0.0.3/ml_pretrained.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 00:31:48.000000 ml-pretrained-0.0.3/ml_pretrained.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 00:31:48.000000 ml-pretrained-0.0.3/ml_pretrained.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:31:48.000000 ml-pretrained-0.0.3/ml_pretrained.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 00:31:48.000000 ml-pretrained-0.0.3/ml_pretrained.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 00:31:48.000000 ml-pretrained-0.0.3/ml_pretrained.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:31:48.585548 ml-pretrained-0.0.3/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:31:48.589548 ml-pretrained-0.0.3/pretrained/vocoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/vocoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/vocoder/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pretrained/vocoder/waveglow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 00:31:48.589548 ml-pretrained-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:31:48.589548 ml-pretrained-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/tests/test_rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 00:31:37.000000 ml-pretrained-0.0.3/tests/test_tacotron2.py
```

### Comparing `ml-pretrained-0.0.2/ml_pretrained.egg-info/SOURCES.txt` & `ml-pretrained-0.0.3/ml_pretrained.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 ml_pretrained.egg-info/PKG-INFO
 ml_pretrained.egg-info/SOURCES.txt
```

### Comparing `ml-pretrained-0.0.2/pretrained/blip.py` & `ml-pretrained-0.0.3/pretrained/blip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.2/pretrained/clip.py` & `ml-pretrained-0.0.3/pretrained/clip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.2/pretrained/hubert.py` & `ml-pretrained-0.0.3/pretrained/hubert.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.2/pretrained/llama.py` & `ml-pretrained-0.0.3/pretrained/llama.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 import torch
 import torch.nn.functional as F
 from omegaconf import MISSING
 from torch import Tensor, nn
 
 from ml.core.config import conf_field
 from ml.core.env import get_model_dir
+from ml.models.lora import maybe_lora
 from ml.models.parallel import ColumnParallelLinear, ParallelEmbedding, RowParallelLinear
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.parallel import parallel_group_info
 from ml.utils.timer import Timer
@@ -123,24 +124,28 @@
     freqs_cis = reshape_for_broadcast(freqs_cis, xq_)
     xq_out = torch.view_as_real(xq_ * freqs_cis).flatten(3)
     xk_out = torch.view_as_real(xk_ * freqs_cis).flatten(3)
     return xq_out.type_as(xq), xk_out.type_as(xk)
 
 
 class Attention(nn.Module):
-    def __init__(self, args: ModelArgs) -> None:
+    def __init__(self, args: ModelArgs, lora_rank: int | None = None) -> None:
         super().__init__()
 
         self.n_local_heads = args.n_heads // parallel_group_info().mp.world_size
         self.head_dim = args.dim // args.n_heads
 
-        self.wq = ColumnParallelLinear(args.dim, args.n_heads * self.head_dim, bias=False, gather_output=False)
-        self.wk = ColumnParallelLinear(args.dim, args.n_heads * self.head_dim, bias=False, gather_output=False)
-        self.wv = ColumnParallelLinear(args.dim, args.n_heads * self.head_dim, bias=False, gather_output=False)
-        self.wo = RowParallelLinear(args.n_heads * self.head_dim, args.dim, bias=False, input_is_parallel=True)
+        wq = ColumnParallelLinear(args.dim, args.n_heads * self.head_dim, bias=False, gather_output=False)
+        wk = ColumnParallelLinear(args.dim, args.n_heads * self.head_dim, bias=False, gather_output=False)
+        wv = ColumnParallelLinear(args.dim, args.n_heads * self.head_dim, bias=False, gather_output=False)
+        wo = RowParallelLinear(args.n_heads * self.head_dim, args.dim, bias=False, input_is_parallel=True)
+        self.wq = maybe_lora(wq, lora_rank)
+        self.wk = maybe_lora(wk, lora_rank)
+        self.wv = maybe_lora(wv, lora_rank)
+        self.wo = maybe_lora(wo, lora_rank)
 
     def forward(
         self,
         x: Tensor,
         freqs_cis: Tensor,
         is_causal: bool,
         cache: tuple[Tensor, Tensor] | None = None,
@@ -174,41 +179,54 @@
 
 class FeedForward(nn.Module):
     def __init__(
         self,
         dim: int,
         hidden_dim: int,
         multiple_of: int,
+        lora_rank: int | None = None,
     ) -> None:
         super().__init__()
 
         hidden_dim = int(2 * hidden_dim / 3)
         hidden_dim = multiple_of * ((hidden_dim + multiple_of - 1) // multiple_of)
 
-        self.w1 = ColumnParallelLinear(dim, hidden_dim, bias=False, gather_output=False)
-        self.w2 = RowParallelLinear(hidden_dim, dim, bias=False, input_is_parallel=True)
-        self.w3 = ColumnParallelLinear(dim, hidden_dim, bias=False, gather_output=False)
+        w1 = ColumnParallelLinear(dim, hidden_dim, bias=False, gather_output=False)
+        w2 = RowParallelLinear(hidden_dim, dim, bias=False, input_is_parallel=True)
+        w3 = ColumnParallelLinear(dim, hidden_dim, bias=False, gather_output=False)
+        self.w1 = maybe_lora(w1, lora_rank)
+        self.w2 = maybe_lora(w2, lora_rank)
+        self.w3 = maybe_lora(w3, lora_rank)
 
     def forward(self, x: Tensor) -> Tensor:
         return self.w2(F.silu(self.w1(x)) * self.w3(x))
 
 
 class TransformerBlock(nn.Module):
-    def __init__(self, layer_id: int, args: ModelArgs) -> None:
+    def __init__(self, layer_id: int, args: ModelArgs, lora_rank: int | None = None) -> None:
         super().__init__()
 
         self.n_heads = args.n_heads
         self.dim = args.dim
         self.head_dim = args.dim // args.n_heads
-        self.attention = Attention(args)
-        self.feed_forward = FeedForward(dim=args.dim, hidden_dim=4 * args.dim, multiple_of=args.multiple_of)
+        self.attention = Attention(args, lora_rank=lora_rank)
+        self.feed_forward = FeedForward(
+            dim=args.dim,
+            hidden_dim=4 * args.dim,
+            multiple_of=args.multiple_of,
+            lora_rank=lora_rank,
+        )
         self.layer_id = layer_id
         self.attention_norm = RMSNorm(args.dim, eps=args.norm_eps)
         self.ffn_norm = RMSNorm(args.dim, eps=args.norm_eps)
 
+        if lora_rank is not None:
+            self.attention_norm.requires_grad_(False)
+            self.ffn_norm.requires_grad_(False)
+
     def forward(
         self,
         x: Tensor,
         freqs_cis: Tensor,
         is_causal: bool,
         cache: tuple[Tensor, Tensor] | None = None,
     ) -> tuple[Tensor, tuple[Tensor, Tensor]]:
@@ -252,35 +270,41 @@
     def decode(self, t: list[int]) -> str:
         return self.sp_model.decode(t)
 
 
 class Llama(nn.Module):
     freqs_cis: Tensor
 
-    def __init__(self, params: ModelArgs, tokenizer: Tokenizer | None = None) -> None:
+    def __init__(self, params: ModelArgs, tokenizer: Tokenizer | None = None, lora_rank: int | None = None) -> None:
         super().__init__()
 
         self.params = params
         self.vocab_size = params.vocab_size
         self.n_layers = params.n_layers
 
         self.tokenizer = tokenizer
 
-        self.tok_embeddings = ParallelEmbedding(params.vocab_size, params.dim)
+        tok_embeddings = ParallelEmbedding(params.vocab_size, params.dim)
+        self.tok_embeddings = maybe_lora(tok_embeddings, lora_rank)
 
         self.layers = nn.ModuleList()
         for layer_id in range(params.n_layers):
-            self.layers.append(TransformerBlock(layer_id, params))
+            self.layers.append(TransformerBlock(layer_id, params, lora_rank=lora_rank))
 
         self.norm = RMSNorm(params.dim, eps=params.norm_eps)
-        self.output = ColumnParallelLinear(params.dim, params.vocab_size, bias=False)
+        output = ColumnParallelLinear(params.dim, params.vocab_size, bias=False)
+        self.output = maybe_lora(output, lora_rank)
 
         freqs_cis = precompute_freqs_cis(self.params.dim // self.params.n_heads, self.params.max_seq_len * 2)
         self.register_buffer("freqs_cis", freqs_cis, persistent=False)
 
+        if lora_rank is not None:
+            self.tok_embeddings.requires_grad_(False)
+            self.norm.requires_grad_(False)
+
     @torch.no_grad()
     def get_mask(self, seqlen: int, ref_tensor: Tensor) -> Tensor | None:
         mask = None
         if seqlen > 1:
             mask = torch.full((1, 1, seqlen, seqlen), float("-inf"), device=ref_tensor.device)
             mask = torch.triu(mask, diagonal=1).type_as(ref_tensor)
         return mask
@@ -384,36 +408,55 @@
         self.device.module_to(llama_model)
         tokenizer = llama_model.tokenizer
         if tokenizer is None:
             raise ValueError("Tokenizer must be set to use predictor")
         self.tokenizer = tokenizer
         self.model = llama_model
 
+    def tokenize(self, prompt: str | None) -> Tensor:
+        if prompt is None:
+            prompt_tokens = torch.full((1, 1), self.tokenizer.bos_id, dtype=torch.long)
+        else:
+            prompt_tokens = torch.tensor(self.tokenizer.encode(prompt, bos=True, eos=False))
+        prompt_tokens = self.device.tensor_to(prompt_tokens)
+        return prompt_tokens
+
     @torch.inference_mode()
-    def generate(
+    def generate_for_tokens(
         self,
-        prompt: str | None = None,
+        prompt_tokens: Tensor,
         max_gen_len: int = 256,
         temperature: float = 0.8,
         top_p: float = 0.95,
     ) -> Iterator[str]:
-        if prompt is None:
-            prompt_tokens = torch.full((1, 1), self.tokenizer.bos_id, dtype=torch.long)
-        else:
-            prompt_tokens = torch.tensor(self.tokenizer.encode(prompt, bos=True, eos=False))
-
         for pred_token, _ in self.model.infer(
-            self.device.tensor_to(prompt_tokens),
+            prompt_tokens,
             max_gen_len=max_gen_len,
             temperature=temperature,
             top_p=top_p,
             eos_id=self.tokenizer.eos_id,
         ):
             yield self.tokenizer.decode(pred_token.tolist())[0]
 
+    @torch.inference_mode()
+    def generate(
+        self,
+        prompt: str | None = None,
+        max_gen_len: int = 256,
+        temperature: float = 0.8,
+        top_p: float = 0.95,
+    ) -> Iterator[str]:
+        prompt_tokens = self.tokenize(prompt)
+        yield from self.generate_for_tokens(
+            prompt_tokens,
+            max_gen_len=max_gen_len,
+            temperature=temperature,
+            top_p=top_p,
+        )
+
     @torch.no_grad()
     def unit_test_forward_matches_infer(self, prompt: str) -> bool:
         """Ensures that the forward pass matches the inference pass.
 
         This is a simple unit test which does argmax decoding for the inference
         pass to get a sequence, then passes the sequence to the forward pass.
         The output of the forward pass should match.
@@ -473,33 +516,29 @@
     with Timer("loading tokenizer", spinner=True):
         tokenizer = Tokenizer(tokenizer_path)
         model_args.vocab_size = tokenizer.n_words
 
     with Timer("building empty model", spinner=True), init_empty_weights():
         model = Llama(model_args, tokenizer)
 
-    # Logs model summary.
-    total_params = sum(p.numel() for p in model.parameters())
-    logger.info("Model %s has %s parameters", key, f"{total_params:,}")
-
     with Timer("moving model to device", spinner=True):
         device = AutoDevice.detect_device().get_device()
         model._apply(meta_to_empty_func(device, torch.half))
 
     def reset_params(module: nn.Module) -> None:
         if hasattr(module, "reset_parameters") and callable(module.reset_parameters):
             module.reset_parameters()
 
     with Timer("resetting parameters", spinner=True):
         model.apply(reset_params)
 
     return model
 
 
-def pretrained_llama(key: PretrainedLlamaKey) -> Llama:
+def pretrained_llama(key: PretrainedLlamaKey, *, lora_rank: int | None = None) -> Llama:
     rank, world_size = parallel_group_info().mp.rank, parallel_group_info().mp.world_size
 
     ckpt_dir, tokenizer_path = get_ckpt_and_tokenizer_path(key)
     if not ckpt_dir.exists():
         raise ValueError(f"LLaMa model {key} not found at {ckpt_dir}; download it first")
     if not tokenizer_path.exists():
         raise ValueError(f"LLaMa tokenizer not found at {tokenizer_path}; download it first")
@@ -520,15 +559,15 @@
     # Builds the tokenizer and updates the vocab size.
     with Timer("loading tokenizer", spinner=True):
         tokenizer = Tokenizer(model_path=tokenizer_path)
         model_args.vocab_size = tokenizer.n_words
 
     # Builds the model with empty weights.
     with Timer("building model skeleton", spinner=True), init_empty_weights():
-        model = Llama(model_args, tokenizer)
+        model = Llama(model_args, tokenizer, lora_rank=lora_rank)
 
     # Logs model summary.
     total_params = sum(p.numel() for p in model.parameters())
     logger.info("Model %s has %s parameters", key, f"{total_params:,}")
 
     # Build the transformer and loads the checkpoint.
     with Timer("loading state dict", spinner=True):
@@ -536,40 +575,46 @@
         model.load_state_dict(checkpoint)
 
     return model
 
 
 def test_worker(
     key: PretrainedLlamaKey,
-    prompt: str,
+    prompt: str | None,
     max_gen_len: int,
     temperature: float,
     top_p: float,
     pretrained: bool,
-    run_unit_test: bool,
 ) -> None:
     model = pretrained_llama(key) if pretrained else empty_llama(key)
     predictor = model.predictor()
 
     # Setting the seed across all processes to make sure that the weights
     # initialize to the same values (needed to make the test pass).
     torch.manual_seed(1337)
 
-    if run_unit_test and not predictor.unit_test_forward_matches_infer(prompt):
-        raise RuntimeError("Unit test failed!")
+    def generate_for_prompt(prompt: str) -> None:
+        print(prompt, end="")
+        for token in predictor.generate(
+            prompt=prompt,
+            max_gen_len=max_gen_len,
+            temperature=temperature,
+            top_p=top_p,
+        ):
+            print(token, end="", flush=True)
+        print()
+
+    if prompt:
+        generate_for_prompt(prompt)
 
-    print(prompt, end="")
-    for token in predictor.generate(
-        prompt=prompt,
-        max_gen_len=max_gen_len,
-        temperature=temperature,
-        top_p=top_p,
-    ):
-        print(token, end="", flush=True)
-    print()
+    else:
+        prompt = input("Prompt: ")
+        while prompt:
+            generate_for_prompt(prompt)
+            prompt = input("Prompt: ")
 
 
 def setup() -> None:
     # Hides some nuisance logs.
     logging.getLogger("torch.distributed").setLevel(logging.ERROR)
     logging.getLogger("torch.nn.parallel.distributed").setLevel(logging.ERROR)
     logging.getLogger("ml.utils.torch_distributed").setLevel(logging.ERROR)
@@ -583,21 +628,20 @@
     parser = argparse.ArgumentParser(description="Tests a pretrained LLaMA model")
     parser.add_argument("key", type=str, choices=get_args(PretrainedLlamaKey))
     parser.add_argument("prompt", type=str)
     parser.add_argument("-m", "--max-gen-len", type=int, default=256)
     parser.add_argument("-t", "--temperature", type=float, default=0.8)
     parser.add_argument("-p", "--top-p", type=float, default=0.95)
     parser.add_argument("-e", "--empty", default=False, action="store_true")
-    parser.add_argument("-s", "--unit-test", default=False, action="store_true")
     args = parser.parse_args()
 
     configure_logging()
 
     key = args.key
-    all_args = args.prompt, args.max_gen_len, args.temperature, args.top_p, not args.empty, args.unit_test
+    all_args = args.prompt, args.max_gen_len, args.temperature, args.top_p, not args.empty
     world_size = PRETRAINED_MODEL_SIZES[key].mp_size
 
     launch_subprocesses(
         functools.partial(test_worker, key, *all_args),
         MultiprocessConfig(
             world_size=world_size,
             model_parallelism=world_size,
```

### Comparing `ml-pretrained-0.0.2/pretrained/rwkv.py` & `ml-pretrained-0.0.3/pretrained/rwkv.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from dataclasses import dataclass
 from typing import Any, Iterator, Literal, Sequence, get_args
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn
 
+from ml.models.lora import maybe_lora
 from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.timer import Timer
 
@@ -178,28 +179,36 @@
 
 class Attention(nn.Module):
     init_x: Tensor
     init_num: Tensor
     init_den: Tensor
     mask: Tensor
 
-    def __init__(self, emb_dim: int, max_tsz: int = 1024) -> None:
+    def __init__(self, emb_dim: int, max_tsz: int = 1024, lora_rank: int | None = None) -> None:
         super().__init__()
 
         self.time_decay = nn.Parameter(torch.empty(emb_dim))
         self.time_first = nn.Parameter(torch.empty(emb_dim))
 
         self.time_mix_k = nn.Parameter(torch.empty(1, 1, emb_dim))
         self.time_mix_v = nn.Parameter(torch.empty(1, 1, emb_dim))
         self.time_mix_r = nn.Parameter(torch.empty(1, 1, emb_dim))
 
-        self.key = nn.Linear(emb_dim, emb_dim, bias=False)
-        self.value = nn.Linear(emb_dim, emb_dim, bias=False)
-        self.receptance = nn.Linear(emb_dim, emb_dim, bias=False)
-        self.output = nn.Linear(emb_dim, emb_dim, bias=False)
+        # Disables updating the time parameters if using LoRA.
+        if lora_rank is not None:
+            self.time_decay.requires_grad_(False)
+            self.time_first.requires_grad_(False)
+            self.time_mix_k.requires_grad_(False)
+            self.time_mix_v.requires_grad_(False)
+            self.time_mix_r.requires_grad_(False)
+
+        self.key = maybe_lora(nn.Linear(emb_dim, emb_dim, bias=False), lora_rank)
+        self.value = maybe_lora(nn.Linear(emb_dim, emb_dim, bias=False), lora_rank)
+        self.receptance = maybe_lora(nn.Linear(emb_dim, emb_dim, bias=False), lora_rank)
+        self.output = maybe_lora(nn.Linear(emb_dim, emb_dim, bias=False), lora_rank)
 
         self.register_buffer("init_x", torch.zeros(1, 1, emb_dim), persistent=False)
         self.register_buffer("init_num", torch.zeros(1, 1, emb_dim), persistent=False)
         self.register_buffer("init_den", torch.zeros(1, 1, emb_dim), persistent=False)
         self.register_buffer("mask", get_mask(max_tsz), persistent=False)
 
     def time_shift(self, last_x: Tensor, x: Tensor) -> Tensor:
@@ -225,23 +234,28 @@
 
         return self.output(rwkv), (x[..., -1:, :], num[..., -1:, :], den[..., -1:, :])
 
 
 class FeedForward(nn.Module):
     init_state: Tensor
 
-    def __init__(self, emb_dim: int, ffn_dim: int) -> None:
+    def __init__(self, emb_dim: int, ffn_dim: int, lora_rank: int | None = None) -> None:
         super().__init__()
 
         self.time_mix_k = nn.Parameter(torch.empty(1, 1, emb_dim))
         self.time_mix_r = nn.Parameter(torch.empty(1, 1, emb_dim))
 
-        self.key = nn.Linear(emb_dim, ffn_dim, bias=False)
-        self.receptance = nn.Linear(emb_dim, emb_dim, bias=False)
-        self.value = nn.Linear(ffn_dim, emb_dim, bias=False)
+        # Disables updating the time parameters if using LoRA.
+        if lora_rank is not None:
+            self.time_mix_k.requires_grad_(False)
+            self.time_mix_r.requires_grad_(False)
+
+        self.key = maybe_lora(nn.Linear(emb_dim, ffn_dim, bias=False), lora_rank)
+        self.receptance = maybe_lora(nn.Linear(emb_dim, emb_dim, bias=False), lora_rank)
+        self.value = maybe_lora(nn.Linear(ffn_dim, emb_dim, bias=False), lora_rank)
 
         self.register_buffer("init_state", torch.zeros(1, 1, emb_dim), persistent=False)
 
     def time_shift(self, last_x: Tensor, x: Tensor) -> Tensor:
         _, tsz, _ = x.shape
         if tsz > 1:
             last_x = torch.cat((last_x, x[..., :-1, :]), dim=-2)
@@ -254,42 +268,55 @@
         r = self.receptance(x * self.time_mix_r + last_x * (1 - self.time_mix_r))
         vk = self.value(F.relu(k) ** 2)
 
         return torch.sigmoid(r) * vk, x[..., -1:, :]
 
 
 class Block(nn.Module):
-    def __init__(self, emb_dim: int, pre_norm: bool) -> None:
+    def __init__(self, emb_dim: int, pre_norm: bool, lora_rank: int | None = None) -> None:
         super().__init__()
 
         self.ln0 = nn.LayerNorm(emb_dim) if pre_norm else None
         self.ln1 = nn.LayerNorm(emb_dim)
         self.ln2 = nn.LayerNorm(emb_dim)
 
-        self.att = Attention(emb_dim)
-        self.ffn = FeedForward(emb_dim, emb_dim * 4)
+        if lora_rank is not None:
+            if self.ln0 is not None:
+                self.ln0.requires_grad_(False)
+            self.ln1.requires_grad_(False)
+            self.ln2.requires_grad_(False)
+
+        self.att = Attention(emb_dim, lora_rank=lora_rank)
+        self.ffn = FeedForward(emb_dim, emb_dim * 4, lora_rank=lora_rank)
 
     def forward(self, x: Tensor, state: State | None = None) -> tuple[Tensor, State]:
         if self.ln0 is not None:
             x = self.ln0(x)
         dx, att_state_out = self.att(self.ln1(x), None if state is None else state[0])
         x = x + dx
         dx, ffn_state_out = self.ffn(self.ln2(x), None if state is None else state[1])
         x = x + dx
         return x, (att_state_out, ffn_state_out)
 
 
 class Rwkv(nn.Module):
-    def __init__(self, emb_dim: int, num_tokens: int, num_layers: int) -> None:
+    def __init__(self, emb_dim: int, num_tokens: int, num_layers: int, lora_rank: int | None = None) -> None:
         super().__init__()
 
-        self.emb = nn.Embedding(num_tokens, emb_dim)
-        self.blocks = nn.ModuleList([Block(emb_dim, i == 0) for i in range(num_layers)])
+        self.emb = maybe_lora(nn.Embedding(num_tokens, emb_dim), lora_rank)
+        self.blocks = nn.ModuleList([Block(emb_dim, i == 0, lora_rank=lora_rank) for i in range(num_layers)])
         self.ln_out = nn.LayerNorm(emb_dim)
-        self.head = nn.Linear(emb_dim, num_tokens, bias=False)
+        self.head = maybe_lora(nn.Linear(emb_dim, num_tokens, bias=False), lora_rank)
+
+        # Disables updating the layer norm parameters if using LoRA.
+        if lora_rank is not None:
+            self.ln_out.requires_grad_(False)
+
+    def tensor_to(self, x: Tensor) -> Tensor:
+        return x.to(self.head.weight)
 
     def forward(self, tokens: Tensor, states_in: list[State] | None = None) -> tuple[Tensor, list[State]]:
         x = self.emb(tokens)
         states_out: list[State] = []
         for i, block in enumerate(self.blocks):
             x, state_out = block(x, None if states_in is None else states_in[i])
             states_out.append(state_out)
@@ -310,26 +337,22 @@
         raise ImportError("Please install tokenizers with: `pip install tokenizers`")
 
     tokenizer_path = ensure_downloaded(TOKENIZER_URL, "rwkv", "tokenizer.json")
     return Tokenizer.from_file(str(tokenizer_path))
 
 
 class RwkvPredictor:
-    def __init__(self, rwkv_model: Rwkv, *, device: BaseDevice | None = None) -> None:
+    def __init__(self, rwkv_model: Rwkv) -> None:
         """Provides an API for sampling from the RWKV model.
 
         Args:
             rwkv_model: The RWKV model to use for sampling.
-            device: The device to use for sampling. If None, the device will be
-                automatically detected.
         """
         super().__init__()
 
-        self.device = AutoDevice.detect_device() if device is None else device
-        self.device.module_to(rwkv_model)
         self.tokenizer = get_tokenizer()
         self.model = rwkv_model
 
     def sample_probs(self, probs: Tensor, temperature: float = 1.0, top_p: float = 0.85) -> Tensor:
         probs = probs ** (1 / temperature)
         probs_sort, probs_idx = torch.sort(probs, dim=-1, descending=True)
         probs_sum = torch.cumsum(probs_sort, dim=-1)
@@ -348,78 +371,84 @@
         temperature: float = 1.0,
         top_p: float = 0.85,
         end_toks: Sequence[int] | None = None,
         end_strs: Sequence[str] | None = None,
     ) -> Iterator[str]:
         tokens = self.tokenizer.encode(prompt).ids
 
-        probs, state = self.model(self.device.tensor_to(torch.tensor([tokens])))
+        probs, state = self.model(self.model.tensor_to(torch.tensor([tokens])))
         probs = probs[:, -1:]
 
         end_toks_set = set() if end_toks is None else set(end_toks)
         end_strs_set = [] if end_strs is None else list(end_strs)
 
         for i in range(max_len):
             token = self.sample_probs(probs, temperature=temperature, top_p=top_p)
             if token in end_toks_set:
                 break
             token_str = self.tokenizer.decode([token.item()])
             yield token_str
             if any(e in token_str for e in end_strs_set):
                 break
             if i < max_len - 1:
-                probs, state = self.model(self.device.tensor_to(torch.tensor([[token]])), state)
+                probs, state = self.model(self.model.tensor_to(torch.tensor([[token]])), state)
 
 
-def pretrained_rwkv(key: PretrainedRwkvKey, *, device: BaseDevice | None = None) -> Rwkv:
+def pretrained_rwkv(key: PretrainedRwkvKey, *, device: BaseDevice | None = None, lora_rank: int | None = None) -> Rwkv:
     device = AutoDevice.detect_device() if device is None else device
     model_args = PRETRAINED_MODEL_SIZES[key]
     ckpt_path = ensure_downloaded(model_args.url, "rwkv", f"{key}.pth", sha256=model_args.sha256)
 
     with Timer("loading model checkpoint", spinner=True):
         ckpt = torch.load(ckpt_path, map_location="cpu")
 
     with Timer("building model skeleton", spinner=True), init_empty_weights():
-        model = Rwkv(model_args.emb_dim, 50277, model_args.num_layers)
-
-    # Logs model summary.
-    total_params = sum(p.numel() for p in model.parameters())
-    logger.info("Model %s has %s parameters", key, f"{total_params:,}")
+        model = Rwkv(model_args.emb_dim, 50277, model_args.num_layers, lora_rank=lora_rank)
 
     # Build the transformer and loads the checkpoint.
     with Timer("loading state dict", spinner=True):
         model._apply(meta_to_empty_func(device.get_device(), torch.half))
         model.load_state_dict(ckpt)
 
     return model
 
 
 def test_rwkv_adhoc() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument("size", type=str, choices=get_args(PretrainedRwkvKey))
-    parser.add_argument("prompt", type=str)
+    parser.add_argument("prompt", type=str, nargs="?")
     parser.add_argument("-t", "--tsz", type=int, default=128)
     parser.add_argument("-m", "--temperature", type=float, default=1.0)
     parser.add_argument("-p", "--top-p", type=float, default=0.85)
     parser.add_argument("-e", "--end-tok", nargs="+", default=[])
     args = parser.parse_args()
 
     configure_logging()
 
     model = pretrained_rwkv(args.size)
     predictor = model.predictor()
 
-    print(args.prompt, end="")
-    for token in predictor.generate(
-        args.prompt,
-        max_len=args.tsz,
-        temperature=args.temperature,
-        top_p=args.top_p,
-        end_strs=args.end_tok,
-    ):
-        print(token, end="", flush=True)
-    print()
+    def generate_for_prompt(prompt: str) -> None:
+        print(prompt, end="")
+        for token in predictor.generate(
+            prompt,
+            max_len=args.tsz,
+            temperature=args.temperature,
+            top_p=args.top_p,
+            end_strs=args.end_tok,
+        ):
+            print(token, end="", flush=True)
+        print()
+
+    if args.prompt:
+        generate_for_prompt(args.prompt)
+
+    else:
+        prompt = input("Prompt: ")
+        while prompt:
+            generate_for_prompt(prompt)
+            prompt = input("Prompt: ")
 
 
 if __name__ == "__main__":
     # python -m pretrained.rwkv
     test_rwkv_adhoc()
```

### Comparing `ml-pretrained-0.0.2/pretrained/sam.py` & `ml-pretrained-0.0.3/pretrained/sam.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.2/pretrained/tacotron2.py` & `ml-pretrained-0.0.3/pretrained/tacotron2.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.2/pretrained/vocoder/__init__.py` & `ml-pretrained-0.0.3/pretrained/vocoder/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.2/pretrained/vocoder/hifigan.py` & `ml-pretrained-0.0.3/pretrained/vocoder/hifigan.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.2/pretrained/vocoder/waveglow.py` & `ml-pretrained-0.0.3/pretrained/vocoder/waveglow.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.2/pyproject.toml` & `ml-pretrained-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.2/setup.py` & `ml-pretrained-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.2/tests/test_rwkv.py` & `ml-pretrained-0.0.3/tests/test_rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.2/tests/test_tacotron2.py` & `ml-pretrained-0.0.3/tests/test_tacotron2.py`

 * *Files identical despite different names*

