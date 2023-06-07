# Comparing `tmp/molgraph-0.3.5.tar.gz` & `tmp/molgraph-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.3.5.tar", last modified: Wed Jun  7 12:36:48 2023, max compression
+gzip compressed data, was "molgraph-0.3.6.tar", last modified: Wed Jun  7 13:26:14 2023, max compression
```

## Comparing `molgraph-0.3.5.tar` & `molgraph-0.3.6.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.446012 molgraph-0.3.5/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.3.5/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     3842 2023-06-07 12:36:48.442012 molgraph-0.3.5/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-05-26 15:32:21.000000 molgraph-0.3.5/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.438012 molgraph-0.3.5/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      408 2022-09-20 11:35:03.000000 molgraph-0.3.5/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      954 2022-09-20 11:35:03.000000 molgraph-0.3.5/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.438012 molgraph-0.3.5/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.3.5/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.438012 molgraph-0.3.5/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.3.5/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.3.5/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.3.5/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.3.5/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2022-09-20 11:35:03.000000 molgraph-0.3.5/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.3.5/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.3.5/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.3.5/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.3.5/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21456 2023-04-12 17:28:19.000000 molgraph-0.3.5/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.3.5/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.3.5/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.438012 molgraph-0.3.5/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3823 2023-06-06 20:54:37.000000 molgraph-0.3.5/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.438012 molgraph-0.3.5/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.3.5/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12448 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11175 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9188 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11222 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10436 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14857 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/attentional/gt_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13035 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/base.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.438012 molgraph-0.3.5/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.3.5/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9825 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9663 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10612 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.3.5/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.3.5/molgraph/layers/geometric/_radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9364 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10190 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/geometric/gcf_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.3.5/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21742 2023-06-06 14:24:00.000000 molgraph-0.3.5/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15527 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/message_passing/mpnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6419 2023-04-17 15:25:58.000000 molgraph-0.3.5/molgraph/layers/ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.3.5/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10714 2022-09-14 10:36:59.000000 molgraph-0.3.5/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.3.5/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-07 12:34:11.000000 molgraph-0.3.5/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2022-08-18 17:05:41.000000 molgraph-0.3.5/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-09-20 11:35:03.000000 molgraph-0.3.5/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.3.5/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11080 2023-06-06 21:11:15.000000 molgraph-0.3.5/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4557 2023-06-06 20:54:37.000000 molgraph-0.3.5/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9592 2023-06-06 21:11:15.000000 molgraph-0.3.5/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4234 2023-06-06 21:11:15.000000 molgraph-0.3.5/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11858 2023-06-06 21:11:15.000000 molgraph-0.3.5/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6753 2023-06-06 21:11:15.000000 molgraph-0.3.5/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20494 2023-06-06 21:11:15.000000 molgraph-0.3.5/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.3.5/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6710 2023-05-26 15:46:41.000000 molgraph-0.3.5/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4613 2023-04-14 12:58:07.000000 molgraph-0.3.5/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3296 2022-09-20 11:35:03.000000 molgraph-0.3.5/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6250 2022-09-14 11:22:14.000000 molgraph-0.3.5/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5418 2022-09-14 10:36:59.000000 molgraph-0.3.5/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.3.5/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2192 2022-06-01 11:22:01.000000 molgraph-0.3.5/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5182 2022-08-15 09:20:55.000000 molgraph-0.3.5/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.3.5/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2022-06-01 11:25:29.000000 molgraph-0.3.5/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-06-01 11:21:46.000000 molgraph-0.3.5/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.3.5/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7883 2023-04-14 12:58:07.000000 molgraph-0.3.5/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7065 2023-04-14 12:58:07.000000 molgraph-0.3.5/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.3.5/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.3.5/molgraph/models/interpretability/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.3.5/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2022-09-20 11:35:03.000000 molgraph-0.3.5/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6831 2023-04-14 12:58:07.000000 molgraph-0.3.5/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:32.000000 molgraph-0.3.5/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:46.000000 molgraph-0.3.5/molgraph/models/pretraining/attribute_masking.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.442012 molgraph-0.3.5/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.3.5/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.3.5/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.3.5/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    39597 2023-06-06 14:24:00.000000 molgraph-0.3.5/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 12:36:48.438012 molgraph-0.3.5/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3842 2023-06-07 12:36:48.000000 molgraph-0.3.5/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3234 2023-06-07 12:36:48.000000 molgraph-0.3.5/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-07 12:36:48.000000 molgraph-0.3.5/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-06-07 12:36:48.000000 molgraph-0.3.5/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-06-07 12:36:48.000000 molgraph-0.3.5/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-07 12:36:48.446012 molgraph-0.3.5/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-04-06 16:32:34.000000 molgraph-0.3.5/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.3.6/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3842 2023-06-07 13:26:14.190172 molgraph-0.3.6/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-05-26 15:32:21.000000 molgraph-0.3.6/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.182171 molgraph-0.3.6/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      408 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      954 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-06-07 13:25:59.000000 molgraph-0.3.6/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.3.6/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.3.6/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.3.6/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.3.6/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.3.6/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.3.6/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21456 2023-04-12 17:28:19.000000 molgraph-0.3.6/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.3.6/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.3.6/molgraph/chemistry/vis.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3823 2023-06-06 20:54:37.000000 molgraph-0.3.6/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.3.6/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12448 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11175 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9188 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11222 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10436 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14857 2023-06-07 13:20:34.000000 molgraph-0.3.6/molgraph/layers/attentional/gt_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13283 2023-06-07 13:25:59.000000 molgraph-0.3.6/molgraph/layers/base.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.3.6/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9825 2023-06-07 12:59:58.000000 molgraph-0.3.6/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9663 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10612 2023-06-07 13:00:51.000000 molgraph-0.3.6/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.3.6/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.3.6/molgraph/layers/geometric/_radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9364 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10190 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/geometric/gcf_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.3.6/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22003 2023-06-07 13:25:59.000000 molgraph-0.3.6/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15527 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/message_passing/mpnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6419 2023-04-17 15:25:58.000000 molgraph-0.3.6/molgraph/layers/ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.3.6/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10713 2023-06-07 13:25:59.000000 molgraph-0.3.6/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.3.6/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2022-08-18 17:05:41.000000 molgraph-0.3.6/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.3.6/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11080 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4557 2023-06-06 20:54:37.000000 molgraph-0.3.6/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9592 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4234 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11858 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6753 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20494 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.3.6/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6710 2023-05-26 15:46:41.000000 molgraph-0.3.6/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4613 2023-04-14 12:58:07.000000 molgraph-0.3.6/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3296 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6250 2022-09-14 11:22:14.000000 molgraph-0.3.6/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5418 2022-09-14 10:36:59.000000 molgraph-0.3.6/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.3.6/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2192 2022-06-01 11:22:01.000000 molgraph-0.3.6/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5182 2022-08-15 09:20:55.000000 molgraph-0.3.6/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.3.6/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2022-06-01 11:25:29.000000 molgraph-0.3.6/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-06-01 11:21:46.000000 molgraph-0.3.6/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.3.6/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7883 2023-04-14 12:58:07.000000 molgraph-0.3.6/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7065 2023-06-07 12:49:03.000000 molgraph-0.3.6/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.3.6/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.3.6/molgraph/models/interpretability/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6831 2023-04-14 12:58:07.000000 molgraph-0.3.6/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:32.000000 molgraph-0.3.6/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:46.000000 molgraph-0.3.6/molgraph/models/pretraining/attribute_masking.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.3.6/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.3.6/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.3.6/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    39597 2023-06-06 14:24:00.000000 molgraph-0.3.6/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.182171 molgraph-0.3.6/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3842 2023-06-07 13:26:14.000000 molgraph-0.3.6/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3234 2023-06-07 13:26:14.000000 molgraph-0.3.6/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-07 13:26:14.000000 molgraph-0.3.6/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-06-07 13:26:14.000000 molgraph-0.3.6/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-06-07 13:26:14.000000 molgraph-0.3.6/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-07 13:26:14.190172 molgraph-0.3.6/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-04-06 16:32:34.000000 molgraph-0.3.6/setup.py
```

### Comparing `molgraph-0.3.5/LICENSE` & `molgraph-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/PKG-INFO` & `molgraph-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.3.5
+Version: 0.3.6
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.3.5/README.md` & `molgraph-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/_filter_warnings.py` & `molgraph-0.3.6/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/__init__.py` & `molgraph-0.3.6/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.3.6/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.3.6/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.3.6/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.3.6/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/conformer_generator.py` & `molgraph-0.3.6/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/conformer_utils.py` & `molgraph-0.3.6/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/encoders.py` & `molgraph-0.3.6/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/features.py` & `molgraph-0.3.6/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.3.6/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/ops.py` & `molgraph-0.3.6/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/chemistry/vis.py` & `molgraph-0.3.6/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/__init__.py` & `molgraph-0.3.6/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.3.6/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.3.6/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.3.6/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.3.6/molgraph/layers/attentional/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.3.6/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.3.6/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/base.py` & `molgraph-0.3.6/molgraph/layers/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -220,61 +220,75 @@
                 edge_feature += edge_feature_residual
             if self._dropout:
                 edge_feature = self._edge_dropout(edge_feature)
             tensor_update = tensor_update.update({'edge_feature': edge_feature})
 
         return tensor_update
 
