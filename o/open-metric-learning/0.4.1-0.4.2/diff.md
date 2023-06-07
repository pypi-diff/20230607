# Comparing `tmp/open-metric-learning-0.4.1.tar.gz` & `tmp/open-metric-learning-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/open-metric-learning-0.4.1.tar", last modified: Fri May 12 16:43:31 2023, max compression
+gzip compressed data, was "dist/open-metric-learning-0.4.2.tar", last modified: Wed Jun  7 18:27:10 2023, max compression
```

## Comparing `open-metric-learning-0.4.1.tar` & `open-metric-learning-0.4.2.tar`

### file list

```diff
@@ -1,202 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    25957 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24533 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/criterion/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/mlp_arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/surrogate_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/triplet.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/triplet_plain.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/triplet_with_miner.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/extractor/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/extractor/extractor_with_mlp.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/extractor/resnet.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/extractor/vit.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/extractor/vit_clip.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/miner/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/all_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/hard_cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/miner_with_bank.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/n_hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/triplets_with_memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/optimizer/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/adadelta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/adagrad.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/adamax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/adamw.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/asgd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/lbfgs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/rmsprop.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/rprop.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/pairwise_model/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/pairwise_model/concat_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/pairwise_model/linear_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/pairwise_model/trivial_distance_siamese.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/postprocessor/pairwise_embeddings.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/postprocessor/pairwise_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/configs/sampler/
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/sampler/balance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/sampler/category_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/sampler/distinct_category_balance.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/configs/scheduler/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/cosine_annealing.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/cyclic.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/lambda.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/multi_step.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/multiplicative.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/one_cycle.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/reduce_on_plateau.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/step.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/configs/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/augs_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/augs_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/augs_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_resize_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_resize_albu_clip.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_resize_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_resize_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/const.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12302 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4428 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/datasets/list_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/datasets/pairs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3739 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/datasets/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/ddp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/ddp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/ddp/patching.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/ddp/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/functional/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/functional/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/functional/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)    25034 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/functional/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/inference/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/inference/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/inference/flat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/inference/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/criterions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     2354 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3106 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/miners.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/lightning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/lightning/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8802 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/callbacks/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/lightning/modules/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/modules/ddp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/modules/extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/modules/pairwise_postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/lightning/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/pipelines/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/pipelines/train.py
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/pipelines/train_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/pipelines/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/losses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/losses/arcface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/losses/surrogate_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     8578 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/losses/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    15976 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/metrics/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/metrics/triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/miners/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/inbatch_all_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     6530 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/inbatch_hard_cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/inbatch_hard_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     5799 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/inbatch_nhard_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/miner_with_bank.py
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/models/
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/models/meta/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/meta/projection.py
--rw-r--r--   0 runner    (1001) docker     (122)     5280 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/meta/siamese.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/pooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     7763 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/models/vit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/clip.py
--rw-r--r--   0 runner    (1001) docker     (122)     5696 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/hubconf.py
--rw-r--r--   0 runner    (1001) docker     (122)    13388 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/vision_transformer_clip.py
--rw-r--r--   0 runner    (1001) docker     (122)     8065 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/registry/
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/miners.py
--rw-r--r--   0 runner    (1001) docker     (122)     2679 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/samplers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/retrieval/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/retrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/retrieval/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/retrieval/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/retrieval/postprocessors/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/samplers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/samplers/balance.py
--rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/samplers/category_balance.py
--rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/samplers/distinct_category_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/transforms/images/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/transforms/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/transforms/images/albumentations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/transforms/images/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/transforms/images/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/oml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/dataframe_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/download_mock_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/oml/utils/images/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3128 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/images/images.py
--rw-r--r--   0 runner    (1001) docker     (122)     6600 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/images/images_resize.py
--rw-r--r--   0 runner    (1001) docker     (122)     4202 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5640 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)    16347 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/misc_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/remote_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/open_metric_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    25957 2023-05-12 16:43:30.000000 open-metric-learning-0.4.1/open_metric_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5159 2023-05-12 16:43:30.000000 open-metric-learning-0.4.1/open_metric_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 16:43:30.000000 open-metric-learning-0.4.1/open_metric_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-05-12 16:43:30.000000 open-metric-learning-0.4.1/open_metric_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-05-12 16:43:30.000000 open-metric-learning-0.4.1/open_metric_learning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/tests/test_build_readme.py
--rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/tests/test_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    26089 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24665 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.673302 open-metric-learning-0.4.2/oml/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.673302 open-metric-learning-0.4.2/oml/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.673302 open-metric-learning-0.4.2/oml/configs/criterion/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/mlp_arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/surrogate_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/triplet.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/triplet_plain.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/criterion/triplet_with_miner.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.677302 open-metric-learning-0.4.2/oml/configs/extractor/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/extractor/extractor_with_mlp.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/extractor/resnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/extractor/vit.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/extractor/vit_clip.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.677302 open-metric-learning-0.4.2/oml/configs/miner/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/all_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/hard_cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/miner_with_bank.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/n_hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/miner/triplets_with_memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.681301 open-metric-learning-0.4.2/oml/configs/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/adadelta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/adagrad.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/adamax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/adamw.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/asgd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/lbfgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/rmsprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/rprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/optimizer/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.681301 open-metric-learning-0.4.2/oml/configs/pairwise_model/
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/pairwise_model/concat_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/pairwise_model/linear_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/pairwise_model/trivial_distance_siamese.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.681301 open-metric-learning-0.4.2/oml/configs/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/postprocessor/pairwise_embeddings.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/postprocessor/pairwise_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.685301 open-metric-learning-0.4.2/oml/configs/sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/sampler/balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/sampler/category_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/sampler/distinct_category_balance.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.685301 open-metric-learning-0.4.2/oml/configs/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/cosine_annealing.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/cyclic.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/lambda.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/multi_step.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/multiplicative.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/one_cycle.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/reduce_on_plateau.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/scheduler/step.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.689301 open-metric-learning-0.4.2/oml/configs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/augs_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/augs_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/augs_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_resize_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_resize_albu_clip.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_resize_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_resize_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/configs/transforms/norm_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/const.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.689301 open-metric-learning-0.4.2/oml/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12302 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3113 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/datasets/list_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/datasets/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3791 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/datasets/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.693302 open-metric-learning-0.4.2/oml/ddp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/ddp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/ddp/patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/ddp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.693302 open-metric-learning-0.4.2/oml/functional/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/functional/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/functional/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25034 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/functional/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.693302 open-metric-learning-0.4.2/oml/inference/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/inference/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/inference/flat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/inference/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.697301 open-metric-learning-0.4.2/oml/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/criterions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2354 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3106 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/miners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/interfaces/samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.697301 open-metric-learning-0.4.2/oml/lightning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.697301 open-metric-learning-0.4.2/oml/lightning/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8880 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/callbacks/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.697301 open-metric-learning-0.4.2/oml/lightning/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/modules/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/modules/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/modules/pairwise_postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.701301 open-metric-learning-0.4.2/oml/lightning/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2956 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7566 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/train_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/lightning/pipelines/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.701301 open-metric-learning-0.4.2/oml/losses/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/losses/arcface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/losses/surrogate_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8578 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/losses/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.701301 open-metric-learning-0.4.2/oml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15994 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/metrics/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/metrics/triplets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.705301 open-metric-learning-0.4.2/oml/miners/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/inbatch_all_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6530 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/inbatch_hard_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/inbatch_hard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/inbatch_nhard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/miner_with_bank.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/miners/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.705301 open-metric-learning-0.4.2/oml/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.705301 open-metric-learning-0.4.2/oml/models/meta/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/meta/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5280 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/meta/siamese.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7763 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.709301 open-metric-learning-0.4.2/oml/models/vit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/clip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5696 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/hubconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13388 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/vision_transformer_clip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8065 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/models/vit/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/registry/
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/miners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2679 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/registry/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/retrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/retrieval/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/retrieval/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/retrieval/postprocessors/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/samplers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/samplers/balance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/samplers/category_balance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/samplers/distinct_category_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.713301 open-metric-learning-0.4.2/oml/transforms/images/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/transforms/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/transforms/images/albumentations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/transforms/images/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/transforms/images/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/oml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/dataframe_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/download_mock_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/oml/utils/images/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3818 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/images/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6600 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/images/images_resize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4202 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5640 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16347 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/misc_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/oml/utils/remote_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/open_metric_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    26089 2023-06-07 18:27:10.000000 open-metric-learning-0.4.2/open_metric_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-06-07 18:27:10.000000 open-metric-learning-0.4.2/open_metric_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 18:27:10.000000 open-metric-learning-0.4.2/open_metric_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-07 18:27:10.000000 open-metric-learning-0.4.2/open_metric_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-07 18:27:10.000000 open-metric-learning-0.4.2/open_metric_learning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 18:27:10.717301 open-metric-learning-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/tests/test_build_readme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-06-07 18:26:48.000000 open-metric-learning-0.4.2/tests/test_outdated_docs.py
```

### Comparing `open-metric-learning-0.4.1/LICENSE` & `open-metric-learning-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/PKG-INFO` & `open-metric-learning-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-metric-learning
-Version: 0.4.1
+Version: 0.4.2
 Summary: OML is a PyTorch-based framework to train and validate the models producing high-quality embeddings.
 Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei
 Author-email: shabanoff.aleksei@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/OML-Team/open-metric-learning
 Project-URL: Bug Tracker, https://github.com/OML-Team/open-metric-learning/issues
