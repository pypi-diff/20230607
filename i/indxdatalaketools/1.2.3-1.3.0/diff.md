# Comparing `tmp/indxdatalaketools-1.2.3.tar.gz` & `tmp/indxdatalaketools-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indxdatalaketools-1.2.3.tar", last modified: Tue Dec 13 14:48:20 2022, max compression
+gzip compressed data, was "indxdatalaketools-1.3.0.tar", last modified: Wed Jun  7 17:02:53 2023, max compression
```

## Comparing `indxdatalaketools-1.2.3.tar` & `indxdatalaketools-1.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.820775 indxdatalaketools-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13876 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      633 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/NOTICE-numpy
--rw-r--r--   0 runner    (1001) docker     (123)   119371 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/NOTICE-opencv-python.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/NOTICE-requests.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-13 14:48:20.820775 indxdatalaketools-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.812775 indxdatalaketools-1.2.3/indxdatalaketools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.812775 indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/Argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/ClientId.py
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/FileMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/PatientData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/ValidationHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.816775 indxdatalaketools-1.2.3/indxdatalaketools/ClientCommands/
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ClientCommands/DataLakeToolsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ClientCommands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.816775 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.816775 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/Changelog/
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/Changelog/Insert.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/Changelog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/ClientOps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.816775 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/Files/
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/Files/Upload.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/Files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.816775 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/PatientsTable/
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/PatientsTable/Insert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/PatientsTable/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/PatientsTable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/DataLakeGlobals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.816775 indxdatalaketools-1.2.3/indxdatalaketools/DataStandardizer/
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/DataStandardizer/FileMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/DataStandardizer/PatientTable.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/DataStandardizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.816775 indxdatalaketools-1.2.3/indxdatalaketools/DocumentClassifierApi/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/DocumentClassifierApi/DocumentClassifierApi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/DocumentClassifierApi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.820775 indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/BigQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/CloudStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/CloudTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/ComputeEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/Scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/SecretManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.820775 indxdatalaketools-1.2.3/indxdatalaketools/GoogleClients/
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/GoogleClients/GoogleClients.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/GoogleClients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/Helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.820775 indxdatalaketools-1.2.3/indxdatalaketools/PatientsHoldingApi/
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/PatientsHoldingApi/HoldingTable.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/PatientsHoldingApi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.820775 indxdatalaketools-1.2.3/indxdatalaketools/PropertiesDBApi/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/PropertiesDBApi/Properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/PropertiesDBApi/PropertiesApi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/PropertiesDBApi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/indxdatalaketools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.812775 indxdatalaketools-1.2.3/indxdatalaketools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-13 14:48:20.000000 indxdatalaketools-1.2.3/indxdatalaketools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2022-12-13 14:48:20.000000 indxdatalaketools-1.2.3/indxdatalaketools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:48:20.000000 indxdatalaketools-1.2.3/indxdatalaketools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-13 14:48:20.000000 indxdatalaketools-1.2.3/indxdatalaketools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2022-12-13 14:48:20.000000 indxdatalaketools-1.2.3/indxdatalaketools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-13 14:48:20.000000 indxdatalaketools-1.2.3/indxdatalaketools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:48:20.820775 indxdatalaketools-1.2.3/man/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/man/DataLakeTools.1
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 14:48:20.820775 indxdatalaketools-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2022-12-13 14:48:09.000000 indxdatalaketools-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.361707 indxdatalaketools-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/NOTICE-numpy
+-rw-r--r--   0 runner    (1001) docker     (123)   119371 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/NOTICE-opencv-python.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/NOTICE-requests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-07 17:02:53.361707 indxdatalaketools-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.357707 indxdatalaketools-1.3.0/indxdatalaketools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.357707 indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/Argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/ClientId.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/FileMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/PatientData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/ValidationHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.357707 indxdatalaketools-1.3.0/indxdatalaketools/ClientCommands/
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ClientCommands/DataLakeToolsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ClientCommands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.357707 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.357707 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/Changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/Changelog/Insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/Changelog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/ClientOps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.357707 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/Files/
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/Files/Upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/Files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.357707 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/PatientsTable/
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/PatientsTable/Insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/PatientsTable/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/PatientsTable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/DataLakeGlobals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.357707 indxdatalaketools-1.3.0/indxdatalaketools/DataStandardizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/DataStandardizer/FileMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/DataStandardizer/PatientTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/DataStandardizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.361707 indxdatalaketools-1.3.0/indxdatalaketools/DocumentClassifierApi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/DocumentClassifierApi/DocumentClassifierApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/DocumentClassifierApi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.361707 indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/BigQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/CloudStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/CloudTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/ComputeEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/Scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/SecretManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.361707 indxdatalaketools-1.3.0/indxdatalaketools/GoogleClients/
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/GoogleClients/GoogleClients.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/GoogleClients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/Helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.361707 indxdatalaketools-1.3.0/indxdatalaketools/PatientsHoldingApi/
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/PatientsHoldingApi/HoldingTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/PatientsHoldingApi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.361707 indxdatalaketools-1.3.0/indxdatalaketools/PropertiesDBApi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/PropertiesDBApi/Properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/PropertiesDBApi/PropertiesApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/PropertiesDBApi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/indxdatalaketools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.357707 indxdatalaketools-1.3.0/indxdatalaketools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-07 17:02:53.000000 indxdatalaketools-1.3.0/indxdatalaketools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-07 17:02:53.000000 indxdatalaketools-1.3.0/indxdatalaketools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:02:53.000000 indxdatalaketools-1.3.0/indxdatalaketools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 17:02:53.000000 indxdatalaketools-1.3.0/indxdatalaketools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-07 17:02:53.000000 indxdatalaketools-1.3.0/indxdatalaketools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 17:02:53.000000 indxdatalaketools-1.3.0/indxdatalaketools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:02:53.361707 indxdatalaketools-1.3.0/man/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/man/DataLakeTools.1
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 17:02:53.361707 indxdatalaketools-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-07 17:02:41.000000 indxdatalaketools-1.3.0/setup.py
```

### Comparing `indxdatalaketools-1.2.3/LICENSE` & `indxdatalaketools-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/NOTICE` & `indxdatalaketools-1.3.0/NOTICE`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/NOTICE-numpy` & `indxdatalaketools-1.3.0/NOTICE-numpy`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/NOTICE-opencv-python.txt` & `indxdatalaketools-1.3.0/NOTICE-opencv-python.txt`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/PKG-INFO` & `indxdatalaketools-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indxdatalaketools
-Version: 1.2.3
+Version: 1.3.0
 Summary: Package that allows the upload of files to a datalake
 Home-page: https://github.com/IntelligentDX-LLC/data-lake-tools
 Author: Ryan McDermott
 Author-email: rmcdermott@intelligentdx.com
 License: Creative Commons Attribution-NonCommercial-NoDerivatives 4.0
 Project-URL: Bug Tracker, https://github.com/IntelligentDX-LLC/data-lake-tools/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/Argument.py` & `indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/Argument.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/ClientId.py` & `indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/ClientId.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/FileMetadata.py` & `indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/FileMetadata.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/PatientData.py` & `indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/PatientData.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/ArgumentValidation/ValidationHelpers.py` & `indxdatalaketools-1.3.0/indxdatalaketools/ArgumentValidation/ValidationHelpers.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/ClientCommands/DataLakeToolsClient.py` & `indxdatalaketools-1.3.0/indxdatalaketools/ClientCommands/DataLakeToolsClient.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/Changelog/Insert.py` & `indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/Changelog/Insert.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/ClientOps.py` & `indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/ClientOps.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/Files/Upload.py` & `indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/Files/Upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,25 +38,30 @@
             Returns:
                 None
         '''
         self.client_uuid = client_uuid
         self.__file_upload_logger = GcpClients.instance().get_logging_client(
         ).logger(client_uuid + '-file-logger')
 
-    def upload_file_to_datalake(self, modality, mrn, metadata, file_path):
+    def upload_file_to_datalake(self, modality, mrn, metadata, file_path, 
+                                patient_uuid=None):
         '''
             Uploads a file to the data lake and sets the metadata
             for that file
             Args:
                 modality    (string): The file's modality
-                mrn         (string): The mrn of the patient to who the files belongs to
+                mrn         (string): The mrn of the patient to who the files 
+                    belongs to
                 metadata    (string): The metadata that is associated with the
                     file
-                file_path   (string): The path to the file we wish to upload to a 
-                    datalake
+                file_path   (string): The path to the file we wish to upload 
+                    to a datalake
+                patient_uuid (string): If this optional argument is set, 
+                    mrn is bypassed and this string is used as the hashed 
+                    patient mrn
             Returns:
                 boolean: True if the File was successfully uploaded, False if 
                     otherwise
                 
         '''
         file_contents = self.__read_file_contents(file_path)
         file_extension = os.path.splitext(file_path)[1]
@@ -66,16 +71,19 @@
         # convert bmp to png
         if '.bmp' == file_extension.lower():
             file_contents = self.__convert_bmp_to_png(file_contents)
             file_root = os.path.splitext(file_path)[0]
             file_path = file_root + '.png'
 
         stripped_mrn = self.__strip_leading_zeros(mrn)
-        hashed_patient_mrn = Helpers.patient_hash(self.client_uuid,
-                                                  [stripped_mrn])[0]
+        if patient_uuid is not None:
+            hashed_patient_mrn = patient_uuid
+        else:
+            hashed_patient_mrn = Helpers.patient_hash(self.client_uuid, 
+                                                      [stripped_mrn])[0]
         hashed_file_name = Helpers.hash_contents_to_file_name(
             file_path, file_contents)
         blob_name = modality + "/" + hashed_patient_mrn + "/" + hashed_file_name
         bucket = GcpClients.instance().get_storage_client().bucket(
             self.client_uuid)
         blob = bucket.blob(blob_name)
```

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/PatientsTable/Insert.py` & `indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/PatientsTable/Insert.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/ClientTools/PatientsTable/Update.py` & `indxdatalaketools-1.3.0/indxdatalaketools/ClientTools/PatientsTable/Update.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/DataStandardizer/FileMetadata.py` & `indxdatalaketools-1.3.0/indxdatalaketools/DataStandardizer/FileMetadata.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/DataStandardizer/PatientTable.py` & `indxdatalaketools-1.3.0/indxdatalaketools/DataStandardizer/PatientTable.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/DocumentClassifierApi/DocumentClassifierApi.py` & `indxdatalaketools-1.3.0/indxdatalaketools/DocumentClassifierApi/DocumentClassifierApi.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/BigQuery.py` & `indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/BigQuery.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/CloudStorage.py` & `indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/CloudTasks.py` & `indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/CloudTasks.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/ComputeEngine.py` & `indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/ComputeEngine.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/Scheduler.py` & `indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/Scheduler.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/GoogleClientWrappers/SecretManager.py` & `indxdatalaketools-1.3.0/indxdatalaketools/GoogleClientWrappers/SecretManager.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/GoogleClients/GoogleClients.py` & `indxdatalaketools-1.3.0/indxdatalaketools/GoogleClients/GoogleClients.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/Helpers.py` & `indxdatalaketools-1.3.0/indxdatalaketools/Helpers.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/PatientsHoldingApi/HoldingTable.py` & `indxdatalaketools-1.3.0/indxdatalaketools/PatientsHoldingApi/HoldingTable.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/PropertiesDBApi/Properties.py` & `indxdatalaketools-1.3.0/indxdatalaketools/PropertiesDBApi/Properties.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools/PropertiesDBApi/PropertiesApi.py` & `indxdatalaketools-1.3.0/indxdatalaketools/PropertiesDBApi/PropertiesApi.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools.egg-info/PKG-INFO` & `indxdatalaketools-1.3.0/indxdatalaketools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indxdatalaketools
-Version: 1.2.3
+Version: 1.3.0
 Summary: Package that allows the upload of files to a datalake
 Home-page: https://github.com/IntelligentDX-LLC/data-lake-tools
 Author: Ryan McDermott
 Author-email: rmcdermott@intelligentdx.com
 License: Creative Commons Attribution-NonCommercial-NoDerivatives 4.0
 Project-URL: Bug Tracker, https://github.com/IntelligentDX-LLC/data-lake-tools/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `indxdatalaketools-1.2.3/indxdatalaketools.egg-info/SOURCES.txt` & `indxdatalaketools-1.3.0/indxdatalaketools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/man/DataLakeTools.1` & `indxdatalaketools-1.3.0/man/DataLakeTools.1`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.2.3/setup.py` & `indxdatalaketools-1.3.0/setup.py`

 * *Files identical despite different names*

