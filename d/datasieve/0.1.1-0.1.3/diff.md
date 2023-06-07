# Comparing `tmp/datasieve-0.1.1.tar.gz` & `tmp/datasieve-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.1.1.tar", max compression
+gzip compressed data, was "datasieve-0.1.3.tar", max compression
```

## Comparing `datasieve-0.1.1.tar` & `datasieve-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1059 2023-06-06 19:08:39.717257 datasieve-0.1.1/LICENSE
--rw-r--r--   0        0        0    11439 2023-06-06 19:08:39.717257 datasieve-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/__init__.py
--rw-r--r--   0        0        0     7803 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/pipeline.py
--rw-r--r--   0        0        0      563 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0      706 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/base_transform.py
--rw-r--r--   0        0        0     5896 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     3214 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1693 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1553 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/sklearn_wrapper.py
--rw-r--r--   0        0        0     1803 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1550 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     3058 2023-06-06 19:08:39.717257 datasieve-0.1.1/datasieve/utils.py
--rw-r--r--   0        0        0      544 2023-06-06 19:08:39.717257 datasieve-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    12065 1970-01-01 00:00:00.000000 datasieve-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-06-07 16:31:26.108443 datasieve-0.1.3/LICENSE
+-rw-r--r--   0        0        0    11780 2023-06-07 16:31:26.108443 datasieve-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/__init__.py
+-rw-r--r--   0        0        0     8427 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/pipeline.py
+-rw-r--r--   0        0        0      567 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0     3228 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/base_transform.py
+-rw-r--r--   0        0        0     5683 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     2748 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1357 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/noise.py
+-rw-r--r--   0        0        0     1432 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1191 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/sklearn_wrapper.py
+-rw-r--r--   0        0        0     1621 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1453 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     3275 2023-06-07 16:31:26.108443 datasieve-0.1.3/datasieve/utils.py
+-rw-r--r--   0        0        0      544 2023-06-07 16:31:26.112444 datasieve-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    12406 1970-01-01 00:00:00.000000 datasieve-0.1.3/PKG-INFO
```

### Comparing `datasieve-0.1.1/LICENSE` & `datasieve-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.1/README.md` & `datasieve-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,53 +14,53 @@
 - remove feature columns based on arbitrary criteria (e.g. low variance features)
 - change feature column names at certain transformations (e.g. PCA)
 - needing outlier classification without removal (see `oulier_check`)
 - passing dynamic parameters to individual transforms of the pipeline
 - passing dataframes/arrays without worrying about converting to arrays and maintaining the proper feature columns
 - customizing backend for parallelization (e.g. Dask, Ray, loky, etc.)
 
-These improved flexibilities allow for more customized/creative transformations. For example, the included `DataSieveDBSCAN` has automated parameter fitting and outlier removal based on clustering. 
+These improved flexibilities allow for more customized/creative transformations. For example, the included `DBSCAN` has automated parameter fitting and outlier removal based on clustering. 
 
 
 ## Usage
 The user builds the pipeline similarly to SKLearn, and can even use SKLearn transforms directly with the `SKLearnWrapper`:
 
 ```python
     from datasieve.pipeline import Pipeline
-    from datasieve.transforms import DataSieveMinMaxScaler, DataSievePCA, DataSieveVarianceThreshold, SVMOutlierExtractor
-    from datasieve.transforms import SKlearnWrapper
+    import datasieve.transforms as dst
+    from sklearn.preprocessing import MinMaxScaler
 
     feature_pipeline = Pipeline([
-        ("detect_constants", DataSieveVarianceThreshold(threshold=0)),
-        ("pre_svm_scaler", SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1)))),
-        ("svm", SVMOutlierExtractor()),
-        ("pca", DataSievePCA(n_components=0.95)),
-        ("post_pca_scaler", SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1))))
+        ("detect_constants", dst.VarianceThreshold(threshold=0)),
+        ("pre_svm_scaler", dst.SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1)))),
+        ("svm", dst.SVMOutlierExtractor()),
+        ("pca", dst.PCA(n_components=0.95)),
+        ("post_pca_scaler", dst.SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1))))
     ])
 
 ```
 
 Once the pipeline is built, it can be fit and transformed similar to a SKLearn pipeline:
 
 ```python
 X, y, sample_weight = feature_pipeline.fit_transform(X, y, sample_weight)
 ```
 
