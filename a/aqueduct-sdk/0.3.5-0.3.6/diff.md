# Comparing `tmp/aqueduct-sdk-0.3.5.tar.gz` & `tmp/aqueduct-sdk-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-sdk-0.3.5.tar", last modified: Wed May 31 20:26:22 2023, max compression
+gzip compressed data, was "aqueduct-sdk-0.3.6.tar", last modified: Wed Jun  7 04:46:50 2023, max compression
```

## Comparing `aqueduct-sdk-0.3.5.tar` & `aqueduct-sdk-0.3.6.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.505823 aqueduct-sdk-0.3.5/aqueduct/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1530 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.509823 aqueduct-sdk-0.3.5/aqueduct/artifacts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/base_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/bool_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/generic_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11713 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/numeric_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6593 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/preview.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/system_metric.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24892 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/artifacts/table_artifact.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.509823 aqueduct-sdk-0.3.5/aqueduct/backend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/backend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28105 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/backend/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6091 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/backend/response_helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39325 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.509823 aqueduct-sdk-0.3.5/aqueduct/constants/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/constants/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6903 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/constants/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/constants/exports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/constants/metrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    52838 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/decorator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3900 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/error.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5523 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7295 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/flow_run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8260 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/github.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.513823 aqueduct-sdk-0.3.5/aqueduct/globals/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/globals/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/globals/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/globals/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/globals/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8506 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/llm_wrapper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/logger.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.513823 aqueduct-sdk-0.3.5/aqueduct/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1976 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21114 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/dag_rules.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      554 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/execution_state.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8353 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/operators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3046 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/resource.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14933 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/response_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/models/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.517823 aqueduct-sdk-0.3.5/aqueduct/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/airflow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/aws.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/aws_lambda.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16165 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/connect_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/databricks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7470 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/dynamic_k8s.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1777 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/ecr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1691 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/gar.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4854 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/google_sheets.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      449 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/k8s.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8963 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4866 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/parameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9337 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5492 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/salesforce.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3431 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/save.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      457 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/spark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13293 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      726 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/resources/validation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3846 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/schedule.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.521824 aqueduct-sdk-0.3.5/aqueduct/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/connect_config_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/dag_delta_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/dag_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/decorator_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/decorators_with_without_parentheses_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/enum_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      909 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/flow_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/helpers_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/metric_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/naming_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15527 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/serialization_test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.521824 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.521824 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/python_function.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.521824 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/test_dependency_folder/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6065 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/tests/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/type_annotations.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/aqueduct/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10726 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/dag_deltas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.5/aqueduct/utils/describe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/format.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/function_packaging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1706 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/local_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/naming.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1416 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/resource_validation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16574 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/type_inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8059 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/aqueduct/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-31 20:26:22.000000 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3144 2023-05-31 20:26:22.000000 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-31 20:26:22.000000 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-05-31 20:26:22.000000 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-31 20:26:22.000000 aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/requirements/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/requirements/python-3-10.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/requirements/python-3-7.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/requirements/python-3-8.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/requirements/python-3-9.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-31 20:26:22.525823 aqueduct-sdk-0.3.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1197 2023-05-31 17:37:48.000000 aqueduct-sdk-0.3.5/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-31 18:17:41.000000 aqueduct-sdk-0.3.5/version
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.183963 aqueduct-sdk-0.3.6/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       34 2023-05-03 19:36:09.000000 aqueduct-sdk-0.3.6/MANIFEST.in
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7716 2023-06-07 04:46:50.183650 aqueduct-sdk-0.3.6/PKG-INFO
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.140208 aqueduct-sdk-0.3.6/aqueduct/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1530 2023-05-03 19:36:09.000000 aqueduct-sdk-0.3.6/aqueduct/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.145922 aqueduct-sdk-0.3.6/aqueduct/artifacts/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/artifacts/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1258 2023-03-20 22:51:19.000000 aqueduct-sdk-0.3.6/aqueduct/artifacts/_create.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3390 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/artifacts/base_artifact.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4230 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/artifacts/bool_artifact.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3729 2023-04-12 05:14:18.000000 aqueduct-sdk-0.3.6/aqueduct/artifacts/create.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4520 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/artifacts/generic_artifact.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    11805 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/artifacts/numeric_artifact.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6593 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/artifacts/preview.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4124 2023-04-20 19:10:16.000000 aqueduct-sdk-0.3.6/aqueduct/artifacts/system_metric.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    25037 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/artifacts/table_artifact.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.147402 aqueduct-sdk-0.3.6/aqueduct/backend/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/backend/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    28217 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/backend/api_client.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6091 2023-05-03 19:34:39.000000 aqueduct-sdk-0.3.6/aqueduct/backend/response_helpers.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    39748 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/client.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.149278 aqueduct-sdk-0.3.6/aqueduct/constants/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/constants/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6927 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/constants/enums.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       26 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/constants/exports.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      251 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/constants/metrics.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    52838 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/decorator.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3900 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/error.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5523 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/flow.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7467 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/flow_run.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     8260 2023-05-09 17:09:45.000000 aqueduct-sdk-0.3.6/aqueduct/github.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.151540 aqueduct-sdk-0.3.6/aqueduct/globals/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      200 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/globals/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      194 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/globals/api_client.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      477 2023-05-03 19:36:09.000000 aqueduct-sdk-0.3.6/aqueduct/globals/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      192 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/globals/dag.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     8506 2023-05-09 17:09:45.000000 aqueduct-sdk-0.3.6/aqueduct/llm_wrapper.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      330 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/logger.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.156106 aqueduct-sdk-0.3.6/aqueduct/models/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/models/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      699 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/models/artifact.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1976 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/models/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    21855 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/models/dag.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2925 2023-04-18 17:47:10.000000 aqueduct-sdk-0.3.6/aqueduct/models/dag_rules.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      554 2023-05-03 19:34:39.000000 aqueduct-sdk-0.3.6/aqueduct/models/execution_state.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     8353 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/models/operators.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3046 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/models/resource.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    14933 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/models/response_models.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      176 2023-04-12 05:14:23.000000 aqueduct-sdk-0.3.6/aqueduct/models/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.165102 aqueduct-sdk-0.3.6/aqueduct/resources/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      285 2023-05-03 19:36:09.000000 aqueduct-sdk-0.3.6/aqueduct/resources/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      465 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/airflow.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      609 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/aws.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      455 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/aws_lambda.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    16165 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/connect_config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      477 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/databricks.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7470 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/dynamic_k8s.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1777 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/ecr.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1691 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/gar.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4854 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/google_sheets.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      449 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/k8s.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     8963 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/mongodb.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4866 2023-05-24 17:09:38.000000 aqueduct-sdk-0.3.6/aqueduct/resources/parameters.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     9337 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5492 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/salesforce.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3431 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/save.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      457 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/spark.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    13293 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/sql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      726 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/resources/validation.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3846 2023-05-03 19:36:09.000000 aqueduct-sdk-0.3.6/aqueduct/schedule.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.171715 aqueduct-sdk-0.3.6/aqueduct/tests/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/tests/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      445 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/tests/connect_config_test.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    19133 2023-03-20 22:51:19.000000 aqueduct-sdk-0.3.6/aqueduct/tests/dag_delta_test.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4058 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/tests/dag_test.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3040 2023-04-20 19:10:16.000000 aqueduct-sdk-0.3.6/aqueduct/tests/decorator_test.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3811 2023-04-20 19:10:16.000000 aqueduct-sdk-0.3.6/aqueduct/tests/decorators_with_without_parentheses_test.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      218 2023-02-24 18:10:20.000000 aqueduct-sdk-0.3.6/aqueduct/tests/enum_test.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      909 2023-05-24 17:09:38.000000 aqueduct-sdk-0.3.6/aqueduct/tests/flow_test.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1398 2023-05-03 19:36:09.000000 aqueduct-sdk-0.3.6/aqueduct/tests/helpers_test.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4498 2023-04-20 19:10:16.000000 aqueduct-sdk-0.3.6/aqueduct/tests/metric_test.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      488 2023-03-20 22:51:19.000000 aqueduct-sdk-0.3.6/aqueduct/tests/naming_test.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    15563 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/aqueduct/tests/serialization_test.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.172109 aqueduct-sdk-0.3.6/aqueduct/tests/test_files/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/tests/test_files/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.172578 aqueduct-sdk-0.3.6/aqueduct/tests/test_files/python_function/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/tests/test_files/python_function/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      170 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/tests/test_files/python_function/python_function.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.173411 aqueduct-sdk-0.3.6/aqueduct/tests/test_files/python_function/test_dependency_folder/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       74 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6065 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/tests/utils.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      225 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/type_annotations.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.179780 aqueduct-sdk-0.3.6/aqueduct/utils/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/utils/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    10726 2023-05-23 00:44:06.000000 aqueduct-sdk-0.3.6/aqueduct/utils/dag_deltas.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1271 2023-01-27 20:50:40.000000 aqueduct-sdk-0.3.6/aqueduct/utils/describe.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       26 2023-02-22 00:09:19.000000 aqueduct-sdk-0.3.6/aqueduct/utils/format.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    11492 2023-04-20 19:10:16.000000 aqueduct-sdk-0.3.6/aqueduct/utils/function_packaging.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1706 2023-04-12 05:14:23.000000 aqueduct-sdk-0.3.6/aqueduct/utils/local_data.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1234 2023-03-20 22:51:19.000000 aqueduct-sdk-0.3.6/aqueduct/utils/naming.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1416 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/utils/resource_validation.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    16574 2023-05-23 00:44:06.000000 aqueduct-sdk-0.3.6/aqueduct/utils/serialization.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2148 2023-04-20 19:10:16.000000 aqueduct-sdk-0.3.6/aqueduct/utils/type_inference.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     8059 2023-06-06 20:20:00.000000 aqueduct-sdk-0.3.6/aqueduct/utils/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.181458 aqueduct-sdk-0.3.6/aqueduct_sdk.egg-info/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7716 2023-06-07 04:46:50.000000 aqueduct-sdk-0.3.6/aqueduct_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3144 2023-06-07 04:46:50.000000 aqueduct-sdk-0.3.6/aqueduct_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        1 2023-06-07 04:46:50.000000 aqueduct-sdk-0.3.6/aqueduct_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      326 2023-06-07 04:46:50.000000 aqueduct-sdk-0.3.6/aqueduct_sdk.egg-info/requires.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        9 2023-06-07 04:46:50.000000 aqueduct-sdk-0.3.6/aqueduct_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:46:50.182980 aqueduct-sdk-0.3.6/requirements/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      325 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/requirements/python-3-10.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      325 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/requirements/python-3-7.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      325 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/requirements/python-3-8.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      325 2023-06-06 20:20:06.000000 aqueduct-sdk-0.3.6/requirements/python-3-9.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       38 2023-06-07 04:46:50.184069 aqueduct-sdk-0.3.6/setup.cfg
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1197 2023-05-03 19:36:09.000000 aqueduct-sdk-0.3.6/setup.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        6 2023-06-06 20:21:12.000000 aqueduct-sdk-0.3.6/version
```

### Comparing `aqueduct-sdk-0.3.5/PKG-INFO` & `aqueduct-sdk-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/__init__.py` & `aqueduct-sdk-0.3.6/aqueduct/__init__.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/artifacts/_create.py` & `aqueduct-sdk-0.3.6/aqueduct/artifacts/_create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/artifacts/bool_artifact.py` & `aqueduct-sdk-0.3.6/aqueduct/artifacts/bool_artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import numpy as np
 from aqueduct.artifacts import preview as artifact_utils
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.constants.enums import OperatorType
 from aqueduct.error import ArtifactNeverComputedException
 from aqueduct.models.dag import DAG
