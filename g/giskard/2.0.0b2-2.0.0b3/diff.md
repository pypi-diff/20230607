# Comparing `tmp/giskard-2.0.0b2.tar.gz` & `tmp/giskard-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard-2.0.0b2.tar", last modified: Tue Jun  6 14:17:49 2023, max compression
+gzip compressed data, was "giskard-2.0.0b3.tar", last modified: Wed Jun  7 01:12:26 2023, max compression
```

## Comparing `giskard-2.0.0b2.tar` & `giskard-2.0.0b3.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.165540 giskard-2.0.0b2/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13101 2023-06-06 14:17:49.165695 giskard-2.0.0b2/PKG-INFO
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12124 2023-04-12 00:50:05.000000 giskard-2.0.0b2/README.md
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.104140 giskard-2.0.0b2/giskard/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1779 2023-06-06 14:00:09.000000 giskard-2.0.0b2/giskard/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-05 15:02:01.000000 giskard-2.0.0b2/giskard/cli.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/cli_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.106323 giskard-2.0.0b2/giskard/client/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/client/dtos.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/client/giskard_client.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/client/io_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/client/project.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b2/giskard/client/python_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.106931 giskard-2.0.0b2/giskard/commands/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15303 2023-06-06 12:13:24.000000 giskard-2.0.0b2/giskard/commands/cli_server.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7042 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/commands/cli_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.108433 giskard-2.0.0b2/giskard/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/core/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11799 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/core/core.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/core/dataset_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-05 15:02:01.000000 giskard-2.0.0b2/giskard/core/errors.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13215 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/core/model_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-05 15:04:55.000000 giskard-2.0.0b2/giskard/core/suite.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/core/validation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.108584 giskard-2.0.0b2/giskard/datasets/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/datasets/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.108765 giskard-2.0.0b2/giskard/datasets/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26419 2023-06-05 15:04:55.000000 giskard-2.0.0b2/giskard/datasets/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.109840 giskard-2.0.0b2/giskard/datasets/metadata/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/datasets/metadata/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/datasets/metadata/indexing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/datasets/metadata/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/datasets/metadata/text_metadata_provider.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.110153 giskard-2.0.0b2/giskard/demo/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2931 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/demo/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/demo/titanic.csv
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.110534 giskard-2.0.0b2/giskard/ml_worker/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b2/giskard/ml_worker/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.111291 giskard-2.0.0b2/giskard/ml_worker/bridge/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/bridge/data_encryptor.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b2/giskard/ml_worker/bridge/error.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-05 15:02:01.000000 giskard-2.0.0b2/giskard/ml_worker/bridge/ml_worker_bridge.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/bridge/service_messages.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.111627 giskard-2.0.0b2/giskard/ml_worker/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/core/log_listener.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5858 2023-06-05 15:58:41.000000 giskard-2.0.0b2/giskard/ml_worker/core/savable.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.112175 giskard-2.0.0b2/giskard/ml_worker/exceptions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b2/giskard/ml_worker/exceptions/IllegalArgumentError.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b2/giskard/ml_worker/exceptions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b2/giskard/ml_worker/exceptions/giskard_exception.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.112591 giskard-2.0.0b2/giskard/ml_worker/generated/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-06 14:17:49.000000 giskard-2.0.0b2/giskard/ml_worker/generated/ml_worker_pb2.py
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-06 14:17:49.000000 giskard-2.0.0b2/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/ml_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.112997 giskard-2.0.0b2/giskard/ml_worker/server/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b2/giskard/ml_worker/server/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26370 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/ml_worker/server/ml_worker_service.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.113915 giskard-2.0.0b2/giskard/ml_worker/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b2/giskard/ml_worker/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.114601 giskard-2.0.0b2/giskard/ml_worker/testing/functions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/testing/functions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3927 2023-06-06 08:42:11.000000 giskard-2.0.0b2/giskard/ml_worker/testing/functions/slicing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6602 2023-06-06 08:42:11.000000 giskard-2.0.0b2/giskard/ml_worker/testing/functions/transformation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.116464 giskard-2.0.0b2/giskard/ml_worker/testing/registry/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/testing/registry/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/testing/registry/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/testing/registry/decorators_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-05 15:02:01.000000 giskard-2.0.0b2/giskard/ml_worker/testing/registry/giskard_test.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-05 15:02:01.000000 giskard-2.0.0b2/giskard/ml_worker/testing/registry/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-05 15:04:55.000000 giskard-2.0.0b2/giskard/ml_worker/testing/registry/slicing_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-05 15:04:55.000000 giskard-2.0.0b2/giskard/ml_worker/testing/registry/transformation_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/testing/registry/udf_repository.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/testing/stat_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/testing/test_result.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1598 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/testing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.117455 giskard-2.0.0b2/giskard/ml_worker/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b2/giskard/ml_worker/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/utils/file_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-05 15:02:01.000000 giskard-2.0.0b2/giskard/ml_worker/utils/logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1948 2023-06-06 14:01:11.000000 giskard-2.0.0b2/giskard/ml_worker/utils/network.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/ml_worker/utils/request_interceptor.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.118385 giskard-2.0.0b2/giskard/models/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/models/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/models/_precooked.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.118544 giskard-2.0.0b2/giskard/models/automodel/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9127 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/models/automodel/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.118802 giskard-2.0.0b2/giskard/models/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34107 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/models/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.120090 giskard-2.0.0b2/giskard/models/cache/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/models/cache/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/models/cache/cache.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.120267 giskard-2.0.0b2/giskard/models/catboost/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/models/catboost/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.120514 giskard-2.0.0b2/giskard/models/function/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/models/function/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.120775 giskard-2.0.0b2/giskard/models/huggingface/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5880 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/models/huggingface/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.121027 giskard-2.0.0b2/giskard/models/langchain/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2627 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/models/langchain/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6342 2023-06-06 08:49:51.000000 giskard-2.0.0b2/giskard/models/model_explanation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.121212 giskard-2.0.0b2/giskard/models/pytorch/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7213 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/models/pytorch/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.121380 giskard-2.0.0b2/giskard/models/sklearn/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4329 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/models/sklearn/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.121552 giskard-2.0.0b2/giskard/models/tensorflow/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1664 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/models/tensorflow/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-05 15:02:01.000000 giskard-2.0.0b2/giskard/models/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/path_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.123158 giskard-2.0.0b2/giskard/scanner/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-05 15:02:01.000000 giskard-2.0.0b2/giskard/scanner/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.123848 giskard-2.0.0b2/giskard/scanner/calibration/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/calibration/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/scanner/calibration/overconfidence_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/scanner/calibration/underconfidence_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.124342 giskard-2.0.0b2/giskard/scanner/common/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/scanner/common/examples.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/scanner/common/loss_based_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.124636 giskard-2.0.0b2/giskard/scanner/data_leakage/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/scanner/data_leakage/data_leakage_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/issues.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.125634 giskard-2.0.0b2/giskard/scanner/llm/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/scanner/llm/toxicity_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-05 15:02:01.000000 giskard-2.0.0b2/giskard/scanner/llm/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/scanner/logger.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.127031 giskard-2.0.0b2/giskard/scanner/performance/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/performance/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-06 11:35:18.000000 giskard-2.0.0b2/giskard/scanner/performance/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/scanner/performance/metrics.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/scanner/performance/performance_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/scanner/result.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.130190 giskard-2.0.0b2/giskard/scanner/robustness/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/scanner/robustness/base_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/robustness/entity_swap.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      953 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/scanner/robustness/ethical_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-06 11:35:18.000000 giskard-2.0.0b2/giskard/scanner/robustness/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/robustness/nationalities.json
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1006 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/scanner/robustness/text_perturbation_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/scanner/robustness/text_transformations.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/scanner/scanner.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.130396 giskard-2.0.0b2/giskard/scanner/stochasticity/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/stochasticity/stochasticity_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.131723 giskard-2.0.0b2/giskard/scanner/templates/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      785 2023-06-06 14:03:22.000000 giskard-2.0.0b2/giskard/scanner/templates/_code_snippet.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.134526 giskard-2.0.0b2/giskard/scanner/templates/_issues/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/templates/_issues/data_leakage.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/templates/_issues/default.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/scanner/templates/_issues/llm_toxicity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/templates/_issues/overconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/templates/_issues/performance.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/templates/_issues/robustness.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/templates/_issues/stochasticity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/templates/_issues/underconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/scanner/templates/_issues_table.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-04 23:03:53.000000 giskard-2.0.0b2/giskard/scanner/templates/_main_content.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-02 09:24:08.000000 giskard-2.0.0b2/giskard/scanner/templates/_tab_header.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      187 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/templates/base.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-06 14:00:12.000000 giskard-2.0.0b2/giskard/scanner/templates/scan_results.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.136595 giskard-2.0.0b2/giskard/scanner/templates/static/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/templates/static/external.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/templates/static/internal.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-02 09:24:08.000000 giskard-2.0.0b2/giskard/scanner/templates/static/style.css
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.137927 giskard-2.0.0b2/giskard/scanner/visualization/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/scanner/visualization/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/scanner/visualization/custom_jinja.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/settings.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.145877 giskard-2.0.0b2/giskard/slicing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/slicing/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/slicing/base.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/slicing/bruteforce_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/slicing/category_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/slicing/multiscale_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/slicing/opt_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/slicing/slice.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/slicing/stop_words.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/slicing/text_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/slicing/tree_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/slicing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.146049 giskard-2.0.0b2/giskard/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.154471 giskard-2.0.0b2/giskard/testing/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/testing/tests/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33301 2023-06-05 15:58:41.000000 giskard-2.0.0b2/giskard/testing/tests/drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30208 2023-06-05 15:58:41.000000 giskard-2.0.0b2/giskard/testing/tests/metamorphic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25763 2023-06-06 11:47:17.000000 giskard-2.0.0b2/giskard/testing/tests/performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10497 2023-06-06 11:35:18.000000 giskard-2.0.0b2/giskard/testing/tests/statistic.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.161697 giskard-2.0.0b2/giskard/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-02 00:09:24.000000 giskard-2.0.0b2/giskard/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5502 2023-06-05 15:02:01.000000 giskard-2.0.0b2/giskard/utils/analytics_collector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-04 21:20:31.000000 giskard-2.0.0b2/giskard/utils/display.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-05 15:02:01.000000 giskard-2.0.0b2/giskard/utils/environment_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.105140 giskard-2.0.0b2/giskard.egg-info/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    13101 2023-06-06 14:17:49.000000 giskard-2.0.0b2/giskard.egg-info/PKG-INFO
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-06 14:17:49.000000 giskard-2.0.0b2/giskard.egg-info/SOURCES.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-06 14:17:49.000000 giskard-2.0.0b2/giskard.egg-info/dependency_links.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-06 14:17:49.000000 giskard-2.0.0b2/giskard.egg-info/entry_points.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-06 14:17:49.000000 giskard-2.0.0b2/giskard.egg-info/requires.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        8 2023-06-06 14:17:49.000000 giskard-2.0.0b2/giskard.egg-info/top_level.txt
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6808 2023-06-06 14:03:22.000000 giskard-2.0.0b2/pyproject.toml
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-06 14:17:49.166118 giskard-2.0.0b2/setup.cfg
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-02 00:09:24.000000 giskard-2.0.0b2/setup.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 14:17:49.165299 giskard-2.0.0b2/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1521 2023-06-04 23:03:53.000000 giskard-2.0.0b2/tests/test_custom_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-02 00:09:24.000000 giskard-2.0.0b2/tests/test_data_drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-02 00:09:24.000000 giskard-2.0.0b2/tests/test_data_processing_pipeline.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-02 00:09:24.000000 giskard-2.0.0b2/tests/test_dataset.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b2/tests/test_logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-02 00:09:24.000000 giskard-2.0.0b2/tests/test_metamorphic_direction.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-02 00:09:24.000000 giskard-2.0.0b2/tests/test_metamorphic_invariance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2800 2023-06-04 23:03:53.000000 giskard-2.0.0b2/tests/test_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-02 00:09:24.000000 giskard-2.0.0b2/tests/test_model_auto_inference.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-02 00:09:24.000000 giskard-2.0.0b2/tests/test_model_explanation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-02 00:09:24.000000 giskard-2.0.0b2/tests/test_model_postprocess.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-06 11:47:17.000000 giskard-2.0.0b2/tests/test_performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-04 23:03:53.000000 giskard-2.0.0b2/tests/test_programmatic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-02 00:09:24.000000 giskard-2.0.0b2/tests/test_project_uploads.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-02 00:09:24.000000 giskard-2.0.0b2/tests/test_statistical.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-02 00:09:24.000000 giskard-2.0.0b2/tests/test_upload.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-06 13:30:20.000000 giskard-2.0.0b2/tests/test_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.103851 giskard-2.0.0b3/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9939 2023-06-07 01:12:26.104009 giskard-2.0.0b3/PKG-INFO
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8623 2023-06-06 23:34:22.000000 giskard-2.0.0b3/README.md
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.065689 giskard-2.0.0b3/giskard/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1779 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/cli.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/cli_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.067443 giskard-2.0.0b3/giskard/client/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/client/dtos.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/client/giskard_client.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/client/io_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/client/project.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b3/giskard/client/python_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.067851 giskard-2.0.0b3/giskard/commands/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15306 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/commands/cli_server.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7042 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/commands/cli_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.069308 giskard-2.0.0b3/giskard/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11799 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/core.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/dataset_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/errors.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13215 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/model_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/suite.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/core/validation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.069530 giskard-2.0.0b3/giskard/datasets/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.069722 giskard-2.0.0b3/giskard/datasets/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26419 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.070967 giskard-2.0.0b3/giskard/datasets/metadata/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/metadata/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/metadata/indexing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/metadata/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/datasets/metadata/text_metadata_provider.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.071396 giskard-2.0.0b3/giskard/demo/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2931 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/demo/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/demo/titanic.csv
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.071781 giskard-2.0.0b3/giskard/ml_worker/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.072619 giskard-2.0.0b3/giskard/ml_worker/bridge/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/bridge/data_encryptor.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/bridge/error.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/bridge/ml_worker_bridge.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/bridge/service_messages.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.072913 giskard-2.0.0b3/giskard/ml_worker/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/core/log_listener.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5858 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/core/savable.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.073403 giskard-2.0.0b3/giskard/ml_worker/exceptions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/exceptions/IllegalArgumentError.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/exceptions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/exceptions/giskard_exception.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.073740 giskard-2.0.0b3/giskard/ml_worker/generated/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard/ml_worker/generated/ml_worker_pb2.py
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/ml_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.073965 giskard-2.0.0b3/giskard/ml_worker/server/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/server/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26425 2023-06-06 23:20:30.000000 giskard-2.0.0b3/giskard/ml_worker/server/ml_worker_service.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.074966 giskard-2.0.0b3/giskard/ml_worker/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b3/giskard/ml_worker/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.075500 giskard-2.0.0b3/giskard/ml_worker/testing/functions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/functions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3927 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/functions/slicing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6602 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/functions/transformation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.076596 giskard-2.0.0b3/giskard/ml_worker/testing/registry/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/decorators_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/giskard_test.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/slicing_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/transformation_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/registry/udf_repository.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/stat_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/testing/test_result.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/ml_worker/testing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.077513 giskard-2.0.0b3/giskard/ml_worker/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b3/giskard/ml_worker/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/utils/file_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/utils/logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1952 2023-06-06 23:20:13.000000 giskard-2.0.0b3/giskard/ml_worker/utils/network.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/ml_worker/utils/request_interceptor.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.078153 giskard-2.0.0b3/giskard/models/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/_precooked.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.078300 giskard-2.0.0b3/giskard/models/automodel/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9181 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/automodel/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.078562 giskard-2.0.0b3/giskard/models/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34228 2023-06-06 23:20:04.000000 giskard-2.0.0b3/giskard/models/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.079220 giskard-2.0.0b3/giskard/models/cache/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/cache/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/cache/cache.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.079379 giskard-2.0.0b3/giskard/models/catboost/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/catboost/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.079529 giskard-2.0.0b3/giskard/models/function/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/function/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.079670 giskard-2.0.0b3/giskard/models/huggingface/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/huggingface/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.079892 giskard-2.0.0b3/giskard/models/langchain/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2619 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/langchain/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6342 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/model_explanation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.080100 giskard-2.0.0b3/giskard/models/pytorch/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/pytorch/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.080241 giskard-2.0.0b3/giskard/models/sklearn/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/sklearn/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.080425 giskard-2.0.0b3/giskard/models/tensorflow/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1656 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/models/tensorflow/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/models/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/path_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.082073 giskard-2.0.0b3/giskard/scanner/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.082613 giskard-2.0.0b3/giskard/scanner/calibration/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/calibration/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/calibration/overconfidence_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/calibration/underconfidence_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.082973 giskard-2.0.0b3/giskard/scanner/common/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/common/examples.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/common/loss_based_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.083136 giskard-2.0.0b3/giskard/scanner/data_leakage/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/data_leakage/data_leakage_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/issues.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.083434 giskard-2.0.0b3/giskard/scanner/llm/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/llm/toxicity_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/llm/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/logger.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.084030 giskard-2.0.0b3/giskard/scanner/performance/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/performance/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/performance/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/performance/metrics.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/performance/performance_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/result.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.087237 giskard-2.0.0b3/giskard/scanner/robustness/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/base_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/entity_swap.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      953 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/ethical_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/nationalities.json
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1006 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/text_perturbation_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/robustness/text_transformations.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/scanner.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.087470 giskard-2.0.0b3/giskard/scanner/stochasticity/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/stochasticity/stochasticity_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.089440 giskard-2.0.0b3/giskard/scanner/templates/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      785 2023-06-06 23:34:22.000000 giskard-2.0.0b3/giskard/scanner/templates/_code_snippet.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.092000 giskard-2.0.0b3/giskard/scanner/templates/_issues/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/data_leakage.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/default.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/llm_toxicity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/overconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/performance.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/robustness.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/stochasticity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues/underconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_issues_table.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_main_content.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/_tab_header.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      187 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/base.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/scan_results.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.093225 giskard-2.0.0b3/giskard/scanner/templates/static/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/static/external.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/static/internal.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/templates/static/style.css
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.093537 giskard-2.0.0b3/giskard/scanner/visualization/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/visualization/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/scanner/visualization/custom_jinja.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/settings.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.096141 giskard-2.0.0b3/giskard/slicing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/base.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/bruteforce_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/category_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/multiscale_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/opt_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/slice.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/stop_words.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/text_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/tree_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/slicing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.096463 giskard-2.0.0b3/giskard/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.099022 giskard-2.0.0b3/giskard/testing/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/testing/tests/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33167 2023-06-06 20:59:14.000000 giskard-2.0.0b3/giskard/testing/tests/drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30208 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/testing/tests/metamorphic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25823 2023-06-06 21:06:58.000000 giskard-2.0.0b3/giskard/testing/tests/performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10497 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/testing/tests/statistic.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.099810 giskard-2.0.0b3/giskard/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6206 2023-06-07 01:11:58.000000 giskard-2.0.0b3/giskard/utils/analytics_collector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/utils/display.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-06 19:53:55.000000 giskard-2.0.0b3/giskard/utils/environment_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.066669 giskard-2.0.0b3/giskard.egg-info/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9939 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/PKG-INFO
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/SOURCES.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/dependency_links.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/entry_points.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/requires.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        8 2023-06-07 01:12:26.000000 giskard-2.0.0b3/giskard.egg-info/top_level.txt
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7375 2023-06-06 23:34:22.000000 giskard-2.0.0b3/pyproject.toml
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-07 01:12:26.104443 giskard-2.0.0b3/setup.cfg
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-06 19:53:55.000000 giskard-2.0.0b3/setup.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 01:12:26.103629 giskard-2.0.0b3/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1513 2023-06-06 20:59:14.000000 giskard-2.0.0b3/tests/test_custom_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_data_drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_data_processing_pipeline.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_dataset.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b3/tests/test_logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_metamorphic_direction.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_metamorphic_invariance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2409 2023-06-06 21:05:44.000000 giskard-2.0.0b3/tests/test_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_model_auto_inference.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_model_explanation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_model_postprocess.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_programmatic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_project_uploads.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_statistical.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_upload.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-06 19:53:55.000000 giskard-2.0.0b3/tests/test_utils.py
```

### Comparing `giskard-2.0.0b2/giskard/__init__.py` & `giskard-2.0.0b3/giskard/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/cli.py` & `giskard-2.0.0b3/giskard/cli.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/cli_utils.py` & `giskard-2.0.0b3/giskard/cli_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/client/giskard_client.py` & `giskard-2.0.0b3/giskard/client/giskard_client.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/client/io_utils.py` & `giskard-2.0.0b3/giskard/client/io_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/client/project.py` & `giskard-2.0.0b3/giskard/client/project.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/client/python_utils.py` & `giskard-2.0.0b3/giskard/client/python_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/commands/cli_server.py` & `giskard-2.0.0b3/giskard/commands/cli_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 client = giskard.GiskardClient(\"{http_tunnel.public_url}\", token)
 
 # To run your model with the Giskard Server, execute these three lines on Google Colab:
 
 %env GSK_EXTERNAL_ML_WORKER_HOST={tcp_addr.hostname}
 %env GSK_EXTERNAL_ML_WORKER_PORT={tcp_addr.port}
 %env GSK_API_KEY=...
-!giskard worker start -u {http_tunnel.public_url}""")
+!giskard worker start -d -u {http_tunnel.public_url}""")
 
     ngrok_process = ngrok.get_ngrok_process()
     try:
         # Block until CTRL-C or some other terminating event
         ngrok_process.proc.wait()
     finally:
         print("Shutting down expose.")
