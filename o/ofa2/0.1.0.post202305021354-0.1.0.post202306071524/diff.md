# Comparing `tmp/ofa2-0.1.0.post202305021354.tar.gz` & `tmp/ofa2-0.1.0.post202306071524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofa2-0.1.0.post202305021354.tar", last modified: Tue May  2 16:54:11 2023, max compression
+gzip compressed data, was "ofa2-0.1.0.post202306071524.tar", last modified: Wed Jun  7 18:24:29 2023, max compression
```

## Comparing `ofa2-0.1.0.post202305021354.tar` & `ofa2-0.1.0.post202306071524.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.800669 ofa2-0.1.0.post202305021354/
--rw-r--r--   0 rafael    (1005) rafael    (1005)     1064 2023-04-17 12:49:36.000000 ofa2-0.1.0.post202305021354/LICENSE
--rw-r--r--   0 rafael    (1005) rafael    (1005)      857 2023-05-02 16:54:11.800669 ofa2-0.1.0.post202305021354/PKG-INFO
--rw-r--r--   0 rafael    (1005) rafael    (1005)    16441 2023-04-17 12:49:36.000000 ofa2-0.1.0.post202305021354/README.md
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.650671 ofa2-0.1.0.post202305021354/ofa2/
--rw-r--r--   0 rafael    (1005) rafael    (1005)        0 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/__init__.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.677337 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/
--rw-r--r--   0 rafael    (1005) rafael    (1005)        0 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/__init__.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.697337 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/data_providers/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      231 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/data_providers/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     1731 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/data_providers/base_provider.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    11126 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/data_providers/imagenet.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.697337 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/
--rw-r--r--   0 rafael    (1005) rafael    (1005)        0 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/__init__.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.700670 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/modules/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      263 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/modules/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    29331 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/modules/dynamic_layers.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    13823 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/modules/dynamic_op.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.704003 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/networks/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      327 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/networks/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    14581 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/networks/ofa_mbv3.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    14157 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/networks/ofa_proxyless.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    12547 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/networks/ofa_resnets.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.704003 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/training/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      244 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/training/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    15225 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/training/progressive_shrinking.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     3124 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/utils.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.704003 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/networks/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      593 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/networks/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    10082 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/networks/mobilenet_v3.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     8250 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/networks/proxyless_nets.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     7845 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/networks/resnets.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.707337 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/run_manager/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      299 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/run_manager/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    18169 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/run_manager/distributed_run_manager.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     7798 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/run_manager/run_config.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    17267 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/run_manager/run_manager.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     3807 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/model_zoo.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.707337 ofa2-0.1.0.post202305021354/ofa2/nas/
--rw-r--r--   0 rafael    (1005) rafael    (1005)        0 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/nas/__init__.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.707337 ofa2-0.1.0.post202305021354/ofa2/nas/accuracy_predictor/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      291 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/nas/accuracy_predictor/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     7637 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/nas/accuracy_predictor/acc_dataset.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     2045 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/nas/accuracy_predictor/acc_predictor.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    13652 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/nas/accuracy_predictor/arch_encoder.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.710670 ofa2-0.1.0.post202305021354/ofa2/nas/efficiency_predictor/
--rw-r--r--   0 rafael    (1005) rafael    (1005)     3051 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/nas/efficiency_predictor/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    19459 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/nas/efficiency_predictor/latency_lookup_table.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.710670 ofa2-0.1.0.post202305021354/ofa2/nas/search_algorithm/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      232 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/nas/search_algorithm/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     5784 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/nas/search_algorithm/evolution.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.750669 ofa2-0.1.0.post202305021354/ofa2/tutorial/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      371 2023-04-26 17:49:54.000000 ofa2-0.1.0.post202305021354/ofa2/tutorial/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     2675 2023-04-28 14:55:50.000000 ofa2-0.1.0.post202305021354/ofa2/tutorial/accuracy_predictor.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     8945 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/tutorial/evolution_finder.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    14989 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/tutorial/flops_table.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     9856 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/tutorial/imagenet_eval_helper.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     7182 2023-05-02 16:52:02.000000 ofa2-0.1.0.post202305021354/ofa2/tutorial/latency_table.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     2798 2023-04-28 14:13:46.000000 ofa2-0.1.0.post202305021354/ofa2/tutorial/multi_objective_optimization.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.784002 ofa2-0.1.0.post202305021354/ofa2/utils/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      379 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     8521 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/common_tools.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     2534 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/flops_counter.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    24146 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/layers.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.800669 ofa2-0.1.0.post202305021354/ofa2/utils/my_dataloader/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      135 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/my_dataloader/__init__.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)    49832 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/my_dataloader/my_data_loader.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     8816 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/my_dataloader/my_data_worker.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     2982 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/my_dataloader/my_distributed_sampler.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     5414 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/my_dataloader/my_random_resize_crop.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     8750 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/my_modules.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     4694 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/pytorch_modules.py
--rw-r--r--   0 rafael    (1005) rafael    (1005)     6949 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/ofa2/utils/pytorch_utils.py
-drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-05-02 16:54:11.660671 ofa2-0.1.0.post202305021354/ofa2.egg-info/
--rw-r--r--   0 rafael    (1005) rafael    (1005)      857 2023-05-02 16:54:11.000000 ofa2-0.1.0.post202305021354/ofa2.egg-info/PKG-INFO
--rw-r--r--   0 rafael    (1005) rafael    (1005)     2566 2023-05-02 16:54:11.000000 ofa2-0.1.0.post202305021354/ofa2.egg-info/SOURCES.txt
--rw-r--r--   0 rafael    (1005) rafael    (1005)        1 2023-05-02 16:54:11.000000 ofa2-0.1.0.post202305021354/ofa2.egg-info/dependency_links.txt
--rw-r--r--   0 rafael    (1005) rafael    (1005)        6 2023-05-02 16:54:11.000000 ofa2-0.1.0.post202305021354/ofa2.egg-info/requires.txt
--rw-r--r--   0 rafael    (1005) rafael    (1005)        5 2023-05-02 16:54:11.000000 ofa2-0.1.0.post202305021354/ofa2.egg-info/top_level.txt
--rw-r--r--   0 rafael    (1005) rafael    (1005)        1 2023-04-17 13:56:25.000000 ofa2-0.1.0.post202305021354/ofa2.egg-info/zip-safe
--rw-r--r--   0 rafael    (1005) rafael    (1005)       38 2023-05-02 16:54:11.800669 ofa2-0.1.0.post202305021354/setup.cfg
--rw-r--r--   0 rafael    (1005) rafael    (1005)     1583 2023-04-17 12:50:06.000000 ofa2-0.1.0.post202305021354/setup.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.057114 ofa2-0.1.0.post202306071524/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     1064 2023-04-17 12:49:36.000000 ofa2-0.1.0.post202306071524/LICENSE
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      857 2023-06-07 18:24:29.057114 ofa2-0.1.0.post202306071524/PKG-INFO
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     1690 2023-06-01 13:03:10.000000 ofa2-0.1.0.post202306071524/README.md
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.027114 ofa2-0.1.0.post202306071524/ofa2/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)        0 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/__init__.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.053780 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)        0 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/__init__.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.053780 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/data_providers/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      231 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/data_providers/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     1731 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/data_providers/base_provider.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    11126 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/data_providers/imagenet.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.053780 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)        0 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/__init__.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.053780 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/modules/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      263 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/modules/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    29331 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/modules/dynamic_layers.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    13823 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/modules/dynamic_op.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.053780 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/networks/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      327 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/networks/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    14581 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/networks/ofa_mbv3.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    14157 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/networks/ofa_proxyless.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    12547 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/networks/ofa_resnets.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.053780 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/training/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      244 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/training/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    15225 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/training/progressive_shrinking.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     3124 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/utils.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.053780 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/networks/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      593 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/networks/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    10082 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/networks/mobilenet_v3.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     8250 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/networks/proxyless_nets.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     7845 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/networks/resnets.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.053780 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/run_manager/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      299 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/run_manager/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    18169 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/run_manager/distributed_run_manager.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     7798 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/run_manager/run_config.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    17267 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/run_manager/run_manager.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     3807 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/model_zoo.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.057114 ofa2-0.1.0.post202306071524/ofa2/nas/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)        0 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/nas/__init__.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.057114 ofa2-0.1.0.post202306071524/ofa2/nas/accuracy_predictor/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      291 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/nas/accuracy_predictor/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     7637 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/nas/accuracy_predictor/acc_dataset.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     2045 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/nas/accuracy_predictor/acc_predictor.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    13652 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/nas/accuracy_predictor/arch_encoder.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.057114 ofa2-0.1.0.post202306071524/ofa2/nas/efficiency_predictor/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     3051 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/nas/efficiency_predictor/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    19459 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/nas/efficiency_predictor/latency_lookup_table.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.057114 ofa2-0.1.0.post202306071524/ofa2/nas/search_algorithm/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      232 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/nas/search_algorithm/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     5784 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/nas/search_algorithm/evolution.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.057114 ofa2-0.1.0.post202306071524/ofa2/tutorial/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      371 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/tutorial/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     2675 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/tutorial/accuracy_predictor.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     8945 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/tutorial/evolution_finder.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    15225 2023-06-07 18:09:30.000000 ofa2-0.1.0.post202306071524/ofa2/tutorial/flops_table.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     9856 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/tutorial/imagenet_eval_helper.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     7182 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/tutorial/latency_table.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     2798 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/tutorial/multi_objective_optimization.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.057114 ofa2-0.1.0.post202306071524/ofa2/utils/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      379 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     8521 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/common_tools.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     2534 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/flops_counter.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    24146 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/layers.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.057114 ofa2-0.1.0.post202306071524/ofa2/utils/my_dataloader/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      135 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/my_dataloader/__init__.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)    49832 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/my_dataloader/my_data_loader.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     8816 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/my_dataloader/my_data_worker.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     2982 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/my_dataloader/my_distributed_sampler.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     5414 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/my_dataloader/my_random_resize_crop.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     8750 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/my_modules.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     4694 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/pytorch_modules.py
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     6949 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/ofa2/utils/pytorch_utils.py
+drwxr-xr-x   0 rafael    (1005) rafael    (1005)        0 2023-06-07 18:24:29.030447 ofa2-0.1.0.post202306071524/ofa2.egg-info/
+-rw-r--r--   0 rafael    (1005) rafael    (1005)      857 2023-06-07 18:24:29.000000 ofa2-0.1.0.post202306071524/ofa2.egg-info/PKG-INFO
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     2566 2023-06-07 18:24:29.000000 ofa2-0.1.0.post202306071524/ofa2.egg-info/SOURCES.txt
+-rw-r--r--   0 rafael    (1005) rafael    (1005)        1 2023-06-07 18:24:29.000000 ofa2-0.1.0.post202306071524/ofa2.egg-info/dependency_links.txt
+-rw-r--r--   0 rafael    (1005) rafael    (1005)        6 2023-06-07 18:24:29.000000 ofa2-0.1.0.post202306071524/ofa2.egg-info/requires.txt
+-rw-r--r--   0 rafael    (1005) rafael    (1005)        5 2023-06-07 18:24:29.000000 ofa2-0.1.0.post202306071524/ofa2.egg-info/top_level.txt
+-rw-r--r--   0 rafael    (1005) rafael    (1005)        1 2023-04-17 13:56:25.000000 ofa2-0.1.0.post202306071524/ofa2.egg-info/zip-safe
+-rw-r--r--   0 rafael    (1005) rafael    (1005)       38 2023-06-07 18:24:29.057114 ofa2-0.1.0.post202306071524/setup.cfg
+-rw-r--r--   0 rafael    (1005) rafael    (1005)     1583 2023-05-30 20:05:19.000000 ofa2-0.1.0.post202306071524/setup.py
```

### Comparing `ofa2-0.1.0.post202305021354/LICENSE` & `ofa2-0.1.0.post202306071524/LICENSE`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/PKG-INFO` & `ofa2-0.1.0.post202306071524/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofa2
-Version: 0.1.0.post202305021354
+Version: 0.1.0.post202306071524
 Summary: Train one network, Search once, Deploy in many scenarios.
 Home-page: https://github.com/ito-rafael/once-for-all-2
 Author: Rafael Ito
 Author-email: ito.rafael@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/data_providers/base_provider.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/data_providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/data_providers/imagenet.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/data_providers/imagenet.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/modules/dynamic_layers.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/modules/dynamic_layers.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/modules/dynamic_op.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/modules/dynamic_op.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/networks/ofa_mbv3.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/networks/ofa_mbv3.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/networks/ofa_proxyless.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/networks/ofa_proxyless.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/networks/ofa_resnets.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/networks/ofa_resnets.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/training/progressive_shrinking.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/training/progressive_shrinking.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/elastic_nn/utils.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/elastic_nn/utils.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/networks/__init__.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/networks/mobilenet_v3.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/networks/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/networks/proxyless_nets.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/networks/proxyless_nets.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/networks/resnets.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/networks/resnets.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/run_manager/distributed_run_manager.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/run_manager/distributed_run_manager.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/run_manager/run_config.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/run_manager/run_config.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/imagenet_classification/run_manager/run_manager.py` & `ofa2-0.1.0.post202306071524/ofa2/imagenet_classification/run_manager/run_manager.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/model_zoo.py` & `ofa2-0.1.0.post202306071524/ofa2/model_zoo.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/nas/accuracy_predictor/acc_dataset.py` & `ofa2-0.1.0.post202306071524/ofa2/nas/accuracy_predictor/acc_dataset.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/nas/accuracy_predictor/acc_predictor.py` & `ofa2-0.1.0.post202306071524/ofa2/nas/accuracy_predictor/acc_predictor.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/nas/accuracy_predictor/arch_encoder.py` & `ofa2-0.1.0.post202306071524/ofa2/nas/accuracy_predictor/arch_encoder.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/nas/efficiency_predictor/__init__.py` & `ofa2-0.1.0.post202306071524/ofa2/nas/efficiency_predictor/__init__.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/nas/efficiency_predictor/latency_lookup_table.py` & `ofa2-0.1.0.post202306071524/ofa2/nas/efficiency_predictor/latency_lookup_table.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/nas/search_algorithm/evolution.py` & `ofa2-0.1.0.post202306071524/ofa2/nas/search_algorithm/evolution.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/tutorial/accuracy_predictor.py` & `ofa2-0.1.0.post202306071524/ofa2/tutorial/accuracy_predictor.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/tutorial/evolution_finder.py` & `ofa2-0.1.0.post202306071524/ofa2/tutorial/evolution_finder.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/tutorial/flops_table.py` & `ofa2-0.1.0.post202306071524/ofa2/tutorial/flops_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -455,32 +455,35 @@
         self.efficiency_dict[base_resolution] = efficiency_dict
         print(
             "Built the %s lookup table (resolution=%d)!"
             % (self.pred_type, base_resolution)
         )
         return efficiency_dict
 
-    def predict_efficiency(self, sample):
-        input_size = sample.get("r", [224])
-        input_size = input_size[0]
-        assert "ks" in sample and "e" in sample and "d" in sample
-        assert len(sample["ks"]) == len(sample["e"]) and len(sample["ks"]) == 20
-        assert len(sample["d"]) == 5
-        total_stats = 0.0
-        for i in range(20):
-            stage = i // 4
-            depth_max = sample["d"][stage]
-            depth = i % 4 + 1
-            if depth > depth_max:
-                continue
-            ks, e = sample["ks"][i], sample["e"][i]
-            total_stats += self.efficiency_dict[input_size]["mobile_inverted_blocks"][
-                i + 1
-            ][(ks, e)]
+    def predict_efficiency(self, population):
+        flops_list = []
+        for individual in population:
+            input_size = individual.get("r", [224])
+            input_size = input_size[0]
+            assert "ks" in individual and "e" in individual and "d" in individual
+            assert len(individual["ks"]) == len(individual["e"]) and len(individual["ks"]) == 20
+            assert len(individual["d"]) == 5
+            total_stats = 0.0
+            for i in range(20):
+                stage = i // 4
+                depth_max = individual["d"][stage]
+                depth = i % 4 + 1
+                if depth > depth_max:
+                    continue
+                ks, e = individual["ks"][i], individual["e"][i]
+                total_stats += self.efficiency_dict[input_size]["mobile_inverted_blocks"][
+                    i + 1
+                ][(ks, e)]
 
-        for key in self.efficiency_dict[input_size]["other_blocks"]:
-            total_stats += self.efficiency_dict[input_size]["other_blocks"][key]
+            for key in self.efficiency_dict[input_size]["other_blocks"]:
+                total_stats += self.efficiency_dict[input_size]["other_blocks"][key]
 
-        total_stats += self.efficiency_dict[input_size]["mobile_inverted_blocks"][0][
-            (3, 1)
-        ]
-        return total_stats
+            total_stats += self.efficiency_dict[input_size]["mobile_inverted_blocks"][0][
+                (3, 1)
+            ]
+            flops_list.append(total_stats)
+        return flops_list
```