+    def get_common_kwargs(self):
+        common_kwargs = dict(
+            kernel_regularizer=self._kernel_regularizer,
+            bias_regularizer=self._bias_regularizer,
+            activity_regularizer=self._activity_regularizer,
+            kernel_constraint=self._kernel_constraint,
+            bias_constraint=self._bias_constraint,
+        )
+        kernel_initializer = self._kernel_initializer.__class__.from_config(
+            self._kernel_initializer.get_config()
+        )
+        bias_initializer = self._bias_initializer.__class__.from_config(
+            self._bias_initializer.get_config()
+        )
+        common_kwargs["kernel_initializer"] = kernel_initializer
+        common_kwargs["bias_initializer"] = bias_initializer
+        return common_kwargs
+    
     def get_kernel(
         self,
         shape: Shape,
         dtype: DType = tf.float32,
         name: str = 'kernel'
     ) -> tf.Variable:
+        common_kwargs = self.get_common_kwargs()
         return self.add_weight(
             name=name,
             shape=shape,
             dtype=dtype,
-            initializer=self._kernel_initializer,
-            regularizer=self._kernel_regularizer,
-            constraint=self._kernel_constraint,
+            initializer=common_kwargs['kernel_initializer'],
+            regularizer=common_kwargs['kernel_regularizer'],
+            constraint=common_kwargs['kernel_constraint'],
             trainable=True
         )
 
     def get_bias(self,
         shape: Shape,
         dtype: DType = tf.float32,
         name: str = 'bias'
     ) -> tf.Variable:
+        common_kwargs = self.get_common_kwargs()
         return self.add_weight(
             name=name,
             shape=shape,
             dtype=dtype,
-            initializer=self._bias_initializer,
-            regularizer=self._bias_regularizer,
-            constraint=self._bias_constraint,
+            initializer=common_kwargs['bias_initializer'],
+            regularizer=common_kwargs['bias_regularizer'],
+            constraint=common_kwargs['bias_constraint'],
             trainable=True
         )
 
     def get_dense(
         self,
         units: int,
         activation: Activation = None,
     ) -> layers.Dense:
         return layers.Dense(
             units,
             activation=activation,
             use_bias=self._use_bias,
-            kernel_initializer=self._kernel_initializer,
-            bias_initializer=self._bias_initializer,
-            kernel_regularizer=self._kernel_regularizer,
-            bias_regularizer=self._bias_regularizer,
-            activity_regularizer=self._activity_regularizer,
-            kernel_constraint=self._kernel_constraint,
-            bias_constraint=self._bias_constraint)
+            **self.get_common_kwargs())
 
     def get_einsum_dense(
         self,
         equation: str,
         output_shape: Shape,
         activation: Activation = None,
     ) -> layers.experimental.EinsumDense:
@@ -287,21 +301,15 @@
             bias_axes = None
 
         return layers.experimental.EinsumDense(
             equation,
             output_shape,
             activation=activation,
             bias_axes=bias_axes,
-            kernel_initializer=self._kernel_initializer,
-            bias_initializer=self._bias_initializer,
-            kernel_regularizer=self._kernel_regularizer,
-            bias_regularizer=self._bias_regularizer,
-            activity_regularizer=self._activity_regularizer,
-            kernel_constraint=self._kernel_constraint,
-            bias_constraint=self._bias_constraint)
+            **self.get_common_kwargs())
 
     def compute_output_shape(
         self,
         input_shape: Shape
     ) -> tf.TensorShape:
         inner_dim = self.units
         if getattr(self, 'merge_mode', None) == 'concat':
```

### Comparing `molgraph-0.3.5/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.3.6/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.3.6/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.3.6/molgraph/layers/convolutional/gin_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.3.6/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/geometric/_radial_basis.py` & `molgraph-0.3.6/molgraph/layers/geometric/_radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.3.6/molgraph/layers/geometric/dtnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.3.6/molgraph/layers/geometric/gcf_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.3.6/molgraph/layers/message_passing/edge_conv.py`

 * *Files 3% similar despite different names*

```diff
@@ -310,15 +310,15 @@
             'activation':
                 activations.serialize(self.activation),
             'recurrent_activation':
                 activations.serialize(self.recurrent_activation),
             'use_bias':
                 self.use_bias,
             'kernel_initializer':
-                initializers.serialize(self.kernel_initializer ),
+                initializers.serialize(self.kernel_initializer),
             'bias_initializer':
                 initializers.serialize(self.bias_initializer),
             'recurrent_initializer':
                 initializers.serialize(self.recurrent_initializer),
             'kernel_regularizer':
                 regularizers.serialize(self.kernel_regularizer),
             'bias_regularizer':
