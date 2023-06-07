# Comparing `tmp/giskard-2.0.0b3.tar.gz` & `tmp/giskard-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard-2.0.0b3.tar", last modified: Wed Jun  7 01:12:26 2023, max compression
+gzip compressed data, was "giskard-2.0.0b4.tar", last modified: Wed Jun  7 11:44:00 2023, max compression
```

## Comparing `giskard-2.0.0b3.tar` & `giskard-2.0.0b4.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.103851 giskard-2.0.0b3/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9939 2023-06-07 01:12:26.104009 giskard-2.0.0b3/PKG-INFO
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8623 2023-06-06 23:34:22.000000 giskard-2.0.0b3/README.md
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.065689 giskard-2.0.0b3/giskard/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1779 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/cli.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/cli_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.067443 giskard-2.0.0b3/giskard/client/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/client/dtos.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/client/giskard_client.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/client/io_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/client/project.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b3/giskard/client/python_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.067851 giskard-2.0.0b3/giskard/commands/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15306 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/commands/cli_server.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7042 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/commands/cli_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.069308 giskard-2.0.0b3/giskard/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11799 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/core.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/dataset_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/errors.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13215 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/model_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/suite.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/validation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.069530 giskard-2.0.0b3/giskard/datasets/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.069722 giskard-2.0.0b3/giskard/datasets/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26419 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.070967 giskard-2.0.0b3/giskard/datasets/metadata/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/metadata/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/metadata/indexing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/metadata/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/metadata/text_metadata_provider.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.071396 giskard-2.0.0b3/giskard/demo/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2931 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/demo/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/demo/titanic.csv
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.071781 giskard-2.0.0b3/giskard/ml_worker/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.072619 giskard-2.0.0b3/giskard/ml_worker/bridge/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/bridge/data_encryptor.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/bridge/error.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/bridge/ml_worker_bridge.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/bridge/service_messages.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.072913 giskard-2.0.0b3/giskard/ml_worker/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/core/log_listener.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5858 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/core/savable.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.073403 giskard-2.0.0b3/giskard/ml_worker/exceptions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/exceptions/IllegalArgumentError.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/exceptions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/exceptions/giskard_exception.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.073740 giskard-2.0.0b3/giskard/ml_worker/generated/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard/ml_worker/generated/ml_worker_pb2.py
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/ml_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.073965 giskard-2.0.0b3/giskard/ml_worker/server/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/server/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26425 2023-06-06 23:20:30.000000 giskard-2.0.0b3/giskard/ml_worker/server/ml_worker_service.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.074966 giskard-2.0.0b3/giskard/ml_worker/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b3/giskard/ml_worker/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.075500 giskard-2.0.0b3/giskard/ml_worker/testing/functions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/functions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3927 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/functions/slicing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6602 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/functions/transformation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.076596 giskard-2.0.0b3/giskard/ml_worker/testing/registry/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/decorators_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/giskard_test.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/slicing_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/transformation_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/udf_repository.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/stat_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/test_result.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/ml_worker/testing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.077513 giskard-2.0.0b3/giskard/ml_worker/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/utils/file_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/utils/logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1952 2023-06-06 23:20:13.000000 giskard-2.0.0b3/giskard/ml_worker/utils/network.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/utils/request_interceptor.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.078153 giskard-2.0.0b3/giskard/models/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/_precooked.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.078300 giskard-2.0.0b3/giskard/models/automodel/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9181 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/automodel/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.078562 giskard-2.0.0b3/giskard/models/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34228 2023-06-06 23:20:04.000000 giskard-2.0.0b3/giskard/models/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.079220 giskard-2.0.0b3/giskard/models/cache/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/cache/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/cache/cache.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.079379 giskard-2.0.0b3/giskard/models/catboost/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/catboost/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.079529 giskard-2.0.0b3/giskard/models/function/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/function/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.079670 giskard-2.0.0b3/giskard/models/huggingface/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/huggingface/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.079892 giskard-2.0.0b3/giskard/models/langchain/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2619 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/langchain/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6342 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/model_explanation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.080100 giskard-2.0.0b3/giskard/models/pytorch/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/pytorch/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.080241 giskard-2.0.0b3/giskard/models/sklearn/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/sklearn/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.080425 giskard-2.0.0b3/giskard/models/tensorflow/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1656 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/tensorflow/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/path_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.082073 giskard-2.0.0b3/giskard/scanner/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.082613 giskard-2.0.0b3/giskard/scanner/calibration/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/calibration/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/calibration/overconfidence_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/calibration/underconfidence_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.082973 giskard-2.0.0b3/giskard/scanner/common/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/common/examples.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/common/loss_based_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.083136 giskard-2.0.0b3/giskard/scanner/data_leakage/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/data_leakage/data_leakage_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/issues.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.083434 giskard-2.0.0b3/giskard/scanner/llm/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/llm/toxicity_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/llm/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/logger.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.084030 giskard-2.0.0b3/giskard/scanner/performance/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/performance/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/performance/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/performance/metrics.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/performance/performance_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/result.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.087237 giskard-2.0.0b3/giskard/scanner/robustness/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/base_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/entity_swap.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      953 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/ethical_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/nationalities.json
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1006 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/text_perturbation_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/text_transformations.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/scanner.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.087470 giskard-2.0.0b3/giskard/scanner/stochasticity/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/stochasticity/stochasticity_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.089440 giskard-2.0.0b3/giskard/scanner/templates/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      785 2023-06-06 23:34:22.000000 giskard-2.0.0b3/giskard/scanner/templates/_code_snippet.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.092000 giskard-2.0.0b3/giskard/scanner/templates/_issues/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/data_leakage.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/default.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/llm_toxicity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/overconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/performance.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/robustness.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/stochasticity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/underconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues_table.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_main_content.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_tab_header.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      187 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/base.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/scan_results.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.093225 giskard-2.0.0b3/giskard/scanner/templates/static/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/static/external.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/static/internal.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/static/style.css
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.093537 giskard-2.0.0b3/giskard/scanner/visualization/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/visualization/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/visualization/custom_jinja.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/settings.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.096141 giskard-2.0.0b3/giskard/slicing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/base.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/bruteforce_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/category_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/multiscale_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/opt_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/slice.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/stop_words.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/text_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/tree_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.096463 giskard-2.0.0b3/giskard/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.099022 giskard-2.0.0b3/giskard/testing/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/testing/tests/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33167 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/testing/tests/drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30208 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/testing/tests/metamorphic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25823 2023-06-06 21:06:58.000000 giskard-2.0.0b3/giskard/testing/tests/performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10497 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/testing/tests/statistic.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.099810 giskard-2.0.0b3/giskard/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6206 2023-06-07 01:11:58.000000 giskard-2.0.0b3/giskard/utils/analytics_collector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/utils/display.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/utils/environment_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.066669 giskard-2.0.0b3/giskard.egg-info/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9939 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/PKG-INFO
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/SOURCES.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/dependency_links.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/entry_points.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/requires.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        8 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/top_level.txt
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7375 2023-06-06 23:34:22.000000 giskard-2.0.0b3/pyproject.toml
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-07 01:12:26.104443 giskard-2.0.0b3/setup.cfg
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-06 19:53:55.000000 giskard-2.0.0b3/setup.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.103629 giskard-2.0.0b3/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1513 2023-06-06 20:59:14.000000 giskard-2.0.0b3/tests/test_custom_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_data_drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_data_processing_pipeline.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_dataset.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b3/tests/test_logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_metamorphic_direction.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_metamorphic_invariance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2409 2023-06-06 21:05:44.000000 giskard-2.0.0b3/tests/test_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_model_auto_inference.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_model_explanation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_model_postprocess.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_programmatic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_project_uploads.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_statistical.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_upload.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.314212 giskard-2.0.0b4/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9939 2023-06-07 11:44:00.314327 giskard-2.0.0b4/PKG-INFO
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8623 2023-06-07 11:37:58.000000 giskard-2.0.0b4/README.md
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.282557 giskard-2.0.0b4/giskard/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1779 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/cli.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/cli_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.284270 giskard-2.0.0b4/giskard/client/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/client/dtos.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/client/giskard_client.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/client/io_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/client/project.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b4/giskard/client/python_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.284823 giskard-2.0.0b4/giskard/commands/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15306 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/commands/cli_server.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7206 2023-06-07 11:36:36.000000 giskard-2.0.0b4/giskard/commands/cli_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.286234 giskard-2.0.0b4/giskard/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/core/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11799 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/core/core.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/core/dataset_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/core/errors.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13215 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/core/model_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/core/suite.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/core/validation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.286393 giskard-2.0.0b4/giskard/datasets/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.286533 giskard-2.0.0b4/giskard/datasets/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26419 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.287270 giskard-2.0.0b4/giskard/datasets/metadata/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/metadata/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/metadata/indexing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/metadata/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/metadata/text_metadata_provider.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.287570 giskard-2.0.0b4/giskard/demo/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2931 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/demo/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/demo/titanic.csv
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.287957 giskard-2.0.0b4/giskard/ml_worker/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.288795 giskard-2.0.0b4/giskard/ml_worker/bridge/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/bridge/data_encryptor.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/bridge/error.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/bridge/ml_worker_bridge.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/bridge/service_messages.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.289261 giskard-2.0.0b4/giskard/ml_worker/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/core/log_listener.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5858 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/core/savable.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.289756 giskard-2.0.0b4/giskard/ml_worker/exceptions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/exceptions/IllegalArgumentError.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/exceptions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/exceptions/giskard_exception.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.290178 giskard-2.0.0b4/giskard/ml_worker/generated/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard/ml_worker/generated/ml_worker_pb2.py
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/ml_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.290465 giskard-2.0.0b4/giskard/ml_worker/server/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/server/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26425 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/server/ml_worker_service.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.291218 giskard-2.0.0b4/giskard/ml_worker/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b4/giskard/ml_worker/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.291691 giskard-2.0.0b4/giskard/ml_worker/testing/functions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/functions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3927 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/testing/functions/slicing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6602 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/testing/functions/transformation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.293043 giskard-2.0.0b4/giskard/ml_worker/testing/registry/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/decorators_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/giskard_test.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/slicing_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/transformation_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/udf_repository.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/stat_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/test_result.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/testing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.294000 giskard-2.0.0b4/giskard/ml_worker/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/utils/file_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/utils/logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1952 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/utils/network.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/utils/request_interceptor.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.294793 giskard-2.0.0b4/giskard/models/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/_precooked.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.294967 giskard-2.0.0b4/giskard/models/automodel/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9181 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/automodel/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.295129 giskard-2.0.0b4/giskard/models/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34228 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.295814 giskard-2.0.0b4/giskard/models/cache/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/cache/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/cache/cache.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.295970 giskard-2.0.0b4/giskard/models/catboost/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/catboost/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.296159 giskard-2.0.0b4/giskard/models/function/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/function/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.296330 giskard-2.0.0b4/giskard/models/huggingface/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/huggingface/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.296486 giskard-2.0.0b4/giskard/models/langchain/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2619 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/langchain/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6342 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/model_explanation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.296667 giskard-2.0.0b4/giskard/models/pytorch/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/pytorch/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.296854 giskard-2.0.0b4/giskard/models/sklearn/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/sklearn/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.297012 giskard-2.0.0b4/giskard/models/tensorflow/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1656 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/tensorflow/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/path_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.298492 giskard-2.0.0b4/giskard/scanner/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.299185 giskard-2.0.0b4/giskard/scanner/calibration/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/calibration/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/calibration/overconfidence_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/calibration/underconfidence_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.299575 giskard-2.0.0b4/giskard/scanner/common/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/common/examples.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/common/loss_based_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.299773 giskard-2.0.0b4/giskard/scanner/data_leakage/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/data_leakage/data_leakage_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/issues.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.300115 giskard-2.0.0b4/giskard/scanner/llm/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/llm/toxicity_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/llm/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/logger.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.300786 giskard-2.0.0b4/giskard/scanner/performance/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/performance/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/performance/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/performance/metrics.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/performance/performance_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/result.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.302843 giskard-2.0.0b4/giskard/scanner/robustness/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/robustness/base_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/robustness/entity_swap.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      953 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/robustness/ethical_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/robustness/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/robustness/nationalities.json
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1006 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/robustness/text_perturbation_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/robustness/text_transformations.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/scanner.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.303115 giskard-2.0.0b4/giskard/scanner/stochasticity/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/stochasticity/stochasticity_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.304145 giskard-2.0.0b4/giskard/scanner/templates/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      785 2023-06-07 11:37:38.000000 giskard-2.0.0b4/giskard/scanner/templates/_code_snippet.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.305367 giskard-2.0.0b4/giskard/scanner/templates/_issues/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/data_leakage.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/default.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/llm_toxicity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/overconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/performance.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/robustness.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/stochasticity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/underconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues_table.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_main_content.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_tab_header.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      187 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/base.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/templates/scan_results.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.306121 giskard-2.0.0b4/giskard/scanner/templates/static/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/static/external.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/static/internal.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/static/style.css
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.306384 giskard-2.0.0b4/giskard/scanner/visualization/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/visualization/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/visualization/custom_jinja.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/settings.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.308207 giskard-2.0.0b4/giskard/slicing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/base.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/bruteforce_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/category_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/multiscale_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/opt_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/slice.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/stop_words.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/text_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/tree_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.308393 giskard-2.0.0b4/giskard/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.309943 giskard-2.0.0b4/giskard/testing/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/testing/tests/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33167 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/testing/tests/drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30208 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/testing/tests/metamorphic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25823 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/testing/tests/performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10370 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/testing/tests/statistic.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.310747 giskard-2.0.0b4/giskard/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5534 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/utils/analytics_collector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/utils/display.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/utils/environment_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.283454 giskard-2.0.0b4/giskard.egg-info/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9939 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/PKG-INFO
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/SOURCES.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/dependency_links.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/entry_points.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/requires.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        8 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/top_level.txt
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7375 2023-06-07 11:37:59.000000 giskard-2.0.0b4/pyproject.toml
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-07 11:44:00.314630 giskard-2.0.0b4/setup.cfg
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-06 19:53:55.000000 giskard-2.0.0b4/setup.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.314027 giskard-2.0.0b4/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1513 2023-06-07 11:12:34.000000 giskard-2.0.0b4/tests/test_custom_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_data_drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_data_processing_pipeline.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_dataset.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b4/tests/test_logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_metamorphic_direction.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_metamorphic_invariance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2409 2023-06-07 11:12:34.000000 giskard-2.0.0b4/tests/test_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_model_auto_inference.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_model_explanation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_model_postprocess.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-07 11:12:34.000000 giskard-2.0.0b4/tests/test_performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-07 11:43:22.000000 giskard-2.0.0b4/tests/test_programmatic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_project_uploads.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_statistical.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_upload.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_utils.py
```

### Comparing `giskard-2.0.0b3/PKG-INFO` & `giskard-2.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
@@ -114,15 +114,15 @@
 
 ## Getting started
 
 <div id="installation">
 
 ### Installation
 ```sh
-pip install "giskard[server]==2.0.0b3"
+pip install "giskard[server]==2.0.0b4"
 
 giskard server start
 ```
 
 That's it. Access at http://localhost:19000
 </div>
 <div id="scan-your-model-to-detect-vulnerabilities">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b3 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b4 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