+from aqueduct.models.execution_state import ExecutionState
 from aqueduct.models.operators import get_operator_type
 from aqueduct.utils.describe import get_readable_description_for_check
 from aqueduct.utils.utils import format_header_for_print
 
 
 class BoolArtifact(BaseArtifact):
     """This class represents a bool within the flow's DAG.
@@ -39,34 +40,33 @@
 
     def __init__(
         self,
         dag: DAG,
         artifact_id: uuid.UUID,
         content: Optional[Union[bool, np.bool_]] = None,
         from_flow_run: bool = False,
+        execution_state: Optional[ExecutionState] = None,
     ):
-        self._dag = dag
-        self._artifact_id = artifact_id
+        super().__init__(dag, artifact_id, content, from_flow_run, execution_state)
 
-        # This parameter indicates whether the artifact is fetched from flow-run or not.
-        self._from_flow_run = from_flow_run
-        self._set_content(content)
-
-    def get(self, parameters: Optional[Dict[str, Any]] = None) -> Union[bool, np.bool_]:
+    def get(self, parameters: Optional[Dict[str, Any]] = None) -> Optional[Union[bool, np.bool_]]:
         """Materializes a BoolArtifact into a boolean.
 
         Returns:
             A boolean representing whether the check passed or not.
 
         Raises:
             InvalidRequestError:
                 An error occurred because of an issue with the user's code or inputs.
             InternalServerError:
                 An unexpected error occurred in the server.
         """
+        if self._is_content_deleted():
+            return None
+
         self._dag.must_get_artifact(self._artifact_id)
 
         if self._from_flow_run:
             if self._get_content() is None:
                 raise ArtifactNeverComputedException(
                     "This artifact was part of an existing flow run but was never computed successfully!",
                 )
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/artifacts/create.py` & `aqueduct-sdk-0.3.6/aqueduct/artifacts/create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/artifacts/generic_artifact.py` & `aqueduct-sdk-0.3.6/aqueduct/artifacts/generic_artifact.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from aqueduct.artifacts import numeric_artifact
 from aqueduct.artifacts import preview as artifact_utils
 from aqueduct.artifacts import system_metric
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.constants.enums import ArtifactType, ExecutionStatus
 from aqueduct.error import ArtifactNeverComputedException
 from aqueduct.models.dag import DAG
+from aqueduct.models.execution_state import ExecutionState
 from aqueduct.utils.utils import format_header_for_print
 
 from aqueduct import globals
 
 
 class GenericArtifact(BaseArtifact, system_metric.SystemMetricMixin):
     """This class represents a generic artifact within the flow's DAG.