@@ -303,24 +303,28 @@
 dataset_root = "mock_dataset/"
 df_train, _ = download_mock_dataset(dataset_root)
 
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False).train()
 optimizer = torch.optim.SGD(extractor.parameters(), lr=1e-6)
 
 train_dataset = DatasetWithLabels(df_train, dataset_root=dataset_root)
-criterion = TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner())
+criterion = TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner(), need_logs=True)
 sampler = BalanceSampler(train_dataset.get_labels(), n_labels=2, n_instances=2)
 train_loader = torch.utils.data.DataLoader(train_dataset, batch_sampler=sampler)
 
 for batch in tqdm(train_loader):
     embeddings = extractor(batch["input_tensors"])
     loss = criterion(embeddings, batch["labels"])
     loss.backward()
     optimizer.step()
     optimizer.zero_grad()
+
+    # info for logging: positive/negative distances, number of active triplets
+    print(criterion.last_logs)
+
 ```
 [comment]:vanilla-train-end
 </p>
 </details>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1kntDAIdIZ9L40jcndguLAb-XqmCFOgS5?usp=sharing)
 <details>
@@ -385,15 +389,15 @@
 Pipelines provide a way to run metric learning experiments via changing only the config file.
 All you need is to prepare your dataset in a required format.
 
 See [Pipelines](https://github.com/OML-Team/open-metric-learning/blob/main/pipelines/) folder for more details:
 * Feature extractor [pipeline](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction)
 * Retrieval postprocessor [pipeline](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/postprocessing) (re-ranking)
 
-## [Zoo](https://open-metric-learning.readthedocs.io/en/latest/postprocessing/zoo.html)
+## [Zoo](https://open-metric-learning.readthedocs.io/en/latest/feature_extraction/zoo.html)
 
 Below are the models trained with OML on 4 public datasets.
 All metrics below were obtained on the images with the sizes of **224 x 224**:
 
 |                      model                      | cmc1  |         dataset          |                                              weights                                              |                                                    experiment                                                     |
 |:-----------------------------------------------:|:-----:|:------------------------:|:-------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|
 | `ViTExtractor.from_pretrained("vits16_inshop")` | 0.921 |    DeepFashion Inshop    |    [link](https://drive.google.com/file/d/1niX-TC8cj6j369t7iU2baHQSVN3MVJbW/view?usp=sharing)     | [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_inshop) |
```

