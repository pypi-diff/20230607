# Comparing `tmp/bayesianbandits-0.3.1.tar.gz` & `tmp/bayesianbandits-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesianbandits-0.3.1.tar", max compression
+gzip compressed data, was "bayesianbandits-0.4.0.tar", max compression
```

## Comparing `bayesianbandits-0.3.1.tar` & `bayesianbandits-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/LICENSE
--rw-r--r--   0        0        0     1093 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/README.md
--rw-r--r--   0        0        0     2740 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/__init__.py
--rw-r--r--   0        0        0     3848 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_arm.py
--rw-r--r--   0        0        0    18314 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_basebandit.py
--rw-r--r--   0        0        0    28409 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_estimators.py
--rw-r--r--   0        0        0     1304 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_np_utils.py
--rw-r--r--   0        0        0     5122 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_policy_decorators.py
--rw-r--r--   0        0        0     2655 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_typing.py
--rw-r--r--   0        0        0      705 2023-06-04 16:59:06.101209 bayesianbandits-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1093 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/README.md
+-rw-r--r--   0        0        0     2740 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/__init__.py
+-rw-r--r--   0        0        0     3660 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_arm.py
+-rw-r--r--   0        0        0    19549 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_basebandit.py
+-rw-r--r--   0        0        0    29470 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_estimators.py
+-rw-r--r--   0        0        0     1304 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_np_utils.py
+-rw-r--r--   0        0        0     5122 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_policy_decorators.py
+-rw-r--r--   0        0        0     2656 2023-06-07 16:57:03.981962 bayesianbandits-0.4.0/bayesianbandits/_typing.py
+-rw-r--r--   0        0        0      705 2023-06-07 16:57:03.989962 bayesianbandits-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.4.0/PKG-INFO
```

### Comparing `bayesianbandits-0.3.1/LICENSE` & `bayesianbandits-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.1/README.md` & `bayesianbandits-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.1/bayesianbandits/__init__.py` & `bayesianbandits-0.4.0/bayesianbandits/__init__.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.1/bayesianbandits/_arm.py` & `bayesianbandits-0.4.0/bayesianbandits/_arm.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     ...         return np.random.normal(size=size)
     ...     def partial_fit(self, X, y):
     ...         pass
     >>> learner = MyLearner()
     >>> arm = Arm("Action taken.", reward_function, learner)
     >>> arm.pull()
     'Action taken.'
-    >>> arm.update(1)
+    >>> arm.update(np.array([[1]]), np.array([1]))
 
     """
 
     def __init__(
         self,
         action_token: Any,
         reward_function: Callable[[ArrayLike], ArrayLike],
@@ -85,29 +85,22 @@
             X_new = np.array([[1]])
         else:
             X_new = np.atleast_2d(X)
 
         return self.reward_function(self.learner.sample(X_new, size))  # type: ignore
 
     @requires_learner
-    def update(self, X: ArrayLike, y: Optional[ArrayLike] = None) -> None:
+    def update(self, X: NDArray[np.float_], y: NDArray[np.float_]) -> None:
         """Update the learner.
 
         If y is None, the data in X is used as the target and X is set to
         a `len(X)` rows of ones.
         """
-
-        if y is None:
-            y_fit = np.atleast_1d(X)
-            X_fit = np.ones_like(y_fit, dtype=np.float64)[:, np.newaxis]
-        else:
-            y_fit, X_fit = np.atleast_1d(y), np.atleast_2d(X)
-
         assert self.learner is not None  # for type checker
-        self.learner.partial_fit(X_fit, y_fit)
+        self.learner.partial_fit(X, y)
 
     @requires_learner
     def decay(
         self,
         X: NDArray[np.float_],
         *,
         decay_rate: Optional[float] = None,
```

### Comparing `bayesianbandits-0.3.1/bayesianbandits/_basebandit.py` & `bayesianbandits-0.4.0/bayesianbandits/_basebandit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from copy import deepcopy
 from dataclasses import Field, dataclass, field
 from functools import cached_property, partial
 from typing import (
     Any,
     Callable,
     ClassVar,
+    Collection,
     Dict,
     MutableMapping,
     Optional,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 import numpy as np
-from numpy.typing import ArrayLike
+from numpy.typing import ArrayLike, NDArray
 from sklearn.base import clone
 from typing_extensions import dataclass_transform
 
+from ._np_utils import groupby_array
 from ._typing import ArmProtocol, BanditProtocol, Learner
 
 
 _B = TypeVar("_B", bound="Bandit")
 
 
 @dataclass_transform(field_specifiers=(Field[Any], field))
@@ -270,15 +272,15 @@
         ...
 
     @overload
     def update(self, X: ArrayLike, y: ArrayLike, /, *, unique_id: Any) -> None:
         ...
 
     def update(
-        self, X: ArrayLike, y: Optional[ArrayLike] = None, /, **kwargs: Dict[str, Any]
+        self, X: ArrayLike, y: Optional[ArrayLike] = None, /, **kwargs: Any
     ) -> None:
         """Update the learner for the last arm pulled.
 
         This method is added to the bandit class by the `bandit` decorator.
 
         Parameters
         ----------