### Comparing `ofa2-0.1.0.post202305021354/ofa2/tutorial/imagenet_eval_helper.py` & `ofa2-0.1.0.post202306071524/ofa2/tutorial/imagenet_eval_helper.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/tutorial/latency_table.py` & `ofa2-0.1.0.post202306071524/ofa2/tutorial/latency_table.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/tutorial/multi_objective_optimization.py` & `ofa2-0.1.0.post202306071524/ofa2/tutorial/multi_objective_optimization.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/utils/common_tools.py` & `ofa2-0.1.0.post202306071524/ofa2/utils/common_tools.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/utils/flops_counter.py` & `ofa2-0.1.0.post202306071524/ofa2/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/utils/layers.py` & `ofa2-0.1.0.post202306071524/ofa2/utils/layers.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/utils/my_dataloader/my_data_loader.py` & `ofa2-0.1.0.post202306071524/ofa2/utils/my_dataloader/my_data_loader.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/utils/my_dataloader/my_data_worker.py` & `ofa2-0.1.0.post202306071524/ofa2/utils/my_dataloader/my_data_worker.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/utils/my_dataloader/my_distributed_sampler.py` & `ofa2-0.1.0.post202306071524/ofa2/utils/my_dataloader/my_distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/utils/my_dataloader/my_random_resize_crop.py` & `ofa2-0.1.0.post202306071524/ofa2/utils/my_dataloader/my_random_resize_crop.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/utils/my_modules.py` & `ofa2-0.1.0.post202306071524/ofa2/utils/my_modules.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/utils/pytorch_modules.py` & `ofa2-0.1.0.post202306071524/ofa2/utils/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2/utils/pytorch_utils.py` & `ofa2-0.1.0.post202306071524/ofa2/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/ofa2.egg-info/PKG-INFO` & `ofa2-0.1.0.post202306071524/ofa2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofa2
-Version: 0.1.0.post202305021354
+Version: 0.1.0.post202306071524
 Summary: Train one network, Search once, Deploy in many scenarios.
 Home-page: https://github.com/ito-rafael/once-for-all-2
 Author: Rafael Ito
 Author-email: ito.rafael@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `ofa2-0.1.0.post202305021354/ofa2.egg-info/SOURCES.txt` & `ofa2-0.1.0.post202306071524/ofa2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ofa2-0.1.0.post202305021354/setup.py` & `ofa2-0.1.0.post202306071524/setup.py`

 * *Files identical despite different names*