### Comparing `open-metric-learning-0.4.1/README.md` & `open-metric-learning-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -274,24 +274,28 @@
 dataset_root = "mock_dataset/"
 df_train, _ = download_mock_dataset(dataset_root)
 
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False).train()
 optimizer = torch.optim.SGD(extractor.parameters(), lr=1e-6)
 
 train_dataset = DatasetWithLabels(df_train, dataset_root=dataset_root)
-criterion = TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner())
+criterion = TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner(), need_logs=True)
 sampler = BalanceSampler(train_dataset.get_labels(), n_labels=2, n_instances=2)
 train_loader = torch.utils.data.DataLoader(train_dataset, batch_sampler=sampler)
 
 for batch in tqdm(train_loader):
     embeddings = extractor(batch["input_tensors"])
     loss = criterion(embeddings, batch["labels"])
     loss.backward()
     optimizer.step()
     optimizer.zero_grad()
+
+    # info for logging: positive/negative distances, number of active triplets
+    print(criterion.last_logs)
+
 ```
 [comment]:vanilla-train-end
 </p>
 </details>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1kntDAIdIZ9L40jcndguLAb-XqmCFOgS5?usp=sharing)
 <details>
@@ -356,15 +360,15 @@
 Pipelines provide a way to run metric learning experiments via changing only the config file.
 All you need is to prepare your dataset in a required format.
 
 See [Pipelines](https://github.com/OML-Team/open-metric-learning/blob/main/pipelines/) folder for more details:
 * Feature extractor [pipeline](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction)
 * Retrieval postprocessor [pipeline](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/postprocessing) (re-ranking)
 
-## [Zoo](https://open-metric-learning.readthedocs.io/en/latest/postprocessing/zoo.html)
+## [Zoo](https://open-metric-learning.readthedocs.io/en/latest/feature_extraction/zoo.html)
 
 Below are the models trained with OML on 4 public datasets.
 All metrics below were obtained on the images with the sizes of **224 x 224**:
 
 |                      model                      | cmc1  |         dataset          |                                              weights                                              |                                                    experiment                                                     |
 |:-----------------------------------------------:|:-----:|:------------------------:|:-------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|
 | `ViTExtractor.from_pretrained("vits16_inshop")` | 0.921 |    DeepFashion Inshop    |    [link](https://drive.google.com/file/d/1niX-TC8cj6j369t7iU2baHQSVN3MVJbW/view?usp=sharing)     | [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_inshop) |
```