@@ -26,47 +27,45 @@
     def __init__(
         self,
         dag: DAG,
         artifact_id: uuid.UUID,
         artifact_type: ArtifactType = ArtifactType.UNTYPED,
         content: Optional[Any] = None,
         from_flow_run: bool = False,
-        execution_status: Optional[ExecutionStatus] = None,
+        execution_state: Optional[ExecutionState] = None,
     ):
         # Cannot initialize a generic artifact's content without also setting its type.
         if content is not None:
             assert artifact_type != ArtifactType.UNTYPED
 
-        self._dag = dag
-        self._artifact_id = artifact_id
-
-        # This parameter indicates whether the artifact is fetched from flow-run or not.
-        self._from_flow_run = from_flow_run
-        self._set_content(content)
-        # This is only relevant to generic artifact produced from flow_run.artifact().
-        # We need this to distinguish between when an artifact's content is None versus
-        # when it fails to compute successfully.
-        self._execution_status = execution_status
+        super().__init__(dag, artifact_id, content, from_flow_run, execution_state)
 
     def get(self, parameters: Optional[Dict[str, Any]] = None) -> Any:
         """Materializes the artifact.
 
         Returns:
             The materialized value.
 
         Raises:
             InvalidRequestError:
                 An error occurred because of an issue with the user's code or inputs.
             InternalServerError:
                 An unexpected error occurred in the server.
         """
