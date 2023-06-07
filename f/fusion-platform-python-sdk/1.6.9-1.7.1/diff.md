# Comparing `tmp/fusion-platform-python-sdk-1.6.9.tar.gz` & `tmp/fusion-platform-python-sdk-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-platform-python-sdk-1.6.9.tar", last modified: Wed May 10 12:55:20 2023, max compression
+gzip compressed data, was "fusion-platform-python-sdk-1.7.1.tar", last modified: Fri May 26 13:45:35 2023, max compression
```

## Comparing `fusion-platform-python-sdk-1.6.9.tar` & `fusion-platform-python-sdk-1.7.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-10 12:55:20.790453 fusion-platform-python-sdk-1.6.9/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.6.9/LICENSE.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.6.9/MANIFEST.in
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-05-10 12:55:20.790113 fusion-platform-python-sdk-1.6.9/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4455 2022-09-01 10:14:11.000000 fusion-platform-python-sdk-1.6.9/README.md
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-10 12:55:20.772712 fusion-platform-python-sdk-1.6.9/fusion_platform/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     6806 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/__main__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/base.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/command.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-10 12:55:20.774908 fusion-platform-python-sdk-1.6.9/fusion_platform/common/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/common/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/common/raise_thread.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/common/utilities.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/documentation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)  1547331 2023-02-08 14:50:52.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/fusion_platform_sdk.pdf
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2237 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/glasgow.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)  1869438 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/lake_district.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/localisations.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/localise.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-10 12:55:20.786533 fusion-platform-python-sdk-1.6.9/fusion_platform/models/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/credit.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/credit.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/data.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/data.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/data_file.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/data_file.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/fields.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    30748 2023-01-13 10:46:35.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/model.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/organisation.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    12611 2022-06-27 13:48:00.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/organisation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/process.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    37970 2023-04-25 06:29:47.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/process.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2602 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/process_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     8982 2023-05-10 09:30:14.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/process_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3264 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/process_service_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10365 2022-06-16 08:00:49.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/process_service_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/process_service_execution_log.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/process_service_execution_log.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/service.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     9709 2022-08-19 10:03:50.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/service.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/user.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/models/user.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/session.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     7233 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/fusion_platform/translations.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-10 12:55:20.789653 fusion-platform-python-sdk-1.6.9/fusion_platform_python_sdk.egg-info/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-05-10 12:55:20.000000 fusion-platform-python-sdk-1.6.9/fusion_platform_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1704 2023-05-10 12:55:20.000000 fusion-platform-python-sdk-1.6.9/fusion_platform_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2023-05-10 12:55:20.000000 fusion-platform-python-sdk-1.6.9/fusion_platform_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       77 2023-05-10 12:55:20.000000 fusion-platform-python-sdk-1.6.9/fusion_platform_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2023-05-10 12:55:20.000000 fusion-platform-python-sdk-1.6.9/fusion_platform_python_sdk.egg-info/requires.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2023-05-10 12:55:20.000000 fusion-platform-python-sdk-1.6.9/fusion_platform_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2023-05-10 12:55:20.790593 fusion-platform-python-sdk-1.6.9/setup.cfg
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1551 2023-05-10 12:55:18.000000 fusion-platform-python-sdk-1.6.9/setup.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-26 13:45:35.840305 fusion-platform-python-sdk-1.7.1/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.7.1/LICENSE.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.7.1/MANIFEST.in
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-05-26 13:45:35.839925 fusion-platform-python-sdk-1.7.1/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4455 2022-09-01 10:14:11.000000 fusion-platform-python-sdk-1.7.1/README.md
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-26 13:45:35.789415 fusion-platform-python-sdk-1.7.1/fusion_platform/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     6806 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/__main__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/base.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/command.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-26 13:45:35.813316 fusion-platform-python-sdk-1.7.1/fusion_platform/common/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/common/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/common/raise_thread.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/common/utilities.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/documentation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  1547331 2023-02-08 14:50:52.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/fusion_platform_sdk.pdf
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2237 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/glasgow.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  1869438 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/lake_district.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/localisations.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/localise.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-26 13:45:35.831790 fusion-platform-python-sdk-1.7.1/fusion_platform/models/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/credit.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/credit.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/data.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/data.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/data_file.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/data_file.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/fields.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    31868 2023-05-24 14:20:34.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/model.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/organisation.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    14976 2023-05-25 09:18:19.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/organisation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    50701 2023-05-26 13:32:08.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2602 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     8982 2023-05-10 09:30:14.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3359 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10487 2023-05-23 06:25:23.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution_log.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution_log.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/service.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     9735 2023-05-24 05:51:58.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/service.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/user.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/user.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/session.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     7576 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/translations.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-26 13:45:35.839212 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1704 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       77 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2023-05-26 13:45:35.840418 fusion-platform-python-sdk-1.7.1/setup.cfg
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1551 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/setup.py
```

### Comparing `fusion-platform-python-sdk-1.6.9/LICENSE.txt` & `fusion-platform-python-sdk-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/PKG-INFO` & `fusion-platform-python-sdk-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.6.9
+Version: 1.7.1
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusion-platform-python-sdk-1.6.9/README.md` & `fusion-platform-python-sdk-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/__init__.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 files, create and execute processes, monitor their execution and then download the corresponding results. Additional functionality is available directly via the
 API, and this is defined within the corresponding OpenAPI 3.0 specification, which can be obtained via a support request.
 
 &copy; [Digital Content Analysis Technology Ltd](https://www.d-cat.co.uk)
 """
 
 # Do not modify the following two lines as they are maintained by the version.sh script.
-__version__ = '1.6.9'
-__version_date__ = '2023-05-10T12:55:18Z'
+__version__ = '1.7.1'
+__version_date__ = '2023-05-26T13:45:33Z'
 
 # Exclude certain sub-modules from documentation.
 # @formatter:off
 __pdoc__ = {
     'base': False,
     'command': False,
     'common': False,
```

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/base.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/base.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/common/raise_thread.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/common/raise_thread.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/common/utilities.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/common/utilities.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/documentation.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/documentation.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/fusion_platform_sdk.pdf` & `fusion-platform-python-sdk-1.7.1/fusion_platform/fusion_platform_sdk.pdf`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/glasgow.geojson` & `fusion-platform-python-sdk-1.7.1/fusion_platform/glasgow.geojson`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/lake_district.geojson` & `fusion-platform-python-sdk-1.7.1/fusion_platform/lake_district.geojson`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/localisations.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/localisations.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/localise.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/localise.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/credit.md` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/credit.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/credit.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/credit.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/data.md` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/data.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/data.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/data.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/data_file.md` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/data_file.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/data_file.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/data_file.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/fields.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/fields.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/model.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,22 @@
     _PATH_CREATE = None
     _PATH_DELETE = None
     _PATH_GET = None
     _PATH_NEW = None
     _PATH_PATCH = None
 
     # Useful fields and templates.
+    _FIELD_AVAILABLE_DISPATCHERS = 'available_dispatchers'
     _FIELD_CONSTRAINED_NAMES = 'constrained_names'
     _FIELD_CONSTRAINED_VALUES = 'constrained_values'
     _FIELD_DATA_TYPE = 'data_type'
+    _FIELD_DISPATCH_INTERMEDIATE = 'dispatch_intermediate'
+    _FIELD_DISPATCHERS = 'dispatchers'
+    _FIELD_DOCUMENTATION_SUMMARY = 'documentation_summary'
+    _FIELD_DOCUMENTATION_DESCRIPTION = 'documentation_description'
     _FIELD_ERROR = 'error'
     _FIELD_EXECUTIONS = 'executions'
     _FIELD_FILE_TYPE = 'file_type'
     _FIELD_GROUP_COUNT = 'group_count'
     _FIELD_GROUP_ID = 'group_id'
     _FIELD_GROUP_INDEX = 'group_index'
     _FIELD_HAS_EXECUTIONS = 'has_executions'
@@ -515,39 +520,50 @@
             for item in response.get(Model._RESPONSE_KEY_LIST, []):
                 model = cls(session)
                 model._set_model_from_response(item, **kwargs)
                 model.__persisted = True
 
                 yield model
 
-    def _new(self, query_parameters=None, **kwargs):
+    def _new(self, query_parameters=None, extras=None, **kwargs):
         """
-        Gets a new template model object by loading it from the Fusion Platform<sup>&reg;</sup>. The explicit base model id value should be provided via a keyword argument. This
-        assumes the model is obtained using a GET RESTful request from the corresponding path, and that the model data is held with the expected dictionary key
-        within the response. The template model is then loaded using the supplied schema to obtain the corresponding Python representation of it, before loading
-        it into the model as a set of read-only attributes.
+        Gets a new template model object by loading it from the Fusion Platform<sup>&reg;</sup>. The explicit base model id value should be provided via a keyword
+        argument. This assumes the model is obtained using a GET RESTful request from the corresponding path, and that the model data is held with the expected
+        dictionary key within the response. The template model is then loaded using the supplied schema to obtain the corresponding Python representation of it,
+        before loading it into the model as a set of read-only attributes. If any extras are provided as a list of tuples (key, attribute), where key refers to the
+        field in the extras, and attribute is the corresponding model attribute to be set from the field, then each is added to the model.
 
         Args:
             query_parameters: The optional query parameters as a dictionary.
+            extras: The optional list of extras tuples (key, attribute) which should be added to the model.
             kwargs: Should include the base model id, if needed.
 
         Raises:
             RequestError: if the new fails.
             ModelError: if the model could not be loaded or validated from the Fusion Platform<sup>&reg;</sup>.
         """
         # Get the data.
         response = self._session.request(path=self._get_path(self.__class__._PATH_NEW, **kwargs), query_parameters=query_parameters)
 
         # Assume that the resulting model is held within the expected key within the resulting dictionary.
         if Model._RESPONSE_KEY_MODEL not in response:
-            raise ModelError(i18n.t('models.model.failed_model_new'))
+            raise ModelError(i18n.t('models.model.failed_model_new_model'))
+
+        # If any extras are required, extract them.
+        if (Model._RESPONSE_KEY_EXTRAS not in response) and (extras is not None):
+            raise ModelError(i18n.t('models.model.failed_model_new_extras'))
 
-        # Add in the keyword arguments to the response so that they are set in the model as well.
         modified_response = response.get(Model._RESPONSE_KEY_MODEL, {})
+        model_extras = response.get(Model._RESPONSE_KEY_EXTRAS, {})
 
+        for key, attribute in (extras if extras is not None else []):
+            if (key is not None) and (attribute is not None):
+                modified_response[attribute] = model_extras.get(key)
+
+        # Add in the keyword arguments to the response so that they are set in the model as well.
         for key, value in kwargs.items():
             modified_response[key] = value
 
         # Load the response into the model. We ignore missing required fields and those which are None.
         self._set_model_from_response(modified_response, partial=True)
 
         # The model is not persisted.
```

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/organisation.md` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/organisation.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/organisation.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/organisation.py`

 * *Files 13% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     _PATH_PATCH = _PATH_BASE
 
     # Add in the custom model paths.
     _PATH_DATA = f"{_PATH_BASE}/data/uploaded"
     _PATH_OWN_SERVICES = f"{_PATH_BASE}/services"
     _PATH_PROCESSES = f"{_PATH_BASE}/processes"
     _PATH_SERVICES = f"{_PATH_BASE}/services/latest"
+    _PATH_DISPATCHERS = f"{_PATH_BASE}/services/dispatchers"
 
     def create_data(self, name, file_type, files, wait=False):
         """
         Creates a data object for the organisation and uploads the corresponding files. Optionally waits for the upload and analysis to complete.
 
         Args:
             name: The name of the data object.
@@ -184,14 +185,36 @@
         filter = self.__class__._build_filter(
             [(self.__class__._FIELD_ID, self.__class__._FILTER_MODIFIER_EQ, id), (self.__class__._FIELD_NAME, self.__class__._FILTER_MODIFIER_BEGINS_WITH, name)])
 
         # Build the partial find generator and execute it.
         find = partial(Data._models_from_api_path, self._session, self._get_path(self.__class__._PATH_DATA), filter=filter, search=search)
         return self.__class__._first_and_generator(find)
 
+    def find_dispatchers(self, id=None, ssd_id=None, name=None, keyword=None, search=None):
+        """
+        Searches for dispatcher services with the specified id, SSD id, (non-unique) name and/or keywords, returning the first object found and an iterator.
+        Dispatchers are specific services used by processes to dispatch outputs to particular destinations. These services should not be used to form processes
+        themselves.
+
+        Args:
+            id: The service id to search for.
+            ssd_id: The SSD id to search for.
+            name: The name to search for (case-sensitive).
+            keyword: The keyword to search for (case-sensitive).
+            search: The term to search for (case-insensitive).
+
+        Returns:
+            The first found dispatcher service object, or None if not found, and an iterator through the found service objects.
+
+        Raises:
+            RequestError: if any get fails.
+            ModelError: if a model could not be loaded or validated from the Fusion Platform<sup>&reg;</sup>.
+        """
+        return self.__find_services(self.__class__._PATH_DISPATCHERS, id, ssd_id, name, keyword, search)
+
     def find_processes(self, id=None, name=None, search=None):
         """
         Searches for the organisation's processes with the specified id and/or (non-unique) name, returning the first object found and an iterator.
 
         Args:
             id: The process id to search for.
             name: The name to search for (case-sensitive).
@@ -207,19 +230,20 @@
         filter = self.__class__._build_filter(
             [(self.__class__._FIELD_ID, self.__class__._FILTER_MODIFIER_EQ, id), (self.__class__._FIELD_NAME, self.__class__._FILTER_MODIFIER_CONTAINS, name)])
 
         # Build the partial find generator and execute it.
         find = partial(Process._models_from_api_path, self._session, self._get_path(self.__class__._PATH_PROCESSES), filter=filter, search=search)
         return self.__class__._first_and_generator(find)
 
-    def find_services(self, id=None, ssd_id=None, name=None, keyword=None, search=None):
+    def __find_services(self, path, id=None, ssd_id=None, name=None, keyword=None, search=None):
         """
         Searches for services with the specified id, SSD id, (non-unique) name and/or keywords, returning the first object found and an iterator.
 
         Args:
+            path: The API path against which the search should be performed.
             id: The service id to search for.
             ssd_id: The SSD id to search for.
             name: The name to search for (case-sensitive).
             keyword: The keyword to search for (case-sensitive).
             search: The term to search for (case-insensitive).
 
         Returns:
@@ -232,17 +256,37 @@
         # Note that name is a key field, and hence we can only search using begins with.
         filter = self.__class__._build_filter(
             [(self.__class__._FIELD_ID, self.__class__._FILTER_MODIFIER_EQ, id), (self.__class__._FIELD_SSD_ID, self.__class__._FILTER_MODIFIER_EQ, ssd_id),
              (self.__class__._FIELD_NAME, self.__class__._FILTER_MODIFIER_BEGINS_WITH, name),
              (self.__class__._FIELD_KEYWORDS, self.__class__._FILTER_MODIFIER_CONTAINS, keyword)])
 
         # Build the partial find generator and execute it.
-        find = partial(Service._models_from_api_path, self._session, self._get_path(self.__class__._PATH_SERVICES), filter=filter, search=search)
+        find = partial(Service._models_from_api_path, self._session, self._get_path(path), filter=filter, search=search)
         return self.__class__._first_and_generator(find)
 
+    def find_services(self, id=None, ssd_id=None, name=None, keyword=None, search=None):
+        """
+        Searches for services with the specified id, SSD id, (non-unique) name and/or keywords, returning the first object found and an iterator.
+
+        Args:
+            id: The service id to search for.
+            ssd_id: The SSD id to search for.
+            name: The name to search for (case-sensitive).
+            keyword: The keyword to search for (case-sensitive).
+            search: The term to search for (case-insensitive).
+
+        Returns:
+            The first found service object, or None if not found, and an iterator through the found service objects.
+
+        Raises:
+            RequestError: if any get fails.
+            ModelError: if a model could not be loaded or validated from the Fusion Platform<sup>&reg;</sup>.
+        """
+        return self.__find_services(self.__class__._PATH_SERVICES, id, ssd_id, name, keyword, search)
+
     def new_process(self, name, service):
         """
         Creates a new template process from the service object. This process is not persisted to the Fusion Platform<sup>&reg;</sup>.
 
         Args:
             name: The name of the process.
             service: The service for which the process is to be created.
@@ -252,15 +296,16 @@
 
         Raises:
             RequestError: if the new fails.
             ModelError: if the model could not be created and validated by the Fusion Platform<sup>&reg;</sup>.
         """
         # Get a new template for the process model using the service.
         process = Process(self._session)
-        process._new(query_parameters={Model._get_id_name(Service.__name__): service.id}, organisation_id=self.id, name=name)
+        process._new(query_parameters={Model._get_id_name(Service.__name__): service.id},
+                     extras=[(self.__class__._FIELD_DISPATCHERS, self.__class__._FIELD_AVAILABLE_DISPATCHERS)], organisation_id=self.id, name=name)
 
         return process
 
     @property
     def own_services(self):
         """
         Provides an iterator through the services owned by the organisation. This includes services which may not yet be approved.
```

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/process.md` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/process_execution.md` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_execution.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/process_execution.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_execution.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/process_service_execution.md` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 * **created_at**: When was the record created?
 * **updated_at**: When was the record last updated?
 * **organisation_id**: The owning organisation.
 * **process_execution_id**: The specific execution of the process.
 * **process_id**: The process executed.
 * **service_id**: The explicit service version of the SSD which has been executed.
 * **image_id**: The image which was executed.
+* **chain_index**: The index in the processing chain for this executed service in the process.
 * **name**: The name of the service which has been executed.
 * **started_at**: When did the execution start?
 * **ended_at**: When did the execution end?
 * **runtime**: The execution runtime in seconds.
 * **cpu**: The number of CPUs used to run the image.
 * **memory**: The memory in megabytes used to run the image.
 * **actions**: The custom actions associated with this execution.
```

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/process_service_execution.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
     updated_at = fields.DateTime(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
 
     organisation_id = fields.UUID(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     process_execution_id = fields.UUID(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     process_id = fields.UUID(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     service_id = fields.UUID(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     image_id = fields.UUID(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
+    chain_index = fields.Integer(allow_none=True, metadata={'read_only': True})  # Changed to prevent this being updated.
 
     name = fields.String(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     started_at = fields.DateTime(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     ended_at = fields.DateTime(allow_none=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     runtime = fields.Integer(allow_none=True, metadata={'read_only': True})  # Changed to prevent this being updated.
 
     # Removed input_size.
```

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/process_service_execution_log.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution_log.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/service.md` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/service.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/service.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,15 @@
 
     organisation_id = fields.UUID(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     ssd_id = fields.UUID(required=True)
 
     version = fields.Integer(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     approval_status = fields.String(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     # Removed latest.
+    # Removed dispatcher.
     featured = fields.String(allow_none=True)
     show_in_latest = fields.Boolean(allow_none=True)  # Changed to optional.
     name = fields.String(required=True)
 
     categories = fields.List(fields.String(required=True), required=True)
     keywords = fields.List(fields.String(required=True), required=True)
```

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/user.md` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/user.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/models/user.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/models/user.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/session.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/session.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform/translations.py` & `fusion-platform-python-sdk-1.7.1/fusion_platform/translations.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,30 +54,33 @@
 i18n.add_translation('models.fields.datetime.format', '\'{input}\' cannot be formatted as a {obj_type}', 'en')
 i18n.add_translation('models.fields.datetime.invalid_awareness', 'Not a valid {awareness} {obj_type}', 'en')
 i18n.add_translation('models.fields.datetime.invalid', 'Not a valid {obj_type}', 'en')
 i18n.add_translation('models.fields.boolean.invalid', 'Not a valid boolean', 'en')
 i18n.add_translation('models.model.update_empty_body', 'Update cannot be requested as there are no attributes to be used (read-only attributes have been removed)', 'en')
 i18n.add_translation('models.model.create_empty_body', 'Create cannot be requested as there are no attributes to be used (read-only attributes have been removed)', 'en')
 i18n.add_translation('models.model.failed_model_validation', 'Failed to validate model: %{message}', 'en')
-i18n.add_translation('models.model.failed_model_new', 'Failed to get model template from response', 'en')
+i18n.add_translation('models.model.failed_model_new_extras', 'Failed to get model extras from response', 'en')
+i18n.add_translation('models.model.failed_model_new_model', 'Failed to get model template from response', 'en')
 i18n.add_translation('models.model.failed_model_send_and_load', 'Failed to request and load model', 'en')
 i18n.add_translation('models.model.no_such_keys', 'No such keys %{keys}', 'en')
 i18n.add_translation('models.model.readonly_property', 'Property %{property} is read-only and cannot be set', 'en')
 i18n.add_translation('models.model.not_persisted', 'Model is not persisted in the Fusion Platform(r)', 'en')
 i18n.add_translation('models.model.already_persisted', 'Model is already persisted in the Fusion Platform(r)', 'en')
 i18n.add_translation('models.process.failed_copy', 'Failed to get process from copy response', 'en')
 i18n.add_translation('models.process.execution_should_have_started', 'Process execution should have started by now', 'en')
 i18n.add_translation('models.process.execution_stopped', 'Process execution has been stopped', 'en')
 i18n.add_translation('models.process.wrong_file_type', 'File type of supplied data object (%{actual}) does not match the file type for the input (%{expected})', 'en')
 i18n.add_translation('models.process.data_not_ready', 'Data object is not ready to be used in a process', 'en')
 i18n.add_translation('models.process.option_wrong_type', 'Option value should be of type %{type}', 'en')
 i18n.add_translation('models.process.cannot_find_option', 'No such option', 'en')
 i18n.add_translation('models.process.cannot_find_input', 'No such input', 'en')
+i18n.add_translation('models.process.cannot_find_dispatcher', 'No such dispatcher', 'en')
 i18n.add_translation('models.process.option_not_specified', 'Option name or object must be provided to set option', 'en')
 i18n.add_translation('models.process.data_not_specified', 'Data object must be provided to set input', 'en')
 i18n.add_translation('models.process.input_not_specified', 'Input number or object must be provided to set input', 'en')
+i18n.add_translation('models.process.dispatcher_not_specified', 'Dispatcher number or name must be provided to add a dispatcher', 'en')
 i18n.add_translation('models.process.no_change_executing', 'Process cannot be modified as it is currently executing', 'en')
 i18n.add_translation('models.process.option.constrained_values.description', 'The constrained values for the option.', 'en')
 i18n.add_translation('models.process.option.constrained_values.title', 'Constrained Values', 'en')
 i18n.add_translation('models.process.option.constrained_names.description', 'The constrained value names for the option.', 'en')
 i18n.add_translation('models.process.option.constrained_names.title', 'Constrained Names', 'en')
 # @formatter:on
```

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform_python_sdk.egg-info/PKG-INFO` & `fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.6.9
+Version: 1.7.1
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusion-platform-python-sdk-1.6.9/fusion_platform_python_sdk.egg-info/SOURCES.txt` & `fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.9/setup.py` & `fusion-platform-python-sdk-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Find the package root directory.
 PACKAGE_DIR = pathlib.Path(__file__).parent
 
 # Set up the package.
 # @formatter:off
 setup(
     name='fusion-platform-python-sdk',
-    version='1.6.9',
+    version='1.7.1',
     description='Python SDK used to interact with the Fusion Platform(r)',
     long_description=(PACKAGE_DIR / 'README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/d-cat-support/fusion-platform-python-sdk',
     author='Digital Content Analysis Technology Ltd',
     author_email='support@d-cat.co.uk',
     license='MIT',
```