@@ -354,30 +354,34 @@
         return input_shape
     
     def _get_dense(self, units):
         return keras.layers.Dense(
             units=units, 
             activation=self.activation,
             use_bias=self.use_bias,
-            kernel_initializer=self.kernel_initializer ,
-            bias_initializer=self.bias_initializer,
+            kernel_initializer=self.kernel_initializer.from_config(
+                self.kernel_initializer.get_config()),
+            bias_initializer=self.bias_initializer.from_config(
+                self.bias_initializer.get_config()),
             kernel_regularizer=self.kernel_regularizer,
             bias_regularizer=self.bias_regularizer,
             activity_regularizer=self.activity_regularizer,
             kernel_constraint=self.kernel_constraint,
             bias_constraint=self.bias_constraint)
     
     def _get_gru(self, units):
         return keras.layers.GRUCell(
             units=units, 
             activation=self.activation,
             recurrent_activation=self.recurrent_activation,
             use_bias=self.use_bias,
-            kernel_initializer=self.kernel_initializer ,
-            bias_initializer=self.bias_initializer,
+            kernel_initializer=self.kernel_initializer.from_config(
+                self.kernel_initializer.get_config()),
+            bias_initializer=self.bias_initializer.from_config(
+                self.bias_initializer.get_config()),
             recurrent_initializer=self.recurrent_initializer,
             kernel_regularizer=self.kernel_regularizer,
             bias_regularizer=self.bias_regularizer,
             recurrent_regularizer=self.recurrent_regularizer,
             kernel_constraint=self.kernel_constraint,
             bias_constraint=self.bias_constraint,
             recurrent_constraint=self.recurrent_constraint)
```

### Comparing `molgraph-0.3.5/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.3.6/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/ops.py` & `molgraph-0.3.6/molgraph/layers/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.3.6/molgraph/layers/positional_encoding/laplacian.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         base_config = super().get_config()
         config = {
             'dim': self.dim,
             'activation': activations.serialize(self.activation),
             'use_bias': self.use_bias,
             'kernel_initializer': initializers.serialize(self.kernel_initializer),
             'bias_initializer': initializers.serialize(self.bias_initializer),
-            'kernel_regularizer': regularizers.serialize(sself.kernel_regularizer),
+            'kernel_regularizer': regularizers.serialize(self.kernel_regularizer),
             'bias_regularizer': regularizers.serialize(self.bias_regularizer),
             'activity_regularizer': regularizers.serialize(self.activity_regularizer),
             'kernel_constraint': constraints.serialize(self.kernel_constraint),
             'bias_constraint': constraints.serialize(self.bias_constraint),
             'node_feature_shape': self._node_feature_shape,
             'positional_encoding_shape': self._positional_encoding_shape,
         }
```

### Comparing `molgraph-0.3.5/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.3.6/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.3.6/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.3.6/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.3.6/molgraph/layers/preprocessing/center_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.3.6/molgraph/layers/preprocessing/dropout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.3.6/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/preprocessing/masking.py` & `molgraph-0.3.6/molgraph/layers/preprocessing/masking.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.3.6/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/preprocessing/projection.py` & `molgraph-0.3.6/molgraph/layers/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.3.6/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.3.6/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/readout/node_readout.py` & `molgraph-0.3.6/molgraph/layers/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/readout/segment_pool.py` & `molgraph-0.3.6/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/readout/set_gather.py` & `molgraph-0.3.6/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.3.6/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/losses/link_losses.py` & `molgraph-0.3.6/molgraph/losses/link_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/losses/masked_losses.py` & `molgraph-0.3.6/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/metrics/masked_metrics.py` & `molgraph-0.3.6/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/metrics/mean_relative_error.py` & `molgraph-0.3.6/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/models/dgin.py` & `molgraph-0.3.6/molgraph/models/dgin.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/models/dmpnn.py` & `molgraph-0.3.6/molgraph/models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.3.6/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/models/interpretability/saliency.py` & `molgraph-0.3.6/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/models/mpnn.py` & `molgraph-0.3.6/molgraph/models/mpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/tensors/_graph_tensor.py` & `molgraph-0.3.6/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.3.6/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph/tensors/graph_tensor.py` & `molgraph-0.3.6/molgraph/tensors/graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/molgraph.egg-info/PKG-INFO` & `molgraph-0.3.6/molgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.3.5
+Version: 0.3.6
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.3.5/molgraph.egg-info/SOURCES.txt` & `molgraph-0.3.6/molgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.5/setup.py` & `molgraph-0.3.6/setup.py`

 * *Files identical despite different names*