+        if self._is_content_deleted():
+            return None
+
         self._dag.must_get_artifact(self._artifact_id)
 
         if self._from_flow_run:
-            if self._execution_status != ExecutionStatus.SUCCEEDED:
+            if (
+                not self._execution_state
+                or self._execution_state.status != ExecutionStatus.SUCCEEDED
+            ):
+                # DELETED case is already covered.
                 raise ArtifactNeverComputedException(
                     "This artifact was part of an existing flow run but was never computed successfully!",
                 )
             elif parameters is not None:
                 raise NotImplementedError(
                     "Parameterizing historical artifacts is not currently supported."
                 )
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/artifacts/numeric_artifact.py` & `aqueduct-sdk-0.3.6/aqueduct/artifacts/numeric_artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     FunctionGranularity,
     FunctionType,
     OperatorType,
 )
 from aqueduct.error import AqueductError, ArtifactNeverComputedException
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG
+from aqueduct.models.execution_state import ExecutionState
 from aqueduct.models.operators import (
     CheckSpec,
     FunctionSpec,
     Operator,
     OperatorSpec,
     get_operator_type,
 )
@@ -64,38 +65,37 @@
 
     def __init__(
         self,
         dag: DAG,
         artifact_id: uuid.UUID,
         content: Optional[Number] = None,
         from_flow_run: bool = False,
+        execution_state: Optional[ExecutionState] = None,
     ):
-        self._dag = dag
-        self._artifact_id = artifact_id
+        super().__init__(dag, artifact_id, content, from_flow_run, execution_state)
 
-        # This parameter indicates whether the artifact is fetched from flow-run or not.
-        self._from_flow_run = from_flow_run
-        self._set_content(content)
-
-    def get(self, parameters: Optional[Dict[str, Any]] = None) -> Number:
+    def get(self, parameters: Optional[Dict[str, Any]] = None) -> Optional[Number]:
         """Materializes a NumericArtifact into its immediate float value.
 
         Returns:
             The evaluated metric as a number.
 
         Raises:
             InvalidRequestError:
                 An error occurred because of an issue with the user's code or inputs.
             InternalServerError:
                 An unexpected error occurred within the Aqueduct cluster.
         """
         self._dag.must_get_artifact(self._artifact_id)
+        if self._is_content_deleted():
+            return None
 
         if self._from_flow_run:
             if self._get_content() is None:
+                # DELETED case is already covered.
                 raise ArtifactNeverComputedException(
                     "This artifact was part of an existing flow run but was never computed successfully!",
                 )
             elif parameters is not None:
                 raise NotImplementedError(
                     "Parameterizing historical artifacts is not currently supported."
                 )
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/artifacts/preview.py` & `aqueduct-sdk-0.3.6/aqueduct/artifacts/preview.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/artifacts/system_metric.py` & `aqueduct-sdk-0.3.6/aqueduct/artifacts/system_metric.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/artifacts/table_artifact.py` & `aqueduct-sdk-0.3.6/aqueduct/artifacts/table_artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     ExecutionMode,
     FunctionGranularity,
     FunctionType,
     OperatorType,
 )
 from aqueduct.error import AqueductError, ArtifactNeverComputedException
 from aqueduct.models.dag import DAG
