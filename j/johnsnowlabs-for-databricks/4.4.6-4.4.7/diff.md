# Comparing `tmp/johnsnowlabs_for_databricks-4.4.6.tar.gz` & `tmp/johnsnowlabs_for_databricks-4.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs_for_databricks-4.4.6.tar", last modified: Sun May 28 18:43:20 2023, max compression
+gzip compressed data, was "johnsnowlabs_for_databricks-4.4.7.tar", last modified: Wed Jun  7 01:00:08 2023, max compression
```

## Comparing `johnsnowlabs_for_databricks-4.4.6.tar` & `johnsnowlabs_for_databricks-4.4.7.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:20.002379 johnsnowlabs_for_databricks-4.4.6/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs_for_databricks-4.4.6/LICENSE
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9293 2023-05-28 18:43:20.002379 johnsnowlabs_for_databricks-4.4.6/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs_for_databricks-4.4.6/README.md
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:19.998379 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:19.998379 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/abstract_base/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2023-05-28 18:29:17.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/abstract_base/software_product.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:19.998379 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:19.998379 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:19.998379 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2023-05-26 21:55:38.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/jsl_home.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:19.998379 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-05-25 04:21:48.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-05-25 02:23:06.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/offline_install.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-05-28 17:28:52.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4710 2023-04-26 14:30:28.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/finance.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/lab.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4639 2023-04-26 14:30:28.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/legal.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4526 2023-05-28 17:25:36.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/medical.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/nlp.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:20.002379 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4925 2023-05-26 21:57:49.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2200 2023-05-28 18:42:02.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/settings.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:20.002379 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4409 2023-05-26 12:08:46.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8127 2023-05-21 06:35:03.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/sparksession_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:20.002379 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/testing/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/visual.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/viz.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-28 18:43:20.002379 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs_for_databricks.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9293 2023-05-28 18:43:19.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs_for_databricks.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2541 2023-05-28 18:43:19.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs_for_databricks.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-28 18:43:19.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs_for_databricks.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      111 2023-05-28 18:43:19.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs_for_databricks.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-05-28 18:43:19.000000 johnsnowlabs_for_databricks-4.4.6/johnsnowlabs_for_databricks.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-05-28 18:43:20.002379 johnsnowlabs_for_databricks-4.4.6/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2065 2023-05-28 18:43:13.000000 johnsnowlabs_for_databricks-4.4.6/setup.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-07 01:00:08.141823 johnsnowlabs_for_databricks-4.4.7/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs_for_databricks-4.4.7/LICENSE
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9293 2023-06-07 01:00:08.141823 johnsnowlabs_for_databricks-4.4.7/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs_for_databricks-4.4.7/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-07 01:00:08.133823 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-07 01:00:08.133823 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2023-05-28 18:29:17.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-07 01:00:08.133823 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-07 01:00:08.133823 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-07 01:00:08.137823 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2023-05-26 21:55:38.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-07 01:00:08.137823 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-05-25 04:21:48.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-05-25 02:23:06.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/offline_install.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-06-06 22:37:19.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4755 2023-06-07 00:53:32.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/finance.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4703 2023-06-07 00:47:56.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4625 2023-06-07 00:48:11.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-07 01:00:08.137823 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4925 2023-05-26 21:57:49.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-06-03 18:20:47.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2201 2023-06-07 00:57:21.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-07 01:00:08.137823 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4409 2023-05-26 12:08:46.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8127 2023-05-21 06:35:03.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-07 01:00:08.141823 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-07 01:00:08.141823 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs_for_databricks.egg-info/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9293 2023-06-07 01:00:08.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs_for_databricks.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2541 2023-06-07 01:00:08.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs_for_databricks.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-06-07 01:00:08.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs_for_databricks.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      115 2023-06-07 01:00:08.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs_for_databricks.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-06-07 01:00:08.000000 johnsnowlabs_for_databricks-4.4.7/johnsnowlabs_for_databricks.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-06-07 01:00:08.141823 johnsnowlabs_for_databricks-4.4.7/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1906 2023-06-07 01:00:04.000000 johnsnowlabs_for_databricks-4.4.7/setup.py
```

### Comparing `johnsnowlabs_for_databricks-4.4.6/LICENSE` & `johnsnowlabs_for_databricks-4.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/PKG-INFO` & `johnsnowlabs_for_databricks-4.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs_for_databricks
-Version: 4.4.6
+Version: 4.4.7
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs_for_databricks-4.4.6/README.md` & `johnsnowlabs_for_databricks-4.4.7/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/__init__.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/finance.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/finance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import traceback
 
 from johnsnowlabs.abstract_base.lib_resolver import try_import_lib
 from johnsnowlabs.utils.env_utils import reverse_compatibility_import
 from johnsnowlabs.utils.print_messages import log_broken_lib
 
 try:
-
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
         from sparknlp_jsl.functions import *
         from sparknlp_jsl.training import *
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
         from sparknlp_jsl.base import FeaturesAssembler
         from sparknlp_jsl.annotator.windowed.windowed_sentence import (
             WindowedSentenceModel,
@@ -83,22 +82,23 @@
             DocumentLogRegClassifierApproach,
             RelationExtractionApproach,
             ChunkMergeApproach,
             NerDisambiguator,
             ContextualParserApproach,
             GenericClassifierApproach,
             Router,
-            NerQuestionGenerator,
             Replacer,
-            # NEW
             ContextualParserModel,
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             Resolution2Chunk,
             ResolverMerger,
+            NerTemplateRenderModel,
+            AverageEmbeddings,
+            Doc2ChunkInternal,
         )
 
         from sparknlp_jsl.modelTracer import ModelTracer
         from sparknlp_jsl import training_log_parser, Deid
         from sparknlp_jsl.compatibility import Compatibility
         from sparknlp_jsl.pretrained import InternalResourceDownloader
         from sparknlp_jsl.eval import (
```

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/legal.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/legal.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,20 +82,22 @@
             DocumentLogRegClassifierApproach,
             RelationExtractionApproach,
             ChunkMergeApproach,
             NerDisambiguator,
             ContextualParserApproach,
             GenericClassifierApproach,
             Router,
-            NerQuestionGenerator,
             AssertionChunkConverter,
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             # Resolution2Chunk,
             ResolverMerger,
+            NerTemplateRenderModel,
+            AverageEmbeddings,
+            Doc2ChunkInternal,
         )
         from sparknlp_jsl.modelTracer import ModelTracer
 
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
 
         from sparknlp_jsl import training_log_parser, Deid
```

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/medical.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/medical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import traceback
+
 from johnsnowlabs.abstract_base.lib_resolver import try_import_lib
 from johnsnowlabs.auto_install.softwares import Software
 from johnsnowlabs.utils.env_utils import reverse_compatibility_import
 from johnsnowlabs.utils.print_messages import log_outdated_lib, log_broken_lib
 
 warning_logged = False
 
@@ -68,14 +69,17 @@
             DocMapperApproach,
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             DocumentMLClassifierApproach,
             DocumentMLClassifierModel,
             Resolution2Chunk,
             MedicalQuestionAnswering,
+            NerTemplateRenderModel,
+            AverageEmbeddings,
+            Doc2ChunkInternal,
         )
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
         from sparknlp_jsl.modelTracer import ModelTracer
         from sparknlp_jsl import training_log_parser, Deid
         from sparknlp_jsl.training_log_parser import ner_log_parser
 
         from sparknlp_jsl.base import FeaturesAssembler
```

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/nlp.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/settings.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 from johnsnowlabs.utils.env_utils import (
     is_running_in_databricks,
     set_py4j_logger_to_error_on_databricks,
     env_required_license,
 )
 
 # These versions are used for auto-installs and version  checks
-raw_version_jsl_lib = "4.4.6"
+raw_version_jsl_lib = "4.4.7"
 raw_version_nlp = "4.4.1"
-raw_version_nlu = "4.2.0"
+raw_version_nlu = "4.2.1"
+
 raw_version_pyspark = "3.1.2"
 raw_version_nlp_display = "4.1"
 
-raw_version_medical = "4.4.2"
-raw_version_secret_medical = "4.4.2"
+raw_version_medical = "4.4.3"
+raw_version_secret_medical = "4.4.3"
 
-raw_version_secret_ocr = "4.4.1"
-raw_version_ocr = "4.4.1"
+raw_version_secret_ocr = "4.4.2"
+raw_version_ocr = "4.4.2"
 
 pypi_page = "https://pypi.org/project/johnsnowlabs"
 json_indent = 4
 enforce_secret_on_version = False
 enforce_versions = True
 
 # Environment
```

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/enums.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/functional.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/py_process.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs/visual.py` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs_for_databricks.egg-info/PKG-INFO` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs_for_databricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs-for-databricks
-Version: 4.4.6
+Version: 4.4.7
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs_for_databricks-4.4.6/johnsnowlabs_for_databricks.egg-info/SOURCES.txt` & `johnsnowlabs_for_databricks-4.4.7/johnsnowlabs_for_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