-This pipeline demonstrates the various components of `DataSieve` which are missing from SKLearn's pipeline. A dataframe `X` (if desired, else users can input a simply array without column names) is input with its associated `y` and `sample_weight` arrays/vectors. The `VarianceThreshold` will first detect and remove any features that have zero variance in X, the `SVMOutlierExtractor` will fit `SGDOneClassSVM` to `X` and then remove the detected outliers in `X`, while also propagating those row removals from `y` and `sample_weight`. Finally, the `PCA` will be fit to the remaining `X` array with the features count changing and getting renamed. The returned `X` dataframe will have the correctly named column features/count, and equal row counts across the `X`, `y`, and `sample_weight` arrays.
+This pipeline demonstrates the various components of `DataSieve` which are missing from SKLearn's pipeline. A dataframe `X` (if desired, else users can input a numpy array without column names) is input with its associated `y` and `sample_weight` arrays/vectors (these are also optional). The `VarianceThreshold` will first detect and remove any features that have zero variance in X, the `SVMOutlierExtractor` will fit `SGDOneClassSVM` to `X` and then remove the detected outliers in `X`, while also propagating those row removals from `y` and `sample_weight`. Finally, the `PCA` will be fit to the remaining `X` array with the features count changing and getting renamed. The returned `X` dataframe will have the correctly named column features/count, and equal row counts across the `X`, `y`, and `sample_weight` arrays.
 
 Next, the `feature_pipeline` can then be used to transform other datasets with the same input feature dimension:
 
 ```python
-X2, _, _ = feature_pipeline.transform(X2)
+Xprime, _, _ = feature_pipeline.transform(X2)
 ```
 
-Finally, similar to SKLearn's pipeline, the `feature_pipeline` can be used to inverse_transform an array `X3` array that has the same dimensions as the returned `X` array from the pipeline:
+Finally, similar to SKLearn's pipeline, the `feature_pipeline` can be used to inverse_transform the array `Xprime` array that has the same dimensions as the returned `X2`/`X` array from the pipeline:
 
 ```python
-Xinv, _ ,_ = feature_pipeline.inverse_transform(X)
+X2, _ ,_ = feature_pipeline.inverse_transform(Xprime)
 ```
 
 
 ## Creating a custom transform
 
 An example would be someone who wants to use `SGDOneClassSVM` to detect and remove outliers from their data set before training:
 
@@ -109,38 +109,51 @@
 ```
 
 
 As shown here, the `fit()` method is actually identical to the SKLearn `fit()` method, but the `transform()` removes data points from X, y, and sample_weight for any outliers detected in the `X` array.
 
 ## Data removal
 
-The command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step's `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `FlowdaptMinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `FlowdaptPipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. 
+The command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step's `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `MinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `Pipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. 
 
 ## Feature modification
 
-Another feature is demonstrated in the `FlowdaptPCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `FlowdaptPipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `FlowdaptVarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `FlowdaptVarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.
+Another feature is demonstrated in the `PCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `Pipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `VarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `VarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.
 
 ## Adding a custom step
 
 Each step of the `Pipeline` *must* contain the following methods:
 
 ```python
-class MyTransformer:
+class MyTransformer(BaseTransform):
     def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        This method is defined by default by the BaseTransform class. But users can override
+        to do something unique (see DBSCAN where this is particularly useful.)
+        """
         X, y, sample_weight = self.fit(X, y, sample_weight)
-        X, y, sample_weight = self.transform(X, y, sample_weight)
-        return X, y, sample_weight, feature_list
+        return self.transform(X, y, sample_weight)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        Some fun fitting method
+        """
         return X, y, sample_weight, feature_list
 
     def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        Transformation of X or y or sample_weight or all three, anything the user
+        wants.
+        """
         return X, y, sample_weight, feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        The inverse transform - it is defined like this by default in BaseTransform class
+        """
         return X, y, sample_weight, feature_list
 ```
 
 This is because these four methods are called automatically by the `Pipeline` object. In most cases, the goal is to add functionality for an existing transformer from the `Scikit-Learn` library. Here is an example of subclassing the `MinMaxScaler` to work with the `FlowdaptPipeline`:
 
 ```python
 class DataSieveMinMaxScaler(MinMaxScaler):
```