+from aqueduct.models.execution_state import ExecutionState
 from aqueduct.models.operators import CheckSpec, FunctionSpec, MetricSpec, OperatorSpec
 from aqueduct.utils.dag_deltas import RemoveCheckOperatorDelta, apply_deltas_to_dag
 from aqueduct.utils.describe import (
     get_readable_description_for_check,
     get_readable_description_for_metric,
 )
 from aqueduct.utils.function_packaging import serialize_function
@@ -58,23 +59,19 @@
 
     def __init__(
         self,
         dag: DAG,
         artifact_id: uuid.UUID,
         content: Optional[pd.DataFrame] = None,
         from_flow_run: bool = False,
+        execution_state: Optional[ExecutionState] = None,
     ):
-        self._dag = dag
-        self._artifact_id = artifact_id
+        super().__init__(dag, artifact_id, content, from_flow_run, execution_state)
 
-        # This parameter indicates whether the artifact is fetched from flow-run or not.
-        self._from_flow_run = from_flow_run
-        self._set_content(content)
-
-    def get(self, parameters: Optional[Dict[str, Any]] = None) -> pd.DataFrame:
+    def get(self, parameters: Optional[Dict[str, Any]] = None) -> Optional[pd.DataFrame]:
         """Materializes TableArtifact into an actual dataframe.
 
         Args:
             parameters:
                 A map from parameter name to its custom value, to be used when evaluating
                 this artifact.
 
@@ -84,17 +81,20 @@
         Raises:
             InvalidRequestError:
                 An error occurred because of an issue with the user's code or inputs.
             InternalServerError:
                 An unexpected error occurred within the Aqueduct cluster.
         """
         self._dag.must_get_artifact(self._artifact_id)
+        if self._is_content_deleted():
+            return None
 
         if self._from_flow_run:
             if self._get_content() is None:
+                # DELETED case is already covered.
                 raise ArtifactNeverComputedException(
                     "This artifact was part of an existing flow run but was never computed successfully!",
                 )
             elif parameters is not None:
                 raise NotImplementedError(
                     "Parameterizing historical artifacts is not currently supported."
                 )
@@ -109,30 +109,33 @@
             # If the artifact was previously generated lazily, materialize the contents.
             if parameters is None and self._get_content() is None:
                 self._set_content(content)
 
         assert isinstance(content, pd.DataFrame)
         return content
 
-    def head(self, n: int = 5, parameters: Optional[Dict[str, Any]] = None) -> pd.DataFrame:
+    def head(
+        self, n: int = 5, parameters: Optional[Dict[str, Any]] = None
+    ) -> Optional[pd.DataFrame]:
         """Returns a preview of the table artifact.
 
         >>> db = client.resource(name="demo/")
         >>> customer_data = db.sql("SELECT * from customers")
         >>> churn_predictions = predict_churn(customer_data)
         >>> churn_predictions.head()
 
         Args:
             n:
                 the number of row previewed. Default to 5.
         Returns:
             A dataframe containing the table contents of this artifact.
         """
         df = self.get(parameters=parameters)
