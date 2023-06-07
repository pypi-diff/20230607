# Comparing `tmp/asociita-0.1.8.tar.gz` & `tmp/asociita-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.1.8.tar", max compression
+gzip compressed data, was "asociita-0.1.9.tar", max compression
```

## Comparing `asociita-0.1.8.tar` & `asociita-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.1.8/LICENSE
--rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/__init__.py
--rw-r--r--   0        0        0     3881 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/components/archiver/archive_manager.py
--rw-r--r--   0        0        0     6970 2023-06-05 13:24:07.885952 asociita-0.1.8/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0     9972 2023-06-05 09:45:20.347198 asociita-0.1.8/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0     2106 2023-06-05 13:51:59.255884 asociita-0.1.8/asociita/components/evaluator/sample_evaluator.py
--rw-r--r--   0        0        0     4370 2023-06-06 11:35:25.808272 asociita-0.1.8/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     7549 2023-06-06 11:41:23.091887 asociita-0.1.8/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     6226 2023-06-06 11:42:03.726476 asociita-0.1.8/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    11069 2023-06-06 11:35:25.808272 asociita-0.1.8/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     2635 2023-05-30 14:56:02.584171 asociita-0.1.8/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     2639 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/datasets/load_cifar.py
--rw-r--r--   0        0        0     2612 2023-05-30 14:56:14.419772 asociita-0.1.8/asociita/datasets/load_fmnist.py
--rw-r--r--   0        0        0     2595 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     6766 2023-05-30 09:52:26.729788 asociita-0.1.8/asociita/datasets/shard_splits.py
--rw-r--r--   0        0        0     5962 2023-05-30 10:15:28.967345 asociita-0.1.8/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.1.8/asociita/exceptions/evaluatorexception.py
--rw-r--r--   0        0        0      322 2023-05-29 08:30:33.477904 asociita-0.1.8/asociita/exceptions/settingexception.py
--rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/models/pytorch/cifar10.py
--rw-r--r--   0        0        0    14810 2023-06-06 11:35:25.808272 asociita-0.1.8/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.1.8/asociita/models/pytorch/fmnist.py
--rw-r--r--   0        0        0      934 2023-05-31 13:26:40.943955 asociita-0.1.8/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     5918 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/utils/computations.py
--rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/utils/handlers.py
--rw-r--r--   0        0        0      572 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1904 2023-06-06 11:38:43.941409 asociita-0.1.8/asociita/utils/loggers.py
--rw-r--r--   0        0        0     7791 2023-06-05 13:21:15.847962 asociita-0.1.8/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.1.8/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.1.8/asociita/utils/showcase.py
--rw-r--r--   0        0        0      678 2023-06-06 11:47:43.566664 asociita-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 asociita-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.1.9/asociita/__init__.py
+-rw-r--r--   0        0        0     3881 2023-05-29 08:30:33.477904 asociita-0.1.9/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0     6970 2023-06-05 13:24:07.885952 asociita-0.1.9/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.1.9/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0     9972 2023-06-05 09:45:20.347198 asociita-0.1.9/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0     2106 2023-06-05 13:51:59.255884 asociita-0.1.9/asociita/components/evaluator/sample_evaluator.py
+-rw-r--r--   0        0        0     4370 2023-06-06 11:35:25.808272 asociita-0.1.9/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     7549 2023-06-06 11:41:23.091887 asociita-0.1.9/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     6226 2023-06-06 11:42:03.726476 asociita-0.1.9/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    11069 2023-06-06 11:35:25.808272 asociita-0.1.9/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     3288 2023-06-07 13:08:30.716688 asociita-0.1.9/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     3012 2023-06-07 14:34:09.128863 asociita-0.1.9/asociita/datasets/load_cifar.py
+-rw-r--r--   0        0        0     2973 2023-06-07 14:34:21.476438 asociita-0.1.9/asociita/datasets/load_fmnist.py
+-rw-r--r--   0        0        0     2955 2023-06-07 14:33:17.378645 asociita-0.1.9/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     1314 2023-06-07 14:34:55.775257 asociita-0.1.9/asociita/datasets/save_blueprint.py
+-rw-r--r--   0        0        0     6830 2023-06-07 14:40:50.095085 asociita-0.1.9/asociita/datasets/shard_splits.py
+-rw-r--r--   0        0        0     5962 2023-05-30 10:15:28.967345 asociita-0.1.9/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.1.9/asociita/exceptions/evaluatorexception.py
+-rw-r--r--   0        0        0      322 2023-05-29 08:30:33.477904 asociita-0.1.9/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/models/pytorch/cifar10.py
+-rw-r--r--   0        0        0    14810 2023-06-06 11:35:25.808272 asociita-0.1.9/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.1.9/asociita/models/pytorch/fmnist.py
+-rw-r--r--   0        0        0      934 2023-05-31 13:26:40.943955 asociita-0.1.9/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     5918 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/utils/computations.py
+-rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/utils/handlers.py
+-rw-r--r--   0        0        0      572 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1904 2023-06-06 11:38:43.941409 asociita-0.1.9/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     7791 2023-06-05 13:21:15.847962 asociita-0.1.9/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.1.9/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/utils/showcase.py
+-rw-r--r--   0        0        0      678 2023-06-07 14:46:31.479257 asociita-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 asociita-0.1.9/PKG-INFO
```

### Comparing `asociita-0.1.8/LICENSE` & `asociita-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/README.md` & `asociita-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/components/archiver/archive_manager.py` & `asociita-0.1.9/asociita/components/archiver/archive_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/components/evaluator/evaluation_manager.py` & `asociita-0.1.9/asociita/components/evaluator/evaluation_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.1.9/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/components/evaluator/or_evaluator.py` & `asociita-0.1.9/asociita/components/evaluator/or_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/components/evaluator/sample_evaluator.py` & `asociita-0.1.9/asociita/components/evaluator/sample_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/components/nodes/federated_node.py` & `asociita-0.1.9/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.1.9/asociita/components/orchestrator/evaluator_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/components/orchestrator/fedopt_orchestrator.py` & `asociita-0.1.9/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.1.9/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/datasets/load_cifar.py` & `asociita-0.1.9/asociita/datasets/load_fmnist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import datasets
 from datasets import load_dataset
