# Comparing `tmp/fusion-platform-python-sdk-1.7.1.tar.gz` & `tmp/fusion-platform-python-sdk-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-platform-python-sdk-1.7.1.tar", last modified: Fri May 26 13:45:35 2023, max compression
+gzip compressed data, was "fusion-platform-python-sdk-1.7.2.tar", last modified: Wed Jun  7 06:23:21 2023, max compression
```

## Comparing `fusion-platform-python-sdk-1.7.1.tar` & `fusion-platform-python-sdk-1.7.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-26 13:45:35.840305 fusion-platform-python-sdk-1.7.1/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.7.1/LICENSE.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.7.1/MANIFEST.in
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-05-26 13:45:35.839925 fusion-platform-python-sdk-1.7.1/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4455 2022-09-01 10:14:11.000000 fusion-platform-python-sdk-1.7.1/README.md
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-26 13:45:35.789415 fusion-platform-python-sdk-1.7.1/fusion_platform/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     6806 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/__main__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/base.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/command.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-26 13:45:35.813316 fusion-platform-python-sdk-1.7.1/fusion_platform/common/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/common/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/common/raise_thread.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/common/utilities.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/documentation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)  1547331 2023-02-08 14:50:52.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/fusion_platform_sdk.pdf
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2237 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/glasgow.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)  1869438 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/lake_district.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/localisations.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/localise.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-26 13:45:35.831790 fusion-platform-python-sdk-1.7.1/fusion_platform/models/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/credit.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/credit.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/data.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/data.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/data_file.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/data_file.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/fields.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    31868 2023-05-24 14:20:34.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/model.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/organisation.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    14976 2023-05-25 09:18:19.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/organisation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    50701 2023-05-26 13:32:08.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2602 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     8982 2023-05-10 09:30:14.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3359 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10487 2023-05-23 06:25:23.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution_log.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution_log.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/service.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     9735 2023-05-24 05:51:58.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/service.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/user.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/models/user.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/session.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     7576 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/fusion_platform/translations.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-05-26 13:45:35.839212 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1704 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       77 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/requires.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2023-05-26 13:45:35.000000 fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2023-05-26 13:45:35.840418 fusion-platform-python-sdk-1.7.1/setup.cfg
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1551 2023-05-26 13:45:33.000000 fusion-platform-python-sdk-1.7.1/setup.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-06-07 06:23:21.607643 fusion-platform-python-sdk-1.7.2/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.7.2/LICENSE.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.7.2/MANIFEST.in
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-06-07 06:23:21.607130 fusion-platform-python-sdk-1.7.2/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4455 2022-09-01 10:14:11.000000 fusion-platform-python-sdk-1.7.2/README.md
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-06-07 06:23:21.582438 fusion-platform-python-sdk-1.7.2/fusion_platform/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     6806 2023-06-07 06:23:18.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/__main__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/base.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/command.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-06-07 06:23:21.586473 fusion-platform-python-sdk-1.7.2/fusion_platform/common/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/common/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/common/raise_thread.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/common/utilities.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/documentation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  1593164 2023-06-07 06:22:45.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/fusion_platform_sdk.pdf
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2237 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/glasgow.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  1869438 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/lake_district.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/localisations.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/localise.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-06-07 06:23:21.602126 fusion-platform-python-sdk-1.7.2/fusion_platform/models/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2023-06-07 06:23:19.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/credit.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/credit.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2023-06-07 06:23:19.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/data.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/data.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2023-06-07 06:23:19.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/data_file.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/data_file.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/fields.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    31868 2023-05-24 14:20:34.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/model.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2023-06-07 06:23:19.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/organisation.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    14976 2023-05-25 09:18:19.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/organisation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2023-06-07 06:23:19.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/process.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    50701 2023-05-26 13:32:08.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/process.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2602 2023-06-07 06:23:19.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/process_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     8982 2023-05-10 09:30:14.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/process_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3359 2023-06-07 06:23:19.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/process_service_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10487 2023-05-23 06:25:23.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/process_service_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2023-06-07 06:23:19.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/process_service_execution_log.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/process_service_execution_log.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2023-06-07 06:23:19.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/service.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     9735 2023-05-24 05:51:58.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/service.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2023-06-07 06:23:19.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/user.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/models/user.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/session.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     7576 2023-06-07 06:23:18.000000 fusion-platform-python-sdk-1.7.2/fusion_platform/translations.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-06-07 06:23:21.606238 fusion-platform-python-sdk-1.7.2/fusion_platform_python_sdk.egg-info/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-06-07 06:23:21.000000 fusion-platform-python-sdk-1.7.2/fusion_platform_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1704 2023-06-07 06:23:21.000000 fusion-platform-python-sdk-1.7.2/fusion_platform_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2023-06-07 06:23:21.000000 fusion-platform-python-sdk-1.7.2/fusion_platform_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       77 2023-06-07 06:23:21.000000 fusion-platform-python-sdk-1.7.2/fusion_platform_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2023-06-07 06:23:21.000000 fusion-platform-python-sdk-1.7.2/fusion_platform_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2023-06-07 06:23:21.000000 fusion-platform-python-sdk-1.7.2/fusion_platform_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2023-06-07 06:23:21.607841 fusion-platform-python-sdk-1.7.2/setup.cfg
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1551 2023-06-07 06:23:18.000000 fusion-platform-python-sdk-1.7.2/setup.py
```

### Comparing `fusion-platform-python-sdk-1.7.1/LICENSE.txt` & `fusion-platform-python-sdk-1.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/PKG-INFO` & `fusion-platform-python-sdk-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusion-platform-python-sdk-1.7.1/README.md` & `fusion-platform-python-sdk-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/__init__.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 files, create and execute processes, monitor their execution and then download the corresponding results. Additional functionality is available directly via the
 API, and this is defined within the corresponding OpenAPI 3.0 specification, which can be obtained via a support request.
 
 &copy; [Digital Content Analysis Technology Ltd](https://www.d-cat.co.uk)
 """
 
 # Do not modify the following two lines as they are maintained by the version.sh script.
-__version__ = '1.7.1'
-__version_date__ = '2023-05-26T13:45:33Z'
+__version__ = '1.7.2'
+__version_date__ = '2023-06-07T06:23:18Z'
 
 # Exclude certain sub-modules from documentation.
 # @formatter:off
 __pdoc__ = {
     'base': False,
     'command': False,
     'common': False,
```

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/base.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/base.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/common/raise_thread.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/common/raise_thread.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/common/utilities.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/common/utilities.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/documentation.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/documentation.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/fusion_platform_sdk.pdf` & `fusion-platform-python-sdk-1.7.2/fusion_platform/fusion_platform_sdk.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 2% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,15 +1,15 @@
 Digital Content Analysis Technology Ltd
 
 Fusion Platform®
 
 Python SDK
 
-Version 1.6
-8th February 2023
+Version 1.7
+7th June 2023
 
 Digital Content Analysis Technology Ltd
 
 Table of Contents
 1
 
 Introduction ..................................................................................................... 4
@@ -64,28 +64,28 @@
 
 7
 
 Creating Processes ......................................................................................... 20
 
 8
 
-Executing and Monitoring Processes .............................................................. 24
+Executing and Monitoring Processes .............................................................. 26
 
 9
 
-Obtaining Execution Inputs and Outputs ........................................................ 28
+Obtaining Execution Inputs and Outputs ........................................................ 30
 
-10 Detailed Example ........................................................................................... 30
-11 SDK Object Attributes and Methods ............................................................... 34
+10 Detailed Example ........................................................................................... 32
+11 SDK Object Attributes and Methods ............................................................... 36
 11.1
 
-Attributes and Methods ................................................................................................................. 34
+Attributes and Methods ................................................................................................................. 36
 
-12 Glossary of Terms........................................................................................... 36
-13 References ..................................................................................................... 38
+12 Glossary of Terms........................................................................................... 38
+13 References ..................................................................................................... 40
 
 2
 
 Digital Content Analysis Technology Ltd
 
 Revision History
 
@@ -206,21 +206,47 @@
 
 Version 1.5
 
 29th November 2022
 
 Issued for Fusion Platform® version 1.5.
 
+Version 1.6
+
+8th February 2023
+
+Issued for Fusion Platform® version 1.6.
+
+rd
+
+Draft
+
+3 May 2023
+
+Added changed_delete_expiry method for process execution.
+
+Draft
+
+23rd May 2023
+
+Added the ability to include dispatchers within a process.
+
+Version 1.7
+
+7th June 2023
+
+Issued for Fusion Platform® version 1.7.
+
 This document has been prepared by Digital Content Analysis Technology Ltd, who can be
 contacted at support@d-cat.co.uk
 Digital Content Analysis Technology Ltd, Registered in Scotland, SC499652.
 This document is copyright and is issued on the strict understanding that it is not to be
 reproduced, copied, or disclosed to a third party, in whole or in part, without the consent of
 Digital Content Analysis Technology Ltd.
-© 2022 Digital Content Analysis Technology Ltd
+© 2023 Digital Content Analysis Technology Ltd
 3
 
 Digital Content Analysis Technology Ltd
 
 1
 
 Introduction
@@ -352,17 +378,17 @@
 will be sent via email or text message to the user account which executed the process to notify
 that the execution or group of executions has finished.
 It is also possible to stop all executions of a process. This will stop all ongoing and future
 executions. Any partial executions will be subject to the associated portion of the charges
 incurred.
 7. Download the outputs from the executed process
 When an execution has completed successfully, the outputs can be downloaded. All the inputs
-and outputs to an execution, and its individual steps, are available for download. The
-individual steps will include, for example, the ingestion of data, so that all the data used by
-the process is available for download.
+to and outputs from an execution are available for download. It also possible to configure a
+process to automatically dispatch outputs to, for example, an AWS S3 bucket, so that the
+download is unnecessary.
 8. Delete completed process
 When a process and its outputs are no longer needed, the process can be deleted. Executions
 will be automatically deleted after a delay configured when the process is created. Deleting a
 process will delete all its executions and their outputs (and therefore stop any further storage
 charges being incurred). Files which have been uploaded explicitly by the user are not
 automatically deleted, only executions and their generated data.
 
@@ -951,65 +977,120 @@
 # ...or using a schedule, which will run the job once, tomorrow.
 then = datetime.now(timezone.utc) + timedelta(days=1)
 process.update(run_type=fusion_platform.RUN_TYPE_RUN_SCHEDULE,
 repeat_count=1, repeat_start=then)
 
 Full details on options, inputs and scheduling can be found in the process information. Section
 11 describes how to get help on the content of the process information.
-When the process has been correctly configured, it can be saved to the Fusion Platform®.
-During this creation, the process will be validated and its corresponding price per execution
-calculated. If the process fails validation, then an exception will be thrown, and the process
-will not be saved.
+In addition to correctly configuring the process input, options and schedule, the process can
+also be configured to dispatch outputs using the available set of dispatchers. For example, a
+dispatcher can be used to automatically send the outputs of the process to an AWS S3 bucket.
 
 22
 
 Digital Content Analysis Technology Ltd
+
+The list of available dispatchers and their options can be obtained from the process model
+using the following:
+Python
+# Find out what dispatchers are available. This will list
+# all the dispatchers with their name and brief description, plus
+# also print out their options.
+for dispatcher in process.available_dispatchers:
+print(dispatcher)
+for option in dispatcher.options:
+print(option)
+
+A dispatcher can be added to the process using the following:
+Python
+# Add the first dispatcher from the list of those available.
+process.add_dispatcher(number=1)
+
+# A dispatcher can also be added using its name.
+process.add_dispatcher(name='AWS S3')
+
+Once a dispatcher has been added to the process, it can be configured and its options set
+using the following:
+Python
+# Configure the options of the first dispatcher which has
+# been added to the process. Note that an option object cannot be
+# used to modify a dispatcher option.
+process.update(dispatcher_number=1, option_name='bucket',
+value='my-bucket')
+
+To view the list of dispatchers which have been added to a process, use the following:
+Python
+# Find out what dispatchers have been added to a process.
+# This will list all the dispatchers with their name and brief
+# description, plus also print out their options.
+for dispatcher in process.dispatchers:
+print(dispatcher)
+for option in dispatcher.options:
+print(option)
+
+23
+
+Digital Content Analysis Technology Ltd
+
+To remove a dispatcher, use the following:
+Python
+# Remove the first dispatcher from the list of those added.
+process.remove_dispatcher(number=1)
+
+When the process has been correctly configured, it can be saved to the Fusion Platform®.
+During this creation, the process will be validated and its corresponding price per execution
+calculated. If the process fails validation, then an exception will be thrown, and the process
+will not be saved.
 Python
 # Attempt to create the process which will first validate it.
 # This will throw an exception if the validation fails.
 process.create()
 # Once created, the price will be available to review.
 print(process.price)
 Important
 
-Prior to execution, the name, options, inputs and schedule of a process may be changed
-using the ‘update’ method. However, once the process has been submitted for
-execution, no values can be changed. If the process is stopped, then the name and
+Prior to execution, the name, options, inputs, schedule and dispatchers of a process may
+be changed using the ‘update’ method. However, once the process has been submitted
+for execution, no values can be changed. If the process is stopped, then the name and
 schedule only may be changed. To change any other values, use a copy of the process
 instead. To obtain a copy, use the ‘copy’ method, which will provide a template process
 with the same values as the original.
 A template process, which is a copy of a process which has already been created or executed,
-can be obtained as follows. This will copy the options, inputs and schedule from the previous
-process, set the name, and then the new template process can be used to modify any of these
-values before being created.
+can be obtained as follows. This will copy the options, inputs, schedule and dispatchers from
+the previous process, set the name, and then the new template process can be used to modify
+any of these values before being created.
 Python
 # Create a copy of a process which has previously been
 # created or executed. This copies the name, options, inputs
 # and schedule.
 process_copy = process.copy(name='Copy of Example')
 # Just like any other new template process, the values can be
 # updated. Here we schedule the execution.
 then = datetime.now(timezone.utc) + timedelta(days=1)
 process_copy.update(
 run_type=fusion_platform.RUN_TYPE_RUN_SCHEDULE,
 repeat_count=1, repeat_start=then)
 # The copied process may then be created.
 process_copy.create()
 
+24
+
+Digital Content Analysis Technology Ltd
+
 When the process is no longer needed, it may be deleted:
 Python
 # Delete the process:
 process.delete()
 
 This will raise an exception in case of insufficient privileges, otherwise the process will be
 deleted. This will first stop any current executions and prevent any further executions taking
 place. Then this will delete any existing executions and their associated outputs, before
 deleting the process itself. This deletion cannot be undone.
 
-23
+25
 
 Digital Content Analysis Technology Ltd
 
 8
 
 Executing and Monitoring Processes
 An iterator through the processes which have been validated and saved for an organisation
@@ -1048,15 +1129,15 @@
 # wait for completion.
 process.execute()
 
 This will execute a process according to its options, inputs and schedule. Every execution will
 incur the price listed with the process. This method will return immediately and will not wait
 for the execution to complete.
 
-24
+26
 
 Digital Content Analysis Technology Ltd
 Important
 
 Once a process has been executed, it may not be modified. To modify the name or
 schedule, the process must first be stopped. To modify any other values, a copy can be
 created of the process.
@@ -1095,15 +1176,15 @@
 time.sleep(10)
 
 # Sleep for 10 seconds.
 
 # The execution has completed without exception.
 print('Execution successfully completed')
 
-25
+27
 
 Digital Content Analysis Technology Ltd
 
 To have the method wait for the execution to complete, turn the ‘wait’ flag on:
 Python
 # Wait for the execution to complete.
 execution.check_complete(wait=True)
@@ -1140,28 +1221,29 @@
 Every process is configured with an output storage period in days which determines how long
 each execution is kept before it is automatically deleted. Prior to deletion, an optional
 notification may be sent via email or text message to the user account which executed the
 process to warn that the execution will be deleted shortly.
 If the automatic deletion should be delayed further, then this delete expiry can be modified
 for an execution as follows:
 
-26
+28
 
 Digital Content Analysis Technology Ltd
 Python
 # Change the delete expiry for an execution to delay it
 # from being deleted for 2 days from now.
 delete_expiry = datetime.now(timezone.utc) + timedelta(days=2)
-execution.update(delete_expiry=delete_expiry)
+execution.change_delete_expiry(delete_expiry=delete_expiry)
 
 If the update fails for any reason, such as invalid parameter values or insufficient privileges,
-then an exception will be thrown. Extending the expiry will mean that additional storage costs
-are incurred for the extra time that the execution’s outputs are stored. All storage charges are
-collated daily. Section 11 describes how to get help on the content of the execution
-information.
+then an exception will be thrown. If the execution is part of a group, then this will also change
+the delete expiry for all executions in the same group. Extending the expiry will mean that
+additional storage costs are incurred for the extra time that the execution’s outputs are
+stored. All storage charges are collated daily. Section 11 describes how to get help on the
+content of the execution information.
 Process executions can be stopped at any time by using the following:
 Python
 # Stop all executions of a process, aborting those running:
 process.stop()
 
 This will first stop the process from running any more executions as per its schedule. It will
 then abort any executions which are in progress. Partial charges will still be incurred for any
@@ -1169,15 +1251,15 @@
 Important
 
 If the process is configured to run only once, then when it has been executed, the process
 will automatically be set to stopped. This enables the process to be run again using the
 same inputs and options. When stopped, the name and schedule for a process may be
 modified.
 
-27
+29
 
 Digital Content Analysis Technology Ltd
 
 9
 
 Obtaining Execution Inputs and Outputs
 Once an execution has completed, then its inputs and outputs can be downloaded. Each
@@ -1212,15 +1294,15 @@
 # Select the first input for a component in this example:
 input = next(component.inputs)
 # Download all files from the input to the local directory:
 for file in input.files:
 print(f"Downloading {file.file_name} ({file.size} bytes)")
 file.download(path=file.file_name)
 
-28
+30
 
 Digital Content Analysis Technology Ltd
 
 Similarly, the files from an output can also be downloaded:
 Python
 # Select the first output for a component in this example:
 output = next(component.output)
@@ -1243,15 +1325,15 @@
 
 The inputs and outputs of an execution are transient and are only available while the
 execution exists. If the execution is deleted, then its inputs and outputs are also deleted.
 To persist any input or output beyond an execution, it can be copied using the ‘copy’
 method for the corresponding data object. All copies are treated as if they have been
 uploaded and therefore exist until they are explicitly deleted.
 
-29
+31
 
 Digital Content Analysis Technology Ltd
 
 10
 
 Detailed Example
 The following shows a detailed example of how to use the SDK to create a process, execute it
@@ -1290,15 +1372,15 @@
 # Find the cloud classification service using its name.
 service, _ = organisation.find_services(
 name='Demo: Sentinel-2 Cloud Classification')
 # Create a template process from the service.
 process = organisation.new_process(name='Example',
 service=service)
 
-30
+32
 
 Digital Content Analysis Technology Ltd
 Python
 # Configure the process to use Lake District National Park
 # as the region of interest.
 process.update(input_number=1, data=lake_district)
 # Configure the service to work on historic data.
@@ -1334,15 +1416,15 @@
 
 # First file only.
 
 files.append(file)
 statistics_path = file.file_name
 file.download(path=statistics_path)
 
-31
+33
 
 Digital Content Analysis Technology Ltd
 Python
 elif component.name == 'Sentinel-2 Cloud Classification':
 print(f"Downloading output from {component.id}")
 output = next(component.outputs)
 file = next(output.files)
@@ -1372,15 +1454,15 @@
 with rasterio.open('mosaic.tif', 'w', ** mosaic_meta) as merged:
 merged.write(mosaic)
 # Display the mosaic image.
 with rasterio.open('mosaic.tif', 'r') as source:
 pyplot.imshow(source.read(1, masked=True), cmap='coolwarm')
 pyplot.show()
 
-32
+34
 
 Digital Content Analysis Technology Ltd
 Python
 # Display the histogram.
 histogram = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
 for metadata in selectors:
 histogram = [first + second for first, second in
@@ -1390,15 +1472,15 @@
 y = [histogram[0], histogram[3], histogram[6], histogram[9]]
 pyplot.bar(x, y)
 pyplot.show()
 # Tidy everything up by deleting the process and the input file.
 process.delete()
 lake_district.delete()
 
-33
+35
 
 Digital Content Analysis Technology Ltd
 
 11
 
 SDK Object Attributes and Methods
 The SDK consists of package functions which control the overall behaviour of the SDK, and
@@ -1476,15 +1558,15 @@
 which allows a template process to be initialised for an organisation.
 
 Attributes and Methods
 Detailed information about the available attributes and methods for the package and its
 classes used to form model objects can be obtained from:
 https://www.d-cat.co.uk/public/fusion_platform_python_sdk/
 
-34
+36
 
 Digital Content Analysis Technology Ltd
 
 Similar information can also be obtained in Python using the following:
 Python
 import fusion_platform
 # Get help on the package methods:
@@ -1492,15 +1574,15 @@
 
 Help on individual classes can be obtained in a similar way:
 Python
 from fusion_platform.models.user import User
 # Get help on the user class:
 help(User)
 
-35
+37
 
 Digital Content Analysis Technology Ltd
 
 12
 
 Glossary of Terms
 Application Programming Interface (API) Typically refers to a software interface (rather
@@ -1581,15 +1663,15 @@
 OpenAPI 3.0 Specification [3]
 
 The standardised specification of a RESTful API
 interface which can be used to document or access
 the API with suitable software which can read the
 specification.
 
-36
+38
 
 Digital Content Analysis Technology Ltd
 
 Portable Network Graphics (PNG)
 
 A type of image file format which uses lossless
 data compression.
@@ -1639,25 +1721,25 @@
 (“?id=1&name=User”).
 
 Zip Archive
 
 A single file which contains other files which have
 been compressed.
 
-37
+39
 
 Digital Content Analysis Technology Ltd
 
 13
 
 References
 [1] QGIS, “Welcome to the QGIS project!,” 2022. [Online]. Available: https://www.qgis.org.
 [Accessed February 2022].
 [2] Mapbox, “geojson.io,” 2022. [Online]. Available: https://geojson.io. [Accessed February
 2022].
 [3] Linux Foundation, “OpenAPI Specification v3.0.3 | Introduction, Definitions, & More,”
 2020. [Online]. Available: https://spec.openapis.org/oas/v3.0.3.html. [Accessed March
 2022].
 
-38
+40
```

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/glasgow.geojson` & `fusion-platform-python-sdk-1.7.2/fusion_platform/glasgow.geojson`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/lake_district.geojson` & `fusion-platform-python-sdk-1.7.2/fusion_platform/lake_district.geojson`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/localisations.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/localisations.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/localise.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/localise.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/credit.md` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/credit.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/credit.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/credit.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/data.md` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/data.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/data.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/data.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/data_file.md` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/data_file.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/data_file.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/data_file.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/fields.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/fields.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/model.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/model.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/organisation.md` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/organisation.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/organisation.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/organisation.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process.md` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/process.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/process.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_execution.md` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/process_execution.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_execution.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/process_execution.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution.md` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/process_service_execution.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/process_service_execution.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/process_service_execution_log.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/process_service_execution_log.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/service.md` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/service.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/service.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/service.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/user.md` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/user.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/models/user.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/models/user.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/session.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/session.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform/translations.py` & `fusion-platform-python-sdk-1.7.2/fusion_platform/translations.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/PKG-INFO` & `fusion-platform-python-sdk-1.7.2/fusion_platform_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusion-platform-python-sdk-1.7.1/fusion_platform_python_sdk.egg-info/SOURCES.txt` & `fusion-platform-python-sdk-1.7.2/fusion_platform_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.1/setup.py` & `fusion-platform-python-sdk-1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Find the package root directory.
 PACKAGE_DIR = pathlib.Path(__file__).parent
 
 # Set up the package.
 # @formatter:off
 setup(
     name='fusion-platform-python-sdk',
-    version='1.7.1',
+    version='1.7.2',
     description='Python SDK used to interact with the Fusion Platform(r)',
     long_description=(PACKAGE_DIR / 'README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/d-cat-support/fusion-platform-python-sdk',
     author='Digital Content Analysis Technology Ltd',
     author_email='support@d-cat.co.uk',
     license='MIT',
```