-        return df.head(n)
+
+        return df.head(n) if df is not None else None
 
     PRESET_METRIC_LIST = ["number_of_missing_values", "number_of_rows", "max", "min", "mean", "std"]
 
     def list_preset_metrics(self) -> List[str]:
         """Returns a list of all preset metrics available on the table artifact.
         These preset metrics can be set via the invoking the preset method on a artifact.
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/backend/api_client.py` & `aqueduct-sdk-0.3.6/aqueduct/backend/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     NoConnectedResourcesException,
     ResourceNotFoundError,
     UnprocessableEntityError,
 )
 from aqueduct.logger import logger
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG, Metadata
+from aqueduct.models.execution_state import ExecutionState
 from aqueduct.models.operators import Operator, ParamSpec
 from aqueduct.models.resource import BaseResource, ResourceInfo
 from aqueduct.models.response_models import (
     DeleteWorkflowResponse,
     DynamicEngineStatusResponse,
     GetDagResponse,
     GetDagResultResponse,
@@ -39,14 +40,15 @@
     RegisterAirflowWorkflowResponse,
     RegisterWorkflowResponse,
     SavedObjectUpdate,
     WorkflowDagResponse,
     WorkflowDagResultResponse,
 )
 from aqueduct.utils.serialization import deserialize
+from dateutil import parser as datetime_parser
 from pkg_resources import get_distribution, parse_version
 
 from ..resources.connect_config import DynamicK8sConfig, ResourceConfig
 from .response_helpers import (
     _construct_preview_response,
     _handle_preview_resp,
     _parse_artifact_result_response,
@@ -606,20 +608,15 @@
         results_resp = requests.get(url, headers=headers)
         self.raise_errors(results_resp)
         dag_results = [GetDagResultResponse(**dag_result) for dag_result in results_resp.json()]
         workflow_dag_results = [
             WorkflowDagResultResponse(
                 id=dag_result.id,
                 created_at=int(
-                    datetime.datetime.strptime(
-                        resp_dags[str(dag_result.dag_id)].created_at[:-4],
-                        "%Y-%m-%dT%H:%M:%S.%f"
-                        if resp_dags[str(dag_result.dag_id)].created_at[-1] == "Z"
-                        else "%Y-%m-%dT%H:%M:%S.%f%z",
-                    ).timestamp()
+                    datetime_parser.parse(resp_dags[str(dag_result.dag_id)].created_at).timestamp()
                 ),
                 status=dag_result.exec_state.status,
                 exec_state=dag_result.exec_state,
                 workflow_dag_id=dag_result.dag_id,
             )
             for dag_result in dag_results
         ]
@@ -646,37 +643,45 @@
         response = requests.get(url, headers=headers)
         self.raise_errors(response)
 
         return [ListWorkflowResponseEntry(**workflow) for workflow in response.json()]
 
     def get_artifact_result_data(
         self, dag_result_id: str, artifact_id: str
-    ) -> Tuple[Optional[Any], ExecutionStatus]:
-        """Returns an empty string if the operator was not successfully executed."""
+    ) -> Tuple[Optional[Any], Optional[ExecutionState]]:
+        """
+        Returns the artifact's result and execution state if available.
+        Prints non-blocking warning if the value if either is not available.
+        """
         headers = self._generate_auth_headers()
         url = self.construct_full_url(
             self.GET_ARTIFACT_RESULT_TEMPLATE % (dag_result_id, artifact_id)
         )
         resp = requests.get(url, headers=headers)
         self.raise_errors(resp)
 
         parsed_response = _parse_artifact_result_response(resp)
-        execution_status = parsed_response["metadata"]["exec_state"]["status"]
+        execution_state = None
+        if "exec_state" in parsed_response["metadata"]:
+            execution_state = ExecutionState(**parsed_response["metadata"]["exec_state"])
 
         serialization_type = parsed_response["metadata"]["serialization_type"]
         artifact_type = parsed_response["metadata"]["artifact_type"]
 
         return_value = None
         if "data" in parsed_response:
             return_value = deserialize(serialization_type, artifact_type, parsed_response["data"])
 
-        if execution_status != ExecutionStatus.SUCCEEDED:
-            logger().warning("Artifact result unavailable due to unsuccessful execution.")
+        if not execution_state:
+            logger().warning("Artifact execution state is unavailable.")
+
+        if return_value is None:
+            logger().warning("Artifact result is unavailable.")
 
-        return (return_value, execution_status)
+        return (return_value, execution_state)
 
     def get_image_url(
         self,
         resource_id: str,
         service: ServiceType,
         image_name: str,
     ) -> GetImageURLResponse:
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/backend/response_helpers.py` & `aqueduct-sdk-0.3.6/aqueduct/backend/response_helpers.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/client.py` & `aqueduct-sdk-0.3.6/aqueduct/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -549,14 +549,15 @@
         artifacts: Optional[Union[BaseArtifact, List[BaseArtifact]]] = None,
         metrics: Optional[List[NumericArtifact]] = None,
         checks: Optional[List[BoolArtifact]] = None,
         k_latest_runs: Optional[int] = None,
         source_flow: Optional[Union[Flow, str, uuid.UUID]] = None,
         run_now: Optional[bool] = None,
         use_local: Optional[bool] = False,
+        disable_snapshots: Optional[bool] = False,
     ) -> Flow:
         """Uploads and kicks off the given flow in the system.
 
         If a flow already exists with the same name, the existing flow will be updated
         to this new state.
 
         The default execution engine of the flow is Aqueduct. In order to specify which
@@ -598,14 +599,18 @@
                 Used to identify the source flow for this flow. This can be identified
                 via an object (Flow), name (str), or id (str or uuid).
             run_now:
                 Used to specify if the flow should run immediately at publish time. The default
                 behavior is 'True'.
             use_local:
                 Must be set if any artifact in the flow is derived from local data.
+            disable_snapshots:
+                If set to 'True', this option disables snapshots for all artifacts
+                that are not generated from parameters, metrics, or checks.
+                It achieves this by calling the `.disable_snapshot()` method on each of these artifacts.
 
         Raises:
             InvalidUserArgumentException:
                 An invalid combination of parameters was provided.
             InvalidCronStringException:
                 An error occurred because the supplied schedule is invalid.
             IncompleteFlowException:
@@ -730,14 +735,17 @@
                 globals.__GLOBAL_CONFIG__.engine,
             ),
             publish_flow_engine_config=generate_engine_config(self._connected_resources, engine),
         )
 
         dag.validate_and_resolve_artifact_names()
 
