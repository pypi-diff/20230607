# Comparing `tmp/hypll-0.0.1.tar.gz` & `tmp/hypll-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypll-0.0.1.tar", last modified: Wed Jun  7 08:17:04 2023, max compression
+gzip compressed data, was "hypll-0.0.2.tar", last modified: Wed Jun  7 12:19:00 2023, max compression
```

## Comparing `hypll-0.0.1.tar` & `hypll-0.0.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.262273 hypll-0.0.1/
--rw-rw-r--   0 max       (1000) max       (1000)     1095 2023-06-07 07:55:44.000000 hypll-0.0.1/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)      147 2023-06-07 08:17:04.262273 hypll-0.0.1/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     1206 2023-06-07 07:56:27.000000 hypll-0.0.1/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.258273 hypll-0.0.1/hypll/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-05-30 15:33:12.000000 hypll-0.0.1/hypll/__init__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.258273 hypll-0.0.1/hypll/manifolds/
--rw-rw-r--   0 max       (1000) max       (1000)       27 2023-06-06 16:15:20.000000 hypll-0.0.1/hypll/manifolds/__init__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.258273 hypll-0.0.1/hypll/manifolds/base/
--rw-rw-r--   0 max       (1000) max       (1000)       31 2023-05-30 15:33:12.000000 hypll-0.0.1/hypll/manifolds/base/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     3198 2023-06-07 07:54:42.000000 hypll-0.0.1/hypll/manifolds/base/manifold.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.258273 hypll-0.0.1/hypll/manifolds/euclidean/
--rw-rw-r--   0 max       (1000) max       (1000)       32 2023-05-30 15:33:12.000000 hypll-0.0.1/hypll/manifolds/euclidean/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     8322 2023-06-07 07:54:40.000000 hypll-0.0.1/hypll/manifolds/euclidean/manifold.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.258273 hypll-0.0.1/hypll/manifolds/poincare_ball/
--rw-rw-r--   0 max       (1000) max       (1000)       68 2023-06-01 15:26:53.000000 hypll-0.0.1/hypll/manifolds/poincare_ball/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     1343 2023-06-01 15:26:53.000000 hypll-0.0.1/hypll/manifolds/poincare_ball/curvature.py
--rw-rw-r--   0 max       (1000) max       (1000)    11930 2023-06-07 08:02:40.000000 hypll-0.0.1/hypll/manifolds/poincare_ball/manifold.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.258273 hypll-0.0.1/hypll/manifolds/poincare_ball/math/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-05-30 15:33:12.000000 hypll-0.0.1/hypll/manifolds/poincare_ball/math/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     5067 2023-05-30 15:33:12.000000 hypll-0.0.1/hypll/manifolds/poincare_ball/math/diffgeom.py
--rw-rw-r--   0 max       (1000) max       (1000)     2383 2023-06-01 15:26:53.000000 hypll-0.0.1/hypll/manifolds/poincare_ball/math/linalg.py
--rw-rw-r--   0 max       (1000) max       (1000)    10548 2023-06-06 16:15:20.000000 hypll-0.0.1/hypll/manifolds/poincare_ball/math/stats.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.258273 hypll-0.0.1/hypll/nn/
--rw-rw-r--   0 max       (1000) max       (1000)      411 2023-06-06 16:15:20.000000 hypll-0.0.1/hypll/nn/__init__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.262273 hypll-0.0.1/hypll/nn/modules/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-05-30 15:33:12.000000 hypll-0.0.1/hypll/nn/modules/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      623 2023-06-07 07:54:37.000000 hypll-0.0.1/hypll/nn/modules/activation.py
--rw-rw-r--   0 max       (1000) max       (1000)     2828 2023-06-07 07:54:36.000000 hypll-0.0.1/hypll/nn/modules/batchnorm.py
--rw-rw-r--   0 max       (1000) max       (1000)     1335 2023-06-07 07:54:22.000000 hypll-0.0.1/hypll/nn/modules/change_manifold.py
--rw-rw-r--   0 max       (1000) max       (1000)      723 2023-06-07 07:54:35.000000 hypll-0.0.1/hypll/nn/modules/container.py
--rw-rw-r--   0 max       (1000) max       (1000)     3483 2023-06-07 07:54:34.000000 hypll-0.0.1/hypll/nn/modules/convolution.py
--rw-rw-r--   0 max       (1000) max       (1000)     1271 2023-06-07 07:54:33.000000 hypll-0.0.1/hypll/nn/modules/embedding.py
--rw-rw-r--   0 max       (1000) max       (1000)      691 2023-06-07 07:54:18.000000 hypll-0.0.1/hypll/nn/modules/flatten.py
--rw-rw-r--   0 max       (1000) max       (1000)     1037 2023-06-07 07:54:31.000000 hypll-0.0.1/hypll/nn/modules/fold.py
--rw-rw-r--   0 max       (1000) max       (1000)     1377 2023-06-07 07:54:30.000000 hypll-0.0.1/hypll/nn/modules/linear.py
--rw-rw-r--   0 max       (1000) max       (1000)     3869 2023-06-07 07:54:29.000000 hypll-0.0.1/hypll/nn/modules/pooling.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.262273 hypll-0.0.1/hypll/optim/
--rw-rw-r--   0 max       (1000) max       (1000)       64 2023-05-30 15:33:12.000000 hypll-0.0.1/hypll/optim/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     6572 2023-06-07 07:54:28.000000 hypll-0.0.1/hypll/optim/adam.py
--rw-rw-r--   0 max       (1000) max       (1000)     5129 2023-06-07 07:54:27.000000 hypll-0.0.1/hypll/optim/sgd.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.262273 hypll-0.0.1/hypll/tensors/
--rw-rw-r--   0 max       (1000) max       (1000)      136 2023-06-05 12:26:01.000000 hypll-0.0.1/hypll/tensors/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     3147 2023-06-07 07:54:26.000000 hypll-0.0.1/hypll/tensors/manifold_parameter.py
--rw-rw-r--   0 max       (1000) max       (1000)     7698 2023-06-07 07:54:25.000000 hypll-0.0.1/hypll/tensors/manifold_tensor.py
--rw-rw-r--   0 max       (1000) max       (1000)     5676 2023-06-07 07:54:24.000000 hypll-0.0.1/hypll/tensors/tangent_tensor.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.262273 hypll-0.0.1/hypll/utils/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-05-30 15:33:12.000000 hypll-0.0.1/hypll/utils/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     1082 2023-06-07 07:54:24.000000 hypll-0.0.1/hypll/utils/layer_utils.py
--rw-rw-r--   0 max       (1000) max       (1000)      149 2023-05-30 15:33:12.000000 hypll-0.0.1/hypll/utils/math.py
--rw-rw-r--   0 max       (1000) max       (1000)     1762 2023-06-07 07:54:23.000000 hypll-0.0.1/hypll/utils/tensor_utils.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.258273 hypll-0.0.1/hypll.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)      147 2023-06-07 08:17:04.000000 hypll-0.0.1/hypll.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     1340 2023-06-07 08:17:04.000000 hypll-0.0.1/hypll.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-07 08:17:04.000000 hypll-0.0.1/hypll.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)       96 2023-06-07 08:17:04.000000 hypll-0.0.1/hypll.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)        6 2023-06-07 08:17:04.000000 hypll-0.0.1/hypll.egg-info/top_level.txt
--rw-rw-r--   0 max       (1000) max       (1000)      519 2023-06-07 07:52:13.000000 hypll-0.0.1/pyproject.toml
--rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-07 08:17:04.262273 hypll-0.0.1/setup.cfg
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 08:17:04.262273 hypll-0.0.1/tests/
--rw-rw-r--   0 max       (1000) max       (1000)     4146 2023-06-07 07:53:27.000000 hypll-0.0.1/tests/test_manifold_tensor.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.781999 hypll-0.0.2/
+-rw-rw-r--   0 max       (1000) max       (1000)     1095 2023-06-07 10:59:16.000000 hypll-0.0.2/LICENSE
+-rw-rw-r--   0 max       (1000) max       (1000)      168 2023-06-07 12:19:00.781999 hypll-0.0.2/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     1206 2023-06-07 10:59:16.000000 hypll-0.0.2/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.777999 hypll-0.0.2/hypll/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/__init__.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.777999 hypll-0.0.2/hypll/manifolds/
+-rw-rw-r--   0 max       (1000) max       (1000)       27 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/__init__.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.777999 hypll-0.0.2/hypll/manifolds/base/
+-rw-rw-r--   0 max       (1000) max       (1000)       31 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/base/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3198 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/base/manifold.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.777999 hypll-0.0.2/hypll/manifolds/euclidean/
+-rw-rw-r--   0 max       (1000) max       (1000)       32 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/euclidean/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     8322 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/euclidean/manifold.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.777999 hypll-0.0.2/hypll/manifolds/poincare_ball/
+-rw-rw-r--   0 max       (1000) max       (1000)       68 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/poincare_ball/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1343 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/poincare_ball/curvature.py
+-rw-rw-r--   0 max       (1000) max       (1000)    11930 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/poincare_ball/manifold.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.777999 hypll-0.0.2/hypll/manifolds/poincare_ball/math/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/poincare_ball/math/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5067 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/poincare_ball/math/diffgeom.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2383 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/poincare_ball/math/linalg.py
+-rw-rw-r--   0 max       (1000) max       (1000)    10548 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/manifolds/poincare_ball/math/stats.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.777999 hypll-0.0.2/hypll/nn/
+-rw-rw-r--   0 max       (1000) max       (1000)      411 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/__init__.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.781999 hypll-0.0.2/hypll/nn/modules/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/modules/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      623 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/modules/activation.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2828 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/modules/batchnorm.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1335 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/modules/change_manifold.py
+-rw-rw-r--   0 max       (1000) max       (1000)      723 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/modules/container.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3483 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/modules/convolution.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1271 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/modules/embedding.py
+-rw-rw-r--   0 max       (1000) max       (1000)      691 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/modules/flatten.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1037 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/modules/fold.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1377 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/modules/linear.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3869 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/nn/modules/pooling.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.781999 hypll-0.0.2/hypll/optim/
+-rw-rw-r--   0 max       (1000) max       (1000)       64 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/optim/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     6572 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/optim/adam.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5129 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/optim/sgd.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.781999 hypll-0.0.2/hypll/tensors/
+-rw-rw-r--   0 max       (1000) max       (1000)      136 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/tensors/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3147 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/tensors/manifold_parameter.py
+-rw-rw-r--   0 max       (1000) max       (1000)     7698 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/tensors/manifold_tensor.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5676 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/tensors/tangent_tensor.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.781999 hypll-0.0.2/hypll/utils/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/utils/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1082 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/utils/layer_utils.py
+-rw-rw-r--   0 max       (1000) max       (1000)      149 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/utils/math.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1762 2023-06-07 10:59:16.000000 hypll-0.0.2/hypll/utils/tensor_utils.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.777999 hypll-0.0.2/hypll.egg-info/
+-rw-rw-r--   0 max       (1000) max       (1000)      168 2023-06-07 12:19:00.000000 hypll-0.0.2/hypll.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     1340 2023-06-07 12:19:00.000000 hypll-0.0.2/hypll.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-07 12:19:00.000000 hypll-0.0.2/hypll.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)      125 2023-06-07 12:19:00.000000 hypll-0.0.2/hypll.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        6 2023-06-07 12:19:00.000000 hypll-0.0.2/hypll.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1000) max       (1000)      565 2023-06-07 12:17:54.000000 hypll-0.0.2/pyproject.toml
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-07 12:19:00.781999 hypll-0.0.2/setup.cfg
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-07 12:19:00.781999 hypll-0.0.2/tests/
+-rw-rw-r--   0 max       (1000) max       (1000)     4146 2023-06-07 10:59:16.000000 hypll-0.0.2/tests/test_manifold_tensor.py
```

### Comparing `hypll-0.0.1/LICENSE` & `hypll-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/README.md` & `hypll-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/manifolds/base/manifold.py` & `hypll-0.0.2/hypll/manifolds/base/manifold.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/manifolds/euclidean/manifold.py` & `hypll-0.0.2/hypll/manifolds/euclidean/manifold.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/manifolds/poincare_ball/curvature.py` & `hypll-0.0.2/hypll/manifolds/poincare_ball/curvature.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/manifolds/poincare_ball/manifold.py` & `hypll-0.0.2/hypll/manifolds/poincare_ball/manifold.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/manifolds/poincare_ball/math/diffgeom.py` & `hypll-0.0.2/hypll/manifolds/poincare_ball/math/diffgeom.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/manifolds/poincare_ball/math/linalg.py` & `hypll-0.0.2/hypll/manifolds/poincare_ball/math/linalg.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/manifolds/poincare_ball/math/stats.py` & `hypll-0.0.2/hypll/manifolds/poincare_ball/math/stats.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/nn/modules/activation.py` & `hypll-0.0.2/hypll/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/nn/modules/batchnorm.py` & `hypll-0.0.2/hypll/nn/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/nn/modules/change_manifold.py` & `hypll-0.0.2/hypll/nn/modules/change_manifold.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/nn/modules/container.py` & `hypll-0.0.2/hypll/nn/modules/container.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/nn/modules/convolution.py` & `hypll-0.0.2/hypll/nn/modules/convolution.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/nn/modules/embedding.py` & `hypll-0.0.2/hypll/nn/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/nn/modules/flatten.py` & `hypll-0.0.2/hypll/nn/modules/flatten.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/nn/modules/fold.py` & `hypll-0.0.2/hypll/nn/modules/fold.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/nn/modules/linear.py` & `hypll-0.0.2/hypll/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/nn/modules/pooling.py` & `hypll-0.0.2/hypll/nn/modules/pooling.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/optim/adam.py` & `hypll-0.0.2/hypll/optim/adam.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/optim/sgd.py` & `hypll-0.0.2/hypll/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/tensors/manifold_parameter.py` & `hypll-0.0.2/hypll/tensors/manifold_parameter.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/tensors/manifold_tensor.py` & `hypll-0.0.2/hypll/tensors/manifold_tensor.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/tensors/tangent_tensor.py` & `hypll-0.0.2/hypll/tensors/tangent_tensor.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/utils/layer_utils.py` & `hypll-0.0.2/hypll/utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll/utils/tensor_utils.py` & `hypll-0.0.2/hypll/utils/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/hypll.egg-info/SOURCES.txt` & `hypll-0.0.2/hypll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypll-0.0.1/pyproject.toml` & `hypll-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hypll"
 description = "A framework for hyperbolic learning in PyTorch"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
     "torch",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
@@ -17,14 +17,18 @@
     "pytest",
     "pytest_mock",
     "sphinx",
     "sphinx-copybutton",
     "sphinx-gallery",
     "sphinx-tabs",
 ]
+docs = [
+    "networkx",
+    "torchvision",
+]
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 profile = "black"
```

### Comparing `hypll-0.0.1/tests/test_manifold_tensor.py` & `hypll-0.0.2/tests/test_manifold_tensor.py`

 * *Files identical despite different names*

