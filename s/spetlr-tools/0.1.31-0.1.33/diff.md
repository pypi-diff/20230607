# Comparing `tmp/spetlr-tools-0.1.31.tar.gz` & `tmp/spetlr-tools-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spetlr-tools-0.1.31.tar", last modified: Wed Jun  7 06:26:49 2023, max compression
+gzip compressed data, was "spetlr-tools-0.1.33.tar", last modified: Wed Jun  7 16:09:23 2023, max compression
```

## Comparing `spetlr-tools-0.1.31.tar` & `spetlr-tools-0.1.33.tar`

### file list

```diff
@@ -1,54 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.434051 spetlr-tools-0.1.31/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-07 06:26:49.434051 spetlr-tools-0.1.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-07 06:26:49.434051 spetlr-tools-0.1.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.426051 spetlr-tools-0.1.31/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/AuthLinkOpener.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/get_ad_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/entry_points/task_entry_point_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/format/validate_camelcased_cols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/helpers/ExtractEncodedBody.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/helpers/get_difference_between_two_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/helpers/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/manipulate_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/test_job/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/RunDetails.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/dbcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/dbfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/testing/DataframeTestCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/testing/TestHandle.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.434051 spetlr-tools-0.1.31/src/spetlrtools/time/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/time/TimeSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.897007 spetlr-tools-0.1.33/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-07 16:09:23.897007 spetlr-tools-0.1.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-07 16:09:23.897007 spetlr-tools-0.1.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.877006 spetlr-tools-0.1.33/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.881006 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.885006 spetlr-tools-0.1.33/src/spetlrtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.885006 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/AuthLinkOpener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/get_ad_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.889007 spetlr-tools-0.1.33/src/spetlrtools/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/DiagramMarkupLibraryParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/DrawioDiagramParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/Edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/HTMLStripper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.889007 spetlr-tools-0.1.33/src/spetlrtools/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/entry_points/task_entry_point_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.889007 spetlr-tools-0.1.33/src/spetlrtools/format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/format/validate_camelcased_cols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.889007 spetlr-tools-0.1.33/src/spetlrtools/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/helpers/ExtractEncodedBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/helpers/get_difference_between_two_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/helpers/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/manipulate_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.893007 spetlr-tools-0.1.33/src/spetlrtools/test_job/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/RunDetails.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/dbcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/dbfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.893007 spetlr-tools-0.1.33/src/spetlrtools/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/testing/DataframeTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/testing/TestHandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.897007 spetlr-tools-0.1.33/src/spetlrtools/time/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/time/TimeSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/time/__init__.py
```

### Comparing `spetlr-tools-0.1.31/LICENSE` & `spetlr-tools-0.1.33/LICENSE`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/setup.cfg` & `spetlr-tools-0.1.33/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
 [options.entry_points]
 console_scripts = 
 	spetlr-freeze-req = spetlrtools.requirements:main
 	spetlr-az-databricks-token = spetlrtools.az_databricks_token.main:main
 	spetlr-test-job = spetlrtools.test_job.main:main
 	spetlr-manipulate-version = spetlrtools.manipulate_version:main
+	spetlr-check-diagram = spetlrtools.diagrams.main:main
 
 [flake8]
 exclude = .git,__pycache__,docs,build,dist,venv
 ignore = E501, W503
 max-line-length = 88
 extend-ignore = E203
```

### Comparing `spetlr-tools-0.1.31/src/spetlr_tools.egg-info/SOURCES.txt` & `spetlr-tools-0.1.33/src/spetlr_tools.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 src/spetlrtools/requirements.py
 src/spetlrtools/az_databricks_token/AuthLinkOpener.py
 src/spetlrtools/az_databricks_token/__init__.py
 src/spetlrtools/az_databricks_token/get_ad_access_token.py
 src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py
 src/spetlrtools/az_databricks_token/main.py
 src/spetlrtools/az_databricks_token/server.py
+src/spetlrtools/diagrams/DiagramMarkupLibraryParser.py
+src/spetlrtools/diagrams/DrawioDiagramParser.py
+src/spetlrtools/diagrams/Edge.py
+src/spetlrtools/diagrams/HTMLStripper.py
+src/spetlrtools/diagrams/__init__.py
+src/spetlrtools/diagrams/main.py
 src/spetlrtools/entry_points/__init__.py
 src/spetlrtools/entry_points/task_entry_point_helper.py
 src/spetlrtools/format/__init__.py
 src/spetlrtools/format/validate_camelcased_cols.py
 src/spetlrtools/helpers/ExtractEncodedBody.py
 src/spetlrtools/helpers/__init__.py
 src/spetlrtools/helpers/get_difference_between_two_dfs.py
```

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/AuthLinkOpener.py` & `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/AuthLinkOpener.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/__init__.py` & `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/get_ad_access_token.py` & `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/get_ad_access_token.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py` & `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/main.py` & `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/server.py` & `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/server.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/entry_points/task_entry_point_helper.py` & `spetlr-tools-0.1.33/src/spetlrtools/entry_points/task_entry_point_helper.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/format/validate_camelcased_cols.py` & `spetlr-tools-0.1.33/src/spetlrtools/format/validate_camelcased_cols.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/helpers/ExtractEncodedBody.py` & `spetlr-tools-0.1.33/src/spetlrtools/helpers/ExtractEncodedBody.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/helpers/get_difference_between_two_dfs.py` & `spetlr-tools-0.1.33/src/spetlrtools/helpers/get_difference_between_two_dfs.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/helpers/module_helper.py` & `spetlr-tools-0.1.33/src/spetlrtools/helpers/module_helper.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/manipulate_version.py` & `spetlr-tools-0.1.33/src/spetlrtools/manipulate_version.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/requirements.py` & `spetlr-tools-0.1.33/src/spetlrtools/requirements.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/test_job/RunDetails.py` & `spetlr-tools-0.1.33/src/spetlrtools/test_job/RunDetails.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/test_job/dbcli.py` & `spetlr-tools-0.1.33/src/spetlrtools/test_job/dbcli.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/test_job/dbfs.py` & `spetlr-tools-0.1.33/src/spetlrtools/test_job/dbfs.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/test_job/fetch.py` & `spetlr-tools-0.1.33/src/spetlrtools/test_job/fetch.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/test_job/submit.py` & `spetlr-tools-0.1.33/src/spetlrtools/test_job/submit.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/test_job/test_main.py` & `spetlr-tools-0.1.33/src/spetlrtools/test_job/test_main.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/testing/DataframeTestCase.py` & `spetlr-tools-0.1.33/src/spetlrtools/testing/DataframeTestCase.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/testing/TestHandle.py` & `spetlr-tools-0.1.33/src/spetlrtools/testing/TestHandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.31/src/spetlrtools/time/TimeSequence.py` & `spetlr-tools-0.1.33/src/spetlrtools/time/TimeSequence.py`

 * *Files identical despite different names*

