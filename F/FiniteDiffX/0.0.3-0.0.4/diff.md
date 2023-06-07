# Comparing `tmp/FiniteDiffX-0.0.3.tar.gz` & `tmp/FiniteDiffX-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiniteDiffX-0.0.3.tar", last modified: Mon Jun  5 12:43:32 2023, max compression
+gzip compressed data, was "FiniteDiffX-0.0.4.tar", last modified: Wed Jun  7 05:10:59 2023, max compression
```

## Comparing `FiniteDiffX-0.0.3.tar` & `FiniteDiffX-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-05 12:43:32.000000 FiniteDiffX-0.0.3/FiniteDiffX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/finitediffx/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/finitediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/finitediffx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/finitediffx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/finitediffx/_src/fgrad.py
--rw-r--r--   0 runner    (1001) docker     (123)    24619 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/finitediffx/_src/finite_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/finitediffx/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:32.928156 FiniteDiffX-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/tests/test_fgrad.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-06-05 12:43:22.000000 FiniteDiffX-0.0.3/tests/test_finite_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9581 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/finitediffx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/finitediffx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/finitediffx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/finitediffx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/finitediffx/_src/fgrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24619 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/finitediffx/_src/finite_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/finitediffx/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/tests/test_fgrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/tests/test_finite_diff.py
```

### Comparing `FiniteDiffX-0.0.3/FiniteDiffX.egg-info/PKG-INFO` & `FiniteDiffX-0.0.4/FiniteDiffX.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FiniteDiffX
-Version: 0.0.3
+Version: 0.0.4
 Summary: Finite difference tools in JAX.
 Home-page: https://github.com/ASEM000/FiniteDiffX
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: MIT
 Keywords: python jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,37 +52,207 @@
 - `divergence(array, accuracy, step_size, method, keepdims)`
 - `hessian(array, accuracy, method, step_size)`
 - `laplacian(array, accuracy, method, step_size)`
 - `curl(array, step_size, method, keep_dims)`
 
 **Function transformation:**
 
-- `fgrad`: similar to `jax.grad` but with finite difference approximation.
+- `fgrad`, and `value_and_fgrad` : similar to `jax.grad` and `jax.value_and_grad` but with finite difference approximation.
 - `define_fdjvp`: define `custom_jvp` rules using finite difference approximation (see example below).
 
 ## 🛠️ Installation<a id="installation"></a>
 
 ```python
 pip install FiniteDiffX
 ```
 
 **Install development version**
 
 ```python
 pip install git+https://github.com/ASEM000/FiniteDiffX
 ```
 
+**If you find it useful to you, consider giving it a star! 🌟**
+
+<br>
+
 ## ⏩ Examples<a id="examples"></a>
 
