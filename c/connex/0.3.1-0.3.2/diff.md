# Comparing `tmp/connex-0.3.1.tar.gz` & `tmp/connex-0.3.2.tar.gz`

## Comparing `connex-0.3.1.tar` & `connex-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 connex-0.3.1/connex/__init__.py
--rw-r--r--   0        0        0    33125 2020-02-02 00:00:00.000000 connex-0.3.1/connex/_network.py
--rw-r--r--   0        0        0    46899 2020-02-02 00:00:00.000000 connex-0.3.1/connex/_plasticity.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 connex-0.3.1/connex/_utils.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 connex-0.3.1/connex/nn/__init__.py
--rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 connex-0.3.1/connex/nn/_dense_mlp.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 connex-0.3.1/connex/nn/_mlp.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 connex-0.3.1/connex/nn/_utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 connex-0.3.1/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 connex-0.3.1/LICENSE
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 connex-0.3.1/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 connex-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    17707 2020-02-02 00:00:00.000000 connex-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 connex-0.3.2/connex/__init__.py
+-rw-r--r--   0        0        0    33075 2020-02-02 00:00:00.000000 connex-0.3.2/connex/_network.py
+-rw-r--r--   0        0        0    46899 2020-02-02 00:00:00.000000 connex-0.3.2/connex/_plasticity.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 connex-0.3.2/connex/_utils.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 connex-0.3.2/connex/nn/__init__.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 connex-0.3.2/connex/nn/_dense_mlp.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 connex-0.3.2/connex/nn/_mlp.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 connex-0.3.2/connex/nn/_utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 connex-0.3.2/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 connex-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 connex-0.3.2/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 connex-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    17686 2020-02-02 00:00:00.000000 connex-0.3.2/PKG-INFO
```

### Comparing `connex-0.3.1/connex/_network.py` & `connex-0.3.2/connex/_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,22 +265,25 @@
                 )
                 vals = _apply_neuron_self_attention(
                     tb, attn_params_n, attn_mask_n, vals
                 )
 
             # Affine transformation, wx + b
             weights, biases = w_and_b[:, :-1], w_and_b[:, -1]
-            affine = (weights * mask) @ vals + biases
+            if self._use_neuron_self_attention:
+                affine = vmap(jnp.dot)(weights * mask, vals) + biases
+            else:
+                affine = (weights * mask) @ vals + biases
 
             # Apply activations/dropout
-            if self._use_adaptive_activations:
-                _apply_activation = vmap(self._apply_activation)
-            else:
-                _apply_activation = vmap(self._apply_activation, in_axes=(0, 0, None))
-            output_values = _apply_activation(tb, affine, ada_params) * dropout_mask[tb]
+            if not self._use_adaptive_activations:
+                ada_params = jnp.ones((tb.shape[0], 2))
+            output_values = (
+                vmap(self._apply_activation)(tb, affine, ada_params) * dropout_mask[tb]
+            )
 
             # Set new values
             values = values.at[tb].set(output_values)
 
         # Return values pertaining to output neurons, with the group-wise
         # output activation applied
         return self._output_transformation(values[self._output_neurons_id])
@@ -332,18 +335,15 @@
         rsqrt = lax.rsqrt(self._num_inputs_per_neuron[id])
         scaled_outer_product = jnp.outer(query, key) * rsqrt
         attention_weights = jnn.softmax(scaled_outer_product - attn_mask)
         return attention_weights @ value + vals
 
     def _apply_activation(self, id: Array, affine: Array, ada_params: Array) -> Array:
         """Function for a single neuron to apply its activation."""
-        ones = jnp.ones((2,))
-        a, b = lax.cond(
-            self._use_adaptive_activations, lambda: ada_params * ones, lambda: ones
-        )
+        a, b = ada_params
         _expand = ft.partial(jnp.expand_dims, axis=0)
         output = lax.cond(
             jnp.isin(id, self._output_neurons_id),
             lambda: _expand(affine),
             lambda: self._hidden_activation(_expand(affine * b)) * a,
         )
         return jnp.squeeze(output)
```

### Comparing `connex-0.3.1/connex/_plasticity.py` & `connex-0.3.2/connex/_plasticity.py`

 * *Files identical despite different names*

### Comparing `connex-0.3.1/connex/_utils.py` & `connex-0.3.2/connex/_utils.py`

 * *Files identical despite different names*

### Comparing `connex-0.3.1/connex/nn/_dense_mlp.py` & `connex-0.3.2/connex/nn/_dense_mlp.py`

 * *Files identical despite different names*

### Comparing `connex-0.3.1/connex/nn/_mlp.py` & `connex-0.3.2/connex/nn/_mlp.py`

 * *Files identical despite different names*

### Comparing `connex-0.3.1/LICENSE` & `connex-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `connex-0.3.1/README.md` & `connex-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -113,11 +113,10 @@
 ## Citation
 
 ```bibtex
 @software{gleyzer2023connex,
   author = {Leonard Gleyzer},
   title = {{C}onnex: Fine-grained Control over Neural Network Topology in {JAX}},
   url = {http://github.com/leonard-gleyzer/connex},
-  version = {0.3.0},
   year = {2023},
 }
 ```
```

### Comparing `connex-0.3.1/pyproject.toml` & `connex-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "connex"
-version = "0.3.1"
+version = "0.3.2"
 description = "Fine-grained, dynamic control of neural network topology in JAX."
 readme = "README.md"
 requires-python ="~=3.9"
 license = {file = "LICENSE"}
 authors = [
   {name = "Leonard Gleyzer", email = "lenny@lenn.ai"},
 ]
```

### Comparing `connex-0.3.1/PKG-INFO` & `connex-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connex
-Version: 0.3.1
+Version: 0.3.2
 Summary: Fine-grained, dynamic control of neural network topology in JAX.
 Project-URL: repository, https://github.com/leonard-gleyzer/connex
 Author-email: Leonard Gleyzer <lenny@lenn.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -339,11 +339,10 @@
 ## Citation
 
 ```bibtex
 @software{gleyzer2023connex,
   author = {Leonard Gleyzer},
   title = {{C}onnex: Fine-grained Control over Neural Network Topology in {JAX}},
   url = {http://github.com/leonard-gleyzer/connex},
-  version = {0.3.0},
   year = {2023},
 }
 ```
```

