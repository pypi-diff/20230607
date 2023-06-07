# Comparing `tmp/tfx-addons-0.6.0rc1.tar.gz` & `tmp/tfx-addons-0.7.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/tfx-addons/tfx-addons/dist/.tmp-7jaz0tqq/tfx-addons-0.6.0rc1.tar", last modified: Mon Apr 17 23:51:57 2023, max compression
+gzip compressed data, was "/home/runner/work/tfx-addons/tfx-addons/dist/.tmp-meyaubuz/tfx-addons-0.7.0rc0.tar", last modified: Wed Jun  7 16:07:34 2023, max compression
```

## Comparing `tfx-addons-0.6.0rc1.tar` & `tfx-addons-0.7.0rc0.tar`

### file list

```diff
@@ -1,111 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/component_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/executor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feature_selection/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feature_selection/component_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/feature_selection/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/feature_selection/example/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feature_selection/example/modules/iris_module_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feature_selection/example/modules/penguins_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/feature_selection/example/modules/pima_indians_module_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/component_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/runner_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/component_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/executor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/runner_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/component_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/base_provider_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/logging_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/logging_provider_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/slack_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/slack_provider_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/mlmd_client/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/mlmd_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/mlmd_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/mlmd_client/client_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/artifact_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/component_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/executor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/tfxtest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/pandas_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/pandas_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/pandas_transform/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/pandas_transform/component_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/pandas_transform/null_preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/sampling/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/sampling/component_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/sampling/example/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/sampling/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/sampling/example/sampler_pipeline_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/sampling/example/sampler_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/sampling/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/sampling/executor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/sampling/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/component/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/component/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/component/component_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/component/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/component/executor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/example/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/example/module_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/example/taxi_example_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/test_data/module_file/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/test_data/module_file/module_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/test_data/schema_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/schema_curation/test_data/schema_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons/xgboost_evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/xgboost_evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/xgboost_evaluator/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/xgboost_evaluator/xgboost_predict_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-04-17 23:51:45.000000 tfx-addons-0.6.0rc1/tfx_addons/xgboost_evaluator/xgboost_predict_extractor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 23:51:57.000000 tfx-addons-0.6.0rc1/tfx_addons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/executor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feature_selection/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feature_selection/component_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/feature_selection/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/feature_selection/example/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feature_selection/example/modules/iris_module_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feature_selection/example/modules/penguins_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/feature_selection/example/modules/pima_indians_module_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/runner_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/executor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/runner_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/base_provider_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/logging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/logging_provider_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/slack_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/slack_provider_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/mlmd_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/mlmd_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/mlmd_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/mlmd_client/client_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/artifact_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/executor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/tfxtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/pandas_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/pandas_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/pandas_transform/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/pandas_transform/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/pandas_transform/null_preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/predictions_to_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/predictions_to_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/predictions_to_bigquery/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/predictions_to_bigquery/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/predictions_to_bigquery/executor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/predictions_to_bigquery/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/predictions_to_bigquery/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/sampling/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/sampling/component_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/sampling/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/sampling/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/sampling/example/sampler_pipeline_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/sampling/example/sampler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/sampling/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/sampling/executor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/sampling/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/component/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/component/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/component/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/component/executor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/example/module_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/example/taxi_example_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/test_data/module_file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/test_data/module_file/module_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/test_data/schema_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/schema_curation/test_data/schema_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons/xgboost_evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/xgboost_evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/xgboost_evaluator/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/xgboost_evaluator/xgboost_predict_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-06-07 16:07:25.000000 tfx-addons-0.7.0rc0/tfx_addons/xgboost_evaluator/xgboost_predict_extractor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 16:07:34.000000 tfx-addons-0.7.0rc0/tfx_addons.egg-info/top_level.txt
```

### Comparing `tfx-addons-0.6.0rc1/LICENSE` & `tfx-addons-0.7.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/PKG-INFO` & `tfx-addons-0.7.0rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfx-addons
-Version: 0.6.0rc1
+Version: 0.7.0rc0
 Summary: TFX Addons libraries
 Home-page: https://github.com/tensorflow/tfx-addons
 Author: The Tensorflow Authors
 Project-URL: Bug Tracker, https://github.com/tensorflow/tfx-addons/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -27,14 +27,15 @@
 Provides-Extra: xgboost_evaluator
 Provides-Extra: sampling
 Provides-Extra: message_exit_handler
 Provides-Extra: pandas_transform
 Provides-Extra: firebase_publisher
 Provides-Extra: huggingface_pusher
 Provides-Extra: model_card_generator
+Provides-Extra: predictions_to_bigquery
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: ci_min
 Provides-Extra: ci_max
 License-File: LICENSE
 
 # TFX Addons
