# Comparing `tmp/esnpy-0.3.0.tar.gz` & `tmp/esnpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esnpy-0.3.0.tar", last modified: Fri Jan  6 14:21:49 2023, max compression
+gzip compressed data, was "esnpy-0.4.0.tar", last modified: Wed Jun  7 09:57:25 2023, max compression
```

## Comparing `esnpy-0.3.0.tar` & `esnpy-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:21:49.521434 esnpy-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-06 14:21:38.000000 esnpy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-01-06 14:21:49.521434 esnpy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-01-06 14:21:38.000000 esnpy-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:21:49.521434 esnpy-0.3.0/esnpy/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-06 14:21:38.000000 esnpy-0.3.0/esnpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-01-06 14:21:38.000000 esnpy-0.3.0/esnpy/esn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-01-06 14:21:38.000000 esnpy-0.3.0/esnpy/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-01-06 14:21:38.000000 esnpy-0.3.0/esnpy/reservoir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-01-06 14:21:38.000000 esnpy-0.3.0/esnpy/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-01-06 14:21:38.000000 esnpy-0.3.0/esnpy/tune.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-06 14:21:38.000000 esnpy-0.3.0/esnpy/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:21:49.521434 esnpy-0.3.0/esnpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-01-06 14:21:49.000000 esnpy-0.3.0/esnpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-06 14:21:49.000000 esnpy-0.3.0/esnpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 14:21:49.000000 esnpy-0.3.0/esnpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-06 14:21:49.000000 esnpy-0.3.0/esnpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-06 14:21:49.000000 esnpy-0.3.0/esnpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-01-06 14:21:38.000000 esnpy-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 14:21:49.521434 esnpy-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:57:25.327108 esnpy-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-07 09:57:15.000000 esnpy-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-07 09:57:25.327108 esnpy-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-07 09:57:15.000000 esnpy-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:57:25.323108 esnpy-0.4.0/esnpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-07 09:57:15.000000 esnpy-0.4.0/esnpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-07 09:57:15.000000 esnpy-0.4.0/esnpy/esn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-07 09:57:15.000000 esnpy-0.4.0/esnpy/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-07 09:57:15.000000 esnpy-0.4.0/esnpy/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-07 09:57:15.000000 esnpy-0.4.0/esnpy/reservoir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-07 09:57:15.000000 esnpy-0.4.0/esnpy/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-07 09:57:15.000000 esnpy-0.4.0/esnpy/tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 09:57:15.000000 esnpy-0.4.0/esnpy/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:57:25.327108 esnpy-0.4.0/esnpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-07 09:57:25.000000 esnpy-0.4.0/esnpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-07 09:57:25.000000 esnpy-0.4.0/esnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:57:25.000000 esnpy-0.4.0/esnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-07 09:57:25.000000 esnpy-0.4.0/esnpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 09:57:25.000000 esnpy-0.4.0/esnpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-07 09:57:15.000000 esnpy-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:57:25.327108 esnpy-0.4.0/setup.cfg
```

### Comparing `esnpy-0.3.0/LICENSE` & `esnpy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esnpy-0.3.0/PKG-INFO` & `esnpy-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esnpy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Out-of-the-box framework for Echo State Networks
 Author-email: Théo BL <biasutto.t@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,16 @@
 
 `esnpy` is an out-of-the-box framework to experiment around ESN and DeepESN.  
 Models have been implemented in pure NumPy/SciPy, so there is no need for a powerful GPU, or any esoteric requirements. 
 
 Right now, the focus is on batch training, and feedback loops have not been taken into account.  
 But feel free to open a ticket a discuss about anything you need, features you want, or even help !
 
