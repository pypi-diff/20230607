# Comparing `tmp/lightly-1.4.6.tar.gz` & `tmp/lightly-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightly-1.4.6.tar", last modified: Tue May 23 16:32:10 2023, max compression
+gzip compressed data, was "lightly-1.4.7.tar", last modified: Wed Jun  7 08:25:57 2023, max compression
```

## Comparing `lightly-1.4.6.tar` & `lightly-1.4.7.tar`

### file list

```diff
@@ -1,410 +1,404 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.647479 lightly-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-23 16:31:57.000000 lightly-1.4.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-23 16:31:57.000000 lightly-1.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-23 16:32:10.647479 lightly-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-05-23 16:31:57.000000 lightly-1.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.611479 lightly-1.4.6/lightly/
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/active_learning/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/active_learning/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/agents/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/active_learning/config/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/config/selection_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/active_learning/scorers/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/keypoint_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/active_learning/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/utils/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/utils/keypoint_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/utils/object_detection_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/api/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_collaboration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_compute_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    29042 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_datasources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_download_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_upload_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_upload_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_upload_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/bitmask.py
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/prediction_singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/swagger_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/swagger_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/version_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/_cli_simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/config/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/crop_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/download_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/embed_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/lightly_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/train_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/upload_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/data/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/_image_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25874 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/_video.py
--rw-r--r--   0 runner    (1001) docker     (123)    49756 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/lightly_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/multi_view_collate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/embedding/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/embedding/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/embedding/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/dcl_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/dino_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/hypersphere_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/msn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/negative_cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/ntx_ent_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/pmsn_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/loss/regularizer/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/regularizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/regularizer/co2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/swav_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/sym_neg_cos_sim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/tico_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/vicreg_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/vicregl_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/_momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/barlowtwins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/byol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/moco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.623479 lightly-1.4.6/lightly/models/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23563 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/modules/heads.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/modules/masked_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/modules/nn_memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/nnclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/simsiam.py
--rw-r--r--   0 runner    (1001) docker     (123)    18480 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.611479 lightly-1.4.6/lightly/openapi_generated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.623479 lightly-1.4.6/lightly/openapi_generated/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    25152 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.623479 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/collaboration_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    48008 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    78621 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/datasources_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   160419 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/docker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/embeddings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/mappings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38782 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/predictions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/quota_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52413 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/samples_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/samplings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/scores_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    97324 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/versioning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.643479 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    23521 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/access_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/api_error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/api_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/async_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/category_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/category_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_entity_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/crop_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16339 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_name_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_license_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_task_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/file_name_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/file_output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/general_job_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_result_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/jobs_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/mongo_object_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/object_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/path_safe_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/redirected_read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/s3_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_input_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/task_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/task_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/team_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/team_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/version_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/video_frame_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.643479 lightly-1.4.6/lightly/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/dino_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/fast_siam_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/image_grid_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/jigsaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/mae_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/moco_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/msn_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/multi_crop_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/multi_view_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/pirl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/random_crop_and_flip_with_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/simclr_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/simsiam_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/smog_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/swav_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/vicreg_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/vicregl_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.643479 lightly-1.4.6/lightly/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.643479 lightly-1.4.6/lightly/utils/cropping/
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/cropping/crop_image_by_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/cropping/read_yolo_label_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/embeddings_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/hipify.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/reordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.611479 lightly-1.4.6/lightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-23 16:31:57.000000 lightly-1.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 16:32:10.647479 lightly-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-23 16:31:57.000000 lightly-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.156761 lightly-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-07 08:25:48.000000 lightly-1.4.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-07 08:25:48.000000 lightly-1.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-07 08:25:57.156761 lightly-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20415 2023-06-07 08:25:48.000000 lightly-1.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.124760 lightly-1.4.7/lightly/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.124760 lightly-1.4.7/lightly/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/active_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.124760 lightly-1.4.7/lightly/active_learning/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/active_learning/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/active_learning/config/selection_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.124760 lightly-1.4.7/lightly/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24922 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_compute_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16198 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32401 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_download_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12930 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_upload_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_upload_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/api_workflow_upload_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/bitmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/prediction_singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/swagger_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/swagger_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/api/version_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.128760 lightly-1.4.7/lightly/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/_cli_simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.128760 lightly-1.4.7/lightly/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/config/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/crop_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/download_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/embed_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/lightly_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/train_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/cli/version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.128760 lightly-1.4.7/lightly/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/data/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/data/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/data/_image_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/data/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25874 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/data/_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49619 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/data/lightly_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/data/multi_view_collate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.128760 lightly-1.4.7/lightly/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/embedding/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/embedding/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/embedding/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.128760 lightly-1.4.7/lightly/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/dcl_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/dino_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/hypersphere_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/msn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/negative_cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/ntx_ent_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/pmsn_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.128760 lightly-1.4.7/lightly/loss/regularizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/regularizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/regularizer/co2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/swav_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/sym_neg_cos_sim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/tico_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/vicreg_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/loss/vicregl_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.132760 lightly-1.4.7/lightly/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/barlowtwins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/byol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/moco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.132760 lightly-1.4.7/lightly/models/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23563 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/modules/heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/modules/masked_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/modules/nn_memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/nnclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/simsiam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18480 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/models/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.124760 lightly-1.4.7/lightly/openapi_generated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.132760 lightly-1.4.7/lightly/openapi_generated/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    25152 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.132760 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/collaboration_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48008 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78621 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/datasources_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160419 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/docker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/embeddings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/mappings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38782 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/predictions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/quota_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52413 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/samples_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/samplings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/scores_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97324 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api/versioning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.152760 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    23521 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/access_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/active_learning_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/api_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/api_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/async_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/category_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/category_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/configuration_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/configuration_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/create_entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/crop_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16339 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_name_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_license_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_task_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/file_name_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/file_output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/general_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_status_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/jobs_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_studio_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/mongo_object_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/object_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/path_safe_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/redirected_read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/s3_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sama_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sama_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sama_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sampling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sampling_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_input_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/shared_access_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/task_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/team_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/team_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/version_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/video_frame_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/openapi_generated/swagger_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.152760 lightly-1.4.7/lightly/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/dino_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/fast_siam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/image_grid_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/jigsaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/mae_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/moco_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/msn_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/multi_crop_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/multi_view_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/pirl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/random_crop_and_flip_with_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/simclr_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/simsiam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/smog_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/swav_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/vicreg_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/transforms/vicregl_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.156761 lightly-1.4.7/lightly/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.156761 lightly-1.4.7/lightly/utils/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/benchmarking/benchmark_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/benchmarking/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/benchmarking/knn_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/benchmarking/linear_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/benchmarking/metric_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/benchmarking/online_linear_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/benchmarking/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/bounding_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.156761 lightly-1.4.7/lightly/utils/cropping/
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/cropping/crop_image_by_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/cropping/read_yolo_label_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/embeddings_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/hipify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/reordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-07 08:25:48.000000 lightly-1.4.7/lightly/utils/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:25:57.124760 lightly-1.4.7/lightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-07 08:25:57.000000 lightly-1.4.7/lightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-06-07 08:25:57.000000 lightly-1.4.7/lightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:25:57.000000 lightly-1.4.7/lightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-07 08:25:57.000000 lightly-1.4.7/lightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-07 08:25:57.000000 lightly-1.4.7/lightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 08:25:57.000000 lightly-1.4.7/lightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 08:25:48.000000 lightly-1.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-07 08:25:57.156761 lightly-1.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-07 08:25:48.000000 lightly-1.4.7/setup.py
```

### Comparing `lightly-1.4.6/LICENSE.txt` & `lightly-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/PKG-INFO` & `lightly-1.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.4.6
+Version: 1.4.7
 Summary: A deep learning package for self-supervised learning
 Author: Philipp Wirth & Igor Susmelj
 Author-email: philipp@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
```

### Comparing `lightly-1.4.6/README.md` & `lightly-1.4.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,14 @@
 ```python
 import torch
 import torchvision
 
 from lightly import loss
 from lightly import transforms
 from lightly.data import LightlyDataset
-from lightly.data.multi_view_collate import MultiViewCollate
 from lightly.models.modules import heads
 
 
 # Create a PyTorch module for the SimCLR model.
 class SimCLR(torch.nn.Module):
     def __init__(self, backbone):
         super().__init__()
@@ -151,26 +150,23 @@
 
 # Build the SimCLR model.
 model = SimCLR(backbone)
 
 # Prepare transform that creates multiple random views for every image.
 transform = transforms.SimCLRTransform(input_size=32, cj_prob=0.5)
 
-# Combine views from multiple images into a batch.
-collate_fn = MultiViewCollate()
 
 # Create a dataset from your image folder.
 dataset = data.LightlyDataset(input_dir="./my/cute/cats/dataset/", transform=transform)
 
 # Build a PyTorch dataloader.
 dataloader = torch.utils.data.DataLoader(
     dataset,  # Pass the dataset to the dataloader.
     batch_size=128,  # A large batch size helps with the learning.
     shuffle=True,  # Shuffling is important!
-    collate_fn=collate_fn,
 )
 
 # Lightly exposes building blocks such as loss functions.
 criterion = loss.NTXentLoss(temperature=0.5)
 
 # Get a PyTorch optimizer.
 optimizer = torch.optim.SGD(model.parameters(), lr=0.1, weight_decay=1e-6)
@@ -280,17 +276,18 @@
 Implemented models and their performance on various datasets. Hyperparameters are not
 tuned for maximum accuracy. For detailed results and more info about the benchmarks click
 [here](https://docs.lightly.ai/self-supervised-learning/getting_started/benchmarks.html).
 
 
 ### Imagenet
 
-| Model       | Backbone | Batch Size | Epochs | Linear Top1 | Linear Top1 Online | KNN Top1 | Tensorboard | Checkpoint |
-|-------------|----------|------------|--------|-------------|--------------------|----------|-------------|------------|
-| SimCLR      | Res50    |        256 |    100 |        63.2 |               63.1 |     44.9 |      [link](https://tensorboard.dev/experiment/JwNs9E02TeeQkS7aljh8dA) |       [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-05-04_09-02-54/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt) |
+| Model       | Backbone | Batch Size | Epochs | Linear Top1 | Finetune Top1 | KNN Top1 | Tensorboard | Checkpoint |
+|-------------|----------|------------|--------|-------------|---------------|----------|-------------|------------|
+| SimCLR      | Res50    |        256 |    100 |        63.2 |           N/A |     44.9 |      [link](https://tensorboard.dev/experiment/JwNs9E02TeeQkS7aljh8dA) |       [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-05-04_09-02-54/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt) |
+| SwAV        | Res50    |        256 |    100 |        67.2 |          75.4 |     49.5 |      [link](https://tensorboard.dev/experiment/Ipx4Oxl5Qkqm5Sl5kWyKKg) |       [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_swav_2023-05-25_08-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)
 
 
 ### ImageNette
 
 | Model       | Backbone | Batch Size | Epochs | KNN Top1 |
 |-------------|----------|------------|--------|----------|
 | BarlowTwins | Res18    |        256 |    800 |    0.852 |
```

### Comparing `lightly-1.4.6/lightly/__init__.py` & `lightly-1.4.7/lightly/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 """
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 __name__ = "lightly"
-__version__ = "1.4.6"
+__version__ = "1.4.7"
 
 import os
 
 try:
     # See (https://github.com/PyTorchLightning/pytorch-lightning)
     # This variable is injected in the __builtins__ by the build
     # process. It used to enable importing subpackages of skimage when
```

### Comparing `lightly-1.4.6/lightly/active_learning/utils/bounding_box.py` & `lightly-1.4.7/lightly/utils/bounding_box.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/api/__init__.py` & `lightly-1.4.7/lightly/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/api/api_workflow_artifacts.py` & `lightly-1.4.7/lightly/api/api_workflow_artifacts.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/api/api_workflow_client.py` & `lightly-1.4.7/lightly/api/api_workflow_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,17 @@
     The APIWorkflowClient is used to communicate with the Lightly API. The client
     can run also more complex workflows which include multiple API calls at once.
 
     The client can be used in combination with the active learning agent.
 
     Args:
         token:
-            The token of the user. For further information on how to get a token,
+            The token of the user. If it is not passed in during initialization, the token
+            will be read from the environment variable LIGHTLY_TOKEN.
+            For further information on how to get a token,
             see: https://docs.lightly.ai/docs/install-lightly#api-token
         dataset_id:
             The id of the dataset. If it is not set, but used by a workflow, the last
             modfied dataset is taken by default.
         embedding_id:
             The id of the embedding to use. If it is not set, but used by a workflow,
             the newest embedding is taken by default
@@ -145,18 +147,19 @@
         self._metadata_configurations_api = MetaDataConfigurationsApi(
             api_client=self.api_client
         )
         self._predictions_api = PredictionsApi(api_client=self.api_client)
 
     @property
     def dataset_id(self) -> str:
-        """The current dataset_id.
+        """The current dataset ID.
 
-        If the dataset_id is set, it is returned.
-        If it is not set, then the dataset_id of the last modified dataset is selected.
+        Future requests with the client will automatically use this dataset ID.
+        If the dataset ID is set, it is returned. Otherwise, the ID of the
+        last modified dataset is selected.
         """
         try:
             return self._dataset_id
         except AttributeError:
             all_datasets: List[DatasetData] = self.get_datasets()
             datasets_sorted = sorted(
                 all_datasets, key=lambda dataset: dataset.last_modified_at
@@ -168,23 +171,23 @@
                     f"Dataset has not been specified, "
                     f"taking the last modified dataset {last_modified_dataset.name} as default dataset."
                 )
             )
             return self._dataset_id
 
     @dataset_id.setter
-    def dataset_id(self, dataset_id: str):
-        """Sets the current dataset id for the client.
+    def dataset_id(self, dataset_id: str) -> None:
+        """Sets the current dataset ID for the client.
 
         Args:
             dataset_id:
                 The new dataset id.
 
         Raises:
-            ValueError if the dataset id does not exist.
+            ValueError if the dataset does not exist.
         """
         if not self.dataset_exists(dataset_id):
             raise ValueError(
                 f"A dataset with the id {dataset_id} does not exist on the web"
                 f"platform."
             )
         self._dataset_id = dataset_id