### Comparing `datasieve-0.1.1/datasieve/pipeline.py` & `datasieve-0.1.3/datasieve/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from typing import List, Tuple, Dict
 import numpy.typing as npt
 import pandas as pd
 import numpy as np
 import copy
+from datasieve.transforms.base_transform import BaseTransform
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
 class Pipeline:
 
     def __init__(self, steps: List[Tuple] = [],
@@ -35,15 +36,15 @@
     def __getitem__(self, name: str):
         for _, (step_name, step) in enumerate(self.steps):
             if step_name == name:
                 return step
 
         logger.warning(f"Could not find step {name} in pipeline, returning None")
         return None
-    
+
     def append(self, step: Tuple[str, object], fitparams: dict = {}):
         """
         Append a step to the pipeline
         :param step: tuple of (str, transform())
         :param fitparams: dictionary of parameters to pass to fit
         """
         if step[0] in self.step_strings:
@@ -61,14 +62,15 @@
         transformations
         """
         X, y, sample_weight = self._validate_arguments(X, y, sample_weight, fit=True)
         feature_list = copy.deepcopy(self.feature_list)
 
         for _, (name, trans) in enumerate(self.steps):
             logger.debug(f"Fit transforming {name}")
+            self._validate_step(trans)
             X, y, sample_weight, feature_list = trans.fit_transform(
                 X,
                 y,
                 sample_weight=sample_weight,
                 feature_list=feature_list,
                 **self.fitparams[name]
             )
@@ -82,14 +84,15 @@
                                                                                      npt.ArrayLike]:
         X, y, sample_weight = self._validate_arguments(
             X, y, sample_weight, outlier_check=outlier_check)
         feature_list = copy.deepcopy(self.feature_list)
 
         for _, (name, trans) in enumerate(self.steps):
             logger.debug(f"Transforming {name}")
+            self._validate_step(trans)
             X, y, sample_weight, feature_list = trans.transform(
                 X,
                 y,
                 sample_weight=sample_weight,
                 feature_list=feature_list,
                 outlier_check=outlier_check,
                 **self.fitparams[name]
@@ -101,14 +104,15 @@
 
     def fit(self, X, y=None, sample_weight=None):
         X, y, sample_weight = self._validate_arguments(X, y, sample_weight, fit=True)
         feature_list = copy.deepcopy(self.feature_list)
 
         for _, (name, trans) in enumerate(self.steps):
             logger.debug(f"Fitting {name}")
+            self._validate_step(trans)
             X, y, sample_weight, feature_list = trans.fit(
                 X,
                 y,
                 sample_weight=sample_weight,
                 feature_list=feature_list,
                 **self.fitparams[name]
             )
@@ -119,14 +123,15 @@
                                                                         npt.ArrayLike,
                                                                         npt.ArrayLike]:
         X, y, sample_weight = self._validate_arguments(X, y, sample_weight)
         feature_list = copy.deepcopy(self.feature_list)
 
         for _, (name, trans) in reversed(list(enumerate(self.steps))):
             logger.debug(f"Inverse Transforming {name}")
+            self._validate_step(trans)
             X, y, sample_weight, feature_list = trans.inverse_transform(
                 X,
                 y=y,
                 sample_weight=sample_weight,
                 feature_list=feature_list,
                 **self.fitparams[name]
             )
@@ -190,7 +195,20 @@
 
         X = pd.DataFrame(X, columns=feature_list)
 
         if y is not None:
             y = pd.DataFrame(y, columns=self.label_list)
 
         return X, y, sample_weight
+
+    def _validate_step(cls, trans: BaseTransform):
+        """
+        Raise exception if `trans` is not a BaseTransform
+        class
+        """
+        if not isinstance(trans, BaseTransform):
+            raise Exception(
+                f"{trans} is not a BaseTransform class. If you are using"
+                "an SKLearn class, please wrap it inside the SKLearnWrapper()."
+            )
+
+        return
```

### Comparing `datasieve-0.1.1/datasieve/transforms/__init__.py` & `datasieve-0.1.3/datasieve/transforms/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from datasieve.transforms.dissimilarity_index import DissimilarityIndex
 from datasieve.transforms.svm_outlier_extractor import SVMOutlierExtractor
-from datasieve.transforms.pca import DataSievePCA
-from datasieve.transforms.dbscan import DataSieveDBSCAN
-from datasieve.transforms.variance_threshold import DataSieveVarianceThreshold
+from datasieve.transforms.pca import PCA
+from datasieve.transforms.dbscan import DBSCAN
+from datasieve.transforms.variance_threshold import VarianceThreshold
 from datasieve.transforms.sklearn_wrapper import SKLearnWrapper
+from datasieve.transforms.noise import Noise
 
 __all__ = (
     "DissimilarityIndex",
     "SVMOutlierExtractor",
-    "DataSievePCA",
-    "DataSieveDBSCAN",
-    "DataSieveVarianceThreshold",
+    "PCA",
+    "DBSCAN",
+    "Noise",
+    "VarianceThreshold",
     "SKLearnWrapper",
 )
```

### Comparing `datasieve-0.1.1/datasieve/transforms/dbscan.py` & `datasieve-0.1.3/datasieve/transforms/dbscan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import logging
 import numpy as np
 import numpy.typing as npt
 from joblib import parallel_backend
-from sklearn.cluster import DBSCAN
+from sklearn import cluster
 from sklearn.neighbors import NearestNeighbors
 from datasieve.utils import remove_outliers
 from datasieve.transforms.base_transform import BaseTransform
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
-class DataSieveDBSCAN(BaseTransform):
+class DBSCAN(BaseTransform):
     """
-    A subclass of the SKLearn DBSCAN that ensures fit, transform, fit_transform and
+    A custom DBSCAN transform with a fit, transform, fit_transform and
     inverse_transform all take the full set of params X, y, sample_weight (even if they
-    are unused) to follow the FlowdaptPipeline API.
+    are unused) to follow the Pipeline API.
 
     fit() automatically finds the optimal epsilon and min_samples for a set of train_features
     transform() appends datapoints to the train_features, using the same epsilon and
     min_samples as computed in fit, to then determing if any of the appended data points
     are outliers.
     """
 
     def __init__(self, backend="loky", n_jobs=-1, **kwargs) -> None:
-        self._skl: DBSCAN = DBSCAN(**kwargs)
+        self._skl: cluster.DBSCAN = cluster.DBSCAN(**kwargs)
         self.train_features: npt.ArrayLike = np.array([])
         self.backend = backend
         self.n_jobs = n_jobs
 
     def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         self.fit(X, y, sample_weight)
 
@@ -61,16 +61,16 @@
         with parallel_backend(self.backend, n_jobs=self.n_jobs):
             self._skl.fit(X)
 
         self.train_features = X
 
         return X, y, sample_weight, feature_list
 
-    def transform(self, X, y=None, sample_weight=None, feature_list=None,
-                  outlier_check=False, **kwargs):
+    def transform(self, X, y=None, sample_weight=None,
+                  feature_list=None, outlier_check=False, **kwargs):
         """
         Given a data point (or data points), append them to the
         train_features and determine if they are inliers.
         """
 
         num_X = X.shape[0]
         fullX = np.concatenate([self.train_features, X], axis=0)
@@ -90,20 +90,14 @@
             )
         else:
             y += inliers
             y -= 1
 
         return X, y, sample_weight, feature_list
 
-    # def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-    #     """
-    #     Unused
-    #     """
-    #     return X, y, sample_weight, feature_list
-
     def compute_epsilon_and_minpts(self, X):
         """
         Automatically compute the epsilon and min_samples for
         "fitting" the DBSCAN.
         """
         def normalise_distances(distances):
             normalised_distances = (distances - distances.min()) / \
