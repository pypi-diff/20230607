# Comparing `tmp/gpflux-0.4.1.tar.gz` & `tmp/gpflux-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpflux-0.4.1.tar", last modified: Tue Mar 28 11:26:17 2023, max compression
+gzip compressed data, was "gpflux-0.4.2.tar", last modified: Wed Jun  7 14:20:24 2023, max compression
```

## Comparing `gpflux-0.4.1.tar` & `gpflux-0.4.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.181062 gpflux-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11354 2023-03-28 11:26:05.000000 gpflux-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-03-28 11:26:17.181062 gpflux-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5295 2023-03-28 11:26:05.000000 gpflux-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.173061 gpflux-0.4.1/gpflux/
--rw-r--r--   0 runner    (1001) docker     (122)      884 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.177062 gpflux-0.4.1/gpflux/architectures/
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6136 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/architectures/constant_input_dim_deep_gp.py
--rw-r--r--   0 runner    (1001) docker     (122)     6351 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.177062 gpflux-0.4.1/gpflux/encoders/
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/encoders/directly_parameterized_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1336 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.177062 gpflux-0.4.1/gpflux/experiment_support/
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/experiment_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/experiment_support/ci_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/experiment_support/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/experiment_support/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (122)    13229 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.177062 gpflux-0.4.1/gpflux/layers/
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.177062 gpflux-0.4.1/gpflux/layers/basis_functions/
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/basis_functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.177062 gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4669 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.177062 gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/quadrature/
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/quadrature/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.181062 gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/random/
--rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11307 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/random/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/random/orthogonal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7928 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/bayesian_dense_layer.py
--rw-r--r--   0 runner    (1001) docker     (122)    16137 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/gp_layer.py
--rw-r--r--   0 runner    (1001) docker     (122)     9526 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/latent_variable_layer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5476 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/likelihood_layer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/layers/trackable_layer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/math.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.181062 gpflux-0.4.1/gpflux/models/
--rw-r--r--   0 runner    (1001) docker     (122)      686 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12385 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/models/deep_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.181062 gpflux-0.4.1/gpflux/optimization/
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10462 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/optimization/keras_natgrad.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     3048 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/runtime_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.181062 gpflux-0.4.1/gpflux/sampling/
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7063 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/sampling/kernel_with_feature_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (122)     7877 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/sampling/sample.py
--rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/sampling/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/types.py
--rw-r--r--   0 runner    (1001) docker     (122)      642 2023-03-28 11:26:05.000000 gpflux-0.4.1/gpflux/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 11:26:17.173061 gpflux-0.4.1/gpflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-03-28 11:26:16.000000 gpflux-0.4.1/gpflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1673 2023-03-28 11:26:16.000000 gpflux-0.4.1/gpflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 11:26:16.000000 gpflux-0.4.1/gpflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-03-28 11:26:16.000000 gpflux-0.4.1/gpflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-28 11:26:16.000000 gpflux-0.4.1/gpflux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-28 11:26:17.181062 gpflux-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-03-28 11:26:05.000000 gpflux-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.201559 gpflux-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11354 2023-06-07 14:20:12.000000 gpflux-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-06-07 14:20:24.201559 gpflux-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5295 2023-06-07 14:20:12.000000 gpflux-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.189559 gpflux-0.4.2/gpflux/
+-rw-r--r--   0 runner    (1001) docker     (122)      884 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.193559 gpflux-0.4.2/gpflux/architectures/
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6136 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/architectures/constant_input_dim_deep_gp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6351 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.193559 gpflux-0.4.2/gpflux/encoders/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/encoders/directly_parameterized_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1336 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.193559 gpflux-0.4.2/gpflux/experiment_support/
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/experiment_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/experiment_support/ci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/experiment_support/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/experiment_support/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13476 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.197559 gpflux-0.4.2/gpflux/layers/
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.197559 gpflux-0.4.2/gpflux/layers/basis_functions/
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/basis_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.197559 gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4669 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.197559 gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/quadrature/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.197559 gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/random/
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11307 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/random/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/random/orthogonal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7928 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/bayesian_dense_layer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16137 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/gp_layer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9526 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/latent_variable_layer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5476 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/likelihood_layer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/layers/trackable_layer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/math.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.197559 gpflux-0.4.2/gpflux/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      686 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12385 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/models/deep_gp.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.201559 gpflux-0.4.2/gpflux/optimization/
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10462 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/optimization/keras_natgrad.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     3048 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/runtime_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.201559 gpflux-0.4.2/gpflux/sampling/
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7063 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/sampling/kernel_with_feature_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7877 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/sampling/sample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/sampling/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-06-07 14:20:12.000000 gpflux-0.4.2/gpflux/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 14:20:24.189559 gpflux-0.4.2/gpflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-06-07 14:20:23.000000 gpflux-0.4.2/gpflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1673 2023-06-07 14:20:23.000000 gpflux-0.4.2/gpflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 14:20:23.000000 gpflux-0.4.2/gpflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-06-07 14:20:23.000000 gpflux-0.4.2/gpflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-07 14:20:23.000000 gpflux-0.4.2/gpflux.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 14:20:24.201559 gpflux-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-06-07 14:20:12.000000 gpflux-0.4.2/setup.py
```

### Comparing `gpflux-0.4.1/LICENSE` & `gpflux-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/PKG-INFO` & `gpflux-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpflux
-Version: 0.4.1
+Version: 0.4.2
 Summary: GPflux: Deep GP library
 Home-page: UNKNOWN
 Author: Secondmind Labs
 Author-email: gpflux@secondmind.ai
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/secondmind-labs/GPflux
 Project-URL: Documentation, https://secondmind-labs.github.io/GPflux/
