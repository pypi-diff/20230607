# Comparing `tmp/spetlr-tools-0.1.30.tar.gz` & `tmp/spetlr-tools-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spetlr-tools-0.1.30.tar", last modified: Mon Apr 17 10:47:45 2023, max compression
+gzip compressed data, was "spetlr-tools-0.1.31.tar", last modified: Wed Jun  7 06:26:49 2023, max compression
```

## Comparing `spetlr-tools-0.1.30.tar` & `spetlr-tools-0.1.31.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:45.978616 spetlr-tools-0.1.30/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/src/spetlr_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-17 10:47:45.000000 spetlr-tools-0.1.30/src/spetlr_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-17 10:47:45.000000 spetlr-tools-0.1.30/src/spetlr_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:47:45.000000 spetlr-tools-0.1.30/src/spetlr_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-17 10:47:45.000000 spetlr-tools-0.1.30/src/spetlr_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:47:45.000000 spetlr-tools-0.1.30/src/spetlr_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-17 10:47:45.000000 spetlr-tools-0.1.30/src/spetlr_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 10:47:45.000000 spetlr-tools-0.1.30/src/spetlr_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/src/spetlrtools/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/AuthLinkOpener.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/get_ad_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/src/spetlrtools/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/entry_points/task_entry_point_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/src/spetlrtools/format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/format/validate_camelcased_cols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/src/spetlrtools/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/helpers/ExtractEncodedBody.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/helpers/get_difference_between_two_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/helpers/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/manipulate_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/src/spetlrtools/test_job/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/test_job/RunDetails.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/test_job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/test_job/dbcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/test_job/dbfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/test_job/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/test_job/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/test_job/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/test_job/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/src/spetlrtools/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/testing/DataframeTestCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/testing/TestHandle.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:47:45.982616 spetlr-tools-0.1.30/src/spetlrtools/time/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/time/TimeSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-17 10:47:33.000000 spetlr-tools-0.1.30/src/spetlrtools/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.434051 spetlr-tools-0.1.31/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-07 06:26:49.434051 spetlr-tools-0.1.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-07 06:26:49.434051 spetlr-tools-0.1.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.426051 spetlr-tools-0.1.31/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 06:26:49.000000 spetlr-tools-0.1.31/src/spetlr_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/AuthLinkOpener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/get_ad_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/entry_points/task_entry_point_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/format/validate_camelcased_cols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/helpers/ExtractEncodedBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/helpers/get_difference_between_two_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/helpers/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/manipulate_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/test_job/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/RunDetails.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/dbcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/dbfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/test_job/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.430051 spetlr-tools-0.1.31/src/spetlrtools/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/testing/DataframeTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/testing/TestHandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:26:49.434051 spetlr-tools-0.1.31/src/spetlrtools/time/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/time/TimeSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-07 06:26:31.000000 spetlr-tools-0.1.31/src/spetlrtools/time/__init__.py
```

### Comparing `spetlr-tools-0.1.30/LICENSE` & `spetlr-tools-0.1.31/LICENSE`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/PKG-INFO` & `spetlr-tools-0.1.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr-tools
-Version: 0.1.30
+Version: 0.1.31
 Summary: Supplements to the python SPark ETL libRary (SPETLR) for Databricks.
 Home-page: https://github.com/spetlr-org/spetlr-tools
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr-tools
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr-tools/issues
```

### Comparing `spetlr-tools-0.1.30/setup.cfg` & `spetlr-tools-0.1.31/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 	spetlr
 	pyyaml==6.0
 	importlib_metadata
 	requests
 	dateparser
 	pytest
 	packaging
+	numpy<=1.24 # Numpy does not support 3.8 if above 1.24
+	urllib3<2.0.0
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
 	check-manifest
```

### Comparing `spetlr-tools-0.1.30/src/spetlr_tools.egg-info/PKG-INFO` & `spetlr-tools-0.1.31/src/spetlr_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr-tools
-Version: 0.1.30
+Version: 0.1.31
 Summary: Supplements to the python SPark ETL libRary (SPETLR) for Databricks.
 Home-page: https://github.com/spetlr-org/spetlr-tools
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr-tools
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr-tools/issues
```

### Comparing `spetlr-tools-0.1.30/src/spetlr_tools.egg-info/SOURCES.txt` & `spetlr-tools-0.1.31/src/spetlr_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/AuthLinkOpener.py` & `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/AuthLinkOpener.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/__init__.py` & `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/get_ad_access_token.py` & `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/get_ad_access_token.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py` & `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/main.py` & `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/az_databricks_token/server.py` & `spetlr-tools-0.1.31/src/spetlrtools/az_databricks_token/server.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/entry_points/task_entry_point_helper.py` & `spetlr-tools-0.1.31/src/spetlrtools/entry_points/task_entry_point_helper.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/format/validate_camelcased_cols.py` & `spetlr-tools-0.1.31/src/spetlrtools/format/validate_camelcased_cols.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/helpers/ExtractEncodedBody.py` & `spetlr-tools-0.1.31/src/spetlrtools/helpers/ExtractEncodedBody.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/helpers/get_difference_between_two_dfs.py` & `spetlr-tools-0.1.31/src/spetlrtools/helpers/get_difference_between_two_dfs.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/helpers/module_helper.py` & `spetlr-tools-0.1.31/src/spetlrtools/helpers/module_helper.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/manipulate_version.py` & `spetlr-tools-0.1.31/src/spetlrtools/manipulate_version.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/requirements.py` & `spetlr-tools-0.1.31/src/spetlrtools/requirements.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/test_job/RunDetails.py` & `spetlr-tools-0.1.31/src/spetlrtools/test_job/RunDetails.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/test_job/dbcli.py` & `spetlr-tools-0.1.31/src/spetlrtools/test_job/dbcli.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/test_job/dbfs.py` & `spetlr-tools-0.1.31/src/spetlrtools/test_job/dbfs.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/test_job/fetch.py` & `spetlr-tools-0.1.31/src/spetlrtools/test_job/fetch.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/test_job/submit.py` & `spetlr-tools-0.1.31/src/spetlrtools/test_job/submit.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/test_job/test_main.py` & `spetlr-tools-0.1.31/src/spetlrtools/test_job/test_main.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/testing/DataframeTestCase.py` & `spetlr-tools-0.1.31/src/spetlrtools/testing/DataframeTestCase.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/testing/TestHandle.py` & `spetlr-tools-0.1.31/src/spetlrtools/testing/TestHandle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Any, List, Union
 
 from pyspark.sql import DataFrame
 from spetlr.tables.TableHandle import TableHandle
 
 
 class TestHandle(TableHandle):
+    __test__ = False  # solves PytestCollectionWarning
+
     def __init__(self, provides: DataFrame = None):
         self.provides = provides
         self.overwritten = None
         self.appended = None
         self.truncated = False
         self.dropped = False
         self.dropped_and_deleted = False
```

### Comparing `spetlr-tools-0.1.30/src/spetlrtools/time/TimeSequence.py` & `spetlr-tools-0.1.31/src/spetlrtools/time/TimeSequence.py`

 * *Files identical despite different names*

