# Comparing `tmp/sarus-0.7.0rc0.tar.gz` & `tmp/sarus-0.7.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.7.0rc0.tar", last modified: Fri Jun  2 15:37:40 2023, max compression
+gzip compressed data, was "sarus-0.7.1.dev0.tar", last modified: Wed Jun  7 14:48:15 2023, max compression
```

## Comparing `sarus-0.7.0rc0.tar` & `sarus-0.7.1.dev0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1556 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.7.0rc0/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.7.0rc0/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.501549 sarus-0.7.0rc0/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      547 2023-06-02 15:33:14.000000 sarus-0.7.0rc0/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13201 2023-06-02 08:49:56.000000 sarus-0.7.0rc0/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.501549 sarus-0.7.0rc0/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3137 2023-06-02 15:33:20.000000 sarus-0.7.0rc0/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13990 2023-06-02 08:52:35.000000 sarus-0.7.0rc0/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.505549 sarus-0.7.0rc0/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.505549 sarus-0.7.0rc0/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.505549 sarus-0.7.0rc0/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/base_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7609 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      688 2023-05-25 13:23:26.000000 sarus-0.7.0rc0/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    20847 2023-05-25 13:23:26.000000 sarus-0.7.0rc0/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2023-06-02 08:49:56.000000 sarus-0.7.0rc0/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4843 2023-06-02 08:49:56.000000 sarus-0.7.0rc0/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42677 2023-06-02 15:33:20.000000 sarus-0.7.0rc0/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.509549 sarus-0.7.0rc0/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/scripts/generate_op_list.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.529549 sarus-0.7.0rc0/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.529549 sarus-0.7.0rc0/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-23 10:20:26.000000 sarus-0.7.0rc0/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.501549 sarus-0.7.0rc0/sarus.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1556 2023-06-02 15:37:40.000000 sarus-0.7.0rc0/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1965 2023-06-02 15:37:40.000000 sarus-0.7.0rc0/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-02 15:37:40.000000 sarus-0.7.0rc0/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.7.0rc0/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      342 2023-06-02 15:37:40.000000 sarus-0.7.0rc0/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-06-02 15:37:40.000000 sarus-0.7.0rc0/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1301 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      109 2023-06-02 15:34:08.000000 sarus-0.7.0rc0/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-02 15:37:40.533549 sarus-0.7.0rc0/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.7.0rc0/tests/test_sanity.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.737425 sarus-0.7.1.dev0/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1558 2023-06-07 14:48:15.737425 sarus-0.7.1.dev0/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.7.1.dev0/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.7.1.dev0/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.721425 sarus-0.7.1.dev0/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-06-07 13:57:15.000000 sarus-0.7.1.dev0/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13201 2023-06-07 13:55:59.000000 sarus-0.7.1.dev0/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.725425 sarus-0.7.1.dev0/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3137 2023-06-07 13:55:59.000000 sarus-0.7.1.dev0/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13990 2023-06-07 13:55:59.000000 sarus-0.7.1.dev0/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.725425 sarus-0.7.1.dev0/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.725425 sarus-0.7.1.dev0/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.725425 sarus-0.7.1.dev0/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.729425 sarus-0.7.1.dev0/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7988 2023-06-07 13:57:15.000000 sarus-0.7.1.dev0/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.729425 sarus-0.7.1.dev0/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      688 2023-06-07 13:55:59.000000 sarus-0.7.1.dev0/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    20840 2023-06-07 13:57:15.000000 sarus-0.7.1.dev0/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-06-07 13:55:59.000000 sarus-0.7.1.dev0/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.729425 sarus-0.7.1.dev0/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.729425 sarus-0.7.1.dev0/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2023-06-07 13:55:59.000000 sarus-0.7.1.dev0/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4843 2023-06-07 13:55:59.000000 sarus-0.7.1.dev0/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.729425 sarus-0.7.1.dev0/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.729425 sarus-0.7.1.dev0/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    43589 2023-06-07 13:57:15.000000 sarus-0.7.1.dev0/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.729425 sarus-0.7.1.dev0/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/scripts/generate_op_list.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.733425 sarus-0.7.1.dev0/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.733425 sarus-0.7.1.dev0/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.737425 sarus-0.7.1.dev0/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-06-07 13:55:59.000000 sarus-0.7.1.dev0/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.737425 sarus-0.7.1.dev0/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-06-07 13:55:59.000000 sarus-0.7.1.dev0/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.737425 sarus-0.7.1.dev0/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-23 10:20:26.000000 sarus-0.7.1.dev0/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.725425 sarus-0.7.1.dev0/sarus.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1558 2023-06-07 14:48:15.000000 sarus-0.7.1.dev0/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1965 2023-06-07 14:48:15.000000 sarus-0.7.1.dev0/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-07 14:48:15.000000 sarus-0.7.1.dev0/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.7.1.dev0/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      342 2023-06-07 14:48:15.000000 sarus-0.7.1.dev0/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-06-07 14:48:15.000000 sarus-0.7.1.dev0/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1301 2023-06-07 14:48:15.741425 sarus-0.7.1.dev0/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      110 2023-06-07 14:06:58.000000 sarus-0.7.1.dev0/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-07 14:48:15.737425 sarus-0.7.1.dev0/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.7.1.dev0/tests/test_sanity.py
```

### Comparing `sarus-0.7.0rc0/PKG-INFO` & `sarus-0.7.1.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.7.0rc0
+Version: 0.7.1.dev0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.7.0rc0/README.rst` & `sarus-0.7.1.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/__init__.py` & `sarus-0.7.1.dev0/sarus/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         std,
         xgboost,
     )
 
     from .sarus import Client, Dataset
     from .utils import eval, eval_policy, floating, integer, length
 
