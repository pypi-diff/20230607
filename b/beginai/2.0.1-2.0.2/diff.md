# Comparing `tmp/beginai-2.0.1.tar.gz` & `tmp/beginai-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beginai-2.0.1.tar", last modified: Sun Apr 30 00:58:36 2023, max compression
+gzip compressed data, was "beginai-2.0.2.tar", last modified: Wed Jun  7 18:32:24 2023, max compression
```

## Comparing `beginai-2.0.1.tar` & `beginai-2.0.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.701349 beginai-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-30 00:58:36.701349 beginai-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-30 00:58:25.000000 beginai-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.673349 beginai-2.0.1/beginai/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.677349 beginai-2.0.1/beginai/conn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/conn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/conn/mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.681349 beginai-2.0.1/beginai/exec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.681349 beginai-2.0.1/beginai/exec/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.689349 beginai-2.0.1/beginai/exec/embeddings/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/category.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/date.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.689349 beginai-2.0.1/beginai/exec/embeddings/instructions/deep_text/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/deep_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/deep_text/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/instructions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/embeddings/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/execute_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/exec/remote_compute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.689349 beginai-2.0.1/beginai/orchapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/orchapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/orchapi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.693349 beginai-2.0.1/beginai/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/storage/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/storage/sqllite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.693349 beginai-2.0.1/beginai/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.693349 beginai-2.0.1/beginai/tests/exec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.697349 beginai-2.0.1/beginai/tests/exec/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.701349 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/boolean_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/category_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/interaction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/location_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/number_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/instructions/text_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/mock_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_interaction_attributes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/tests/exec/embeddings/worker_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.701349 beginai-2.0.1/beginai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-30 00:58:25.000000 beginai-2.0.1/beginai/utils/syft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:58:36.677349 beginai-2.0.1/beginai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-30 00:58:36.000000 beginai-2.0.1/beginai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-30 00:58:36.000000 beginai-2.0.1/beginai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:58:36.000000 beginai-2.0.1/beginai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-30 00:58:36.000000 beginai-2.0.1/beginai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 00:58:36.000000 beginai-2.0.1/beginai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-30 00:58:36.701349 beginai-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-30 00:58:35.000000 beginai-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-07 18:32:24.445422 beginai-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-07 18:32:14.000000 beginai-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.441422 beginai-2.0.2/beginai/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.441422 beginai-2.0.2/beginai/conn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/conn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/conn/mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.441422 beginai-2.0.2/beginai/exec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.441422 beginai-2.0.2/beginai/exec/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/exec/embeddings/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/date.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/exec/embeddings/instructions/deep_text/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/deep_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/deep_text/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/execute_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/remote_compute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/orchapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/orchapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/orchapi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/storage/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/storage/sqllite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/tests/exec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/tests/exec/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/boolean_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/category_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/interaction_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/location_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/number_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/text_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/mock_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_interaction_attributes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/utils/syft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.441422 beginai-2.0.2/beginai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-07 18:32:24.000000 beginai-2.0.2/beginai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-07 18:32:24.000000 beginai-2.0.2/beginai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:32:24.000000 beginai-2.0.2/beginai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-07 18:32:24.000000 beginai-2.0.2/beginai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:32:24.000000 beginai-2.0.2/beginai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 18:32:24.445422 beginai-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-07 18:32:23.000000 beginai-2.0.2/setup.py
```

### Comparing `beginai-2.0.1/PKG-INFO` & `beginai-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beginai
-Version: 2.0.1
+Version: 2.0.2
 Summary: A library to interact with Begin AI platform in order to build personalisation algorithms.
 Home-page: https://docs.begin.ai
 Author: Begin AI Research & Engineering
 Author-email: engineering@begin.ai
 License: Proprietary
 Description: 
                 This is Begin AI python SDK for both batch processing and application integration.
```

### Comparing `beginai-2.0.1/beginai/conn/mqtt.py` & `beginai-2.0.2/beginai/conn/mqtt.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/exec/embeddings/apply.py` & `beginai-2.0.2/beginai/exec/embeddings/apply.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,16 @@
             filename, self.INTERACTIONS, unique_identifier_column, target_object, created_at_column=created_at_column, file_separator=file_separator)
 
     def _add_data_to_files_dictionary(self, filename, object_name, uuid_column, target_object={}, label_column=None, created_at_column=None, file_separator=","):
         self.files[object_name] = {
             'data': self._read_file(filename, file_separator),
             'uuid_column': uuid_column.lower(),
             'target_object': target_object,
-            'label_column': label_column,
-            'created_at_column': created_at_column,
+            'label_column': label_column.lower() if label_column is not None else None,
+            'created_at_column': created_at_column.lower() if created_at_column is not None else None,
         }
 
     def _read_file(self, filename, file_separator):
         if filename == '' or filename is None:
             raise ValueError('File must be provided')
 
         df = pd.read_csv(filename, dtype=str, sep=file_separator)
@@ -161,15 +161,14 @@
                         self.embeddings[object_key] = []
 
                     self.embeddings[object_key] = object_data
 
     def _preparing_dataframe(self, df: pd.DataFrame, object_config: dict, object_key: str, instructions: dict) -> pd.DataFrame:
         label_column = object_config['label_column']
         created_at_column = object_config['created_at_column']