```

### Comparing `gpflux-0.4.1/README.md` & `gpflux-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/__init__.py` & `gpflux-0.4.2/gpflux/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/architectures/constant_input_dim_deep_gp.py` & `gpflux-0.4.2/gpflux/architectures/constant_input_dim_deep_gp.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/callbacks.py` & `gpflux-0.4.2/gpflux/callbacks.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/encoders/__init__.py` & `gpflux-0.4.2/gpflux/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/encoders/directly_parameterized_encoder.py` & `gpflux-0.4.2/gpflux/encoders/directly_parameterized_encoder.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/exceptions.py` & `gpflux-0.4.2/gpflux/exceptions.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/experiment_support/__init__.py` & `gpflux-0.4.2/gpflux/experiment_support/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/experiment_support/ci_utils.py` & `gpflux-0.4.2/gpflux/experiment_support/ci_utils.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/experiment_support/plotting.py` & `gpflux-0.4.2/gpflux/experiment_support/plotting.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/experiment_support/tensorboard.py` & `gpflux-0.4.2/gpflux/experiment_support/tensorboard.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/helpers.py` & `gpflux-0.4.2/gpflux/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 :class:`~gpflow.inducing_variables.MultioutputInducingVariables`,
 :class:`~gpflow.mean_functions.MeanFunction`, and :class:`~gpflux.layers.GPLayer` objects.
 """
 
 import inspect
 import warnings
 from dataclasses import fields
-from typing import List, Optional, Type, TypeVar, Union
+from typing import List, Optional, Type, TypeVar, Union, Any
 
 import numpy as np
 
 import gpflow
 from gpflow import default_float
 from gpflow.inducing_variables import (
     InducingPoints,
@@ -257,15 +257,18 @@
     )
     return gp_layer
 
 
 T = TypeVar("T")
 
 
-def make_dataclass_from_class(dataclass: Type[T], instance: object, **updates: object) -> T:
+# HACK to get mypy to pass, should be (dataclass: Type[T], ...) -> T:
+# mypy said: gpflux/helpers.py:271: error: Argument 1 to "fields" has incompatible type "Type[T]";
+# expected "Union[DataclassInstance, Type[DataclassInstance]]"  [arg-type]
+def make_dataclass_from_class(dataclass: Any, instance: object, **updates: object) -> Any:
     """
     Take a regular object ``instance`` with a superset of fields for a
     :class:`dataclasses.dataclass` (``@dataclass``-decorated class), and return an
     instance of the dataclass. The ``instance`` has all of the dataclass's fields
     but might also have more. ``key=value`` keyword arguments supersede the fields in ``instance``.
     """
     dataclass_keys = [f.name for f in fields(dataclass)]
```

### Comparing `gpflux-0.4.1/gpflux/layers/__init__.py` & `gpflux-0.4.2/gpflux/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/basis_functions/__init__.py` & `gpflux-0.4.2/gpflux/layers/basis_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/__init__.py` & `gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/base.py` & `gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/base.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/quadrature/__init__.py` & `gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/quadrature/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/quadrature/gaussian.py` & `gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/quadrature/gaussian.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/random/__init__.py` & `gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/random/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/random/base.py` & `gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/random/base.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/random/orthogonal.py` & `gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/random/orthogonal.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/basis_functions/fourier_features/utils.py` & `gpflux-0.4.2/gpflux/layers/basis_functions/fourier_features/utils.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/bayesian_dense_layer.py` & `gpflux-0.4.2/gpflux/layers/bayesian_dense_layer.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/gp_layer.py` & `gpflux-0.4.2/gpflux/layers/gp_layer.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/latent_variable_layer.py` & `gpflux-0.4.2/gpflux/layers/latent_variable_layer.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/likelihood_layer.py` & `gpflux-0.4.2/gpflux/layers/likelihood_layer.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/layers/trackable_layer.py` & `gpflux-0.4.2/gpflux/layers/trackable_layer.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/losses.py` & `gpflux-0.4.2/gpflux/losses.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/math.py` & `gpflux-0.4.2/gpflux/math.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/models/__init__.py` & `gpflux-0.4.2/gpflux/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/models/deep_gp.py` & `gpflux-0.4.2/gpflux/models/deep_gp.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/optimization/__init__.py` & `gpflux-0.4.2/gpflux/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/optimization/keras_natgrad.py` & `gpflux-0.4.2/gpflux/optimization/keras_natgrad.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/runtime_checks.py` & `gpflux-0.4.2/gpflux/runtime_checks.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/sampling/__init__.py` & `gpflux-0.4.2/gpflux/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/sampling/kernel_with_feature_decomposition.py` & `gpflux-0.4.2/gpflux/sampling/kernel_with_feature_decomposition.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/sampling/sample.py` & `gpflux-0.4.2/gpflux/sampling/sample.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/sampling/utils.py` & `gpflux-0.4.2/gpflux/sampling/utils.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/types.py` & `gpflux-0.4.2/gpflux/types.py`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/gpflux/version.py` & `gpflux-0.4.2/gpflux/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Adds __version__"""
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
```

### Comparing `gpflux-0.4.1/gpflux.egg-info/PKG-INFO` & `gpflux-0.4.2/gpflux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpflux
-Version: 0.4.1
+Version: 0.4.2
 Summary: GPflux: Deep GP library
 Home-page: UNKNOWN
 Author: Secondmind Labs
 Author-email: gpflux@secondmind.ai
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/secondmind-labs/GPflux
 Project-URL: Documentation, https://secondmind-labs.github.io/GPflux/
```

### Comparing `gpflux-0.4.1/gpflux.egg-info/SOURCES.txt` & `gpflux-0.4.2/gpflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpflux-0.4.1/setup.py` & `gpflux-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from setuptools import find_namespace_packages, setup
 
 requirements = [
     "deprecated",
     "gpflow>=2.6.3",
     "numpy",
     "scipy",
-    "tensorflow>=2.5.0,<2.12.0; platform_system!='Darwin' or platform_machine!='arm64'",
+    "tensorflow>=2.5.0,<2.13.0; platform_system!='Darwin' or platform_machine!='arm64'",
     # NOTE: Support of Apple Silicon MacOS platforms is in an experimental mode
-    "tensorflow-macos>=2.5.0,<2.12.0; platform_system=='Darwin' and platform_machine=='arm64'",
+    "tensorflow-macos>=2.5.0,<2.13.0; platform_system=='Darwin' and platform_machine=='arm64'",
     # NOTE: once we require tensorflow-probability>=0.12, we can remove our custom deepcopy handling
     "tensorflow-probability>=0.13.0,<0.20.0",
 ]
 
 with open("README.md", "r") as file:
     long_description = file.read()
```