@@ -295,37 +297,61 @@
 
         Options
         -------
         unique_id : Any
             Unique identifier for the pull. Required when the `@delayed_reward`
             decorator is used.
         """
-        if y is None and self._contextual:
-            raise ValueError(
-                "X and y must both be array-likes for a contextual bandit."
-            )
-        elif y is not None and not self._contextual:
-            raise ValueError(
-                "The second argument must be None for a non-contextual bandit."
-                " The first argument to `update` must be the outcome."
-            )
+        if self._contextual:
+            if y is None:
+                raise ValueError(
+                    "X and y must both be array-likes for a contextual bandit."
+                )
+            y_fit, X_fit = np.atleast_1d(y), np.atleast_2d(X)
+        else:
+            if y is not None:
+                raise ValueError(
+                    "The second argument must be None for a non-contextual bandit."
+                    " The first argument to `update` must be the outcome."
+                )
+            y_fit = np.atleast_1d(X)
+            X_fit = np.ones_like(y_fit, dtype=np.float64)[:, np.newaxis]
 
         if self.__class__._delayed_reward is True:
-            unique_id = kwargs.get("unique_id")
+            unique_id: Union[Collection[Any], str, None] = kwargs.get("unique_id", None)
             if unique_id is None:
                 raise ValueError(
                     "The `unique_id` keyword argument is required when the "
                     "`delayed_reward = True`."
                 )
+            # check if `unique_id` is a non-string iterable
+            elif isinstance(unique_id, Collection) and not isinstance(unique_id, str):
+                return self._update_batch(
+                    X_fit, y_fit, cast(Collection[Any], unique_id)
+                )
+
             arm_to_update = self.arms[self.cache.pop(unique_id)]  # type: ignore
 
         else:
             arm_to_update = cast(ArmProtocol, self.last_arm_pulled)
 
-        arm_to_update.update(X, y)
+        arm_to_update.update(X_fit, y_fit)
+
+    def _update_batch(
+        self, X: NDArray[np.float_], y: NDArray[np.float_], unique_ids: Collection[Any]
+    ):
+        # fetch the arms names from the cache
+        assert self.cache is not None  # for the type checker
+        arm_names = np.array(
+            [self.cache.pop(unique_id) for unique_id in unique_ids], dtype=str
+        )
+
+        for X_part, y_part, arms in groupby_array(X, y, arm_names, by=arm_names):
+            arm_name = arms[0]
+            self.arms[arm_name].update(X_part, y_part)
 
     @overload
     def sample(self, X: ArrayLike, /, *, size: int = 1) -> ArrayLike:
         ...
 
     @overload
     def sample(self, /, *, size: int = 1) -> ArrayLike:
@@ -359,19 +385,28 @@
             raise ValueError("X must be None for a non-contextual bandit.")
         # choose an arm, draw a sample, and repeat `size` times
         # TODO: this is not the most efficient way to do this
         # but I can't imagine a situation where this would be a bottleneck.
         return np.array([self.policy(X).sample(X) for _ in range(size)])
 
     @overload
-    def decay(self, /, *, decay_last_arm: bool = True) -> None:
+    def decay(
+        self, /, *, decay_rate: Optional[float] = None, decay_last_arm: bool = True
+    ) -> None:
         ...
 
     @overload
-    def decay(self, X: ArrayLike, /, *, decay_last_arm: bool = True) -> None:
+    def decay(
+        self,
+        X: ArrayLike,
+        /,
+        *,
+        decay_rate: Optional[float] = None,
+        decay_last_arm: bool = True,
+    ) -> None:
         ...
 
     def decay(
         self,
         X: Optional[ArrayLike] = None,
         /,
         *,
```

### Comparing `bayesianbandits-0.3.1/bayesianbandits/_estimators.py` & `bayesianbandits-0.4.0/bayesianbandits/_estimators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 from __future__ import annotations
+
 from collections import defaultdict
-from functools import partial
+from functools import cached_property, partial
 from typing import Any, Dict, Optional, Union, cast
 
 import numpy as np
-from numpy.typing import NDArray, ArrayLike
-from scipy.linalg import solve
-from scipy.stats import dirichlet, gamma, multivariate_normal, multivariate_t
+from numpy.typing import ArrayLike, NDArray
+from scipy.linalg import cholesky, solve
+from scipy.stats import (
+    Covariance,
+    dirichlet,
+    gamma,
+    multivariate_normal,
+    multivariate_t,
+)
+from scipy.stats._multivariate import _squeeze_output
 from sklearn.base import BaseEstimator, ClassifierMixin, RegressorMixin  # type: ignore
-from sklearn.utils.validation import check_array  # type: ignore
-from sklearn.utils.validation import check_X_y  # type: ignore
-from sklearn.utils.validation import NotFittedError, check_is_fitted
+from sklearn.utils.validation import (
+    NotFittedError,
+    check_array,  # type: ignore
+    check_is_fitted,
+    check_X_y,  # type: ignore
+)
 from typing_extensions import Self
 
 from ._np_utils import groupby_array
 
 
 class DirichletClassifier(BaseEstimator, ClassifierMixin):  # type: ignore
     """