-VERSION = "0.6.7rc1"
+VERSION = "0.7.0"
 
 __all__ = [
     "Dataset",
     "Client",
     "length",
     "eval",
     "eval_policy",
```

### Comparing `sarus-0.7.0rc0/sarus/config.yaml` & `sarus-0.7.1.dev0/sarus/config.yaml`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/context/local_sdk.py` & `sarus-0.7.1.dev0/sarus/context/local_sdk.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/dataspec_wrapper.py` & `sarus-0.7.1.dev0/sarus/dataspec_wrapper.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/debug.py` & `sarus-0.7.1.dev0/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/imblearn/over_sampling.py` & `sarus-0.7.1.dev0/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/imblearn/pipeline.py` & `sarus-0.7.1.dev0/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/imblearn/under_sampling.py` & `sarus-0.7.1.dev0/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/legacy/tensorflow/dataset.py` & `sarus-0.7.1.dev0/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/legacy/tensorflow/model.py` & `sarus-0.7.1.dev0/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/manager/arrow_local.py` & `sarus-0.7.1.dev0/sarus/manager/arrow_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/manager/arrow_remote.py` & `sarus-0.7.1.dev0/sarus/manager/arrow_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/manager/base_remote.py` & `sarus-0.7.1.dev0/sarus/manager/base_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/manager/cache_scalar_local.py` & `sarus-0.7.1.dev0/sarus/manager/cache_scalar_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/manager/dataspec_api.py` & `sarus-0.7.1.dev0/sarus/manager/dataspec_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,21 +48,37 @@
         f"{client.url()}/dataspecs/{uuid}",
     )
     end = time.perf_counter()
     logger.debug(
         f"GET /dataspecs/{uuid} {resp.status_code} ({end-start:.2f}s)"
     )
     if resp.status_code == HTTPStatus.NOT_FOUND:
-        return None, 0.0
+        return None
 
     raise_response(resp)
 
     proto = dict_deserialize(resp.json()["dataspec"])
+    return client.context().factory().create(proto)
+
+
+def get_epsilon(
+    client: Client, uuid: str
+) -> t.Tuple[t.Optional[st.DataSpec], float]:
+    """Fetch a single Dataspec from the server and the consumed epsilon."""
+    resp: Response = client.session().get(
+        f"{client.url()}/dataspecs/{uuid}/epsilon",
+    )
+
+    if resp.status_code == HTTPStatus.NOT_FOUND:
+        return None, 0.0
+
+    raise_response(resp)
+
     epsilon = resp.json()["epsilon"]
-    return client.context().factory().create(proto), epsilon
+    return epsilon
 
 
 def pull_dataspec_graph(client: Client, uuid: str) -> None:
     """Fetch a dataspec's computation graph and store it."""
     start = time.perf_counter()
     resp: Response = client.session().get(
         f"{client.url()}/dataspecs/{uuid}/graph",
```

### Comparing `sarus-0.7.0rc0/sarus/manager/ops/api.py` & `sarus-0.7.1.dev0/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/manager/parquet_local.py` & `sarus-0.7.1.dev0/sarus/manager/parquet_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/manager/sdk_manager.py` & `sarus-0.7.1.dev0/sarus/manager/sdk_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         # applied access rule
         delta = admin_ds.get("accesses").pop(0).get("delta")
         return float(delta)
 
     def consumed_epsilon(self, dataspec: st.DataSpec) -> float:
         """Get the consumed epsilon from the server."""
         # TODO works only when the value is already computed on the server side
-        _, epsilon = api.get_dataspec(self.client(), dataspec.uuid())
+        epsilon = api.get_epsilon(self.client(), dataspec.uuid())
         return epsilon
 
     def client(self) -> Client:
         """Return the sarus.Client object used to make API calls."""
         return self._client
 
     def is_cached(self, dataspec: st.DataSpec) -> bool:
@@ -146,15 +146,15 @@
                 referrables = (
                     list(computation_graph["dataspecs"])
                     + list(computation_graph["transforms"])
                     + list(computation_graph["attributes"])
                 )
                 api.push_dataspec_graph(self._client, referrables)
 
-        ds, _ = api.get_dataspec(self.client(), dataspec.uuid())
+        ds = api.get_dataspec(self.client(), dataspec.uuid())
         return ds is not None
 
     def is_big_data(self, dataset: st.Dataset) -> bool:
         """Method to compute is_big data if the status
         is not in the storage and the dataset is source
         we retrieve it via an api call"""
```

### Comparing `sarus-0.7.0rc0/sarus/manager/typing.py` & `sarus-0.7.1.dev0/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/manager/value_local.py` & `sarus-0.7.1.dev0/sarus/manager/value_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/manager/value_remote.py` & `sarus-0.7.1.dev0/sarus/manager/value_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/numpy/scalars.py` & `sarus-0.7.1.dev0/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/pandas/core.py` & `sarus-0.7.1.dev0/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/pandas/dataframe.py` & `sarus-0.7.1.dev0/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sarus.py` & `sarus-0.7.1.dev0/sarus/sarus.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 import logging
 import os
 import re
 import sys
 import tarfile
 import tempfile
 import textwrap
+import pprint
 import time
 import typing as t
 import warnings
 import webbrowser
 from dataclasses import dataclass
 from io import BytesIO
 from typing import Any, Dict, List, Optional
@@ -86,14 +87,28 @@
         import tensorflow as tf
 
         import sarus.legacy.tensorflow as sltf
     except ModuleNotFoundError:
         pass  # error message in sarus_data_spec.typing
 
 
+class MessageToUserException(Exception):
+    """An exception meant to print a message to the user when printed by
+    the REPL after being raised.
+    """
+
+    args: t.Tuple[str]
+
+    def __str__(self) -> str:
+        indented_msg = "\n"
+        indented_msg += textwrap.indent(self.args[0], "  ")
+
+        return indented_msg
+
+
 @dataclass
 class Synthetic:
     """Simple class to represent synthetic data."""
 
     data: Optional[pa.Table] = None
     rows: Optional[int] = None
 
@@ -844,15 +859,15 @@
             with open(path, "r") as load_file:
                 saved_data = json.load(load_file)
 
             user_ds_uuid = saved_data["user_ds_uuid"]
             wrapper_type = saved_data["wrapper_type"]
 
         pull_dataspec_graph(client=self, uuid=user_ds_uuid)
-        ds, _ = get_dataspec(client=self, uuid=user_ds_uuid)
+        ds = get_dataspec(client=self, uuid=user_ds_uuid)
 
         sources_ds = ds.sources(sp.type_name(sp.Dataset))
         for source in sources_ds:
             if not source.is_public():
                 self.dataset(source["slugname"])
 
         if to_dataset and ds.prototype() == sp.Dataset:
@@ -989,14 +1004,15 @@
 
     def query(
         self,
         query: str,
         target_epsilon: Optional[float] = None,
         verbose: bool = True,
         use_old_query=False,
+        debug=False,
     ) -> int:
         """Execute a SQL query.
 
         Args:
             query (String): SQL query
 
             target_epsilon (Optional[float]): Maximum privacy budget (epsilon) to assign to the query.
@@ -1007,14 +1023,16 @@
                 Default target epsilon is 0 if the access is a Differentially-Private access with
                 per-user or per-group limit; default value equals to per-query limit if the access is
                 a Differentially-Private access with a per-query limit only. Meaning Sarus maximizes result
                 accuracy in the given privacy constraints. See user documentation to know more.
 
             use_old_query (bool): Whether to use the v1 version of the query task.
 
+            debug (bool): Print the remote traceback if available
+
         Returns:
             int: Id of the task.
         """
         endpoint = "query"
         if use_old_query:
             endpoint = "query_v1"
 
@@ -1035,31 +1053,41 @@
                     "limit exceeded"
                 )
             else:
                 http_status_code = request.status_code
                 http_status_name = http.HTTPStatus(http_status_code).name
                 try:
                     error_message = request.json()["error_message"]