@@ -59,15 +59,15 @@
                                 [Scan Example]
 And of course, Giskard works with any model, any environment and integrates
 seamlessly with your favorite tools â¤µï¸
                  [https://github.com/Giskard-AI/giskard/blob/
       9f9f9994ab5deb503ed9c64e672982432a493cca/readme/tools.png?raw=true]
 
 ## Getting started
-### Installation ```sh pip install "giskard[server]==2.0.0b3" giskard server
+### Installation ```sh pip install "giskard[server]==2.0.0b4" giskard server
 start ``` That's it. Access at http://localhost:19000
 ### Scan your model to detect vulnerabilities After having wrapped your [model]
 (https://docs.giskard.ai/en/latest/guides/wrap_model/index.html) & [dataset]
 (https://docs.giskard.ai/en/latest/guides/wrap_dataset/index.html), you can
 scan your model for vulnerabilities using: ```python import giskard model, df =
 giskard.demo.titanic() model = giskard.Model(model=model,
 model_type="classification") dataset = giskard.Dataset( df=df,
```

### Comparing `giskard-2.0.0b3/README.md` & `giskard-2.0.0b4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 ## Getting started
 
 <div id="installation">
 
 ### Installation
 ```sh
-pip install "giskard[server]==2.0.0b3"
+pip install "giskard[server]==2.0.0b4"
 
 giskard server start
 ```
 
 That's it. Access at http://localhost:19000
 </div>
 <div id="scan-your-model-to-detect-vulnerabilities">
```

#### html2text {}

```diff
@@ -41,15 +41,15 @@
                                 [Scan Example]
 And of course, Giskard works with any model, any environment and integrates
 seamlessly with your favorite tools â¤µï¸
                  [https://github.com/Giskard-AI/giskard/blob/
       9f9f9994ab5deb503ed9c64e672982432a493cca/readme/tools.png?raw=true]
 
 ## Getting started
-### Installation ```sh pip install "giskard[server]==2.0.0b3" giskard server
+### Installation ```sh pip install "giskard[server]==2.0.0b4" giskard server
 start ``` That's it. Access at http://localhost:19000
 ### Scan your model to detect vulnerabilities After having wrapped your [model]
 (https://docs.giskard.ai/en/latest/guides/wrap_model/index.html) & [dataset]
 (https://docs.giskard.ai/en/latest/guides/wrap_dataset/index.html), you can
 scan your model for vulnerabilities using: ```python import giskard model, df =
 giskard.demo.titanic() model = giskard.Model(model=model,
 model_type="classification") dataset = giskard.Dataset( df=df,
```

### Comparing `giskard-2.0.0b3/giskard/__init__.py` & `giskard-2.0.0b4/giskard/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/cli.py` & `giskard-2.0.0b4/giskard/cli.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/cli_utils.py` & `giskard-2.0.0b4/giskard/cli_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/client/giskard_client.py` & `giskard-2.0.0b4/giskard/client/giskard_client.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/client/io_utils.py` & `giskard-2.0.0b4/giskard/client/io_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/client/project.py` & `giskard-2.0.0b4/giskard/client/project.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/client/python_utils.py` & `giskard-2.0.0b4/giskard/client/python_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/commands/cli_server.py` & `giskard-2.0.0b4/giskard/commands/cli_server.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/commands/cli_worker.py` & `giskard-2.0.0b4/giskard/commands/cli_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,15 +142,18 @@
         if ml_worker:
             asyncio.get_event_loop().run_until_complete(ml_worker.stop())
     except lockfile.AlreadyLocked:
         existing_pid = read_pid_from_pidfile(pid_file_path)
         logger.warning(
             f"Another ML Worker {_ml_worker_description(is_server, url)} "
             f"is already running with PID: {existing_pid}. "
-            f"Not starting a new one."
+            "Not starting a new one. "
+            "To stop a running worker for this instance execute: \"giskard worker stop\" or "
+            "\"giskard worker stop -a\" to stop all running workers"
+
         )
     finally:
         if pid_file.i_am_locking():
             pid_file.release()
 
 
 def _ml_worker_description(is_server, url):
```

### Comparing `giskard-2.0.0b3/giskard/core/core.py` & `giskard-2.0.0b4/giskard/core/core.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/core/dataset_validation.py` & `giskard-2.0.0b4/giskard/core/dataset_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/core/errors.py` & `giskard-2.0.0b4/giskard/core/errors.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/core/model_validation.py` & `giskard-2.0.0b4/giskard/core/model_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/core/suite.py` & `giskard-2.0.0b4/giskard/core/suite.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/core/validation.py` & `giskard-2.0.0b4/giskard/core/validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/datasets/__init__.py` & `giskard-2.0.0b4/giskard/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/datasets/base/__init__.py` & `giskard-2.0.0b4/giskard/datasets/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/datasets/metadata/indexing.py` & `giskard-2.0.0b4/giskard/datasets/metadata/indexing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/datasets/metadata/registry.py` & `giskard-2.0.0b4/giskard/datasets/metadata/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/datasets/metadata/text_metadata_provider.py` & `giskard-2.0.0b4/giskard/datasets/metadata/text_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/demo/__init__.py` & `giskard-2.0.0b4/giskard/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/demo/titanic.csv` & `giskard-2.0.0b4/giskard/demo/titanic.csv`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/bridge/data_encryptor.py` & `giskard-2.0.0b4/giskard/ml_worker/bridge/data_encryptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/bridge/ml_worker_bridge.py` & `giskard-2.0.0b4/giskard/ml_worker/bridge/ml_worker_bridge.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/core/log_listener.py` & `giskard-2.0.0b4/giskard/ml_worker/core/log_listener.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/core/savable.py` & `giskard-2.0.0b4/giskard/ml_worker/core/savable.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/generated/ml_worker_pb2.py` & `giskard-2.0.0b4/giskard/ml_worker/generated/ml_worker_pb2.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/generated/ml_worker_pb2_grpc.py` & `giskard-2.0.0b4/giskard/ml_worker/generated/ml_worker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/ml_worker.py` & `giskard-2.0.0b4/giskard/ml_worker/ml_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/server/ml_worker_service.py` & `giskard-2.0.0b4/giskard/ml_worker/server/ml_worker_service.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/functions/slicing.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/functions/slicing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/functions/transformation.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/functions/transformation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/registry/decorators.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/registry/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/registry/decorators_utils.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/registry/decorators_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/registry/giskard_test.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/registry/giskard_test.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/registry/registry.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/registry/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/registry/slicing_function.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/registry/slicing_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/registry/transformation_function.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/registry/transformation_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/registry/udf_repository.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/registry/udf_repository.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/stat_utils.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/stat_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/test_result.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/test_result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/testing/utils.py` & `giskard-2.0.0b4/giskard/ml_worker/testing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/utils/logging.py` & `giskard-2.0.0b4/giskard/ml_worker/utils/logging.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/utils/network.py` & `giskard-2.0.0b4/giskard/ml_worker/utils/network.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/ml_worker/utils/request_interceptor.py` & `giskard-2.0.0b4/giskard/ml_worker/utils/request_interceptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/__init__.py` & `giskard-2.0.0b4/giskard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/_precooked.py` & `giskard-2.0.0b4/giskard/models/_precooked.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/automodel/__init__.py` & `giskard-2.0.0b4/giskard/models/automodel/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/base/__init__.py` & `giskard-2.0.0b4/giskard/models/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/cache/__init__.py` & `giskard-2.0.0b4/giskard/models/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/cache/cache.py` & `giskard-2.0.0b4/giskard/models/cache/cache.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/catboost/__init__.py` & `giskard-2.0.0b4/giskard/models/catboost/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/function/__init__.py` & `giskard-2.0.0b4/giskard/models/function/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/huggingface/__init__.py` & `giskard-2.0.0b4/giskard/models/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/langchain/__init__.py` & `giskard-2.0.0b4/giskard/models/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/model_explanation.py` & `giskard-2.0.0b4/giskard/models/model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/pytorch/__init__.py` & `giskard-2.0.0b4/giskard/models/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/sklearn/__init__.py` & `giskard-2.0.0b4/giskard/models/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/tensorflow/__init__.py` & `giskard-2.0.0b4/giskard/models/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/models/utils.py` & `giskard-2.0.0b4/giskard/models/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/path_utils.py` & `giskard-2.0.0b4/giskard/path_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/__init__.py` & `giskard-2.0.0b4/giskard/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/calibration/issues.py` & `giskard-2.0.0b4/giskard/scanner/calibration/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/calibration/overconfidence_detector.py` & `giskard-2.0.0b4/giskard/scanner/calibration/overconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/calibration/underconfidence_detector.py` & `giskard-2.0.0b4/giskard/scanner/calibration/underconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/common/examples.py` & `giskard-2.0.0b4/giskard/scanner/common/examples.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/common/loss_based_detector.py` & `giskard-2.0.0b4/giskard/scanner/common/loss_based_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/data_leakage/data_leakage_detector.py` & `giskard-2.0.0b4/giskard/scanner/data_leakage/data_leakage_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/decorators.py` & `giskard-2.0.0b4/giskard/scanner/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/issues.py` & `giskard-2.0.0b4/giskard/scanner/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/llm/toxicity_detector.py` & `giskard-2.0.0b4/giskard/scanner/llm/toxicity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/llm/utils.py` & `giskard-2.0.0b4/giskard/scanner/llm/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/performance/issues.py` & `giskard-2.0.0b4/giskard/scanner/performance/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/performance/metrics.py` & `giskard-2.0.0b4/giskard/scanner/performance/metrics.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/performance/performance_bias_detector.py` & `giskard-2.0.0b4/giskard/scanner/performance/performance_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/registry.py` & `giskard-2.0.0b4/giskard/scanner/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/result.py` & `giskard-2.0.0b4/giskard/scanner/result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/robustness/base_detector.py` & `giskard-2.0.0b4/giskard/scanner/robustness/base_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/robustness/entity_swap.py` & `giskard-2.0.0b4/giskard/scanner/robustness/entity_swap.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/robustness/ethical_bias_detector.py` & `giskard-2.0.0b4/giskard/scanner/robustness/ethical_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/robustness/issues.py` & `giskard-2.0.0b4/giskard/scanner/robustness/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/robustness/nationalities.json` & `giskard-2.0.0b4/giskard/scanner/robustness/nationalities.json`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/robustness/text_perturbation_detector.py` & `giskard-2.0.0b4/giskard/scanner/robustness/text_perturbation_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/robustness/text_transformations.py` & `giskard-2.0.0b4/giskard/scanner/robustness/text_transformations.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/scanner.py` & `giskard-2.0.0b4/giskard/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/stochasticity/stochasticity_detector.py` & `giskard-2.0.0b4/giskard/scanner/stochasticity/stochasticity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_code_snippet.html` & `giskard-2.0.0b4/giskard/scanner/templates/_code_snippet.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
     <div class="text-sm">
         <pre><code class="language-python rounded">{% raw %}from giskard import GiskardClient
 test_suite = results.generate_test_suite("My first test suite")
 
 # To start the Giskard server, run in your terminal within the Python
 # environment containing the dependencies of your model: 
-giskard server start --version 2.0.0b3
+giskard server start --version 2.0.0b4
 giskard worker start -u http://localhost:19000/
 
 # Then upload your test suite to the opened Giskard server
 client = GiskardClient("http://localhost:19000", "GISKARD_API_KEY")
 client.create_project("my_project_id", "my_project_name")
 test_suite.upload(client, "my_project_id"){% endraw %}
 </code></pre>
```

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_issues/data_leakage.html` & `giskard-2.0.0b4/giskard/scanner/templates/_issues/data_leakage.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_issues/default.html` & `giskard-2.0.0b4/giskard/scanner/templates/_issues/default.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_issues/llm_toxicity.html` & `giskard-2.0.0b4/giskard/scanner/templates/_issues/llm_toxicity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_issues/overconfidence.html` & `giskard-2.0.0b4/giskard/scanner/templates/_issues/overconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_issues/performance.html` & `giskard-2.0.0b4/giskard/scanner/templates/_issues/performance.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_issues/robustness.html` & `giskard-2.0.0b4/giskard/scanner/templates/_issues/robustness.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_issues/stochasticity.html` & `giskard-2.0.0b4/giskard/scanner/templates/_issues/stochasticity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_issues/underconfidence.html` & `giskard-2.0.0b4/giskard/scanner/templates/_issues/underconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_issues_table.html` & `giskard-2.0.0b4/giskard/scanner/templates/_issues_table.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_main_content.html` & `giskard-2.0.0b4/giskard/scanner/templates/_main_content.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/_tab_header.html` & `giskard-2.0.0b4/giskard/scanner/templates/_tab_header.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/scan_results.html` & `giskard-2.0.0b4/giskard/scanner/templates/scan_results.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/static/external.js` & `giskard-2.0.0b4/giskard/scanner/templates/static/external.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/static/internal.js` & `giskard-2.0.0b4/giskard/scanner/templates/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/templates/static/style.css` & `giskard-2.0.0b4/giskard/scanner/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/scanner/visualization/custom_jinja.py` & `giskard-2.0.0b4/giskard/scanner/visualization/custom_jinja.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/settings.py` & `giskard-2.0.0b4/giskard/settings.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/slicing/base.py` & `giskard-2.0.0b4/giskard/slicing/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/slicing/bruteforce_slicer.py` & `giskard-2.0.0b4/giskard/slicing/bruteforce_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/slicing/category_slicer.py` & `giskard-2.0.0b4/giskard/slicing/category_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/slicing/multiscale_slicer.py` & `giskard-2.0.0b4/giskard/slicing/multiscale_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/slicing/opt_slicer.py` & `giskard-2.0.0b4/giskard/slicing/opt_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/slicing/slice.py` & `giskard-2.0.0b4/giskard/slicing/slice.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/slicing/stop_words.py` & `giskard-2.0.0b4/giskard/slicing/stop_words.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/slicing/text_slicer.py` & `giskard-2.0.0b4/giskard/slicing/text_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/slicing/tree_slicer.py` & `giskard-2.0.0b4/giskard/slicing/tree_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/slicing/utils.py` & `giskard-2.0.0b4/giskard/slicing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/testing/__init__.py` & `giskard-2.0.0b4/giskard/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/testing/tests/drift.py` & `giskard-2.0.0b4/giskard/testing/tests/drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/testing/tests/metamorphic.py` & `giskard-2.0.0b4/giskard/testing/tests/metamorphic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/testing/tests/performance.py` & `giskard-2.0.0b4/giskard/testing/tests/performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard/testing/tests/statistic.py` & `giskard-2.0.0b4/giskard/testing/tests/statistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Statistical tests"""
 import numbers
 import numpy as np
-import pandas as pd
 from typing import Optional
 
 from giskard import test
 from giskard.datasets.base import Dataset
 from giskard.ml_worker.testing.test_result import TestResult, TestMessage, TestMessageLevel
 from giskard.ml_worker.testing.utils import validate_classification_label
 from giskard.ml_worker.testing.registry.slicing_function import SlicingFunction
@@ -110,30 +109,26 @@
         passed:
             TRUE if metric > threshold
     """
     if slicing_function:
         dataset = dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=dataset, dataset_name="dataset", test_name="test_output_in_range")
 
-    results_df = pd.DataFrame()
-
     prediction_results = model.predict(dataset)
 
     if model.is_regression:
-        results_df["output"] = prediction_results.raw_prediction
+        output = prediction_results.raw_prediction
 
     elif model.is_classification:
-        results_df["output"] = prediction_results.all_predictions[classification_label]
+        output = prediction_results.all_predictions[classification_label]
 
     else:
         raise ValueError(f"Prediction task is not supported: {model.meta.model_type}")
 
-    passed_idx = dataset.df.loc[
-        (results_df["output"] <= max_range) & (results_df["output"] >= min_range)
-        ].index.values
+    passed_idx = dataset.df.loc[(output <= max_range) & (output >= min_range)].index.values
 
     passed_ratio = len(passed_idx) / len(dataset)
 
     return TestResult(
         actual_slices_size=[len(dataset)],
         metric=passed_ratio,
         passed=bool(passed_ratio >= threshold),
```

### Comparing `giskard-2.0.0b3/giskard/utils/analytics_collector.py` & `giskard-2.0.0b4/giskard/utils/analytics_collector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import hashlib
 import os
 import platform
-import time
 import uuid
-from dataclasses import dataclass
 from functools import wraps
-from queue import Queue
 from threading import Lock
-from typing import Dict, Optional, Any
+from typing import Dict, Optional
 
 import requests
 from mixpanel import Mixpanel
 
 from giskard.settings import settings
 from giskard.utils import fullname, threaded
 from giskard.utils.environment_detector import EnvironmentDetector
@@ -75,57 +72,33 @@
         "dataset_rows": dataset.df.shape[0],
         "dataset_cols": dataset.df.shape[1],
         "dataset_column_types": column_types,
         "dataset_column_dtypes": column_dtypes,
     }
 
 
-@dataclass
-class TelemetryMessage:
-    distinct_id: Any
-    event_name: Any
-    properties: Any
-    meta: Any
-
-
 class GiskardAnalyticsCollector:
     lock = Lock()
     ip: Optional[str]
     dev_mp_project_key = "4cca5fabca54f6df41ea500e33076c99"
     prod_mp_project_key = "2c3efacc6c26ffb991a782b476b8c620"
     server_info: Optional[Dict] = None
     mp: Mixpanel
     giskard_version: Optional[str]
     environment: str
-    queue: Queue[TelemetryMessage] = Queue()
 
     def __init__(self) -> None:
         self.is_enabled = not settings.disable_analytics
         self.giskard_version = None
         self.ip = None
         self.environment = EnvironmentDetector().detect()
         if self.is_enabled:
             self.mp = self.configure_mixpanel()
             self.distinct_user_id = GiskardAnalyticsCollector.machine_based_user_id()
 
-    @threaded
-    def _consume(self):
-        while True:
-            event = self.queue.get(block=True)
-            self.mp.track(
-                distinct_id=self.distinct_user_id,
-                event_name=event.event_name,
-                properties=dict(event.merged_props),
-                meta=event.meta
-            )
-            time.sleep(1)
-
-    def _submit(self, msg):
-        self.queue.put(msg, block=True)
-
     @staticmethod
     @analytics_method
     def configure_mixpanel() -> Mixpanel:
         is_dev_mode = os.environ.get("GISKARD_DEV_MODE", "n").lower() in ["yes", "true", "1"]
 
         return Mixpanel(
             GiskardAnalyticsCollector.dev_mp_project_key
@@ -162,17 +135,17 @@
                 "environment": self.environment
             }
             if properties is not None:
                 merged_props = {**merged_props, **properties}
             if self.server_info is not None:
                 merged_props = {**merged_props, **self.server_info}
 
-            self._submit(TelemetryMessage(
+            self.mp.track(
                 distinct_id=self.distinct_user_id, event_name=event_name, properties=dict(merged_props), meta=meta
-            ))
+            )
 
     @staticmethod
     def machine_based_user_id():
         try:
             return anonymize(str(uuid.getnode()) + os.getlogin())
         except BaseException:  # noqa NOSONAR
             # https://bugs.python.org/issue40821
```

### Comparing `giskard-2.0.0b3/giskard/utils/environment_detector.py` & `giskard-2.0.0b4/giskard/utils/environment_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard.egg-info/PKG-INFO` & `giskard-2.0.0b4/giskard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
@@ -114,15 +114,15 @@
 
 ## Getting started
 
 <div id="installation">
 
 ### Installation
 ```sh
-pip install "giskard[server]==2.0.0b3"
+pip install "giskard[server]==2.0.0b4"
 
 giskard server start
 ```
 
 That's it. Access at http://localhost:19000
 </div>
 <div id="scan-your-model-to-detect-vulnerabilities">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b3 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b4 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
@@ -59,15 +59,15 @@
                                 [Scan Example]
 And of course, Giskard works with any model, any environment and integrates
 seamlessly with your favorite tools â¤µï¸
                  [https://github.com/Giskard-AI/giskard/blob/
       9f9f9994ab5deb503ed9c64e672982432a493cca/readme/tools.png?raw=true]
 
 ## Getting started
-### Installation ```sh pip install "giskard[server]==2.0.0b3" giskard server
+### Installation ```sh pip install "giskard[server]==2.0.0b4" giskard server
 start ``` That's it. Access at http://localhost:19000
 ### Scan your model to detect vulnerabilities After having wrapped your [model]
 (https://docs.giskard.ai/en/latest/guides/wrap_model/index.html) & [dataset]
 (https://docs.giskard.ai/en/latest/guides/wrap_dataset/index.html), you can
 scan your model for vulnerabilities using: ```python import giskard model, df =
 giskard.demo.titanic() model = giskard.Model(model=model,
 model_type="classification") dataset = giskard.Dataset( df=df,
```

### Comparing `giskard-2.0.0b3/giskard.egg-info/SOURCES.txt` & `giskard-2.0.0b4/giskard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/giskard.egg-info/requires.txt` & `giskard-2.0.0b4/giskard.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/pyproject.toml` & `giskard-2.0.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 "Twitter" = "https://twitter.com/giskard_ai"
 
 
 [project]
 name = "giskard"
 readme = "README.md"
 license = { text = "Apache Software License 2.0" }
-version = "2.0.0b3"
+version = "2.0.0b4"
 description = "The testing framework dedicated to ML models, from tabular to LLMs"
 authors = [
     { name = "Giskard AI", email = "hello@giskard.ai" },
 ]
 keywords = [
     "Artificial Intelligence",
     "Machine Learning",
```

### Comparing `giskard-2.0.0b3/setup.py` & `giskard-2.0.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_custom_model.py` & `giskard-2.0.0b4/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_data_drift.py` & `giskard-2.0.0b4/tests/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_data_processing_pipeline.py` & `giskard-2.0.0b4/tests/test_data_processing_pipeline.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_dataset.py` & `giskard-2.0.0b4/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_metamorphic_direction.py` & `giskard-2.0.0b4/tests/test_metamorphic_direction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_metamorphic_invariance.py` & `giskard-2.0.0b4/tests/test_metamorphic_invariance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_model.py` & `giskard-2.0.0b4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_model_auto_inference.py` & `giskard-2.0.0b4/tests/test_model_auto_inference.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_model_explanation.py` & `giskard-2.0.0b4/tests/test_model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_model_postprocess.py` & `giskard-2.0.0b4/tests/test_model_postprocess.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_performance.py` & `giskard-2.0.0b4/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_programmatic.py` & `giskard-2.0.0b4/tests/test_programmatic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_project_uploads.py` & `giskard-2.0.0b4/tests/test_project_uploads.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_statistical.py` & `giskard-2.0.0b4/tests/test_statistical.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b3/tests/test_upload.py` & `giskard-2.0.0b4/tests/test_upload.py`

 * *Files identical despite different names*

