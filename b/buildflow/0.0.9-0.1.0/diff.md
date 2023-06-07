# Comparing `tmp/buildflow-0.0.9.tar.gz` & `tmp/buildflow-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildflow-0.0.9.tar", last modified: Thu Mar 16 21:11:25 2023, max compression
+gzip compressed data, was "buildflow-0.1.0.tar", last modified: Wed Jun  7 20:41:11 2023, max compression
```

## Comparing `buildflow-0.0.9.tar` & `buildflow-0.1.0.tar`

### file list

```diff
@@ -1,79 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.690326 buildflow-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-03-16 21:11:13.000000 buildflow-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-03-16 21:11:25.690326 buildflow-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-16 21:11:13.000000 buildflow-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.678326 buildflow-0.0.9/buildflow/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.678326 buildflow-0.0.9/buildflow/api/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.682325 buildflow-0.0.9/buildflow/api/_vision/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/api/_vision/process_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/api/_vision/process_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/api/_vision/process_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/api/_vision/processor_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/api/_vision/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/api/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/api/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/api/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.682325 buildflow-0.0.9/buildflow/migration/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/migration/beam_migrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.682325 buildflow-0.0.9/buildflow/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.686326 buildflow-0.0.9/buildflow/runtime/ray_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18777 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/bigquery_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/bigquery_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/duckdb_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/duckdb_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/empty_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/empty_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/file_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/gcs_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/gcs_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/pubsub_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/pubsub_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/pubsub_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/redis_stream_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/redis_stream_io_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.686326 buildflow-0.0.9/buildflow/runtime/ray_io/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/schemas/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/ray_io/schemas/bigquery_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/runtime/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.690326 buildflow-0.0.9/buildflow/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/samples/bigquery_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/samples/class_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/samples/csv_bigquery_walkthrough.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/samples/decorator_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/samples/local_pubsub_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/samples/local_pubsub_walkthrough.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/samples/pubsub_walkthrough.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-16 21:11:13.000000 buildflow-0.0.9/buildflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.678326 buildflow-0.0.9/buildflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-03-16 21:11:25.000000 buildflow-0.0.9/buildflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-16 21:11:25.000000 buildflow-0.0.9/buildflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 21:11:25.000000 buildflow-0.0.9/buildflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-16 21:11:25.000000 buildflow-0.0.9/buildflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-16 21:11:25.000000 buildflow-0.0.9/buildflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.678326 buildflow-0.0.9/integration_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.690326 buildflow-0.0.9/integration_tests/pubsub_to_local_parquet/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-16 21:11:13.000000 buildflow-0.0.9/integration_tests/pubsub_to_local_parquet/pubsub_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-16 21:11:13.000000 buildflow-0.0.9/integration_tests/pubsub_to_local_parquet/pubsub_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-16 21:11:13.000000 buildflow-0.0.9/integration_tests/pubsub_to_local_parquet/pubsub_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.690326 buildflow-0.0.9/integration_tests/pubsub_to_pubsub/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-16 21:11:13.000000 buildflow-0.0.9/integration_tests/pubsub_to_pubsub/pubsub_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-16 21:11:13.000000 buildflow-0.0.9/integration_tests/pubsub_to_pubsub/pubsub_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-16 21:11:13.000000 buildflow-0.0.9/integration_tests/pubsub_to_pubsub/pubsub_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:11:25.690326 buildflow-0.0.9/integration_tests/pubsub_to_pubsub_multi_output/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-16 21:11:13.000000 buildflow-0.0.9/integration_tests/pubsub_to_pubsub_multi_output/pubsub_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-16 21:11:13.000000 buildflow-0.0.9/integration_tests/pubsub_to_pubsub_multi_output/pubsub_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-16 21:11:13.000000 buildflow-0.0.9/integration_tests/pubsub_to_pubsub_multi_output/pubsub_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-03-16 21:11:13.000000 buildflow-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 21:11:25.690326 buildflow-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.332065 buildflow-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-07 20:41:00.000000 buildflow-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-07 20:41:11.332065 buildflow-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-07 20:41:00.000000 buildflow-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.312064 buildflow-0.1.0/buildflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.316065 buildflow-0.1.0/buildflow/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/depends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/infra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.316065 buildflow-0.1.0/buildflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.316065 buildflow-0.1.0/buildflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.316065 buildflow-0.1.0/buildflow/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/grid/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/infra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/infra/actors/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/infra/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/infra/actors/pulumi_infra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/infra/actors/setup_infra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/infra/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/node/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/node/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/processor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.324065 buildflow-0.1.0/buildflow/core/runtime/actors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/pull_process_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/pull_process_push_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/runtime_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/autoscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/autoscale_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.324065 buildflow-0.1.0/buildflow/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.324065 buildflow-0.1.0/buildflow/io/depends/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/depends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/depends/depends.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.324065 buildflow-0.1.0/buildflow/io/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.328065 buildflow-0.1.0/buildflow/io/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/file_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/file_provider_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.328065 buildflow-0.1.0/buildflow/io/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/bigquery_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/gcp_pub_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/gcp_pub_sub_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/gcs_file_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/gcs_file_stream_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.328065 buildflow-0.1.0/buildflow/io/providers/gcp/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/utils/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/utils/setup_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/pulsing_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/pulsing_provider_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.328065 buildflow-0.1.0/buildflow/io/providers/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/schemas/bigquery_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/schemas/bigquery_schemas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/schemas/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/schemas/converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.332065 buildflow-0.1.0/buildflow/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/migration/beam_migrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.332065 buildflow-0.1.0/buildflow/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/samples/csv_bigquery_walkthrough.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/samples/pubsub_walkthrough.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.312064 buildflow-0.1.0/buildflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.312064 buildflow-0.1.0/integration_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.332065 buildflow-0.1.0/integration_tests/pubsub_to_pubsub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-07 20:41:00.000000 buildflow-0.1.0/integration_tests/pubsub_to_pubsub/pubsub_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-07 20:41:00.000000 buildflow-0.1.0/integration_tests/pubsub_to_pubsub/pubsub_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-07 20:41:00.000000 buildflow-0.1.0/integration_tests/pubsub_to_pubsub/pubsub_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-07 20:41:00.000000 buildflow-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:41:11.332065 buildflow-0.1.0/setup.cfg
```

### Comparing `buildflow-0.0.9/LICENSE` & `buildflow-0.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Apache License
 ==============
 
