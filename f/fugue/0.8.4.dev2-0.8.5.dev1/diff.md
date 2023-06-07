# Comparing `tmp/fugue-0.8.4.dev2.tar.gz` & `tmp/fugue-0.8.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugue-0.8.4.dev2.tar", last modified: Mon May  8 16:09:17 2023, max compression
+gzip compressed data, was "fugue-0.8.5.dev1.tar", last modified: Wed Jun  7 07:41:03 2023, max compression
```

## Comparing `fugue-0.8.4.dev2.tar` & `fugue-0.8.5.dev1.tar`

### file list

```diff
@@ -1,325 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/interfaceless.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue/bag/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/bag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/bag/array_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/bag/bag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/collections/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/collections/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/collections/yielded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue/column/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/column/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/column/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/column/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/array_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/arrow_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/dataframe_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataset/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/execution/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/execution/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/execution/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/execution/native_execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/_builtins/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/_builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/_builtins/creators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/_builtins/outputters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/_builtins/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/creator/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/creator/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/creator/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/outputter/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/outputter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/outputter/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/outputter/outputter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/processor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/processor/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/transformer/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/transformer/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/rpc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/rpc/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/sql/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/sql/_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/sql/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/sql/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_contrib/contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_contrib/seaborn/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_contrib/seaborn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_contrib/viz/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_contrib/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_contrib/viz/_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    18462 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    20479 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_ibis/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_ibis/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/execution/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/execution/pandas_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/nbextension/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/nbextension/description.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/nbextension/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_polars/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_polars/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_polars/polars_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_polars/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_ray/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_ray/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/_utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/_utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_spark/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_spark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_utils/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    32541 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/bag_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    75748 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/builtin_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/dataframe_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    50559 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/execution_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/ibis_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_version/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 16:09:17.935146 fugue-0.8.4.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/tests/fugue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/tests/fugue/bag/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/bag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/bag/test_array_bag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/tests/fugue/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/collections/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/collections/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/tests/fugue/column/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/column/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/column/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/column/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_array_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_arrow_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_dataframe_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/test_naive_execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/extensions/creator/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/creator/test_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/extensions/outputter/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/outputter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/outputter/test_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/extensions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/processor/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_cotransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_output_cotransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_output_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/rpc/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/rpc/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/rpc/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/sql/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/sql/test_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/sql/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/sql/test_workflow_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/test_interfaceless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/utils/test_interfaceless.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/utils/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/utils/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/test_runtime_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/test_workflow_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/test_workflow_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_dask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_ibis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_ibis/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/mock/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/mock/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_polars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_polars/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_polars/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_polars/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ray/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ray/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ray/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ray/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_spark_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_spark/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/utils/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/utils/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/utils/test_partition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/interfaceless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/_utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/bag/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/bag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/bag/array_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/bag/bag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/collections/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/collections/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/collections/yielded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/column/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/column/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/column/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/column/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/array_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/arrow_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/dataframe_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataframe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataset/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/execution/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/execution/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/execution/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/execution/native_execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/_builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/_builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/_builtins/creators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/_builtins/outputters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/_builtins/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/creator/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/creator/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/creator/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/outputter/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/outputter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/outputter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/outputter/outputter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/processor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/processor/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/extensions/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/transformer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/transformer/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/extensions/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/rpc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/rpc/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/sql/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/sql/_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/sql/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/sql/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.978742 fugue-0.8.5.dev1/fugue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-07 07:41:03.000000 fugue-0.8.5.dev1/fugue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.982743 fugue-0.8.5.dev1/fugue_contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_contrib/contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_contrib/seaborn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_contrib/seaborn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_contrib/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_contrib/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_contrib/viz/_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_dask/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_duckdb/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_ibis/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/execution/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/execution/pandas_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ibis/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/nbextension/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/nbextension/description.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_notebook/nbextension/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_polars/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_polars/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_polars/polars_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_polars/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.986743 fugue-0.8.5.dev1/fugue_ray/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/_utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/_utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_ray/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/fugue_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/fugue_spark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/_utils/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_spark/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/fugue_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/fugue_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/bag_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76338 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/builtin_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/dataframe_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50948 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/execution_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_test/ibis_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/fugue_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/fugue_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-07 07:41:03.990743 fugue-0.8.5.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-07 07:38:42.000000 fugue-0.8.5.dev1/setup.py
```

### Comparing `fugue-0.8.4.dev2/LICENSE` & `fugue-0.8.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/PKG-INFO` & `fugue-0.8.5.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.4.dev2
+Version: 0.8.5.dev1
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
         