@@ -515,23 +526,33 @@
         self._initialize_prior(X)
 
         self._fit_helper(X, y)
 
         return self
 
     def _initialize_prior(self, X: NDArray[Any]) -> None:
-        if isinstance(self.random_state, int):
+        if isinstance(self.random_state, int) or self.random_state is None:
             self.random_state_ = np.random.default_rng(self.random_state)
         else:
             self.random_state_ = self.random_state
 
         self.n_features_ = X.shape[1]
         self.coef_ = np.zeros(self.n_features_)
         self.cov_inv_ = np.eye(self.n_features_) / self.alpha
 
+    @cached_property
+    def cov_(self) -> Covariance:
+        """
+        The covariance matrix of the model.
+        """
+        cov = solve(
+            self.cov_inv_, np.eye(self.n_features_), check_finite=False, assume_a="pos"
+        )
+        return Covariance.from_cholesky(cholesky(cov, lower=True))
+
     def _fit_helper(self, X: NDArray[Any], y: NDArray[Any]):
         # Apply the learning rate to the new data, if there are multiple observations
         # in the batch. This is done to ensure that one-at-a-time updates are
         # equivalent to batch updates.
         if len(X) > 1:
             obs_decays = np.flip(
                 np.power(np.sqrt(self.learning_rate), np.arange(len(X)))
@@ -548,14 +569,17 @@
             cov_inv,
             prior_decay * self.cov_inv_ @ self.coef_ + self.beta * X.T @ y,
             check_finite=False,
             assume_a="pos",
         )
 
         self.cov_inv_ = cov_inv
+        # Delete the cached covariance matrix, since it is no longer valid
+        if hasattr(self, "cov_"):
+            del self.cov_
         self.coef_ = coef
 
     def partial_fit(self, X: NDArray[Any], y: NDArray[Any]):
         """
         Update the model using X as training data and y as target values.
         """
         try:
@@ -592,25 +616,19 @@
         Sample from the model posterior at X.
         """
         try:
             check_is_fitted(self, "coef_")
         except NotFittedError:
             self._initialize_prior(X)
 
-        cov = solve(
-            self.cov_inv_, np.eye(self.n_features_), check_finite=False, assume_a="pos"
-        )
         rv_gen = partial(
             multivariate_normal.rvs, size=size, random_state=self.random_state_
         )
 
-        samples = np.atleast_1d(rv_gen(self.coef_, cov))  # type: ignore
-
-        if self.n_features_ == 1:
-            samples = np.expand_dims(samples, -1)
+        samples = np.atleast_1d(rv_gen(self.coef_, self.cov_))  # type: ignore
 
         return np.atleast_2d(samples @ X.T)  # type: ignore
 
     def decay(self, X: NDArray[Any], *, decay_rate: Optional[float] = None) -> None:
         """
         Decay the prior by a factor of `learning_rate`.
         """
@@ -709,19 +727,19 @@
 
     Furthermore, this model implements a `sample` method for sampling from the
     posterior distribution. Because the variance is unknown, the samples are
     drawn from the marginal posterior distribution of the weights, which is a
     multivariate t distribution.
 
     >>> est.sample(X[[0]], size=5)
-    array([[14.02432731],
-           [14.27002665],
-           [13.76856141],
-           [14.81894146],
-           [14.33232679]])
+    array([[15.01030526],
+           [14.64281737],
+           [15.21457505],
+           [14.1703107 ],
+           [14.57089036]])
 
     """
 
     def __init__(
         self,
         *,
         mu: ArrayLike = 0.0,
@@ -735,15 +753,15 @@
         self.lam = lam
         self.a = a
         self.b = b
         self.learning_rate = learning_rate
         self.random_state = random_state
 
     def _initialize_prior(self, X: NDArray[Any]) -> None:
-        if isinstance(self.random_state, int):
+        if isinstance(self.random_state, int) or self.random_state is None:
             self.random_state_ = np.random.default_rng(self.random_state)
         else:
             self.random_state_ = self.random_state
 
         self.n_features_ = X.shape[1]
         if np.isscalar(self.mu):
             self.coef_ = np.full(self.n_features_, self.mu, dtype=np.float_)
@@ -801,36 +819,60 @@
             y.T @ y
             + prior_decay * self.coef_.T @ self.cov_inv_ @ self.coef_
             - m_n.T @ V_n @ m_n
         )
 
         # Posteriors become priors for the next batch
         self.cov_inv_ = V_n