-                    wrapped_message = textwrap.indent(error_message, "  |")
+                    message_to_user = error_message
 
-                    raise Exception(wrapped_message)
+                    error_chain = request.json().get("error_chain", None)
+                    if error_chain is not None and debug:
+                        message_to_user += "\n\nRemote Traceback:\n\n"
+                        message_to_user += pprint.pformat(error_chain)
+                    raise MessageToUserException(message_to_user)
                 except (json.JSONDecodeError, KeyError):
                     raise Exception(
                         f"Error while sending a query.\
                                                              Full Gateway answer was:{request}"
                     )
 
         task_id = request.json()["task"]
         dataset_id = request.json()["dataset"]["id"]
         start_eps = request.json()["dataset"]["accesses"][0]["current_epsilon"]
         status = self._poll_query_status(task_id)
         error_message = status.get("error_message", None)
+        error_chain = status.get("error_chain", None)
+
         if error_message is not None:
-            wrapped_message = textwrap.indent(error_message, "  |")
-            raise Exception(wrapped_message)
+            message_to_user = error_message
+
+            if error_chain is not None and debug:
+                message_to_user += "\n\nRemote Traceback:\n\n"
+                message_to_user += pprint.pformat(error_chain)
+            raise MessageToUserException(message_to_user)
         if verbose:
             ds = self._fetch_dataset_by_id(dataset_id)
             logging.info(
                 f"Actual privacy consumption (epsilon): "
                 f"{ds.epsilon-start_eps:.03f}"
             )