+The documentation for the latest release is available on [the github page](https://nizil.github.io/esnpy).
+
 Note from the author: *`esnpy` is a small projet I initiated during my master intership, and have recently cleaned up. I might keep working on it for fun, but If you want/need a more robust framework, [ReservoirPy](https://github.com/reservoirpy/reservoirpy) might be the one you're searching for ;)*
 
 ## Getting Started
 
 ### Installation
 
 **From PyPI**
@@ -117,27 +119,31 @@
 
 `Initializer` is defined by a `init() -> Matrix` function. 
 `esnpy` provides implementations of initializer for both uniform and gaussian distribution of weights, and for both dense and sparse matrix.
 
 `Tuner` is defined by a `init(matrix : Matrix) -> Matrix` function, which can be used to modify the weights after initialization.
 For example, `esnpy` provides a `SpectralRadiusTuner` to change the spectral radius of a weights matrix.
 
-#### `Trainer`
+#### `Trainer` and `Reader`
 
 `esnpy.train.Trainer` is responsible to create the output weights matrix from the training data and targets.  
-It is defined by a `train(inputs: Matrix, data: Matrix, target: Matrix) -> Matrix` function.
+It is defined by a `train(inputs: Matrix, data: Matrix, target: Matrix) -> Reader` function.
+
+The `Reader` is then responsible for computing the final result from the reservoir activations through `__call__`.
 
-`esnpy` provides a `RidgeTrainer` to compute the output weights using a ridge regression. 
+`esnpy` provides a `RidgeTrainer` to compute the output weights using a ridge regression, and a `SklearnTrainer` (more on this one later). 
 This trainer has three parameters : one float, the regularization parameter's weight `alpha`, and two optionals boolean (default to true) `use_bias` and `use_input` to control if we should use a bias and the input to compute the readout weights.
 
+`SklearnTrainer` is an adapter wrapping scikit-learn model, relying on methods `fit` and `predict`. The feature is still experimental, chaos might ensure. 
+
 ## Code Examples 
 
 Want to see some code in action ? Take a look at the `examples/` directory:
-- `MackeyGlass/` demonstrates how to learn to predict a time series,
-- `TrajectoryClassification/` demonstrates how to learn to classify 2D trajectories.
+- `mackey_glass.py` demonstrates how to learn to predict a time series,
+- `trajectory_classification/` demonstrates how to learn to classify 2D trajectories.
 
 ## Bibliography
 
 Based on:
 - *The "echo state" approach to analysing and training recurrent neural networks* by Herbert Jaeger ([pdf](https://www.ai.rug.nl/minds/uploads/EchoStatesTechRep.pdf)),
 - *A pratical guide to applying Echo State Networks* by Mantas Lukoševičius ([pdf](https://www.ai.rug.nl/minds/uploads/PracticalESN.pdf)),
 - *Design of deep echo state networks* by Claudio Gallicchio and al ([link](https://www.sciencedirect.com/science/article/pii/S0893608018302223)),
```

### Comparing `esnpy-0.3.0/README.md` & `esnpy-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 `esnpy` is an out-of-the-box framework to experiment around ESN and DeepESN.  
 Models have been implemented in pure NumPy/SciPy, so there is no need for a powerful GPU, or any esoteric requirements. 
 
 Right now, the focus is on batch training, and feedback loops have not been taken into account.  
 But feel free to open a ticket a discuss about anything you need, features you want, or even help !
 
+The documentation for the latest release is available on [the github page](https://nizil.github.io/esnpy).
+
 Note from the author: *`esnpy` is a small projet I initiated during my master intership, and have recently cleaned up. I might keep working on it for fun, but If you want/need a more robust framework, [ReservoirPy](https://github.com/reservoirpy/reservoirpy) might be the one you're searching for ;)*
 
 ## Getting Started
 
 ### Installation
 
 **From PyPI**
@@ -75,27 +77,31 @@
 
 `Initializer` is defined by a `init() -> Matrix` function. 
 `esnpy` provides implementations of initializer for both uniform and gaussian distribution of weights, and for both dense and sparse matrix.
 
 `Tuner` is defined by a `init(matrix : Matrix) -> Matrix` function, which can be used to modify the weights after initialization.
 For example, `esnpy` provides a `SpectralRadiusTuner` to change the spectral radius of a weights matrix.
 
-#### `Trainer`
+#### `Trainer` and `Reader`
 
 `esnpy.train.Trainer` is responsible to create the output weights matrix from the training data and targets.  
-It is defined by a `train(inputs: Matrix, data: Matrix, target: Matrix) -> Matrix` function.
+It is defined by a `train(inputs: Matrix, data: Matrix, target: Matrix) -> Reader` function.
+
+The `Reader` is then responsible for computing the final result from the reservoir activations through `__call__`.
 
-`esnpy` provides a `RidgeTrainer` to compute the output weights using a ridge regression. 
+`esnpy` provides a `RidgeTrainer` to compute the output weights using a ridge regression, and a `SklearnTrainer` (more on this one later). 
 This trainer has three parameters : one float, the regularization parameter's weight `alpha`, and two optionals boolean (default to true) `use_bias` and `use_input` to control if we should use a bias and the input to compute the readout weights.
 
+`SklearnTrainer` is an adapter wrapping scikit-learn model, relying on methods `fit` and `predict`. The feature is still experimental, chaos might ensure. 
+
 ## Code Examples 
 
 Want to see some code in action ? Take a look at the `examples/` directory:
-- `MackeyGlass/` demonstrates how to learn to predict a time series,
-- `TrajectoryClassification/` demonstrates how to learn to classify 2D trajectories.
+- `mackey_glass.py` demonstrates how to learn to predict a time series,
+- `trajectory_classification/` demonstrates how to learn to classify 2D trajectories.
 
 ## Bibliography
 
 Based on:
 - *The "echo state" approach to analysing and training recurrent neural networks* by Herbert Jaeger ([pdf](https://www.ai.rug.nl/minds/uploads/EchoStatesTechRep.pdf)),
 - *A pratical guide to applying Echo State Networks* by Mantas Lukoševičius ([pdf](https://www.ai.rug.nl/minds/uploads/PracticalESN.pdf)),
 - *Design of deep echo state networks* by Claudio Gallicchio and al ([link](https://www.sciencedirect.com/science/article/pii/S0893608018302223)),
```

### Comparing `esnpy-0.3.0/esnpy/esn.py` & `esnpy-0.4.0/esnpy/esn.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 __all__ = ["ESN", "DeepESN"]
 
 
 class BaseESN(ABC):
     def __init__(self, trainer: Trainer):
         super().__init__()
         self._trainer = trainer
-        self._Wout = None
+        self._reader = None
 
     @abstractmethod
     def _warmup(self, data: MatrixType):
         pass
 
     @abstractmethod
     def _forward(self, data: MatrixType) -> MatrixType:
         pass
 
     def fit(self, warmup: MatrixType, data: MatrixType, target: MatrixType):
         self._warmup(warmup)
         states = self._forward(data)
-        self._Wout = self._trainer.train(data, states, target)
+        self._reader = self._trainer.train(data, states, target)
 
     def transform(self, data: MatrixType) -> MatrixType:
-        if self._Wout is None:
+        if self._reader is None:
             raise RuntimeError("Don't call transform before fit !")
         states = self._forward(data)
         inputs = []
         if self._trainer.use_bias:
             inputs.append(np.ones((states.shape[0], 1)))
         if self._trainer.use_input:
             inputs.append(data)
         inputs.append(states)
-        return np.hstack(inputs).dot(self._Wout)
+        return self._reader(np.hstack(inputs))
 
 
 class ESN(BaseESN):
     """Echo State Network implementation."""
 
     def __init__(self, reservoir: Reservoir, trainer: Trainer):
         super().__init__(trainer)
```

### Comparing `esnpy-0.3.0/esnpy/init.py` & `esnpy-0.4.0/esnpy/init.py`

 * *Files identical despite different names*

### Comparing `esnpy-0.3.0/esnpy/reservoir.py` & `esnpy-0.4.0/esnpy/reservoir.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             self._Win = tuner.tune(self._Win)
         # init internal weights
         self._W = config.intern_init.init((config.size, config.size))
         for tuner in config.intern_tuners:
             self._W = tuner.tune(self._W)
 
     def __update(self, vector: VectorType) -> MatrixType:
-        update = vector.dot(self._Win) + self._W.dot(self._state)
+        update = vector @ self._Win + self._W @ self._state
         self._state = self._a * self._fn(update) + (1 - self._a) * self._state
         return self._state
 
     def __call__(self, data: MatrixType) -> MatrixType:
         outputs = np.zeros((data.shape[0], self._W.shape[0]))
         for i, vec in enumerate(data):
             if self._input_bias:
```

### Comparing `esnpy-0.3.0/esnpy/train.py` & `esnpy-0.4.0/esnpy/train.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 # -*- coding: utf-8 -*-
 from abc import ABC, abstractmethod
-from .type import MatrixType
 import numpy as np
 from scipy import linalg
+from .type import MatrixType
+from .reader import MatrixReader, SklearnReader
 
-__all__ = ["Trainer", "RidgeTrainer"]
+__all__ = ["Trainer", "RidgeTrainer", "SklearnTrainer"]
 
 
 class Trainer(ABC):
-    @abstractmethod
     def train(
-        self, data: MatrixType, states: MatrixType, target: MatrixType
+        self, inputs: MatrixType, states: MatrixType, target: MatrixType
+    ) -> MatrixType:
+        data = []
+        if self._bias:
+            data.append(np.ones((states.shape[0], 1)))
+        if self._input:
+            data.append(inputs)
+        data.append(states)
+        data = np.hstack(data)
+        return self.compute_readout(data, target)
+
+    @abstractmethod
+    def compute_readout(
+        self, data: MatrixType, target: MatrixType
     ) -> MatrixType:
         pass
 
     @property
     @abstractmethod
     def use_bias(self):
         pass
@@ -36,21 +49,38 @@
     def use_bias(self):
         return self._bias
 
     @property
     def use_input(self):
         return self._input
 
-    def train(
-        self, inputs: MatrixType, states: MatrixType, target: MatrixType
+    def compute_readout(
+        self, data: MatrixType, target: MatrixType
     ) -> MatrixType:
-        data = []
-        if self._bias:
-            data.append(np.ones((states.shape[0], 1)))
-        if self._input:
-            data.append(inputs)
-        data.append(states)
-        data = np.hstack(data)
-        return linalg.solve(
-            np.dot(data.T, data) + self._alpha * np.eye(data.shape[1]),
-            np.dot(data.T, target),
+        return MatrixReader(
+            linalg.solve(
+                data.T @ data + self._alpha * np.eye(data.shape[1]),
+                data.T @ target,
+            )
         )
+
+
+class SklearnTrainer(Trainer):
+    def __init__(self, sklearn_model, use_bias: bool = True, use_input=True):
+        super().__init__()
+        self._model = sklearn_model
+        self._bias = use_bias
+        self._input = use_input
+
+    @property
+    def use_bias(self):
+        return self._bias
+
+    @property
+    def use_input(self):
+        return self._input
+
+    def compute_readout(
+        self, data: MatrixType, target: MatrixType
+    ) -> MatrixType:
+        self._model.fit(data, target)
+        return SklearnReader(self._model)
```

### Comparing `esnpy-0.3.0/esnpy/tune.py` & `esnpy-0.4.0/esnpy/tune.py`

 * *Files identical despite different names*

### Comparing `esnpy-0.3.0/esnpy.egg-info/PKG-INFO` & `esnpy-0.4.0/esnpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esnpy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Out-of-the-box framework for Echo State Networks
 Author-email: Théo BL <biasutto.t@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,16 @@
 
 `esnpy` is an out-of-the-box framework to experiment around ESN and DeepESN.  
 Models have been implemented in pure NumPy/SciPy, so there is no need for a powerful GPU, or any esoteric requirements. 
 
 Right now, the focus is on batch training, and feedback loops have not been taken into account.  
 But feel free to open a ticket a discuss about anything you need, features you want, or even help !
 
+The documentation for the latest release is available on [the github page](https://nizil.github.io/esnpy).
+
 Note from the author: *`esnpy` is a small projet I initiated during my master intership, and have recently cleaned up. I might keep working on it for fun, but If you want/need a more robust framework, [ReservoirPy](https://github.com/reservoirpy/reservoirpy) might be the one you're searching for ;)*
 
 ## Getting Started
 
 ### Installation
 
 **From PyPI**
@@ -117,27 +119,31 @@
 
 `Initializer` is defined by a `init() -> Matrix` function. 
 `esnpy` provides implementations of initializer for both uniform and gaussian distribution of weights, and for both dense and sparse matrix.
 
 `Tuner` is defined by a `init(matrix : Matrix) -> Matrix` function, which can be used to modify the weights after initialization.
 For example, `esnpy` provides a `SpectralRadiusTuner` to change the spectral radius of a weights matrix.
 
-#### `Trainer`
+#### `Trainer` and `Reader`
 
 `esnpy.train.Trainer` is responsible to create the output weights matrix from the training data and targets.  
-It is defined by a `train(inputs: Matrix, data: Matrix, target: Matrix) -> Matrix` function.
+It is defined by a `train(inputs: Matrix, data: Matrix, target: Matrix) -> Reader` function.
+
+The `Reader` is then responsible for computing the final result from the reservoir activations through `__call__`.
 
-`esnpy` provides a `RidgeTrainer` to compute the output weights using a ridge regression. 
+`esnpy` provides a `RidgeTrainer` to compute the output weights using a ridge regression, and a `SklearnTrainer` (more on this one later). 
 This trainer has three parameters : one float, the regularization parameter's weight `alpha`, and two optionals boolean (default to true) `use_bias` and `use_input` to control if we should use a bias and the input to compute the readout weights.
 
+`SklearnTrainer` is an adapter wrapping scikit-learn model, relying on methods `fit` and `predict`. The feature is still experimental, chaos might ensure. 
+
 ## Code Examples 
 
 Want to see some code in action ? Take a look at the `examples/` directory:
-- `MackeyGlass/` demonstrates how to learn to predict a time series,
-- `TrajectoryClassification/` demonstrates how to learn to classify 2D trajectories.
+- `mackey_glass.py` demonstrates how to learn to predict a time series,
+- `trajectory_classification/` demonstrates how to learn to classify 2D trajectories.
 
 ## Bibliography
 
 Based on:
 - *The "echo state" approach to analysing and training recurrent neural networks* by Herbert Jaeger ([pdf](https://www.ai.rug.nl/minds/uploads/EchoStatesTechRep.pdf)),
 - *A pratical guide to applying Echo State Networks* by Mantas Lukoševičius ([pdf](https://www.ai.rug.nl/minds/uploads/PracticalESN.pdf)),
 - *Design of deep echo state networks* by Claudio Gallicchio and al ([link](https://www.sciencedirect.com/science/article/pii/S0893608018302223)),
```

### Comparing `esnpy-0.3.0/pyproject.toml` & `esnpy-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools", "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "esnpy"
-version = "0.3.0"
+version = "0.4.0"
 description = "Out-of-the-box framework for Echo State Networks"
 readme = "README.md"
 authors = [{name = "Théo BL", email = "biasutto.t@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
```