+        # Delete the cached shape_ property so it is recalculated
+        if hasattr(self, "shape_"):
+            del self.shape_
         self.coef_ = m_n
         self.a_ = a_n
         self.b_ = b_n
 
+    @cached_property
+    def shape_(self) -> Covariance:
+        extra_var = self.b_ / self.a_ * np.eye(self.n_features_)
+        shape = solve(self.cov_inv_, extra_var, check_finite=False, assume_a="pos")
+        return Covariance.from_cholesky(cholesky(shape, lower=True))
+
     def sample(self, X: NDArray[Any], size: int = 1) -> NDArray[np.float64]:
         """
         Sample from the coefficient marginal posterior at X. This is equivalent to
         sampling from a multivariate t distribution with the posterior mean and
         covariance, and degrees of freedom equal to 2 * a.
         """
         try:
             check_is_fitted(self, "coef_")
         except NotFittedError:
             self._initialize_prior(X)
 
-        extra_var = self.b_ / self.a_ * np.eye(self.n_features_)
-        shape = solve(self.cov_inv_, extra_var, check_finite=False, assume_a="pos")
-
         df = 2 * self.a_
-        rv_gen = partial(multivariate_t.rvs, size=size, random_state=self.random_state_)
 
-        samples = np.atleast_1d(rv_gen(self.coef_, shape, df))  # type: ignore
+        # Reimplement multivariate_t.rvs because scipy doesn't support
+        # Covariance objects
+
+        dim, loc, _, df = multivariate_t._process_parameters(
+            self.coef_, self.shape_.covariance, df
+        )
+
+        x = self.random_state_.chisquare(df, size=size) / df
+
+        z = multivariate_normal.rvs(
+            np.zeros(dim),
+            self.shape_,
+            size=size,
+            random_state=self.random_state_,
+        )
+        samples = loc + z / np.sqrt(x)[..., None]
+        samples = _squeeze_output(samples)
+
+        # End of multivariate_t.rvs implementation
+
         if self.n_features_ == 1:
             samples = np.expand_dims(samples, -1)
 
         return np.atleast_2d(samples @ X.T)  # type: ignore
 
     def decay(self, X: NDArray[Any], *, decay_rate: Optional[float] = None) -> None:
         """
```

### Comparing `bayesianbandits-0.3.1/bayesianbandits/_np_utils.py` & `bayesianbandits-0.4.0/bayesianbandits/_np_utils.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.1/bayesianbandits/_policy_decorators.py` & `bayesianbandits-0.4.0/bayesianbandits/_policy_decorators.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.1/bayesianbandits/_typing.py` & `bayesianbandits-0.4.0/bayesianbandits/_typing.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         ...
 
     def sample(
         self, X: Optional[ArrayLike] = None, size: int = 1
     ) -> NDArray[np.float_]:
         ...
 
-    def update(self, X: ArrayLike, y: Optional[ArrayLike] = None) -> None:
+    def update(self, X: NDArray[np.float_], y: NDArray[np.float_]) -> None:
         ...
 
     def decay(
         self,
         X: NDArray[np.float_],
         *,
         decay_rate: Optional[float] = None,
```

### Comparing `bayesianbandits-0.3.1/pyproject.toml` & `bayesianbandits-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bayesianbandits"
-version = "0.3.1"
+version = "0.4.0"
 description = ""
 authors = ["Rishi Kulkarni <rishi@kulkarni.science>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
 scipy = "^1.10.0"
```

### Comparing `bayesianbandits-0.3.1/PKG-INFO` & `bayesianbandits-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesianbandits
-Version: 0.3.1
+Version: 0.4.0
 Summary: 
 Author: Rishi Kulkarni
 Author-email: rishi@kulkarni.science
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