```

### Comparing `datasieve-0.1.1/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.1.3/datasieve/transforms/dissimilarity_index.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,20 +21,14 @@
         self.avg_mean_dist: float = 0
         self.trained_data: npt.ArrayLike = np.array([])
         self.di_threshold = di_threshold
         self.di_values: npt.ArrayLike = np.array([])
         self.n_jobs = n_jobs
         self.backend = backend
 
-    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        self.fit(X, y, sample_weight)
-        X, y, sample_weight, feature_list = self.transform(
-            X, y, sample_weight, feature_list)
-        return X, y, sample_weight, feature_list
-
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         """
         Compute the distances, save the average mean distance
         and save the trained_data array for future use
         """
 
         with parallel_backend(self.backend, n_jobs=self.n_jobs):
@@ -73,13 +67,7 @@
         if num_tossed > 0:
             logger.info(
                 f"DI tossed {num_tossed} predictions for "
                 "being too far from training data."
             )
 
         return X, y, sample_weight, feature_list
-
-    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        Unused
-        """
-        return X, y, sample_weight, feature_list
```

### Comparing `datasieve-0.1.1/datasieve/transforms/pca.py` & `datasieve-0.1.3/datasieve/transforms/pca.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from sklearn.decomposition import PCA
+from sklearn import decomposition
 from datasieve.transforms.base_transform import BaseTransform
 import logging
 import numpy as np
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
-class DataSievePCA(BaseTransform):
+class PCA(BaseTransform):
     """
     A subclass of the SKLearn PCA that ensures fit, transform, fit_transform and
     inverse_transform all take the full set of params X, y, sample_weight (even if they
     are unused) to follow the FlowdaptPipeline API.
     """
 
-    def __init__(self, n_components=0.9999, **kwargs):
-        self._skl = PCA(n_components=n_components, **kwargs)
-
-    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None):
-        X, y, sample_weight, feature_list = self.fit(X, y, sample_weight, feature_list)
-        return self.transform(X, y, sample_weight, feature_list)
+    def __init__(self, **kwargs):
+        self._skl: decomposition.PCA = decomposition.PCA(**kwargs)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         n_components = X.shape[1]
         self._skl.fit(X)
 
         n_keep_components = self._skl.n_components_
         self.feature_list = [f"PC{i}" for i in range(0, n_keep_components)]
```

### Comparing `datasieve-0.1.1/datasieve/transforms/sklearn_wrapper.py` & `datasieve-0.1.3/datasieve/transforms/sklearn_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datasieve.transforms.base_transform import BaseTransform
 from sklearn.base import BaseEstimator
 from joblib import parallel_backend
 
+
 class SKLearnWrapper(BaseTransform):
     """
     Wrapper that takes *most* SKLearn transforms and allows them to
     work wiith the datasieve pipeline
     """
     def __init__(self, sklearninstance: BaseEstimator, n_jobs=-1, backend="loky", **kwargs):
         self.backend = backend
@@ -13,21 +14,16 @@
         self._skl = sklearninstance
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         with parallel_backend(self.backend, n_jobs=self.n_jobs):
             self._skl = self._skl.fit(X, y=y)
         return X, y, sample_weight, feature_list
 
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+    def transform(self, X, y=None, sample_weight=None,
+                  feature_list=None, outlier_check=False, **kwargs):
         with parallel_backend(self.backend, n_jobs=self.n_jobs):
             X = self._skl.transform(X)
         return X, y, sample_weight, feature_list
 
-    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        self.fit(X, y=y, sample_weight=sample_weight, feature_list=feature_list)
-        X, y, sample_weight, feature_list = self.transform(X, y=y, sample_weight=sample_weight,
-                                                           feature_list=feature_list)
-        return X, y, sample_weight, feature_list
-
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         X = self._skl.inverse_transform(X)
         return X, y, sample_weight, feature_list
```

### Comparing `datasieve-0.1.1/datasieve/transforms/svm_outlier_extractor.py` & `datasieve-0.1.3/datasieve/transforms/svm_outlier_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         self.fit(X, y, sample_weight=sample_weight)
         return self.transform(X, y, sample_weight, feature_list)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         self._skl.fit(X, y=y, sample_weight=sample_weight)
         return X, y, sample_weight, feature_list
 
-    def transform(self, X, y=None, sample_weight=None, feature_list=None,
-                  outlier_check=False, **kwargs):
+    def transform(self, X, y=None, sample_weight=None,
+                  feature_list=None, outlier_check=False, **kwargs):
         y_pred = self._skl.predict(X)
         y_pred = np.where(y_pred == -1, 0, y_pred)
         if not outlier_check:
             X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
             num_tossed = len(y_pred) - len(X)
             if num_tossed > 0:
                 logger.info(
@@ -38,13 +38,7 @@
                     "as outliers."
                 )
         else:
             y += y_pred
             y -= 1
 
         return X, y, sample_weight, feature_list
-
-    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        Unused
-        """
-        return X, y, sample_weight, feature_list
```

### Comparing `datasieve-0.1.1/datasieve/transforms/variance_threshold.py` & `datasieve-0.1.3/datasieve/transforms/noise.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-import logging
-import numpy as np
-from sklearn.feature_selection import VarianceThreshold
 from datasieve.transforms.base_transform import BaseTransform