### Comparing `open-metric-learning-0.4.1/oml/const.py` & `open-metric-learning-0.4.2/oml/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,7 +91,11 @@
 X2_KEY = "x2"
 Y1_KEY = "y1"
 Y2_KEY = "y2"
 INDEX_KEY = "idx"
 
 PAIR_1ST_KEY = "input_tensors_1"
 PAIR_2ND_KEY = "input_tensors_2"
+
+IMAGE_EXTENSIONS = ["jpg", "jpeg", "JPG", "JPEG", "png"]
+
+HYDRA_VERSION = "1.1"
```

### Comparing `open-metric-learning-0.4.1/oml/datasets/base.py` & `open-metric-learning-0.4.2/oml/datasets/base.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/datasets/pairs.py` & `open-metric-learning-0.4.2/oml/datasets/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/datasets/triplet.py` & `open-metric-learning-0.4.2/oml/datasets/triplet.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
             triplets: List of triplets
             im_root: Images directory
             transforms: Image transforms
             expand_ratio: Set expand_ratio > 0 to generate additional triplets.
                           We keep positive pairs, but generale negative ones randomly.
                           After this procedure you dataset's length will increased (1 + expand_ratio) times
             f_imread: Function to read image from disk
+            cache_size: Size of the dataset's cache
             index_key: Key to put samples' ids into the batches
 
         """
         assert expand_ratio >= 0
 
         warnings.warn("For now we do not keep this dataset up to date. Use it carefully.")
```

### Comparing `open-metric-learning-0.4.1/oml/ddp/patching.py` & `open-metric-learning-0.4.2/oml/ddp/patching.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/ddp/utils.py` & `open-metric-learning-0.4.2/oml/ddp/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/functional/label_smoothing.py` & `open-metric-learning-0.4.2/oml/functional/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/functional/losses.py` & `open-metric-learning-0.4.2/oml/functional/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/functional/metrics.py` & `open-metric-learning-0.4.2/oml/functional/metrics.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/inference/abstract.py` & `open-metric-learning-0.4.2/oml/inference/abstract.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/inference/flat.py` & `open-metric-learning-0.4.2/oml/inference/flat.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     return outputs
 
 
 def inference_on_dataframe(
     dataset_root: Union[Path, str],
     dataframe_name: str,
     extractor: IExtractor,
-    transforms_extraction: TTransforms,
+    transforms: TTransforms,
     output_cache_path: Optional[Union[str, Path]] = None,
     num_workers: int = 0,
     batch_size: int = 128,
     use_fp16: bool = False,
 ) -> Tuple[Tensor, Tensor, DataFrame, DataFrame]:
     df = pd.read_csv(Path(dataset_root) / dataframe_name)
 
@@ -68,15 +68,15 @@
     if (output_cache_path is not None) and Path(output_cache_path).is_file():
         embeddings = torch.load(output_cache_path, map_location="cpu")
         print("Embeddings have been loaded from the disk.")
     else:
         embeddings = inference_on_images(
             model=extractor,
             paths=df[PATHS_COLUMN],
-            transform=transforms_extraction,
+            transform=transforms,
             num_workers=num_workers,
             batch_size=batch_size,
             verbose=True,
             use_fp16=use_fp16,
             accumulate_on_cpu=True,
         )
         if output_cache_path is not None:
```

### Comparing `open-metric-learning-0.4.1/oml/inference/pairs.py` & `open-metric-learning-0.4.2/oml/inference/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/interfaces/criterions.py` & `open-metric-learning-0.4.2/oml/interfaces/criterions.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/interfaces/datasets.py` & `open-metric-learning-0.4.2/oml/interfaces/datasets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/interfaces/metrics.py` & `open-metric-learning-0.4.2/oml/interfaces/metrics.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/interfaces/miners.py` & `open-metric-learning-0.4.2/oml/interfaces/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/interfaces/models.py` & `open-metric-learning-0.4.2/oml/interfaces/models.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/interfaces/retrieval.py` & `open-metric-learning-0.4.2/oml/interfaces/retrieval.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/interfaces/samplers.py` & `open-metric-learning-0.4.2/oml/interfaces/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/lightning/callbacks/metric.py` & `open-metric-learning-0.4.2/oml/lightning/callbacks/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         log_images: bool = False,
         loader_idx: int = 0,
         samples_in_getitem: int = 1,
     ):
         """
         Args:
             metric: Metric