-_Version 2.0, January 2004_  
+_Version 2.0, January 2004_
 _&lt;<http://www.apache.org/licenses/>&gt;_
 
 ### Terms and Conditions for use, reproduction, and distribution
 
 #### 1. Definitions
 
 “License” shall mean the terms and conditions for use, reproduction, and
@@ -176,19 +176,19 @@
 identifying information. (Don't include the brackets!) The text should be
 enclosed in the appropriate comment syntax for the file format. We also
 recommend that a file or class name and description of purpose be included on
 the same “printed page” as the copyright notice for easier identification within
 third-party archives.
 
     Copyright [yyyy] [name of copyright owner]
-    
+
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
-    
+
       http://www.apache.org/licenses/LICENSE-2.0
-    
+
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
```

### Comparing `buildflow-0.0.9/PKG-INFO` & `buildflow-0.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,27 @@
-Metadata-Version: 2.1
-Name: buildflow
-Version: 0.0.9
-Summary: buildflow is a unified **batch** and **streaming** framework that turns any python function into a scalable data pipeline that can read from our supported IO resources.
-Author-email: Caleb Van Dyke <caleb@launchflow.com>, Josh Tanke <josh@launchflow.com>
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # BuildFlow
 
 ![CI](https://github.com/launchflow/buildflow/actions/workflows/python_ci.yaml/badge.svg)
+![GCP Tests](https://github.com/launchflow/buildflow/actions/workflows/gcp_integration.yaml/badge.svg)
 [![Discord Shield](https://discordapp.com/api/guilds/1082821064180117575/widget.png?style=shield)](https://discordapp.com/invite/wz7fjHyrCA)
 
 **BuildFlow**, is an open source framework that lets you build a data pipeline by simply attaching a decorator to a Python function. All you need to do is describe where your input is coming from and where your output should be written, and BuildFlow handles the rest. No configuration outside of the code is required.
 
-
 Key Features:
 
 - Unified **batch** and **streaming** [Processor API](https://www.buildflow.dev/docs/processors/overview)
 - Production-grade [IO connectors](https://www.buildflow.dev/docs/io-connectors/overview) for popular cloud services & storage systems
 - IO templates for common data pipelines (e.g. [file upload notifications](https://www.buildflow.dev/docs/io-connectors/gcs_notifications))
 - Automatic [resource creation / management](https://www.buildflow.dev/docs/resource-creation) for popular cloud resources
 - [Schema validation](https://www.buildflow.dev/docs/schema-validation) powered by Python dataclasses and type hints
 - Automatic parallelism powered by [Ray](https://ray.io)
 
 ## Quick Links
 
-- **Docs**: https://www.buildflow.dev/docs/intro
+- **Docs**: https://www.buildflow.dev/docs
 - **Walkthroughs**: https://www.buildflow.dev/docs/category/walk-throughs
 - **Discord**: https://discordapp.com/invite/wz7fjHyrCA
 
 ## Quickstart
 
 ### Install
 
@@ -61,15 +47,26 @@
 def stream_processor(pubsub_message):
   # TODO(developer): Implement processing logic
   ...
   # The output is sent to the sink provider
   return pubsub_message
 
 # Start the processor(s)
-flow.run(num_replicas=4)
+flow.run().output()
 ```
 
 For a more in depth tutorial see our [walkthroughs](https://www.buildflow.dev/docs/category/walk-throughs).
 
 ## Windows Users
 
 Our runtime is built on [Ray](https://ray.io/), where Windows support is currently in beta. See the [Ray docs](https://docs.ray.io/en/latest/ray-overview/installation.html#windows-support) for more info.
+
+## Code Health Checks
+
+We use [black](https://github.com/psf/black) and [ruff](https://github.com/charliermarsh/ruff) with [pre-commit](https://pre-commit.com/) hooks to perform health checks.
+To setup these locally:
+
+- Clone the repo
+- Install the `dev` dependencies like `python -m pip install .[dev]
+- Check if pre-commit is installed correctly by running `pre-commit --version`
+- Setup pre-commit to run before every commit on staged changes by running `pre-commit install`
+- Pre-commit can also be ran manually as `pre-commit run --all-files`
```

### Comparing `buildflow-0.0.9/buildflow/api/processor.py` & `buildflow-0.1.0/buildflow/api/processor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from typing import Any, Iterable
 
-from buildflow.api.io import SourceType, SinkType
+from buildflow.api.io import SinkType, SourceType
+
+
+ProcessorID = str
 
 
 class ProcessorAPI:
+    processor_id: ProcessorID
 
     # This lifecycle method defines the input reference for the processor.
-    def source(self) -> SourceType:
-        raise NotImplementedError('source not implemented')
+    @classmethod
+    def source(cls) -> SourceType:
+        raise NotImplementedError("source not implemented")
 
     # This lifecycle method defines the output reference for the processor.
-    def sink(self) -> SinkType:
-        raise NotImplementedError('sink not implemented')
+    @classmethod
+    def sink(cls) -> SinkType:
+        raise NotImplementedError("sink not implemented")
 
     # You can also define multiple outputs.
+    @classmethod
     def sinks(self) -> Iterable[SinkType]:
-        raise NotImplementedError('sinks not implemented')
+        raise NotImplementedError("sinks not implemented")
 
-    # This lifecycle method initializes any shared state.
+    # This lifecycle method is called once per replica.
     def setup(self):
-        raise NotImplementedError('setup not implemented')
+        raise NotImplementedError("setup not implemented")
 
     # This lifecycle method is called once per payload.
-    def process(self, payload: Any):
-        raise NotImplementedError('process not implemented')
-
-    # Returns the arg spec of the process method.
-    def processor_arg_spec(self):
-        raise NotImplementedError('process not implemented')
+    def process(self, payload: Any, **kwargs):
+        raise NotImplementedError("process not implemented")
```

### Comparing `buildflow-0.0.9/buildflow/runtime/ray_io/gcs_io.py` & `buildflow-0.1.0/buildflow/io/providers/gcp/gcs_file_stream.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,136 +1,163 @@
-import dataclasses
-import logging
-from typing import Any, Dict, List, Optional
+from dataclasses import dataclass
+from typing import Any, Callable, Dict, List, Optional, Type
 
 from google.api_core import exceptions
-from google.cloud import storage
+import pulumi
+import pulumi_gcp
 
-from buildflow.api import io
-from buildflow.runtime.ray_io import pubsub_io
-from buildflow.runtime.ray_io import pubsub_utils
+from buildflow.io.providers import (
+    PullProvider,
+    PulumiProvider,
+)
+from buildflow.io.providers.base import PullResponse, PulumiResources
+from buildflow.io.providers.gcp import gcp_pub_sub
+from buildflow.io.providers.gcp.utils import clients as gcp_clients
+from buildflow.io.providers.schemas import converters
 
 
-@dataclasses.dataclass
+@dataclass
 class GCSFileEvent:
     # Metadata about that action taken.
     metadata: Dict[str, Any]
+    billing_project: str
 
     @property
     def blob(self) -> bytes:
-        if self.metadata['eventType'] == 'OBJECT_DELETE':
-            raise ValueError('Can\'t fetch blob for `OBJECT_DELETE` event.')
-        client = storage.Client()
-        bucket = client.bucket(bucket_name=self.metadata['bucketId'])
-        blob = bucket.get_blob(self.metadata['objectId'])
+        if self.metadata["eventType"] == "OBJECT_DELETE":
+            raise ValueError("Can't fetch blob for `OBJECT_DELETE` event.")
+        client = gcp_clients.get_storage_client(self.billing_project)
+        bucket = client.bucket(bucket_name=self.metadata["bucketId"])
+        blob = bucket.get_blob(self.metadata["objectId"])
         return blob.download_as_bytes()
 
 
-@dataclasses.dataclass
-class GCSFileNotifications(io.Source):
-    bucket_name: str
-    project_id: str
-    # The pubsub topic that is configured to point at the bucket. If not set
-    # we will create one.
-    pubsub_topic: str = ''
-    # The pubsub subscription that is configure to point at the bucket. If not
-    # set we will create one.
-    pubsub_subscription: str = ''
-    # The event types that should trigger the stream. This is only used if we
-    # are attaching a new notification listener to your bucket. Defaults to
-    # only new uploads. If set to None will listen to all uploads.
-    event_types: Optional[List[str]] = ('OBJECT_FINALIZE', )
-
-    # Internal values to track if the user provide the topics or we are
-    # creating them. If the user is providing them we will assume things are
-    # configured correctly.
-    _managed_subscriber = True
-    _managed_publisher = True
-
-    def __post_init__(self):
-        if not self.pubsub_topic:
-            self.pubsub_topic = f'projects/{self.project_id}/topics/{self.bucket_name}_notifications'  # noqa: E501
-            logging.info(
-                f'No pubsub topic provided. Defaulting to {self.pubsub_topic}.'
-            )
-        else:
-            self._managed_publisher = False
-        if not self.pubsub_subscription:
-            self.pubsub_subscription = f'projects/{self.project_id}/subscriptions/{self.bucket_name}_subscriber'  # noqa: E501
-            logging.info('No pubsub subscription provided. Defaulting to '
-                         f'{self.pubsub_subscription}.')
-        else:
-            self._managed_subscriber = False
+class GCSFileStreamProvider(PullProvider, PulumiProvider):
+    def __init__(
+        self,
+        *,
+        bucket_name: str,
+        project_id: str,
+        event_types: Optional[List[str]] = ("OBJECT_FINALIZE",),
+        force_destroy: bool = False,
+    ):
+        """
+        Args:
+            bucket_name: The name of the bucket to stream from.
+            project_id: The project id that the bucket is in.
+            pubsub_topic: The pubsub topic that is configured to point at the bucket.
+                If not set we will create one.
+            pubsub_subscription: The pubsub subscription that is configure to point at
+                the bucket. If not set we will create one.
+            event_types: The event types that should trigger the stream. This is only
+                used if we are attaching a new notification listener to your bucket.
+                Defaults to only new uploads. If set to None will listen to all events.
+            force_destroy: If set to True will delete contents of the bucket on destroy.
+
+        """
+        self.bucket_name = bucket_name
+        self.project_id = project_id
+        self.event_types = list(event_types)
+        self.force_destroy = force_destroy
+        self._managed_publisher = True
+        self._managed_subscriber = True
+        self._topic_name = f"{self.bucket_name}_notifications"
+        self._subscription_name = f"{self.bucket_name}_subscriber"
+        self._pubsub_topic = f"projects/{self.project_id}/topics/{self._topic_name}"
+        self.subscription_provider = gcp_pub_sub.GCPPubSubSubscriptionProvider(
+            project_id=self.project_id,
+            topic_id=self._pubsub_topic,
+            subscription_name=self._subscription_name,
+            batch_size=1000,
+            include_attributes=True,
+        )
+
+    async def pull(self) -> PullResponse:
+        pull_response = await self.subscription_provider.pull()
+        payload = [
+            GCSFileEvent(metadata=payload.attributes, billing_project=self.project_id)
+            for payload in pull_response.payload
+        ]
+        return PullResponse(payload=payload, ack_info=pull_response.ack_info)
+
+    # TODO: This should not be Optional (goes against Pullable base class)
+    async def backlog(self) -> Optional[int]:
+        return await self.subscription_provider.backlog()
+
+    async def ack(self, ack_info, success: bool):
+        return await self.subscription_provider.ack(ack_info, success)
+
+    def pull_converter(self, user_defined_type: Type) -> Callable[[Any], Any]:
+        if (
+            not issubclass(user_defined_type, GCSFileEvent)
+            and user_defined_type is not None
+        ):
+            raise ValueError("Input type for GCS file stream should be: `GCSFileEvent`")
+        return converters.identity()
+
+    def pulumi(self, type_: Optional[Type]) -> PulumiResources:
+        # TODO: should support additional parameters for all resource creation.
+        # probably most importantly the bucket (location, ttl, etc..)
+        resources = []
+        exports = {}
+        topic_resource = pulumi_gcp.pubsub.Topic(
+            self._topic_name, name=self._topic_name, project=self.project_id
+        )
+
+        resources.append(topic_resource)
+        exports["gcp.pubsub.topic.name"] = topic_resource.name
+
+        gcs_account = pulumi_gcp.storage.get_project_service_account(
+            project=self.project_id, user_project=self.project_id
+        )
+        binding = pulumi_gcp.pubsub.TopicIAMBinding(
+            "binding",
+            opts=pulumi.ResourceOptions(depends_on=[topic_resource]),
+            topic=self._pubsub_topic,
+            role="roles/pubsub.publisher",
+            members=[f"serviceAccount:{gcs_account.email_address}"],
+        )
+        resources.append(binding)
+
+        subscription_resource = pulumi_gcp.pubsub.Subscription(
+            self._subscription_name,
+            opts=pulumi.ResourceOptions(depends_on=[topic_resource]),
+            name=self._subscription_name,
+            topic=self._pubsub_topic,
+            project=self.project_id,
+            ack_deadline_seconds=10 * 60,
+            message_retention_duration="1200s",
+        )
+
+        resources.append(subscription_resource)
+        exports["gcp.pubsub.subscription.name"] = subscription_resource.name
 
-    def setup(self):
+        exports["gcp.pubsub.subscription.name"] = subscription_resource.name
 
-        storage_client = storage.Client()
-        bucket = None
+        notification_depends = [topic_resource, binding]
+
+        # First check if the bucket exists.
         try:
-            bucket = storage_client.get_bucket(self.bucket_name)
-        except exceptions.NotFound:
-            print(f'bucket {self.bucket_name} not found attempting to create')
-            try:
-                print(f'Creating bucket: {self.bucket_name}')
-                bucket = storage_client.create_bucket(self.bucket_name,
-                                                      project=self.project_id)
-            except exceptions.PermissionDenied:
-                raise ValueError(
-                    f'Failed to create bucket: {self.bucket_name}. Please '
-                    'ensure you have permission to read the existing bucket '
-                    'or permission to create a new bucket if needed.')
-
-        if self._managed_subscriber:
-            gcs_notify_sa = (
-                f'serviceAccount:service-{bucket.project_number}@gs-project-accounts.iam.gserviceaccount.com'  # noqa: E501
+            gcp_clients.get_storage_client(self.project_id).get_bucket(self.bucket_name)
+        except (exceptions.Forbidden, exceptions.NotFound):
+            bucket = pulumi_gcp.storage.Bucket(
+                self.bucket_name,
+                name=self.bucket_name,
+                location="US",
+                project=self.project_id,
+                force_destroy=self.force_destroy,
             )
-            pubsub_utils.maybe_create_subscription(
-                self.pubsub_subscription,
-                self.pubsub_topic,
-                publisher_members=[gcs_notify_sa])
-        if self._managed_publisher:
-            notification_found = False
-            try:
-                _, _, _, topic_name = self.pubsub_topic.split('/')
-                # gotcha 1: have to list through notifications to get the topic
-                notifications = bucket.list_notifications()
-                for notification in notifications:
-                    if (notification.topic_name == topic_name
-                            and notification.bucket.name == self.bucket_name):
-                        notification_found = True
-                        break
-
-            except exceptions.PermissionDenied:
-                raise ValueError(
-                    'Failed to create bucket notification for bucket: '
-                    f'{self.bucket_name}. Please ensure you have permission '
-                    'to modify the bucket.')
-            if not notification_found:
-                print(f'bucket notification for bucket {self.bucket_name} not '
-                      'found attempting to create')
-                try:
-                    print(
-                        f'Creating notification for bucket {self.bucket_name}')
-                    _, project, _, topic = self.pubsub_topic.split('/')
-                    # gotcha 2: you cant pass the full topic path
-                    bucket.notification(topic_name=topic,
-                                        topic_project=project,
-                                        event_types=self.event_types).create()
-                except exceptions.PermissionDenied:
-                    raise ValueError(
-                        'Failed to create bucket notification for bucket: '
-                        f'{self.bucket_name}. Please ensure you have '
-                        'permission to modify the bucket.')
-
-    def preprocess(self, message: pubsub_io.PubsubMessage) -> GCSFileEvent:
-        return GCSFileEvent(metadata=message.attributes)
-
-    def actor(self, ray_sinks):
-        return pubsub_io.PubSubSourceActor.remote(
-            ray_sinks,
-            pubsub_io.PubSubSource(self.pubsub_subscription,
-                                   self.pubsub_topic,
-                                   include_attributes=True))
-
-    @classmethod
-    def is_streaming(cls) -> bool:
-        return True
+            resources.append(bucket)
+            exports["gcp.storage.bucket.name"] = self.bucket_name
+            notification_depends.append(bucket)
+
+        notification = pulumi_gcp.storage.Notification(
+            f"{self.bucket_name}_notification",
+            opts=pulumi.ResourceOptions(depends_on=notification_depends),
+            payload_format="JSON_API_V1",
+            bucket=self.bucket_name,
+            event_types=self.event_types,
+            topic=self._pubsub_topic,
+        )
+
+        resources.append(notification)
+        return PulumiResources(resources=resources, exports=exports)
```

### Comparing `buildflow-0.0.9/buildflow/runtime/ray_io/pubsub_utils.py` & `buildflow-0.1.0/buildflow/io/providers/gcp/utils/setup_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,89 @@
 """Utils for working with pubsub."""
 
+import logging
 from typing import List
 
 from google.api_core import exceptions
-from google.iam.v1 import iam_policy_pb2
-from google.iam.v1 import policy_pb2
-from google.cloud import pubsub
+from google.iam.v1 import iam_policy_pb2, policy_pb2
 
+from buildflow.io.providers.gcp.utils import clients
 
-def maybe_create_topic(pubsub_topic: str, publisher_members: List[str] = []):
-    publisher_client = pubsub.PublisherClient()
+
+def maybe_create_topic(
+    *, pubsub_topic: str, billing_project: str, publisher_members: List[str] = []
+):
+    publisher_client = clients.get_publisher_client(billing_project)
     try:
         publisher_client.get_topic(topic=pubsub_topic)
     except exceptions.NotFound:
-        print(f'topic {pubsub_topic} not found attempting to create')
+        logging.info(f"topic {pubsub_topic} not found attempting to create")
         try:
-            print(f'Creating topic: {pubsub_topic}')
+            logging.info(f"Creating topic: {pubsub_topic}")
             topic = publisher_client.create_topic(name=pubsub_topic)
             if publisher_members:
                 iam_policy = publisher_client.get_iam_policy(
-                    request=iam_policy_pb2.GetIamPolicyRequest(
-                        resource=topic.name))
+                    request=iam_policy_pb2.GetIamPolicyRequest(resource=topic.name)
+                )
                 added_publisher = False
                 for binding in iam_policy.bindings:
-                    if binding.role == 'roles/pubsub.publisher':
+                    if binding.role == "roles/pubsub.publisher":
                         binding.members.extend(publisher_members)
                         added_publisher = True
                 if not added_publisher:
                     iam_policy.bindings.append(
-                        policy_pb2.Binding(role='roles/pubsub.publisher',
-                                           members=publisher_members))
+                        policy_pb2.Binding(
+                            role="roles/pubsub.publisher", members=publisher_members
+                        )
+                    )
                 publisher_client.set_iam_policy(
                     request=iam_policy_pb2.SetIamPolicyRequest(
-                        resource=topic.name, policy=iam_policy))
+                        resource=topic.name, policy=iam_policy
+                    )
+                )
         except exceptions.PermissionDenied:
             raise ValueError(
-                f'Failed to create topic: {pubsub_topic}. Please '
-                'ensure you have permission to read the existing topic or '
-                'permission to create a new topic if needed.')
+                f"Failed to create topic: {pubsub_topic}. Please "
+                "ensure you have permission to read the existing topic or "
+                "permission to create a new topic if needed."
+            )
 
 
-def maybe_create_subscription(pubsub_subscription: str,
-                              pubsub_topic: str,
-                              publisher_members: List[str] = []):
-    subscriber_client = pubsub.SubscriberClient()
+def maybe_create_subscription(
+    *,
+    pubsub_subscription: str,
+    pubsub_topic: str,
+    billing_project: str,
+    publisher_members: List[str] = [],
+):
+    subscriber_client = clients.get_subscriber_client(billing_project)
     try:
         subscriber_client.get_subscription(subscription=pubsub_subscription)
     except exceptions.NotFound:
         if not pubsub_topic:
             raise ValueError(
-                f'subscription: {pubsub_subscription} was not found, '
-                'please provide the topic so we can create the '
-                'subscriber or ensure you have read access to the '
-                'subscribe.')
-        maybe_create_topic(pubsub_topic, publisher_members)
+                f"subscription: {pubsub_subscription} was not found, "
+                "please provide the topic so we can create the "
+                "subscriber or ensure you have read access to the "
+                "subscribe."
+            )
+        maybe_create_topic(
+            pubsub_topic=pubsub_topic,
+            publisher_members=publisher_members,
+            billing_project=billing_project,
+        )
         try:
-            print(f'Creating subscription: {pubsub_subscription}')
-            subscriber_client.create_subscription(name=pubsub_subscription,
-                                                  topic=pubsub_topic,
-                                                  # TODO: we should make this
-                                                  # configurable.
-                                                  ack_deadline_seconds=600)
+            logging.info(f"Creating subscription: {pubsub_subscription}")
+            subscriber_client.create_subscription(
+                name=pubsub_subscription,
+                topic=pubsub_topic,
+                # TODO: we should make this
+                # configurable.
+                ack_deadline_seconds=600,
+            )
         except exceptions.PermissionDenied:
             raise ValueError(
-                f'Failed to create subscription: {pubsub_subscription}. '
-                'Please ensure you have permission to read the '
-                'existing subscription or permission to create a new '
-                'subscription if needed.')
+                f"Failed to create subscription: {pubsub_subscription}. "
+                "Please ensure you have permission to read the "
+                "existing subscription or permission to create a new "
+                "subscription if needed."
+            )
```

### Comparing `buildflow-0.0.9/buildflow/runtime/ray_io/schemas/bigquery_test.py` & `buildflow-0.1.0/buildflow/io/providers/schemas/bigquery_schemas_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,173 +2,160 @@
 import dataclasses
 from datetime import date, datetime, time
 from typing import Optional, List, Union
 import unittest
 
 from google.cloud import bigquery
 
-from buildflow.runtime.ray_io.schemas import bigquery as bq_schemas
+from buildflow.io.providers.schemas import bigquery_schemas as bq_schemas
 
 
 class BigqueryTest(unittest.TestCase):
-
     def test_primitive_types(self):
-
         @dataclass
         class Schema:
             int_field: int
             str_field: str
             float_field: float
             timestamp: datetime
             bytes_field: bytes
             bool_field: bool
             date_field: date
             time_field: time
 
-        bq_schema = bq_schemas.dataclass_to_bq_schema(
-            dataclasses.fields(Schema))
+        bq_schema = bq_schemas.dataclass_fields_to_bq_schema(dataclasses.fields(Schema))
 
         expected_schema = [
             bigquery.SchemaField(
-                name='int_field',
-                field_type='INTEGER',
-                mode='REQUIRED',
+                name="int_field",
+                field_type="INTEGER",
+                mode="REQUIRED",
             ),
             bigquery.SchemaField(
-                name='str_field',
-                field_type='STRING',
-                mode='REQUIRED',
+                name="str_field",
+                field_type="STRING",
+                mode="REQUIRED",
             ),
             bigquery.SchemaField(
-                name='float_field',
-                field_type='FLOAT',
-                mode='REQUIRED',
+                name="float_field",
+                field_type="FLOAT",
+                mode="REQUIRED",
             ),
             bigquery.SchemaField(
-                name='timestamp',
-                field_type='TIMESTAMP',
-                mode='REQUIRED',
+                name="timestamp",
+                field_type="TIMESTAMP",
+                mode="REQUIRED",
             ),
             bigquery.SchemaField(
-                name='bytes_field',
-                field_type='BYTES',
-                mode='REQUIRED',
+                name="bytes_field",
+                field_type="BYTES",
+                mode="REQUIRED",
             ),
             bigquery.SchemaField(
-                name='bool_field',
-                field_type='BOOL',
-                mode='REQUIRED',
+                name="bool_field",
+                field_type="BOOL",
+                mode="REQUIRED",
             ),
             bigquery.SchemaField(
-                name='date_field',
-                field_type='DATE',
-                mode='REQUIRED',
+                name="date_field",
+                field_type="DATE",
+                mode="REQUIRED",
             ),
             bigquery.SchemaField(
-                name='time_field',
-                field_type='TIME',
-                mode='REQUIRED',
+                name="time_field",
+                field_type="TIME",
+                mode="REQUIRED",
             ),
         ]
 
         self.assertEqual(bq_schema, expected_schema)
 
     def test_repeated(self):
-
         @dataclass
         class Schema:
             int_field: List[int]
 
         expected_schema = [
             bigquery.SchemaField(
-                name='int_field',
-                field_type='INTEGER',
-                mode='REPEATED',
+                name="int_field",
+                field_type="INTEGER",
+                mode="REPEATED",
             )
         ]
 
-        bq_schema = bq_schemas.dataclass_to_bq_schema(
-            dataclasses.fields(Schema))
+        bq_schema = bq_schemas.dataclass_fields_to_bq_schema(dataclasses.fields(Schema))
         self.assertEqual(bq_schema, expected_schema)
 
     def test_optional(self):
-
         @dataclass
         class Schema:
             int_field: Optional[int]
 
         expected_schema = [
             bigquery.SchemaField(
-                name='int_field',
-                field_type='INTEGER',
-                mode='NULLABLE',
+                name="int_field",
+                field_type="INTEGER",
+                mode="NULLABLE",
             )
         ]
 
-        bq_schema = bq_schemas.dataclass_to_bq_schema(
-            dataclasses.fields(Schema))
+        bq_schema = bq_schemas.dataclass_fields_to_bq_schema(dataclasses.fields(Schema))
         self.assertEqual(bq_schema, expected_schema)
 
     def test_record(self):
-
         @dataclass
         class Nested:
             val: int
 
         @dataclass
         class Schema:
             opt_nested: Optional[Nested]
             req_nested: Nested
             list_nested: List[Nested]
 
         expected_schema = [
             bigquery.SchemaField(
-                name='opt_nested',
-                field_type='RECORD',
-                mode='NULLABLE',
+                name="opt_nested",
+                field_type="RECORD",
+                mode="NULLABLE",
                 fields=[
-                    bigquery.SchemaField(name='val',
-                                         field_type='INTEGER',
-                                         mode='REQUIRED',
-                                         fields=[])
+                    bigquery.SchemaField(
+                        name="val", field_type="INTEGER", mode="REQUIRED", fields=[]
+                    )
                 ],
             ),
             bigquery.SchemaField(
-                name='req_nested',
-                field_type='RECORD',
-                mode='REQUIRED',
+                name="req_nested",
+                field_type="RECORD",
+                mode="REQUIRED",
                 fields=[
-                    bigquery.SchemaField(name='val',
-                                         field_type='INTEGER',
-                                         mode='REQUIRED',
-                                         fields=[])
+                    bigquery.SchemaField(
+                        name="val", field_type="INTEGER", mode="REQUIRED", fields=[]
+                    )
                 ],
             ),
             bigquery.SchemaField(
-                name='list_nested',
-                field_type='RECORD',
-                mode='REPEATED',
+                name="list_nested",
+                field_type="RECORD",
+                mode="REPEATED",
                 fields=[
-                    bigquery.SchemaField(name='val',
-                                         field_type='INTEGER',
-                                         mode='REQUIRED',
-                                         fields=[])
+                    bigquery.SchemaField(
+                        name="val", field_type="INTEGER", mode="REQUIRED", fields=[]
+                    )
                 ],
-            )
+            ),
         ]
 
-        bq_schema = bq_schemas.dataclass_to_bq_schema(
-            dataclasses.fields(Schema))
+        bq_schema = bq_schemas.dataclass_fields_to_bq_schema(dataclasses.fields(Schema))
         self.assertEqual(bq_schema, expected_schema)
 
     def test_unknown_type(self):
-
         @dataclass
         class Schema:
             int_field: Union[int, float]
 
         with self.assertRaises(ValueError):
-            bq_schemas.dataclass_to_bq_schema(dataclasses.fields(Schema))
+            bq_schemas.dataclass_fields_to_bq_schema(dataclasses.fields(Schema))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `buildflow-0.0.9/buildflow/samples/csv_bigquery_walkthrough.py` & `buildflow-0.1.0/buildflow/samples/csv_bigquery_walkthrough.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# flake8: noqa
-import argparse
 import csv
 import dataclasses
 import datetime
+import os
 import io
-import sys
 from typing import List
 
 import buildflow
-from buildflow import Flow
+from buildflow import Node, InfraConfig, SchemaValidation
 
-# Parser to allow run time configuration of arguments
-parser = argparse.ArgumentParser()
-parser.add_argument('--gcp_project', type=str, required=True)
-parser.add_argument('--bucket_name', type=str, required=True)
-args, _ = parser.parse_known_args(sys.argv)
+gcp_project = os.environ["GCP_PROJECT"]
+bucket_name = os.environ["BUCKET_NAME"]
+bigquery_table = os.environ.get("BIGQUERY_TABLE", "wiki-page-views")
+dataset = os.environ.get("DATASET", "buildflow_walkthrough")
 
 # Set up a subscriber for the source.
 # The source will setup a Pub/Sub topic and subscription to listen to new files
 # uploaded to the GCS bucket.
-source = buildflow.GCSFileNotifications(project_id=args.gcp_project,
-                                        bucket_name=args.bucket_name)
+source = buildflow.io.GCSFileStream(
+    project_id=gcp_project, bucket_name=bucket_name, force_destroy=True
+)
 # Set up a BigQuery table for the sink.
 # If this table does not exist yet BuildFlow will create it.
-sink = buildflow.BigQuerySink(
-    table_id=f'{args.gcp_project}.buildflow_walkthrough.csv_bigquery')
+sink = buildflow.io.BigQueryTable(
+    table_id=f"{gcp_project}.{dataset}.{bigquery_table}", destroy_protection=False
+)
 
 
 # Nested dataclasses can be used inside of your schemas.
 @dataclasses.dataclass
 class HourAggregate:
     hour: datetime.datetime
     stat: int
@@ -43,31 +42,35 @@
     wiki: str
     title: str
     daily_page_views: int
     max_page_views_per_hour: HourAggregate
     min_page_views_per_hour: HourAggregate
 
 
-flow = Flow()
+infra_config = InfraConfig(
+    schema_validation=SchemaValidation.LOG_WARNING,
+    require_confirmation=False,
+    log_level="WARNING",
+)
+app = Node(infra_config=infra_config)
 
 
 # Define our processor.
-@flow.processor(source=source, sink=sink)
-def process(
-        gcs_file_event: buildflow.GCSFileEvent
-) -> List[AggregateWikiPageViews]:
+@app.processor(source=source, sink=sink)
+def process(gcs_file_event: buildflow.io.GCSFileEvent) -> List[AggregateWikiPageViews]:
     csv_string = gcs_file_event.blob.decode()
     csv_reader = csv.DictReader(io.StringIO(csv_string))
     aggregate_stats = {}
     for row in csv_reader:
-        timestamp = datetime.datetime.strptime(row['datehour'],
-                                               '%Y-%m-%d %H:%M:%S.%f %Z')
-        wiki = row['wiki']
-        title = row['title']
-        views = row['views']
+        timestamp = datetime.datetime.strptime(
+            row["datehour"], "%Y-%m-%d %H:%M:%S.%f %Z"
+        )
+        wiki = row["wiki"]
+        title = row["title"]
+        views = row["views"]
 
         key = (wiki, title)
         if key in aggregate_stats:
             stats = aggregate_stats[key]
             stats.daily_page_views += views
             if views > stats.max_page_views_per_hour.stat:
                 stats.max_page_views_per_hour = HourAggregate(timestamp, views)
@@ -82,9 +85,9 @@
                 max_page_views_per_hour=HourAggregate(timestamp, views),
                 min_page_views_per_hour=HourAggregate(timestamp, views),
             )
 
     return list(aggregate_stats.values())
 
 
-# Run your flow.
-flow.run()
+if __name__ == "__main__":
+    app.run()
```

### Comparing `buildflow-0.0.9/buildflow/samples/pubsub_walkthrough.py` & `buildflow-0.1.0/buildflow/samples/pubsub_walkthrough.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-# flake8: noqa
-import argparse
 import dataclasses
 from datetime import datetime
-import sys
+import os
 from typing import Any, Dict
 
 import buildflow
-from buildflow import Flow
+from buildflow import Node, InfraConfig, SchemaValidation
 
-# Parser to allow run time configuration of arguments
-parser = argparse.ArgumentParser()
-parser.add_argument('--gcp_project', type=str, required=True)
-args, _ = parser.parse_known_args(sys.argv)
+gcp_project = os.environ["GCP_PROJECT"]
+bigquery_table = os.environ.get("BIGQUERY_TABLE", "taxi_rides")
+subscription = os.environ.get("SUBSCRIPTION", "taxi-rides-sub")
+dataset = os.environ.get("DATASET", "buildflow_walkthrough")
 
 # Set up a subscriber for the source.
 # If this subscriber does not exist yet BuildFlow will create it.
-input_sub = buildflow.PubSubSource(
-    subscription=f'projects/{args.gcp_project}/subscriptions/taxiride-sub',
-    topic='projects/pubsub-public-data/topics/taxirides-realtime')
+input_sub = buildflow.io.GCPPubSubSubscription(
+    project_id=gcp_project,
+    subscription_name=subscription,
+    topic_id="projects/pubsub-public-data/topics/taxirides-realtime",
+)
 # Set up a BigQuery table for the sink.
 # If this table does not exist yet BuildFlow will create it.
-output_table = buildflow.BigQuerySink(
-    table_id=f'{args.gcp_project}.buildflow_walkthrough.taxi_ride_data')
+output_table = buildflow.io.BigQueryTable(
+    table_id=f"{gcp_project}.{dataset}.{bigquery_table}",
+    destroy_protection=False,
+)
 
 
 # Define an output type for our pipeline.
 # By using a dataclass we can ensure our python type hints are validated
 # against the BigQuery table's schema.
 @dataclasses.dataclass
 class TaxiOutput:
@@ -36,18 +38,23 @@
     timestamp: datetime
     meter_reading: float
     meter_increment: float
     ride_status: str
     passenger_count: int
 
 
-flow = Flow()
+infra_config = InfraConfig(
+    schema_validation=SchemaValidation.LOG_WARNING,
+    require_confirmation=False,
+    log_level="WARNING",
+)
+app = Node(infra_config=infra_config)
 
 
 # Define our processor.
-@flow.processor(source=input_sub, sink=output_table)
+@app.processor(source=input_sub, sink=output_table)
 def process(element: Dict[str, Any]) -> TaxiOutput:
-    return element
+    return TaxiOutput(**element)
 
 
-# Run our flow.
-flow.run()
+if __name__ == "__main__":
+    app.run()
```

### Comparing `buildflow-0.0.9/buildflow.egg-info/PKG-INFO` & `buildflow-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: buildflow
-Version: 0.0.9
+Version: 0.1.0
 Summary: buildflow is a unified **batch** and **streaming** framework that turns any python function into a scalable data pipeline that can read from our supported IO resources.
 Author-email: Caleb Van Dyke <caleb@launchflow.com>, Josh Tanke <josh@launchflow.com>
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # BuildFlow
 
 ![CI](https://github.com/launchflow/buildflow/actions/workflows/python_ci.yaml/badge.svg)
+![GCP Tests](https://github.com/launchflow/buildflow/actions/workflows/gcp_integration.yaml/badge.svg)
 [![Discord Shield](https://discordapp.com/api/guilds/1082821064180117575/widget.png?style=shield)](https://discordapp.com/invite/wz7fjHyrCA)
 
 **BuildFlow**, is an open source framework that lets you build a data pipeline by simply attaching a decorator to a Python function. All you need to do is describe where your input is coming from and where your output should be written, and BuildFlow handles the rest. No configuration outside of the code is required.
 
-
 Key Features:
 
 - Unified **batch** and **streaming** [Processor API](https://www.buildflow.dev/docs/processors/overview)
 - Production-grade [IO connectors](https://www.buildflow.dev/docs/io-connectors/overview) for popular cloud services & storage systems
 - IO templates for common data pipelines (e.g. [file upload notifications](https://www.buildflow.dev/docs/io-connectors/gcs_notifications))
 - Automatic [resource creation / management](https://www.buildflow.dev/docs/resource-creation) for popular cloud resources
 - [Schema validation](https://www.buildflow.dev/docs/schema-validation) powered by Python dataclasses and type hints
 - Automatic parallelism powered by [Ray](https://ray.io)
 
 ## Quick Links
 
-- **Docs**: https://www.buildflow.dev/docs/intro
+- **Docs**: https://www.buildflow.dev/docs
 - **Walkthroughs**: https://www.buildflow.dev/docs/category/walk-throughs
 - **Discord**: https://discordapp.com/invite/wz7fjHyrCA
 
 ## Quickstart
 
 ### Install
 
@@ -61,15 +61,26 @@
 def stream_processor(pubsub_message):
   # TODO(developer): Implement processing logic
   ...
   # The output is sent to the sink provider
   return pubsub_message
 
 # Start the processor(s)
-flow.run(num_replicas=4)
+flow.run().output()
 ```
 
 For a more in depth tutorial see our [walkthroughs](https://www.buildflow.dev/docs/category/walk-throughs).
 
 ## Windows Users
 
 Our runtime is built on [Ray](https://ray.io/), where Windows support is currently in beta. See the [Ray docs](https://docs.ray.io/en/latest/ray-overview/installation.html#windows-support) for more info.
+
+## Code Health Checks
+
+We use [black](https://github.com/psf/black) and [ruff](https://github.com/charliermarsh/ruff) with [pre-commit](https://pre-commit.com/) hooks to perform health checks.
+To setup these locally:
+
+- Clone the repo
+- Install the `dev` dependencies like `python -m pip install .[dev]
+- Check if pre-commit is installed correctly by running `pre-commit --version`
+- Setup pre-commit to run before every commit on staged changes by running `pre-commit install`
+- Pre-commit can also be ran manually as `pre-commit run --all-files`
```

### Comparing `buildflow-0.0.9/integration_tests/pubsub_to_pubsub/pubsub_publish.py` & `buildflow-0.1.0/integration_tests/pubsub_to_pubsub/pubsub_publish.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 import json
+import os
 import time
 
 from google.api_core import exceptions
 from google.cloud import pubsub_v1
 
+
+gcp_project = os.environ["GCP_PROJECT"]
+validation_sub = os.environ["VALIDATION_SUB"]
+incoming_topic = os.environ["INCOMING_TOPIC"]
+outgoing_topic = os.environ["OUTGOING_TOPIC"]
+
 # CREATE THE VALIDATION SUBSCRIPTION
 # this is used out side of buildflow so we have to create it.
 subscriber = pubsub_v1.SubscriberClient()
-subscription_path = subscriber.subscription_path('pubsub-test-project',
-                                                 'validation')
+subscription_path = subscriber.subscription_path(gcp_project, validation_sub)
 # Wrap the subscriber in a 'with' block to automatically call close()
 # to close the underlying gRPC channel when done.
 subscriber = pubsub_v1.SubscriberClient()
 while True:
     try:
         subscription = subscriber.create_subscription(
             request={
-                'name': subscription_path,
-                'topic':
-                'projects/pubsub-test-project/topics/outgoing_topic'
-            })
+                "name": subscription_path,
+                "topic": f"projects/{gcp_project}/topics/{outgoing_topic}",
+            }
+        )
         break
     except exceptions.NotFound:
         time.sleep(2)
 
 _TIMEOUT_SECS = 60
 
-topic = 'projects/pubsub-test-project/topics/incoming_topic'
+topic = f"projects/{gcp_project}/topics/{incoming_topic}"
 client = pubsub_v1.PublisherClient()
 topics = []
 start_time = time.time()
 while topic not in topics:
-    topics = list(client.list_topics(project='projects/pubsub-test-project'))
+    topics = list(client.list_topics(project=f"projects/{gcp_project}"))
     topics = [t.name for t in topics]
     if time.time() - start_time > _TIMEOUT_SECS:
-        raise ValueError(f'Unable to find topic: {topic}')
+        raise ValueError(f"Unable to find topic: {topic}")
     time.sleep(1)
 
-print('Publishing to: ', topic)
-future = client.publish(topic, json.dumps({'val': 1}).encode('UTF-8'))
+print("Publishing to: ", topic)
+future = client.publish(topic, json.dumps({"val": 1}).encode("UTF-8"))
 future.result()
```

### Comparing `buildflow-0.0.9/integration_tests/pubsub_to_pubsub/pubsub_validation.py` & `buildflow-0.1.0/integration_tests/pubsub_to_pubsub/pubsub_validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import json
+import os
 from concurrent.futures import TimeoutError
 
 from google.cloud import pubsub_v1
 
 
-# CREATE THE VALIDATION SUBSCRIPTION
+gcp_project = os.environ["GCP_PROJECT"]
+validation_sub = os.environ["VALIDATION_SUB"]
+
+
 # this is used out side of buildflow so we have to create it.
 subscriber = pubsub_v1.SubscriberClient()
-subscription_path = subscriber.subscription_path('pubsub-test-project',
-                                                 'validation')
+subscription_path = subscriber.subscription_path(gcp_project, validation_sub)
 
-expected_data = {'output_val': 2}
+expected_data = {"output_val": 2}
 
 match = False
 
 
 def callback(message):
     global match
     try:
         got = json.loads(message.data.decode())
-        assert expected_data == got, f'expected: {expected_data} got: {got}'
+        assert expected_data == got, f"expected: {expected_data} got: {got}"
         match = True
     finally:
         message.ack()
 
 
 with pubsub_v1.SubscriberClient() as subscriber:
     future = subscriber.subscribe(subscription_path, callback=callback)
-    print('Subscribing to: ', subscription_path)
+    print("Subscribing to: ", subscription_path)
     try:
         future.result(timeout=20)
     except TimeoutError:
-        print('Reached validation subscriber timeout.')
+        print("Reached validation subscriber timeout.")
 
-assert match, 'no match found from output topic.'
+assert match, "no match found from output topic."
```

### Comparing `buildflow-0.0.9/pyproject.toml` & `buildflow-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,88 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "buildflow"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
     { name = "Caleb Van Dyke", email = "caleb@launchflow.com" },
     { name = "Josh Tanke", email = "josh@launchflow.com" },
 ]
 description = "buildflow is a unified **batch** and **streaming** framework that turns any python function into a scalable data pipeline that can read from our supported IO resources."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
+    # TODO: split up AWS and GCP dependencies.
+    "boto3",
+    "dacite",
     "duckdb==0.6.0",
+    "google-auth",
     "google-cloud-bigquery",
     "google-cloud-bigquery-storage",
+    "google-cloud-monitoring",
     "google-cloud-pubsub",
     "google-cloud-storage",
     # TODO: https://github.com/grpc/grpc/issues/31885
-    "grpcio==1.48.2",
+    "grpcio<1.51.1",
     "fastparquet",
     "opentelemetry-api",
     "opentelemetry-sdk",
     "opentelemetry-exporter-otlp",
     "opentelemetry-exporter-jaeger",
     "pandas",
+    "pulumi==3.35.3",
+    "pulumi_gcp",
     "pyarrow",
     "pyyaml",
-    "ray",
+    "ray[default] > 2.0.0",
+    "typer",
     "redis",
 ]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "License :: OSI Approved :: Apache Software License",
 ]
 
 [project.optional-dependencies]
 dev = [
+    "moto",
     "pytest",
-    "flake8",
+    "pytest-cov",
+    "pytest-timeout",
+    "ruff",
+    "black",
+    "pre-commit",
     "setuptools",
     "wheel"
 ]
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
+
+[project.scripts]
+buildflow = "buildflow.cli.main:main"
+
+[tool.coverage.report]
+# Regexes for lines to exclude from consideration
+exclude_also = [
+    # Don't complain about missing debug-only code:
+    "def __repr__",
+    # Don't complain if tests don't hit defensive assertion code:
+    "raise AssertionError",
+    "raise NotImplementedError",
+    "if __name__ == .__main__.:",
+    # Don't complain about abstract methods, they aren't run:
+    "@(abc\\.)?abstractmethod",
+]
+ignore_errors = true
+# Files to ignore
+omit = [
+    # Exclude samples
+    "buildflow/samples/*",
+    "buildflow/cli/*",
+    # Exclude skipped / prototype code
+    "buildflow/runtime/ray_io/duckdb_io*"
+]
```