+### **`Array` accepting functions:**
+
+```python
+
+import jax
+jax.config.update("jax_enable_x64", True)
+import jax.numpy as jnp
+import numpy.testing as npt
+
+import finitediffx as fdx
+
+# lets first define a vector valued function F: R^3 -> R^3
+# F = F1, F2
+# F1 = x^2 + y^3
+# F2 = x^4 + y^3
+# F3 = 0
+# F = [x**2 + y**3, x**4 + y**3, 0]
+
+x, y, z = [jnp.linspace(0, 1, 100)] * 3
+dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
+X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
+F1 = X**2 + Y**3
+F2 = X**4 + Y**3
+F3 = jnp.zeros_like(F1)
+F = jnp.stack([F1, F2, F3], axis=0)
+
+```
+
+<details>
+
+<summary>Difference</summary>
+
+```python
+
+# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
+dF1dx = fdx.difference(F1, axis=0, step_size=dx, accuracy=6, method="central")
+dF1dx_exact = 2 * X
+npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
+
+# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
+dF2dy = fdx.difference(F2, axis=1, step_size=dy, accuracy=6)
+dF2dy_exact = 3 * Y**2
+npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Divergence</summary>
+
+```python
+
+# ∇.F : the divergence of F
+divF = fdx.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6, method="central")
+divF_exact = 2 * X + 3 * Y**2
+npt.assert_allclose(divF, divF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Gradient</summary>
+
+```python
+
+# ∇F1 : the gradient of F1
+gradF1 = fdx.gradient(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
+gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
+npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Laplacian</summary>
+
+```python
+
+# ΔF1 : laplacian of F1
+lapF1 = fdx.laplacian(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
+lapF1_exact = 2 + 6 * Y
+npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Curl</summary>
+
+```python
+
+# ∇xF : the curl of F
+curlF = fdx.curl(F, step_size=(dx, dy, dz), accuracy=6, method="central")
+curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
+npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Jacobian</summary>
+
+```python
+
+# Jacobian of F
+JF = fdx.jacobian(F, accuracy=4, step_size=(dx, dy, dz), method="central")
+JF_exact = jnp.array(
+    [
+        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
+        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
+        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Hessian</summary>
+
+```python
+
+# Hessian of F1
+HF1 = fdx.hessian(F1, accuracy=4, step_size=(dx, dy, dz), method="central")
+HF1_exact = jnp.array(
+    [
+        [
+            2 * jnp.ones_like(X),  # ∂2F1/∂x2
+            0 * jnp.ones_like(X),  # ∂2F1/∂xy
+            0 * jnp.ones_like(X),  # ∂2F1/∂xz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂yx
+            6 * Y**2,              # ∂2F1/∂y2
+            0 * jnp.ones_like(X),  # ∂2F1/∂yz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂zx
+            0 * jnp.ones_like(X),  # ∂2F1/∂zy
+            0 * jnp.ones_like(X),  # ∂2F1/∂z2
+        ],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<br><br>
+
 ### **Function transformation:**
 
 **`fgrad`**:
 
 `fgrad` can be used in a similar way to `jax.grad`, however the `fgrad` differentiates a function based on the finite difference rules.
 
+<details> <summary> Example </summary>
+
 ```python
 
 import jax
 from jax import numpy as jnp
 import numpy as onp  # Not jax-traceable
 import finitediffx as fdx
 import functools as ft
@@ -111,18 +281,43 @@
     print(np2_rosenbach2_fdx_style2(1.,2.))
     print(jnp_rosenbach2(1., 2.))
 # 402.0000951997936
 # 402.0000000002219
 # 402.0
 ```
 
+Also works on pytrees
+
+```python
+
+import finitediffx as fdx
+
+params = {"a":1., "b":2., "c":3.}
+
+@fdx.fgrad
+def func(params):
+    return params["a"]**2+params["b"]
+
+func(params)
+# {'a': Array(1.9995117, dtype=float32),
+#  'b': Array(0.9995117, dtype=float32),
+#  'c': Array(0., dtype=float32)}
+
+```
+
+</details>
+
+<br>
+
 **`define_fdjvp`**
 
 `define_fdjvp` combines `custom_jvp` and `fgrad` to define custom finite difference rules,when used with `pure_callback` it can to make non-tracable code works within `jax` machinary.
 
+<details> <summary> Example </summary>
+
 _This example is based on the comment from `jax` proposed [`JEP`](https://github.com/google/jax/issues/15425)_
 
 For example this code will fail to work with `jax` transformations, becasue it uses `numpy` functions.
 
 ```python
 import numpy as onp
 import jax
@@ -200,109 +395,12 @@
     # manually set step size
     step_size=1e-3,
 )
 @wrap_pure_callback
 def numpy_func(x: onp.ndarray) -> onp.ndarray:
     return onp.power(x, 2)
 
-
 print(numpy_func(1.0))
 # 2.0000048
-
 ```
 
-### **`Array` accepting functions:**
-
-```python
-
-import jax
-
-jax.config.update("jax_enable_x64", True)
-import jax.numpy as jnp
-import numpy.testing as npt
-
-import finitediffx as fdx
-
-
-# lets first define a vector valued function F: R^3 -> R^3
-# F = F1, F2
-# F1 = x^2 + y^3
-# F2 = x^4 + y^3
-# F3 = 0
-# F = [x**2 + y**3, x**4 + y**3, 0]
-
-x, y, z = [jnp.linspace(0, 1, 100)] * 3
-dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
-X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
-F1 = X**2 + Y**3
-F2 = X**4 + Y**3
-F3 = jnp.zeros_like(F1)
-F = jnp.stack([F1, F2, F3], axis=0)
-
-# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
-dF1dx = fdx.difference(F1, axis=0, step_size=dx, accuracy=6, method="central")
-dF1dx_exact = 2 * X
-npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
-
-# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
-dF2dy = fdx.difference(F2, axis=1, step_size=dy, accuracy=6)
-dF2dy_exact = 3 * Y**2
-npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
-
-# ∇.F : the divergence of F
-divF = fdx.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6, method="central")
-divF_exact = 2 * X + 3 * Y**2
-npt.assert_allclose(divF, divF_exact, atol=1e-7)
-
-# ∇F1 : the gradient of F1
-gradF1 = fdx.gradient(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
-gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
-npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
-
-# ΔF1 : laplacian of F1
-lapF1 = fdx.laplacian(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
-lapF1_exact = 2 + 6 * Y
-npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
-
-# ∇xF : the curl of F
-curlF = fdx.curl(F, step_size=(dx, dy, dz), accuracy=6, method="central")
-curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
-npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
-
-# Jacobian of F
-JF = fdx.jacobian(F, accuracy=4, step_size=(dx, dy, dz), method="central")
-JF_exact = jnp.array(
-    [
-        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
-        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
-        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
-# Hessian of F1
-HF1 = fdx.hessian(F1, accuracy=4, step_size=(dx, dy, dz), method="central")
-HF1_exact = jnp.array(
-    [
-        [
-            2 * jnp.ones_like(X),  # ∂2F1/∂x2
-            0 * jnp.ones_like(X),  # ∂2F1/∂xy
-            0 * jnp.ones_like(X),  # ∂2F1/∂xz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂yx
-            6 * Y**2,              # ∂2F1/∂y2
-            0 * jnp.ones_like(X),  # ∂2F1/∂yz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂zx
-            0 * jnp.ones_like(X),  # ∂2F1/∂zy
-            0 * jnp.ones_like(X),  # ∂2F1/∂z2
-        ],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
-
-
-
-```
+</details>
```

### Comparing `FiniteDiffX-0.0.3/LICENSE` & `FiniteDiffX-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.3/PKG-INFO` & `FiniteDiffX-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FiniteDiffX
-Version: 0.0.3
+Version: 0.0.4
 Summary: Finite difference tools in JAX.
 Home-page: https://github.com/ASEM000/FiniteDiffX
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: MIT
 Keywords: python jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,37 +52,207 @@
 - `divergence(array, accuracy, step_size, method, keepdims)`
 - `hessian(array, accuracy, method, step_size)`
 - `laplacian(array, accuracy, method, step_size)`
 - `curl(array, step_size, method, keep_dims)`
 
 **Function transformation:**
 
-- `fgrad`: similar to `jax.grad` but with finite difference approximation.
+- `fgrad`, and `value_and_fgrad` : similar to `jax.grad` and `jax.value_and_grad` but with finite difference approximation.
 - `define_fdjvp`: define `custom_jvp` rules using finite difference approximation (see example below).
 
 ## 🛠️ Installation<a id="installation"></a>
 
 ```python
 pip install FiniteDiffX
 ```
 
 **Install development version**
 
 ```python
 pip install git+https://github.com/ASEM000/FiniteDiffX
 ```
 
+**If you find it useful to you, consider giving it a star! 🌟**
+
+<br>
+
 ## ⏩ Examples<a id="examples"></a>
 
+### **`Array` accepting functions:**
+
+```python
+
+import jax
+jax.config.update("jax_enable_x64", True)
+import jax.numpy as jnp
+import numpy.testing as npt
+
+import finitediffx as fdx
+
+# lets first define a vector valued function F: R^3 -> R^3
+# F = F1, F2
+# F1 = x^2 + y^3
+# F2 = x^4 + y^3
+# F3 = 0
+# F = [x**2 + y**3, x**4 + y**3, 0]
+
+x, y, z = [jnp.linspace(0, 1, 100)] * 3
+dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
+X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
+F1 = X**2 + Y**3
+F2 = X**4 + Y**3
+F3 = jnp.zeros_like(F1)
+F = jnp.stack([F1, F2, F3], axis=0)
+
+```
+
+<details>
+
+<summary>Difference</summary>
+
+```python
+
+# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
+dF1dx = fdx.difference(F1, axis=0, step_size=dx, accuracy=6, method="central")
+dF1dx_exact = 2 * X
+npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
+
+# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
+dF2dy = fdx.difference(F2, axis=1, step_size=dy, accuracy=6)
+dF2dy_exact = 3 * Y**2
+npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Divergence</summary>
+
+```python
+
+# ∇.F : the divergence of F
+divF = fdx.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6, method="central")
+divF_exact = 2 * X + 3 * Y**2
+npt.assert_allclose(divF, divF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Gradient</summary>
+
+```python
+
+# ∇F1 : the gradient of F1
+gradF1 = fdx.gradient(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
+gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
+npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Laplacian</summary>
+
+```python
+
+# ΔF1 : laplacian of F1
+lapF1 = fdx.laplacian(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
+lapF1_exact = 2 + 6 * Y
+npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Curl</summary>
+
+```python
+
+# ∇xF : the curl of F
+curlF = fdx.curl(F, step_size=(dx, dy, dz), accuracy=6, method="central")
+curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
+npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Jacobian</summary>
+
+```python
+
+# Jacobian of F
+JF = fdx.jacobian(F, accuracy=4, step_size=(dx, dy, dz), method="central")
+JF_exact = jnp.array(
+    [
+        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
+        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
+        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Hessian</summary>
+
+```python
+
+# Hessian of F1
+HF1 = fdx.hessian(F1, accuracy=4, step_size=(dx, dy, dz), method="central")
+HF1_exact = jnp.array(
+    [
+        [
+            2 * jnp.ones_like(X),  # ∂2F1/∂x2
+            0 * jnp.ones_like(X),  # ∂2F1/∂xy
+            0 * jnp.ones_like(X),  # ∂2F1/∂xz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂yx
+            6 * Y**2,              # ∂2F1/∂y2
+            0 * jnp.ones_like(X),  # ∂2F1/∂yz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂zx
+            0 * jnp.ones_like(X),  # ∂2F1/∂zy
+            0 * jnp.ones_like(X),  # ∂2F1/∂z2
+        ],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<br><br>
+
 ### **Function transformation:**
 
 **`fgrad`**:
 
 `fgrad` can be used in a similar way to `jax.grad`, however the `fgrad` differentiates a function based on the finite difference rules.
 
+<details> <summary> Example </summary>
+
 ```python
 
 import jax
 from jax import numpy as jnp
 import numpy as onp  # Not jax-traceable
 import finitediffx as fdx
 import functools as ft
@@ -111,18 +281,43 @@
     print(np2_rosenbach2_fdx_style2(1.,2.))
     print(jnp_rosenbach2(1., 2.))
 # 402.0000951997936
 # 402.0000000002219
 # 402.0
 ```
 
+Also works on pytrees
+
+```python
+
+import finitediffx as fdx
+
+params = {"a":1., "b":2., "c":3.}
+
+@fdx.fgrad
+def func(params):
+    return params["a"]**2+params["b"]
+
+func(params)
+# {'a': Array(1.9995117, dtype=float32),
+#  'b': Array(0.9995117, dtype=float32),
+#  'c': Array(0., dtype=float32)}
+
+```
+
+</details>
+
+<br>
+
 **`define_fdjvp`**
 
 `define_fdjvp` combines `custom_jvp` and `fgrad` to define custom finite difference rules,when used with `pure_callback` it can to make non-tracable code works within `jax` machinary.
 
+<details> <summary> Example </summary>
+
 _This example is based on the comment from `jax` proposed [`JEP`](https://github.com/google/jax/issues/15425)_
 
 For example this code will fail to work with `jax` transformations, becasue it uses `numpy` functions.
 
 ```python
 import numpy as onp
 import jax
@@ -200,109 +395,12 @@
     # manually set step size
     step_size=1e-3,
 )
 @wrap_pure_callback
 def numpy_func(x: onp.ndarray) -> onp.ndarray:
     return onp.power(x, 2)
 
-
 print(numpy_func(1.0))
 # 2.0000048
-
 ```
 
-### **`Array` accepting functions:**
-
-```python
-
-import jax
-
-jax.config.update("jax_enable_x64", True)
-import jax.numpy as jnp
-import numpy.testing as npt
-
-import finitediffx as fdx
-
-
-# lets first define a vector valued function F: R^3 -> R^3
-# F = F1, F2
-# F1 = x^2 + y^3
-# F2 = x^4 + y^3
-# F3 = 0
-# F = [x**2 + y**3, x**4 + y**3, 0]
-
-x, y, z = [jnp.linspace(0, 1, 100)] * 3
-dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
-X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
-F1 = X**2 + Y**3
-F2 = X**4 + Y**3
-F3 = jnp.zeros_like(F1)
-F = jnp.stack([F1, F2, F3], axis=0)
-
-# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
-dF1dx = fdx.difference(F1, axis=0, step_size=dx, accuracy=6, method="central")
-dF1dx_exact = 2 * X
-npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
-
-# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
-dF2dy = fdx.difference(F2, axis=1, step_size=dy, accuracy=6)
-dF2dy_exact = 3 * Y**2
-npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
-
-# ∇.F : the divergence of F
-divF = fdx.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6, method="central")
-divF_exact = 2 * X + 3 * Y**2
-npt.assert_allclose(divF, divF_exact, atol=1e-7)
-
-# ∇F1 : the gradient of F1
-gradF1 = fdx.gradient(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
-gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
-npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
-
-# ΔF1 : laplacian of F1
-lapF1 = fdx.laplacian(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
-lapF1_exact = 2 + 6 * Y
-npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
-
-# ∇xF : the curl of F
-curlF = fdx.curl(F, step_size=(dx, dy, dz), accuracy=6, method="central")
-curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
-npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
-
-# Jacobian of F
-JF = fdx.jacobian(F, accuracy=4, step_size=(dx, dy, dz), method="central")
-JF_exact = jnp.array(
-    [
-        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
-        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
-        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
-# Hessian of F1
-HF1 = fdx.hessian(F1, accuracy=4, step_size=(dx, dy, dz), method="central")
-HF1_exact = jnp.array(
-    [
-        [
-            2 * jnp.ones_like(X),  # ∂2F1/∂x2
-            0 * jnp.ones_like(X),  # ∂2F1/∂xy
-            0 * jnp.ones_like(X),  # ∂2F1/∂xz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂yx
-            6 * Y**2,              # ∂2F1/∂y2
-            0 * jnp.ones_like(X),  # ∂2F1/∂yz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂zx
-            0 * jnp.ones_like(X),  # ∂2F1/∂zy
-            0 * jnp.ones_like(X),  # ∂2F1/∂z2
-        ],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
-
-
-
-```
+</details>
```

### Comparing `FiniteDiffX-0.0.3/README.md` & `FiniteDiffX-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -29,37 +29,207 @@
 - `divergence(array, accuracy, step_size, method, keepdims)`
 - `hessian(array, accuracy, method, step_size)`
 - `laplacian(array, accuracy, method, step_size)`
 - `curl(array, step_size, method, keep_dims)`
 
 **Function transformation:**
 
-- `fgrad`: similar to `jax.grad` but with finite difference approximation.
+- `fgrad`, and `value_and_fgrad` : similar to `jax.grad` and `jax.value_and_grad` but with finite difference approximation.
 - `define_fdjvp`: define `custom_jvp` rules using finite difference approximation (see example below).
 
 ## 🛠️ Installation<a id="installation"></a>
 
 ```python
 pip install FiniteDiffX
 ```
 
 **Install development version**
 
 ```python
 pip install git+https://github.com/ASEM000/FiniteDiffX
 ```
 
+**If you find it useful to you, consider giving it a star! 🌟**
+
+<br>
+
 ## ⏩ Examples<a id="examples"></a>
 
+### **`Array` accepting functions:**
+
+```python
+
+import jax
+jax.config.update("jax_enable_x64", True)
+import jax.numpy as jnp
+import numpy.testing as npt
+
+import finitediffx as fdx
+
+# lets first define a vector valued function F: R^3 -> R^3
+# F = F1, F2
+# F1 = x^2 + y^3
+# F2 = x^4 + y^3
+# F3 = 0
+# F = [x**2 + y**3, x**4 + y**3, 0]
+
+x, y, z = [jnp.linspace(0, 1, 100)] * 3
+dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
+X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
+F1 = X**2 + Y**3
+F2 = X**4 + Y**3
+F3 = jnp.zeros_like(F1)
+F = jnp.stack([F1, F2, F3], axis=0)
+
+```
+
+<details>
+
+<summary>Difference</summary>
+
+```python
+
+# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
+dF1dx = fdx.difference(F1, axis=0, step_size=dx, accuracy=6, method="central")
+dF1dx_exact = 2 * X
+npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
+
+# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
+dF2dy = fdx.difference(F2, axis=1, step_size=dy, accuracy=6)
+dF2dy_exact = 3 * Y**2
+npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Divergence</summary>
+
+```python
+
+# ∇.F : the divergence of F
+divF = fdx.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6, method="central")
+divF_exact = 2 * X + 3 * Y**2
+npt.assert_allclose(divF, divF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Gradient</summary>
+
+```python
+
+# ∇F1 : the gradient of F1
+gradF1 = fdx.gradient(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
+gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
+npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Laplacian</summary>
+
+```python
+
+# ΔF1 : laplacian of F1
+lapF1 = fdx.laplacian(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
+lapF1_exact = 2 + 6 * Y
+npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Curl</summary>
+
+```python
+
+# ∇xF : the curl of F
+curlF = fdx.curl(F, step_size=(dx, dy, dz), accuracy=6, method="central")
+curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
+npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Jacobian</summary>
+
+```python
+
+# Jacobian of F
+JF = fdx.jacobian(F, accuracy=4, step_size=(dx, dy, dz), method="central")
+JF_exact = jnp.array(
+    [
+        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
+        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
+        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<details>
+
+<summary>Hessian</summary>
+
+```python
+
+# Hessian of F1
+HF1 = fdx.hessian(F1, accuracy=4, step_size=(dx, dy, dz), method="central")
+HF1_exact = jnp.array(
+    [
+        [
+            2 * jnp.ones_like(X),  # ∂2F1/∂x2
+            0 * jnp.ones_like(X),  # ∂2F1/∂xy
+            0 * jnp.ones_like(X),  # ∂2F1/∂xz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂yx
+            6 * Y**2,              # ∂2F1/∂y2
+            0 * jnp.ones_like(X),  # ∂2F1/∂yz
+        ],
+        [
+            0 * jnp.ones_like(X),  # ∂2F1/∂zx
+            0 * jnp.ones_like(X),  # ∂2F1/∂zy
+            0 * jnp.ones_like(X),  # ∂2F1/∂z2
+        ],
+    ]
+)
+npt.assert_allclose(JF, JF_exact, atol=1e-7)
+
+```
+
+</details>
+
+<br><br>
+
 ### **Function transformation:**
 
 **`fgrad`**:
 
 `fgrad` can be used in a similar way to `jax.grad`, however the `fgrad` differentiates a function based on the finite difference rules.
 
+<details> <summary> Example </summary>
+
 ```python
 
 import jax
 from jax import numpy as jnp
 import numpy as onp  # Not jax-traceable
 import finitediffx as fdx
 import functools as ft
@@ -88,18 +258,43 @@
     print(np2_rosenbach2_fdx_style2(1.,2.))
     print(jnp_rosenbach2(1., 2.))
 # 402.0000951997936
 # 402.0000000002219
 # 402.0
 ```
 
+Also works on pytrees
+
+```python
+
+import finitediffx as fdx
+
+params = {"a":1., "b":2., "c":3.}
+
+@fdx.fgrad
+def func(params):
+    return params["a"]**2+params["b"]
+
+func(params)
+# {'a': Array(1.9995117, dtype=float32),
+#  'b': Array(0.9995117, dtype=float32),
+#  'c': Array(0., dtype=float32)}
+
+```
+
+</details>
+
+<br>
+
 **`define_fdjvp`**
 
 `define_fdjvp` combines `custom_jvp` and `fgrad` to define custom finite difference rules,when used with `pure_callback` it can to make non-tracable code works within `jax` machinary.
 
+<details> <summary> Example </summary>
+
 _This example is based on the comment from `jax` proposed [`JEP`](https://github.com/google/jax/issues/15425)_
 
 For example this code will fail to work with `jax` transformations, becasue it uses `numpy` functions.
 
 ```python
 import numpy as onp
 import jax
@@ -177,109 +372,12 @@
     # manually set step size
     step_size=1e-3,
 )
 @wrap_pure_callback
 def numpy_func(x: onp.ndarray) -> onp.ndarray:
     return onp.power(x, 2)
 
-
 print(numpy_func(1.0))
 # 2.0000048
-
 ```
 
-### **`Array` accepting functions:**
-
-```python
-
-import jax
-
-jax.config.update("jax_enable_x64", True)
-import jax.numpy as jnp
-import numpy.testing as npt
-
-import finitediffx as fdx
-
-
-# lets first define a vector valued function F: R^3 -> R^3
-# F = F1, F2
-# F1 = x^2 + y^3
-# F2 = x^4 + y^3
-# F3 = 0
-# F = [x**2 + y**3, x**4 + y**3, 0]
-
-x, y, z = [jnp.linspace(0, 1, 100)] * 3
-dx, dy, dz = x[1] - x[0], y[1] - y[0], z[1] - z[0]
-X, Y, Z = jnp.meshgrid(x, y, z, indexing="ij")
-F1 = X**2 + Y**3
-F2 = X**4 + Y**3
-F3 = jnp.zeros_like(F1)
-F = jnp.stack([F1, F2, F3], axis=0)
-
-# ∂F1/∂x : differentiate F1 with respect to x (i.e axis=0)
-dF1dx = fdx.difference(F1, axis=0, step_size=dx, accuracy=6, method="central")
-dF1dx_exact = 2 * X
-npt.assert_allclose(dF1dx, dF1dx_exact, atol=1e-7)
-
-# ∂F2/∂y : differentiate F2 with respect to y (i.e axis=1)
-dF2dy = fdx.difference(F2, axis=1, step_size=dy, accuracy=6)
-dF2dy_exact = 3 * Y**2
-npt.assert_allclose(dF2dy, dF2dy_exact, atol=1e-7)
-
-# ∇.F : the divergence of F
-divF = fdx.divergence(F, step_size=(dx, dy, dz), keepdims=False, accuracy=6, method="central")
-divF_exact = 2 * X + 3 * Y**2
-npt.assert_allclose(divF, divF_exact, atol=1e-7)
-
-# ∇F1 : the gradient of F1
-gradF1 = fdx.gradient(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
-gradF1_exact = jnp.stack([2 * X, 3 * Y**2, 0 * X], axis=0)
-npt.assert_allclose(gradF1, gradF1_exact, atol=1e-7)
-
-# ΔF1 : laplacian of F1
-lapF1 = fdx.laplacian(F1, step_size=(dx, dy, dz), accuracy=6, method="central")
-lapF1_exact = 2 + 6 * Y
-npt.assert_allclose(lapF1, lapF1_exact, atol=1e-7)
-
-# ∇xF : the curl of F
-curlF = fdx.curl(F, step_size=(dx, dy, dz), accuracy=6, method="central")
-curlF_exact = jnp.stack([F1 * 0, F1 * 0, 4 * X**3 - 3 * Y**2], axis=0)
-npt.assert_allclose(curlF, curlF_exact, atol=1e-7)
-
-# Jacobian of F
-JF = fdx.jacobian(F, accuracy=4, step_size=(dx, dy, dz), method="central")
-JF_exact = jnp.array(
-    [
-        [2 * X, 3 * Y**2, jnp.zeros_like(X)],
-        [4 * X**3, 3 * Y**2, jnp.zeros_like(X)],
-        [jnp.zeros_like(X), jnp.zeros_like(X), jnp.zeros_like(X)],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
-# Hessian of F1
-HF1 = fdx.hessian(F1, accuracy=4, step_size=(dx, dy, dz), method="central")
-HF1_exact = jnp.array(
-    [
-        [
-            2 * jnp.ones_like(X),  # ∂2F1/∂x2
-            0 * jnp.ones_like(X),  # ∂2F1/∂xy
-            0 * jnp.ones_like(X),  # ∂2F1/∂xz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂yx
-            6 * Y**2,              # ∂2F1/∂y2
-            0 * jnp.ones_like(X),  # ∂2F1/∂yz
-        ],
-        [
-            0 * jnp.ones_like(X),  # ∂2F1/∂zx
-            0 * jnp.ones_like(X),  # ∂2F1/∂zy
-            0 * jnp.ones_like(X),  # ∂2F1/∂z2
-        ],
-    ]
-)
-npt.assert_allclose(JF, JF_exact, atol=1e-7)
-
-
-
-
-```
+</details>
```

### Comparing `FiniteDiffX-0.0.3/finitediffx/__init__.py` & `FiniteDiffX-0.0.4/finitediffx/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ._src.fgrad import Offset, define_fdjvp, fgrad
+from ._src.fgrad import Offset, define_fdjvp, fgrad, value_and_fgrad
 from ._src.finite_diff import (
     curl,
     difference,
     divergence,
     gradient,
     hessian,
     jacobian,
@@ -29,14 +29,15 @@
     "divergence",
     "difference",
     "gradient",
     "jacobian",
     "laplacian",
     "hessian",
     "fgrad",
+    "value_and_fgrad",
     "Offset",
     "define_fdjvp",
     "generate_finitediff_coeffs",
 )
 
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

### Comparing `FiniteDiffX-0.0.3/finitediffx/_src/__init__.py` & `FiniteDiffX-0.0.4/finitediffx/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.3/finitediffx/_src/finite_diff.py` & `FiniteDiffX-0.0.4/finitediffx/_src/finite_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,16 +404,16 @@
     array: jax.Array,
     *,
     accuracy: int | tuple[int, ...] = 1,
     step_size: float | tuple[float, ...] = 1,
     keepdims: bool = True,
     method: MethodKind = "central",
 ) -> jax.Array:
-    """Compute the ∇.F of input array where F is a vector field whose components are the first axis of x
-    and returns a scalar field
+    """Compute the ∇.F of input array where F is a vector field whose components
+    are the first axis of x and returns a scalar field
 
     Args:
         x: input array where the leading axis is the dimension of the vector field
         accuracy: accuracy order of the gradient. Default is 1, can be a tuple for each axis
         step_size: step size. Default is 1, can be a tuple for each axis
         method: the method to use (forward, central, backward). Default is central
         keepdims: whether to keep the leading dimension. Default is True.
@@ -671,16 +671,16 @@
     array: jax.Array,
     *,
     accuracy: int | tuple[int, ...] = 1,
     step_size: float | tuple[float, ...] | jax.Array = 1,
     method: MethodKind = "central",
     keepdims: bool = True,
 ) -> jax.Array:
-    """Compute the ∇×F of input array where F is a vector field whose components are the first axis of x
-    and returns a vector field
+    """Compute the ∇×F of input array where F is a vector field whose components
+    are the first axis of x and returns a vector field
 
     Index notation: εijk dFk/dxj
 
     Args:
         x: input array where the leading axis is the dimension of the vector field
         accuracy: accuracy order of the gradient. Default is 1, can be a tuple for each axis
         step_size: step size. Default is 1, can be a tuple for each axis
```

### Comparing `FiniteDiffX-0.0.3/finitediffx/_src/utils.py` & `FiniteDiffX-0.0.4/finitediffx/_src/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import functools as ft
+import math
 from typing import Any
 
 import jax
 import jax.numpy as jnp
 
 
 def _check_and_return(value: Any, ndim: int, name: str):
@@ -41,19 +42,17 @@
     Args:
         derivative : derivative order
 
     Returns:
         tuple[float | int, ...]: central difference offsets
     """
     if derivative < 1:
-        msg = f"derivative must be >= 1 for forward offset generation, got {derivative}"
-        raise ValueError(msg)
+        raise ValueError(f"{derivative=} <1 for forward offset generation")
     if accuracy < 1:
-        msg = f"accuracy must be >= 2 for forward offset generation, got {accuracy}"
-        raise ValueError(msg)
+        raise ValueError(f"{accuracy=} <1 for forward offset generation")
 
     # ref:https://en.wikipedia.org/wiki/Finite_difference_coefficient
     return tuple(range(0, (derivative + accuracy)))
 
 
 def _generate_central_offsets(
     derivative: int,
@@ -64,19 +63,17 @@
     Args:
         derivative : derivative order
 
     Returns:
         tuple[float | int, ...]: central difference offsets
     """
     if derivative < 1:
-        msg = f"derivative must be >= 1 for central offset generation, got {derivative}"
-        raise ValueError(msg)
+        raise ValueError(f"{derivative=} <1 for central offset generation")
     if accuracy < 2:
-        msg = f"accuracy must be >= 2 for central offset generation, got {accuracy}"
-        raise ValueError(msg)
+        raise ValueError(f"{accuracy=} <2 for central offset generation")
 
     # ref:https://en.wikipedia.org/wiki/Finite_difference_coefficient
     left = -((derivative + accuracy - 1) // 2)
     right = (derivative + accuracy - 1) // 2 + 1
     return tuple(range(left, right))
 
 
@@ -89,24 +86,35 @@
     Args:
         derivative : derivative order
 
     Returns:
         tuple[float | int, ...]: central difference offsets
     """
     if derivative < 1:
-        msg = f"derivative must be >= 1 for back offset generation, got {derivative}"
-        raise ValueError(msg)
+        raise ValueError(f"{derivative=} <1 for back offset generation")
     if accuracy < 1:
-        msg = f"accuracy must be >= 2 for back offset generation, got {accuracy}"
-        raise ValueError(msg)
+        raise ValueError(f"{accuracy=} <1 for back offset generation")
 
     return tuple(range(-(derivative + accuracy - 1), 1))
 
 
 @ft.partial(jax.jit, static_argnums=(1,))
+def _generate_finitediff_coeffs(
+    offsets: tuple[float | int, ...],
+    derivative: int,
+) -> jax.Array:
+    N = len(offsets)
+    A = jnp.repeat(jnp.array(offsets)[None, :], repeats=N, axis=0)
+    A **= jnp.arange(0, N).reshape(-1, 1)
+    index = jnp.arange(N)
+    B = jnp.where(index == derivative, math.factorial(derivative), 0)[:, None]
+
+    return (jnp.linalg.inv(A) @ B).flatten()
+
+
 def generate_finitediff_coeffs(
     offsets: tuple[float | int, ...],
     derivative: int,
 ) -> jax.Array:
     """Generate FD coeffs
 
     Args:
@@ -125,16 +133,11 @@
         >>> # translates to  1*f(x-1) - 2*f(x) + 1*f(x+1)
 
     See:
         https://en.wikipedia.org/wiki/Finite_difference_coefficient
         https://web.media.mit.edu/~crtaylor/calculator.html
     """
 
-    if derivative >= (N := len(offsets)):
+    if derivative >= len(offsets):
         raise ValueError(f"{len(offsets)=} must be larger than {derivative=}.")
 
-    A = jnp.repeat(jnp.array(offsets)[None, :], repeats=N, axis=0)
-    A **= jnp.arange(0, N).reshape(-1, 1)
-    index = jnp.arange(N)
-    factorial = jnp.prod(jnp.arange(1, derivative + 1))
-    B = jnp.where(index == derivative, factorial, 0)[:, None]
-    return (jnp.linalg.inv(A) @ B).flatten()
+    return _generate_finitediff_coeffs(offsets, derivative)
```

### Comparing `FiniteDiffX-0.0.3/setup.py` & `FiniteDiffX-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.3/tests/test_finite_diff.py` & `FiniteDiffX-0.0.4/tests/test_finite_diff.py`

 * *Files identical despite different names*