```

### Comparing `giskard-2.0.0b2/giskard/commands/cli_worker.py` & `giskard-2.0.0b3/giskard/commands/cli_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/core/core.py` & `giskard-2.0.0b3/giskard/core/core.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/core/dataset_validation.py` & `giskard-2.0.0b3/giskard/core/dataset_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/core/errors.py` & `giskard-2.0.0b3/giskard/core/errors.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/core/model_validation.py` & `giskard-2.0.0b3/giskard/core/model_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/core/suite.py` & `giskard-2.0.0b3/giskard/core/suite.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/core/validation.py` & `giskard-2.0.0b3/giskard/core/validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/datasets/__init__.py` & `giskard-2.0.0b3/giskard/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/datasets/base/__init__.py` & `giskard-2.0.0b3/giskard/datasets/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/datasets/metadata/indexing.py` & `giskard-2.0.0b3/giskard/datasets/metadata/indexing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/datasets/metadata/registry.py` & `giskard-2.0.0b3/giskard/datasets/metadata/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/datasets/metadata/text_metadata_provider.py` & `giskard-2.0.0b3/giskard/datasets/metadata/text_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/demo/__init__.py` & `giskard-2.0.0b3/giskard/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/demo/titanic.csv` & `giskard-2.0.0b3/giskard/demo/titanic.csv`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/bridge/data_encryptor.py` & `giskard-2.0.0b3/giskard/ml_worker/bridge/data_encryptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/bridge/ml_worker_bridge.py` & `giskard-2.0.0b3/giskard/ml_worker/bridge/ml_worker_bridge.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/core/log_listener.py` & `giskard-2.0.0b3/giskard/ml_worker/core/log_listener.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/core/savable.py` & `giskard-2.0.0b3/giskard/ml_worker/core/savable.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/generated/ml_worker_pb2.py` & `giskard-2.0.0b3/giskard/ml_worker/generated/ml_worker_pb2.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/generated/ml_worker_pb2_grpc.py` & `giskard-2.0.0b3/giskard/ml_worker/generated/ml_worker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/ml_worker.py` & `giskard-2.0.0b3/giskard/ml_worker/ml_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/server/ml_worker_service.py` & `giskard-2.0.0b3/giskard/ml_worker/server/ml_worker_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import asyncio
 import logging
-import math
 import os
 import platform
 import sys
 import tempfile
 import time
 from io import StringIO
 from pathlib import Path
 
 import google
 import grpc
+import math
 import numpy as np
 import pandas as pd
 import pkg_resources
 import psutil
 import tqdm
 
 import giskard
@@ -343,15 +343,15 @@
         input_df = pd.DataFrame({k: [v] for k, v in request.columns.items()})
         if model.meta.feature_names:
             input_df = input_df[model.meta.feature_names]
         (list_words, list_weights) = explain_text(model, input_df, text_column, text_document, n_samples)
         map_features_weight = dict(zip(model.meta.classification_labels, list_weights))
         return ml_worker_pb2.ExplainTextResponse(
             weights={
-                k: ml_worker_pb2.ExplainTextResponse.WeightsPerFeature(
+                str(k): ml_worker_pb2.ExplainTextResponse.WeightsPerFeature(
                     weights=[weight for weight in map_features_weight[k]]
                 )
                 for k in map_features_weight
             },
             words=list_words,
         )
 
@@ -533,15 +533,16 @@
             slices=map_dataset_process_function_meta('SLICE'),
             transformations=map_dataset_process_function_meta('TRANSFORMATION')
         )
 
     @staticmethod
     def pandas_df_to_proto_df(df):
         return ml_worker_pb2.DataFrame(
-            rows=[ml_worker_pb2.DataRow(columns=r.astype(str).to_dict()) for _, r in df.iterrows()]
+            rows=[ml_worker_pb2.DataRow(columns={str(k): v for k, v in r.astype(str).to_dict().items()}) for _, r in
+                  df.iterrows()]
         )
 
     @staticmethod
     def pandas_series_to_proto_series(self, series):
         return
```

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/functions/slicing.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/functions/slicing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/functions/transformation.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/functions/transformation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/registry/decorators.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/registry/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/registry/decorators_utils.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/registry/decorators_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/registry/giskard_test.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/registry/giskard_test.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/registry/registry.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/registry/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/registry/slicing_function.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/registry/slicing_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/registry/transformation_function.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/registry/transformation_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/registry/udf_repository.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/registry/udf_repository.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/stat_utils.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/stat_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/test_result.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/test_result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/testing/utils.py` & `giskard-2.0.0b3/giskard/ml_worker/testing/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
 from functools import wraps