```

### Comparing `sarus-0.7.0rc0/sarus/scripts/generate_op_list.py` & `sarus-0.7.1.dev0/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sklearn/__init__.py` & `sarus-0.7.1.dev0/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sklearn/cluster.py` & `sarus-0.7.1.dev0/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sklearn/compose.py` & `sarus-0.7.1.dev0/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sklearn/decomposition.py` & `sarus-0.7.1.dev0/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sklearn/ensemble.py` & `sarus-0.7.1.dev0/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sklearn/impute.py` & `sarus-0.7.1.dev0/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sklearn/linear_model.py` & `sarus-0.7.1.dev0/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sklearn/model_selection.py` & `sarus-0.7.1.dev0/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sklearn/pipeline.py` & `sarus-0.7.1.dev0/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sklearn/preprocessing.py` & `sarus-0.7.1.dev0/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/sklearn/svm.py` & `sarus-0.7.1.dev0/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/skopt/searchcv.py` & `sarus-0.7.1.dev0/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/std/types.py` & `sarus-0.7.1.dev0/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/typing.py` & `sarus-0.7.1.dev0/sarus/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/utils.py` & `sarus-0.7.1.dev0/sarus/utils.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/wrapper_factory.py` & `sarus-0.7.1.dev0/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus/xgboost/xgboost.py` & `sarus-0.7.1.dev0/sarus/xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/sarus.egg-info/PKG-INFO` & `sarus-0.7.1.dev0/sarus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.7.0rc0
+Version: 0.7.1.dev0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.7.0rc0/sarus.egg-info/SOURCES.txt` & `sarus-0.7.1.dev0/sarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus-0.7.0rc0/setup.cfg` & `sarus-0.7.1.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [options]
 zip_safe = False
 python_requires = >=3.7, <3.11
 packages = find:
 include_package_data = True
 install_requires = 
-	sarus-data-spec-public==3.3.0
+	sarus-data-spec-public==3.4.1
 	cloudpickle>=1.2, <2.1
 	pyarrow >= 11.0
 
 [options.extras_require]
 sklearn = 
 	scikit-learn==1.2.2
 	scipy==1.9.0
```