+        if disable_snapshots:
+            dag.disable_op_output_snapshots()
+
         if dag.engine_config.type == RuntimeType.AIRFLOW:
             if run_now is not None:
                 raise InvalidUserArgumentException(
                     "run_now parameter is not supported for Airflow engine."
                 )
             # This is an Airflow workflow
             resp = globals.__GLOBAL_API_CLIENT__.register_airflow_workflow(dag)
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/constants/enums.py` & `aqueduct-sdk-0.3.6/aqueduct/constants/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     UNKNOWN = "unknown"
     SUCCEEDED = "succeeded"
     RUNNING = "running"
     FAILED = "failed"
     PENDING = "pending"
     REGISTERED = "registered"
     CANCELED = "canceled"
+    DELETED = "deleted"
 
 
 class NotificationLogLevel(str, Enum, metaclass=MetaEnum):
     SUCCESS = "success"
     WARNING = "warning"
     ERROR = "error"
     INFO = "info"
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/decorator.py` & `aqueduct-sdk-0.3.6/aqueduct/decorator.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/error.py` & `aqueduct-sdk-0.3.6/aqueduct/error.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/flow.py` & `aqueduct-sdk-0.3.6/aqueduct/flow.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/flow_run.py` & `aqueduct-sdk-0.3.6/aqueduct/flow_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,20 +94,20 @@
 
         param_operators = self._dag.list_operators(filter_to=[OperatorType.PARAM])
         if len(param_operators) > 0:
             print(format_header_for_print("Parameters"))
             for param_op in param_operators:
                 (
                     param_content,
-                    execution_status,
+                    execution_state,
                 ) = globals.__GLOBAL_API_CLIENT__.get_artifact_result_data(
                     self._id, str(param_op.outputs[0])
                 )
 
-                if execution_status != ExecutionStatus.SUCCEEDED:
+                if not execution_state or execution_state.status != ExecutionStatus.SUCCEEDED:
                     param_content = "Parameter not successfully initialized."
 
                 print("* " + param_op.name + ": " + str(param_content))
 
         if self.status() == ExecutionStatus.FAILED:
             print(format_header_for_print("Failures"))
 