+import numbers
 from typing import Optional
 
 from giskard.datasets.base import Dataset
 from giskard.core.core import SupportedModelTypes
 
 
 class Direction(Enum):
@@ -16,19 +17,32 @@
     @wraps(func)
     def wrapper(*args, **kwargs):
         reference_slice = kwargs.get('reference_dataset', None)
         actual_slice = kwargs.get('dataset', None)
         model = kwargs.get('model', None)
         classification_label = kwargs.get('classification_label', None)
         target = getattr(reference_slice, 'target', getattr(actual_slice, 'target', None))
+
+        # Try to automatically cast `classification_label` to the right type
+        if (
+            classification_label is not None
+            and model is not None
+            and isinstance(model.meta.classification_labels[0], numbers.Number)
+        ):
+            try:
+                classification_label = int(classification_label)
+            except ValueError:
+                pass
+
+        # Validate the label
         if target and classification_label and model:
             assert classification_label != target, (
-                f'By "classification_label", we refer to one of the values: '
+                'By "classification_label", we refer to one of the values: '
                 f'{model.meta.classification_labels} and not the target: "{target}". '
-                f'Please re-assign this argument.'
+                'Please re-assign this argument.'
             )
 
         assert (
             model.meta.model_type != SupportedModelTypes.CLASSIFICATION
             or classification_label in model.meta.classification_labels
         ), f'"{classification_label}" is not part of model labels: {model.meta.classification_labels}'
         return func(*args, **kwargs)