+            log_images: Set ``True`` if you want to have visual logging
             loader_idx: Idx of the loader to calculate metric for
             samples_in_getitem: Some of the datasets return several samples when calling ``__getitem__``,
                 so we need to handle it for the proper calculation. For most of the cases this value equals to 1,
                 but for the dataset which explicitly return triplets, this value must be equal to 3,
                 for a dataset of pairs it must be equal to 2.
 
         """
@@ -100,15 +101,15 @@
             log_str = f"{LOG_IMAGE_FOLDER}/{metric_log_str}"
             if isinstance(pl_module.logger, NeptuneLogger):
                 pl_module.logger.experiment[log_str].log(File.as_image(fig))
             elif isinstance(pl_module.logger, TensorBoardLogger):
                 fig.canvas.draw()
                 data = np.frombuffer(fig.canvas.tostring_rgb(), dtype=np.uint8)
                 data = data.reshape(fig.canvas.get_width_height()[::-1] + (3,))
-                pl_module.logger.experiment.add_image(log_str, np.swapaxes(data, 0, 2), pl_module.current_epoch)
+                pl_module.logger.experiment.add_image(log_str, np.transpose(data, (2, 0, 1)), pl_module.current_epoch)
             else:
                 raise ValueError(f"Logging with {type(pl_module.logger)} is not supported yet.")
 
     def on_validation_epoch_end(self, trainer: pl.Trainer, pl_module: pl.LightningModule) -> None:
         self._ready_to_accumulate = False
         if self._collected_samples != self._expected_samples:
             self._raise_computation_error()
```

### Comparing `open-metric-learning-0.4.1/oml/lightning/modules/ddp.py` & `open-metric-learning-0.4.2/oml/lightning/modules/ddp.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/lightning/modules/extractor.py` & `open-metric-learning-0.4.2/oml/lightning/modules/extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     This is a base module to train your model with Lightning.
 
     """
 
     def __init__(
         self,
         extractor: IExtractor,
-        criterion: nn.Module,
-        optimizer: torch.optim.Optimizer,
+        criterion: Optional[nn.Module] = None,
+        optimizer: Optional[torch.optim.Optimizer] = None,
         scheduler: Optional[_LRScheduler] = None,
         scheduler_interval: str = "step",
         scheduler_frequency: int = 1,
         input_tensors_key: str = INPUT_TENSORS_KEY,
         labels_key: str = LABELS_KEY,
         embeddings_key: str = EMBEDDINGS_KEY,
         scheduler_monitor_metric: Optional[str] = None,
@@ -89,14 +89,17 @@
 
         return loss
 
     def validation_step(self, batch: Dict[str, Any], batch_idx: int, *_: Any) -> Dict[str, Any]:
         embeddings = self.model.extract(batch[self.input_tensors_key])
         return {**batch, **{self.embeddings_key: embeddings}}
 
+    def predict_step(self, batch: Dict[str, Any], batch_idx: int, *_: Any) -> Dict[str, Any]:
+        return self.validation_step(batch, batch_idx)
+
     def configure_optimizers(self) -> Any:
         if self.scheduler is None:
             return self.optimizer
         else:
             scheduler = {
                 "scheduler": self.scheduler,
                 "interval": self.scheduler_interval,
```

### Comparing `open-metric-learning-0.4.1/oml/lightning/modules/pairwise_postprocessing.py` & `open-metric-learning-0.4.2/oml/lightning/modules/pairwise_postprocessing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/lightning/pipelines/parser.py` & `open-metric-learning-0.4.2/oml/lightning/pipelines/parser.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/lightning/pipelines/train.py` & `open-metric-learning-0.4.2/oml/lightning/pipelines/train.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/lightning/pipelines/train_postprocessor.py` & `open-metric-learning-0.4.2/oml/lightning/pipelines/train_postprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         cache_file = None
 
     emb_train, emb_val, df_train, df_val = inference_on_dataframe(
         extractor=extractor,
         dataset_root=cfg["dataset_root"],
         output_cache_path=cache_file,
         dataframe_name=cfg["dataframe_name"],
-        transforms_extraction=get_transforms_by_cfg(cfg["transforms_extraction"]),
+        transforms=get_transforms_by_cfg(cfg["transforms_extraction"]),
         num_workers=cfg["num_workers"],
         batch_size=cfg["batch_size_inference"],
         use_fp16=int(cfg.get("precision", 32)) == 16,
     )
 
     train_dataset = DatasetWithLabels(
         df=df_train,
```

### Comparing `open-metric-learning-0.4.1/oml/lightning/pipelines/validate.py` & `open-metric-learning-0.4.2/oml/lightning/pipelines/validate.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/losses/arcface.py` & `open-metric-learning-0.4.2/oml/losses/arcface.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/losses/surrogate_precision.py` & `open-metric-learning-0.4.2/oml/losses/surrogate_precision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/losses/triplet.py` & `open-metric-learning-0.4.2/oml/losses/triplet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/metrics/accumulation.py` & `open-metric-learning-0.4.2/oml/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/metrics/embeddings.py` & `open-metric-learning-0.4.2/oml/metrics/embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
             print("\nMetrics:")
             pprint(metric_to_return)
 
         return metric_to_return  # type: ignore
 
     def visualize(self) -> Tuple[Collection[plt.Figure], Collection[str]]:
         """
-        Visualize worst queries by metrics.
+        Visualize worst queries by all the available metrics.
         """
         metrics_flat = flatten_dict(self.metrics, ignored_keys=self.metrics_to_exclude_from_visualization)
         figures = []
         titles = []
         for metric_name in metrics_flat:
             if self.visualize_only_main_category and not metric_name.startswith(OVERALL_CATEGORIES_KEY):
                 continue
```

### Comparing `open-metric-learning-0.4.1/oml/metrics/triplets.py` & `open-metric-learning-0.4.2/oml/metrics/triplets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/miners/cross_batch.py` & `open-metric-learning-0.4.2/oml/miners/cross_batch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/miners/inbatch_all_tri.py` & `open-metric-learning-0.4.2/oml/miners/inbatch_all_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/miners/inbatch_hard_cluster.py` & `open-metric-learning-0.4.2/oml/miners/inbatch_hard_cluster.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/miners/inbatch_hard_tri.py` & `open-metric-learning-0.4.2/oml/miners/inbatch_hard_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/miners/inbatch_nhard_tri.py` & `open-metric-learning-0.4.2/oml/miners/inbatch_nhard_tri.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     ) -> TTripletsIds:
         """
         This method samples the hard triplets inside the batch based on distance between features.
 
         Args:
             features: Features with the shape of ``[batch_size, feature_size]``
             labels: Labels with the size of ``batch_size``
+            *_: Anything here will be ignored
             ignore_anchor_mask: Parameter allows you to specify the ids of features that cannot be used as anchors. Can
             be useful with memory banks to create triplets in which at least one vector will have gradients.
 
         Returns:
             The batch of the triplets in the order below:
             ``(anchor, positive, negative)``
         """
```

### Comparing `open-metric-learning-0.4.1/oml/miners/miner_with_bank.py` & `open-metric-learning-0.4.2/oml/miners/miner_with_bank.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/miners/pairs.py` & `open-metric-learning-0.4.2/oml/miners/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/models/meta/projection.py` & `open-metric-learning-0.4.2/oml/models/meta/projection.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/models/meta/siamese.py` & `open-metric-learning-0.4.2/oml/models/meta/siamese.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/models/pooling.py` & `open-metric-learning-0.4.2/oml/models/pooling.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/models/resnet.py` & `open-metric-learning-0.4.2/oml/models/resnet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/models/utils.py` & `open-metric-learning-0.4.2/oml/models/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/models/vit/clip.py` & `open-metric-learning-0.4.2/oml/models/vit/clip.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/models/vit/hubconf.py` & `open-metric-learning-0.4.2/oml/models/vit/hubconf.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/models/vit/vision_transformer.py` & `open-metric-learning-0.4.2/oml/models/vit/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/models/vit/vision_transformer_clip.py` & `open-metric-learning-0.4.2/oml/models/vit/vision_transformer_clip.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/models/vit/vit.py` & `open-metric-learning-0.4.2/oml/models/vit/vit.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/registry/__init__.py` & `open-metric-learning-0.4.2/oml/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/registry/losses.py` & `open-metric-learning-0.4.2/oml/registry/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/registry/miners.py` & `open-metric-learning-0.4.2/oml/registry/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/registry/models.py` & `open-metric-learning-0.4.2/oml/registry/models.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/registry/optimizers.py` & `open-metric-learning-0.4.2/oml/registry/optimizers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/registry/postprocessors.py` & `open-metric-learning-0.4.2/oml/registry/postprocessors.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/registry/samplers.py` & `open-metric-learning-0.4.2/oml/registry/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/registry/schedulers.py` & `open-metric-learning-0.4.2/oml/registry/schedulers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/registry/transforms.py` & `open-metric-learning-0.4.2/oml/registry/transforms.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/retrieval/postprocessors/pairwise.py` & `open-metric-learning-0.4.2/oml/retrieval/postprocessors/pairwise.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/samplers/balance.py` & `open-metric-learning-0.4.2/oml/samplers/balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/samplers/category_balance.py` & `open-metric-learning-0.4.2/oml/samplers/category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/samplers/distinct_category_balance.py` & `open-metric-learning-0.4.2/oml/samplers/distinct_category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/transforms/images/albumentations.py` & `open-metric-learning-0.4.2/oml/transforms/images/albumentations.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/transforms/images/torchvision.py` & `open-metric-learning-0.4.2/oml/transforms/images/torchvision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/utils/dataframe_format.py` & `open-metric-learning-0.4.2/oml/utils/dataframe_format.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/utils/download_mock_dataset.py` & `open-metric-learning-0.4.2/oml/utils/download_mock_dataset.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/utils/images/images.py` & `open-metric-learning-0.4.2/oml/utils/images/images.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import multiprocessing as mp
+from functools import partial
 from io import BytesIO
 from pathlib import Path
-from typing import Callable, Union
+from typing import Callable, List, Optional, Union
+
+from tqdm import tqdm
 
 try:
     from albumentations.augmentations.functional import pad
 except (AttributeError, ModuleNotFoundError, ImportError):
     from albumentations.augmentations.geometric.functional import pad
 
 import cv2
@@ -94,14 +98,32 @@
     return img
 
 
 def square_pad(img: np.ndarray) -> np.ndarray:
     return pad(img, min_height=max(img.shape), min_width=max(img.shape), border_mode=0, value=PAD_COLOR)
 
 
+def try_to_open_image(im_path: Path, f_imread: TImReader) -> Optional[str]:
+    try:
+        _ = f_imread(im_path)
+        return None
+    except Exception:
+        return str(im_path)
+
+
+def find_broken_images(images_list: List[Path], f_imread: TImReader, num_processes: int = 10) -> List[str]:
+    try_to_open_image_ = partial(try_to_open_image, f_imread=f_imread)
+
+    with mp.Pool(processes=num_processes) as p:
+        results = list(tqdm(p.imap(try_to_open_image_, images_list), total=len(images_list)))
+
+    results = list(filter(lambda x: x is not None, results))
+    return results
+
+
 __all__ = [
     "TImage",
     "TImReader",
     "tensor_to_numpy_image",
     "imread_cv2",
     "imread_pillow",
     "draw_bbox",
```

### Comparing `open-metric-learning-0.4.1/oml/utils/images/images_resize.py` & `open-metric-learning-0.4.2/oml/utils/images/images_resize.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/utils/io.py` & `open-metric-learning-0.4.2/oml/utils/io.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/utils/misc.py` & `open-metric-learning-0.4.2/oml/utils/misc.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/utils/misc_torch.py` & `open-metric-learning-0.4.2/oml/utils/misc_torch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/oml/utils/remote_storage.py` & `open-metric-learning-0.4.2/oml/utils/remote_storage.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/open_metric_learning.egg-info/PKG-INFO` & `open-metric-learning-0.4.2/open_metric_learning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-metric-learning
-Version: 0.4.1
+Version: 0.4.2
 Summary: OML is a PyTorch-based framework to train and validate the models producing high-quality embeddings.
 Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei
 Author-email: shabanoff.aleksei@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/OML-Team/open-metric-learning
 Project-URL: Bug Tracker, https://github.com/OML-Team/open-metric-learning/issues
@@ -303,24 +303,28 @@
 dataset_root = "mock_dataset/"
 df_train, _ = download_mock_dataset(dataset_root)
 
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False).train()
 optimizer = torch.optim.SGD(extractor.parameters(), lr=1e-6)
 
 train_dataset = DatasetWithLabels(df_train, dataset_root=dataset_root)
-criterion = TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner())
+criterion = TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner(), need_logs=True)
 sampler = BalanceSampler(train_dataset.get_labels(), n_labels=2, n_instances=2)
 train_loader = torch.utils.data.DataLoader(train_dataset, batch_sampler=sampler)
 
 for batch in tqdm(train_loader):
     embeddings = extractor(batch["input_tensors"])
     loss = criterion(embeddings, batch["labels"])
     loss.backward()
     optimizer.step()
     optimizer.zero_grad()
