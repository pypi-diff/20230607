# Comparing `tmp/synapticflow-0.0.6.tar.gz` & `tmp/synapticflow-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapticflow-0.0.6.tar", max compression
+gzip compressed data, was "synapticflow-0.0.7.tar", max compression
```

## Comparing `synapticflow-0.0.6.tar` & `synapticflow-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.6/LICENSE
--rw-r--r--   0        0        0     3224 2023-05-23 10:23:44.455127 synapticflow-0.0.6/README.md
--rw-r--r--   0        0        0     1202 2023-06-06 13:34:52.821642 synapticflow-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      320 2023-06-06 13:34:55.576371 synapticflow-0.0.6/synapticflow/__init__.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.512954 synapticflow-0.0.6/synapticflow/decision/__init__.py
--rw-r--r--   0        0        0     1464 2023-05-18 16:57:01.513061 synapticflow-0.0.6/synapticflow/decision/decision.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.513202 synapticflow-0.0.6/synapticflow/encoding/__init__.py
--rw-r--r--   0        0        0    10258 2023-05-23 10:23:44.456505 synapticflow-0.0.6/synapticflow/encoding/encoders.py
--rw-r--r--   0        0        0       51 2023-05-18 16:57:01.513461 synapticflow-0.0.6/synapticflow/learning/__init__.py
--rw-r--r--   0        0        0    26577 2023-06-03 21:23:56.780325 synapticflow-0.0.6/synapticflow/learning/learning_rules.py
--rw-r--r--   0        0        0     1252 2023-05-18 16:57:01.513703 synapticflow-0.0.6/synapticflow/learning/rewards.py
--rw-r--r--   0        0        0      102 2023-05-18 16:57:01.513880 synapticflow-0.0.6/synapticflow/network/__init__.py
--rw-r--r--   0        0        0    13001 2023-05-23 17:43:23.832730 synapticflow-0.0.6/synapticflow/network/connections.py
--rw-r--r--   0        0        0     4766 2023-05-18 16:57:01.514217 synapticflow-0.0.6/synapticflow/network/monitors.py
--rw-r--r--   0        0        0     7874 2023-05-18 16:57:01.514367 synapticflow-0.0.6/synapticflow/network/network.py
--rw-r--r--   0        0        0    87912 2023-05-23 10:23:44.458566 synapticflow-0.0.6/synapticflow/network/neural_populations.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.515139 synapticflow-0.0.6/synapticflow/plotting/__init__.py
--rw-r--r--   0        0        0      463 2023-05-18 16:57:01.515777 synapticflow-0.0.6/synapticflow/plotting/plotting.py
--rw-r--r--   0        0        0    16715 2023-05-23 10:23:44.459154 synapticflow-0.0.6/synapticflow/plotting/visualization.py
--rw-r--r--   0        0        0       19 2023-05-23 10:23:44.459454 synapticflow-0.0.6/synapticflow/synapticflow.py
--rw-r--r--   0        0        0      303 2023-05-18 16:57:01.515915 synapticflow-0.0.6/synapticflow/utils.py
--rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 synapticflow-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3224 2023-05-23 10:23:44.455127 synapticflow-0.0.7/README.md
+-rw-r--r--   0        0        0     1202 2023-06-07 14:47:17.865118 synapticflow-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      320 2023-06-07 14:47:24.782225 synapticflow-0.0.7/synapticflow/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.512954 synapticflow-0.0.7/synapticflow/decision/__init__.py
+-rw-r--r--   0        0        0     1464 2023-05-18 16:57:01.513061 synapticflow-0.0.7/synapticflow/decision/decision.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.513202 synapticflow-0.0.7/synapticflow/encoding/__init__.py
+-rw-r--r--   0        0        0    10258 2023-05-23 10:23:44.456505 synapticflow-0.0.7/synapticflow/encoding/encoders.py
+-rw-r--r--   0        0        0       51 2023-05-18 16:57:01.513461 synapticflow-0.0.7/synapticflow/learning/__init__.py
+-rw-r--r--   0        0        0    26654 2023-06-07 09:56:47.129024 synapticflow-0.0.7/synapticflow/learning/learning_rules.py
+-rw-r--r--   0        0        0     1252 2023-05-18 16:57:01.513703 synapticflow-0.0.7/synapticflow/learning/rewards.py
+-rw-r--r--   0        0        0      102 2023-05-18 16:57:01.513880 synapticflow-0.0.7/synapticflow/network/__init__.py
+-rw-r--r--   0        0        0    13078 2023-06-06 19:01:02.280100 synapticflow-0.0.7/synapticflow/network/connections.py
+-rw-r--r--   0        0        0     4766 2023-05-18 16:57:01.514217 synapticflow-0.0.7/synapticflow/network/monitors.py
+-rw-r--r--   0        0        0     7874 2023-05-18 16:57:01.514367 synapticflow-0.0.7/synapticflow/network/network.py
+-rw-r--r--   0        0        0    87912 2023-05-23 10:23:44.458566 synapticflow-0.0.7/synapticflow/network/neural_populations.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.515139 synapticflow-0.0.7/synapticflow/plotting/__init__.py
+-rw-r--r--   0        0        0      463 2023-05-18 16:57:01.515777 synapticflow-0.0.7/synapticflow/plotting/plotting.py
+-rw-r--r--   0        0        0    16715 2023-05-23 10:23:44.459154 synapticflow-0.0.7/synapticflow/plotting/visualization.py
+-rw-r--r--   0        0        0       19 2023-05-23 10:23:44.459454 synapticflow-0.0.7/synapticflow/synapticflow.py
+-rw-r--r--   0        0        0      303 2023-05-18 16:57:01.515915 synapticflow-0.0.7/synapticflow/utils.py
+-rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 synapticflow-0.0.7/PKG-INFO
```

### Comparing `synapticflow-0.0.6/LICENSE` & `synapticflow-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.6/README.md` & `synapticflow-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.6/pyproject.toml` & `synapticflow-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "synapticflow"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     "Arsham Gholamzadeh Khoee <arsham.gh97@gmail.com>",
     "Mobin Nesari <mobinnesari81@gmail.com>",
     "Mohammad Mehdi Begmaz <mohammadmehdi.begmaz@gmail.com>",
     "Negar Sourati <negarsourati@gmail.com>"
 ]
 maintainers =[
```

### Comparing `synapticflow-0.0.6/synapticflow/decision/decision.py` & `synapticflow-0.0.7/synapticflow/decision/decision.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.6/synapticflow/encoding/encoders.py` & `synapticflow-0.0.7/synapticflow/encoding/encoders.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.6/synapticflow/learning/learning_rules.py` & `synapticflow-0.0.7/synapticflow/learning/learning_rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,27 +41,27 @@
 
     def __init__(
         self,
         connection: AbstractConnection,
         lr: Optional[Union[float, Sequence[float]]] = None,
         weight_decay: float = 0.,
         reduction: Optional[callable] = None,
-        boundry: str = 'hard',
+        boundary: str = 'hard',
         **kwargs
     ) -> None:
         
         assert not isinstance(connection, RandomConnection), 'RandomConnection is not learnable!'
         
         if lr is None:
             lr = [0., 0.]
         elif isinstance(lr, float) or isinstance(lr, int):
             lr = [lr, lr]
 
         self.connection = connection
-        self.boundry = boundry
+        self.boundary = boundary
 
         self.lr = torch.tensor(lr, dtype=torch.float)
 
         self.weight_decay = 1 - weight_decay if weight_decay else 1.
         
         if reduction is None:
             if self.connection.pre.batch_size == 1:
@@ -80,15 +80,15 @@
         None
 
         """
         if self.weight_decay:
             self.connection.w *= self.weight_decay
         if (
             self.connection.w_min != -np.inf or self.connection.w_max != np.inf
-        ) and not isinstance(self, NoOp) and (self.boundry == 'hard'):
+        ) and not isinstance(self, NoOp) and (self.boundary == 'hard'):
             self.connection.w.clamp_(self.connection.w_min,
                                      self.connection.w_max)
         
         if isinstance(self.connection, SparseConnection):
             self.connection.w *= self.connection.sparse_mask
 
 class NoOp(LearningRule):
@@ -146,23 +146,23 @@
 
     def __init__(
         self,
         connection: AbstractConnection,
         lr: Optional[Union[float, Sequence[float]]] = None,
         reduction: Optional[callable] = None,
         weight_decay: float = 0.,
-        boundry: str = 'hard',
+        boundary: str = 'hard',
         **kwargs
     ) -> None:
         super().__init__(
             connection=connection,
             lr=lr,
             reduction=reduction,
             weight_decay=weight_decay,
-            boundry=boundry,
+            boundary=boundary,
             **kwargs
         )
         """
         Consider the additional required parameters and fill the body\
         accordingly.
         """
         assert (self.connection.pre.spike_trace and self.connection.post.spike_trace), "Both pre- and post-synaptic nodes must record spike traces"
@@ -179,15 +179,15 @@
             
         if self.lr[1].any():
             post_s = self.connection.post.s.view(batch_size, -1).unsqueeze(1).float() * self.lr[1]
             pre_traces = self.connection.pre.traces.view(batch_size, -1).unsqueeze(2)
             dw = self.reduction(torch.bmm(pre_traces, post_s), dim=0)
             del pre_traces, post_s
         
-        if self.boundry == 'soft':
+        if self.boundary == 'soft':
             self.connection.w += (dw * ((self.connection.w - self.connection.w_min) * (self.connection.w_max - self.connection.w) / (self.connection.w_max - self.connection.w_min)))
         else:
             self.connection.w += dw
 
         super().update()
 
         """
@@ -205,24 +205,24 @@
 
     def __init__(
         self,
         connection: AbstractConnection,
         lr: Optional[Union[float, Sequence[float]]] = None,
         reduction: Optional[callable] = None,
         weight_decay: float = 0.,
-        boundry: str = 'hard',
+        boundary: str = 'hard',
         window_steps: int = 10,
         **kwargs
     ) -> None:
         super().__init__(
             connection=connection,
             lr=lr,
             reduction=reduction,
             weight_decay=weight_decay,
-            boundry=boundry,
+            boundary=boundary,
             **kwargs
         )
         self.window_steps = window_steps
         self.pre_traces = torch.zeros(window_steps, *connection.pre.shape)
         self.post_traces = torch.zeros(window_steps, *connection.post.shape)
         self.pre_traces_i = 0
         self.post_traces_i = 0
@@ -252,15 +252,15 @@
         
         print(self.post_traces_i)
         print(self.post_traces)
         print(post_traces_sum)
        
         dw = self.connection.pre.dt * (-self.lr[0] * post_traces_sum.view(*self.connection.post.shape, 1).matmul(self.connection.pre.s.float().view(1, *self.connection.pre.shape)).T + self.lr[1] * pre_traces_sum.view(*self.connection.pre.shape, 1).matmul(self.connection.post.s.float().view(1, *self.connection.post.shape)))
         
-        if self.boundry == 'soft':
+        if self.boundary == 'soft':
             self.connection.w += (dw * ((self.connection.w - self.connection.w_min) * (self.connection.w_max - self.connection.w) / (self.connection.w_max - self.connection.w_min)))
         else:
             self.connection.w += dw
 
         """
 
         Implement the dynamics and updating rule. You might need to call the\
@@ -272,23 +272,23 @@
 class MSTDP(LearningRule):
     def __init__(
         self,
         connection: AbstractConnection,
         lr: Optional[Union[float, Sequence[float]]] = None,
         reduction: Optional[callable] = None,
         weight_decay: float = 0.,
-        boundry: str = 'hard',
+        boundary: str = 'hard',
         **kwargs
     ) -> None:
         super().__init__(
             connection=connection,
             lr=lr,
             reduction=reduction,
             weight_decay=weight_decay,
-            boundry=boundry,
+            boundary=boundary,
             **kwargs
         )
         """
         Consider the additional required parameters and fill the body\
         accordingly.
         """
         self.tc_plus = torch.tensor(kwargs.get("tc_plus", 20.0))
@@ -296,23 +296,23 @@
         
     def update(self, **kwargs) -> None:
         batch_size = self.connection.pre.batch_size
         
         if not hasattr(self, "p_plus"):
             self.p_plus = torch.zeros(
                 batch_size,
-                self.pre.n,
-                device=self.pre.s.device,
+                self.connection.pre.n,
+                device=self.connection.pre.s.device,
             )
         
         if not hasattr(self, "p_minus"):
             self.p_minus = torch.zeros(
                 batch_size,
-                self.post.n,
-                device=self.post.s.device
+                self.connection.post.n,
+                device=self.connection.post.s.device
             )
             
         if not hasattr(self, "eligibility"):
             self.eligibility = torch.zeros(
                 batch_size,
                 *self.connection.w.shape,
                 device=self.connection.w.device
@@ -345,15 +345,15 @@
         self.p_minus *= torch.exp(-self.connection.pre.dt / self.tc_minus)
         self.p_minus += a_minus * post_s
         
         self.eligibility = torch.bmm(
             self.p_plus.unsqueeze(2), post_s.unsqueeze(1)
         ) + torch.bmm(pre_s.unsqueeze(2), self.p_minus.unsqueeze(1))
         
-        if self.boundry == 'soft':
+        if self.boundary == 'soft':
             self.connection.w += (dw * ((self.connection.w - self.connection.w_min) * (self.connection.w_max - self.connection.w) / (self.connection.w_max - self.connection.w_min)))
         else:
             self.connection.w += dw
         
 
 class RSTDP(LearningRule):
     """
@@ -365,24 +365,24 @@
 
     def __init__(
         self,
         connection: AbstractConnection,
         lr: Optional[Union[float, Sequence[float]]] = None,
         reduction: Optional[callable] = None,
         weight_decay: float = 0.,
-        boundry: str = 'hard',
+        boundary: str = 'hard',
         tau_c: Union[float, torch.Tensor] = 0.1,
         **kwargs
     ) -> None:
         super().__init__(
             connection=connection,
             lr=lr,
             reduction=reduction,
             weight_decay=weight_decay,
-            boundry=boundry,
+            boundary=boundary,
             **kwargs
         )
         self.c = torch.zeros(*connection.post.shape,*connection.pre.shape)
         #self.register_buffer("tau_c", torch.tensor(tau_c, dtype=torch.float))
 
         self.tau_c = tau_c
         """
@@ -397,15 +397,15 @@
         dc = (-self.c / self.tau_c) * self.connection.pre.dt + (self.connection.pre.dt * (-self.lr[0] * self.connection.post.traces.view(*self.connection.post.shape, 1).matmul(self.connection.pre.s.view(1, *self.connection.pre.shape).float()) + (self.lr[1] * self.connection.pre.traces.view(*self.connection.pre.shape, 1).matmul(self.connection.post.s.view(1, *self.connection.post.shape).float())).T) * delta)
         self.c += dc
         
         
         dw = self.connection.pre.dt * (self.c * da)
         dw = dw.T
         
-        if self.boundry == 'soft':
+        if self.boundary == 'soft':
             self.connection.w += (dw * ((self.connection.w - self.connection.w_min) * (self.connection.w_max - self.connection.w) / (self.connection.w_max - self.connection.w_min)))
         else:
             self.connection.w += dw
             
         """
 
         Implement the dynamics and updating rule. You might need to call the
@@ -422,15 +422,15 @@
     
     def __init__(
         self,
         connection: AbstractConnection,
         lr: Optional[Union[float, Sequence[float]]] = None,
         reduction: Optional[callable] = None,
         weight_decay: float = 0.,
-        boundry: str = 'hard',
+        boundary: str = 'hard',
         delay_learning: bool = False,
         A_positive: float = 1,
         A_negative: float = 1,
         tau_positive: float = 1,
         tau_negative: float = 1,
         B_positive: float = 1,
         B_negative: float = 1,
@@ -459,15 +459,15 @@
         """
         
         super().__init__(
             connection=connection,
             lr=lr,
             reduction=reduction,
             weight_decay=weight_decay,
-            boundry=boundry
+            boundary=boundary
             **kwargs
         )
         
         self.delay_learning = delay_learning
         self.delay_mem = torch.zeros((self.connection.pre.n, self.connection.post.n), dtype=torch.float32)
         self.A_positive = A_positive
         self.A_negative = A_negative
@@ -490,20 +490,20 @@
         # Checks if any modification should be applied on weights
         delta_w = self.F(delta_time) * (float(delta_time.any()))
         
         # Checks if any modification should be applied on delays
         delta_d = self.G(delta_time) * (float(self.delay_learning))
         
         # Apply modification on weights and delays
-        if self.boundry == 'soft':
+        if self.boundary == 'soft':
             self.connection.w += delta_w * ((self.connection.w - self.connection.w_min) * (self.connection.w_max - self.connection.w) / (self.connection.w_max - self.connection.w_min))
         else:
             self.connection.w += delta_w
             
-        if self.boundry == 'soft':
+        if self.boundary == 'soft':
             self.connection.d += delta_d * ((self.connection.d - self.connection.d_min) * (self.connection.d_max - self.connection.d) / (self.connection.d_max - self.connection.d_min))
         else:
             self.connection.d += delta_d
         
         # Remove old memory
         self.delay_mem.masked_fill_(delta_time != 0, 0)
         
@@ -556,15 +556,15 @@
     
     def __init__(
         self,
         connection: AbstractConnection,
         lr: Optional[Union[float, Sequence[float]]] = None,
         reduction: Optional[callable] = None,
         weight_decay: float = 0.,
-        boundry: str = 'hard',
+        boundary: str = 'hard',
         A_positive: float = 0.2,
         A_negative: float = 0.2,
         tau_positive: float = 0.01,
         tau_negative: float = 0.01,
         **kwargs
     ) -> None:
         
@@ -582,15 +582,15 @@
         tau_negative (float) : Constant for weights changes exponential rate. Default: 1
         """
         
         super().__init__(
             connection=connection,
             lr=lr,
             weight_decay=weight_decay,
-            boundry=boundry,
+            boundary=boundary,
             reduction=reduction,
             **kwargs
         )
         
         self.weight_mem = torch.zeros((self.connection.pre.n, self.connection.post.n), dtype=torch.float32)
         self.A_positive = A_positive
         self.A_negative = A_negative
@@ -607,15 +607,15 @@
         delta_time[delta_time.nonzero(as_tuple=True)] += 1
         delta_w = torch.zeros_like(self.connection.w)
         
         # Checks if any modification should be applied on weights
         delta_w = self.F(delta_time) * (float(delta_time.any()))
         
         # Apply modification on weights and delays
-        if self.boundry == 'soft':
+        if self.boundary == 'soft':
             self.connection.w += delta_w * ((self.connection.w - self.connection.w_min) * (self.connection.w_max - self.connection.w) / (self.connection.w_max - self.connection.w_min))
         else:
             self.connection.w += delta_w
         
         # Remove old memory
         self.weight_mem.masked_fill_(delta_time != 0, 0)
         
@@ -651,23 +651,23 @@
     """
     
     def __init__(self,
                  connection: AbstractConnection, 
                  lr: Optional[Union[float, Sequence[float], Sequence[torch.Tensor]]] = None,
                  reduction: Optional[callable] = None,
                  weight_decay: float = 0.0,
-                 boundry: str = 'hard',
+                 boundary: str = 'hard',
                  **kwargs
                  ) -> None:
         super().__init__(
                          connection=connection,
                          lr=lr,
                          reduction=reduction,
                          weight_decay=weight_decay,
-                         boundry=boundry
+                         boundary=boundary
                          **kwargs)
         
         assert self.connection.pre.spike_trace, "Pre-synaptic population should record spike traces."
         assert (connection.w_min != -np.inf and connection.w_max != np.inf), "Connection should define finite w_min and w_max"
         
         self.w_min = connection.w_min
         self.w_max = connection.w_max
@@ -687,13 +687,13 @@
             outer_product = self.reduction(torch.bmm(pre_s, post_trace), dim=0)
             update -= self.lr[0] * outer_product * (self.connection.w - self.w_min)
             
         if self.lr[1].any():
             outer_product = self.reduction(torch.bmm(pre_trace, post_s), dim=0)
             update += self.lr[1] * outer_product * (self.w_max - self.connection.w)
             
-        if self.boundry == 'soft':
+        if self.boundary == 'soft':
             self.connection.w += update * ((self.connection.w - self.w_min) * (self.w_max - self.connection.w) / (self.connection.w_max - self.connection.w_min))
         else:
             self.connection.w += update
         
         super().update()
```

### Comparing `synapticflow-0.0.6/synapticflow/learning/rewards.py` & `synapticflow-0.0.7/synapticflow/learning/rewards.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.6/synapticflow/network/connections.py` & `synapticflow-0.0.7/synapticflow/network/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from abc import ABC, abstractmethod
 from typing import Union, Sequence
 
 import torch
 from torch.nn import Module, Parameter
+import random
 
 from ..network.neural_populations import NeuralPopulation
 
 import math
 
 
 class AbstractConnection(ABC, torch.nn.Module):
@@ -230,14 +231,15 @@
                          d=d,
                          d_min=d_min,
                          d_max=d_max,
                          mask=mask,
                          **kwargs)
         
         torch.manual_seed(random_seed)
+        random.seed(random_seed)
         if w is None:
             if (self.w_min == float('-inf')) or (self.w_max == float('inf')):
                 w = torch.clamp(torch.rand(pre.n, post.n), self.w_min, self.w_max)
             else:
                 w = self.w_min + torch.rand(pre.n, post.n) * (self.w_max - self.w_min)
         else:
             if (self.w_min != float('-inf')) or (self.w_max != float('inf')):
@@ -258,18 +260,20 @@
         b = kwargs.get("b", None)
         if b is not None:
             print(b)
             self.b = Parameter(b, requires_grad=False)
         else:
             self.b = None
         
-        self.sparse_mask = torch.zeros((self.pre.n, self.post.n))
-        indicesx = torch.randperm(self.pre.n)[:math.ceil((1 - sparsity) * self.pre.n * self.post.n)]
-        indicesy = torch.randperm(self.post.n)[:math.ceil((1 - sparsity) * self.pre.n * self.post.n)]
-        self.sparse_mask[indicesx, indicesy] = 1
+        self.sparse_mask = torch.ones((self.pre.n, self.post.n))
+        indices = [(i, j) for i in range(self.sparse_mask.shape[0]) for j in range(self.sparse_mask.shape[1])]
+        random.shuffle(indices)
+        num_zeros = int(sparsity * self.sparse_mask.numel())
+        for i,j in indices[:num_zeros]:
+            self.sparse_mask[i][j] = 0
         self.w *= self.sparse_mask
     
 
     def reset_state_variables(self) -> None:
         """
         Contains resetting logic for the connection.
         """
```

### Comparing `synapticflow-0.0.6/synapticflow/network/monitors.py` & `synapticflow-0.0.7/synapticflow/network/monitors.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.6/synapticflow/network/network.py` & `synapticflow-0.0.7/synapticflow/network/network.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.6/synapticflow/network/neural_populations.py` & `synapticflow-0.0.7/synapticflow/network/neural_populations.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.6/synapticflow/plotting/visualization.py` & `synapticflow-0.0.7/synapticflow/plotting/visualization.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.6/PKG-INFO` & `synapticflow-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapticflow
-Version: 0.0.6
+Version: 0.0.7
 Summary: A powerful Python package for simulating spiking neural networks (SNNs) using PyTorch with GPU acceleration.
 Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network (SNN)
 Author: Arsham Gholamzadeh Khoee
 Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee
 Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: synapticflow Version: 0.0.6 Summary: A powerful
+Metadata-Version: 2.1 Name: synapticflow Version: 0.0.7 Summary: A powerful
 Python package for simulating spiking neural networks (SNNs) using PyTorch with
 GPU acceleration. Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network
 (SNN) Author: Arsham Gholamzadeh Khoee Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 2 Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
```