+import numpy as np
 
-logger = logging.getLogger('datasieve.pipeline')
-
-
-class DataSieveVarianceThreshold(BaseTransform):
-
-    def __init__(self, **kwargs) -> None:
-        self._skl: VarianceThreshold = VarianceThreshold(**kwargs)
-        self.feature_list: list = []
-        self.mask = None
 
-    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        self.fit(X, y, sample_weight, feature_list)
-        return self.transform(X, y, sample_weight, feature_list)
+class Noise(BaseTransform):
+    """
+    Add noise to the train features only. Anything that passes through `transform` remains
+    untouched. This makes this step unique in the sense that `fit_transform()` is the
+    only way to apply noise to the train features.
+    """
+    def __init__(self, mu=0, sigma=0.01, **kwargs):
+        self.mu = mu
+        self.sigma = sigma
+        self.noise = np.array([])
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        self._skl.fit(X)
-        self.mask = self._skl.get_support()
-        if feature_list is not None:
-            self.feature_list = np.array(feature_list)[self.mask]
-            logger.info("Variance will remove features "
-                        f"{len(feature_list) - len(self.feature_list)} "
-                        f"on transform. {np.array(feature_list)[~self.mask]}")
-        else:
-            self.feature_list = None
-
-        return X, y, sample_weight, self.feature_list
-
-    def transform(self, X, y=None, sample_weight=None, outlier_check=False, feature_list=None):
-
-        # use mask to filter X array
-        X = X[:, self.mask]
+        """
+        During the fit we do not expect any transformation to occur
+        """
+        self.noise = np.random.normal(self.mu, self.sigma, [X.shape[0], X.shape[1]])
+        return X, y, sample_weight, feature_list
 