+
+    # info for logging: positive/negative distances, number of active triplets
+    print(criterion.last_logs)
+
 ```
 [comment]:vanilla-train-end
 </p>
 </details>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1kntDAIdIZ9L40jcndguLAb-XqmCFOgS5?usp=sharing)
 <details>
@@ -385,15 +389,15 @@
 Pipelines provide a way to run metric learning experiments via changing only the config file.
 All you need is to prepare your dataset in a required format.
 
 See [Pipelines](https://github.com/OML-Team/open-metric-learning/blob/main/pipelines/) folder for more details:
 * Feature extractor [pipeline](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction)
 * Retrieval postprocessor [pipeline](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/postprocessing) (re-ranking)
 
-## [Zoo](https://open-metric-learning.readthedocs.io/en/latest/postprocessing/zoo.html)
+## [Zoo](https://open-metric-learning.readthedocs.io/en/latest/feature_extraction/zoo.html)
 
 Below are the models trained with OML on 4 public datasets.
 All metrics below were obtained on the images with the sizes of **224 x 224**:
 
 |                      model                      | cmc1  |         dataset          |                                              weights                                              |                                                    experiment                                                     |
 |:-----------------------------------------------:|:-----:|:------------------------:|:-------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|
 | `ViTExtractor.from_pretrained("vits16_inshop")` | 0.921 |    DeepFashion Inshop    |    [link](https://drive.google.com/file/d/1niX-TC8cj6j369t7iU2baHQSVN3MVJbW/view?usp=sharing)     | [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_inshop) |
```