+from asociita.datasets.shard_transformation import Shard_Transformation
 from asociita.datasets.shard_splits import Shard_Splits
 from asociita.utils.showcase import save_random
 from asociita.utils.handlers import Handler
 import copy
 import pandas as pd
 import numpy as np
 
-def load_cifar(settings: dict) -> list[datasets.arrow_dataset.Dataset,
+def load_fmnist(settings: dict) -> list[datasets.arrow_dataset.Dataset,
                                        list[list[list[datasets.arrow_dataset.Dataset]]]]:
-    """Loads the CIFAR dataset, splits it into the number of shards, pre-process selected
+    """Loads the FMNIST dataset, splits it into the number of shards, pre-process selected
     shards (subsets) and returns in a following format:
     list[   
         "Orchestrator Data"[
             Dataset
             ],   
         "Agents Data"[
             "Agent N"[
@@ -29,32 +30,35 @@
     Args:
         settings (dict) : A dictionary containing all the dataset settings.
     Returns:
         list[datasets.arrow_dataset.Dataset,
                                        list[list[list[datasets.arrow_dataset.Dataset]]]]"""
     
     # Using the 'test' data as a orchestrator validaiton set.
-    orchestrator_data = load_dataset('cifar10', split='test')
+    orchestrator_data = load_dataset('fashion_mnist', split='test')
     # Using the 'train' data as a dataset reserved for agents
-    dataset = load_dataset('cifar10', split='train')
+    dataset = load_dataset('fashion_mnist', split='train')
 
-    orchestrator_data = orchestrator_data.rename_column('img', 'image')
-    dataset = dataset.rename_column('img', 'image')
-
-    # Type: Random Uniform (Sharding) -> Same size, random distribution
-    if settings['split_type'] == 'random_uniform':
-        return [orchestrator_data, Shard_Splits.random_uniform(dataset=dataset, settings=settings)]
+    # Type: Homogeneous Size and Distribution (Sharding) -> Same size, similar distribution 
+    if settings['split_type'] == 'homogeneous':
+        return [orchestrator_data, Shard_Splits.homogeneous(dataset=dataset, settings=settings)]
+    
+    # Type: Heterogeneous Size, Homogeneous Distribution -> Differeny size (draws from exponential distribution), similar distribution
+    elif settings['split_type'] == 'heterogeneous_size':
+        return [orchestrator_data, Shard_Splits.heterogeneous_size(dataset=dataset, settings=settings)]
     
-    # Type: Uniform with Imbalanced Classes -> Samze size, different (random) distributions with heavy imbalance on selected clients
-    if settings['split_type'] == 'random_imbalanced':
-        return [orchestrator_data, Shard_Splits.random_imbalanced(dataset=dataset, settings=settings)]
+    # Type: Dominant clients are sampled first according to the pre-defined in-sample distribution. Then rest of the clients draws from 
+    # left-over data instances
+    elif settings['split_type'] == "dominant_sampling":
+        return [orchestrator_data, Shard_Splits.dominant_sampling(dataset=dataset, settings=settings)]
 
-    # Type: Same Dataset -> One dataset copied n times.
+    # Type: Dataset replication -> One dataset copied n times.
     elif settings['split_type'] == 'replicate_same_dataset':
         return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
     
     # Type: Blocks - One dataset copied inside one block (cluster)
     elif settings['split_type'] == 'split_in_blocks':
         return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
     
     else:
         raise "Unable to generate the dataset. Provided split-type does not exist."
+
```

### Comparing `asociita-0.1.8/asociita/datasets/load_fmnist.py` & `asociita-0.1.9/asociita/datasets/load_mnist.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from asociita.datasets.shard_splits import Shard_Splits
 from asociita.utils.showcase import save_random
 from asociita.utils.handlers import Handler
 import copy
 import pandas as pd
 import numpy as np
 
-def load_fmnist(settings: dict) -> list[datasets.arrow_dataset.Dataset,
+def load_mnist(settings: dict) -> list[datasets.arrow_dataset.Dataset,
                                        list[list[list[datasets.arrow_dataset.Dataset]]]]:
     """Loads the MNIST dataset, splits it into the number of shards, pre-process selected
     shards (subsets) and returns in a following format:
     list[   
         "Orchestrator Data"[
             Dataset
             ],   
@@ -30,27 +30,32 @@
     Args:
         settings (dict) : A dictionary containing all the dataset settings.
     Returns:
         list[datasets.arrow_dataset.Dataset,
                                        list[list[list[datasets.arrow_dataset.Dataset]]]]"""
     
     # Using the 'test' data as a orchestrator validaiton set.
-    orchestrator_data = load_dataset('fashion_mnist', split='test')
+    orchestrator_data = load_dataset('mnist', split='test')
     # Using the 'train' data as a dataset reserved for agents
-    dataset = load_dataset('fashion_mnist', split='train')
+    dataset = load_dataset('mnist', split='train')
 
-    # Type: Random Uniform (Sharding) -> Same size, random distribution
-    if settings['split_type'] == 'random_uniform':
-        return [orchestrator_data, Shard_Splits.random_uniform(dataset=dataset, settings=settings)]
+    # Type: Homogeneous Size and Distribution (Sharding) -> Same size, similar distribution 
+    if settings['split_type'] == 'homogeneous':
+        return [orchestrator_data, Shard_Splits.homogeneous(dataset=dataset, settings=settings)]
     
-    # Type: Uniform with Imbalanced Classes -> Samze size, different (random) distributions with heavy imbalance on selected clients
-    if settings['split_type'] == 'random_imbalanced':
-        return [orchestrator_data, Shard_Splits.random_imbalanced(dataset=dataset, settings=settings)]
+    # Type: Heterogeneous Size, Homogeneous Distribution -> Differeny size (draws from exponential distribution), similar distribution
+    elif settings['split_type'] == 'heterogeneous_size':
+        return [orchestrator_data, Shard_Splits.heterogeneous_size(dataset=dataset, settings=settings)]
+    
+    # Type: Dominant clients are sampled first according to the pre-defined in-sample distribution. Then rest of the clients draws from 
+    # left-over data instances
+    elif settings['split_type'] == "dominant_sampling":
+        return [orchestrator_data, Shard_Splits.dominant_sampling(dataset=dataset, settings=settings)]
 
-    # Type: Same Dataset -> One dataset copied n times.
+    # Type: Dataset replication -> One dataset copied n times.
     elif settings['split_type'] == 'replicate_same_dataset':
         return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
     
     # Type: Blocks - One dataset copied inside one block (cluster)
     elif settings['split_type'] == 'split_in_blocks':
         return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
```

### Comparing `asociita-0.1.8/asociita/datasets/load_mnist.py` & `asociita-0.1.9/asociita/datasets/load_cifar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import datasets
 from datasets import load_dataset
-from asociita.datasets.shard_transformation import Shard_Transformation
 from asociita.datasets.shard_splits import Shard_Splits
 from asociita.utils.showcase import save_random
 from asociita.utils.handlers import Handler
 import copy
 import pandas as pd
 import numpy as np
 
-def load_mnist(settings: dict) -> list[datasets.arrow_dataset.Dataset,
+def load_cifar(settings: dict) -> list[datasets.arrow_dataset.Dataset,
                                        list[list[list[datasets.arrow_dataset.Dataset]]]]:
-    """Loads the MNIST dataset, splits it into the number of shards, pre-process selected
+    """Loads the CIFAR dataset, splits it into the number of shards, pre-process selected
     shards (subsets) and returns in a following format:
     list[   
         "Orchestrator Data"[
             Dataset
             ],   
         "Agents Data"[
             "Agent N"[
@@ -30,27 +29,35 @@
     Args:
         settings (dict) : A dictionary containing all the dataset settings.
     Returns:
         list[datasets.arrow_dataset.Dataset,
                                        list[list[list[datasets.arrow_dataset.Dataset]]]]"""
     
     # Using the 'test' data as a orchestrator validaiton set.
-    orchestrator_data = load_dataset('mnist', split='test')
+    orchestrator_data = load_dataset('cifar10', split='test')
     # Using the 'train' data as a dataset reserved for agents
-    dataset = load_dataset('mnist', split='train')
+    dataset = load_dataset('cifar10', split='train')
 
-    # Type: Random Uniform (Sharding) -> Same size, random distribution
-    if settings['split_type'] == 'random_uniform':
-        return [orchestrator_data, Shard_Splits.random_uniform(dataset=dataset, settings=settings)]
+    orchestrator_data = orchestrator_data.rename_column('img', 'image')
+    dataset = dataset.rename_column('img', 'image')
+
+    # Type: Homogeneous Size and Distribution (Sharding) -> Same size, similar distribution 
+    if settings['split_type'] == 'homogeneous':
+        return [orchestrator_data, Shard_Splits.homogeneous(dataset=dataset, settings=settings)]
+    
+    # Type: Heterogeneous Size, Homogeneous Distribution -> Differeny size (draws from exponential distribution), similar distribution
+    elif settings['split_type'] == 'heterogeneous_size':
+        return [orchestrator_data, Shard_Splits.heterogeneous_size(dataset=dataset, settings=settings)]
     
-    # Type: Uniform with Imbalanced Classes -> Samze size, different (random) distributions with heavy imbalance on selected clients
-    if settings['split_type'] == 'random_imbalanced':
-        return [orchestrator_data, Shard_Splits.random_imbalanced(dataset=dataset, settings=settings)]
+    # Type: Dominant clients are sampled first according to the pre-defined in-sample distribution. Then rest of the clients draws from 
+    # left-over data instances
+    elif settings['split_type'] == "dominant_sampling":
+        return [orchestrator_data, Shard_Splits.dominant_sampling(dataset=dataset, settings=settings)]
 
-    # Type: Same Dataset -> One dataset copied n times.
+    # Type: Dataset replication -> One dataset copied n times.
     elif settings['split_type'] == 'replicate_same_dataset':
         return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
     
     # Type: Blocks - One dataset copied inside one block (cluster)
     elif settings['split_type'] == 'split_in_blocks':
         return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
```

### Comparing `asociita-0.1.8/asociita/datasets/shard_splits.py` & `asociita-0.1.9/asociita/datasets/shard_splits.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import datasets
 from datasets import load_dataset
 from asociita.datasets.shard_transformation import Shard_Transformation
 from asociita.utils.handlers import Handler
 from asociita.utils.showcase import save_random
 import copy
+import numpy as np
 
-
+def rescale_vector_tosum(vector, desired_sum):
+    norm_const = desired_sum / vector.sum()
+    vector = vector * norm_const
+    vector = vector.astype(int)
+    l = desired_sum - vector.sum()
+    np.argpartition(vector, l)
+    for _ in range(l):
+        vector[np.argmin(vector)] += 1
+    return vector
 
 class Shard_Splits:
     """a common class for creating various splits among the clients"""
 
     @staticmethod
-    def random_uniform(dataset: datasets.arrow_dataset.Dataset,
-                       settings: dict):
+    def homogeneous(dataset: datasets.arrow_dataset.Dataset,
+                    settings: dict):
         nodes_data = []
         for shard in range(settings['shards']): # Each shard corresponds to one agent.
             agent_data = dataset.shard(num_shards=settings['shards'], index=shard)
             
             # Shard transformation
             if shard in settings['transformations'].keys():
                 if settings['save_transformations']:
@@ -26,39 +35,51 @@
                     save_random(original_imgs, agent_data['image'], settings['transformations'][shard]["transformation_type"])
 
             # In-shard split between test and train data.
             agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
             nodes_data.append([agent_data['train'], agent_data['test']])
         return nodes_data
     
+    @staticmethod
+    def heterogeneous_size(dataset: datasets.arrow_dataset.Dataset,
+                      settings: dict):
+        nodes_data = []
+        clients = settings['agents']
+        beta = len(dataset) / clients # Average shard size
+        rng = np.random.default_rng(42)
+
+        # Drawing from exponential distribution size of the local sample
+        shards_sizes = rng.exponential(scale=beta, size=clients)
+        shards_sizes = rescale_vector_tosum(vector = shards_sizes, desired_sum = len(dataset))
+        print(shards_sizes)
+
+        dataset = dataset.shuffle(seed=42)
+        moving_idx = 0
+        for agent in range(clients):
+            ag_idx = moving_idx + shards_sizes[agent]
+            agent_data = dataset.select(range(moving_idx, ag_idx))
+            moving_idx = ag_idx
+            agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
+            nodes_data.append([agent_data['train'], agent_data['test']])
+        return nodes_data
 
     @staticmethod
-    def random_imbalanced(dataset: datasets.arrow_dataset.Dataset,
+    def dominant_sampling(dataset: datasets.arrow_dataset.Dataset,
                           settings: dict):
         nodes_data = []
         no_agents = settings['agents']
         imbalanced_agents = settings['imbalanced_clients']
         agents = [agent for agent in range(no_agents)]
         pandas_df = dataset.to_pandas().drop('image', axis=1)
         labels = sorted(pandas_df.label.unique())
-
-        save_distribution = False
-        print_distribution = False
-        
-        if settings.get('save_distribution'):
-            distribution_blueprint = []
-            save_distribution = True
-        if settings.get('print_distribution'):
-            print_distribution = True
         if settings.get('custom_sample_size'):
             sample_size = settings['custom_sample_size']
         else:
             sample_size = int(len(dataset) / no_agents)
     
-
         # I) Sampling dominant clients
         for agent in agents:
             if agent in imbalanced_agents:
                 # 1. Sampling indexes
                 sampling_weights = {key: (1 - imbalanced_agents[agent][1]) / (len(labels) - 1) for key in labels}
                 sampling_weights[imbalanced_agents[agent][0]] = imbalanced_agents[agent][1]
                 
@@ -67,56 +88,37 @@
                 # counts = pandas_df['label'].value_counts()[pandas_df['label'].value_counts() > required_samples]
                 
                 # 2. Apllying weights
                 pandas_df["weights"] = pandas_df['label'].apply(lambda x: sampling_weights[x])
                 sample = pandas_df.sample(n = sample_size, weights='weights', random_state=42)
                 
                 counts = sample['label'].value_counts().sort_index()
-                if print_distribution:
-                    print(f"Distribution of client {agent} is : {counts}")
-                if save_distribution:
-                    ag = counts.to_dict()
-                    distribution = {'agent':agent}
-                    distribution.update(ag)
-                    distribution_blueprint.append(distribution)
                 # 3. Selecting indexes and performing test - train split.
-                sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
+                sampled_data = dataset.filter(lambda idx: idx in list(sample.index), with_indices=True)
                 agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
                 nodes_data.append([agent_data['train'], agent_data['test']])
                 
                 # 4. Removing samples indexes
                 pandas_df.drop(sample.index, inplace=True)
             else:
                 nodes_data.append([]) # Inserting placeholder to preserve in-list order.
 
 
-        # II) Sampling balanced clients
+        # II) Sampling non-dominant clients
         for agent in agents:
             if agent not in imbalanced_agents:
                 # 1. Sampling indexes
                 sample = pandas_df.sample(n = sample_size, random_state=42)
                 counts = sample['label'].value_counts().sort_index()
-                if print_distribution:
-                    print(f"Distribution of client {agent} is : {counts}")
-                if save_distribution:
-                    ag = counts.to_dict()
-                    distribution = {'agent':agent}
-                    distribution.update(ag)
-                    distribution_blueprint.append(distribution)
                 # 2. Selecting indexes and performing test - train split.
                 sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
                 agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
                 nodes_data[agent] = ([agent_data['train'], agent_data['test']])
                 # 3. Removing samples indexes
                 pandas_df.drop(sample.index, inplace=True)
-        
-        if save_distribution:
-            Handler.save_csv_file(file = distribution_blueprint,
-                                  saving_path=settings['save_path'],
-                                  file_name='distribution_blueprint.csv')
         return nodes_data
 
     @staticmethod
     def replicate_same_dataset(dataset: datasets.arrow_dataset.Dataset,
                                settings: dict):
         nodes_data = []
         agent_data = dataset.shard(num_shards=1, index=0)
```

### Comparing `asociita-0.1.8/asociita/datasets/shard_transformation.py` & `asociita-0.1.9/asociita/datasets/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/models/pytorch/cifar10.py` & `asociita-0.1.9/asociita/models/pytorch/cifar10.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/models/pytorch/federated_model.py` & `asociita-0.1.9/asociita/models/pytorch/federated_model.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/models/pytorch/mnist.py` & `asociita-0.1.9/asociita/models/pytorch/mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/utils/computations.py` & `asociita-0.1.9/asociita/utils/computations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/utils/custom_transformations.py` & `asociita-0.1.9/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/utils/handlers.py` & `asociita-0.1.9/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/utils/helpers.py` & `asociita-0.1.9/asociita/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/utils/loggers.py` & `asociita-0.1.9/asociita/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/utils/optimizers.py` & `asociita-0.1.9/asociita/utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/utils/orchestrations.py` & `asociita-0.1.9/asociita/utils/orchestrations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/asociita/utils/showcase.py` & `asociita-0.1.9/asociita/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.8/pyproject.toml` & `asociita-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asociita"
-version = "0.1.8"
+version = "0.1.9"
 description = "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting."
 authors = ["Maciej Zuziak <maciejkrzysztof.zuziak@isti.cnr.it>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Scolpe/Asociita"
 repository = "https://github.com/Scolpe/Asociita"
```

### Comparing `asociita-0.1.8/PKG-INFO` & `asociita-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.1.8
+Version: 0.1.9
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