```

### Comparing `giskard-2.0.0b2/giskard/ml_worker/utils/logging.py` & `giskard-2.0.0b3/giskard/ml_worker/utils/logging.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/ml_worker/utils/network.py` & `giskard-2.0.0b3/giskard/ml_worker/utils/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,12 +49,12 @@
             latest_release_date = max(map(lambda r: datetime.datetime.fromisoformat(r['upload_time']), resources))
             releases_dates[ver] = latest_release_date
         latest_version, latest_release_date = max(releases_dates.items(), key=lambda x: x[1])
 
         if latest_release_date > releases_dates[current_version]:
             warning(
                 "You're using a pre-release version of giskard while a "
-                "new version is available, please install it with\n"
-                f"pip install giskard=={latest_version}"
+                "new version is available, please install it with: "
+                f"pip install \"giskard=={latest_version}\""
             )
     except BaseException as e:
         logger.exception("Failed to fetch latest giskard version", e)
```

### Comparing `giskard-2.0.0b2/giskard/ml_worker/utils/request_interceptor.py` & `giskard-2.0.0b3/giskard/ml_worker/utils/request_interceptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/models/__init__.py` & `giskard-2.0.0b3/giskard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/models/_precooked.py` & `giskard-2.0.0b3/giskard/models/_precooked.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/models/automodel/__init__.py` & `giskard-2.0.0b3/giskard/models/automodel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,16 @@
             is_overriden = cls.__name__ != 'Model'  # TODO: Improve this
             if is_overriden:
                 if not giskard_cls:
                     giskard_cls = CloudpickleBasedModel
                 # if save_model and load_model are overriden, replace them, if not, these equalities will be identities.
                 possibly_overriden_cls = cls
                 possibly_overriden_cls.save_model = giskard_cls.save_model
-                possibly_overriden_cls.load_wrapped_model = giskard_cls.load_wrapped_model
+                possibly_overriden_cls.load_model = giskard_cls.load_model
+                possibly_overriden_cls.should_save_model_class = True
             elif giskard_cls:
                 input_type = "'prediction_function'" if giskard_cls == PredictionFunctionModel else "'model'"
                 logger.info(
                     "Your "
                     + input_type
                     + " is successfully wrapped by Giskard's '"
                     + str(giskard_cls.__name__)
```

### Comparing `giskard-2.0.0b2/giskard/models/base/__init__.py` & `giskard-2.0.0b3/giskard/models/base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,15 +357,15 @@
             raw_prediction = self.predict_df(unpredicted_df)
             self._cache.set_cache(dataset.row_hashes[missing], raw_prediction)
             cached_predictions.loc[missing] = raw_prediction.tolist()
 
         # TODO: check if there is a better solution
         return np.array(np.array(cached_predictions).tolist())
 
-    def upload(self, client: GiskardClient, project_key, validate_ds=None) -> None:
+    def upload(self, client: GiskardClient, project_key, validate_ds=None) -> str:
         """
         Uploads the model to a Giskard project using the provided Giskard client. Also validates the model
         using the given validation dataset, if any.
 
         Args:
             client (GiskardClient): A Giskard client instance to use for uploading the model.
             project_key (str): The project key to use for the upload.
@@ -381,14 +381,16 @@
         with tempfile.TemporaryDirectory(prefix="giskard-model-") as f:
             self.save(f)
 
             if client is not None:
                 client.log_artifacts(f, posixpath.join(project_key, "models", str(self.id)))
                 client.save_model_meta(project_key, self.id, self.meta, platform.python_version(), get_size(f))
 
+        return str(self.id)
+
     @classmethod
     def download(cls, client: GiskardClient, project_key, model_id):
         """
         Downloads the specified model from the Giskard server and loads it into memory.
 
         Args:
             client (GiskardClient): The client instance that will connect to the Giskard server.
@@ -469,15 +471,18 @@
         constructor_params["id"] = model_id
         del constructor_params["loader_module"]
         del constructor_params["loader_class"]
 
         if class_file.exists():
             with open(class_file, "rb") as f:
                 clazz = cloudpickle.load(f)
-                return clazz(**(constructor_params | kwargs))
+                clazz_kwargs = {}
+                clazz_kwargs.update(constructor_params)
+                clazz_kwargs.update(kwargs)
+                return clazz(**clazz_kwargs)
         else:
             raise ValueError(
                 f"Cannot load model ({cls.__module__}.{cls.__name__}), "
                 f"{MODEL_CLASS_PKL} file not found and 'load' method isn't overriden"
             )
 
 
@@ -666,19 +671,19 @@
         kwargs["model_postprocessing_function"] = cls.load_model_postprocessing_function(local_dir)
         model_id, meta = cls.read_meta_from_local_dir(local_dir)
         constructor_params = meta.__dict__
         constructor_params["id"] = model_id
         constructor_params = constructor_params.copy()
         constructor_params.update(kwargs)
 
-        return cls(model=cls.load_wrapped_model(local_dir), **constructor_params)
+        return cls(model=cls.load_model(local_dir), **constructor_params)
 
     @classmethod
     @abstractmethod
-    def load_wrapped_model(cls, local_dir):
+    def load_model(cls, local_dir):
         """
         Loading the ``model`` object. The de-serialization depends on the model type:
 
         - ``mlflow`` methods are used if the ``model`` is from either of ``sklearn``, ``catboost``, ``pytorch`` or ``tensorflow``.
         - ``transformers`` methods are used if the ``model`` is from ``huggingface``.
         - ``langchain`` methods are used if the ``model`` is from ``langchain``.
         """
@@ -740,15 +745,15 @@
         except ValueError:
             raise ValueError(
                 "We couldn't save your model with cloudpickle. Please provide us with your own "
                 "serialisation method by overriding the save_model() and load_model() methods."
             )
 
     @classmethod
-    def load_wrapped_model(cls, local_dir):
+    def load_model(cls, local_dir):
         local_path = Path(local_dir)
         model_path = local_path / "model.pkl"
         if model_path.exists():
             with open(model_path, "rb") as f:
                 model = cloudpickle.load(f)
                 return model
         else:
```

### Comparing `giskard-2.0.0b2/giskard/models/cache/__init__.py` & `giskard-2.0.0b3/giskard/models/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/models/cache/cache.py` & `giskard-2.0.0b3/giskard/models/cache/cache.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/models/catboost/__init__.py` & `giskard-2.0.0b3/giskard/models/catboost/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/models/function/__init__.py` & `giskard-2.0.0b3/giskard/models/function/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/models/huggingface/__init__.py` & `giskard-2.0.0b3/giskard/models/huggingface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             **kwargs,
         )
 
         self.huggingface_module = model.__class__
         self.pipeline_task = model.task if isinstance(model, pipelines.Pipeline) else None
 
     @classmethod
-    def load_wrapped_model(cls, local_path):
+    def load_model(cls, local_path):
         huggingface_meta_file = Path(local_path) / "giskard-model-huggingface-meta.yaml"
         if huggingface_meta_file.exists():
             with open(huggingface_meta_file) as f:
                 huggingface_meta = yaml.load(f, Loader=yaml.Loader)
 
         if huggingface_meta["pipeline_task"]:
             return pipeline(huggingface_meta["pipeline_task"], local_path)
```

### Comparing `giskard-2.0.0b2/giskard/models/langchain/__init__.py` & `giskard-2.0.0b3/giskard/models/langchain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             **kwargs,
         )
 
     def save_model(self, local_path, mlflow_meta):
         mlflow.langchain.save_model(self.model, path=local_path, mlflow_model=mlflow_meta)
 
     @classmethod
-    def load_wrapped_model(cls, local_dir):
+    def load_model(cls, local_dir):
         return mlflow.langchain.load_model(local_dir)
 
     def model_predict(self, df):
         return [self.model.predict(**data) for data in df.to_dict('records')]
 
     def rewrite_prompt(self, template, input_variables=None, **kwargs):
         from langchain import LLMChain
```

### Comparing `giskard-2.0.0b2/giskard/models/model_explanation.py` & `giskard-2.0.0b3/giskard/models/model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/models/pytorch/__init__.py` & `giskard-2.0.0b3/giskard/models/pytorch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         )
 
         self.device = device
         self.torch_dtype = torch_dtype
         self.iterate_dataset = iterate_dataset
 
     @classmethod
-    def load_wrapped_model(cls, local_dir):
+    def load_model(cls, local_dir):
         return mlflow.pytorch.load_model(local_dir)
 
     def save_model(self, local_path, mlflow_meta: mlflow.models.Model):
         mlflow.pytorch.save_model(self.model, path=local_path, mlflow_model=mlflow_meta)
 
     def _get_predictions_from_iterable(self, data):
         # Fault tolerance: try to convert to the right format in special cases