@@ -214,14 +217,17 @@
         )
         return list_ordered
 
     def get_filenames(self) -> List[str]:
         """Downloads the list of filenames from the server.
 
         This is an expensive operation, especially for large datasets.
+
+        Returns:
+            Names of files in the current dataset.
         """
         filenames_on_server = self._mappings_api.get_sample_mappings_by_dataset_id(
             dataset_id=self.dataset_id, field="fileName"
         )
         return filenames_on_server
 
     def upload_file_with_signed_url(
@@ -236,20 +242,20 @@
         Args:
             file:
                 The file to upload.
             signed_write_url:
                 The url to upload the file to. As no authorization is used,
                 the url must be a signed write url.
             headers:
-                Specific headers for the request.
+                Specific headers for the request. Defaults to None.
             session:
                 Optional requests session used to upload the file.
 
         Returns:
-            The response of the put request, usually a 200 for the success case.
+            The response of the put request.
 
         """
 
         # check to see if server side encryption for S3 is desired
         # see https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingServerSideEncryption.html
         # see https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingKMSEncryption.html
         lightly_s3_sse_kms_key = os.environ.get(LIGHTLY_S3_SSE_KMS_KEY, "").strip()
```

### Comparing `lightly-1.4.6/lightly/api/api_workflow_collaboration.py` & `lightly-1.4.7/lightly/api/api_workflow_collaboration.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 )
 from lightly.openapi_generated.swagger_client.models.shared_access_type import (
     SharedAccessType,
 )
 
 
 class _CollaborationMixin:
-    def share_dataset_only_with(self, dataset_id: str, user_emails: List[str]):
-        """Shares dataset with a list of users
+    def share_dataset_only_with(self, dataset_id: str, user_emails: List[str]) -> None:
+        """Shares a dataset with a list of users.
 
         This method overwrites the list of users that have had access to the dataset
-        before. If you want to add someone new to the list make sure you get the
-        list of users with access beforehand and add them as well.
+        before. If you want to add someone new to the list, make sure you first fetch
+        the list of users with access and include them in the `user_emails`
+        parameter.
 
         Args:
-          dataset_id:
-            Identifier of dataset
-          user_emails:
-            List of email addresses of users to grant write permission
+            dataset_id:
+                ID of the dataset to be shared.
+            user_emails:
+                List of email addresses of users who will get access to the dataset.
 
         Examples:
           >>> # share a dataset with a user
           >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
           >>> client.share_dataset_only_with(dataset_id="MY_DATASET_ID", user_emails=["user@something.com"])
           >>>
           >>> # share dataset with a user while keep sharing it with previous users
@@ -44,22 +45,22 @@
             access_type=SharedAccessType.WRITE, users=user_emails, creator=self._creator
         )
         self._collaboration_api.create_or_update_shared_access_config_by_dataset_id(
             body=body, dataset_id=dataset_id
         )
 
     def get_shared_users(self, dataset_id: str) -> List[str]:
-        """Get list of users that have access to the dataset
+        """Fetches a list of users that have access to the dataset.
 
         Args:
-          dataset_id:
-            Identifier of dataset
+            dataset_id:
+                Dataset ID.
 
         Returns:
-          List of email addresses of users that have write access to the dataset
+            List of email addresses of users that have write access to the dataset.
 
         Examples:
             >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
             >>> client.get_shared_users(dataset_id="MY_DATASET_ID")
             >>> ["user@something.com"]
         """
```

### Comparing `lightly-1.4.6/lightly/api/api_workflow_compute_worker.py` & `lightly-1.4.7/lightly/api/api_workflow_compute_worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,133 +35,182 @@
 
 class InvalidConfigurationError(RuntimeError):
     pass
 
 
 @dataclasses.dataclass
 class ComputeWorkerRunInfo:
-    """
-    Contains information about a compute worker run that is useful for monitoring it.
+    """Information about a Lightly Worker run.
 
     Attributes:
         state:
-            The state of the compute worker run.
+            The state of the Lightly Worker run.
         message:
-            The last message of the compute worker run.
+            The last message of the Lightly Worker run.
     """
 
     state: Union[
         DockerRunState, DockerRunScheduledState.OPEN, STATE_SCHEDULED_ID_NOT_FOUND
     ]
     message: str
 
     def in_end_state(self) -> bool:
-        """Returns wether the compute worker has ended"""
+        """Checks whether the Lightly Worker run has ended."""
         return self.state in [
             DockerRunState.COMPLETED,
             DockerRunState.ABORTED,
             DockerRunState.FAILED,
             DockerRunState.CRASHED,
             STATE_SCHEDULED_ID_NOT_FOUND,
         ]
 
     def ended_successfully(self) -> bool:
-        """
-        Returns wether the compute worker ended successfully or failed.
-        Raises a ValueError if the compute worker is still running.
+        """Checkes whether the Lightly Worker run ended successfully or failed.
+
+        Returns:
+            A boolean value indicating if the Lightly Worker run was successful.
+            True if the run was successful.
+
+        Raises:
+            ValueError:
+                If the Lightly Worker run is still in progress.
         """
         if not self.in_end_state():
-            raise ValueError("Compute worker is still running")
+            raise ValueError("Lightly Worker run is still in progress.")
         return self.state == DockerRunState.COMPLETED
 
 
 class _ComputeWorkerMixin:
     def register_compute_worker(
         self, name: str = "Default", labels: Optional[List[str]] = None
     ) -> str:
-        """Registers a new compute worker.
+        """Registers a new Lightly Worker.
 
-        If a worker with the same name already exists, the worker id of the existing
-        worker is returned instead of registering a new worker.
+        The ID of the registered worker will be returned. If a worker with the same
+        name already exists, the ID of the existing worker is returned.
 
         Args:
             name:
                 The name of the Lightly Worker.
             labels:
                 The labels of the Lightly Worker.
                 See our docs for more information regarding the labels parameter:
                 https://docs.lightly.ai/docs/assign-scheduled-runs-to-specific-workers
 
         Returns:
-            The id of the newly registered compute worker.
+            ID of the registered Lightly Worker.
 
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>> worker_id = client.register_compute_worker(name="my-worker", labels=["worker-label"])
+            >>> worker_id
+            '64709eac61e9ce68180a6529'
         """
         if labels is None:
             labels = []
         request = CreateDockerWorkerRegistryEntryRequest(
             name=name,
             worker_type=DockerWorkerType.FULL,
             labels=labels,
             creator=self._creator,
         )
         response = self._compute_worker_api.register_docker_worker(request)
         return response.id
 
     def get_compute_worker_ids(self) -> List[str]:
-        """Fetches the IDs of all registered compute workers.
+        """Fetches the IDs of all registered Lightly Workers.
 
         Returns:
             A list of worker IDs.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>> worker_ids = client.get_compute_worker_ids()
+            >>> worker_ids
+            ['64709eac61e9ce68180a6529', '64709f8f61e9ce68180a652a']
         """
         entries = self._compute_worker_api.get_docker_worker_registry_entries()
         return [entry.id for entry in entries]
 
     def get_compute_workers(self) -> List[DockerWorkerRegistryEntryData]:
-        """Fetches details of all registered compute workers.
+        """Fetches details of all registered Lightly Workers.
 
         Returns:
-            A list of compute workers.
+            A list of Lightly Worker details.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>> workers = client.get_compute_workers()
+            >>> workers
+            [{'created_at': 1685102336056,
+                'docker_version': '2.6.0',
+                'id': '64709eac61e9ce68180a6529',
+                'labels': [],
+                ...
+            }]
         """
         entries: list[
             DockerWorkerRegistryEntryData
         ] = self._compute_worker_api.get_docker_worker_registry_entries()
         return entries
 
-    def delete_compute_worker(self, worker_id: str):
-        """Removes a compute worker.
+    def delete_compute_worker(self, worker_id: str) -> None:
+        """Removes a Lightly Worker.
 
         Args:
             worker_id:
-                The id of the worker to remove.
+                ID of the worker to be removed.
 
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>> worker_ids = client.get_compute_worker_ids()
+            >>> worker_ids
+            ['64709eac61e9ce68180a6529']
+            >>> client.delete_compute_worker(worker_id="64709eac61e9ce68180a6529")
+            >>> client.get_compute_worker_ids()
+            []
         """
         self._compute_worker_api.delete_docker_worker_registry_entry_by_id(worker_id)
 
     def create_compute_worker_config(
         self,
         worker_config: Optional[Dict[str, Any]] = None,
         lightly_config: Optional[Dict[str, Any]] = None,
         selection_config: Optional[Union[Dict[str, Any], SelectionConfig]] = None,
     ) -> str:
-        """Creates a new configuration for a compute worker run.
+        """Creates a new configuration for a Lightly Worker run.
 
         See our docs for more information regarding the different configurations:
         https://docs.lightly.ai/docs/all-configuration-options
 
         Args:
             worker_config:
-                Compute worker configuration.
+                Lightly Worker configuration.
             lightly_config:
                 Lightly configuration.
             selection_config:
                 Selection configuration.
 
         Returns:
-            The id of the created config.
+            The ID of the created config.
 
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>> selection_config = {
+            ...     "n_samples": 3,
+            ...     "strategies": [
+            ...         {
+            ...             "input": {"type": "RANDOM", "random_seed": 42},
+            ...             "strategy": {"type": "WEIGHTS"},
+            ...         }
+            ...     ],
+            ... }
+            >>> config_id = client.create_compute_worker_config(
+            ...     selection_config=selection_config,
+            ... )
         """
         if isinstance(selection_config, dict):
             selection = selection_config_from_dict(cfg=selection_config)
         else:
             selection = selection_config
 
         if worker_config is not None:
@@ -209,15 +258,15 @@
         """Schedules a run with the given configurations.
 
         See our docs for more information regarding the different configurations:
         https://docs.lightly.ai/docs/all-configuration-options
 
         Args:
             worker_config:
-                Compute worker configuration.
+                Lightly Worker configuration.
             lightly_config:
                 Lightly configuration.
             selection_config:
                 Selection configuration.
             runs_on:
                 The required labels the Lightly Worker must have to take the job.
                 See our docs for more information regarding the runs_on paramter:
@@ -233,14 +282,21 @@
                     402: Insufficient plan
                     403: Not authorized for this resource or invalid token
                     404: Resource (dataset or config) not found
                     422: Missing or invalid file in datasource
             InvalidConfigError:
                 If one of the configurations is invalid.
 
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>> selection_config = {...}
+            >>> worker_labels = ["worker-label"]
+            >>> run_id = client.schedule_compute_worker_run(
+            ...     selection_config=selection_config, runs_on=worker_labels
+            ... )
         """
         if runs_on is None:
             runs_on = []
         config_id = self.create_compute_worker_config(
             worker_config=worker_config,
             lightly_config=lightly_config,
             selection_config=selection_config,
@@ -253,77 +309,154 @@
         )
         response = self._compute_worker_api.create_docker_run_scheduled_by_dataset_id(
             body=request,
             dataset_id=self.dataset_id,
         )
         return response.id
 
-    def get_compute_worker_runs(
+    def get_compute_worker_runs_iter(
         self,
         dataset_id: Optional[str] = None,
-    ) -> List[DockerRunData]:
-        """Get all compute worker runs for the user.
+    ) -> Iterator[DockerRunData]:
+        """Returns an iterator over all Lightly Worker runs for the user.
 
         Args:
             dataset_id:
-                If set, then only runs for the given dataset are returned.
+                Target dataset ID. Optional. If set, only runs with the given dataset
+                will be returned.
 
         Returns:
-            Runs sorted by creation time from old to new.
+            Runs iterator.
 
         """
         if dataset_id is not None:
-            runs: List[DockerRunData] = utils.paginate_endpoint(
+            return utils.paginate_endpoint(
                 self._compute_worker_api.get_docker_runs_query_by_dataset_id,
                 dataset_id=dataset_id,
             )
         else:
-            runs: List[DockerRunData] = utils.paginate_endpoint(
+            return utils.paginate_endpoint(
                 self._compute_worker_api.get_docker_runs,
             )
+
+    def get_compute_worker_runs(
+        self,
+        dataset_id: Optional[str] = None,
+    ) -> List[DockerRunData]:
+        """Fetches all Lightly Worker runs for the user.
+
+        Args:
+            dataset_id:
+                Target dataset ID. Optional. If set, only runs with the given dataset
+                will be returned.
+
+        Returns:
+            Runs sorted by creation time from the oldest to the latest.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>> client.get_compute_worker_runs()
+            [{'artifacts': [...],
+             'config_id': '6470a16461e9ce68180a6530',
+             'created_at': 1679479418110,
+             'dataset_id': '6470a36361e9ce68180a6531',
+             'docker_version': '2.6.0',
+             ...
+             }]
+        """
+        runs: List[DockerRunData] = list(self.get_compute_worker_runs_iter(dataset_id))
         sorted_runs = sorted(runs, key=lambda run: run.created_at or -1)
         return sorted_runs
 
     def get_compute_worker_run(self, run_id: str) -> DockerRunData:
-        """Returns a run given its id.
+        """Fetches a Lightly Worker run.
+
+        Args:
+            run_id: Run ID.
+
+        Returns:
+            Details of the Lightly Worker run.
 
         Raises:
             ApiException:
-                If no run with the given id exists.
+                If no run with the given ID exists.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>> client.get_compute_worker_run(run_id="6470a20461e9ce68180a6530")
+            {'artifacts': [...],
+             'config_id': '6470a16461e9ce68180a6530',
+             'created_at': 1679479418110,
+             'dataset_id': '6470a36361e9ce68180a6531',
+             'docker_version': '2.6.0',
+             ...
+             }
         """
         return self._compute_worker_api.get_docker_run_by_id(run_id=run_id)
 
     def get_compute_worker_run_from_scheduled_run(
         self,
         scheduled_run_id: str,
     ) -> DockerRunData:
-        """Returns a run given its scheduled run id.
+        """Fetches a Lightly Worker run given its scheduled run ID.
+
+        Args:
+            scheduled_run_id: Scheduled run ID.
+
+        Returns:
+            Details of the Lightly Worker run.
 
         Raises:
             ApiException:
-                If no run with the given scheduled run id exists or if the scheduled
-                run has not yet started being processed by a worker.
+                If no run with the given scheduled run ID exists or if the scheduled
+                run is not yet picked up by a worker.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>> client.get_compute_worker_run_from_scheduled_run(scheduled_run_id="646f338a8a5613b57d8b73a1")
+            {'artifacts': [...],
+             'config_id': '6470a16461e9ce68180a6530',
+             'created_at': 1679479418110,
+             'dataset_id': '6470a36361e9ce68180a6531',
+             'docker_version': '2.6.0',
+             ...
+            }
         """
         return self._compute_worker_api.get_docker_run_by_scheduled_id(
             scheduled_id=scheduled_run_id
         )
 
     def get_scheduled_compute_worker_runs(
         self,
         state: Optional[str] = None,
     ) -> List[DockerRunScheduledData]:
-        """Returns a list of all scheduled compute worker runs for the current
-        dataset.
+        """Returns a list of scheduled Lightly Worker runs with the current dataset.
 
         Args:
             state:
                 DockerRunScheduledState value. If specified, then only runs in the given
                 state are returned. If omitted, then runs which have not yet finished
                 (neither 'DONE' nor 'CANCELED') are returned. Valid states are 'OPEN',
                 'LOCKED', 'DONE', and 'CANCELED'.
+
+        Returns:
+            A list of scheduled Lightly Worker runs.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>> client.get_scheduled_compute_worker_runs(state="OPEN")
+            [{'config_id': '646f34608a5613b57d8b73cc',
+             'created_at': 1685009508254,
+             'dataset_id': '6470a36361e9ce68180a6531',
+             'id': '646f338a8a5613b57d8b73a1',
+             'last_modified_at': 1685009542667,
+             'owner': '643d050b8bcb91967ded65df',
+             'priority': 'MID',
+             'runs_on': ['worker-label'],
+             'state': 'OPEN'}]
         """
         if state is not None:
             return self._compute_worker_api.get_docker_runs_scheduled_by_dataset_id(
                 dataset_id=self.dataset_id,
                 state=state,
             )
         return self._compute_worker_api.get_docker_runs_scheduled_by_dataset_id(
@@ -332,18 +465,18 @@
 
     def _get_scheduled_run_by_id(self, scheduled_run_id: str) -> DockerRunScheduledData:
         """Returns the schedule run data given the id of the scheduled run.
 
         TODO (MALTE, 09/2022): Have a proper API endpoint for doing this.
         Args:
             scheduled_run_id:
-                The id with which the run was scheduled.
+                The ID with which the run was scheduled.
 
         Returns:
-            Data about the scheduled run.
+            Defails of the scheduled run.
 
         """
         try:
             run: DockerRunScheduledData = next(
                 run
                 for run in retry(
                     lambda: self._compute_worker_api.get_docker_runs_scheduled_by_dataset_id(
@@ -357,25 +490,25 @@
             raise ApiException(
                 f"No scheduled run found for run with scheduled_run_id='{scheduled_run_id}'."
             )
 
     def get_compute_worker_run_info(
         self, scheduled_run_id: str
     ) -> ComputeWorkerRunInfo:
-        """Returns information about the compute worker run.
+        """Returns information about the Lightly Worker run.
 
         Args:
             scheduled_run_id:
-                The id with which the run was scheduled.
+                ID of the scheduled run.
 
         Returns:
-            Data about the compute worker run.
+            Details of the Lightly Worker run.
 
         Examples:
-            >>> # Scheduled a compute worker run and get its state
+            >>> # Scheduled a Lightly Worker run and get its state
             >>> scheduled_run_id = client.schedule_compute_worker_run(...)
             >>> run_info = client.get_compute_worker_run_info(scheduled_run_id)
             >>> print(run_info)
 
         """
         """
         Because we currently (09/2022) have different Database entries for a ScheduledRun and DockerRun,
@@ -410,33 +543,32 @@
                     "being picked up by a Lightly Worker.",
                 )
         return info
 
     def compute_worker_run_info_generator(
         self, scheduled_run_id: str
     ) -> Iterator[ComputeWorkerRunInfo]:
-        """
-        Yields information about a compute worker run
+        """Pulls information about a Lightly Worker run continuously.
 
-        Polls the compute worker status every 30s.
-        If the status changed, it will yield a new ComputeWorkerRunInfo.
-        If the compute worker run finished, the generator stops.
+        Polls the Lightly Worker status every 30s.
+        If the status changed, an update pops up.
+        If the Lightly Worker run finished, the generator stops.
 
         Args:
             scheduled_run_id:
                 The id with which the run was scheduled.
 
         Returns:
-            Generator of information about the compute worker run status.
+            Generator of information about the Lightly Worker run status.
 
         Examples:
-            >>> # Scheduled a compute worker run and monitor its state
+            >>> # Scheduled a Lightly Worker run and monitor its state
             >>> scheduled_run_id = client.schedule_compute_worker_run(...)
             >>> for run_info in client.compute_worker_run_info_generator(scheduled_run_id):
-            >>>     print(f"Compute worker run is now in state='{run_info.state}' with message='{run_info.message}'")
+            >>>     print(f"Lightly Worker run is now in state='{run_info.state}' with message='{run_info.message}'")
             >>>
 
         """
         last_run_info = None
         while True:
             run_info = self.get_compute_worker_run_info(
                 scheduled_run_id=scheduled_run_id
@@ -452,21 +584,21 @@
 
             # Wait before polling the state again
             time.sleep(30)  # Keep this at 30s or larger to prevent rate limiting.
 
             last_run_info = run_info
 
     def get_compute_worker_run_tags(self, run_id: str) -> List[TagData]:
-        """Returns all tags from a run for the current dataset.
+        """Returns all tags from a run with the current dataset.
 
         Only returns tags for runs made with Lightly Worker version >=2.4.2.
 
         Args:
             run_id:
-                Run id from which to return tags.
+                Run ID from which to return tags.
 
         Returns:
             List of tags created by the run. The tags are ordered by creation date from
             newest to oldest.
 
         Examples:
             >>> # Get filenames from last run.
```

### Comparing `lightly-1.4.6/lightly/api/api_workflow_datasources.py` & `lightly-1.4.7/lightly/api/api_workflow_datasources.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             "DatasourcesApi.get_list_of_raw_samples_from_datasource_by_dataset_id",
             "DatasourcesApi.get_list_of_raw_samples_predictions_from_datasource_by_dataset_id",
             "DatasourcesApi.get_list_of_raw_samples_metadata_from_datasource_by_dataset_id",
         ],
         from_: int = 0,
         to: Optional[int] = None,
         relevant_filenames_file_name: Optional[str] = None,
-        use_redirected_read_url: Optional[bool] = False,
+        use_redirected_read_url: bool = False,
         progress_bar: Optional[tqdm.tqdm] = None,
         **kwargs,
     ) -> List[Tuple[str, str]]:
         if to is None:
             to = int(time.time())
         relevant_filenames_kwargs = (
             {"relevant_filenames_file_name": relevant_filenames_file_name}
@@ -97,41 +97,52 @@
         return [(file_name, read_url) for file_name, read_url in sample_map.items()]
 
     def download_raw_samples(
         self,
         from_: int = 0,
         to: Optional[int] = None,
         relevant_filenames_file_name: Optional[str] = None,
-        use_redirected_read_url: Optional[bool] = False,
+        use_redirected_read_url: bool = False,
         progress_bar: Optional[tqdm.tqdm] = None,
     ) -> List[Tuple[str, str]]:
-        """Downloads all filenames and read urls from the datasource between `from_` and `to`.
+        """Downloads filenames and read urls from the datasource.
 
-        Samples which have timestamp == `from_` or timestamp == `to` will also be included.
+        Only samples with timestamp between `from_` (inclusive) and `to` (inclusive)
+        will be downloaded.
 
         Args:
             from_:
-                Unix timestamp from which on samples are downloaded.
+                Unix timestamp from which on samples are downloaded. Defaults to the
+                very beginning (timestamp 0).
             to:
                 Unix timestamp up to and including which samples are downloaded.
+                Defaults to the current timestamp.
             relevant_filenames_file_name:
-                The path to the relevant filenames text file in the cloud bucket.
-                The path is relative to the datasource root.
+                Path to the relevant filenames text file in the cloud bucket.
+                The path is relative to the datasource root. Optional.
             use_redirected_read_url:
-                By default this is set to false unless a S3DelegatedAccess is configured in which
-                case its always true and this param has no effect.
-                When true this will return RedirectedReadUrls instead of ReadUrls meaning that
-                returned URLs allow for unlimited access to the file
+                Flag for redirected read urls. When this flag is true,
+                RedirectedReadUrls are returned instead of ReadUrls, meaning that the
+                returned URLs have unlimited access to the file.
+                Defaults to False. When S3DelegatedAccess is configured, this flag has
+                no effect because RedirectedReadUrls are always returned.
             progress_bar:
                 Tqdm progress bar to show how many samples have already been
                 retrieved.
 
         Returns:
-           A list of (filename, url) tuples, where each tuple represents a sample
+            A list of (filename, url) tuples where each tuple represents a sample.
 
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.download_raw_samples()
+            [('image-1.png', 'https://......'), ('image-2.png', 'https://......')]
         """
         samples = self._download_raw_files(
             download_function=self._datasources_api.get_list_of_raw_samples_from_datasource_by_dataset_id,
             from_=from_,
             to=to,
             relevant_filenames_file_name=relevant_filenames_file_name,
             use_redirected_read_url=use_redirected_read_url,
@@ -143,50 +154,63 @@
         self,
         task_name: str,
         from_: int = 0,
         to: Optional[int] = None,
         relevant_filenames_file_name: Optional[str] = None,
         run_id: Optional[str] = None,
         relevant_filenames_artifact_id: Optional[str] = None,
-        use_redirected_read_url: Optional[bool] = False,
+        use_redirected_read_url: bool = False,
         progress_bar: Optional[tqdm.tqdm] = None,
     ) -> List[Tuple[str, str]]:
-        """Downloads all prediction filenames and read urls from the datasource between `from_` and `to`.
+        """Downloads prediction filenames and read urls from the datasource.
 
-        Samples which have timestamp == `from_` or timestamp == `to` will also be included.
+        Only samples with timestamp between `from_` (inclusive) and `to` (inclusive)
+        will be downloaded.
 
         Args:
             task_name:
                 Name of the prediction task.
             from_:
-                Unix timestamp from which on samples are downloaded.
+                Unix timestamp from which on samples are downloaded. Defaults to the
+                very beginning (timestamp 0).
             to:
                 Unix timestamp up to and including which samples are downloaded.
+                Defaults to the current timestamp.
             relevant_filenames_file_name:
-                The path to the relevant filenames text file in the cloud bucket.
-                The path is relative to the datasource root.
+                Path to the relevant filenames text file in the cloud bucket.
+                The path is relative to the datasource root. Optional.
             run_id:
-                Run ID. Should be given along with `relevant_filenames_artifact_id` to
-                download relevant files only.
+                Run ID. Optional. Should be given along with
+                `relevant_filenames_artifact_id` to download relevant files only.
             relevant_filenames_artifact_id:
-                ID of the relevant filename artifact. Should be given along with
-                `run_id` to download relevant files only. Note that this is different
-                from `relevant_filenames_file_name`.
+                ID of the relevant filename artifact. Optional. Should be given along
+                with `run_id` to download relevant files only. Note that this is
+                different from `relevant_filenames_file_name`.
             use_redirected_read_url:
-                By default this is set to false unless a S3DelegatedAccess is configured in which
-                case its always true and this param has no effect.
-                When true this will return RedirectedReadUrls instead of ReadUrls meaning that
-                returned URLs allow for unlimited access to the file
+                Flag for redirected read urls. When this flag is true,
+                RedirectedReadUrls are returned instead of ReadUrls, meaning that the
+                returned URLs have unlimited access to the file.
+                Defaults to False. When S3DelegatedAccess is configured, this flag has
+                no effect because RedirectedReadUrls are always returned.
             progress_bar:
                 Tqdm progress bar to show how many prediction files have already been
                 retrieved.
 
         Returns:
-           A list of (filename, url) tuples, where each tuple represents a sample
+            A list of (filename, url) tuples where each tuple represents a sample.
 
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> task_name = "object-detection"
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.download_raw_predictions(task_name=task_name)
+            [('.lightly/predictions/object-detection/image-1.json', 'https://......'),
+             ('.lightly/predictions/object-detection/image-2.json', 'https://......')]
         """
         if run_id is not None and relevant_filenames_artifact_id is None:
             raise ValueError(
                 "'relevant_filenames_artifact_id' should not be `None` when 'run_id' "
                 "is specified."
             )
         if run_id is None and relevant_filenames_artifact_id is not None:
@@ -216,48 +240,60 @@
     def download_raw_metadata(
         self,
         from_: int = 0,
         to: Optional[int] = None,
         run_id: Optional[str] = None,
         relevant_filenames_artifact_id: Optional[str] = None,
         relevant_filenames_file_name: Optional[str] = None,
-        use_redirected_read_url: Optional[bool] = False,
+        use_redirected_read_url: bool = False,
         progress_bar: Optional[tqdm.tqdm] = None,
     ) -> List[Tuple[str, str]]:
-        """Downloads all metadata filenames and read urls from the datasource between `from_` and `to`.
+        """Downloads all metadata filenames and read urls from the datasource.
 
-        Samples which have timestamp == `from_` or timestamp == `to` will also be included.
+        Only samples with timestamp between `from_` (inclusive) and `to` (inclusive)
+        will be downloaded.
 
         Args:
             from_:
-                Unix timestamp from which on samples are downloaded.
+                Unix timestamp from which on samples are downloaded. Defaults to the
+                very beginning (timestamp 0).
             to:
                 Unix timestamp up to and including which samples are downloaded.
+                Defaults to the current timestamp.
             relevant_filenames_file_name:
-                The path to the relevant filenames text file in the cloud bucket.
-                The path is relative to the datasource root.
+                Path to the relevant filenames text file in the cloud bucket.
+                The path is relative to the datasource root. Optional.
             run_id:
-                Run ID. Should be given along with `relevant_filenames_artifact_id` to
-                download relevant files only.
+                Run ID. Optional. Should be given along with
+                `relevant_filenames_artifact_id` to download relevant files only.
             relevant_filenames_artifact_id:
-                ID of the relevant filename artifact. Should be given along with
-                `run_id` to download relevant files only. Note that this is different
-                from `relevant_filenames_file_name`.
+                ID of the relevant filename artifact. Optional. Should be given along
+                with `run_id` to download relevant files only. Note that this is
+                different from `relevant_filenames_file_name`.
             use_redirected_read_url:
-                By default this is set to false unless a S3DelegatedAccess is configured in which
-                case its always true and this param has no effect.
-                When true this will return RedirectedReadUrls instead of ReadUrls meaning that
-                returned URLs allow for unlimited access to the file
+                Flag for redirected read urls. When this flag is true,
+                RedirectedReadUrls are returned instead of ReadUrls, meaning that the
+                returned URLs have unlimited access to the file.
+                Defaults to False. When S3DelegatedAccess is configured, this flag has
+                no effect because RedirectedReadUrls are always returned.
             progress_bar:
                 Tqdm progress bar to show how many metadata files have already been
                 retrieved.
 
         Returns:
-           A list of (filename, url) tuples, where each tuple represents a sample
+            A list of (filename, url) tuples where each tuple represents a sample.
 
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.download_raw_metadata()
+            [('.lightly/metadata/object-detection/image-1.json', 'https://......'),
+             ('.lightly/metadata/object-detection/image-2.json', 'https://......')]
         """
         if run_id is not None and relevant_filenames_artifact_id is None:
             raise ValueError(
                 "'relevant_filenames_artifact_id' should not be `None` when 'run_id' "
                 "is specified."
             )
         if run_id is None and relevant_filenames_artifact_id is not None:
@@ -281,32 +317,40 @@
             progress_bar=progress_bar,
             **relevant_filenames_kwargs,
         )
         return samples
 
     def download_new_raw_samples(
         self,
-        use_redirected_read_url: Optional[bool] = False,
+        use_redirected_read_url: bool = False,
     ) -> List[Tuple[str, str]]:
         """Downloads filenames and read urls of unprocessed samples from the datasource.
 
         All samples after the timestamp of `ApiWorkflowClient.get_processed_until_timestamp()` are
-        fetched. After downloading the samples the timestamp is updated to the current time.
+        fetched. After downloading the samples, the timestamp is updated to the current time.
         This function can be repeatedly called to retrieve new samples from the datasource.
 
         Args:
             use_redirected_read_url:
-                By default this is set to false unless a S3DelegatedAccess is configured in which
-                case its always true and this param has no effect.
-                When true this will return RedirectedReadUrls instead of ReadUrls meaning that
-                returned URLs allow for unlimited access to the file
+                Flag for redirected read urls. When this flag is true,
+                RedirectedReadUrls are returned instead of ReadUrls, meaning that the
+                returned URLs have unlimited access to the file.
+                Defaults to False. When S3DelegatedAccess is configured, this flag has
+                no effect because RedirectedReadUrls are always returned.
 
         Returns:
-            A list of (filename, url) tuples, where each tuple represents a sample
+            A list of (filename, url) tuples where each tuple represents a sample.
 
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.download_new_raw_samples()
+            [('image-3.png', 'https://......'), ('image-4.png', 'https://......')]
         """
         from_ = self.get_processed_until_timestamp()
 
         if from_ != 0:
             # We already processed samples at some point.
             # Add 1 because the samples with timestamp == from_
             # have already been processed
@@ -322,38 +366,60 @@
         self.update_processed_until_timestamp(timestamp=to)
         return data
 
     def get_processed_until_timestamp(self) -> int:
         """Returns the timestamp until which samples have been processed.
 
         Returns:
-            Unix timestamp of last processed sample
+            Unix timestamp of last processed sample.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.get_processed_until_timestamp()
+            1684750513
         """
         response: DatasourceProcessedUntilTimestampResponse = self._datasources_api.get_datasource_processed_until_timestamp_by_dataset_id(
             dataset_id=self.dataset_id
         )
         timestamp = int(response.processed_until_timestamp)
         return timestamp
 
     def update_processed_until_timestamp(self, timestamp: int) -> None:
         """Sets the timestamp until which samples have been processed.
 
         Args:
             timestamp:
-                Unix timestamp of last processed sample
+                Unix timestamp of last processed sample.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset.
+            >>> # All samples are processed at this moment.
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.download_new_raw_samples()
+            []
+            >>>
+            >>> # Set timestamp to an earlier moment to reprocess samples
+            >>> client.update_processed_until_timestamp(1684749813)
+            >>> client.download_new_raw_samples()
+            [('image-3.png', 'https://......'), ('image-4.png', 'https://......')]
         """
         body = DatasourceProcessedUntilTimestampRequest(
             processed_until_timestamp=timestamp
         )
         self._datasources_api.update_datasource_processed_until_timestamp_by_dataset_id(
             dataset_id=self.dataset_id, body=body
         )
 
     def get_datasource(self) -> DatasourceConfig:
-        """Calls the api to return the datasource of the current dataset.
+        """Returns the datasource of the current dataset.
 
         Returns:
             Datasource data of the datasource of the current dataset.
 
         Raises:
             ApiException if no datasource was configured.
 
@@ -638,16 +704,17 @@
     ):
         """Returns a read-url for .lightly/predictions/{filename}.
 
         Args:
             filename:
                 Filename for which to get the read-url.
 
-        Returns the read-url. If the file does not exist, a read-url is returned
-        anyways.
+        Returns:
+            A read-url to the file. Note that a URL will be returned even if the file does not
+            exist.
 
         """
         return self._datasources_api.get_prediction_file_read_url_from_datasource_by_dataset_id(
             self.dataset_id,
             filename,
         )
 
@@ -657,16 +724,17 @@
     ):
         """Returns a read-url for .lightly/metadata/{filename}.
 
         Args:
             filename:
                 Filename for which to get the read-url.
 
-        Returns the read-url. If the file does not exist, a read-url is returned
-        anyways.
+        Returns:
+            A read-url to the file. Note that a URL will be returned even if the file does not
+            exist.
 
         """
         return self._datasources_api.get_metadata_file_read_url_from_datasource_by_dataset_id(
             self.dataset_id,
             filename,
         )
 
@@ -676,32 +744,33 @@
     ) -> str:
         """Returns a read-url for .lightly/embeddings/{filename}.
 
         Args:
             filename:
                 Filename for which to get the read-url.
 
-        Returns the read-url. If the file does not exist, a read-url is returned
-        anyways.
+        Returns:
+            A read-url to the file. Note that a URL will be returned even if the file does not
+            exist.
 
         """
         return self._datasources_api.get_custom_embedding_file_read_url_from_datasource_by_dataset_id(
             self.dataset_id,
             filename,
         )
 
     def list_datasource_permissions(
         self,
     ) -> Dict[str, Union[bool, Optional[DatasourceConfigVerifyDataErrors]]]:
-        """List granted access permissions for the datasource set up with a dataset.
+        """Lists granted access permissions for the datasource set up with a dataset.
 
         Returns a string dictionary, with each permission mapped to a boolean value,
-        see the example below. Additionally, there is the ``errors`` key. If there
-        are permission errors it maps to a dictionary from permission name to the
-        error message, otherwise the value is ``None``.
+        see the example below. Additionally, there is the ``errors`` key. Permission
+        errors are stored in a dictionary where permission names are keys and error
+        messages are values. If there is no error, the value is ``None``.
 
         >>> from lightly.api import ApiWorkflowClient
         >>> client = ApiWorkflowClient(
         ...    token="MY_LIGHTLY_TOKEN", dataset_id="MY_DATASET_ID"
         ... )
         >>> client.list_datasource_permissions()
         {'can_list': True,
```

### Comparing `lightly-1.4.6/lightly/api/api_workflow_export.py` & `lightly-1.4.7/lightly/api/api_workflow_export.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,44 +20,59 @@
 
 
 class _ExportDatasetMixin:
     def export_label_studio_tasks_by_tag_id(
         self,
         tag_id: str,
     ) -> List[Dict]:
-        """Exports samples in a format compatible with Label Studio.
+        """Fetches samples in a format compatible with Label Studio.
 
         The format is documented here:
         https://labelstud.io/guide/tasks.html#Basic-Label-Studio-JSON-format
 
+        More information:
+        https://docs.lightly.ai/docs/labelstudio-integration
+
         Args:
             tag_id:
                 Id of the tag which should exported.
 
         Returns:
             A list of dictionaries in a format compatible with Label Studio.
 
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.export_label_studio_tasks_by_tag_id(tag_id="646f34608a5613b57d8b73cc")
+            [{'id': 0, 'data': {'image': '...', ...}}]
         """
-        label_studio_tasks = paginate_endpoint(
-            self._tags_api.export_tag_to_label_studio_tasks,
-            page_size=20000,
-            dataset_id=self.dataset_id,
-            tag_id=tag_id,
+        label_studio_tasks = list(
+            paginate_endpoint(
+                self._tags_api.export_tag_to_label_studio_tasks,
+                page_size=20000,
+                dataset_id=self.dataset_id,
+                tag_id=tag_id,
+            )
         )
         return label_studio_tasks
 
     def export_label_studio_tasks_by_tag_name(
         self,
         tag_name: str,
     ) -> List[Dict]:
-        """Exports samples in a format compatible with Label Studio.
+        """Fetches samples in a format compatible with Label Studio.
 
         The format is documented here:
         https://labelstud.io/guide/tasks.html#Basic-Label-Studio-JSON-format
 
+        More information:
+        https://docs.lightly.ai/docs/labelstudio-integration
+
         Args:
             tag_name:
                 Name of the tag which should exported.
 
         Returns:
             A list of dictionaries in a format compatible with Label Studio.
 
@@ -74,49 +89,64 @@
         tag = self.get_tag_by_name(tag_name)
         return self.export_label_studio_tasks_by_tag_id(tag.id)
 
     def export_label_box_data_rows_by_tag_id(
         self,
         tag_id: str,
     ) -> List[Dict]:
-        """Exports samples in a format compatible with Labelbox v3.
+        """Fetches samples in a format compatible with Labelbox v3.
 
         The format is documented here: https://docs.labelbox.com/docs/images-json
 
+        More information:
+        https://docs.lightly.ai/docs/labelbox
+
         Args:
             tag_id:
-                Id of the tag which should exported.
+                ID of the tag which should exported.
 
         Returns:
             A list of dictionaries in a format compatible with Labelbox v3.
 
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.export_label_box_data_rows_by_tag_id(tag_id="646f34608a5613b57d8b73cc")
+            [{'externalId': '2218961434_7916358f53_z.jpg', 'imageUrl': ...}]
         """
         warnings.warn(
             DeprecationWarning(
                 "This method exports data in the deprecated Labelbox v3 format and "
                 "will be removed in the future. Use export_label_box_v4_data_rows_by_tag_id "
                 "to export data in the Labelbox v4 format instead."
             )
         )
-        label_box_data_rows = paginate_endpoint(
-            self._tags_api.export_tag_to_label_box_data_rows,
-            page_size=20000,
-            dataset_id=self.dataset_id,
-            tag_id=tag_id,
+        label_box_data_rows = list(
+            paginate_endpoint(
+                self._tags_api.export_tag_to_label_box_data_rows,
+                page_size=20000,
+                dataset_id=self.dataset_id,
+                tag_id=tag_id,
+            )
         )
         return label_box_data_rows
 
     def export_label_box_data_rows_by_tag_name(
         self,
         tag_name: str,
     ) -> List[Dict]:
-        """Exports samples in a format compatible with Labelbox v3.
+        """Fetches samples in a format compatible with Labelbox v3.
 
         The format is documented here: https://docs.labelbox.com/docs/images-json
 
+        More information:
+        https://docs.lightly.ai/docs/labelbox
+
         Args:
             tag_name:
                 Name of the tag which should exported.
 
         Returns:
             A list of dictionaries in a format compatible with Labelbox v3.
 
@@ -140,40 +170,56 @@
         tag = self.get_tag_by_name(tag_name)
         return self.export_label_box_data_rows_by_tag_id(tag.id)
 
     def export_label_box_v4_data_rows_by_tag_id(
         self,
         tag_id: str,
     ) -> List[Dict]:
-        """Exports samples in a format compatible with Labelbox v4.
+        """Fetches samples in a format compatible with Labelbox v4.
 
         The format is documented here: https://docs.labelbox.com/docs/images-json
 
+        More information:
+        https://docs.lightly.ai/docs/labelbox
+
         Args:
             tag_id:
-                Id of the tag which should exported.
+                ID of the tag which should exported.
         Returns:
             A list of dictionaries in a format compatible with Labelbox v4.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.export_label_box_v4_data_rows_by_tag_id(tag_id="646f34608a5613b57d8b73cc")
+            [{'row_data': '...', 'global_key': 'image-1.jpg', 'media_type': 'IMAGE'}
         """
-        label_box_data_rows = paginate_endpoint(
-            self._tags_api.export_tag_to_label_box_v4_data_rows,
-            page_size=20000,
-            dataset_id=self.dataset_id,
-            tag_id=tag_id,
+        label_box_data_rows = list(
+            paginate_endpoint(
+                self._tags_api.export_tag_to_label_box_v4_data_rows,
+                page_size=20000,
+                dataset_id=self.dataset_id,
+                tag_id=tag_id,
+            )
         )
         return label_box_data_rows
 
     def export_label_box_v4_data_rows_by_tag_name(
         self,
         tag_name: str,
     ) -> List[Dict]:
-        """Exports samples in a format compatible with Labelbox.
+        """Fetches samples in a format compatible with Labelbox.
 
         The format is documented here: https://docs.labelbox.com/docs/images-json
 
+        More information:
+        https://docs.lightly.ai/docs/labelbox
+
         Args:
             tag_name:
                 Name of the tag which should exported.
         Returns:
             A list of dictionaries in a format compatible with Labelbox.
         Examples:
             >>> # write json file which can be imported in Label Studio
@@ -187,43 +233,56 @@
         tag = self.get_tag_by_name(tag_name)
         return self.export_label_box_v4_data_rows_by_tag_id(tag.id)
 
     def export_filenames_by_tag_id(
         self,
         tag_id: str,
     ) -> str:
-        """Exports a list of the samples filenames within a certain tag.
+        """Fetches samples filenames within a certain tag by tag ID.
+
+        More information:
+        https://docs.lightly.ai/docs/filenames-and-readurls
 
         Args:
             tag_id:
-                Id of the tag which should exported.
+                ID of the tag which should exported.
 
         Returns:
-            A list of the samples filenames within a certain tag.
+            A list of filenames of samples within a certain tag.
 
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.export_filenames_by_tag_id("646b40d6c06aae1b91294a9e")
+            'image-1.jpg\nimage-2.jpg\nimage-3.jpg'
         """
         filenames = retry(
             self._tags_api.export_tag_to_basic_filenames,
             dataset_id=self.dataset_id,
             tag_id=tag_id,
         )
         return filenames
 
     def export_filenames_by_tag_name(
         self,
         tag_name: str,
     ) -> str:
-        """Exports a list of the samples filenames within a certain tag.
+        """Fetches samples filenames within a certain tag by tag name.
+
+        More information:
+        https://docs.lightly.ai/docs/filenames-and-readurls
 
         Args:
             tag_name:
                 Name of the tag which should exported.
 
         Returns:
-            A list of the samples filenames within a certain tag.
+            A list of filenames of samples within a certain tag.
 
         Examples:
             >>> # write json file which can be imported in Label Studio
             >>> filenames = client.export_filenames_by_tag_name(
             >>>     'initial-tag'
             >>> )
             >>>
@@ -234,19 +293,22 @@
         tag = self.get_tag_by_name(tag_name)
         return self.export_filenames_by_tag_id(tag.id)
 
     def export_filenames_and_read_urls_by_tag_id(
         self,
         tag_id: str,
     ) -> List[Dict[str, str]]:
-        """Export filenames, read URLs, and datasource URLs from the given tag.
+        """Fetches filenames, read URLs, and datasource URLs from the given tag.
+
+        More information:
+        https://docs.lightly.ai/docs/filenames-and-readurls
 
         Args:
             tag_id:
-                Id of the tag which should exported.
+                ID of the tag which should exported.
 
         Returns:
             A list of dictionaries with the keys "filename", "readUrl" and "datasourceUrl".
             An example:
             [
                 {
                     "fileName": "sample1.jpg",
@@ -297,22 +359,25 @@
             )
         ]
 
     def export_filenames_and_read_urls_by_tag_name(
         self,
         tag_name: str,
     ) -> List[Dict[str, str]]:
-        """Export filenames, read URLs, and datasource URLs from the given tag name.
+        """Fetches filenames, read URLs, and datasource URLs from the given tag name.
+
+        More information:
+        https://docs.lightly.ai/docs/filenames-and-readurls
 
         Args:
             tag_name:
                 Name of the tag which should exported.
 
         Returns:
-            A list of dictionaries with the keys "filename", "readUrl" and "datasourceUrl".
+            A list of dictionaries with keys "filename", "readUrl" and "datasourceUrl".
 
         Examples:
             >>> # write json file which can be used to access the actual file contents.
             >>> mappings = client.export_filenames_and_read_urls_by_tag_name(
             >>>     'initial-tag'
             >>> )
             >>>
```

### Comparing `lightly-1.4.6/lightly/api/api_workflow_predictions.py` & `lightly-1.4.7/lightly/api/api_workflow_predictions.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 class _PredictionsMixin:
     def create_or_update_prediction_task_schema(
         self,
         schema: PredictionTaskSchema,
         prediction_version_id: int = -1,
     ) -> None:
-        """Creates or updates the prediction task schema
+        """Creates or updates the prediction task schema.
 
         Args:
             schema:
                 The prediction task schema.
             prediction_version_id:
-                A numerical id (e.g timestamp) to distinguish different predictions of different model versions.
-                Use the same id if you don't require versioning or if you wish to overwrite the previous schema.
+                A numerical ID (e.g., timestamp) to distinguish different predictions of different model versions.
+                Use the same ID if you don't require versioning or if you wish to overwrite the previous schema.
 
         Example:
           >>> import time
           >>> from lightly.api import ApiWorkflowClient
           >>> from lightly.openapi_generated.swagger_client import (
           >>>     PredictionTaskSchema,
           >>>     TaskType,
@@ -58,25 +58,25 @@
         sample_id_to_prediction_singletons: Mapping[
             str, Sequence[PredictionSingletonRepr]
         ],
         prediction_version_id: int = -1,
         progress_bar: Optional[tqdm.tqdm] = None,
         max_workers: int = 8,
     ) -> None:
-        """Creates or updates the predictions for specific samples
+        """Creates or updates the predictions for specific samples.
 
         Args:
             sample_id_to_prediction_singletons
                 A mapping from the sample_id of the sample to its corresponding prediction singletons.
                 The singletons can be from different tasks and different types.
 
             prediction_version_id:
-                 A numerical id (e.g timestamp) to distinguish different predictions of different model versions.
-                 Use the same id if you don't require versioning or if you wish to overwrite the previous schema.
-                 This id must match the id of a prediction task schema.
+                A numerical ID (e.g., timestamp) to distinguish different predictions of different model versions.
+                Use the same id if you don't require versioning or if you wish to overwrite the previous schema.
+                This ID must match the ID of a prediction task schema.
 
             progress_bar:
                 Tqdm progress bar to show how many prediction files have already been uploaded.
 
             max_workers:
                 Maximum number of workers uploading predictions in parallel.
 
@@ -133,25 +133,27 @@
 
     def create_or_update_prediction(
         self,
         sample_id: str,
         prediction_singletons: Sequence[PredictionSingletonRepr],
         prediction_version_id: int = -1,
     ) -> None:
-        """Creates or updates the predictions for one specific sample
+        """Creates or updates predictions for one specific sample.
 
         Args:
             sample_id
-                The id of the sample
+                The ID of the sample.
 
             prediction_version_id:
-                And id to distinguish different predictions for the same sample.
+                A numerical ID (e.g., timestamp) to distinguish different predictions of different model versions.
+                Use the same id if you don't require versioning or if you wish to overwrite the previous schema.
+                This ID must match the ID of a prediction task schema.
 
             prediction_singletons:
-                The predictions to upload for that sample
+                Predictions to be uploaded for the designated sample.
         """
         prediction_singletons_for_sending = [
             singleton.to_dict() for singleton in prediction_singletons
         ]
         self._predictions_api.create_or_update_prediction_by_sample_id(
             body=prediction_singletons_for_sending,
             dataset_id=self.dataset_id,
```

### Comparing `lightly-1.4.6/lightly/api/api_workflow_selection.py` & `lightly-1.4.7/lightly/api/api_workflow_selection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 import warnings
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 import numpy as np
+from numpy.typing import NDArray
 
 from lightly.active_learning.config.selection_config import SelectionConfig
 from lightly.openapi_generated.swagger_client import ActiveLearningScoreCreateRequest
 from lightly.openapi_generated.swagger_client.models.job_state import JobState
 from lightly.openapi_generated.swagger_client.models.job_status_data import (
     JobStatusData,
 )
@@ -29,63 +30,74 @@
         scores = scores.astype(np.float64)
 
     # convert to list and return
     return list(scores)
 
 
 class _SelectionMixin:
-    def upload_scores(self, al_scores: Dict[str, np.ndarray], query_tag_id: str):
+    def upload_scores(
+        self, al_scores: Dict[str, NDArray[np.float_]], query_tag_id: str
+    ) -> None:
+        """Uploads active learning scores for a tag.
+
+        Args:
+            al_scores:
+                Active learning scores. Must be a mapping between score names
+                and score arrays. The length of each score array must match samples
+                in the designated tag.
+            query_tag_id: ID of the desired tag.
+        """
         # iterate over all available score types and upload them
         for score_type, score_values in al_scores.items():
             body = ActiveLearningScoreCreateRequest(
                 score_type=score_type,
                 scores=_parse_active_learning_scores(score_values),
             )
             self._scores_api.create_or_update_active_learning_score_by_tag_id(
                 body,
                 dataset_id=self.dataset_id,
                 tag_id=query_tag_id,
             )
 
-    def sampling(self, *args, **kwargs):
-        warnings.warn(
-            DeprecationWarning(
-                "ApiWorkflowClient.sampling() is deprecated "
-                "in favour of ApiWorkflowClient.selection() "
-                "and will be removed in the future."
-            ),
-        )
-        return self.selection(*args, **kwargs)
-
     def selection(
         self,
         selection_config: SelectionConfig,
-        preselected_tag_id: str = None,
-        query_tag_id: str = None,
+        preselected_tag_id: Optional[str] = None,
+        query_tag_id: Optional[str] = None,
     ) -> TagData:
         """Performs a selection given the arguments.
 
         Args:
             selection_config:
                 The configuration of the selection.
             preselected_tag_id:
-                The tag defining the already chosen samples (e.g. already labelled ones), default: None.
+                The tag defining the already chosen samples (e.g., already
+                labelled ones). Optional.
             query_tag_id:
-                The tag defining where to sample from, default: None resolves to the initial-tag.
+                ID of the tag where samples should be fetched. None resolves to
+                `initial-tag`. Defaults to None.
 
         Returns:
             The newly created tag of the selection.
 
         Raises:
-            ApiException
-            ValueError
-            RuntimeError
+            RuntimeError:
+                When a tag with the tag name specified in the selection config already exists.
+                When `initial-tag` does not exist in the dataset.
+                When the selection task fails.
 
         """
 
+        warnings.warn(
+            DeprecationWarning(
+                "ApiWorkflowClient.selection() is deprecated "
+                "and will be removed in the future."
+            ),
+        )
+
         # make sure the tag name does not exist yet
         tags = self.get_all_tags()
         if selection_config.name in [tag.name for tag in tags]:
             raise RuntimeError(
                 f"There already exists a tag with tag_name {selection_config.name}."
             )
         if len(tags) == 0:
@@ -148,16 +160,16 @@
         )
 
         return new_tag_data
 
     def _create_selection_create_request(
         self,
         selection_config: SelectionConfig,
-        preselected_tag_id: str,
-        query_tag_id: str,
+        preselected_tag_id: Optional[str],
+        query_tag_id: Optional[str],
     ) -> SamplingCreateRequest:
         """Creates a SamplingCreateRequest
 
         First, it checks how many samples are already labeled by
             getting the number of samples in the preselected_tag_id.
         Then the stopping_condition.n_samples
             is set to be the number of already labeled samples + the selection_config.batch_size.
```

### Comparing `lightly-1.4.6/lightly/api/api_workflow_upload_dataset.py` & `lightly-1.4.7/lightly/api/api_workflow_upload_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Upload Dataset Mixin """
 
 
 import os
 import warnings
 from concurrent.futures.thread import ThreadPoolExecutor
 from datetime import datetime
-from typing import Dict, Union
+from typing import Any, Dict, Optional, Union
 
 import tqdm
 from lightly_utils import image_processing
 
 from lightly.api.utils import (
     MAXIMUM_FILENAME_LENGTH,
     build_azure_signed_url_write_headers,
@@ -57,33 +57,33 @@
     """Mixin to upload datasets to the Lightly Api."""
 
     def upload_dataset(
         self,
         input: Union[str, "LightlyDataset"],
         max_workers: int = 8,
         mode: str = "thumbnails",
-        custom_metadata: Union[Dict, None] = None,
-    ):
-        """Uploads a dataset to to the Lightly cloud solution.
+        custom_metadata: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        """Uploads a dataset to the Lightly Platform.
 
         Args:
             input:
                 Either the path to the dataset, e.g. "path/to/dataset",
-                or the dataset in form of a LightlyDataset
+                or the dataset in form of a LightlyDataset.
             max_workers:
                 Maximum number of workers uploading images in parallel.
             mode:
                 One of [full, thumbnails, metadata]. Whether to upload
                 thumbnails, full images, or metadata only.
             custom_metadata:
-                COCO-style dictionary of custom metadata to be uploaded.
+                COCO-style dictionary of custom metadata to be uploaded. Optional.
 
         Raises:
             ValueError:
-                If dataset is too large or input has the wrong type
+                If dataset is too large or input has the wrong type.
             RuntimeError:
                 If the connection to the server failed.
 
         """
 
         # get all tags of the dataset
         tags = self.get_all_tags()
@@ -252,15 +252,15 @@
         self,
         image,
         filename: str,
         filepath: str,
         mode: str,
         custom_metadata: Union[Dict, None] = None,
         datasource_type: str = "LIGHTLY",
-    ):
+    ) -> None:
         """Uploads a single image to the Lightly platform."""
         # check whether the filepath is too long
         if not check_filename(filepath):
             msg = (
                 "Filepath {filepath} is longer than the allowed maximum of "
                 f"{MAXIMUM_FILENAME_LENGTH} characters and will be skipped."
             )
```

### Comparing `lightly-1.4.6/lightly/api/api_workflow_upload_embeddings.py` & `lightly-1.4.7/lightly/api/api_workflow_upload_embeddings.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
 
 class EmbeddingDoesNotExistError(ValueError):
     pass
 
 
 class _UploadEmbeddingsMixin:
-    def _get_csv_reader_from_read_url(self, read_url: str):
+    def _get_csv_reader_from_read_url(self, read_url: str) -> None:
         """Makes a get request to the signed read url and returns the .csv file."""
         request = Request(read_url, method="GET")
         with urlopen(request) as response:
             buffer = io.StringIO(response.read().decode("utf-8"))
             reader = csv.reader(buffer)
 
         return reader
 
-    def set_embedding_id_to_latest(self):
-        """Sets the self.embedding_id to the one of the latest on the server."""
+    def set_embedding_id_to_latest(self) -> None:
+        """Sets the embedding ID in the API client to the latest embedding ID in the current dataset."""
         embeddings_on_server: List[
             DatasetEmbeddingData
         ] = self._embeddings_api.get_embeddings_by_dataset_id(
             dataset_id=self.dataset_id
         )
         if len(embeddings_on_server) == 0:
             raise RuntimeError(
@@ -47,21 +47,21 @@
             )
         # return first entry as the API returns newest first
         self.embedding_id = embeddings_on_server[0].id
 
     def get_embedding_by_name(
         self, name: str, ignore_suffix: bool = True
     ) -> DatasetEmbeddingData:
-        """Gets an embedding form the server by name.
+        """Fetches an embedding in the current dataset by name.
 
         Args:
             name:
-                The name of the embedding to get.
+                The name of the desired embedding.
             ignore_suffix:
-                If true, a suffix of the embedding name on the server
+                If true, a suffix of the embedding name in the current dataset
                 is ignored.
 
         Returns:
             The embedding data.
 
         Raises:
             EmbeddingDoesNotExistError:
@@ -90,20 +90,20 @@
         except StopIteration:
             raise EmbeddingDoesNotExistError(
                 f"Embedding with the specified name "
                 f"does not exist on the server: {name}"
             )
         return embedding
 
-    def upload_embeddings(self, path_to_embeddings_csv: str, name: str):
-        """Uploads embeddings to the server.
+    def upload_embeddings(self, path_to_embeddings_csv: str, name: str) -> None:
+        """Uploads embeddings to the Lightly Platform.
 
         First checks that the specified embedding name is not on the server. If it is, the upload is aborted.
-        Then creates a new csv with the embeddings in the order specified on the server. Next it uploads it to the server.
-        The received embedding_id is saved as a property of self.
+        Then creates a new csv file with the embeddings in the order specified on the server. Next uploads it
+        to the Lightly Platform. The received embedding ID is stored in the API client.
 
         Args:
             path_to_embeddings_csv:
                 The path to the .csv containing the embeddings, e.g. "path/to/embeddings.csv"
             name:
                 The name of the embedding. If an embedding with such a name already exists on the server,
                 the upload is aborted.
@@ -163,30 +163,30 @@
             body = Trigger2dEmbeddingJobRequest(
                 dimensionality_reduction_method=dimensionality_reduction_method
             )
             self._embeddings_api.trigger2d_embeddings_job(
                 body=body, dataset_id=self.dataset_id, embedding_id=self.embedding_id
             )
 
-    def append_embeddings(self, path_to_embeddings_csv: str, embedding_id: str):
-        """Concatenates the embeddings from the server to the local ones.
+    def append_embeddings(self, path_to_embeddings_csv: str, embedding_id: str) -> None:
+        """Concatenates embeddings from the Lightly Platform to the local ones.
 
-        Loads the embedding csv file belonging to the embedding_id, and
-        appends all of its rows to the local embeddings file located at
+        Loads the embedding csv file with the corresponding embedding ID in the current dataset
+        and appends all of its rows to the local embeddings file located at
         'path_to_embeddings_csv'.
 
         Args:
             path_to_embeddings_csv:
                 The path to the csv containing the local embeddings.
             embedding_id:
-                Id of the embedding summary of the embeddings on the server.
+                ID of the embedding summary of the embeddings on the Lightly Platform.
 
         Raises:
             RuntimeError:
-                If the number of columns in the local and the remote
+                If the number of columns in the local embeddings file and that of the remote
                 embeddings file mismatch.
 
         """
 
         # read embedding from API
         embedding_read_url = self._embeddings_api.get_embeddings_csv_read_url_by_id(
             self.dataset_id, embedding_id
```

### Comparing `lightly-1.4.6/lightly/api/api_workflow_upload_metadata.py` & `lightly-1.4.7/lightly/api/api_workflow_upload_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from bisect import bisect_left
 from concurrent.futures import ThreadPoolExecutor
-from typing import Dict, List, Union
+from typing import Any, Dict, List, Union
 
+from requests import Response
 from tqdm import tqdm
 
 from lightly.api.utils import retry
 from lightly.openapi_generated.swagger_client.models.configuration_entry import (
     ConfigurationEntry,
 )
 from lightly.openapi_generated.swagger_client.models.configuration_set_request import (
@@ -21,27 +22,27 @@
 from lightly.utils.io import COCO_ANNOTATION_KEYS
 
 
 class InvalidCustomMetadataWarning(Warning):
     pass
 
 
-def _assert_key_exists_in_custom_metadata(key: str, dictionary: Dict):
+def _assert_key_exists_in_custom_metadata(key: str, dictionary: Dict[str, Any]):
     """Raises a formatted KeyError if key is not a key of the dictionary."""
     if key not in dictionary.keys():
         raise KeyError(
             f"Key {key} not found in custom metadata.\n"
             f"Found keys: {dictionary.keys()}"
         )
 
 
 class _UploadCustomMetadataMixin:
     """Mixin of helpers to allow upload of custom metadata."""
 
-    def verify_custom_metadata_format(self, custom_metadata: Dict):
+    def verify_custom_metadata_format(self, custom_metadata: Dict) -> None:
         """Verifies that the custom metadata is in the correct format.
 
         Args:
             custom_metadata:
                 Dictionary of custom metadata, see upload_custom_metadata for
                 the required format.
 
@@ -54,15 +55,15 @@
             COCO_ANNOTATION_KEYS.images, custom_metadata
         )
         _assert_key_exists_in_custom_metadata(
             COCO_ANNOTATION_KEYS.custom_metadata, custom_metadata
         )
 
     def index_custom_metadata_by_filename(
-        self, custom_metadata: Dict
+        self, custom_metadata: Dict[str, Any]
     ) -> Dict[str, Union[Dict, None]]:
         """Creates an index to lookup custom metadata by filename.
 
         Args:
             custom_metadata:
                 Dictionary of custom metadata, see upload_custom_metadata for
                 the required format.
@@ -89,22 +90,26 @@
         filename_to_metadata = {
             filename: image_id_to_custom_metadata.get(image_id, None)
             for (filename, image_id) in filename_to_image_id.items()
         }
         return filename_to_metadata
 
     def upload_custom_metadata(
-        self, custom_metadata: Dict, verbose: bool = False, max_workers: int = 8
-    ):
-        """Uploads custom metadata to the Lightly platform.
+        self,
+        custom_metadata: Dict[str, Any],
+        verbose: bool = False,
+        max_workers: int = 8,
+    ) -> None:
+        """Uploads custom metadata to the Lightly Platform.
 
         The custom metadata is expected in a format similar to the COCO annotations:
         Under the key "images" there should be a list of dictionaries, each with
-        a file_name and id. Under the key "metadata" the custom metadata is stored
-        as a list of dictionaries, each with a image_id to match it to the image.
+        a file_name and id. Under the key "metadata", the custom metadata is stored
+        as a list of dictionaries, each with an image ID that corresponds to an image
+        under the key "images".
 
         Example:
             >>> custom_metadata = {
             >>>     "images": [
             >>>         {
             >>>             "file_name": "image0.jpg",
             >>>             "id": 0,
@@ -134,15 +139,15 @@
             >>>     ]
             >>> }
 
         Args:
             custom_metadata:
                 Custom metadata as described above.
             verbose:
-                If True displays a progress bar during the upload.
+                If True, displays a progress bar during the upload.
             max_workers:
                 Maximum number of concurrent threads during upload.
 
         """
 
         self.verify_custom_metadata_format(custom_metadata)
 
@@ -209,22 +214,22 @@
             if verbose:
                 results = tqdm(results, unit="metadata", total=len(upload_requests))
             # iterate over results to make sure they are completed
             list(results)
 
     def create_custom_metadata_config(
         self, name: str, configs: List[ConfigurationEntry]
-    ):
+    ) -> Response:
         """Creates custom metadata config from a list of configurations.
 
         Args:
             name:
                 The name of the custom metadata configuration.
             configs:
-                List of configuration entries each specifying.
+                List of metadata configuration entries.
 
         Returns:
             The API response.
 
         Examples:
             >>> from lightly.openapi_generated.swagger_codegen.models.configuration_entry import ConfigurationEntry
             >>> entry = ConfigurationEntry(
```

### Comparing `lightly-1.4.6/lightly/api/bitmask.py` & `lightly-1.4.7/lightly/api/bitmask.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/api/download.py` & `lightly-1.4.7/lightly/api/download.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/api/patch.py` & `lightly-1.4.7/lightly/api/patch.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/api/prediction_singletons.py` & `lightly-1.4.7/lightly/api/prediction_singletons.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/api/swagger_api_client.py` & `lightly-1.4.7/lightly/api/swagger_api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/api/swagger_rest_client.py` & `lightly-1.4.7/lightly/api/swagger_rest_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/api/utils.py` & `lightly-1.4.7/lightly/api/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 import io
 import os
 import random
+import threading
 import time
 from enum import Enum
-from typing import List, Optional
+from typing import Iterator, List, Optional
 
 # the following two lines are needed because
 # PIL misidentifies certain jpeg images as MPOs
 from PIL import JpegImagePlugin
 
 JpegImagePlugin._getmp = lambda: None
 
@@ -62,38 +63,52 @@
             # max retries exceeded
             if current_retries >= max_retries:
                 raise RuntimeError(
                     f"Maximum retries exceeded! Original exception: {type(e)}: {str(e)}"
                 ) from e
 
 
-def paginate_endpoint(fn, page_size=5000, *args, **kwargs) -> List:
+class Paginated(Iterator):
+    def __init__(self, fn, page_size, *args, **kwargs):
+        self.entries: List = []
+        self.offset = 0
+        self.fn = fn
+        self.page_size = page_size
+        self.args = args
+        self.kwargs = kwargs
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if len(self.entries) == 0:
+            chunk = retry(
+                self.fn,
+                page_offset=self.offset * self.page_size,
+                page_size=self.page_size,
+                *self.args,
+                **self.kwargs,
+            )
+            if len(chunk) == 0:
+                raise StopIteration
+            self.offset += 1
+            self.entries.extend(chunk)
+        return self.entries.pop(0)
+
+
+def paginate_endpoint(fn, page_size=5000, *args, **kwargs) -> Iterator:
     """Paginates an API endpoint
 
     Args:
         fn:
             The endpoint which will be paginated until there is not any more data
         page_size:
             The size of the pages to pull
     """
-    entries: List = []
-    offset = 0
-    has_more = True
-    while has_more:
-        chunk = retry(
-            fn, page_offset=offset * page_size, page_size=page_size, *args, **kwargs
-        )
-        # if we don't find more data, stop pagination otherwise get next chunk
-        if len(chunk) == 0:
-            has_more = False
-        else:
-            entries.extend(chunk)
-            offset += 1
-
-    return entries
+    return Paginated(fn, page_size, *args, **kwargs)
 
 
 def getenv(key: str, default: str):
     """Return the value of the environment variable key if it exists,
     or default if it doesn’t.
 
     """
```

### Comparing `lightly-1.4.6/lightly/api/version_checking.py` & `lightly-1.4.7/lightly/api/version_checking.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/cli/_cli_simclr.py` & `lightly-1.4.7/lightly/cli/_cli_simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/cli/_helpers.py` & `lightly-1.4.7/lightly/cli/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/cli/config/config.yaml` & `lightly-1.4.7/lightly/cli/config/config.yaml`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/cli/crop_cli.py` & `lightly-1.4.7/lightly/cli/crop_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # All Rights Reserved
 import os.path
 from typing import List
 
 import hydra
 import yaml
 
-from lightly.active_learning.utils import BoundingBox
 from lightly.cli._helpers import fix_hydra_arguments, fix_input_path
 from lightly.data import LightlyDataset
+from lightly.utils.bounding_box import BoundingBox
 from lightly.utils.cropping.crop_image_by_bounding_boxes import (
     crop_dataset_by_bounding_boxes_and_save,
 )
 from lightly.utils.cropping.read_yolo_label_file import read_yolo_label_file
 from lightly.utils.hipify import bcolors
```

### Comparing `lightly-1.4.6/lightly/cli/download_cli.py` & `lightly-1.4.7/lightly/cli/download_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/cli/embed_cli.py` & `lightly-1.4.7/lightly/cli/embed_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/cli/train_cli.py` & `lightly-1.4.7/lightly/cli/train_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/cli/upload_cli.py` & `lightly-1.4.7/lightly/api/api_workflow_download_dataset.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,262 +1,318 @@
-# -*- coding: utf-8 -*-
-"""**Lightly Upload:** Upload images to the Lightly platform.
-
-This module contains the entrypoint for the **lightly-upload**
-command-line interface.
-"""
-
-# Copyright (c) 2020. Lightly AG and its affiliates.
-# All Rights Reserved
-import json
+import io
 import os
-from typing import Union
-
-import hydra
-import torchvision
+import warnings
+from concurrent.futures.thread import ThreadPoolExecutor
+from typing import Dict, List, Optional
+from urllib.request import Request, urlopen
+
+import tqdm
+from PIL import Image
+
+from lightly.api import download
+from lightly.api.bitmask import BitMask
+from lightly.api.utils import paginate_endpoint, retry
+from lightly.openapi_generated.swagger_client import (
+    DatasetEmbeddingData,
+    FileNameFormat,
+    ImageType,
+)
+from lightly.utils.hipify import bcolors
+
+
+def _make_dir_and_save_image(output_dir: str, filename: str, img: Image):
+    """Saves the images and creates necessary subdirectories."""
+    path = os.path.join(output_dir, filename)
+
+    head = os.path.split(path)[0]
+    if not os.path.exists(head):
+        os.makedirs(head)
+
+    img.save(path)
+    img.close()
+
+
+def _get_image_from_read_url(read_url: str):
+    """Makes a get request to the signed read url and returns the image."""
+    request = Request(read_url, method="GET")
+    with urlopen(request) as response:
+        blob = response.read()
+        img = Image.open(io.BytesIO(blob))
+    return img
+
+
+class _DownloadDatasetMixin:
+    def download_dataset(
+        self,
+        output_dir: str,
+        tag_name: str = "initial-tag",
+        max_workers: int = 8,
+        verbose: bool = True,
+    ) -> None:
+        """Downloads images from the web-app and stores them in output_dir.
+
+        Args:
+            output_dir:
+                Where to store the downloaded images.
+            tag_name:
+                Name of the tag which should be downloaded.
+            max_workers:
+                Maximum number of workers downloading images in parallel.
+            verbose:
+                Whether or not to show the progress bar.
+
+        Raises:
+            ValueError:
+                If the specified tag does not exist on the dataset.
+            RuntimeError:
+                If the connection to the server failed.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.download_dataset("/tmp/data")
+            Downloading 3 images (with 3 workers):
+            100%|██████████████████████████████████| 3/3 [00:01<00:00,  1.99imgs/s]
+        """
+
+        # check if images are available
+        dataset = self._datasets_api.get_dataset_by_id(self.dataset_id)
+        if dataset.img_type != ImageType.FULL:
+            # only thumbnails or metadata available
+            raise ValueError(
+                f"Dataset with id {self.dataset_id} has no downloadable images!"
+            )
 
-from lightly.api.api_workflow_client import ApiWorkflowClient
-from lightly.api.api_workflow_upload_embeddings import EmbeddingDoesNotExistError
-from lightly.cli._helpers import cpu_count, fix_hydra_arguments, fix_input_path
-from lightly.data import LightlyDataset
-from lightly.openapi_generated.swagger_client import Creator
-from lightly.utils.hipify import bcolors, print_as_warning
+        # check if tag exists
+        available_tags = self.get_all_tags()
+        try:
+            tag = next(tag for tag in available_tags if tag.name == tag_name)
+        except StopIteration:
+            raise ValueError(
+                f"Dataset with id {self.dataset_id} has no tag {tag_name}!"
+            )
 
-SUCCESS_RETURN_VALUE = "Success"
+        # get sample ids
+        sample_ids = self._mappings_api.get_sample_mappings_by_dataset_id(
+            self.dataset_id, field="_id"
+        )
 
+        indices = BitMask.from_hex(tag.bit_mask_data).to_indices()
+        sample_ids = [sample_ids[i] for i in indices]
 
-def _upload_cli(cfg, is_cli_call=True) -> Union[str, None]:
-    """
+        filenames_on_server = self.get_filenames()
+        filenames = [filenames_on_server[i] for i in indices]
 
-    Returns:
-        if no errors were encountered:
-            SUCCESS_RETURN_VALUE
-        else:
-            None
+        downloadables = zip(sample_ids, filenames)
 
-    """
-    # TODO (Malte, 19.01,2023): Remove the _upload_cli completely
-    print_as_warning(
-        message="DeprecationWarning: Uploading via CLI is deprecated and will be removed soon! "
-        "Please use the Lightly Worker instead: https://docs.lightly.ai/docs/install-lightly\n",
-    )
-
-    input_dir = cfg["input_dir"]
-    if input_dir and is_cli_call:
-        input_dir = fix_input_path(input_dir)
-
-    path_to_embeddings = cfg["embeddings"]
-    if path_to_embeddings and is_cli_call:
-        path_to_embeddings = fix_input_path(path_to_embeddings)
-
-    dataset_id = cfg["dataset_id"]
-    token = cfg["token"]
-    new_dataset_name = cfg["new_dataset_name"]
-
-    cli_api_args_wrong = False
-    if not token:
-        print_as_warning("Please specify your access token.")
-        cli_api_args_wrong = True
-
-    if dataset_id:
-        if new_dataset_name:
-            print_as_warning(
-                "Please specify either the dataset_id of an existing dataset "
-                "or a new_dataset_name, but not both."
+        # handle the case where len(sample_ids) < max_workers
+        max_workers = min(len(sample_ids), max_workers)
+        max_workers = max(max_workers, 1)
+
+        if verbose:
+            print(
+                f"Downloading {bcolors.OKGREEN}{len(sample_ids)}{bcolors.ENDC} images (with {bcolors.OKGREEN}{max_workers}{bcolors.ENDC} workers):",
+                flush=True,
             )
-            cli_api_args_wrong = True
-        else:
-            api_workflow_client = ApiWorkflowClient(
-                token=token,
-                dataset_id=dataset_id,
-                creator=Creator.USER_PIP_LIGHTLY_MAGIC,
-            )
-    else:
-        if new_dataset_name:
-            api_workflow_client = ApiWorkflowClient(
-                token=token, creator=Creator.USER_PIP_LIGHTLY_MAGIC
-            )
-            api_workflow_client.create_dataset(dataset_name=new_dataset_name)
-        else:
-            print_as_warning(
-                "Please specify either the dataset_id of an existing dataset "
-                "or a new_dataset_name."
-            )
-            cli_api_args_wrong = True
-    # delete the dataset_id as it might be an empty string
-    # Use api_workflow_client.dataset_id instead
-    del dataset_id
-
-    if cli_api_args_wrong:
-        print_as_warning("For help, try: lightly-upload --help")
-        return
-
-    # potentially load custom metadata
-    custom_metadata = None
-    if cfg["custom_metadata"]:
-        path_to_custom_metadata = fix_input_path(cfg["custom_metadata"])
-        print(
-            "Loading custom metadata from "
-            f"{bcolors.OKBLUE}{path_to_custom_metadata}{bcolors.ENDC}"
+            pbar = tqdm.tqdm(unit="imgs", total=len(sample_ids))
+            tqdm_lock = tqdm.tqdm.get_lock()
+
+        # define lambda function for concurrent download
+        def lambda_(i):
+            sample_id, filename = i
+            # try to download image
+            try:
+                read_url = self._samples_api.get_sample_image_read_url_by_id(
+                    self.dataset_id,
+                    sample_id,
+                    type="full",
+                )
+                img = _get_image_from_read_url(read_url)
+                _make_dir_and_save_image(output_dir, filename, img)
+                success = True
+            except Exception as e:  # pylint: disable=broad-except
+                warnings.warn(f"Downloading of image {filename} failed with error {e}")
+                success = False
+
+            # update the progress bar
+            if verbose:
+                tqdm_lock.acquire()
+                pbar.update(1)
+                tqdm_lock.release()
+            # return whether the download was successful
+            return success
+
+        with ThreadPoolExecutor(max_workers=max_workers) as executor:
+            results = list(executor.map(lambda_, downloadables, chunksize=1))
+
+        if not all(results):
+            msg = "Warning: Unsuccessful download! "
+            msg += "Failed at image: {}".format(results.index(False))
+            warnings.warn(msg)
+
+    def get_all_embedding_data(self) -> List[DatasetEmbeddingData]:
+        """Fetches embedding data of all embeddings for this dataset.
+
+        Returns:
+            A list of embedding data.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.get_all_embedding_data()
+            [{'created_at': 1684750552181,
+             'id': '646b40d88355e2f54c6d2235',
+             'is2d': False,
+             'is_processed': True,
+             'name': 'default_20230522_10h15m50s'}]
+        """
+        return self._embeddings_api.get_embeddings_by_dataset_id(
+            dataset_id=self.dataset_id
         )
-        with open(path_to_custom_metadata, "r") as f:
-            custom_metadata = json.load(f)
 
-    # set the number of workers if unset
-    if cfg["loader"]["num_workers"] < 0:
-        # set the number of workers to the number of CPUs available,
-        # but minimum of 8
-        num_workers = max(8, cpu_count())
-        num_workers = min(32, num_workers)
-        cfg["loader"]["num_workers"] = num_workers
-
-    size = cfg["resize"]
-    if not isinstance(size, int):
-        size = tuple(size)
-    transform = None
-    if isinstance(size, tuple) or size > 0:
-        transform = torchvision.transforms.Resize(size)
-
-    if input_dir:
-        if not cfg.append and len(api_workflow_client.get_all_tags()) > 0:
-            print_as_warning(
-                "The dataset you specified already has samples. "
-                "If you want to add additional samples, you need to specify "
-                "append=True as CLI argument."
-            )
-            return
+    def get_embedding_data_by_name(self, name: str) -> DatasetEmbeddingData:
+        """Fetches embedding data with the given name for this dataset.
+
+        Args:
+            name: Embedding name.
 
-        mode = cfg["upload"]
-        dataset = LightlyDataset(input_dir=input_dir, transform=transform)
-        api_workflow_client.upload_dataset(
-            input=dataset,
-            mode=mode,
-            max_workers=cfg["loader"]["num_workers"],
-            custom_metadata=custom_metadata,
+        Returns:
+            Embedding data.
+
+        Raises:
+            ValueError:
+                If no embedding with this name exists.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.get_embedding_data_by_name("embedding-data")
+            [{'created_at': 1654756552401,
+             'id': '646f346004d77b4e1424e67e',
+             'is2d': False,
+             'is_processed': True,
+             'name': 'embedding-data'}]
+        """
+        for embedding_data in self.get_all_embedding_data():
+            if embedding_data.name == name:
+                return embedding_data
+        raise ValueError(
+            f"There are no embeddings with name '{name}' for dataset with id "
+            f"'{self.dataset_id}'."
         )
-        print("Finished the upload of the dataset.")
 
-    if path_to_embeddings:
-        name = cfg["embedding_name"]
-        if not cfg.append:
-            try:
-                embedding = api_workflow_client.get_embedding_by_name(
-                    name=name, ignore_suffix=True
-                )
-                print_as_warning(
-                    "The dataset you specified already has an embedding. "
-                    "If you want to add additional samples, you need to specify "
-                    "append=True as CLI argument."
-                )
-                return
-            except EmbeddingDoesNotExistError:
-                pass
-        api_workflow_client.upload_embeddings(
-            path_to_embeddings_csv=path_to_embeddings, name=name
+    def download_embeddings_csv_by_id(
+        self,
+        embedding_id: str,
+        output_path: str,
+    ) -> None:
+        """Downloads embeddings with the given embedding id from the dataset.
+
+        Args:
+            embedding_id: ID of the embedding data to be downloaded.
+            output_path: Where the downloaded embedding data should be stored.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.download_embeddings_csv_by_id(
+            ...     embedding_id="646f346004d77b4e1424e67e",
+            ...     output_path="/tmp/embeddings.csv"
+            ... )
+            >>>
+            >>> # File content:
+            >>> # filenames,embedding_0,embedding_1,embedding_...,labels
+            >>> # image-1.png,0.2124302,-0.26934767,...,0
+        """
+        read_url = self._embeddings_api.get_embeddings_csv_read_url_by_id(
+            dataset_id=self.dataset_id, embedding_id=embedding_id
         )
-        print("Finished upload of embeddings.")
+        download.download_and_write_file(url=read_url, output_path=output_path)
+
+    def download_embeddings_csv(self, output_path: str) -> None:
+        """Downloads the latest embeddings from the dataset.
 
-    if custom_metadata is not None and not input_dir:
-        # upload custom metadata separately
-        api_workflow_client.upload_custom_metadata(
-            custom_metadata,
-            verbose=True,
-            max_workers=cfg["loader"]["num_workers"],
+        Args:
+            output_path: Where the downloaded embedding data should be stored.
+
+        Raises:
+            RuntimeError:
+                If no embeddings could be found for the dataset.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.download_embeddings_csv(output_path="/tmp/embeddings.csv")
+            >>>
+            >>> # File content:
+            >>> # filenames,embedding_0,embedding_1,embedding_...,labels
+            >>> # image-1.png,0.2124302,-0.26934767,...,0
+        """
+        last_embedding = _get_latest_default_embedding_data(
+            embeddings=self.get_all_embedding_data()
+        )
+        if last_embedding is None:
+            raise RuntimeError(
+                f"Could not find embeddings for dataset with id '{self.dataset_id}'."
+            )
+        self.download_embeddings_csv_by_id(
+            embedding_id=last_embedding.id,
+            output_path=output_path,
         )
 
-    if new_dataset_name:
-        print(
-            f"The dataset_id of the newly created dataset is "
-            f"{bcolors.OKBLUE}{api_workflow_client.dataset_id}{bcolors.ENDC}"
+    def export_label_studio_tasks_by_tag_id(
+        self,
+        tag_id: str,
+    ) -> List[Dict]:
+        """Exports samples in a format compatible with Label Studio.
+
+        The format is documented here:
+        https://labelstud.io/guide/tasks.html#Basic-Label-Studio-JSON-format
+
+        Args:
+            tag_id:
+                Id of the tag which should exported.
+
+        Returns:
+            A list of dictionaries in a format compatible with Label Studio.
+
+        Examples:
+            >>> client = ApiWorkflowClient(token="MY_AWESOME_TOKEN")
+            >>>
+            >>> # Already created some Lightly Worker runs with this dataset
+            >>> client.set_dataset_id_by_name("my-dataset")
+            >>> client.export_label_studio_tasks_by_tag_id(tag_id="646f34608a5613b57d8b73cc")
+            [{'id': 0, 'data': {'image': '...', ...}}]
+        """
+        label_studio_tasks = list(
+            paginate_endpoint(
+                self._tags_api.export_tag_to_label_studio_tasks,
+                page_size=20000,
+                dataset_id=self.dataset_id,
+                tag_id=tag_id,
+            )
         )
+        return label_studio_tasks
 
-    os.environ[
-        cfg["environment_variable_names"]["lightly_last_dataset_id"]
-    ] = api_workflow_client.dataset_id
-
-    return SUCCESS_RETURN_VALUE
-
-
-@hydra.main(**fix_hydra_arguments(config_path="config", config_name="config"))
-def upload_cli(cfg):
-    """Upload images/embeddings from the command-line to the Lightly platform.
-
-    Args:
-        cfg:
-            The default configs are loaded from the config file.
-            To overwrite them please see the section on the config file
-            (.config.config.yaml).
-
-    Command-Line Args:
-        input_dir:
-            Path to the input directory where images are stored.
-        embeddings:
-            Path to the csv file storing the embeddings generated by
-            lightly.
-        token:
-            User access token to the Lightly platform. If needs to be
-            specified to upload the images and embeddings to the platform.
-        dataset_id:
-            Identifier of the dataset on the Lightly platform.
-            Either the dataset_id or the new_dataset_name need to be
-            specified.
-        new_dataset_name:
-            The name of the new dataset to create on the Lightly platform.
-            Either the dataset_id or the new_dataset_name need to be
-            specified.
-        upload:
-            String to determine whether to upload the full images,
-            thumbnails only, or metadata only.
-
-            Must be one of ['full', 'thumbnails', 'metadata']
-        embedding_name:
-            Assign the embedding a name in order to identify it on the
-            Lightly platform.
-        resize:
-            Desired size of the uploaded images. If negative, default size is
-            used. If size is a sequence like (h, w), output size will be matched
-            to this. If size is an int, smaller edge of the image will be
-            matched to this number. i.e, if height > width, then image will be
-            rescaled to (size * height / width, size).
-        custom_metadata:
-            Path to a .json file containing custom metadata. The file must be in
-            the COCO annotations (although annotations can be empty) format and
-            contain an additional field `metadata` storing a list of metadata
-            entries. The metadata entries are matched with the images via
-            `image_id`.
-
-    Examples:
-        >>> # create a new dataset on the Lightly platform and upload full images to it
-        >>> lightly-upload input_dir=data/ token='123' new_dataset_name='new_dataset_name_xyz'
-        >>>
-        >>> # upload full images to the Lightly platform to an existing dataset
-        >>> lightly-upload input_dir=data/ token='123' dataset_id='XYZ'
-        >>>
-        >>> # create a new dataset on the Lightly platform and upload thumbnails to it
-        >>> lightly-upload input_dir=data/ token='123' new_dataset_name='new_dataset_name_xyz' upload='thumbnails'
-        >>>
-        >>> # upload metadata to the Lightly platform
-        >>> lightly-upload input_dir=data/ token='123' dataset_id='XYZ' upload='metadata'
-        >>>
-        >>> # upload embeddings to the Lightly platform (must have uploaded images beforehand)
-        >>> lightly-upload embeddings=embeddings.csv token='123' dataset_id='XYZ'
-        >>>
-        >>> # upload both, images and embeddings in a single command
-        >>> lightly-upload input_dir=data/ embeddings=embeddings.csv upload='full' \\
-        >>>     token='123' dataset_id='XYZ'
-        >>>
-        >>> # create a new dataset on the Lightly platform and upload both, images and embeddings
-        >>> lightly-upload input_dir=data/ embeddings=embeddings.csv upload='full' \\
-        >>>     token='123' new_dataset_name='new_dataset_name_xyz'
-        >>>
-        >>> # upload a dataset with custom metadata
-        >>> lightly-upload input_dir=data/ token='123' dataset_id='XYZ' custom_metadata=custom_metadata.json
-        >>>
-        >>> # upload custom metadata to an existing dataset
-        >>> lightly-upload token='123' dataset_id='XYZ' custom_metadata=custom_metadata.json
 
+def _get_latest_default_embedding_data(
+    embeddings: List[DatasetEmbeddingData],
+) -> Optional[DatasetEmbeddingData]:
+    """Returns the latest embedding data with a default name or None if no such
+    default embedding exists.
     """
-    return _upload_cli(cfg)
-
-
-def entry():
-    upload_cli()
+    default_embeddings = [e for e in embeddings if e.name.startswith("default")]
+    if default_embeddings:
+        last_embedding = sorted(default_embeddings, key=lambda e: e.created_at)[-1]
+        return last_embedding
+    else:
+        return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lightly-1.4.6/lightly/cli/version_cli.py` & `lightly-1.4.7/lightly/cli/version_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/core.py` & `lightly-1.4.7/lightly/core.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/data/__init__.py` & `lightly-1.4.7/lightly/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/data/_helpers.py` & `lightly-1.4.7/lightly/data/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/data/_image.py` & `lightly-1.4.7/lightly/data/_image.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/data/_image_loaders.py` & `lightly-1.4.7/lightly/data/_image_loaders.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/data/_utils.py` & `lightly-1.4.7/lightly/data/_utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/data/_video.py` & `lightly-1.4.7/lightly/data/_video.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/data/collate.py` & `lightly-1.4.7/lightly/data/collate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1344,11 +1344,10 @@
 
         return (views_global, views_local, grids_global, grids_local), labels, fnames
 
 
 def _deprecation_warning_collate_functions() -> None:
     warn(
         "Collate functions are deprecated and will be removed in favor of transforms in v1.4.0.\n"
-        "Please use MultiViewCollate in `lightly.data.multi_view_collate` together with the correct transform for your model instead.\n"
         "See https://docs.lightly.ai/self-supervised-learning/examples/models.html for examples.",
         category=DeprecationWarning,
     )
```

### Comparing `lightly-1.4.6/lightly/data/dataset.py` & `lightly-1.4.7/lightly/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/data/lightly_subset.py` & `lightly-1.4.7/lightly/data/lightly_subset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/data/multi_view_collate.py` & `lightly-1.4.7/lightly/data/multi_view_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/embedding/_base.py` & `lightly-1.4.7/lightly/embedding/_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/embedding/callbacks.py` & `lightly-1.4.7/lightly/embedding/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/embedding/embedding.py` & `lightly-1.4.7/lightly/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/__init__.py` & `lightly-1.4.7/lightly/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/barlow_twins_loss.py` & `lightly-1.4.7/lightly/loss/barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/dcl_loss.py` & `lightly-1.4.7/lightly/loss/dcl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/dino_loss.py` & `lightly-1.4.7/lightly/loss/dino_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/hypersphere_loss.py` & `lightly-1.4.7/lightly/loss/hypersphere_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/memory_bank.py` & `lightly-1.4.7/lightly/loss/memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/msn_loss.py` & `lightly-1.4.7/lightly/loss/msn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/negative_cosine_similarity.py` & `lightly-1.4.7/lightly/loss/negative_cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/ntx_ent_loss.py` & `lightly-1.4.7/lightly/loss/ntx_ent_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/pmsn_loss.py` & `lightly-1.4.7/lightly/loss/pmsn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/regularizer/co2.py` & `lightly-1.4.7/lightly/loss/regularizer/co2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/swav_loss.py` & `lightly-1.4.7/lightly/loss/swav_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/sym_neg_cos_sim_loss.py` & `lightly-1.4.7/lightly/loss/sym_neg_cos_sim_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/tico_loss.py` & `lightly-1.4.7/lightly/loss/tico_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/vicreg_loss.py` & `lightly-1.4.7/lightly/loss/vicreg_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/loss/vicregl_loss.py` & `lightly-1.4.7/lightly/loss/vicregl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/__init__.py` & `lightly-1.4.7/lightly/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/_momentum.py` & `lightly-1.4.7/lightly/models/_momentum.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/barlowtwins.py` & `lightly-1.4.7/lightly/models/barlowtwins.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/batchnorm.py` & `lightly-1.4.7/lightly/models/batchnorm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/byol.py` & `lightly-1.4.7/lightly/models/byol.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/moco.py` & `lightly-1.4.7/lightly/models/moco.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/modules/__init__.py` & `lightly-1.4.7/lightly/models/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/modules/heads.py` & `lightly-1.4.7/lightly/models/modules/heads.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/modules/masked_autoencoder.py` & `lightly-1.4.7/lightly/models/modules/masked_autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/modules/nn_memory_bank.py` & `lightly-1.4.7/lightly/models/modules/nn_memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/nnclr.py` & `lightly-1.4.7/lightly/models/nnclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/resnet.py` & `lightly-1.4.7/lightly/models/resnet.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/simclr.py` & `lightly-1.4.7/lightly/models/simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/simsiam.py` & `lightly-1.4.7/lightly/models/simsiam.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/utils.py` & `lightly-1.4.7/lightly/models/utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/models/zoo.py` & `lightly-1.4.7/lightly/models/zoo.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/__init__.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/__init__.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/collaboration_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/collaboration_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/datasets_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/datasources_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/datasources_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/docker_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/docker_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/embeddings_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/embeddings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/jobs_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/mappings_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/mappings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/predictions_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/predictions_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/quota_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/quota_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/samples_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/samples_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/samplings_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/samplings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/scores_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/scores_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/tags_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/teams_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/versioning_api.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api/versioning_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/api_client.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/configuration.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/__init__.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/access_role.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/access_role.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_scores.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/active_learning_scores.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/api_error_code.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/api_error_code.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/api_error_response.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/async_task_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/async_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/bounding_box.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/category_id.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/category_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/category_name.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/category_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/configuration_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_entry.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/configuration_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_set_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/configuration_set_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_entity_response.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/create_entity_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/creator.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/crop_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/crop_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_creator.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_name.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_name_query.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_name_query.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_update_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dataset_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_base.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_local.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_local.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_purpose.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_purpose.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_license_information.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_license_information.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_state.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_task_description.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_task_description.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_user_stats.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_user_stats.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_name.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_state.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/docker_worker_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/embedding2d_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/file_name_format.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/file_name_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/file_output_format.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/file_output_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/general_job_result.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/general_job_result.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/image_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/image_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_result_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_result_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_state.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_status_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_data_result.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_status_data_result.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_meta.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_status_meta.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/jobs_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/jobs_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_data_row.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_box_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_task.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_studio_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/mongo_object_id.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/mongo_object_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/object_id.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/object_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/path_safe_name.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/path_safe_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singletons.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_singletons.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/probabilities.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/probabilities.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/questionnaire_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/questionnaire_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/read_url.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/redirected_read_url.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/redirected_read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/s3_region.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/s3_region.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_task.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sama_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_task_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sama_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_tasks.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sama_tasks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_data_modes.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_data_modes.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_meta_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_sort_by.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_sort_by.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_update_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_write_urls.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sample_write_urls.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_config.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sampling_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sampling_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_method.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sampling_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/score.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/score.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sector.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/sector.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_config_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_input_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_input_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/shared_access_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_entry.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_change_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_create_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_creator.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_name.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_update_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/task_name.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/task_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/task_type.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/task_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/team_basic_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/team_basic_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/team_role.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/team_role.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/timestamp.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/timestamp.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/version_number.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/version_number.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/video_frame_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/video_frame_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/openapi_generated/swagger_client/rest.py` & `lightly-1.4.7/lightly/openapi_generated/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/__init__.py` & `lightly-1.4.7/lightly/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/dino_transform.py` & `lightly-1.4.7/lightly/transforms/dino_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/fast_siam_transform.py` & `lightly-1.4.7/lightly/transforms/fast_siam_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/gaussian_blur.py` & `lightly-1.4.7/lightly/transforms/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/image_grid_transform.py` & `lightly-1.4.7/lightly/transforms/image_grid_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/jigsaw.py` & `lightly-1.4.7/lightly/transforms/jigsaw.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/mae_transform.py` & `lightly-1.4.7/lightly/transforms/mae_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/moco_transform.py` & `lightly-1.4.7/lightly/transforms/moco_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/msn_transform.py` & `lightly-1.4.7/lightly/transforms/msn_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/multi_crop_transform.py` & `lightly-1.4.7/lightly/transforms/multi_crop_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/multi_view_transform.py` & `lightly-1.4.7/lightly/transforms/multi_view_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/pirl_transform.py` & `lightly-1.4.7/lightly/transforms/pirl_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/random_crop_and_flip_with_grid.py` & `lightly-1.4.7/lightly/transforms/random_crop_and_flip_with_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,26 +134,28 @@
     def __init__(
         self,
         grid_size: int = 7,
         crop_size: int = 224,
         crop_min_scale: float = 0.05,
         crop_max_scale: float = 0.2,
         hf_prob: float = 0.5,
+        vf_prob: float = 0.5,
     ):
         super().__init__()
         self.grid_size = grid_size
         self.crop_size = crop_size
         self.crop_min_scale = crop_min_scale
         self.crop_max_scale = crop_max_scale
         self.hf_prob = hf_prob
+        self.vf_prob = vf_prob
         self.resized_crop = RandomResizedCropWithLocation(
             size=self.crop_size, scale=(self.crop_min_scale, self.crop_max_scale)
         )
         self.horizontal_flip = RandomHorizontalFlipWithLocation(self.hf_prob)
-        self.vertical_flip = RandomVerticalFlipWithLocation(self.hf_prob)
+        self.vertical_flip = RandomVerticalFlipWithLocation(self.vf_prob)
 
     def forward(self, img: Image.Image) -> Tuple[Image.Image, torch.Tensor]:
         """Applies random cropping and horizontal flipping to an image, and returns the
         transformed image and a grid tensor used to map the image back to the original image
         space in an NxN grid.
 
         Args:
```

### Comparing `lightly-1.4.6/lightly/transforms/rotation.py` & `lightly-1.4.7/lightly/transforms/rotation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/simclr_transform.py` & `lightly-1.4.7/lightly/transforms/simclr_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/simsiam_transform.py` & `lightly-1.4.7/lightly/transforms/simsiam_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/smog_transform.py` & `lightly-1.4.7/lightly/transforms/smog_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/solarize.py` & `lightly-1.4.7/lightly/transforms/solarize.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/swav_transform.py` & `lightly-1.4.7/lightly/transforms/swav_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/vicreg_transform.py` & `lightly-1.4.7/lightly/transforms/vicreg_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/transforms/vicregl_transform.py` & `lightly-1.4.7/lightly/transforms/vicregl_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         global_gaussian_blur_kernel_size: Optional[float] = None,
         local_gaussian_blur_kernel_size: Optional[float] = None,
         global_gaussian_blur_sigmas: Tuple[float, float] = (0.1, 2),
         local_gaussian_blur_sigmas: Tuple[float, float] = (0.1, 2),
         global_solarize_prob: float = 0.0,
         local_solarize_prob: float = 0.2,
         hf_prob: float = 0.5,
+        vf_prob: float = 0.0,
         cj_prob: float = 1.0,
         cj_strength: float = 0.5,
         cj_bright: float = 0.8,
         cj_contrast: float = 0.8,
         cj_sat: float = 0.4,
         cj_hue: float = 0.2,
         random_gray_scale: float = 0.2,
@@ -111,14 +112,15 @@
     ):
         global_transform = (
             RandomResizedCropAndFlip(
                 crop_size=global_crop_size,
                 crop_min_scale=global_crop_scale[0],
                 crop_max_scale=global_crop_scale[1],
                 hf_prob=hf_prob,
+                vf_prob=vf_prob,
                 grid_size=global_grid_size,
             ),
             VICRegLViewTransform(
                 gaussian_blur_prob=global_gaussian_blur_prob,
                 gaussian_blur_kernel_size=global_gaussian_blur_kernel_size,
                 gaussian_blur_sigmas=global_gaussian_blur_sigmas,
                 solarize_prob=global_solarize_prob,
```

### Comparing `lightly-1.4.6/lightly/utils/cropping/crop_image_by_bounding_boxes.py` & `lightly-1.4.7/lightly/utils/cropping/crop_image_by_bounding_boxes.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import warnings
 from pathlib import Path
 from typing import List
 
 from PIL import Image
 from tqdm import tqdm
 
-from lightly.active_learning.utils import BoundingBox
 from lightly.data import LightlyDataset
+from lightly.utils.bounding_box import BoundingBox
 
 
 def crop_dataset_by_bounding_boxes_and_save(
     dataset: LightlyDataset,
     output_dir: str,
     bounding_boxes_list_list: List[List[BoundingBox]],
     class_indices_list_list: List[List[int]],
```

### Comparing `lightly-1.4.6/lightly/utils/cropping/read_yolo_label_file.py` & `lightly-1.4.7/lightly/utils/cropping/read_yolo_label_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Tuple
 
-from lightly.active_learning.utils import BoundingBox
+from lightly.utils.bounding_box import BoundingBox
 
 
 def read_yolo_label_file(
     filepath: str, padding: float, separator: str = " "
 ) -> Tuple[List[int], List[BoundingBox]]:
     """Reads a file in the yolo file format
```

### Comparing `lightly-1.4.6/lightly/utils/debug.py` & `lightly-1.4.7/lightly/utils/debug.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/utils/dist.py` & `lightly-1.4.7/lightly/utils/dist.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/utils/embeddings_2d.py` & `lightly-1.4.7/lightly/utils/embeddings_2d.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/utils/hipify.py` & `lightly-1.4.7/lightly/utils/hipify.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/utils/io.py` & `lightly-1.4.7/lightly/utils/io.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/utils/lars.py` & `lightly-1.4.7/lightly/utils/lars.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/utils/reordering.py` & `lightly-1.4.7/lightly/utils/reordering.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/utils/scheduler.py` & `lightly-1.4.7/lightly/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly/utils/version_compare.py` & `lightly-1.4.7/lightly/utils/version_compare.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/lightly.egg-info/PKG-INFO` & `lightly-1.4.7/lightly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.4.6
+Version: 1.4.7
 Summary: A deep learning package for self-supervised learning
 Author: Philipp Wirth & Igor Susmelj
 Author-email: philipp@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
```

### Comparing `lightly-1.4.6/lightly.egg-info/SOURCES.txt` & `lightly-1.4.7/lightly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,16 @@
 lightly.egg-info/PKG-INFO
 lightly.egg-info/SOURCES.txt
 lightly.egg-info/dependency_links.txt
 lightly.egg-info/entry_points.txt
 lightly.egg-info/requires.txt
 lightly.egg-info/top_level.txt
 lightly/active_learning/__init__.py
-lightly/active_learning/agents/__init__.py
-lightly/active_learning/agents/agent.py
 lightly/active_learning/config/__init__.py
 lightly/active_learning/config/selection_config.py
-lightly/active_learning/scorers/__init__.py
-lightly/active_learning/scorers/classification.py
-lightly/active_learning/scorers/detection.py
-lightly/active_learning/scorers/keypoint_detection.py
-lightly/active_learning/scorers/scorer.py
-lightly/active_learning/scorers/semantic_segmentation.py
-lightly/active_learning/utils/__init__.py
-lightly/active_learning/utils/bounding_box.py
-lightly/active_learning/utils/keypoint_predictions.py
-lightly/active_learning/utils/object_detection_output.py
 lightly/api/__init__.py
 lightly/api/api_workflow_artifacts.py
 lightly/api/api_workflow_client.py
 lightly/api/api_workflow_collaboration.py
 lightly/api/api_workflow_compute_worker.py
 lightly/api/api_workflow_datasets.py
 lightly/api/api_workflow_datasources.py
@@ -54,15 +42,14 @@
 lightly/cli/_cli_simclr.py
 lightly/cli/_helpers.py
 lightly/cli/crop_cli.py
 lightly/cli/download_cli.py
 lightly/cli/embed_cli.py
 lightly/cli/lightly_cli.py
 lightly/cli/train_cli.py
-lightly/cli/upload_cli.py
 lightly/cli/version_cli.py
 lightly/cli/config/__init__.py
 lightly/cli/config/config.yaml
 lightly/cli/config/get_config.py
 lightly/data/__init__.py
 lightly/data/_helpers.py
 lightly/data/_image.py
@@ -368,18 +355,27 @@
 lightly/transforms/smog_transform.py
 lightly/transforms/solarize.py
 lightly/transforms/swav_transform.py
 lightly/transforms/utils.py
 lightly/transforms/vicreg_transform.py
 lightly/transforms/vicregl_transform.py
 lightly/utils/__init__.py
+lightly/utils/bounding_box.py
 lightly/utils/debug.py
 lightly/utils/dist.py
 lightly/utils/embeddings_2d.py
 lightly/utils/hipify.py
 lightly/utils/io.py
 lightly/utils/lars.py
 lightly/utils/reordering.py
 lightly/utils/scheduler.py
 lightly/utils/version_compare.py
+lightly/utils/benchmarking/__init__.py
+lightly/utils/benchmarking/benchmark_module.py
+lightly/utils/benchmarking/knn.py
+lightly/utils/benchmarking/knn_classifier.py
+lightly/utils/benchmarking/linear_classifier.py
+lightly/utils/benchmarking/metric_callback.py
+lightly/utils/benchmarking/online_linear_classifier.py
+lightly/utils/benchmarking/topk.py
 lightly/utils/cropping/crop_image_by_bounding_boxes.py
 lightly/utils/cropping/read_yolo_label_file.py
```

### Comparing `lightly-1.4.6/lightly.egg-info/requires.txt` & `lightly-1.4.7/lightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.4.6/setup.py` & `lightly-1.4.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
     entry_points = {
         "console_scripts": [
             "lightly-crop = lightly.cli.crop_cli:entry",
             "lightly-train = lightly.cli.train_cli:entry",
             "lightly-embed = lightly.cli.embed_cli:entry",
             "lightly-magic = lightly.cli.lightly_cli:entry",
-            "lightly-upload = lightly.cli.upload_cli:entry",
             "lightly-download = lightly.cli.download_cli:entry",
             "lightly-version = lightly.cli.version_cli:entry",
         ]
     }
 
     long_description = load_description()
 
@@ -87,20 +86,18 @@
         "lightly.embedding",
         "lightly.loss",
         "lightly.loss.regularizer",
         "lightly.models",
         "lightly.models.modules",
         "lightly.transforms",
         "lightly.utils",
+        "lightly.utils.benchmarking",
         "lightly.utils.cropping",
         "lightly.active_learning",
-        "lightly.active_learning.agents",
         "lightly.active_learning.config",
-        "lightly.active_learning.scorers",
-        "lightly.active_learning.utils",
         "lightly.openapi_generated",
         "lightly.openapi_generated.swagger_client",
         "lightly.openapi_generated.swagger_client.api",
         "lightly.openapi_generated.swagger_client.models",
     ]
 
     project_urls = {
```