@@ -23,14 +23,16 @@
         **Fugue is a unified interface for distributed computing that lets users execute Python, Pandas, and SQL code on Spark, Dask, and Ray with minimal rewrites**.
         
         Fugue is most commonly used for:
         
         *   **Parallelizing or scaling existing Python and Pandas code** by bringing it to Spark, Dask, or Ray with minimal rewrites.
         *   Using [FugueSQL](https://fugue-tutorials.readthedocs.io/tutorials/quick_look/ten_minutes_sql.html) to **define end-to-end workflows** on top of Pandas, Spark, and Dask DataFrames. FugueSQL is an enhanced SQL interface that can invoke Python code.
         
+        To see how Fugue compares to other frameworks like dbt, Arrow, Ibis, PySpark Pandas, see the [comparisons](https://fugue-tutorials.readthedocs.io/#how-does-fugue-compare-to)
+        
         ## [Fugue API](https://fugue-tutorials.readthedocs.io/tutorials/quick_look/ten_minutes.html)
         
         The Fugue API is a collection of functions that are capable of running on Pandas, Spark, Dask, and Ray. The simplest way to use Fugue is the [`transform()` function](https://fugue-tutorials.readthedocs.io/tutorials/beginner/transform.html). This lets users parallelize the execution of a single function by bringing it to Spark, Dask, or Ray. In the example below, the `map_letter_to_food()` function takes in a mapping and applies it on a column. This is just Pandas and Python so far (without Fugue).
         
         ```python
         import pandas as pd
         from typing import Dict
@@ -218,24 +220,26 @@
         
         FugueSQL backends:
         
         *   Pandas - FugueSQL can run on Pandas
         *   [Duckdb](https://github.com/duckdb/duckdb) - in-process SQL OLAP database management
         *   [dask-sql](https://github.com/dask-contrib/dask-sql) - SQL interface for Dask
         *   SparkSQL
-        *   BigQuery
+        *   [BigQuery](https://fugue-tutorials.readthedocs.io/tutorials/integrations/warehouses/bigquery.html)
+        *   Trino
         
         
         Fugue is available as a backend or can integrate with the following projects:
         
         *   [WhyLogs](https://whylogs.readthedocs.io/en/latest/examples/integrations/Fugue_Profiling.html?highlight=fugue) - data profiling
         *   [PyCaret](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/pycaret.html) - low code machine learning
         *   [Nixtla](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/nixtla.html) - timeseries modelling
         *   [Prefect](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/prefect.html) - workflow orchestration
         *   [Pandera](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/pandera.html) - data validation
+        *   [Datacompy (by Capital One)](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/datacompy.html) - comparing DataFrames
         
         Registered 3rd party extensions (majorly for Fugue SQL) include:
         
         *   [Pandas plot](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.html) - visualize data using matplotlib or plotly
         *   [Seaborn](https://seaborn.pydata.org/api.html) - visualize data using seaborn
         *   [WhyLogs](https://whylogs.readthedocs.io/en/latest/examples/integrations/Fugue_Profiling.html?highlight=fugue) - visualize data profiling
         *   [Vizzu](https://github.com/vizzuhq/ipyvizzu) - visualize data using ipyvizzu
@@ -248,16 +252,15 @@
         
         *   [How LyftLearn Democratizes Distributed Compute through Kubernetes Spark and Fugue](https://eng.lyft.com/how-lyftlearn-democratizes-distributed-compute-through-kubernetes-spark-and-fugue-c0875b97c3d9)
         *   [Clobotics - Large Scale Image Processing with Spark through Fugue](https://medium.com/fugue-project/large-scale-image-processing-with-spark-through-fugue-e510b9813da8)
         
         ### Mentioned Uses
         
         *   [Productionizing Data Science at Interos, Inc. (LinkedIn post by Anthony Holten)](https://www.linkedin.com/posts/anthony-holten_pandas-spark-dask-activity-7022628193983459328-QvcF)
-        
-        *   [Multiple Time Series Forecasting with Fugue & Nixtla at Bain & Company(LinkedIn post by Fahad Akbar)](https://www.linkedin.com/posts/fahadakbar_fugue-datascience-forecasting-activity-7041119034813124608-u08q?utm_source=share&utm_medium=member_desktop)
+        *   [Multiple Time Series Forecasting with Fugue & Nixtla at Bain & Company (LinkedIn post by Fahad Akbar)](https://www.linkedin.com/posts/fahadakbar_fugue-datascience-forecasting-activity-7041119034813124608-u08q?utm_source=share&utm_medium=member_desktop)
         
         ## Further Resources
         
         View some of our latest conferences presentations and content. For a more complete list, check the [Content](https://fugue-tutorials.readthedocs.io/tutorials/resources/content.html) page in the tutorials.
         
         ### Blogs
         
@@ -281,14 +284,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: sql
 Provides-Extra: cpp_sql_parser
 Provides-Extra: spark
 Provides-Extra: dask
 Provides-Extra: ray
 Provides-Extra: duckdb
 Provides-Extra: polars
 Provides-Extra: ibis
```

### Comparing `fugue-0.8.4.dev2/README.md` & `fugue-0.8.5.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 **Fugue is a unified interface for distributed computing that lets users execute Python, Pandas, and SQL code on Spark, Dask, and Ray with minimal rewrites**.
 
 Fugue is most commonly used for:
 
 *   **Parallelizing or scaling existing Python and Pandas code** by bringing it to Spark, Dask, or Ray with minimal rewrites.
 *   Using [FugueSQL](https://fugue-tutorials.readthedocs.io/tutorials/quick_look/ten_minutes_sql.html) to **define end-to-end workflows** on top of Pandas, Spark, and Dask DataFrames. FugueSQL is an enhanced SQL interface that can invoke Python code.
 
+To see how Fugue compares to other frameworks like dbt, Arrow, Ibis, PySpark Pandas, see the [comparisons](https://fugue-tutorials.readthedocs.io/#how-does-fugue-compare-to)
+
 ## [Fugue API](https://fugue-tutorials.readthedocs.io/tutorials/quick_look/ten_minutes.html)
 
 The Fugue API is a collection of functions that are capable of running on Pandas, Spark, Dask, and Ray. The simplest way to use Fugue is the [`transform()` function](https://fugue-tutorials.readthedocs.io/tutorials/beginner/transform.html). This lets users parallelize the execution of a single function by bringing it to Spark, Dask, or Ray. In the example below, the `map_letter_to_food()` function takes in a mapping and applies it on a column. This is just Pandas and Python so far (without Fugue).
 
 ```python
 import pandas as pd
 from typing import Dict
@@ -210,24 +212,26 @@
 
 FugueSQL backends:
 
 *   Pandas - FugueSQL can run on Pandas
 *   [Duckdb](https://github.com/duckdb/duckdb) - in-process SQL OLAP database management
 *   [dask-sql](https://github.com/dask-contrib/dask-sql) - SQL interface for Dask
 *   SparkSQL
-*   BigQuery
+*   [BigQuery](https://fugue-tutorials.readthedocs.io/tutorials/integrations/warehouses/bigquery.html)
+*   Trino
 
 
 Fugue is available as a backend or can integrate with the following projects:
 
 *   [WhyLogs](https://whylogs.readthedocs.io/en/latest/examples/integrations/Fugue_Profiling.html?highlight=fugue) - data profiling
 *   [PyCaret](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/pycaret.html) - low code machine learning
 *   [Nixtla](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/nixtla.html) - timeseries modelling
 *   [Prefect](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/prefect.html) - workflow orchestration
 *   [Pandera](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/pandera.html) - data validation
+*   [Datacompy (by Capital One)](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/datacompy.html) - comparing DataFrames
 
 Registered 3rd party extensions (majorly for Fugue SQL) include:
 
 *   [Pandas plot](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.html) - visualize data using matplotlib or plotly
 *   [Seaborn](https://seaborn.pydata.org/api.html) - visualize data using seaborn
 *   [WhyLogs](https://whylogs.readthedocs.io/en/latest/examples/integrations/Fugue_Profiling.html?highlight=fugue) - visualize data profiling
 *   [Vizzu](https://github.com/vizzuhq/ipyvizzu) - visualize data using ipyvizzu
@@ -240,16 +244,15 @@
 
 *   [How LyftLearn Democratizes Distributed Compute through Kubernetes Spark and Fugue](https://eng.lyft.com/how-lyftlearn-democratizes-distributed-compute-through-kubernetes-spark-and-fugue-c0875b97c3d9)
 *   [Clobotics - Large Scale Image Processing with Spark through Fugue](https://medium.com/fugue-project/large-scale-image-processing-with-spark-through-fugue-e510b9813da8)
 
 ### Mentioned Uses
 
 *   [Productionizing Data Science at Interos, Inc. (LinkedIn post by Anthony Holten)](https://www.linkedin.com/posts/anthony-holten_pandas-spark-dask-activity-7022628193983459328-QvcF)
-
-*   [Multiple Time Series Forecasting with Fugue & Nixtla at Bain & Company(LinkedIn post by Fahad Akbar)](https://www.linkedin.com/posts/fahadakbar_fugue-datascience-forecasting-activity-7041119034813124608-u08q?utm_source=share&utm_medium=member_desktop)
+*   [Multiple Time Series Forecasting with Fugue & Nixtla at Bain & Company (LinkedIn post by Fahad Akbar)](https://www.linkedin.com/posts/fahadakbar_fugue-datascience-forecasting-activity-7041119034813124608-u08q?utm_source=share&utm_medium=member_desktop)
 
 ## Further Resources
 
 View some of our latest conferences presentations and content. For a more complete list, check the [Content](https://fugue-tutorials.readthedocs.io/tutorials/resources/content.html) page in the tutorials.
 
 ### Blogs
```

### Comparing `fugue-0.8.4.dev2/fugue/__init__.py` & `fugue-0.8.5.dev1/fugue/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/_utils/display.py` & `fugue-0.8.5.dev1/fugue/_utils/display.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/_utils/exception.py` & `fugue-0.8.5.dev1/fugue/_utils/exception.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/_utils/interfaceless.py` & `fugue-0.8.5.dev1/fugue/_utils/interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/_utils/io.py` & `fugue-0.8.5.dev1/fugue/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/api.py` & `fugue-0.8.5.dev1/fugue/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/bag/array_bag.py` & `fugue-0.8.5.dev1/fugue/bag/array_bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/bag/bag.py` & `fugue-0.8.5.dev1/fugue/bag/bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/collections/partition.py` & `fugue-0.8.5.dev1/fugue/collections/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/collections/sql.py` & `fugue-0.8.5.dev1/fugue/collections/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from logging import Logger
 from typing import Any, Callable, Dict, Iterable, Optional, Tuple, Union
 from uuid import uuid4
 
 from triad import to_uuid
 
 from fugue._utils.registry import fugue_plugin
-import sqlglot
+from fugue._utils.misc import import_fsql_dependency
 
 _TEMP_TABLE_EXPR_PREFIX = "<tmpdf:"
 _TEMP_TABLE_EXPR_SUFFIX = ">"
 
 
 class TempTableName:
     """Generating a temporary, random and globaly unique table name"""
@@ -34,14 +34,16 @@
     :return: the transpiled SQL
     """
     if (
         from_dialect is not None
         and to_dialect is not None
         and from_dialect != to_dialect
     ):
+        sqlglot = import_fsql_dependency("sqlglot")
+
         return " ".join(sqlglot.transpile(raw, read=from_dialect, write=to_dialect))
     else:
         return raw
 
 
 class StructuredRawSQL:
     """The Raw SQL object containing table references and dialect information.
```

### Comparing `fugue-0.8.4.dev2/fugue/collections/yielded.py` & `fugue-0.8.5.dev1/fugue/collections/yielded.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/column/expressions.py` & `fugue-0.8.5.dev1/fugue/column/expressions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/column/functions.py` & `fugue-0.8.5.dev1/fugue/column/functions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/column/sql.py` & `fugue-0.8.5.dev1/fugue/column/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/constants.py` & `fugue-0.8.5.dev1/fugue/constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataframe/__init__.py` & `fugue-0.8.5.dev1/fugue/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataframe/api.py` & `fugue-0.8.5.dev1/fugue/dataframe/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataframe/array_dataframe.py` & `fugue-0.8.5.dev1/fugue/dataframe/array_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataframe/arrow_dataframe.py` & `fugue-0.8.5.dev1/fugue/dataframe/arrow_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataframe/dataframe.py` & `fugue-0.8.5.dev1/fugue/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataframe/dataframe_iterable_dataframe.py` & `fugue-0.8.5.dev1/fugue/dataframe/dataframe_iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataframe/dataframes.py` & `fugue-0.8.5.dev1/fugue/dataframe/dataframes.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataframe/function_wrapper.py` & `fugue-0.8.5.dev1/fugue/dataframe/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataframe/iterable_dataframe.py` & `fugue-0.8.5.dev1/fugue/dataframe/iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataframe/pandas_dataframe.py` & `fugue-0.8.5.dev1/fugue/dataframe/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataframe/utils.py` & `fugue-0.8.5.dev1/fugue/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataset/api.py` & `fugue-0.8.5.dev1/fugue/dataset/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dataset/dataset.py` & `fugue-0.8.5.dev1/fugue/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/dev.py` & `fugue-0.8.5.dev1/fugue/dev.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/exceptions.py` & `fugue-0.8.5.dev1/fugue/exceptions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/execution/api.py` & `fugue-0.8.5.dev1/fugue/execution/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/execution/execution_engine.py` & `fugue-0.8.5.dev1/fugue/execution/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/execution/factory.py` & `fugue-0.8.5.dev1/fugue/execution/factory.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/execution/native_execution_engine.py` & `fugue-0.8.5.dev1/fugue/execution/native_execution_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 import os
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 import pandas as pd
-from qpd_pandas import run_sql_on_pandas
-from qpd_pandas.engine import PandasUtils
 from triad import Schema
 from triad.collections.dict import IndexedOrderedDict
 from triad.collections.fs import FileSystem
 from triad.utils.assertion import assert_or_throw
+from triad.utils.pandas_like import PandasUtils
 
 from fugue._utils.io import load_df, save_df
+from fugue._utils.misc import import_fsql_dependency
 from fugue.collections.partition import (
     PartitionCursor,
     PartitionSpec,
     parse_presort_exp,
 )
 from fugue.collections.sql import StructuredRawSQL
 from fugue.dataframe import (
@@ -51,18 +51,20 @@
         return _to_native_execution_engine_df(df, schema)
 
     @property
     def is_distributed(self) -> bool:
         return False
 
     def select(self, dfs: DataFrames, statement: StructuredRawSQL) -> DataFrame:
+        qpd_pandas = import_fsql_dependency("qpd_pandas")
+
         _dfs, _sql = self.encode(dfs, statement)
         _dd = {k: self.to_df(v).as_pandas() for k, v in _dfs.items()}  # type: ignore
 
-        df = run_sql_on_pandas(_sql, _dd, ignore_case=True)
+        df = qpd_pandas.run_sql_on_pandas(_sql, _dd, ignore_case=True)
         return self.to_df(df)
 
 
 class PandasMapEngine(MapEngine):
     @property
     def execution_engine_constraint(self) -> Type[ExecutionEngine]:
         return NativeExecutionEngine
```

### Comparing `fugue-0.8.4.dev2/fugue/extensions/__init__.py` & `fugue-0.8.5.dev1/fugue/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/_builtins/__init__.py` & `fugue-0.8.5.dev1/fugue/extensions/_builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/_builtins/creators.py` & `fugue-0.8.5.dev1/fugue/extensions/_builtins/creators.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/_builtins/outputters.py` & `fugue-0.8.5.dev1/fugue/extensions/_builtins/outputters.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/_builtins/processors.py` & `fugue-0.8.5.dev1/fugue/extensions/_builtins/processors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/_utils.py` & `fugue-0.8.5.dev1/fugue/extensions/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/context.py` & `fugue-0.8.5.dev1/fugue/extensions/context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/creator/convert.py` & `fugue-0.8.5.dev1/fugue/extensions/creator/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/creator/creator.py` & `fugue-0.8.5.dev1/fugue/extensions/creator/creator.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/outputter/convert.py` & `fugue-0.8.5.dev1/fugue/extensions/outputter/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/outputter/outputter.py` & `fugue-0.8.5.dev1/fugue/extensions/outputter/outputter.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/processor/convert.py` & `fugue-0.8.5.dev1/fugue/extensions/processor/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/processor/processor.py` & `fugue-0.8.5.dev1/fugue/extensions/processor/processor.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/transformer/convert.py` & `fugue-0.8.5.dev1/fugue/extensions/transformer/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/extensions/transformer/transformer.py` & `fugue-0.8.5.dev1/fugue/extensions/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/plugins.py` & `fugue-0.8.5.dev1/fugue/plugins.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/registry.py` & `fugue-0.8.5.dev1/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/rpc/base.py` & `fugue-0.8.5.dev1/fugue/rpc/base.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/rpc/flask.py` & `fugue-0.8.5.dev1/fugue/rpc/flask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/sql/_utils.py` & `fugue-0.8.5.dev1/fugue/sql/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import re
 from typing import Any, Dict, Optional
 
-import jinja2
-from jinja2 import Template
 from triad import assert_or_throw
 
 from ..collections.yielded import Yielded
 from ..exceptions import FugueSQLError
 from ..workflow.workflow import FugueWorkflow, WorkflowDataFrame
 
 MATCH_QUOTED_STRING = r"([\"'])(({|%|})*)\1"
@@ -14,14 +12,17 @@
 
 def fill_sql_template(sql: str, params: Dict[str, Any]):
     """Prepare string to be executed, inserts params into sql template
     ---
     :param sql: jinja compatible template
     :param params: params to be inserted into template
     """
+    import jinja2
+    from jinja2 import Template
+
     try:
         if "self" in params:
             params = {k: v for k, v in params.items() if k != "self"}
         single_quote_pattern = "'{{% raw %}}{}{{% endraw %}}'"
         double_quote_pattern = '"{{% raw %}}{}{{% endraw %}}"'
         new_sql = re.sub(
             MATCH_QUOTED_STRING,
```

### Comparing `fugue-0.8.4.dev2/fugue/sql/_visitors.py` & `fugue-0.8.5.dev1/fugue/sql/_visitors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/sql/api.py` & `fugue-0.8.5.dev1/fugue/sql/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/sql/workflow.py` & `fugue-0.8.5.dev1/fugue/sql/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from builtins import isinstance
 from typing import Any, Dict, Tuple
 
-from fugue_sql_antlr import FugueSQLParser
 from triad.utils.assertion import assert_or_throw
 from triad.utils.convert import get_caller_global_local_vars
 
+from fugue._utils.misc import import_fsql_dependency
+
 from ..collections.yielded import Yielded
 from ..constants import FUGUE_CONF_SQL_DIALECT, FUGUE_CONF_SQL_IGNORE_CASE
 from ..dataframe.api import is_df
 from ..dataframe.dataframe import DataFrame
 from ..workflow.workflow import FugueWorkflow, WorkflowDataFrame, WorkflowDataFrames
 from ._utils import LazyWorkflowDataFrame, fill_sql_template
-from ._visitors import FugueSQLHooks, _Extensions
 
 
 class FugueSQLWorkflow(FugueWorkflow):
     """Fugue workflow that supports Fugue SQL. Please read |FugueSQLTutorial|."""
 
     def __init__(self, compile_conf: Any = None):
         super().__init__(compile_conf)
@@ -33,14 +32,18 @@
         for k, v in variables.items():
             if isinstance(v, WorkflowDataFrame) and v.workflow is self:
                 self._sql_vars[k] = v
 
     def _sql(
         self, code: str, *args: Any, **kwargs: Any
     ) -> Dict[str, Tuple[WorkflowDataFrame, WorkflowDataFrames, LazyWorkflowDataFrame]]:
+        FugueSQLParser = import_fsql_dependency("fugue_sql_antlr").FugueSQLParser
+
+        from ._visitors import FugueSQLHooks, _Extensions
+
         # TODO: move dict construction to triad
         params: Dict[str, Any] = {}
         for a in args:
             assert_or_throw(
                 isinstance(a, Dict), lambda: f"args can only have dict: {a}"
             )
             params.update(a)
```

### Comparing `fugue-0.8.4.dev2/fugue/workflow/_checkpoint.py` & `fugue-0.8.5.dev1/fugue/workflow/_checkpoint.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/workflow/_tasks.py` & `fugue-0.8.5.dev1/fugue/workflow/_tasks.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/workflow/_workflow_context.py` & `fugue-0.8.5.dev1/fugue/workflow/_workflow_context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/workflow/api.py` & `fugue-0.8.5.dev1/fugue/workflow/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/workflow/module.py` & `fugue-0.8.5.dev1/fugue/workflow/module.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue/workflow/workflow.py` & `fugue-0.8.5.dev1/fugue/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue.egg-info/PKG-INFO` & `fugue-0.8.5.dev1/fugue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.4.dev2
+Version: 0.8.5.dev1
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
         
@@ -23,14 +23,16 @@
         **Fugue is a unified interface for distributed computing that lets users execute Python, Pandas, and SQL code on Spark, Dask, and Ray with minimal rewrites**.
         
         Fugue is most commonly used for:
         
         *   **Parallelizing or scaling existing Python and Pandas code** by bringing it to Spark, Dask, or Ray with minimal rewrites.
         *   Using [FugueSQL](https://fugue-tutorials.readthedocs.io/tutorials/quick_look/ten_minutes_sql.html) to **define end-to-end workflows** on top of Pandas, Spark, and Dask DataFrames. FugueSQL is an enhanced SQL interface that can invoke Python code.
         
+        To see how Fugue compares to other frameworks like dbt, Arrow, Ibis, PySpark Pandas, see the [comparisons](https://fugue-tutorials.readthedocs.io/#how-does-fugue-compare-to)
+        
         ## [Fugue API](https://fugue-tutorials.readthedocs.io/tutorials/quick_look/ten_minutes.html)
         
         The Fugue API is a collection of functions that are capable of running on Pandas, Spark, Dask, and Ray. The simplest way to use Fugue is the [`transform()` function](https://fugue-tutorials.readthedocs.io/tutorials/beginner/transform.html). This lets users parallelize the execution of a single function by bringing it to Spark, Dask, or Ray. In the example below, the `map_letter_to_food()` function takes in a mapping and applies it on a column. This is just Pandas and Python so far (without Fugue).
         
         ```python
         import pandas as pd
         from typing import Dict
@@ -218,24 +220,26 @@
         
         FugueSQL backends:
         
         *   Pandas - FugueSQL can run on Pandas
         *   [Duckdb](https://github.com/duckdb/duckdb) - in-process SQL OLAP database management
         *   [dask-sql](https://github.com/dask-contrib/dask-sql) - SQL interface for Dask
         *   SparkSQL
-        *   BigQuery
+        *   [BigQuery](https://fugue-tutorials.readthedocs.io/tutorials/integrations/warehouses/bigquery.html)
+        *   Trino
         
         
         Fugue is available as a backend or can integrate with the following projects:
         
         *   [WhyLogs](https://whylogs.readthedocs.io/en/latest/examples/integrations/Fugue_Profiling.html?highlight=fugue) - data profiling
         *   [PyCaret](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/pycaret.html) - low code machine learning
         *   [Nixtla](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/nixtla.html) - timeseries modelling
         *   [Prefect](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/prefect.html) - workflow orchestration
         *   [Pandera](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/pandera.html) - data validation
+        *   [Datacompy (by Capital One)](https://fugue-tutorials.readthedocs.io/tutorials/integrations/ecosystem/datacompy.html) - comparing DataFrames
         
         Registered 3rd party extensions (majorly for Fugue SQL) include:
         
         *   [Pandas plot](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.html) - visualize data using matplotlib or plotly
         *   [Seaborn](https://seaborn.pydata.org/api.html) - visualize data using seaborn
         *   [WhyLogs](https://whylogs.readthedocs.io/en/latest/examples/integrations/Fugue_Profiling.html?highlight=fugue) - visualize data profiling
         *   [Vizzu](https://github.com/vizzuhq/ipyvizzu) - visualize data using ipyvizzu
@@ -248,16 +252,15 @@
         
         *   [How LyftLearn Democratizes Distributed Compute through Kubernetes Spark and Fugue](https://eng.lyft.com/how-lyftlearn-democratizes-distributed-compute-through-kubernetes-spark-and-fugue-c0875b97c3d9)
         *   [Clobotics - Large Scale Image Processing with Spark through Fugue](https://medium.com/fugue-project/large-scale-image-processing-with-spark-through-fugue-e510b9813da8)
         
         ### Mentioned Uses
         
         *   [Productionizing Data Science at Interos, Inc. (LinkedIn post by Anthony Holten)](https://www.linkedin.com/posts/anthony-holten_pandas-spark-dask-activity-7022628193983459328-QvcF)
-        
-        *   [Multiple Time Series Forecasting with Fugue & Nixtla at Bain & Company(LinkedIn post by Fahad Akbar)](https://www.linkedin.com/posts/fahadakbar_fugue-datascience-forecasting-activity-7041119034813124608-u08q?utm_source=share&utm_medium=member_desktop)
+        *   [Multiple Time Series Forecasting with Fugue & Nixtla at Bain & Company (LinkedIn post by Fahad Akbar)](https://www.linkedin.com/posts/fahadakbar_fugue-datascience-forecasting-activity-7041119034813124608-u08q?utm_source=share&utm_medium=member_desktop)
         
         ## Further Resources
         
         View some of our latest conferences presentations and content. For a more complete list, check the [Content](https://fugue-tutorials.readthedocs.io/tutorials/resources/content.html) page in the tutorials.
         
         ### Blogs
         
@@ -281,14 +284,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: sql
 Provides-Extra: cpp_sql_parser
 Provides-Extra: spark
 Provides-Extra: dask
 Provides-Extra: ray
 Provides-Extra: duckdb
 Provides-Extra: polars
 Provides-Extra: ibis
```

### Comparing `fugue-0.8.4.dev2/fugue_contrib/seaborn/__init__.py` & `fugue-0.8.5.dev1/fugue_contrib/seaborn/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_contrib/viz/__init__.py` & `fugue-0.8.5.dev1/fugue_contrib/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_contrib/viz/_ext.py` & `fugue-0.8.5.dev1/fugue_contrib/viz/_ext.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_dask/_io.py` & `fugue-0.8.5.dev1/fugue_dask/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_dask/_utils.py` & `fugue-0.8.5.dev1/fugue_dask/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, Optional
 
 import dask.dataframe as pd
 import numpy as np
 import pandas
 import pyarrow as pa
 from dask.distributed import Client, get_client
-from qpd_dask.engine import DaskUtils as DaskUtilsBase
+from triad.utils.pandas_like import PandasLikeUtils
 from triad.utils.pyarrow import to_pandas_dtype, to_single_pandas_dtype
 
 import fugue.api as fa
 from fugue.constants import FUGUE_CONF_DEFAULT_PARTITIONS
 
 from ._constants import FUGUE_DASK_CONF_DEFAULT_PARTITIONS
 
@@ -19,15 +19,18 @@
     n = conf.get(
         FUGUE_DASK_CONF_DEFAULT_PARTITIONS,
         conf.get(FUGUE_CONF_DEFAULT_PARTITIONS, -1),
     )
     return n if n > 0 else fa.get_current_parallelism() * 2
 
 
-class DaskUtils(DaskUtilsBase):
+class DaskUtils(PandasLikeUtils[pd.DataFrame, pd.Series]):
+    def concat_dfs(self, *dfs: pd.DataFrame) -> pd.DataFrame:
+        return pd.concat(list(dfs))
+
     def get_or_create_client(self, client: Optional[Client] = None):
         if client is not None:
             return client
         try:
             return get_client()
         except ValueError:
             return Client(processes=True)
```

### Comparing `fugue-0.8.4.dev2/fugue_dask/dataframe.py` & `fugue-0.8.5.dev1/fugue_dask/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_dask/execution_engine.py` & `fugue-0.8.5.dev1/fugue_dask/execution_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 import os
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 import dask.dataframe as dd
 import pandas as pd
 from distributed import Client
-from qpd_dask import run_sql_on_dask
 from triad.collections import Schema
 from triad.collections.dict import IndexedOrderedDict, ParamDict
 from triad.collections.fs import FileSystem
 from triad.utils.assertion import assert_or_throw
 from triad.utils.hash import to_uuid
 from triad.utils.threading import RunOnce
 
 from fugue import StructuredRawSQL
+from fugue._utils.misc import import_fsql_dependency
 from fugue.collections.partition import (
     PartitionCursor,
     PartitionSpec,
     parse_presort_exp,
 )
 from fugue.constants import KEYWORD_PARALLELISM, KEYWORD_ROWCOUNT
 from fugue.dataframe import (
@@ -49,17 +49,19 @@
         return to_dask_engine_df(df, schema)
 
     @property
     def is_distributed(self) -> bool:
         return True
 
     def select(self, dfs: DataFrames, statement: StructuredRawSQL) -> DataFrame:
+        qpd_dask = import_fsql_dependency("qpd_dask")
+
         _dfs, _sql = self.encode(dfs, statement)
         dask_dfs = {k: self.to_df(v).native for k, v in _dfs.items()}  # type: ignore
-        df = run_sql_on_dask(_sql, dask_dfs, ignore_case=True)
+        df = qpd_dask.run_sql_on_dask(_sql, dask_dfs, ignore_case=True)
         return DaskDataFrame(df)
 
 
 class DaskMapEngine(MapEngine):
     @property
     def execution_engine_constraint(self) -> Type[ExecutionEngine]:
         return DaskExecutionEngine
```

### Comparing `fugue-0.8.4.dev2/fugue_dask/ibis_engine.py` & `fugue-0.8.5.dev1/fugue_dask/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_dask/registry.py` & `fugue-0.8.5.dev1/fugue_dask/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_duckdb/_io.py` & `fugue-0.8.5.dev1/fugue_duckdb/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_duckdb/_utils.py` & `fugue-0.8.5.dev1/fugue_duckdb/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,19 @@
     "UINTEGER": pa.uint32(),
     "USMALLINT": pa.uint16(),
     "UTINYINT": pa.uint8(),
     "VARCHAR": pa.string(),
     "TIME": pa.time32("ms"),
 }
 
-_PA_TYPES_TO_DUCK: Dict[pa.DataType, str] = {v: k for k, v in _DUCK_TYPES_TO_PA.items()}
+_PA_TYPES_TO_DUCK: Dict[pa.DataType, str] = {
+    v: k
+    for k, v in list(_DUCK_TYPES_TO_PA.items())
+    + [("VARCHAR", pa.large_string()), ("BLOB", pa.large_binary())]
+}
 
 
 def encode_column_name(name: str) -> str:
     return quote_name(name, quote='"')
 
 
 def encode_column_names(names: Iterable[str]) -> Iterable[str]:
@@ -90,16 +94,17 @@
         if pa.types.is_decimal(tp):
             return f"DECIMAL({tp.precision}, {tp.scale})"
         return _PA_TYPES_TO_DUCK[tp]
     except Exception:  # pragma: no cover
         raise ValueError(f"can't convert {tp} to DuckDB data type")
 
 
-def to_pa_type(duck_type: str) -> pa.DataType:
+def to_pa_type(duck_type_raw: Any) -> pa.DataType:
     try:
+        duck_type = str(duck_type_raw)  # for duckdb >= 0.8.0
         if duck_type.endswith("[]"):
             return pa.list_(to_pa_type(duck_type[:-2]))
         p = duck_type.find("(")
         if p > 0:
             tp = duck_type[:p]
             if tp == "STRUCT":
                 fields = [
```

### Comparing `fugue-0.8.4.dev2/fugue_duckdb/dask.py` & `fugue-0.8.5.dev1/fugue_duckdb/dask.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     def to_df(self, df: Any, schema: Any = None) -> DuckDataFrame:
         if isinstance(df, (dd.DataFrame, DaskDataFrame)):
             ddf = self._to_dask_df(df, schema)
             if all(not pa.types.is_nested(f.type) for f in ddf.schema.fields):
                 res = DuckDataFrame(self.connection.from_df(ddf.as_pandas()))
             else:
                 res = DuckDataFrame(
-                    duckdb.arrow(ddf.as_arrow(), connection=self.connection)
+                    duckdb.from_arrow(ddf.as_arrow(), connection=self.connection)
                 )
             if ddf.has_metadata:  # pragma: no cover
                 res.reset_metadata(ddf.metadata)
             return res
         return super().to_df(df, schema)
 
     def repartition(self, df: DataFrame, partition_spec: PartitionSpec) -> DataFrame:
```

### Comparing `fugue-0.8.4.dev2/fugue_duckdb/dataframe.py` & `fugue-0.8.5.dev1/fugue_duckdb/dataframe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 from typing import Any, Dict, Iterable, List, Optional
 
 import pandas as pd
 import pyarrow as pa
 from duckdb import DuckDBPyRelation
 from triad import Schema
+from triad.utils.pyarrow import LARGE_TYPES_REPLACEMENT, replace_types_in_table
 
 from fugue import ArrayDataFrame, ArrowDataFrame, DataFrame, LocalBoundedDataFrame
 from fugue.exceptions import FugueDataFrameOperationError, FugueDatasetEmptyError
 from fugue.plugins import (
+    as_arrow,
     as_fugue_dataset,
     as_local_bounded,
     get_column_names,
     get_num_partitions,
+    get_schema,
     is_df,
 )
 
 from ._utils import encode_column_name, to_duck_type, to_pa_type
 
 
 class DuckDataFrame(LocalBoundedDataFrame):
     """DataFrame that wraps DuckDB ``DuckDBPyRelation``.
 
     :param rel: ``DuckDBPyRelation`` object
     """
 
     def __init__(self, rel: DuckDBPyRelation):
         self._rel = rel
-        super().__init__(schema=self._get_schema)
-
-    def _get_schema(self) -> Schema:
-        return Schema(
-            [
-                pa.field(x, to_pa_type(y))
-                for x, y in zip(self._rel.columns, self._rel.types)
-            ]
-        )
+        super().__init__(schema=lambda: _duck_get_schema(self._rel))
 
     @property
     def alias(self) -> str:
         return "_" + str(id(self._rel))  # DuckDBPyRelation.alias is not always unique
 
     @property
     def native(self) -> DuckDBPyRelation:
@@ -94,15 +89,15 @@
                 fields.append(
                     f"CAST({encode_column_name(f1.name)} AS {tp}) "
                     f"AS {encode_column_name(f1.name)}"
                 )
         return DuckDataFrame(self._rel.project(", ".join(fields)))
 
     def as_arrow(self, type_safe: bool = False) -> pa.Table:
-        return self._rel.arrow()
+        return _duck_as_arrow(self._rel)
 
     def as_pandas(self) -> pd.DataFrame:
         if any(pa.types.is_nested(f.type) for f in self.schema.fields):
             # Duckdb has issue to directly convert nested types to pandas
             return ArrowDataFrame(self.as_arrow()).as_pandas()
         return self._rel.to_df()
 
@@ -165,14 +160,26 @@
 
 
 @as_local_bounded.candidate(lambda df: isinstance(df, DuckDBPyRelation))
 def _duck_as_local(df: DuckDBPyRelation) -> DuckDBPyRelation:
     return df
 
 
+@as_arrow.candidate(lambda df: isinstance(df, DuckDBPyRelation))
+def _duck_as_arrow(df: DuckDBPyRelation) -> pa.Table:
+    _df = df.arrow()
+    _df = replace_types_in_table(_df, LARGE_TYPES_REPLACEMENT, recursive=True)
+    return _df
+
+
+@get_schema.candidate(lambda df: isinstance(df, DuckDBPyRelation))
+def _duck_get_schema(df: DuckDBPyRelation) -> Schema:
+    return Schema([pa.field(x, to_pa_type(y)) for x, y in zip(df.columns, df.types)])
+
+
 @get_column_names.candidate(lambda df: isinstance(df, DuckDBPyRelation))
 def _get_duckdb_columns(df: DuckDBPyRelation) -> List[Any]:
     return list(df.columns)
 
 
 def _assert_no_missing(df: DuckDBPyRelation, columns: Iterable[Any]) -> None:
     missing = set(columns) - set(df.columns)
```

### Comparing `fugue-0.8.4.dev2/fugue_duckdb/execution_engine.py` & `fugue-0.8.5.dev1/fugue_duckdb/execution_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from ._io import DuckDBIO
 from ._utils import (
     encode_column_name,
     encode_column_names,
     encode_schema_names,
     encode_value_to_expr,
 )
-from .dataframe import DuckDataFrame
+from .dataframe import DuckDataFrame, _duck_as_arrow
 
 _FUGUE_DUCKDB_PRAGMA_CONFIG_PREFIX = "fugue.duckdb.pragma."
 _FUGUE_DUCKDB_EXTENSIONS = "fugue.duckdb.extensions"
 
 
 class DuckDBEngine(SQLEngine):
     """DuckDB SQL backend implementation.
@@ -104,16 +104,16 @@
         result = self.execution_engine.connection.query(query)  # type: ignore
         return DuckDataFrame(result)
 
     def _other_select(self, dfs: DataFrames, statement: str) -> DataFrame:
         conn = duckdb.connect()
         try:
             for k, v in dfs.items():
-                duckdb.arrow(v.as_arrow(), connection=conn).create_view(k)
-            return ArrowDataFrame(conn.execute(statement).arrow())
+                duckdb.from_arrow(v.as_arrow(), connection=conn).create_view(k)
+            return ArrowDataFrame(_duck_as_arrow(conn.execute(statement)))
         finally:
             conn.close()
 
     def _get_table(self, table: str) -> Optional[Dict[str, Any]]:
         if isinstance(self.execution_engine, DuckExecutionEngine):
             # TODO: this is over simplified
             con = self.execution_engine.connection
@@ -225,15 +225,15 @@
         df: DataFrame,
         lazy: bool = False,
         **kwargs: Any,
     ) -> DataFrame:
         # TODO: we should create DuckDB table, but it has bugs, so can't use by 0.3.1
         if isinstance(df, DuckDataFrame):
             # materialize
-            res: DataFrame = ArrowDataFrame(df.native.arrow())
+            res: DataFrame = ArrowDataFrame(df.as_arrow())
         else:
             res = self.to_df(df)
         res.reset_metadata(df.metadata)
         return res
 
     def join(
         self,
@@ -536,20 +536,22 @@
             assert_or_throw(
                 schema is None,
                 ValueError("schema must be None when df is a DataFrame"),
             )
             if isinstance(df, DuckDataFrame):
                 return df
             rdf = DuckDataFrame(
-                duckdb.arrow(df.as_arrow(), connection=engine.connection)
+                duckdb.from_arrow(df.as_arrow(), connection=engine.connection)
             )
             rdf.reset_metadata(df.metadata if df.has_metadata else None)
             return rdf
         tdf = ArrowDataFrame(df, schema)
-        return DuckDataFrame(duckdb.arrow(tdf.native, connection=engine.connection))
+        return DuckDataFrame(
+            duckdb.from_arrow(tdf.native, connection=engine.connection)
+        )
 
     res = _gen_duck()
     if create_view:
         with engine._context_lock:
             if res.alias not in engine._registered_dfs:
                 res.native.create_view(res.alias, replace=True)
                 # must hold the reference of the df so the id will not be reused
```

### Comparing `fugue-0.8.4.dev2/fugue_duckdb/ibis_engine.py` & `fugue-0.8.5.dev1/fugue_duckdb/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_duckdb/registry.py` & `fugue-0.8.5.dev1/fugue_duckdb/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ibis/_utils.py` & `fugue-0.8.5.dev1/fugue_ibis/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ibis/dataframe.py` & `fugue-0.8.5.dev1/fugue_ibis/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ibis/execution/ibis_engine.py` & `fugue-0.8.5.dev1/fugue_ibis/execution/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ibis/execution/pandas_backend.py` & `fugue-0.8.5.dev1/fugue_ibis/execution/pandas_backend.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ibis/execution_engine.py` & `fugue-0.8.5.dev1/fugue_ibis/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ibis/extensions.py` & `fugue-0.8.5.dev1/fugue_ibis/extensions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_notebook/__init__.py` & `fugue-0.8.5.dev1/fugue_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_notebook/env.py` & `fugue-0.8.5.dev1/fugue_notebook/env.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_notebook/nbextension/main.js` & `fugue-0.8.5.dev1/fugue_notebook/nbextension/main.js`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_polars/polars_dataframe.py` & `fugue-0.8.5.dev1/fugue_polars/polars_dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 
 import pandas as pd
 import polars as pl
 import pyarrow as pa
 from triad.collections.schema import Schema
 from triad.exceptions import InvalidOperationError
 from triad.utils.assertion import assert_or_throw
+from triad.utils.pyarrow import (
+    LARGE_TYPES_REPLACEMENT,
+    replace_types_in_schema,
+    replace_types_in_table,
+)
 
 from fugue import ArrowDataFrame
 from fugue.api import (
+    as_arrow,
     drop_columns,
     get_column_names,
     get_schema,
     is_df,
     rename,
     select_columns,
 )
@@ -24,15 +30,15 @@
     get_num_partitions,
     is_bounded,
     is_empty,
     is_local,
 )
 from fugue.exceptions import FugueDataFrameOperationError
 
-from ._utils import build_empty_pl, pl_as_arrow, to_schema
+from ._utils import build_empty_pl
 
 
 class PolarsDataFrame(LocalBoundedDataFrame):
     """DataFrame that wraps :func:`pyarrow.Table <pa:pyarrow.table>`. Please also read
     |DataFrameTutorial| to understand this Fugue concept
 
     :param df: polars DataFrame or None, defaults to None
@@ -51,15 +57,15 @@
             return
         else:
             assert_or_throw(
                 schema is None,
                 InvalidOperationError("can't reset schema for pl.DataFrame"),
             )
             self._native = df
-            super().__init__(to_schema(df))
+            super().__init__(_get_pl_schema(df))
 
     @property
     def native(self) -> pl.DataFrame:
         """:func:`pyarrow.Table <pa:pyarrow.table>`"""
         return self._native
 
     def native_as_df(self) -> pl.DataFrame:
@@ -103,51 +109,58 @@
         return PolarsDataFrame(_rename_pl_dataframe(self.native, columns))
 
     def alter_columns(self, columns: Any) -> DataFrame:
         adf = ArrowDataFrame(self.as_arrow()).alter_columns(columns)
         return PolarsDataFrame(pl.from_arrow(adf.native))
 
     def as_arrow(self, type_safe: bool = False) -> pa.Table:
-        return pl_as_arrow(self.native)
+        return _pl_as_arrow(self.native)
 
     def as_array(
         self, columns: Optional[List[str]] = None, type_safe: bool = False
     ) -> List[Any]:
         tdf = self.native
         if columns is not None:
             tdf = tdf.select(columns)
         return [list(row) for row in tdf.rows()]
 
     def as_array_iterable(
         self, columns: Optional[List[str]] = None, type_safe: bool = False
     ) -> Iterable[Any]:
         if not self.empty:
-            yield from ArrowDataFrame(pl_as_arrow(self.native)).as_array_iterable(
+            yield from ArrowDataFrame(_pl_as_arrow(self.native)).as_array_iterable(
                 columns=columns
             )
 
     def as_dict_iterable(
         self, columns: Optional[List[str]] = None
     ) -> Iterable[Dict[str, Any]]:
         if not self.empty:
-            yield from ArrowDataFrame(pl_as_arrow(self.native)).as_dict_iterable(
+            yield from ArrowDataFrame(_pl_as_arrow(self.native)).as_dict_iterable(
                 columns=columns
             )
 
 
 @as_local.candidate(lambda df: isinstance(df, pl.DataFrame))
 def _pl_as_local(df: pl.DataFrame) -> pl.DataFrame:
     return df
 
 
 @as_local_bounded.candidate(lambda df: isinstance(df, pl.DataFrame))
 def _pl_as_local_bounded(df: pl.DataFrame) -> pl.DataFrame:
     return df
 
 
+@as_arrow.candidate(lambda df: isinstance(df, pl.DataFrame))
+def _pl_as_arrow(df: pl.DataFrame) -> pa.Table:
+    adf = df.to_arrow()
+    adf = replace_types_in_table(adf, LARGE_TYPES_REPLACEMENT)
+    return adf
+
+
 @is_df.candidate(lambda df: isinstance(df, pl.DataFrame))
 def _pl_is_df(df: pl.DataFrame) -> bool:
     return True
 
 
 @count.candidate(lambda df: isinstance(df, pl.DataFrame))
 def _pl_count(df: pl.DataFrame) -> int:
@@ -177,15 +190,17 @@
 @get_column_names.candidate(lambda df: isinstance(df, pl.DataFrame))
 def _get_pl_columns(df: pl.DataFrame) -> List[Any]:
     return list(df.schema.keys())
 
 
 @get_schema.candidate(lambda df: isinstance(df, pl.DataFrame))
 def _get_pl_schema(df: pl.DataFrame) -> Schema:
-    return to_schema(df)
+    adf = df.to_arrow()
+    schema = replace_types_in_schema(adf.schema, LARGE_TYPES_REPLACEMENT)
+    return Schema(schema)
 
 
 @rename.candidate(lambda df, *args, **kwargs: isinstance(df, pl.DataFrame))
 def _rename_pl_dataframe(df: pl.DataFrame, columns: Dict[str, Any]) -> pl.DataFrame:
     if len(columns) == 0:
         return df
     assert_or_throw(
```

### Comparing `fugue-0.8.4.dev2/fugue_polars/registry.py` & `fugue-0.8.5.dev1/fugue_polars/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ray/_constants.py` & `fugue-0.8.5.dev1/fugue_ray/_constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ray/_utils/cluster.py` & `fugue-0.8.5.dev1/fugue_ray/_utils/cluster.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ray/_utils/dataframe.py` & `fugue-0.8.5.dev1/fugue_ray/_utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ray/_utils/io.py` & `fugue-0.8.5.dev1/fugue_ray/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ray/dataframe.py` & `fugue-0.8.5.dev1/fugue_ray/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ray/execution_engine.py` & `fugue-0.8.5.dev1/fugue_ray/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_ray/registry.py` & `fugue-0.8.5.dev1/fugue_ray/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_spark/_utils/convert.py` & `fugue-0.8.5.dev1/fugue_spark/_utils/convert.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,32 @@
+import pickle
 from typing import Any, Iterable, List, Tuple
 
-import cloudpickle
 import pandas as pd
 import pyarrow as pa
 import pyspark.sql as ps
 import pyspark.sql.types as pt
 from pyarrow.types import is_list, is_struct, is_timestamp
 from pyspark.sql.pandas.types import from_arrow_type, to_arrow_type
 from triad.collections import Schema
 from triad.utils.assertion import assert_arg_not_none, assert_or_throw
 from triad.utils.pyarrow import TRIAD_DEFAULT_TIMESTAMP
 from triad.utils.schema import quote_name
+
+import fugue.api as fa
+from fugue import DataFrame
+
 from .misc import is_spark_dataframe
 
+try:
+    from pyspark.sql.types import TimestampNTZType  # pylint: disable-all
+except ImportError:  # pragma: no cover
+    # pyspark < 3.2
+    from pyspark.sql.types import TimestampType as TimestampNTZType
+
 
 def to_spark_schema(obj: Any) -> pt.StructType:
     assert_arg_not_none(obj, "schema")
     if isinstance(obj, pt.StructType):
         return obj
     if is_spark_dataframe(obj):
         return obj.schema
@@ -104,28 +114,52 @@
     else:
         for row in rows:
             data = row.asDict(recursive=True)
             r = [data[n] for n in schema.names]
             yield r
 
 
+def to_spark_df(session: ps.SparkSession, df: Any, schema: Any = None) -> ps.DataFrame:
+    if schema is not None and not isinstance(schema, pt.StructType):
+        schema = to_spark_schema(schema)
+    if isinstance(df, pd.DataFrame):
+        if pd.__version__ >= "2" and session.version < "3.4":  # pragma: no cover
+            # pyspark < 3.4 does not support pandas 2 when doing
+            # createDataFrame, see this issue:
+            # https://stackoverflow.com/a/75926954/12309438
+            # this is a workaround with the cost of memory and speed.
+            if schema is None:
+                schema = to_spark_schema(fa.get_schema(df))
+            df = fa.as_fugue_df(df).as_array(type_safe=True)
+        return session.createDataFrame(df, schema=schema)
+    if isinstance(df, DataFrame):
+        if pd.__version__ >= "2" and session.version < "3.4":  # pragma: no cover
+            if schema is None:
+                schema = to_spark_schema(df.schema)
+            return session.createDataFrame(df.as_array(type_safe=True), schema=schema)
+        return session.createDataFrame(df.as_pandas(), schema=schema)
+    else:
+        return session.createDataFrame(df, schema=schema)
+
+
 def to_pandas(df: ps.DataFrame) -> pd.DataFrame:
     if pd.__version__ < "2" or not any(
-        isinstance(x.dataType, (pt.TimestampType, pt.TimestampNTZType))
+        isinstance(x.dataType, (pt.TimestampType, TimestampNTZType))
         for x in df.schema.fields
     ):
         return df.toPandas()
+    else:
 
-    def serialize(dfs):  # pragma: no cover
-        for df in dfs:
-            data = cloudpickle.dumps(df)
-            yield pd.DataFrame([[data]], columns=["data"])
+        def serialize(dfs):  # pragma: no cover
+            for df in dfs:
+                data = pickle.dumps(df)
+                yield pd.DataFrame([[data]], columns=["data"])
 
-    sdf = df.mapInPandas(serialize, schema="data binary")
-    return pd.concat(cloudpickle.loads(x.data) for x in sdf.collect())
+        sdf = df.mapInPandas(serialize, schema="data binary")
+        return pd.concat(pickle.loads(x.data) for x in sdf.collect())
 
 
 # TODO: the following function always set nullable to true,
 # but should we use field.nullable?
 def _to_arrow_type(dt: pt.DataType) -> pa.DataType:
     if isinstance(dt, pt.TimestampType):
         return TRIAD_DEFAULT_TIMESTAMP
```

### Comparing `fugue-0.8.4.dev2/fugue_spark/_utils/io.py` & `fugue-0.8.5.dev1/fugue_spark/_utils/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import pyspark.sql as ps
-from fugue.collections.partition import PartitionSpec
-from fugue.dataframe import DataFrame
-from fugue._utils.io import FileParser, save_df
-from fugue_spark.dataframe import SparkDataFrame
-from fugue_spark._utils.convert import to_schema, to_spark_schema
 from pyspark.sql import SparkSession
 from triad.collections import Schema
+from triad.collections.dict import ParamDict
 from triad.collections.fs import FileSystem
 from triad.utils.assertion import assert_or_throw
-from triad.collections.dict import ParamDict
+
+from fugue._utils.io import FileParser, save_df
+from fugue.collections.partition import PartitionSpec
+from fugue.dataframe import DataFrame
+from fugue_spark.dataframe import SparkDataFrame
+
+from .convert import to_schema, to_spark_schema
 
 
 class SparkIO(object):
     def __init__(self, spark_session: SparkSession, fs: FileSystem):
         self._session = spark_session
         self._fs = fs
         self._loads: Dict[str, Callable[..., DataFrame]] = {
```

### Comparing `fugue-0.8.4.dev2/fugue_spark/_utils/misc.py` & `fugue-0.8.5.dev1/fugue_spark/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_spark/_utils/partition.py` & `fugue-0.8.5.dev1/fugue_spark/_utils/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_spark/dataframe.py` & `fugue-0.8.5.dev1/fugue_spark/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_spark/execution_engine.py` & `fugue-0.8.5.dev1/fugue_spark/execution_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 )
 from fugue.dataframe.arrow_dataframe import _build_empty_arrow
 from fugue.dataframe.utils import get_join_schemas
 from fugue.exceptions import FugueDataFrameInitError
 from fugue.execution.execution_engine import ExecutionEngine, MapEngine, SQLEngine
 
 from ._constants import FUGUE_SPARK_CONF_USE_PANDAS_UDF, FUGUE_SPARK_DEFAULT_CONF
-from ._utils.convert import to_schema, to_spark_schema, to_type_safe_input
+from ._utils.convert import to_schema, to_spark_schema, to_type_safe_input, to_spark_df
 from ._utils.io import SparkIO
 from ._utils.misc import is_spark_connect as _is_spark_connect, is_spark_dataframe
 from ._utils.partition import even_repartition, hash_repartition, rand_repartition
 from .dataframe import SparkDataFrame
 
 _TO_SPARK_JOIN_MAP: Dict[str, str] = {
     "inner": "inner",
@@ -242,14 +242,15 @@
                         pdf = PandasDataFrame(
                             df.reset_index(drop=True),
                             input_schema,
                             pandas_df_wrapper=True,
                         )
                         if not cursor_set:
                             cursor.set(lambda: pdf.peek_array(), 0, 0)
+                            cursor_set = True
                         yield pdf
 
             input_df = IterablePandasDataFrame(get_dfs(), input_schema)
             if input_df.empty:
                 yield PandasDataFrame([], output_schema).as_pandas()
                 return
             if on_init_once is not None:
@@ -276,14 +277,15 @@
                             # be added with a timezong, this is to fix the issue
                             func = get_alter_func(
                                 adf.schema, input_schema.pa_schema, safe=False
                             )
                         pdf = ArrowDataFrame(func(adf))
                         if not cursor_set:
                             cursor.set(lambda: pdf.peek_array(), 0, 0)
+                            cursor_set = True
                         yield pdf
 
             input_df = IterableArrowDataFrame(get_dfs(), input_schema)
             if input_df.empty:
                 yield from _build_empty_arrow(output_schema).to_batches()
                 return
             if on_init_once is not None:
@@ -729,70 +731,57 @@
             if isinstance(df, DataFrame):
                 assert_or_throw(
                     schema is None,
                     ValueError("schema must be None when df is a DataFrame"),
                 )
                 if isinstance(df, SparkDataFrame):
                     return df
-                if isinstance(df, ArrowDataFrame):
-                    raw_df: Any = df.as_pandas()
-                    sdf = self.spark_session.createDataFrame(
-                        raw_df, to_spark_schema(df.schema)
-                    )
-                    return SparkDataFrame(sdf, df.schema)
                 if isinstance(df, (ArrayDataFrame, IterableDataFrame)):
                     adf = ArrowDataFrame(df.as_array(type_safe=False), df.schema)
-                    raw_df = adf.as_pandas()
-                    sdf = self.spark_session.createDataFrame(
-                        raw_df, to_spark_schema(df.schema)
-                    )
+                    sdf = to_spark_df(self.spark_session, adf, df.schema)
                     return SparkDataFrame(sdf, df.schema)
                 if any(pa.types.is_struct(t) for t in df.schema.types):
-                    sdf = self.spark_session.createDataFrame(
-                        df.as_array(type_safe=True), to_spark_schema(df.schema)
+                    sdf = to_spark_df(
+                        self.spark_session, df.as_array(type_safe=True), df.schema
                     )
                 else:
-                    sdf = self.spark_session.createDataFrame(
-                        df.as_pandas(), to_spark_schema(df.schema)
-                    )
+                    sdf = to_spark_df(self.spark_session, df, df.schema)
                 return SparkDataFrame(sdf, df.schema)
             if is_spark_dataframe(df):
                 return SparkDataFrame(df, None if schema is None else to_schema(schema))
             if isinstance(df, RDD):
                 assert_arg_not_none(schema, "schema")
-                sdf = self.spark_session.createDataFrame(df, to_spark_schema(schema))
+                sdf = to_spark_df(self.spark_session, df, schema)
                 return SparkDataFrame(sdf, to_schema(schema))
             if isinstance(df, pd.DataFrame):
                 if PD_UTILS.empty(df):
                     temp_schema = to_spark_schema(PD_UTILS.to_schema(df))
-                    sdf = self.spark_session.createDataFrame([], temp_schema)
+                    sdf = to_spark_df(self.spark_session, [], temp_schema)
                 else:
-                    sdf = self.spark_session.createDataFrame(df)
+                    sdf = to_spark_df(self.spark_session, df)
                 return SparkDataFrame(sdf, schema)
 
             # use arrow dataframe here to handle nulls in int cols
             assert_or_throw(
                 schema is not None, FugueDataFrameInitError("schema can't be None")
             )
             adf = ArrowDataFrame(df, to_schema(schema))
             map_pos = [i for i, t in enumerate(adf.schema.types) if pa.types.is_map(t)]
             if len(map_pos) == 0:
-                sdf = self.spark_session.createDataFrame(
-                    adf.as_array(), to_spark_schema(adf.schema)
-                )
+                sdf = to_spark_df(self.spark_session, adf.as_array(), adf.schema)
             else:
 
                 def to_dict(rows: Iterable[List[Any]]) -> Iterable[List[Any]]:
                     for row in rows:
                         for p in map_pos:
                             row[p] = dict(row[p])
                         yield row
 
-                sdf = self.spark_session.createDataFrame(
-                    to_dict(adf.as_array_iterable()), to_spark_schema(adf.schema)
+                sdf = to_spark_df(
+                    self.spark_session, to_dict(adf.as_array_iterable()), adf.schema
                 )
             return SparkDataFrame(sdf, adf.schema)
 
         res = _to_df()
         if res is not df and isinstance(df, DataFrame) and df.has_metadata:
             res.reset_metadata(df.metadata)
```

### Comparing `fugue-0.8.4.dev2/fugue_spark/ibis_engine.py` & `fugue-0.8.5.dev1/fugue_spark/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_spark/registry.py` & `fugue-0.8.5.dev1/fugue_spark/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_test/bag_suite.py` & `fugue-0.8.5.dev1/fugue_test/bag_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_test/builtin_suite.py` & `fugue-0.8.5.dev1/fugue_test/builtin_suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 # pylint: disable-all
+try:
+    import qpd_pandas  # noqa: F401
+
+    HAS_QPD = True
+except ImportError:  # pragma: no cover
+    HAS_QPD = False
 
 import datetime
 import os
 import pickle
 from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional
 from unittest import TestCase
 from uuid import uuid4
@@ -798,14 +804,15 @@
                 d = a.cross_join(b, c)
                 dag.df(
                     [[1, 10, 2, 4], [1, 10, 3, 4], [2, 20, 2, 4], [2, 20, 3, 4]],
                     "a:int,b:int,c:int,d:int",
                 ).assert_eq(d)
             dag.run(self.engine)
 
+        @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_df_select(self):
             with FugueWorkflow() as dag:
                 # wildcard
                 a = dag.df([[1, 10], [2, 20], [3, 30]], "x:int,y:int")
                 a.select("*").assert_eq(a)
 
                 # column transformation
@@ -849,47 +856,51 @@
 
             with FugueWorkflow() as dag:
                 a = dag.df([[0]], "a:long")
                 b = dag.df([[0]], "a:long")
                 dag.select("select * from", a).assert_eq(b)
             dag.run(self.engine, {"fugue.sql.compile.ignore_case": True})
 
+        @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_df_filter(self):
             with FugueWorkflow() as dag:
                 a = dag.df([[1, 10], [2, 20], [3, 30]], "x:int,y:int")
                 b = dag.df([[2, 20]], "x:int,y:int")
                 a.filter((col("y") > 15) & (col("y") < 25)).assert_eq(b)
             dag.run(self.engine)
 
+        @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_df_assign(self):
             with FugueWorkflow() as dag:
                 a = dag.df([[1, 10], [2, 20], [3, 30]], "x:int,y:int")
                 b = dag.df([[1, "x"], [2, "x"], [3, "x"]], "x:int,y:str")
                 a.assign(y="x").assert_eq(b)
 
                 a = dag.df([[1, 10], [2, 20], [3, 30]], "x:int,y:int")
                 b = dag.df(
                     [[1, "x", 11], [2, "x", 21], [3, "x", 31]], "x:int,y:str,z:double"
                 )
                 a.assign(lit("x").alias("y"), z=(col("y") + 1).cast(float)).assert_eq(b)
             dag.run(self.engine)
 
+        @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_aggregate(self):
             with FugueWorkflow() as dag:
                 a = dag.df([[1, 10], [1, 200], [3, 30]], "x:int,y:int")
                 b = dag.df([[1, 200], [3, 30]], "x:int,y:int")
                 c = dag.df([[-200, 200, 70]], "y:int,zz:int,ww:int")
                 a.partition_by("x").aggregate(ff.max(col("y"))).assert_eq(b)
                 a.aggregate(
                     ff.min(-col("y")),
                     zz=ff.max(col("y")),
                     ww=((ff.min(col("y")) + ff.max(col("y"))) / 3).cast("int32"),
                 ).assert_eq(c)
             dag.run(self.engine)
 
+        @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_select(self):
             class MockEngine(QPDPandasEngine):
                 def __init__(self, execution_engine, p: int = 0):
                     super().__init__(execution_engine)
                     self.p = p
 
                 def select(self, dfs, statement):
@@ -1626,14 +1637,15 @@
                 df = df.transform(t5, schema="a:binary", callback=cb3.call)
                 df.persist().yield_dataframe_as("x", as_local=True)
             dag.run(self.engine)
             assert dag.yields["x"].result.is_local
 
             assert 4 == cb3.n
 
+        @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_sql_api(self):
             def tr(df: pd.DataFrame, n=1) -> pd.DataFrame:
                 return df + n
 
             with fa.engine_context(self.engine):
                 df1 = fa.as_fugue_df([[0, 1], [2, 3], [4, 5]], schema="a:long,b:int")
                 df2 = pd.DataFrame([[0, 10], [1, 100]], columns=["a", "c"])
@@ -1672,14 +1684,15 @@
                     as_fugue=False,
                     as_local=True,
                 )
                 assert not isinstance(sdf4, DataFrame)
                 assert fa.is_local(sdf4)
 
         @pytest.mark.skipif(os.name == "nt", reason="Skip Windows")
+        @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_any_column_name(self):
 
             f_parquet = os.path.join(str(self.tmpdir), "a.parquet")
             f_csv = os.path.join(str(self.tmpdir), "a.csv")
 
             # schema: *,`c *`:long
             def tr(df: pd.DataFrame) -> pd.DataFrame:
```

### Comparing `fugue-0.8.4.dev2/fugue_test/dataframe_suite.py` & `fugue-0.8.5.dev1/fugue_test/dataframe_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/fugue_test/execution_suite.py` & `fugue-0.8.5.dev1/fugue_test/execution_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 # pylint: disable-all
+try:
+    import qpd_pandas  # noqa: F401
+
+    HAS_QPD = True
+except ImportError:  # pragma: no cover
+    HAS_QPD = False
 
 import copy
 import os
 import pickle
 from datetime import datetime
 from unittest import TestCase
 
@@ -92,26 +98,28 @@
 
             # should handle empty pandas dataframe
             o = ArrayDataFrame([], "a:double,b:str")
             pdf = pd.DataFrame([[0.1, "a"]], columns=["a", "b"])
             pdf = pdf[pdf.a < 0]
             df_eq(o, fa.as_fugue_engine_df(e, pdf), throw=True)
 
+        @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_filter(self):
             a = ArrayDataFrame(
                 [[1, 2], [None, 2], [None, 1], [3, 4], [None, 4]],
                 "a:double,b:int",
             )
             b = fa.filter(a, col("a").not_null())
             df_eq(b, [[1, 2], [3, 4]], "a:double,b:int", throw=True)
             c = fa.filter(a, col("a").not_null() & (col("b") < 3))
             df_eq(c, [[1, 2]], "a:double,b:int", throw=True)
             c = fa.filter(a, col("a") + col("b") == 3)
             df_eq(c, [[1, 2]], "a:double,b:int", throw=True)
 
+        @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_select(self):
             a = ArrayDataFrame(
                 [[1, 2], [None, 2], [None, 1], [3, 4], [None, 4]], "a:double,b:int"
             )
 
             # simple
             b = fa.select(a, col("b"), (col("b") + 1).alias("c").cast(str))
@@ -162,14 +170,15 @@
                 col_b.cast(float).alias("c"),
                 having=(col_b >= 7) | (col("a") == 1),
             )
             df_eq(
                 b, [[1, "1", 2], [None, "1", 7]], "a:double,o:str,c:double", throw=True
             )
 
+        @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_assign(self):
             a = ArrayDataFrame(
                 [[1, 2], [None, 2], [None, 1], [3, 4], [None, 4]], "a:double,b:int"
             )
 
             b = fa.assign(a, x=1, b=col("b").cast(str), c=(col("b") + 1).cast(int))
             df_eq(
@@ -181,14 +190,15 @@
                     [3, "4", 1, 5],
                     [None, "4", 1, 5],
                 ],
                 "a:double,b:str,x:long,c:long",
                 throw=True,
             )
 
+        @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_aggregate(self):
             a = ArrayDataFrame(
                 [[1, 2], [None, 2], [None, 1], [3, 4], [None, 4]], "a:double,b:int"
             )
 
             b = fa.aggregate(
                 df=a,
```

### Comparing `fugue-0.8.4.dev2/fugue_test/ibis_suite.py` & `fugue-0.8.5.dev1/fugue_test/ibis_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/setup.cfg` & `fugue-0.8.5.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev2/setup.py` & `fugue-0.8.5.dev1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,60 +17,69 @@
         assert tag == __version__, "release tag and version mismatch"
     return __version__
 
 
 setup(
     name="fugue",
     version=get_version(),
-    packages=find_packages(),
+    packages=find_packages(include=["fugue*"]),
     description="An abstraction layer for distributed computation",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     license="Apache-2.0",
     author="The Fugue Development Team",
     author_email="hello@fugue.ai",
     keywords="distributed spark dask sql dsl domain specific language",
     url="http://github.com/fugue-project/fugue",
     install_requires=[
-        "triad>=0.8.6",
+        "triad>=0.9.0",
         "adagio>=0.2.4",
-        "qpd>=0.4.1",
-        "fugue-sql-antlr>=0.1.6",
         "pyarrow>=0.15.1",
         "pandas>=1.2.0",
+        # sql dependencies
+        "qpd>=0.4.3",
+        "fugue-sql-antlr>=0.1.6",
         "sqlglot",
         "jinja2",
     ],
     extras_require={
+        "sql": [
+            "qpd>=0.4.3",
+            "fugue-sql-antlr>=0.1.6",
+            "sqlglot",
+            "jinja2",
+        ],
         "cpp_sql_parser": ["fugue-sql-antlr[cpp]>=0.1.6"],
-        "spark": ["pyspark"],
+        "spark": ["pyspark>=3.1.1"],
         "dask": [
             "dask[distributed,dataframe]; python_version < '3.8'",
             "dask[distributed,dataframe]>=2022.9.0; python_version >= '3.8'",
-            "qpd[dask]>=0.4.1",
+            "qpd[dask]>=0.4.3",
         ],
         "ray": ["ray[data]>=2.0.0", "duckdb>=0.5.0", "pyarrow>=6.0.1"],
         "duckdb": [
             "duckdb>=0.5.0",
             "pyarrow>=6.0.1",
             "numpy",
         ],
         "polars": ["polars"],
         "ibis": [
             "ibis-framework>=2.1.1; python_version < '3.8'",
             "ibis-framework>=3.2.0; python_version >= '3.8'",
         ],
         "notebook": ["notebook", "jupyterlab", "ipython>=7.10.0"],
         "all": [
+            "sqlglot",
+            "jinja2",
             "fugue-sql-antlr[cpp]>=0.1.6",
-            "pyspark",
+            "pyspark>=3.1.1",
             "dask[distributed,dataframe]; python_version < '3.8'",
             "dask[distributed,dataframe]>=2022.9.0; python_version >= '3.8'",
             "ray[data]>=2.0.0",
-            "qpd[dask]>=0.4.0",
+            "qpd[dask]>=0.4.3",
             "notebook",
             "jupyterlab",
             "ipython>=7.10.0",
             "duckdb>=0.5.0",
             "pyarrow>=6.0.1",
             "ibis-framework>=2.1.1; python_version < '3.8'",
             "ibis-framework>=3.2.0; python_version >= '3.8'",
```