### Comparing `open-metric-learning-0.4.1/open_metric_learning.egg-info/SOURCES.txt` & `open-metric-learning-0.4.2/open_metric_learning.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 oml/__init__.py
 oml/const.py
-oml/exceptions.py
 oml/configs/__init__.py
 oml/configs/criterion/arcface.yaml
 oml/configs/criterion/mlp_arcface.yaml
 oml/configs/criterion/surrogate_precision.yaml
 oml/configs/criterion/triplet.yaml
 oml/configs/criterion/triplet_plain.yaml
 oml/configs/criterion/triplet_with_miner.yaml
@@ -88,14 +87,15 @@
 oml/lightning/callbacks/metric.py
 oml/lightning/modules/__init__.py
 oml/lightning/modules/ddp.py
 oml/lightning/modules/extractor.py
 oml/lightning/modules/pairwise_postprocessing.py
 oml/lightning/pipelines/__init__.py
 oml/lightning/pipelines/parser.py
+oml/lightning/pipelines/predict.py
 oml/lightning/pipelines/train.py
 oml/lightning/pipelines/train_postprocessor.py
 oml/lightning/pipelines/validate.py
 oml/losses/__init__.py
 oml/losses/arcface.py
 oml/losses/surrogate_precision.py
 oml/losses/triplet.py
@@ -157,8 +157,9 @@
 oml/utils/images/images_resize.py
 open_metric_learning.egg-info/PKG-INFO
 open_metric_learning.egg-info/SOURCES.txt
 open_metric_learning.egg-info/dependency_links.txt
 open_metric_learning.egg-info/requires.txt
 open_metric_learning.egg-info/top_level.txt
 tests/test_build_readme.py
-tests/test_imports.py
+tests/test_imports.py
+tests/test_outdated_docs.py
```

### Comparing `open-metric-learning-0.4.1/setup.py` & `open-metric-learning-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/tests/test_build_readme.py` & `open-metric-learning-0.4.2/tests/test_build_readme.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.1/tests/test_imports.py` & `open-metric-learning-0.4.2/tests/test_imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import pytest
 
 from oml.const import PROJECT_ROOT
 
 LIBS_TO_IGNORE = ["torch_xla"]
 
-NEED_TO_TEST_NOTEBOOKS = False
+NEED_TO_TEST_NOTEBOOKS = True
 
 
 def get_imports_from_files() -> List[Tuple[str, str]]:
     files = get_files_with_imports()
 
     file_import_pairs = []
```