@@ -88,14 +89,15 @@
 * [tfxa.feature_selection](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/feature_selection)
 * [tfxa.firebase_publisher](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/firebase_publisher)
 * [tfxa.huggingface_pusher](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/huggingface_pusher)
 * [tfxa.message_exit_handler](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/message_exit_handler) 
 * [tfxa.mlmd_client](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/mlmd_client) 
 * [tfxa.model_card_generator](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/model_card_generator)
 * [tfxa.pandas_transform](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/pandas_transform) 
+* [tfxa.predictions_to_bigquery](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/predictions_to_bigquery) 
 * [tfxa.sampling](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/sampling)
 * [tfxa.schema_curation](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/schema_curation) 
 * [tfxa.xgboost_evaluator](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/xgboost_evaluator)
  
 
 Check out [proposals](https://github.com/tensorflow/tfx-addons/tree/main/proposals) for a list of existing or upcoming projects proposals for TFX Addons.
```

### Comparing `tfx-addons-0.6.0rc1/README.md` & `tfx-addons-0.7.0rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 * [tfxa.feature_selection](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/feature_selection)
 * [tfxa.firebase_publisher](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/firebase_publisher)
 * [tfxa.huggingface_pusher](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/huggingface_pusher)
 * [tfxa.message_exit_handler](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/message_exit_handler) 
 * [tfxa.mlmd_client](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/mlmd_client) 
 * [tfxa.model_card_generator](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/model_card_generator)
 * [tfxa.pandas_transform](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/pandas_transform) 
+* [tfxa.predictions_to_bigquery](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/predictions_to_bigquery) 
 * [tfxa.sampling](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/sampling)
 * [tfxa.schema_curation](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/schema_curation) 
 * [tfxa.xgboost_evaluator](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/xgboost_evaluator)
  
 
 Check out [proposals](https://github.com/tensorflow/tfx-addons/tree/main/proposals) for a list of existing or upcoming projects proposals for TFX Addons.
```

### Comparing `tfx-addons-0.6.0rc1/setup.py` & `tfx-addons-0.7.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/component.py` & `tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/component.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/component_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/component_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/converters.py` & `tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/converters.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/executor.py` & `tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/executor.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feast_examplegen/executor_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/feast_examplegen/executor_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feature_selection/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feature_selection/component.py` & `tfx-addons-0.7.0rc0/tfx_addons/feature_selection/component.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feature_selection/component_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/feature_selection/component_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feature_selection/example/modules/iris_module_file.py` & `tfx-addons-0.7.0rc0/tfx_addons/feature_selection/example/modules/iris_module_file.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feature_selection/example/modules/penguins_module.py` & `tfx-addons-0.7.0rc0/tfx_addons/feature_selection/example/modules/penguins_module.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/feature_selection/example/modules/pima_indians_module_file.py` & `tfx-addons-0.7.0rc0/tfx_addons/feature_selection/example/modules/pima_indians_module_file.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/component.py` & `tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/component.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/component_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/component_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/executor.py` & `tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/executor.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/runner.py` & `tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/runner.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/firebase_publisher/runner_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/firebase_publisher/runner_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/component.py` & `tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/component.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/component_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/component_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/executor.py` & `tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/executor.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/executor_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/executor_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/runner.py` & `tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/runner.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/huggingface_pusher/runner_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/huggingface_pusher/runner_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/component.py` & `tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/component.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/component_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/component_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/constants.py` & `tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/constants.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/base_provider.py` & `tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/base_provider_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/base_provider_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/logging_provider.py` & `tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/logging_provider.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/logging_provider_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/logging_provider_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/slack_provider.py` & `tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/slack_provider.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/message_exit_handler/message_providers/slack_provider_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/message_exit_handler/message_providers/slack_provider_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/mlmd_client/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/mlmd_client/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/mlmd_client/client.py` & `tfx-addons-0.7.0rc0/tfx_addons/mlmd_client/client.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/mlmd_client/client_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/mlmd_client/client_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/artifact.py` & `tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/artifact.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/artifact_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/artifact_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/component.py` & `tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/component.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/component_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/component_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/executor.py` & `tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/executor.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/executor_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/executor_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/model_card_generator/tfxtest.py` & `tfx-addons-0.7.0rc0/tfx_addons/model_card_generator/tfxtest.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/pandas_transform/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/pandas_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/pandas_transform/component.py` & `tfx-addons-0.7.0rc0/tfx_addons/pandas_transform/component.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/pandas_transform/component_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/pandas_transform/component_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/sampling/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/sampling/component.py` & `tfx-addons-0.7.0rc0/tfx_addons/sampling/component.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/sampling/component_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/sampling/component_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/sampling/example/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/sampling/example/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/sampling/example/sampler_pipeline_local.py` & `tfx-addons-0.7.0rc0/tfx_addons/sampling/example/sampler_pipeline_local.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/sampling/example/sampler_utils.py` & `tfx-addons-0.7.0rc0/tfx_addons/sampling/example/sampler_utils.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/sampling/executor.py` & `tfx-addons-0.7.0rc0/tfx_addons/sampling/executor.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/sampling/executor_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/sampling/executor_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/sampling/spec.py` & `tfx-addons-0.7.0rc0/tfx_addons/sampling/spec.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/schema_curation/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/schema_curation/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/schema_curation/component/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/schema_curation/component/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/schema_curation/component/component.py` & `tfx-addons-0.7.0rc0/tfx_addons/schema_curation/component/component.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/schema_curation/component/component_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/schema_curation/component/component_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/schema_curation/component/executor.py` & `tfx-addons-0.7.0rc0/tfx_addons/schema_curation/component/executor.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/schema_curation/component/executor_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/schema_curation/component/executor_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/schema_curation/example/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/schema_curation/example/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/schema_curation/example/module_file.py` & `tfx-addons-0.7.0rc0/tfx_addons/schema_curation/example/module_file.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/schema_curation/example/taxi_example_local.py` & `tfx-addons-0.7.0rc0/tfx_addons/schema_curation/example/taxi_example_local.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/schema_curation/test_data/module_file/module_file.py` & `tfx-addons-0.7.0rc0/tfx_addons/schema_curation/test_data/module_file/module_file.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/schema_curation/test_data/schema_gen/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/schema_curation/test_data/schema_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/version.py` & `tfx-addons-0.7.0rc0/tfx_addons/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Define TFX Addons version information."""
 
 # We follow Semantic Versioning (https://semver.org/)
 _MAJOR_VERSION = "0"
-_MINOR_VERSION = "6"
+_MINOR_VERSION = "7"
 _PATCH_VERSION = "0"
 
 # When building releases, we can update this value on the release branch to
 # reflect the current release candidate ('rc0', 'rc1') or, finally, the official
 # stable release (indicated by `_VERSION_SUFFIX = ''`). Outside the context of a
 # release branch, the current version is by default assumed to be a
 # 'development' version, labeled 'dev'.
-_VERSION_SUFFIX = "rc1"
+_VERSION_SUFFIX = "rc0"
 
 # Example, '0.1.0-dev'
 __version__ = ".".join([_MAJOR_VERSION, _MINOR_VERSION, _PATCH_VERSION])
 if _VERSION_SUFFIX:
   __version__ = "{}-{}".format(__version__, _VERSION_SUFFIX)
 
 # Required TFX version [min, max)
@@ -75,9 +75,10 @@
     ],
     "pandas_transform": [f"tfx{_TFXVERSION_CONSTRAINT}", "pandas>=1.0.0,<2.0"],
     "firebase_publisher":
     [f"tfx{_TFXVERSION_CONSTRAINT}", "firebase-admin>=5.0.0,<6.0.0"],
     "huggingface_pusher":
     [f"tfx{_TFXVERSION_CONSTRAINT}", "huggingface-hub>=0.10.0,<1.0.0"],
     "model_card_generator":
-    [f"tfx{_TFXVERSION_CONSTRAINT}", "model-card-toolkit>=2.0.0,<3.0.0"]
+    [f"tfx{_TFXVERSION_CONSTRAINT}", "model-card-toolkit>=2.0.0,<3.0.0"],
+    "predictions_to_bigquery": [f"tfx{_TFXVERSION_CONSTRAINT}"]
 }
```

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/xgboost_evaluator/__init__.py` & `tfx-addons-0.7.0rc0/tfx_addons/xgboost_evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/xgboost_evaluator/component.py` & `tfx-addons-0.7.0rc0/tfx_addons/xgboost_evaluator/component.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/xgboost_evaluator/xgboost_predict_extractor.py` & `tfx-addons-0.7.0rc0/tfx_addons/xgboost_evaluator/xgboost_predict_extractor.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons/xgboost_evaluator/xgboost_predict_extractor_test.py` & `tfx-addons-0.7.0rc0/tfx_addons/xgboost_evaluator/xgboost_predict_extractor_test.py`

 * *Files identical despite different names*

### Comparing `tfx-addons-0.6.0rc1/tfx_addons.egg-info/PKG-INFO` & `tfx-addons-0.7.0rc0/tfx_addons.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfx-addons
-Version: 0.6.0rc1
+Version: 0.7.0rc0
 Summary: TFX Addons libraries
 Home-page: https://github.com/tensorflow/tfx-addons
 Author: The Tensorflow Authors
 Project-URL: Bug Tracker, https://github.com/tensorflow/tfx-addons/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -27,14 +27,15 @@
 Provides-Extra: xgboost_evaluator
 Provides-Extra: sampling
 Provides-Extra: message_exit_handler
 Provides-Extra: pandas_transform
 Provides-Extra: firebase_publisher
 Provides-Extra: huggingface_pusher
 Provides-Extra: model_card_generator
+Provides-Extra: predictions_to_bigquery
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: ci_min
 Provides-Extra: ci_max
 License-File: LICENSE
 
 # TFX Addons
@@ -88,14 +89,15 @@
 * [tfxa.feature_selection](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/feature_selection)
 * [tfxa.firebase_publisher](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/firebase_publisher)
 * [tfxa.huggingface_pusher](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/huggingface_pusher)
 * [tfxa.message_exit_handler](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/message_exit_handler) 
 * [tfxa.mlmd_client](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/mlmd_client) 
 * [tfxa.model_card_generator](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/model_card_generator)
 * [tfxa.pandas_transform](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/pandas_transform) 
+* [tfxa.predictions_to_bigquery](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/predictions_to_bigquery) 
 * [tfxa.sampling](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/sampling)
 * [tfxa.schema_curation](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/schema_curation) 
 * [tfxa.xgboost_evaluator](https://github.com/tensorflow/tfx-addons/tree/main/tfx_addons/xgboost_evaluator)
  
 
 Check out [proposals](https://github.com/tensorflow/tfx-addons/tree/main/proposals) for a list of existing or upcoming projects proposals for TFX Addons.
```

### Comparing `tfx-addons-0.6.0rc1/tfx_addons.egg-info/SOURCES.txt` & `tfx-addons-0.7.0rc0/tfx_addons.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,20 @@
 tfx_addons/model_card_generator/executor.py
 tfx_addons/model_card_generator/executor_test.py
 tfx_addons/model_card_generator/tfxtest.py
 tfx_addons/pandas_transform/__init__.py
 tfx_addons/pandas_transform/component.py
 tfx_addons/pandas_transform/component_test.py
 tfx_addons/pandas_transform/null_preprocessing.py
+tfx_addons/predictions_to_bigquery/__init__.py
+tfx_addons/predictions_to_bigquery/component.py
+tfx_addons/predictions_to_bigquery/executor.py
+tfx_addons/predictions_to_bigquery/executor_test.py
+tfx_addons/predictions_to_bigquery/test_component.py
+tfx_addons/predictions_to_bigquery/utils.py
 tfx_addons/sampling/__init__.py
 tfx_addons/sampling/component.py
 tfx_addons/sampling/component_test.py
 tfx_addons/sampling/executor.py
 tfx_addons/sampling/executor_test.py
 tfx_addons/sampling/spec.py
 tfx_addons/sampling/example/__init__.py
```

### Comparing `tfx-addons-0.6.0rc1/tfx_addons.egg-info/requires.txt` & `tfx-addons-0.7.0rc0/tfx_addons.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 [all]
-model-card-toolkit<3.0.0,>=2.0.0
-pandas<2.0,>=1.0.0
-feast<0.23.0,>=0.21.3
-ml_pipelines_sdk<1.11.0,>=1.6.0
-firebase-admin<6.0.0,>=5.0.0
-kfp<2.0,>=1.8
-pydantic<2.0,>=1.8.0
 ml_metadata<1.11.0,>=1.6.0
+scikit_learn<2.0.0,>=1.0.2
+firebase-admin<6.0.0,>=5.0.0
 tensorflow>=2.0.0
+kfp<2.0,>=1.8
 slackclient<3.0,>=2.9.0
-xgboost>=1.0.0
-tfx<1.11.0,>=1.6.0
+pydantic<2.0,>=1.8.0
+model-card-toolkit<3.0.0,>=2.0.0
+ml_pipelines_sdk<1.11.0,>=1.6.0
 huggingface-hub<1.0.0,>=0.10.0
-scikit_learn<2.0.0,>=1.0.2
+feast<0.23.0,>=0.21.3
+tfx<1.11.0,>=1.6.0
+xgboost>=1.0.0
+pandas<2.0,>=1.0.0
 
 [ci_max]
 tfx~=1.10.0
 tensorflow~=2.9.0
 
 [ci_min]
 tfx~=1.6.0
@@ -53,14 +53,17 @@
 tfx<1.11.0,>=1.6.0
 model-card-toolkit<3.0.0,>=2.0.0
 
 [pandas_transform]
 tfx<1.11.0,>=1.6.0
 pandas<2.0,>=1.0.0
 
+[predictions_to_bigquery]
+tfx<1.11.0,>=1.6.0
+
 [sampling]
 tfx<1.11.0,>=1.6.0
 tensorflow>=2.0.0
 
 [schema_curation]
 tfx<1.11.0,>=1.6.0
```

