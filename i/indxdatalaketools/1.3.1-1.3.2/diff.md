# Comparing `tmp/indxdatalaketools-1.3.1.tar.gz` & `tmp/indxdatalaketools-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indxdatalaketools-1.3.1.tar", last modified: Wed Jun  7 17:48:56 2023, max compression
+gzip compressed data, was "indxdatalaketools-1.3.2.tar", last modified: Wed Jun  7 18:04:53 2023, max compression
```

## Comparing `indxdatalaketools-1.3.1.tar` & `indxdatalaketools-1.3.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.850950 indxdatalaketools-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/NOTICE-numpy
--rw-r--r--   0 runner    (1001) docker     (123)   119371 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/NOTICE-opencv-python.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/NOTICE-requests.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-07 17:48:56.850950 indxdatalaketools-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.842950 indxdatalaketools-1.3.1/indxdatalaketools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/Argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/ClientId.py
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/FileMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/PatientData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/ValidationHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/ClientCommands/
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ClientCommands/DataLakeToolsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ClientCommands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/Changelog/
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/Changelog/Insert.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/Changelog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/ClientOps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/Files/
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/Files/Upload.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/Files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/PatientsTable/
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/PatientsTable/Insert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/PatientsTable/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/PatientsTable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/DataLakeGlobals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/DataStandardizer/
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/DataStandardizer/FileMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/DataStandardizer/PatientTable.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/DataStandardizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/DocumentClassifierApi/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/DocumentClassifierApi/DocumentClassifierApi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/DocumentClassifierApi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/BigQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/CloudStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/CloudTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/ComputeEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/Scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/SecretManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/GoogleClients/
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/GoogleClients/GoogleClients.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/GoogleClients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/Helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/PatientsHoldingApi/
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/PatientsHoldingApi/HoldingTable.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/PatientsHoldingApi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.846950 indxdatalaketools-1.3.1/indxdatalaketools/PropertiesDBApi/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/PropertiesDBApi/Properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/PropertiesDBApi/PropertiesApi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/PropertiesDBApi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/indxdatalaketools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.842950 indxdatalaketools-1.3.1/indxdatalaketools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-07 17:48:56.000000 indxdatalaketools-1.3.1/indxdatalaketools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-07 17:48:56.000000 indxdatalaketools-1.3.1/indxdatalaketools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:48:56.000000 indxdatalaketools-1.3.1/indxdatalaketools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 17:48:56.000000 indxdatalaketools-1.3.1/indxdatalaketools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-07 17:48:56.000000 indxdatalaketools-1.3.1/indxdatalaketools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 17:48:56.000000 indxdatalaketools-1.3.1/indxdatalaketools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:48:56.850950 indxdatalaketools-1.3.1/man/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/man/DataLakeTools.1
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 17:48:56.850950 indxdatalaketools-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-07 17:48:47.000000 indxdatalaketools-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.484108 indxdatalaketools-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/NOTICE-numpy
+-rw-r--r--   0 runner    (1001) docker     (123)   119371 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/NOTICE-opencv-python.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/NOTICE-requests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-07 18:04:53.484108 indxdatalaketools-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.476108 indxdatalaketools-1.3.2/indxdatalaketools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.476108 indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/Argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/ClientId.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/FileMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/PatientData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/ValidationHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.476108 indxdatalaketools-1.3.2/indxdatalaketools/ClientCommands/
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ClientCommands/DataLakeToolsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ClientCommands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.476108 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.476108 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/Changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/Changelog/Insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/Changelog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/ClientOps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.480108 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/Files/
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/Files/Upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/Files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.480108 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/PatientsTable/
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/PatientsTable/Insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/PatientsTable/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/PatientsTable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/DataLakeGlobals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.480108 indxdatalaketools-1.3.2/indxdatalaketools/DataStandardizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/DataStandardizer/FileMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/DataStandardizer/PatientTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/DataStandardizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.480108 indxdatalaketools-1.3.2/indxdatalaketools/DocumentClassifierApi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/DocumentClassifierApi/DocumentClassifierApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/DocumentClassifierApi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.480108 indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/BigQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/CloudStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/CloudTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/ComputeEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/Scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/SecretManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.480108 indxdatalaketools-1.3.2/indxdatalaketools/GoogleClients/
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/GoogleClients/GoogleClients.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/GoogleClients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/Helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.480108 indxdatalaketools-1.3.2/indxdatalaketools/PatientsHoldingApi/
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/PatientsHoldingApi/HoldingTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/PatientsHoldingApi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.484108 indxdatalaketools-1.3.2/indxdatalaketools/PropertiesDBApi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/PropertiesDBApi/Properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/PropertiesDBApi/PropertiesApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/PropertiesDBApi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/indxdatalaketools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.476108 indxdatalaketools-1.3.2/indxdatalaketools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-07 18:04:53.000000 indxdatalaketools-1.3.2/indxdatalaketools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-07 18:04:53.000000 indxdatalaketools-1.3.2/indxdatalaketools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:04:53.000000 indxdatalaketools-1.3.2/indxdatalaketools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 18:04:53.000000 indxdatalaketools-1.3.2/indxdatalaketools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-07 18:04:53.000000 indxdatalaketools-1.3.2/indxdatalaketools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 18:04:53.000000 indxdatalaketools-1.3.2/indxdatalaketools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:04:53.484108 indxdatalaketools-1.3.2/man/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/man/DataLakeTools.1
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:04:53.484108 indxdatalaketools-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-07 18:04:38.000000 indxdatalaketools-1.3.2/setup.py
```

### Comparing `indxdatalaketools-1.3.1/LICENSE` & `indxdatalaketools-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/NOTICE` & `indxdatalaketools-1.3.2/NOTICE`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/NOTICE-numpy` & `indxdatalaketools-1.3.2/NOTICE-numpy`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/NOTICE-opencv-python.txt` & `indxdatalaketools-1.3.2/NOTICE-opencv-python.txt`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/PKG-INFO` & `indxdatalaketools-1.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indxdatalaketools
-Version: 1.3.1
+Version: 1.3.2
 Summary: Package that allows the upload of files to a datalake
 Home-page: https://github.com/IntelligentDX-LLC/data-lake-tools
 Author: Ryan McDermott
 Author-email: rmcdermott@intelligentdx.com
 License: Creative Commons Attribution-NonCommercial-NoDerivatives 4.0
 Project-URL: Bug Tracker, https://github.com/IntelligentDX-LLC/data-lake-tools/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/Argument.py` & `indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/Argument.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/ClientId.py` & `indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/ClientId.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/FileMetadata.py` & `indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/FileMetadata.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/PatientData.py` & `indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/PatientData.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/ArgumentValidation/ValidationHelpers.py` & `indxdatalaketools-1.3.2/indxdatalaketools/ArgumentValidation/ValidationHelpers.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/ClientCommands/DataLakeToolsClient.py` & `indxdatalaketools-1.3.2/indxdatalaketools/ClientCommands/DataLakeToolsClient.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/Changelog/Insert.py` & `indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/Changelog/Insert.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/ClientOps.py` & `indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/ClientOps.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/Files/Upload.py` & `indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/Files/Upload.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/PatientsTable/Insert.py` & `indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/PatientsTable/Insert.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/ClientTools/PatientsTable/Update.py` & `indxdatalaketools-1.3.2/indxdatalaketools/ClientTools/PatientsTable/Update.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/DataStandardizer/FileMetadata.py` & `indxdatalaketools-1.3.2/indxdatalaketools/DataStandardizer/FileMetadata.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/DataStandardizer/PatientTable.py` & `indxdatalaketools-1.3.2/indxdatalaketools/DataStandardizer/PatientTable.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/DocumentClassifierApi/DocumentClassifierApi.py` & `indxdatalaketools-1.3.2/indxdatalaketools/DocumentClassifierApi/DocumentClassifierApi.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/BigQuery.py` & `indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/BigQuery.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/CloudStorage.py` & `indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/CloudTasks.py` & `indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/CloudTasks.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/ComputeEngine.py` & `indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/ComputeEngine.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/Scheduler.py` & `indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/Scheduler.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/GoogleClientWrappers/SecretManager.py` & `indxdatalaketools-1.3.2/indxdatalaketools/GoogleClientWrappers/SecretManager.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/GoogleClients/GoogleClients.py` & `indxdatalaketools-1.3.2/indxdatalaketools/GoogleClients/GoogleClients.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/Helpers.py` & `indxdatalaketools-1.3.2/indxdatalaketools/Helpers.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/PatientsHoldingApi/HoldingTable.py` & `indxdatalaketools-1.3.2/indxdatalaketools/PatientsHoldingApi/HoldingTable.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/PropertiesDBApi/Properties.py` & `indxdatalaketools-1.3.2/indxdatalaketools/PropertiesDBApi/Properties.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools/PropertiesDBApi/PropertiesApi.py` & `indxdatalaketools-1.3.2/indxdatalaketools/PropertiesDBApi/PropertiesApi.py`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools.egg-info/PKG-INFO` & `indxdatalaketools-1.3.2/indxdatalaketools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indxdatalaketools
-Version: 1.3.1
+Version: 1.3.2
 Summary: Package that allows the upload of files to a datalake
 Home-page: https://github.com/IntelligentDX-LLC/data-lake-tools
 Author: Ryan McDermott
 Author-email: rmcdermott@intelligentdx.com
 License: Creative Commons Attribution-NonCommercial-NoDerivatives 4.0
 Project-URL: Bug Tracker, https://github.com/IntelligentDX-LLC/data-lake-tools/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `indxdatalaketools-1.3.1/indxdatalaketools.egg-info/SOURCES.txt` & `indxdatalaketools-1.3.2/indxdatalaketools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/man/DataLakeTools.1` & `indxdatalaketools-1.3.2/man/DataLakeTools.1`

 * *Files identical despite different names*

### Comparing `indxdatalaketools-1.3.1/setup.py` & `indxdatalaketools-1.3.2/setup.py`

 * *Files identical despite different names*