```

### Comparing `giskard-2.0.0b2/giskard/models/sklearn/__init__.py` & `giskard-2.0.0b3/giskard/models/sklearn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             raise ValueError("Unsupported model type")
 
         mlflow.sklearn.save_model(
             self.model, path=local_path, pyfunc_predict_fn=pyfunc_predict_fn, mlflow_model=mlflow_meta
         )
 
     @classmethod
-    def load_wrapped_model(cls, local_dir):
+    def load_model(cls, local_dir):
         return mlflow.sklearn.load_model(local_dir)
 
     def model_predict(self, df):
         if self.is_regression:
             return self.model.predict(df)
         else:
             return self.model.predict_proba(df)
```

### Comparing `giskard-2.0.0b2/giskard/models/tensorflow/__init__.py` & `giskard-2.0.0b3/giskard/models/tensorflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             feature_names=feature_names,
             classification_threshold=classification_threshold,
             classification_labels=classification_labels,
             **kwargs
         )
 
     @classmethod
-    def load_wrapped_model(cls, local_path):
+    def load_model(cls, local_path):
         return mlflow.tensorflow.load_model(local_path)
 
     def save_model(self, local_path, mlflow_meta: mlflow.models.Model):
         mlflow.tensorflow.save_model(self.model, path=local_path, mlflow_model=mlflow_meta)
 
     def model_predict(self, data):
         return self.model.predict(data)
```

### Comparing `giskard-2.0.0b2/giskard/models/utils.py` & `giskard-2.0.0b3/giskard/models/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/path_utils.py` & `giskard-2.0.0b3/giskard/path_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/__init__.py` & `giskard-2.0.0b3/giskard/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/calibration/issues.py` & `giskard-2.0.0b3/giskard/scanner/calibration/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/calibration/overconfidence_detector.py` & `giskard-2.0.0b3/giskard/scanner/calibration/overconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/calibration/underconfidence_detector.py` & `giskard-2.0.0b3/giskard/scanner/calibration/underconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/common/examples.py` & `giskard-2.0.0b3/giskard/scanner/common/examples.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/common/loss_based_detector.py` & `giskard-2.0.0b3/giskard/scanner/common/loss_based_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/data_leakage/data_leakage_detector.py` & `giskard-2.0.0b3/giskard/scanner/data_leakage/data_leakage_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/decorators.py` & `giskard-2.0.0b3/giskard/scanner/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/issues.py` & `giskard-2.0.0b3/giskard/scanner/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/llm/toxicity_detector.py` & `giskard-2.0.0b3/giskard/scanner/llm/toxicity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/llm/utils.py` & `giskard-2.0.0b3/giskard/scanner/llm/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/performance/issues.py` & `giskard-2.0.0b3/giskard/scanner/performance/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/performance/metrics.py` & `giskard-2.0.0b3/giskard/scanner/performance/metrics.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/performance/performance_bias_detector.py` & `giskard-2.0.0b3/giskard/scanner/performance/performance_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/registry.py` & `giskard-2.0.0b3/giskard/scanner/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/result.py` & `giskard-2.0.0b3/giskard/scanner/result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/robustness/base_detector.py` & `giskard-2.0.0b3/giskard/scanner/robustness/base_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/robustness/entity_swap.py` & `giskard-2.0.0b3/giskard/scanner/robustness/entity_swap.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/robustness/ethical_bias_detector.py` & `giskard-2.0.0b3/giskard/scanner/robustness/ethical_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/robustness/issues.py` & `giskard-2.0.0b3/giskard/scanner/robustness/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/robustness/nationalities.json` & `giskard-2.0.0b3/giskard/scanner/robustness/nationalities.json`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/robustness/text_perturbation_detector.py` & `giskard-2.0.0b3/giskard/scanner/robustness/text_perturbation_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/robustness/text_transformations.py` & `giskard-2.0.0b3/giskard/scanner/robustness/text_transformations.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/scanner.py` & `giskard-2.0.0b3/giskard/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/stochasticity/stochasticity_detector.py` & `giskard-2.0.0b3/giskard/scanner/stochasticity/stochasticity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_code_snippet.html` & `giskard-2.0.0b3/giskard/scanner/templates/_code_snippet.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
     <div class="text-sm">
         <pre><code class="language-python rounded">{% raw %}from giskard import GiskardClient
 test_suite = results.generate_test_suite("My first test suite")
 
 # To start the Giskard server, run in your terminal within the Python
 # environment containing the dependencies of your model: 
-giskard server start --version 2.0.0b2
+giskard server start --version 2.0.0b3
 giskard worker start -u http://localhost:19000/
 
 # Then upload your test suite to the opened Giskard server
 client = GiskardClient("http://localhost:19000", "GISKARD_API_KEY")
 client.create_project("my_project_id", "my_project_name")
 test_suite.upload(client, "my_project_id"){% endraw %}
 </code></pre>
```

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_issues/data_leakage.html` & `giskard-2.0.0b3/giskard/scanner/templates/_issues/data_leakage.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_issues/default.html` & `giskard-2.0.0b3/giskard/scanner/templates/_issues/default.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_issues/llm_toxicity.html` & `giskard-2.0.0b3/giskard/scanner/templates/_issues/llm_toxicity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_issues/overconfidence.html` & `giskard-2.0.0b3/giskard/scanner/templates/_issues/overconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_issues/performance.html` & `giskard-2.0.0b3/giskard/scanner/templates/_issues/performance.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_issues/robustness.html` & `giskard-2.0.0b3/giskard/scanner/templates/_issues/robustness.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_issues/stochasticity.html` & `giskard-2.0.0b3/giskard/scanner/templates/_issues/stochasticity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_issues/underconfidence.html` & `giskard-2.0.0b3/giskard/scanner/templates/_issues/underconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_issues_table.html` & `giskard-2.0.0b3/giskard/scanner/templates/_issues_table.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_main_content.html` & `giskard-2.0.0b3/giskard/scanner/templates/_main_content.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/_tab_header.html` & `giskard-2.0.0b3/giskard/scanner/templates/_tab_header.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/scan_results.html` & `giskard-2.0.0b3/giskard/scanner/templates/scan_results.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/static/external.js` & `giskard-2.0.0b3/giskard/scanner/templates/static/external.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/static/internal.js` & `giskard-2.0.0b3/giskard/scanner/templates/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/templates/static/style.css` & `giskard-2.0.0b3/giskard/scanner/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/scanner/visualization/custom_jinja.py` & `giskard-2.0.0b3/giskard/scanner/visualization/custom_jinja.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/settings.py` & `giskard-2.0.0b3/giskard/settings.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/slicing/base.py` & `giskard-2.0.0b3/giskard/slicing/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/slicing/bruteforce_slicer.py` & `giskard-2.0.0b3/giskard/slicing/bruteforce_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/slicing/category_slicer.py` & `giskard-2.0.0b3/giskard/slicing/category_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/slicing/multiscale_slicer.py` & `giskard-2.0.0b3/giskard/slicing/multiscale_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/slicing/opt_slicer.py` & `giskard-2.0.0b3/giskard/slicing/opt_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/slicing/slice.py` & `giskard-2.0.0b3/giskard/slicing/slice.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/slicing/stop_words.py` & `giskard-2.0.0b3/giskard/slicing/stop_words.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/slicing/text_slicer.py` & `giskard-2.0.0b3/giskard/slicing/text_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/slicing/tree_slicer.py` & `giskard-2.0.0b3/giskard/slicing/tree_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/slicing/utils.py` & `giskard-2.0.0b3/giskard/slicing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/testing/__init__.py` & `giskard-2.0.0b3/giskard/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/testing/tests/drift.py` & `giskard-2.0.0b3/giskard/testing/tests/drift.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numbers
 import re
 import typing
 import uuid
 from collections import Counter
 from typing import Optional, List
 
 import numpy as np