@@ -162,44 +162,47 @@
         """
         flow_run_dag = self._dag
         artifact_from_dag = flow_run_dag.get_artifact_by_name(name)
 
         if artifact_from_dag is None:
             return None
 
-        content, execution_status = globals.__GLOBAL_API_CLIENT__.get_artifact_result_data(
+        content, execution_state = globals.__GLOBAL_API_CLIENT__.get_artifact_result_data(
             self._id, str(artifact_from_dag.id)
         )
 
         if not isinstance(artifact_from_dag.type, ArtifactType):
             raise InternalAqueductError("The artifact's type can not be recognized.")
 
         if artifact_from_dag.type is ArtifactType.TABLE:
             return table_artifact.TableArtifact(
                 self._dag,
                 artifact_from_dag.id,
                 content=content,
                 from_flow_run=True,
+                execution_state=execution_state,
             )
         elif artifact_from_dag.type is ArtifactType.NUMERIC:
             return numeric_artifact.NumericArtifact(
                 self._dag,
                 artifact_from_dag.id,
                 content=content,
                 from_flow_run=True,
+                execution_state=execution_state,
             )
         elif artifact_from_dag.type is ArtifactType.BOOL:
             return bool_artifact.BoolArtifact(
                 self._dag,
                 artifact_from_dag.id,
                 content=content,
                 from_flow_run=True,
+                execution_state=execution_state,
             )
         else:
             return generic_artifact.GenericArtifact(
                 self._dag,
                 artifact_from_dag.id,
                 artifact_from_dag.type,
                 content=content,
                 from_flow_run=True,
-                execution_status=execution_status,
+                execution_state=execution_state,
             )
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/github.py` & `aqueduct-sdk-0.3.6/aqueduct/github.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/llm_wrapper.py` & `aqueduct-sdk-0.3.6/aqueduct/llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/models/artifact.py` & `aqueduct-sdk-0.3.6/aqueduct/models/artifact.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,10 +10,13 @@
     id: uuid.UUID
     name: str
     type: ArtifactType
     # Whether this artifact was given a name explicitly by the user.
     # If true, this artifact name is expected to be unique in the DAG.
     explicitly_named: bool = False
     from_local_data: bool = False
+    # Whether the content of this artifact will be persisted
+    # after workflow execution.
+    should_persist: bool = True
 
     class Config:
         fields = {"explicitly_named": {"exclude": ...}, "from_local_data": {"exclude": ...}}
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/models/config.py` & `aqueduct-sdk-0.3.6/aqueduct/models/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/models/dag.py` & `aqueduct-sdk-0.3.6/aqueduct/models/dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,14 +453,30 @@
         """Updates an artifact to have a user-specified name. This means the artifact is
         now explicitly named.
         """
         artifact = self.must_get_artifact(artifact_id)
         artifact.name = new_name
         artifact.explicitly_named = True
 
+    def update_artifact_should_persist(self, artifact_id: uuid.UUID, should_persist: bool) -> None:
+        self.must_get_artifact(artifact_id).should_persist = should_persist
+
+    def disable_op_output_snapshots(self) -> None:
+        # Disable snapshots that may contain sensitive user data.
+        # For now, this means snapshots not from param, check, and metrics.
+        for op in self.list_operators():
+            if get_operator_type(op) not in [
+                OperatorType.CHECK,
+                OperatorType.METRIC,
+                OperatorType.SYSTEM_METRIC,
+                OperatorType.PARAM,
+            ]:
+                for artf_id in op.outputs:
+                    self.update_artifact_should_persist(artf_id, False)
+
     def update_param_spec(self, name: str, new_spec: OperatorSpec) -> None:
         """Checks that:
         1) The parameter already exists, and there is not more than one with the same name.
         2) The spec is a parameter spec.
 
         The new parameter's value must also be of the same type, but we enforce during execution.
         """
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/models/dag_rules.py` & `aqueduct-sdk-0.3.6/aqueduct/models/dag_rules.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/models/execution_state.py` & `aqueduct-sdk-0.3.6/aqueduct/models/execution_state.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/models/operators.py` & `aqueduct-sdk-0.3.6/aqueduct/models/operators.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/models/resource.py` & `aqueduct-sdk-0.3.6/aqueduct/models/resource.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/models/response_models.py` & `aqueduct-sdk-0.3.6/aqueduct/models/response_models.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/aws.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/aws.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/connect_config.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/connect_config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/dynamic_k8s.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/dynamic_k8s.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/ecr.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/ecr.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/gar.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/gar.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/google_sheets.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/google_sheets.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/mongodb.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/mongodb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/parameters.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/parameters.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/s3.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/salesforce.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/salesforce.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/save.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/save.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/sql.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/sql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/resources/validation.py` & `aqueduct-sdk-0.3.6/aqueduct/resources/validation.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/schedule.py` & `aqueduct-sdk-0.3.6/aqueduct/schedule.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/tests/dag_delta_test.py` & `aqueduct-sdk-0.3.6/aqueduct/tests/dag_delta_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/tests/dag_test.py` & `aqueduct-sdk-0.3.6/aqueduct/tests/dag_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/tests/decorator_test.py` & `aqueduct-sdk-0.3.6/aqueduct/tests/decorator_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/tests/decorators_with_without_parentheses_test.py` & `aqueduct-sdk-0.3.6/aqueduct/tests/decorators_with_without_parentheses_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/tests/flow_test.py` & `aqueduct-sdk-0.3.6/aqueduct/tests/flow_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/tests/helpers_test.py` & `aqueduct-sdk-0.3.6/aqueduct/tests/helpers_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/tests/metric_test.py` & `aqueduct-sdk-0.3.6/aqueduct/tests/metric_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/tests/serialization_test.py` & `aqueduct-sdk-0.3.6/aqueduct/tests/serialization_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     )
 
     assert extract_artifact.json() == json.dumps(
         {
             "id": str(artifact_id),
             "name": artifact_name,
             "type": ArtifactType.TABLE,
+            "should_persist": True,
         }
     )
 
 
 def test_operator_serialization():
     op_id = uuid.uuid4()
     other_ids = [uuid.uuid4(), uuid.uuid4()]
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct/tests/utils.py` & `aqueduct-sdk-0.3.6/aqueduct/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/utils/dag_deltas.py` & `aqueduct-sdk-0.3.6/aqueduct/utils/dag_deltas.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/utils/describe.py` & `aqueduct-sdk-0.3.6/aqueduct/utils/describe.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/utils/function_packaging.py` & `aqueduct-sdk-0.3.6/aqueduct/utils/function_packaging.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/utils/local_data.py` & `aqueduct-sdk-0.3.6/aqueduct/utils/local_data.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/utils/naming.py` & `aqueduct-sdk-0.3.6/aqueduct/utils/naming.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/utils/resource_validation.py` & `aqueduct-sdk-0.3.6/aqueduct/utils/resource_validation.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/utils/serialization.py` & `aqueduct-sdk-0.3.6/aqueduct/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/utils/type_inference.py` & `aqueduct-sdk-0.3.6/aqueduct/utils/type_inference.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct/utils/utils.py` & `aqueduct-sdk-0.3.6/aqueduct/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/PKG-INFO` & `aqueduct-sdk-0.3.6/aqueduct_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-sdk-0.3.5/aqueduct_sdk.egg-info/SOURCES.txt` & `aqueduct-sdk-0.3.6/aqueduct_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.5/setup.py` & `aqueduct-sdk-0.3.6/setup.py`

 * *Files identical despite different names*