-        return X, y, sample_weight, self.feature_list
+    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        We only want the train features to have noise added to them, so during a fit_transform
+        we add noise.
+        """
+        self.fit(X)
+        X += self.noise
+        return X, y, sample_weight, feature_list
 
-    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None):
+    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        We do not add any transformation when this is applied to test features
+        """
         return X, y, sample_weight, feature_list
```

### Comparing `datasieve-0.1.1/datasieve/utils.py` & `datasieve-0.1.3/datasieve/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from joblib import parallel_backend
 import pandas as pd
 from sklearn.metrics import pairwise_distances
 import numpy as np
 import logging
+import numpy.typing as npt
+from typing import Union
 
 logger = logging.getLogger('datasieve.utils')
 
 
-def remove_outliers(X, y=None, sample_weight=None, inliers=None):
+def remove_outliers(X: npt.ArrayLike,
+                    y: Union[npt.ArrayLike, None] = None,
+                    sample_weight: Union[npt.ArrayLike, None] = None,
+                    inliers: Union[npt.ArrayLike, None] = None):
     """
     Utility that takes 3 arrays and the outlier detection
     to remove data points equally across the 3 arrays
     and return them.
 
     :param X: Primary array where outlier points should be removed
     :param y: secondary array that should have the same points as the
```

### Comparing `datasieve-0.1.1/pyproject.toml` & `datasieve-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datasieve"
-version = "0.1.1"
+version = "0.1.3"
 description = "This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)"
 authors = ['Robert Caulk']
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `datasieve-0.1.1/PKG-INFO` & `datasieve-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasieve
-Version: 0.1.1
+Version: 0.1.3
 Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
 License: MIT
 Author: Robert Caulk
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -30,53 +30,53 @@
 - remove feature columns based on arbitrary criteria (e.g. low variance features)
 - change feature column names at certain transformations (e.g. PCA)
 - needing outlier classification without removal (see `oulier_check`)
 - passing dynamic parameters to individual transforms of the pipeline
 - passing dataframes/arrays without worrying about converting to arrays and maintaining the proper feature columns
 - customizing backend for parallelization (e.g. Dask, Ray, loky, etc.)
 
-These improved flexibilities allow for more customized/creative transformations. For example, the included `DataSieveDBSCAN` has automated parameter fitting and outlier removal based on clustering. 
+These improved flexibilities allow for more customized/creative transformations. For example, the included `DBSCAN` has automated parameter fitting and outlier removal based on clustering. 
 
 
 ## Usage
 The user builds the pipeline similarly to SKLearn, and can even use SKLearn transforms directly with the `SKLearnWrapper`:
 
 ```python
     from datasieve.pipeline import Pipeline
-    from datasieve.transforms import DataSieveMinMaxScaler, DataSievePCA, DataSieveVarianceThreshold, SVMOutlierExtractor
-    from datasieve.transforms import SKlearnWrapper
+    import datasieve.transforms as dst
+    from sklearn.preprocessing import MinMaxScaler
 
     feature_pipeline = Pipeline([
-        ("detect_constants", DataSieveVarianceThreshold(threshold=0)),
-        ("pre_svm_scaler", SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1)))),
-        ("svm", SVMOutlierExtractor()),
-        ("pca", DataSievePCA(n_components=0.95)),
-        ("post_pca_scaler", SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1))))
+        ("detect_constants", dst.VarianceThreshold(threshold=0)),
+        ("pre_svm_scaler", dst.SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1)))),
+        ("svm", dst.SVMOutlierExtractor()),
+        ("pca", dst.PCA(n_components=0.95)),
+        ("post_pca_scaler", dst.SKlearnWrapper(MinMaxScaler(feature_range=(-1, 1))))
     ])
 
 ```
 
 Once the pipeline is built, it can be fit and transformed similar to a SKLearn pipeline:
 
 ```python
 X, y, sample_weight = feature_pipeline.fit_transform(X, y, sample_weight)
 ```
 
-This pipeline demonstrates the various components of `DataSieve` which are missing from SKLearn's pipeline. A dataframe `X` (if desired, else users can input a simply array without column names) is input with its associated `y` and `sample_weight` arrays/vectors. The `VarianceThreshold` will first detect and remove any features that have zero variance in X, the `SVMOutlierExtractor` will fit `SGDOneClassSVM` to `X` and then remove the detected outliers in `X`, while also propagating those row removals from `y` and `sample_weight`. Finally, the `PCA` will be fit to the remaining `X` array with the features count changing and getting renamed. The returned `X` dataframe will have the correctly named column features/count, and equal row counts across the `X`, `y`, and `sample_weight` arrays.
+This pipeline demonstrates the various components of `DataSieve` which are missing from SKLearn's pipeline. A dataframe `X` (if desired, else users can input a numpy array without column names) is input with its associated `y` and `sample_weight` arrays/vectors (these are also optional). The `VarianceThreshold` will first detect and remove any features that have zero variance in X, the `SVMOutlierExtractor` will fit `SGDOneClassSVM` to `X` and then remove the detected outliers in `X`, while also propagating those row removals from `y` and `sample_weight`. Finally, the `PCA` will be fit to the remaining `X` array with the features count changing and getting renamed. The returned `X` dataframe will have the correctly named column features/count, and equal row counts across the `X`, `y`, and `sample_weight` arrays.
 
 Next, the `feature_pipeline` can then be used to transform other datasets with the same input feature dimension:
 
 ```python
-X2, _, _ = feature_pipeline.transform(X2)
+Xprime, _, _ = feature_pipeline.transform(X2)
 ```
 
-Finally, similar to SKLearn's pipeline, the `feature_pipeline` can be used to inverse_transform an array `X3` array that has the same dimensions as the returned `X` array from the pipeline:
+Finally, similar to SKLearn's pipeline, the `feature_pipeline` can be used to inverse_transform the array `Xprime` array that has the same dimensions as the returned `X2`/`X` array from the pipeline:
 
 ```python
-Xinv, _ ,_ = feature_pipeline.inverse_transform(X)
+X2, _ ,_ = feature_pipeline.inverse_transform(Xprime)
 ```
 
 
 ## Creating a custom transform
 
 An example would be someone who wants to use `SGDOneClassSVM` to detect and remove outliers from their data set before training:
 
@@ -125,38 +125,51 @@
 ```
 
 
 As shown here, the `fit()` method is actually identical to the SKLearn `fit()` method, but the `transform()` removes data points from X, y, and sample_weight for any outliers detected in the `X` array.
 
 ## Data removal
 
-The command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step's `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `FlowdaptMinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `FlowdaptPipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. 
+The command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step's `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `MinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `Pipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. 
 
 ## Feature modification
 
-Another feature is demonstrated in the `FlowdaptPCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `FlowdaptPipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `FlowdaptVarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `FlowdaptVarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.
+Another feature is demonstrated in the `PCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `Pipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `VarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `VarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.
 
 ## Adding a custom step
 
 Each step of the `Pipeline` *must* contain the following methods:
 
 ```python
-class MyTransformer:
+class MyTransformer(BaseTransform):
     def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        This method is defined by default by the BaseTransform class. But users can override
+        to do something unique (see DBSCAN where this is particularly useful.)
+        """
         X, y, sample_weight = self.fit(X, y, sample_weight)
-        X, y, sample_weight = self.transform(X, y, sample_weight)
-        return X, y, sample_weight, feature_list
+        return self.transform(X, y, sample_weight)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        Some fun fitting method
+        """
         return X, y, sample_weight, feature_list
 
     def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        Transformation of X or y or sample_weight or all three, anything the user
+        wants.
+        """
         return X, y, sample_weight, feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        The inverse transform - it is defined like this by default in BaseTransform class
+        """
         return X, y, sample_weight, feature_list
 ```
 
 This is because these four methods are called automatically by the `Pipeline` object. In most cases, the goal is to add functionality for an existing transformer from the `Scikit-Learn` library. Here is an example of subclassing the `MinMaxScaler` to work with the `FlowdaptPipeline`:
 
 ```python
 class DataSieveMinMaxScaler(MinMaxScaler):
```