@@ -111,15 +112,15 @@
     # it's necessary for comparison purposes to normalize expected_frequencies
     # so that reference and actual has the same size
     # See https://github.com/scipy/scipy/blob/v1.8.0/scipy/stats/_stats_py.py#L6787
     k_norm = actual_series.shape[0] / reference_series.shape[0]
     output_data = pd.DataFrame(columns=["Modality", "Reference_frequencies", "Actual_frequencies", "Chi_square"])
     for i in range(len(all_modalities)):
         chi_square_value = (actual_frequencies[i] - expected_frequencies[i] * k_norm) ** 2 / (
-                expected_frequencies[i] * k_norm
+            expected_frequencies[i] * k_norm
         )
         chi_square += chi_square_value
 
         row = {
             "Modality": all_modalities[i],
             "Reference_frequencies": expected_frequencies[i],
             "Actual_frequencies": actual_frequencies[i],
@@ -134,24 +135,24 @@
     else:
         p_value = 0
     return chi_square, p_value, output_data
 
 
 def _validate_feature_type(gsk_dataset, column_name, feature_type):
     assert (
-            gsk_dataset.column_types[column_name] == feature_type
+        gsk_dataset.column_types[column_name] == feature_type
     ), f'Column "{column_name}" is not of type "{feature_type}"'
 
 
 def _validate_column_name(actual_ds, reference_ds, column_name):
     assert (
-            column_name in actual_ds.columns
+        column_name in actual_ds.columns
     ), f'"{column_name}" is not a column of Actual Dataset Columns: {", ".join(actual_ds.columns)}'
     assert (
-            column_name in reference_ds.columns
+        column_name in reference_ds.columns
     ), f'"{column_name}" is not a column of Reference Dataset Columns: {", ".join(reference_ds.columns)}'
 
 
 def _validate_series_notempty(actual_series, reference_series):
     if actual_series.empty:
         raise ValueError("Actual Series computed from the column is empty")
     if reference_series.empty:
@@ -165,18 +166,23 @@
     actual_series = actual_ds.df[column_name]
     reference_series = reference_ds.df[column_name]
     _validate_series_notempty(actual_series, reference_series)
     return actual_series, reference_series
 
 
 @test(name='Categorical drift (PSI)')
-def test_drift_psi(actual_dataset: Dataset, reference_dataset: Dataset, column_name: str,
-                   slicing_function: Optional[SlicingFunction] = None,
-                   threshold: float = 0.2, max_categories: int = 20,
-                   psi_contribution_percent: float = 0.2) -> TestResult:
+def test_drift_psi(
+    actual_dataset: Dataset,
+    reference_dataset: Dataset,
+    column_name: str,
+    slicing_function: Optional[SlicingFunction] = None,
+    threshold: float = 0.2,
+    max_categories: int = 20,
+    psi_contribution_percent: float = 0.2,
+) -> TestResult:
     """
     Test if the PSI score between the actual and reference datasets is below the threshold for
     a given categorical feature
 
     Example : The test is passed when the  PSI score of gender between reference and actual sets is below 0.2
 
     Args:
@@ -210,17 +216,15 @@
     if slicing_function:
         test_name = "test_drift_psi"
         actual_dataset = actual_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
         reference_dataset = reference_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
 
-    actual_series, reference_series = _extract_series(actual_dataset,
-                                                      reference_dataset,
-                                                      column_name, "category")
+    actual_series, reference_series = _extract_series(actual_dataset, reference_dataset, column_name, "category")
 
     messages, passed, total_psi = _test_series_drift_psi(
         actual_series,
         reference_series,
         "data",
         max_categories,
         psi_contribution_percent,
@@ -233,17 +237,23 @@
         passed=passed,
         metric=total_psi,
         messages=messages,
     )
 
 
 @test(name='Categorical drift (Chi-squared)')
-def test_drift_chi_square(actual_dataset: Dataset, reference_dataset: Dataset, column_name: str,
-                          slicing_function: Optional[SlicingFunction] = None, threshold: float = 0.05,
-                          max_categories: int = 20, chi_square_contribution_percent: float = 0.2) -> TestResult:
+def test_drift_chi_square(
+    actual_dataset: Dataset,
+    reference_dataset: Dataset,
+    column_name: str,
+    slicing_function: Optional[SlicingFunction] = None,
+    threshold: float = 0.05,
+    max_categories: int = 20,
+    chi_square_contribution_percent: float = 0.2,
+) -> TestResult:
     """
     Test if the p-value of the chi square test between the actual and reference datasets is
     above the threshold for a given categorical feature
 
     Example : The test is passed when the pvalue of the chi square test of the categorical variable between
      reference and actual sets is higher than 0.05. It means that chi square test cannot be rejected at 5% level
      and that we cannot assume drift for this variable.
@@ -279,17 +289,15 @@
     if slicing_function:
         test_name = "test_drift_chi_square"
         actual_dataset = actual_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
         reference_dataset = reference_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
 
-    actual_series, reference_series = _extract_series(actual_dataset,
-                                                      reference_dataset,
-                                                      column_name, "category")
+    actual_series, reference_series = _extract_series(actual_dataset, reference_dataset, column_name, "category")
 
     messages, p_value, passed = _test_series_drift_chi(
         actual_series,
         reference_series,
         "data",
         chi_square_contribution_percent,
         max_categories,
@@ -302,17 +310,21 @@
         passed=passed,
         metric=p_value,
         messages=messages,
     )
 
 
 @test(name='Numerical drift (Kolmogorov-Smirnov)')
-def test_drift_ks(actual_dataset: Dataset, reference_dataset: Dataset, column_name: str,
-                  slicing_function: Optional[SlicingFunction] = None,
-                  threshold: float = 0.05) -> TestResult:
+def test_drift_ks(
+    actual_dataset: Dataset,
+    reference_dataset: Dataset,
+    column_name: str,
+    slicing_function: Optional[SlicingFunction] = None,
+    threshold: float = 0.05,
+) -> TestResult:
     """
     Test if the pvalue of the KS test between the actual and reference datasets is above
     the threshold for a given numerical feature
 
     Example : The test is passed when the pvalue of the KS test of the numerical variable
     between the actual and reference datasets is higher than 0.05. It means that the KS test
     cannot be rejected at 5% level and that we cannot assume drift for this variable.
@@ -342,36 +354,39 @@
     if slicing_function:
         test_name = "test_drift_ks"
         actual_dataset = actual_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
         reference_dataset = reference_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
 
-    actual_series, reference_series = _extract_series(actual_dataset,
-                                                      reference_dataset,
-                                                      column_name, "numeric")
+    actual_series, reference_series = _extract_series(actual_dataset, reference_dataset, column_name, "numeric")
 
     result = _calculate_ks(actual_series, reference_series)
 
     passed = bool(result.pvalue >= threshold)
 
     messages = _generate_message_ks(passed, result, threshold, "data")
 
     return TestResult(
         actual_slices_size=[len(actual_series)],
         reference_slices_size=[len(reference_series)],
         passed=passed,
         metric=result.pvalue,
-        messages=messages
+        messages=messages,
     )
 
 
 @test(name='Numerical drift (Earth mover\'s distance)')
-def test_drift_earth_movers_distance(actual_dataset: Dataset, reference_dataset: Dataset, column_name: str,
-                                     slicing_function: Optional[SlicingFunction] = None, threshold: float = 0.2) -> TestResult:
+def test_drift_earth_movers_distance(
+    actual_dataset: Dataset,
+    reference_dataset: Dataset,
+    column_name: str,
+    slicing_function: Optional[SlicingFunction] = None,
+    threshold: float = 0.2,
+) -> TestResult:
     """
     Test if the earth movers distance between the actual and reference datasets is
     below the threshold for a given numerical feature
 
     Example : The test is passed when the earth movers distance of the numerical
      variable between the actual and reference datasets is lower than 0.1.
      It means that we cannot assume drift for this variable.
@@ -401,17 +416,15 @@
     if slicing_function:
         test_name = "test_drift_earth_movers_distance"
         actual_dataset = actual_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
         reference_dataset = reference_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
 
-    actual_series, reference_series = _extract_series(actual_dataset,
-                                                      reference_dataset,
-                                                      column_name, "numeric")
+    actual_series, reference_series = _extract_series(actual_dataset, reference_dataset, column_name, "numeric")
 
     metric = _calculate_earth_movers_distance(actual_series, reference_series)
 
     passed = bool(metric <= threshold)
 
     messages: Optional[List[TestMessage]] = None
 
@@ -428,17 +441,23 @@
         passed=True if threshold is None else passed,
         metric=metric,
         messages=messages,
     )
 
 
 @test(name='Label drift (PSI)')
-def test_drift_prediction_psi(model: BaseModel, actual_dataset: Dataset, reference_dataset: Dataset,
-                              slicing_function: Optional[SlicingFunction] = None, max_categories: int = 10,
-                              threshold: float = 0.2, psi_contribution_percent: float = 0.2):
+def test_drift_prediction_psi(
+    model: BaseModel,
+    actual_dataset: Dataset,
+    reference_dataset: Dataset,
+    slicing_function: Optional[SlicingFunction] = None,
+    max_categories: int = 10,
+    threshold: float = 0.2,
+    psi_contribution_percent: float = 0.2,
+):
     """
     Test if the PSI score between the reference and actual datasets is below the threshold
     for the classification labels predictions
 
     Example : The test is passed when the  PSI score of classification labels prediction
     for females between reference and actual sets is below 0.2
 
@@ -496,20 +515,20 @@
         passed=passed,
         metric=total_psi,
         messages=messages,
     )
 
 
 def _test_series_drift_psi(
-        actual_series,
-        reference_series,
-        test_data,
-        max_categories,
-        psi_contribution_percent,
-        threshold,
+    actual_series,
+    reference_series,
+    test_data,
+    max_categories,
+    psi_contribution_percent,
+    threshold,
 ):
     total_psi, output_data = _calculate_drift_psi(actual_series, reference_series, max_categories)
     passed = True if threshold is None else bool(total_psi <= threshold)
     main_drifting_modalities_bool = output_data["Psi"] > psi_contribution_percent * total_psi
     messages = _generate_message_modalities(main_drifting_modalities_bool, output_data, test_data)
     return messages, passed, total_psi
 
@@ -525,17 +544,23 @@
                 text=f"The {test_data} is drifting for the following modalities: {','.join(filtered_modalities)}",
             )
         ]
     return messages
 
 
 @test(name='Label drift (Chi-squared)')
-def test_drift_prediction_chi_square(model: BaseModel, actual_dataset: Dataset, reference_dataset: Dataset,
-                                     slicing_function: Optional[SlicingFunction] = None, max_categories: int = 10,
-                                     threshold: float = 0.05, chi_square_contribution_percent: float = 0.2):
+def test_drift_prediction_chi_square(
+    model: BaseModel,
+    actual_dataset: Dataset,
+    reference_dataset: Dataset,
+    slicing_function: Optional[SlicingFunction] = None,
+    max_categories: int = 10,
+    threshold: float = 0.05,
+    chi_square_contribution_percent: float = 0.2,
+):
     """
     Test if the Chi Square value between the reference and actual datasets is below the threshold
     for the classification labels predictions for a given slice
 
     Example : The test is passed when the  Chi Square value of classification labels prediction
     for females between reference and actual sets is below 0.05
 
