# Comparing `tmp/ml-management-0.0.34.tar.gz` & `tmp/ml-management-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.34.tar", last modified: Tue May 30 12:44:33 2023, max compression
+gzip compressed data, was "dist/ml-management-0.0.35.tar", last modified: Wed Jun  7 14:31:26 2023, max compression
```

## Comparing `ml-management-0.0.34.tar` & `ml-management-0.0.35.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       18 2023-02-15 13:35:59.000000 ml-management-0.0.34/MANIFEST.in
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.34/ML_management/__init__.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/collectors/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      120 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1092 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      456 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1318 2023-05-30 12:24:50.000000 ml-management-0.0.34/ML_management/collectors/collectors.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/collectors/dummy/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      463 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/collectors/s3/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    10557 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/collectors/topic_markers/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)   331440 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3167 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/dataset_loader_template/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2407 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.673273 ml-management-0.0.34/ML_management/executor_template/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/executor_template/default_executors/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      895 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      843 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      869 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4566 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      402 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      334 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/mlmanagement/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      581 2023-03-13 10:54:54.000000 ml-management-0.0.34/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3392 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5054 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    12327 2023-05-30 12:24:50.000000 ml-management-0.0.34/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    10262 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      201 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5001 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      316 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/models/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.34/ML_management/models/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      949 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/models/patterns/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4202 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      561 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      445 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/registry/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.34/ML_management/registry/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2566 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/registry/exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     7556 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/tests/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.34/ML_management/tests/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3361 2023-02-15 13:35:59.000000 ml-management-0.0.34/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     9298 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ML_management/uploader_data/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1582 2023-05-26 11:00:04.000000 ml-management-0.0.34/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      312 2023-05-30 12:44:33.677273 ml-management-0.0.34/PKG-INFO
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       56 2023-02-15 13:35:59.000000 ml-management-0.0.34/README.md
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        7 2023-05-30 12:44:18.000000 ml-management-0.0.34/VERSION
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-30 12:44:33.677273 ml-management-0.0.34/ml_management.egg-info/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      312 2023-05-30 12:44:33.000000 ml-management-0.0.34/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2449 2023-05-30 12:44:33.000000 ml-management-0.0.34/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        1 2023-05-30 12:44:33.000000 ml-management-0.0.34/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      154 2023-05-30 12:44:33.000000 ml-management-0.0.34/ml_management.egg-info/requires.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       14 2023-05-30 12:44:33.000000 ml-management-0.0.34/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       38 2023-05-30 12:44:33.677273 ml-management-0.0.34/setup.cfg
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1053 2023-05-30 12:24:50.000000 ml-management-0.0.34/setup.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.313684 ml-management-0.0.35/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)       18 2022-11-15 15:35:02.000000 ml-management-0.0.35/MANIFEST.in
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.305684 ml-management-0.0.35/ML_management/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.35/ML_management/__init__.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/collectors/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      120 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     1092 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      456 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     1318 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/collectors.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/collectors/dummy/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      463 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/collectors/s3/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)    10557 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)   331440 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     3167 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/dataset_loader_template/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     2407 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      457 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/executor_template/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      895 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      843 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      869 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     4566 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      402 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      334 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/mlmanagement/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      581 2022-09-29 11:08:30.000000 ml-management-0.0.35/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     3392 2023-03-13 16:12:20.000000 ml-management-0.0.35/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     5054 2023-03-13 16:12:20.000000 ml-management-0.0.35/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)    13486 2023-06-07 12:57:40.000000 ml-management-0.0.35/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)    10262 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      201 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     5001 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      316 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/models/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.35/ML_management/models/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      949 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/models/patterns/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     4202 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      561 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      445 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      457 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/registry/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.35/ML_management/registry/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     2566 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/registry/exceptions.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     7556 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/tests/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-12-07 10:58:45.000000 ml-management-0.0.35/ML_management/tests/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     3361 2022-12-07 10:58:45.000000 ml-management-0.0.35/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     9298 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.313684 ml-management-0.0.35/ML_management/uploader_data/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     1582 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      312 2023-06-07 14:31:26.313684 ml-management-0.0.35/PKG-INFO
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)       56 2022-08-01 13:04:47.000000 ml-management-0.0.35/README.md
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        7 2023-06-07 14:31:07.000000 ml-management-0.0.35/VERSION
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.313684 ml-management-0.0.35/ml_management.egg-info/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      312 2023-06-07 14:31:26.000000 ml-management-0.0.35/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     2449 2023-06-07 14:31:26.000000 ml-management-0.0.35/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        1 2023-06-07 14:31:26.000000 ml-management-0.0.35/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      154 2023-06-07 14:31:26.000000 ml-management-0.0.35/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)       14 2023-06-07 14:31:26.000000 ml-management-0.0.35/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)       38 2023-06-07 14:31:26.313684 ml-management-0.0.35/setup.cfg
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     1053 2023-05-31 08:55:31.000000 ml-management-0.0.35/setup.py
```

### Comparing `ml-management-0.0.34/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.35/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/collectors/collectors.py` & `ml-management-0.0.35/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.35/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.35/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.35/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.35/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.35/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.35/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.35/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.35/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.35/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.35/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.35/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.35/ML_management/mlmanagement/mlmanagement.py`

 * *Files 11% similar despite different names*

```diff
@@ -102,14 +102,63 @@
             ).format(active_run_stack[0].info.run_id)
         )
     _active_run = request_for_function(inspect.currentframe())
     active_run_stack.append(_active_run)
     return _active_run
 
 
+def _add_job_registration_metainfo(
+    registration_timestamp,
+    init_model_version_run_id,
+    name,
+    job_executor_name,
+    job_executor_version,
+    dataset_loader_name,
+    dataset_loader_version,
+    model_name,
+    model_version,
+    new_model_name,
+    experiment_name,
+    periodic_type,
+    cron_expression,
+    metric_name,
+    optimal_min,
+    choice_criteria,
+    executor_model_params_json,
+    data_params_json,
+    collector_name,
+):
+    """Add job metainfo on job registration. For internal use only."""
+    return request_for_function(inspect.currentframe())
+
+
+def _add_job_start_metainfo(
+    job_name,
+    start_timestamp,
+):
+    """Add job metainfo on execution start. For internal use only."""
+    return request_for_function(inspect.currentframe())
+
+
+def _add_job_end_metainfo(
+    job_name,
+    end_timestamp,
+):
+    """Add job metainfo on execution end. For internal use only."""
+    return request_for_function(inspect.currentframe())
+
+
+def _add_job_fail_metainfo(
+    job_name,
+    end_timestamp,
+):
+    """Add job metainfo on execution fail. For internal use only."""
+    return request_for_function(inspect.currentframe())
+
+
 def log_model(
     artifact_path,
     upload_model_mode: Optional[UploadModelMode] = None,
     loader_module=None,
     data_path=None,
     code_path=None,
     conda_env=None,
```

### Comparing `ml-management-0.0.34/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.35/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.35/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.35/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.35/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.35/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/registry/exceptions.py` & `ml-management-0.0.35/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/registry/registry_manager.py` & `ml-management-0.0.35/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.35/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.35/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.35/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.35/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.34/setup.py` & `ml-management-0.0.35/setup.py`

 * *Files identical despite different names*