-
         # Rename columns representing begin constructs as identified by the user
         if object_key != self.INTERACTIONS and label_column is not None:
             try:
                 df = df.rename(
                     columns={label_column: self.LABELS}, errors="raise")
             except:
                 raise ValueError(
```

### Comparing `beginai-2.0.1/beginai/exec/embeddings/instructions/__init__.py` & `beginai-2.0.2/beginai/exec/embeddings/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/exec/embeddings/instructions/date.py` & `beginai-2.0.2/beginai/exec/embeddings/instructions/date.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from datetime import date, datetime
 
 class Age(object):
 
     def __init__(self):
         pass
 
+    def _convert_to_date(self, value):
+        try:
+            return datetime.strptime(value, "%d-%m-%Y").date()
+        except Exception:
+            return datetime.strptime(value, "%Y-%m-%d").date()    
+
     def apply(self, value):
-        born = datetime.strptime(value, "%d-%m-%Y").date()
+        born = self._convert_to_date(value)
         today = date.today()
         return today.year - born.year - ((today.month, today.day) < (born.month, born.day))
 
 class CompareDates(object):
     """
     compare dates from two fields.
     """
```

### Comparing `beginai-2.0.1/beginai/exec/embeddings/instructions/deep_text/bpe.py` & `beginai-2.0.2/beginai/exec/embeddings/instructions/deep_text/bpe.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/exec/embeddings/instructions/interaction.py` & `beginai-2.0.2/beginai/exec/embeddings/instructions/interaction.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/exec/embeddings/instructions/location.py` & `beginai-2.0.2/beginai/exec/embeddings/instructions/location.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/exec/embeddings/instructions/number.py` & `beginai-2.0.2/beginai/exec/embeddings/instructions/number.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/exec/embeddings/instructions/parser.py` & `beginai-2.0.2/beginai/exec/embeddings/instructions/parser.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/exec/embeddings/instructions/text.py` & `beginai-2.0.2/beginai/exec/embeddings/instructions/text.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/exec/embeddings/instructions/utils.py` & `beginai-2.0.2/beginai/exec/embeddings/instructions/utils.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/exec/embeddings/worker.py` & `beginai-2.0.2/beginai/exec/embeddings/worker.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/exec/execute_compute.py` & `beginai-2.0.2/beginai/exec/execute_compute.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/exec/remote_compute.py` & `beginai-2.0.2/beginai/exec/remote_compute.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/orchapi/api.py` & `beginai-2.0.2/beginai/orchapi/api.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/boolean_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/boolean_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/category_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/category_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/date_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/date_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/interaction_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/interaction_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/location_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/location_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/number_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/number_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/parser_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/parser_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         "tokens": {"input_ids": [], "attention_mask": [], "len_": 0},
         "identifiers": {},
         "created_at": None
     }
     assert json.dumps(results, sort_keys=True) == json.dumps(
         expected, sort_keys=True)
 
-
+@freeze_time("2021-05-16")
 def test_parse_instructions_with_interactions_only():
     instructions = json.loads("""
     {
         "instructions":{
             "interactions":{
                 "home":{
                     "actions":[ "test"],
@@ -300,15 +300,15 @@
                     "dosomething": {
                         "embedding": None,
                         "created_at": 1234
                     }
                 },
                 "20": {
                     "react": {
-                        "embedding": [31.0, 18.0],
+                        "embedding": [30.0, 18.0],
                         "created_at": None
                     }
                 }
             }
         }
     }
     assert json.dumps(results, sort_keys=True) == json.dumps(
```

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/instructions/text_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/text_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/mock_service.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/mock_service.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_interaction_attributes_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_interaction_attributes_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/tests/exec/embeddings/worker_test.py` & `beginai-2.0.2/beginai/tests/exec/embeddings/worker_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai/utils/syft.py` & `beginai-2.0.2/beginai/utils/syft.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/beginai.egg-info/PKG-INFO` & `beginai-2.0.2/beginai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beginai
-Version: 2.0.1
+Version: 2.0.2
 Summary: A library to interact with Begin AI platform in order to build personalisation algorithms.
 Home-page: https://docs.begin.ai
 Author: Begin AI Research & Engineering
 Author-email: engineering@begin.ai
 License: Proprietary
 Description: 
                 This is Begin AI python SDK for both batch processing and application integration.
```

### Comparing `beginai-2.0.1/beginai.egg-info/SOURCES.txt` & `beginai-2.0.2/beginai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beginai-2.0.1/setup.py` & `beginai-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 REQ_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "pip-dep")
 core_reqs, core_dependency_links = get_requirements(os.path.join(REQ_DIR, "requirements.txt"))
 
 
 if __name__ == "__main__":
     setup(
         name="beginai",
-        version="2.0.1",
+        version="2.0.2",
         author="Begin AI Research & Engineering",
         author_email="engineering@begin.ai",
         description="A library to interact with Begin AI platform in order to build personalisation algorithms.",
         long_description="""
         This is Begin AI python SDK for both batch processing and application integration. 
         It can be used to integrate applications with Begin.ai orchestration platform to deliver applications with
         personalisation algorithms to do:
```