@@ -594,33 +619,38 @@
         passed=passed,
         metric=p_value,
         messages=messages,
     )
 
 
 def _test_series_drift_chi(
-        actual_series,
-        reference_series,
-        test_data,
-        chi_square_contribution_percent,
-        max_categories,
-        threshold,
+    actual_series,
+    reference_series,
+    test_data,
+    chi_square_contribution_percent,
+    max_categories,
+    threshold,
 ):
     chi_square, p_value, output_data = _calculate_chi_square(actual_series, reference_series, max_categories)
     passed = bool(p_value > threshold)
     main_drifting_modalities_bool = output_data["Chi_square"] > chi_square_contribution_percent * chi_square
     messages = _generate_message_modalities(main_drifting_modalities_bool, output_data, test_data)
     return messages, p_value, passed
 
 
 @test(name='Classification Probability drift (Kolmogorov-Smirnov)', tags=['classification'])
 @validate_classification_label
-def test_drift_prediction_ks(model: BaseModel, actual_dataset: Dataset, reference_dataset: Dataset,
-                             slicing_function: Optional[SlicingFunction] = None, classification_label: Optional[str] = None,
-                             threshold: Optional[float] = None) -> TestResult:
+def test_drift_prediction_ks(
+    model: BaseModel,
+    actual_dataset: Dataset,
+    reference_dataset: Dataset,
+    slicing_function: Optional[SlicingFunction] = None,
+    classification_label: Optional[str] = None,
+    threshold: Optional[float] = None,
+) -> TestResult:
     """
     Test if the pvalue of the KS test for prediction between the reference and actual datasets for
      a given subpopulation is above the threshold
 
     Example : The test is passed when the pvalue of the KS test for the prediction for females
      between reference and actual dataset is higher than 0.05. It means that the KS test cannot be
      rejected at 5% level and that we cannot assume drift for this variable.
@@ -654,14 +684,21 @@
     if slicing_function:
         test_name = "test_drift_prediction_ks"
         actual_dataset = actual_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
         reference_dataset = reference_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
 
+    # Try to automatically cast `classification_label` to the right type
+    if classification_label is not None and isinstance(model.meta.classification_labels[0], numbers.Number):
+        try:
+            classification_label = int(classification_label)
+        except ValueError:
+            pass
+
     prediction_reference = (
         pd.Series(model.predict(reference_dataset).all_predictions[classification_label].values)
         if model.is_classification
         else pd.Series(model.predict(reference_dataset).prediction)
     )
     prediction_actual = (
         pd.Series(model.predict(actual_dataset).all_predictions[classification_label].values)
@@ -687,25 +724,30 @@
 def _generate_message_ks(passed, result, threshold, data_type):
     messages: Optional[List[TestMessage]] = None
     if not passed:
         messages = [
             TestMessage(
                 type=TestMessageLevel.ERROR,
                 text=f"The {data_type} is drifting (p-value is equal to {np.round(result.pvalue, 9)} "
-                     f"and is below the test risk level {threshold}) ",
+                f"and is below the test risk level {threshold}) ",
             )
         ]
     return messages
 
 
 @test(name='Classification Probability drift (Earth mover\'s distance)', tags=['classification'])
 @validate_classification_label
-def test_drift_prediction_earth_movers_distance(model: BaseModel, actual_dataset: Dataset, reference_dataset: Dataset,
-                                                slicing_function: Optional[SlicingFunction] = None,
-                                                classification_label: Optional[str] = None, threshold: float = 0.2) -> TestResult:
+def test_drift_prediction_earth_movers_distance(
+    model: BaseModel,
+    actual_dataset: Dataset,
+    reference_dataset: Dataset,
+    slicing_function: Optional[SlicingFunction] = None,
+    classification_label: Optional[str] = None,
+    threshold: float = 0.2,
+) -> TestResult:
     """
     Test if the Earth Mover’s Distance value between the reference and actual datasets is
     below the threshold for the classification labels predictions for classification
     model and prediction for regression models
 
     Example :
     Classification : The test is passed when the  Earth Mover’s Distance value of classification
@@ -738,14 +780,21 @@
     if slicing_function:
         test_name = "test_drift_prediction_earth_movers_distance"
         actual_dataset = actual_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=actual_dataset, dataset_name="actual_dataset", test_name=test_name)
         reference_dataset = reference_dataset.slice(slicing_function)
         check_slice_not_empty(sliced_dataset=reference_dataset, dataset_name="reference_dataset", test_name=test_name)
 
+    # Try to automatically cast `classification_label` to the right type
+    if classification_label is not None and isinstance(model.meta.classification_labels[0], numbers.Number):
+        try:
+            classification_label = int(classification_label)
+        except ValueError:
+            pass
+
     prediction_reference = (
         model.predict(reference_dataset).all_predictions[classification_label].values
         if model.is_classification
         else model.predict(reference_dataset).prediction
     )
     prediction_actual = (
         model.predict(actual_dataset).all_predictions[classification_label].values
@@ -759,15 +808,15 @@
     messages: Optional[typing.List[TestMessage]] = None
 
     if not passed:
         messages = [
             TestMessage(
                 type=TestMessageLevel.ERROR,
                 text=f"The prediction is drifting (metric is equal to {np.round(metric, 9)} "
-                     f"and is above the test risk level {threshold}) ",
+                f"and is above the test risk level {threshold}) ",
             )
         ]
 
     return TestResult(
         actual_slices_size=[len(actual_dataset)],
         reference_slices_size=[len(reference_dataset)],
         passed=bool(True if threshold is None else metric <= threshold),
```

### Comparing `giskard-2.0.0b2/giskard/testing/tests/metamorphic.py` & `giskard-2.0.0b3/giskard/testing/tests/metamorphic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/testing/tests/performance.py` & `giskard-2.0.0b3/giskard/testing/tests/performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,16 @@
     if len(model.meta.classification_labels) == 2:
         metric = roc_auc_score(dataset.df[dataset.target], model.predict(dataset).raw[:, 1])
     else:
         predictions = model.predict(dataset).all_predictions
         non_declared_categories = set(predictions.columns) - set(dataset.df[dataset.target].unique())
         assert not len(
             non_declared_categories
-        ), f'Predicted classes don\'t exist in the dataset "{dataset.target}" column: {non_declared_categories}'
+        ), f'Predicted classes don\'t exist in the dataset "{dataset.target}" column: {non_declared_categories}. ' \
+           'ROC AUC score is not defined in that case.'
 
         metric = roc_auc_score(dataset.df[dataset.target], predictions, multi_class="ovo")
 
     return TestResult(actual_slices_size=[len(dataset)], metric=metric, passed=bool(metric >= threshold))
 
 
 @test(name='F1', tags=['performance', 'classification', 'ground_truth'])
```

### Comparing `giskard-2.0.0b2/giskard/testing/tests/statistic.py` & `giskard-2.0.0b3/giskard/testing/tests/statistic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard/utils/analytics_collector.py` & `giskard-2.0.0b3/giskard/utils/analytics_collector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import hashlib
 import os
 import platform
+import time
 import uuid
+from dataclasses import dataclass
 from functools import wraps
+from queue import Queue
 from threading import Lock
-from typing import Dict, Optional
+from typing import Dict, Optional, Any
 
 import requests
 from mixpanel import Mixpanel
 
 from giskard.settings import settings
 from giskard.utils import fullname, threaded
 from giskard.utils.environment_detector import EnvironmentDetector
@@ -72,33 +75,57 @@
         "dataset_rows": dataset.df.shape[0],
         "dataset_cols": dataset.df.shape[1],
         "dataset_column_types": column_types,
         "dataset_column_dtypes": column_dtypes,
     }
 
 
+@dataclass
+class TelemetryMessage:
+    distinct_id: Any
+    event_name: Any
+    properties: Any
+    meta: Any
+
+
 class GiskardAnalyticsCollector:
     lock = Lock()
     ip: Optional[str]
     dev_mp_project_key = "4cca5fabca54f6df41ea500e33076c99"
     prod_mp_project_key = "2c3efacc6c26ffb991a782b476b8c620"
     server_info: Optional[Dict] = None
     mp: Mixpanel
     giskard_version: Optional[str]
     environment: str
+    queue: Queue[TelemetryMessage] = Queue()
 
     def __init__(self) -> None:
         self.is_enabled = not settings.disable_analytics
         self.giskard_version = None
         self.ip = None
         self.environment = EnvironmentDetector().detect()
         if self.is_enabled:
             self.mp = self.configure_mixpanel()
             self.distinct_user_id = GiskardAnalyticsCollector.machine_based_user_id()
 
+    @threaded
+    def _consume(self):
+        while True:
+            event = self.queue.get(block=True)
+            self.mp.track(
+                distinct_id=self.distinct_user_id,
+                event_name=event.event_name,
+                properties=dict(event.merged_props),
+                meta=event.meta
+            )
+            time.sleep(1)
+
+    def _submit(self, msg):
+        self.queue.put(msg, block=True)
+
     @staticmethod
     @analytics_method
     def configure_mixpanel() -> Mixpanel:
         is_dev_mode = os.environ.get("GISKARD_DEV_MODE", "n").lower() in ["yes", "true", "1"]
 
         return Mixpanel(
             GiskardAnalyticsCollector.dev_mp_project_key
@@ -135,23 +162,23 @@
                 "environment": self.environment
             }
             if properties is not None:
                 merged_props = {**merged_props, **properties}
             if self.server_info is not None:
                 merged_props = {**merged_props, **self.server_info}
 
-            self.mp.track(
+            self._submit(TelemetryMessage(
                 distinct_id=self.distinct_user_id, event_name=event_name, properties=dict(merged_props), meta=meta
-            )
+            ))
 
     @staticmethod
     def machine_based_user_id():
         try:
             return anonymize(str(uuid.getnode()) + os.getlogin())
-        except BaseException:  # noqa
+        except BaseException:  # noqa NOSONAR
             # https://bugs.python.org/issue40821
             return "unknown"
 
     def initialize_geo(self):
         """
         Query a user's IP address to convert it to an aggregated telemetry:
             - city
@@ -159,13 +186,13 @@
             - country
         IP address itself **isn't stored** by in the telemetry data
         """
         with GiskardAnalyticsCollector.lock:
             if self.ip:
                 return
             try:
-                self.ip = requests.get('http://ip-api.com/json').json().get('query', 'unknown')
-            except:  # noqa
+                self.ip = requests.get('http://ip-api.com/json').json().get('query', 'unknown')  # noqa NOSONAR
+            except:  # noqa NOSONAR
                 self.ip = "unknown"
 
 
 analytics = GiskardAnalyticsCollector()
```

### Comparing `giskard-2.0.0b2/giskard/utils/environment_detector.py` & `giskard-2.0.0b3/giskard/utils/environment_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard.egg-info/SOURCES.txt` & `giskard-2.0.0b3/giskard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/giskard.egg-info/requires.txt` & `giskard-2.0.0b3/giskard.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/pyproject.toml` & `giskard-2.0.0b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,19 @@
 name = "torch"
 
 
 
 [tool.pdm.scripts]
 proto = "setup.py grpc"
 # add "-n auto" to the pytest command to parallelize the execution
-test.cmd = "pytest -c pyproject.toml --cov=giskard --cov-report=xml tests"
+test.cmd = "pytest -c pyproject.toml tests --cov=giskard --cov-report=xml --disable-warnings"
 test.env = { GSK_DISABLE_ANALYTICS = "True"}
+# for some reason github runners don't work when calling 'pdm test -m "not slow"'
+test-fast.cmd = "pytest -n auto -m 'not slow' -c pyproject.toml tests --cov=giskard --cov-report=xml --disable-warnings"
+test-fast.env = { GSK_DISABLE_ANALYTICS = "True"}
 lint = "flake8 giskard tests"
 doc = "python -m sphinx_autobuild docs docs/_build/html"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "typing-extensions>=4.5.0",
     "black>=23.3.0",
@@ -86,23 +89,30 @@
 [tool.setuptools.package-data]
 giskard = ["**/*.html", "**/*.css", "**/*.js", "**/*.json", "**/*titanic.csv"]
 
 [project.scripts]
 giskard = "giskard.cli:cli"
 
 [project.urls]
-repository = "https://github.com/Giskard-AI/giskard"
-homepage = "https://giskard-ai"
+"Homepage" = "https://giskard.ai"
+"Source Code" = "https://github.com/Giskard-AI/giskard"
+"Bug Tracker" = "https://github.com/Giskard-AI/giskard/issues"
+"Documentation" = "https://docs.giskard.ai/"
+"Discord" = "https://discord.gg/ABvfpbu69R"
+"Linkedin" = "https://www.linkedin.com/company/giskard-ai"
+"Mastodon" = "https://fosstodon.org/@Giskard"
+"Twitter" = "https://twitter.com/giskard_ai"
+
 
 [project]
 name = "giskard"
 readme = "README.md"
 license = { text = "Apache Software License 2.0" }
-version = "2.0.0b2"
-description = "Inspect your AI models visually, find bugs, give feedback 🕵️‍♀️ 💬"
+version = "2.0.0b3"
+description = "The testing framework dedicated to ML models, from tabular to LLMs"
 authors = [
     { name = "Giskard AI", email = "hello@giskard.ai" },
 ]
 keywords = [
     "Artificial Intelligence",
     "Machine Learning",
     "Quality",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `giskard-2.0.0b2/setup.py` & `giskard-2.0.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_custom_model.py` & `giskard-2.0.0b3/tests/test_custom_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from tests.utils import MockedClient
 
 
 def test_custom_model(linear_regression_diabetes: BaseModel):
     with MockedClient() as (client, mr):
         class MyModel(WrapperModel):
             @classmethod
-            def load_wrapped_model(cls, local_dir):
+            def load_model(cls, local_dir):
                 pass
 
             def save_model(self, local_path: Union[str, Path]) -> None:
                 pass
 
             def model_predict(self, df):
                 pass
```

### Comparing `giskard-2.0.0b2/tests/test_data_drift.py` & `giskard-2.0.0b3/tests/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_data_processing_pipeline.py` & `giskard-2.0.0b3/tests/test_data_processing_pipeline.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_dataset.py` & `giskard-2.0.0b3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_metamorphic_direction.py` & `giskard-2.0.0b3/tests/test_metamorphic_direction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_metamorphic_invariance.py` & `giskard-2.0.0b3/tests/test_metamorphic_invariance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_model.py` & `giskard-2.0.0b3/tests/test_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import tempfile
-import time
 from pathlib import Path
-from time import perf_counter
 
 import numpy as np
 import pytest
 
 from giskard import Model
 from giskard.core.core import SupportedModelTypes
 
@@ -32,37 +30,29 @@
     assert (res.probabilities >= 0).all() and (res.probabilities <= 1).all()
     assert np.array_equal(
         german_credit_catboost.predict(german_credit_test_data).probabilities,
         original_predictions,
     ), "Predictions are not the same after changing features order"
 
 
-def test_prediction_cache_loaded_model(linear_regression_diabetes, linear_regression_diabetes_raw, diabetes_dataset, request):
+def test_prediction_cache_loaded_model(linear_regression_diabetes, linear_regression_diabetes_raw, diabetes_dataset):
     nb_of_prediction_calls = [0]
 
     def prediction_fn(df):
-        # simulate slowish prediction
-        time.sleep(1)
         nb_of_prediction_calls[0] += 1
         return np.ones(df.shape[0])
 
     with tempfile.TemporaryDirectory(prefix="cache_dir-") as cache_dir, \
             tempfile.TemporaryDirectory(prefix="model_dir-") as model_dir:
         model = Model(prediction_fn,
                       model_type=SupportedModelTypes.REGRESSION,
                       feature_names=linear_regression_diabetes.meta.feature_names,
                       prediction_cache_dir=Path(cache_dir))
 
-        start = perf_counter()
         predictions = model.predict(diabetes_dataset)
-        first_elapsed = perf_counter() - start
         model.save(model_dir)
 
         loaded_model = Model.load(model_dir, prediction_cache_dir=Path(cache_dir))
-        start = perf_counter()
         second_predictions = loaded_model.predict(diabetes_dataset)
-        second_elapsed = perf_counter() - start
 
         assert np.all(np.equal(predictions.raw, second_predictions.raw))
         assert nb_of_prediction_calls[0] == 1
-        # prediction from cache takes at most 5% of the original time
-        assert second_elapsed / first_elapsed < 0.05
```

### Comparing `giskard-2.0.0b2/tests/test_model_auto_inference.py` & `giskard-2.0.0b3/tests/test_model_auto_inference.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_model_explanation.py` & `giskard-2.0.0b3/tests/test_model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_model_postprocess.py` & `giskard-2.0.0b3/tests/test_model_postprocess.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_performance.py` & `giskard-2.0.0b3/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_programmatic.py` & `giskard-2.0.0b3/tests/test_programmatic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_project_uploads.py` & `giskard-2.0.0b3/tests/test_project_uploads.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_statistical.py` & `giskard-2.0.0b3/tests/test_statistical.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b2/tests/test_upload.py` & `giskard-2.0.0b3/tests/test_upload.py`

 * *Files identical despite different names*

