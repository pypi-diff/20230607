# Comparing `tmp/MRdataset-0.1.3.tar.gz` & `tmp/MRdataset-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MRdataset-0.1.3.tar", last modified: Fri Nov  4 21:26:06 2022, max compression
+gzip compressed data, was "MRdataset-0.1.6.tar", last modified: Wed Jun  7 17:10:34 2023, max compression
```

## Comparing `MRdataset-0.1.3.tar` & `MRdataset-0.1.6.tar`

### file list

```diff
@@ -1,55 +1,62 @@
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2022-11-04 21:26:06.000000 MRdataset-0.1.3/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       89 2022-06-21 16:48:36.000000 MRdataset-0.1.3/HISTORY.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      584 2022-11-04 21:26:06.000000 MRdataset-0.1.3/setup.cfg
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      587 2022-06-21 16:48:36.000000 MRdataset-0.1.3/LICENSE
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      195 2022-09-06 20:52:38.000000 MRdataset-0.1.3/AUTHORS.rst
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2022-11-04 21:26:06.000000 MRdataset-0.1.3/MRdataset.egg-info/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       76 2022-11-04 21:26:06.000000 MRdataset-0.1.3/MRdataset.egg-info/entry_points.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       60 2022-11-04 21:26:06.000000 MRdataset-0.1.3/MRdataset.egg-info/requires.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2713 2022-11-04 21:26:06.000000 MRdataset-0.1.3/MRdataset.egg-info/PKG-INFO
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       10 2022-11-04 21:26:06.000000 MRdataset-0.1.3/MRdataset.egg-info/top_level.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        1 2022-11-04 21:26:06.000000 MRdataset-0.1.3/MRdataset.egg-info/not-zip-safe
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        1 2022-11-04 21:26:06.000000 MRdataset-0.1.3/MRdataset.egg-info/dependency_links.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      996 2022-11-04 21:26:06.000000 MRdataset-0.1.3/MRdataset.egg-info/SOURCES.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      314 2022-09-09 16:23:42.000000 MRdataset-0.1.3/MANIFEST.in
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1598 2022-09-09 20:54:42.000000 MRdataset-0.1.3/setup.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2713 2022-11-04 21:26:06.000000 MRdataset-0.1.3/PKG-INFO
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     3550 2022-09-06 20:50:53.000000 MRdataset-0.1.3/CONTRIBUTING.rst
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2022-11-04 21:26:06.000000 MRdataset-0.1.3/docs/
--rwxrwxr-x   0 sinhah    (1000) sinhah    (1000)     5051 2022-09-09 16:10:26.000000 MRdataset-0.1.3/docs/conf.py
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2022-11-04 21:26:06.000000 MRdataset-0.1.3/docs/build/
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2022-11-04 21:26:06.000000 MRdataset-0.1.3/docs/build/html/
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2022-11-04 21:26:06.000000 MRdataset-0.1.3/docs/build/html/_static/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      286 2022-01-31 15:50:09.000000 MRdataset-0.1.3/docs/build/html/_static/file.png
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       90 2022-01-31 15:50:09.000000 MRdataset-0.1.3/docs/build/html/_static/plus.png
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       90 2022-01-31 15:50:09.000000 MRdataset-0.1.3/docs/build/html/_static/minus.png
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       64 2022-09-09 19:00:19.000000 MRdataset-0.1.3/docs/modules.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       28 2022-06-21 16:48:36.000000 MRdataset-0.1.3/docs/history.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      806 2022-09-09 18:00:16.000000 MRdataset-0.1.3/docs/make.bat
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      609 2022-09-09 18:00:15.000000 MRdataset-0.1.3/docs/Makefile
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       33 2022-06-21 16:48:36.000000 MRdataset-0.1.3/docs/contributing.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      475 2022-09-09 18:12:48.000000 MRdataset-0.1.3/docs/index.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       28 2022-06-21 16:48:36.000000 MRdataset-0.1.3/docs/authors.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)  1402324 2022-10-31 20:50:15.000000 MRdataset-0.1.3/docs/mrQA1.png
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      527 2022-09-06 20:57:49.000000 MRdataset-0.1.3/docs/MRdataset.tests.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       27 2022-06-21 16:48:36.000000 MRdataset-0.1.3/docs/readme.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1154 2022-09-06 20:49:43.000000 MRdataset-0.1.3/docs/installation.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1096 2022-10-13 20:22:16.000000 MRdataset-0.1.3/docs/MRdataset.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1897 2022-10-13 20:22:16.000000 MRdataset-0.1.3/README.rst
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2022-11-04 21:26:06.000000 MRdataset-0.1.3/MRdataset/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      497 2022-11-04 21:26:06.000000 MRdataset-0.1.3/MRdataset/_version.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      332 2022-07-13 15:35:48.000000 MRdataset-0.1.3/MRdataset/__mrdataset__.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     6115 2022-10-30 20:15:58.000000 MRdataset-0.1.3/MRdataset/bids_dataset.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     4040 2022-10-28 15:16:03.000000 MRdataset-0.1.3/MRdataset/utils.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    21555 2022-10-27 21:06:03.000000 MRdataset-0.1.3/MRdataset/base.py
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2022-11-04 21:26:06.000000 MRdataset-0.1.3/MRdataset/tests/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      180 2022-07-24 21:50:18.000000 MRdataset-0.1.3/MRdataset/tests/config.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1689 2022-07-25 16:26:45.000000 MRdataset-0.1.3/MRdataset/tests/test_MRdataset.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       39 2022-06-21 16:48:36.000000 MRdataset-0.1.3/MRdataset/tests/__init__.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     6465 2022-09-09 17:54:25.000000 MRdataset-0.1.3/MRdataset/config.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     5938 2022-10-31 15:40:06.000000 MRdataset-0.1.3/MRdataset/dicom_dataset.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2798 2022-10-27 21:34:20.000000 MRdataset-0.1.3/MRdataset/cli.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     6097 2022-10-14 18:54:11.000000 MRdataset-0.1.3/MRdataset/simulate.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    12743 2022-10-27 19:18:13.000000 MRdataset-0.1.3/MRdataset/common_dicom.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      245 2022-09-09 16:23:42.000000 MRdataset-0.1.3/MRdataset/__init__.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    81180 2022-09-09 16:24:48.000000 MRdataset-0.1.3/versioneer.py
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:10:34.560889 MRdataset-0.1.6/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      227 2023-06-07 17:08:43.000000 MRdataset-0.1.6/AUTHORS.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     3550 2022-09-06 20:50:53.000000 MRdataset-0.1.6/CONTRIBUTING.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      587 2022-06-21 16:48:36.000000 MRdataset-0.1.6/LICENSE
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      294 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MANIFEST.in
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:10:34.560889 MRdataset-0.1.6/MRdataset/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      302 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/__init__.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      332 2022-07-13 15:35:48.000000 MRdataset-0.1.6/MRdataset/__mrdataset__.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      497 2023-06-07 17:10:34.560889 MRdataset-0.1.6/MRdataset/_version.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    30840 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/base.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     6659 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/bids_utils.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2805 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/cli.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     5736 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/common.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     5798 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/config.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     6587 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/dicom.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    17340 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/dicom_utils.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     3402 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/fastbids.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      931 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/log.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     7665 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/naive_bids.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     6103 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/simulate.py
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:10:34.560889 MRdataset-0.1.6/MRdataset/tests/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       39 2022-06-21 16:48:36.000000 MRdataset-0.1.6/MRdataset/tests/__init__.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      180 2022-07-24 21:50:18.000000 MRdataset-0.1.6/MRdataset/tests/config.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1989 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/tests/test_MRdataset.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      522 2023-03-23 20:22:50.000000 MRdataset-0.1.6/MRdataset/tests/test_functions.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2792 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/tests/test_merge.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    11284 2023-06-07 17:08:43.000000 MRdataset-0.1.6/MRdataset/utils.py
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:10:34.556888 MRdataset-0.1.6/MRdataset.egg-info/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1331 2023-06-07 17:10:34.000000 MRdataset-0.1.6/MRdataset.egg-info/PKG-INFO
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1147 2023-06-07 17:10:34.000000 MRdataset-0.1.6/MRdataset.egg-info/SOURCES.txt
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        1 2023-06-07 17:10:34.000000 MRdataset-0.1.6/MRdataset.egg-info/dependency_links.txt
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       75 2023-06-07 17:10:34.000000 MRdataset-0.1.6/MRdataset.egg-info/entry_points.txt
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        1 2023-06-07 17:10:34.000000 MRdataset-0.1.6/MRdataset.egg-info/not-zip-safe
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       67 2023-06-07 17:10:34.000000 MRdataset-0.1.6/MRdataset.egg-info/requires.txt
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       10 2023-06-07 17:10:34.000000 MRdataset-0.1.6/MRdataset.egg-info/top_level.txt
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1331 2023-06-07 17:10:34.560889 MRdataset-0.1.6/PKG-INFO
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      515 2023-06-07 17:08:43.000000 MRdataset-0.1.6/README.rst
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:10:34.560889 MRdataset-0.1.6/docs/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1151 2023-06-07 17:08:43.000000 MRdataset-0.1.6/docs/API.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      609 2022-09-09 18:00:15.000000 MRdataset-0.1.6/docs/Makefile
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       28 2022-06-21 16:48:36.000000 MRdataset-0.1.6/docs/authors.rst
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:10:34.556888 MRdataset-0.1.6/docs/build/
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:10:34.556888 MRdataset-0.1.6/docs/build/html/
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:10:34.560889 MRdataset-0.1.6/docs/build/html/_images/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    69541 2023-04-02 18:36:05.000000 MRdataset-0.1.6/docs/build/html/_images/hierarchy.jpg
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:10:34.560889 MRdataset-0.1.6/docs/build/html/_static/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      286 2022-07-14 07:38:19.000000 MRdataset-0.1.6/docs/build/html/_static/file.png
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       90 2022-07-14 07:38:19.000000 MRdataset-0.1.6/docs/build/html/_static/minus.png
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       90 2022-07-14 07:38:19.000000 MRdataset-0.1.6/docs/build/html/_static/plus.png
+-rwxrwxr-x   0 sinhah    (1000) sinhah    (1000)     5256 2023-06-07 17:08:43.000000 MRdataset-0.1.6/docs/conf.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       33 2022-06-21 16:48:36.000000 MRdataset-0.1.6/docs/contributing.rst
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:10:34.560889 MRdataset-0.1.6/docs/images/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    69541 2023-06-07 17:08:43.000000 MRdataset-0.1.6/docs/images/hierarchy.jpg
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      761 2023-06-07 17:08:43.000000 MRdataset-0.1.6/docs/index.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1161 2023-06-07 17:08:43.000000 MRdataset-0.1.6/docs/installation.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      806 2022-09-09 18:00:16.000000 MRdataset-0.1.6/docs/make.bat
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)  1402324 2022-10-31 20:50:15.000000 MRdataset-0.1.6/docs/mrQA1.png
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    45098 2023-06-07 17:08:43.000000 MRdataset-0.1.6/docs/mrdataset-structure.png
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2211 2023-06-07 17:08:43.000000 MRdataset-0.1.6/docs/usage.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      584 2023-06-07 17:10:34.560889 MRdataset-0.1.6/setup.cfg
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1605 2023-06-07 17:08:43.000000 MRdataset-0.1.6/setup.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    81180 2022-09-09 16:24:48.000000 MRdataset-0.1.6/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `MRdataset-0.1.3/setup.cfg` & `MRdataset-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `MRdataset-0.1.3/LICENSE` & `MRdataset-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MRdataset-0.1.3/MRdataset.egg-info/SOURCES.txt` & `MRdataset-0.1.6/MRdataset.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 AUTHORS.rst
 CONTRIBUTING.rst
-HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 versioneer.py
 MRdataset/__init__.py
 MRdataset/__mrdataset__.py
 MRdataset/_version.py
 MRdataset/base.py
-MRdataset/bids_dataset.py
+MRdataset/bids_utils.py
 MRdataset/cli.py
-MRdataset/common_dicom.py
+MRdataset/common.py
 MRdataset/config.py
-MRdataset/dicom_dataset.py
+MRdataset/dicom.py
+MRdataset/dicom_utils.py
+MRdataset/fastbids.py
+MRdataset/log.py
+MRdataset/naive_bids.py
 MRdataset/simulate.py
 MRdataset/utils.py
 MRdataset.egg-info/PKG-INFO
 MRdataset.egg-info/SOURCES.txt
 MRdataset.egg-info/dependency_links.txt
 MRdataset.egg-info/entry_points.txt
 MRdataset.egg-info/not-zip-safe
 MRdataset.egg-info/requires.txt
 MRdataset.egg-info/top_level.txt
 MRdataset/tests/__init__.py
 MRdataset/tests/config.py
 MRdataset/tests/test_MRdataset.py
-docs/MRdataset.rst
-docs/MRdataset.tests.rst
+MRdataset/tests/test_functions.py
+MRdataset/tests/test_merge.py
+docs/API.rst
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
-docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
-docs/modules.rst
 docs/mrQA1.png
-docs/readme.rst
+docs/mrdataset-structure.png
+docs/usage.rst
+docs/build/html/_images/hierarchy.jpg
 docs/build/html/_static/file.png
 docs/build/html/_static/minus.png
-docs/build/html/_static/plus.png
+docs/build/html/_static/plus.png
+docs/images/hierarchy.jpg
```

### Comparing `MRdataset-0.1.3/setup.py` & `MRdataset-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     history = history_file.read()
 
 requirements = [
     'dicom2nifti>=2.4.2',
     'nibabel',
     'pydicom',
     'dictdiffer',
-    'pandas',
+    'pandas>=1.5.2',
     'pybids'
 ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Pradeep Raamana",
```

### Comparing `MRdataset-0.1.3/CONTRIBUTING.rst` & `MRdataset-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MRdataset-0.1.3/docs/conf.py` & `MRdataset-0.1.6/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.viewcode',
-              'sphinx.ext.napoleon']
+              'sphinx.ext.napoleon',
+              'sphinx.ext.mathjax']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
@@ -45,15 +46,15 @@
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'MRdataset'
-copyright = "2022, Harsh Sinha"
+copyright = "2023, Harsh Sinha"
 author = "Harsh Sinha"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
@@ -62,15 +63,15 @@
 release = MRdataset.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -164,9 +165,11 @@
      'MRdataset Documentation',
      author,
      'MRdataset',
      'One line description of project.',
      'Miscellaneous'),
 ]
 
+# -- Options for MathJAX support ---------------------------------------
+mathjax_path = "https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"
```

### Comparing `MRdataset-0.1.3/docs/make.bat` & `MRdataset-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MRdataset-0.1.3/docs/Makefile` & `MRdataset-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MRdataset-0.1.3/docs/mrQA1.png` & `MRdataset-0.1.6/docs/mrQA1.png`

 * *Files identical despite different names*

### Comparing `MRdataset-0.1.3/docs/installation.rst` & `MRdataset-0.1.6/docs/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 
 
 From sources
 ------------
 
 The sources for MRdataset can be downloaded from the `Github repo`_.
 
-You can either clone the public repository:
+You can clone the public repository:
 
 .. code-block:: console
 
     $ git clone git://github.com/Open-Minds-Lab/MRdataset
+..
+    Or download the `tarball`_:
 
-Or download the `tarball`_:
+    .. code-block:: console
 
-.. code-block:: console
-
-    $ curl -OJL https://github.com/Open-Minds-Lab/MRdataset/tarball/master
+        $ curl -OJL https://github.com/Open-Minds-Lab/MRdataset/tarball/master
 
 Once you have a copy of the source, you can install it with:
 
 .. code-block:: console
 
     $ python setup.py install
```

### Comparing `MRdataset-0.1.3/docs/MRdataset.rst` & `MRdataset-0.1.6/docs/API.rst`

 * *Files 11% similar despite different names*

```diff
@@ -8,36 +8,39 @@
 
 High level API
 ------------------------------
 The high level API of MRdataset shows how to interface with neuroimaging datasets
 using the elements in Core API. Here is a summarized reference of classes
 which can be used to import BIDS dataset and DICOM dataset.
 
-.. automodule:: MRdataset.bids_dataset
+.. automodule:: MRdataset.dicom
    :members:
    :undoc-members:
    :show-inheritance:
 
-.. automodule:: MRdataset.dicom_dataset
+
+.. automodule:: MRdataset.naive_bids
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+.. automodule:: MRdataset.fastbids
    :members:
    :undoc-members:
    :show-inheritance:
 
 
+
 Core API
 ---------------------
 The Core API contains modules for important elements (e.g. Modality,
 Subject, Run etc.in a neuroimaging experiment.
 
 .. automodule:: MRdataset.base
    :members:
    :undoc-members:
    :show-inheritance:
 
-
-Module contents
----------------
-
-.. automodule:: MRdataset
+.. automodule:: MRdataset.common
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `MRdataset-0.1.3/README.rst` & `MRdataset-0.1.6/docs/usage.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,70 @@
-===========
-Quickstart
-===========
-
-
-.. image:: https://img.shields.io/pypi/v/MRdataset.svg
-        :target: https://pypi.python.org/pypi/MRdataset
-
-MRdataset
-----------
-* a unified interface to various neuroimaging datasets such as DICOM, BIDS and any other generic format etc
-* Documentation: https://open-minds-lab.github.io/MRdataset/
-
-
 Command line usage
 ------------------
 
 MRdataset can be used on the command line interface. For a DICOM dataset::
 
-    mrds --data_root /path/to/dataset --style dicom
+    mrds --data-source /path/to/dataset --format dicom
 
 For a BIDS dataset::
 
-    mrds --data_root /path/to/dataset --style bids
+    mrds --data-source /path/to/dataset --format bids
 
 
-API/programmatic usage
+API usage
 ----------------------
+The following section provides a brief overview of the API. For more details,
+please refer to the Jupyter Notebook `tutorial`_.
 
 To use MRdataset in a project::
 
     import MRdataset
 
-The most important method is ``import_dataset``. It
-creates an appropriate object depending as per ``style`` argument.
+The most important method is ``import_dataset``. The dataset type
+such as ``dicom`` or ``bids`` can be specified using the ``ds_format`` argument.
 
 First of all, you have to import the relevant module::
 
     from MRdataset import import_dataset
 
 Given a valid folder path to a dataset of MR images (e.g. DICOM images),
-it creates a ``MRdataset.base.Project`` object.::
+it creates a dataset.::
 
-    data_root = '/home/user/datasets/ABCD'
-    dataset = import_dataset(data_root=data_root,
-                             style='dicom',
+    data_folder = '/home/user/datasets/ABCD'
+    dataset = import_dataset(data_source=data_folder,
+                             ds_format='dicom',
                              name='ABCD')
 
 By default, the ``import_dataset`` expects a DICOM dataset. However, this can
-be changed using ``style`` argument. For example, use ``style='bids'`` for
+be changed using ``ds_format`` argument. For example, use ``ds_format='bids'`` for
 importing a BIDS dataset.
 
 The library is highly extensible, and a developer can extend it to their own
 neuroimaging formats. For example, to create an interface with a new format, say
-NID (NeuroImaging Dataset), inherit ``MRdataset.base.Project`` in a file
+NID (NeuroImaging Dataset), inherit ``MRdataset.base.BaseDataset`` in a file
 ``NID_dataset.py``::
 
-    from MRdataset import Project
-    class NIDDataset(Project):
-        def __init__():
+    from MRdataset.base import BaseDataset
+    class NIDDataset(BaseDataset):
+        def __init__(data_source):
+            super().init(data_source)
             pass
 
          def walk():
             pass
 
+Finally, ``save_mr_dataset`` and ``load_mr_dataset`` can be used to save and load a
+dataset. For example, to save a dataset::
+
+    from MRdataset import save_mr_dataset
+    save_mr_dataset(dataset, '/home/user/datasets/xyz.mrds.pkl')
+
+
+Similarly, to load a dataset::
 
-Implement, these two functions. You can directly use ``style='nid'``. Thats it!
-No more changes required.
+    from MRdataset import load_mr_dataset
+    dataset = load_mr_dataset('/home/user/datasets/xyz.mrds.pkl')
 
+Note that the dataset is saved as a pickle file with an extension ``.mrds.pkl``.
 
+.. _tutorial: https://nbviewer.org/github/Open-Minds-Lab/MRdataset/blob/parallel/docs/usage.ipynb
```

### Comparing `MRdataset-0.1.3/MRdataset/bids_dataset.py` & `MRdataset-0.1.6/MRdataset/naive_bids.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,158 +1,192 @@
-import logging
-from pathlib import Path
-
+"""BIDS dataset class for MRdataset"""
 from bids import BIDSLayout
 
-from MRdataset.base import Project, Run, Modality, Subject, Session
-from MRdataset.config import datatypes
-from MRdataset.utils import select_parameters, get_ext
-
-# Module-level logger
-logger = logging.getLogger('root')
+from MRdataset.base import BaseDataset, Run, Modality, Subject, Session
+from MRdataset.config import VALID_DATATYPES
+from MRdataset.log import logger
+from MRdataset.bids_utils import select_parameters
 
 
 # TODO: check what if each variable is None. Apply try catch
-class BIDSDataset(Project):
+class BIDSDataset(BaseDataset):
     """
-
+    Container to manage the properties and methods of a BIDS dataset downloaded
+    from OpenNeuro. It is a subclass of BaseDataset. Expects the data_source to
+    contain JSON files for reading image acquisition parameters. Use
+    include_nifti_header to extract parameter from nifti headers.
     """
 
     def __init__(self,
-                 name='mind',
-                 data_root=None,
-                 metadata_root=None,
-                 include_phantom=False,
-                 reindex=False,
-                 include_nifti_header=False):
+                 name=None,
+                 data_source=None,
+                 is_complete=True,
+                 include_nifti_header=False,
+                 **_kwargs):
 
         """
         Parameters
         ----------
         name : str
             an identifier/name for the dataset
-        data_root : Path or str
+        data_source : Path or str or List
             directory containing dicom files, supports nested hierarchies
-        metadata_root : str or Path
-            directory to store cache
-        include_phantom : bool
-            whether to include localizer/aahead_scout/phantom/acr
-        reindex : bool
-            If true, rejects stored cache and rebuilds index
+        is_complete : bool
+            whether the dataset is complete
         include_nifti_header :
             whether to check nifti headers for compliance,
-            only used when --style==bids
+            only used when --ds_format==bids
         Examples
         --------
-        >>> from MRdataset.bids_dataset import BIDSDataset
+        >>> from MRdataset.naive_bids import BIDSDataset
         >>> dataset = BIDSDataset()
         """
 
-        super().__init__(name, data_root, metadata_root)
-
-        self.include_phantom = include_phantom
+        super().__init__(data_source)
+        self.is_complete = is_complete
         self.include_nifti_header = include_nifti_header
-        indexed = self.cache_path.exists()
-        if not indexed or reindex:
-            self.walk()
-            self.save_dataset()
-        else:
-            self.load_dataset()
+        self.name = name
 
-    def get_filters(self, subject=None, session=None, datatype=None):
+    def get_filters(self, subject: str = None,
+                    session: str = None, datatype: str = None):
+        """
+        Given subject id, session id, and datatype, the function would create
+        a dictionary to fetch the appropriate file from BIDS Layout. It just
+        creates the filter dictionary, doesn't fetch the files itself.
+
+        Parameters
+        ----------
+        subject : subject id
+        session : session id
+        datatype : one of datatypes like anat, func, dwi etc
+
+        Returns
+        -------
+        Dict to specify the filter parameters
+        """
         filters = {'extension': ['json']}
         if subject:
             filters['subject'] = subject
         if session:
             filters['session'] = session
         if datatype:
             filters['datatype'] = datatype
         if self.include_nifti_header:
             filters['extension'].append('nii.gz')
             filters['extension'].append('nii')
         return filters
 
     def walk(self):
-        """parses the file tree to populate them in a desirable hierarchy"""
-        print("Started building BIDSLayout .. ")
-        bids_layout = BIDSLayout(self.data_root, validate=False)
-        print("Completed BIDSLayout .. ")
+        """
+        Parses the file tree to populate them in a desirable hierarchy.
+        Extracts relevant parameters and stores it in project. Creates
+        a desirable hierarchy for a neuroimaging experiment
+        """
+        print('Started building BIDSLayout .. ')
+        if isinstance(self.data_source, list):
+            data_source = self.data_source[0]
+        else:
+            data_source = self.data_source
+
+        bids_layout = BIDSLayout(data_source, validate=False)
+        print('Completed BIDSLayout .. ')
 
         filters = self.get_filters()
         if not bids_layout.get(**filters):
-            raise EOFError('No JSON files found at --data_root {}'.format(
-                self.data_root))
+            raise EOFError(f'No JSON files found at --data_source'
+                           f' {data_source}')
 
-        for datatype in datatypes:
-            modality_obj = self.get_modality(datatype)
+        for datatype in VALID_DATATYPES:
+            modality_obj = self.get_modality_by_name(datatype)
             if modality_obj is None:
                 modality_obj = Modality(datatype)
 
             layout_subjects = bids_layout.get_subjects()
             if not layout_subjects:
-                raise EOFError("No Subjects found in dataset")
-            for nSub in layout_subjects:
-                subject_obj = modality_obj.get_subject(nSub)
+                raise ValueError('No Subjects found in dataset')
+            for n_sub in layout_subjects:
+                subject_obj = modality_obj.get_subject_by_name(n_sub)
                 if subject_obj is None:
-                    subject_obj = Subject(nSub)
+                    subject_obj = Subject(n_sub)
 
-                layout_sessions = bids_layout.get_sessions(subject=nSub)
+                layout_sessions = bids_layout.get_sessions(subject=n_sub)
 
                 if not layout_sessions:
-                    logger.info("No sessions found. '1' is default "
-                                "session name")
-                    session_node = subject_obj.get_session('1')
+                    logger.info('No sessions found. 1 is default '
+                                'session name')
+                    session_node = subject_obj.get_session_by_name('1')
                     if session_node is None:
                         session_node = Session('1')
 
-                    filters = self.get_filters(nSub, datatype)
+                    filters = self.get_filters(subject=n_sub, datatype=datatype)
                     # {'subject': nSub,
                     #        'datatype': datatype,
                     #        'extension': 'json'}
                     session_node = self.parse(session_node,
                                               filters,
                                               bids_layout)
                     if session_node.runs:
                         subject_obj.add_session(session_node)
                 else:
                     # If there are sessions
-                    for nSess in layout_sessions:
-                        session_node = subject_obj.get_session(nSess)
+                    for n_sess in layout_sessions:
+                        session_node = subject_obj.get_session_by_name(n_sess)
                         if session_node is None:
-                            session_node = Session(nSess)
-                            filters = self.get_filters(nSub, nSess, datatype)
+                            session_node = Session(n_sess)
+                            filters = self.get_filters(subject=n_sub,
+                                                       session=n_sess,
+                                                       datatype=datatype)
                             # {'subject': nSub,
                             # 'session': nSess,
                             # 'datatype': datatype,
                             # 'extension': 'json'}
                             session_node = self.parse(session_node,
                                                       filters,
                                                       bids_layout)
                         if session_node.runs:
                             subject_obj.add_session(session_node)
                 if subject_obj.sessions:
                     modality_obj.add_subject(subject_obj)
             if modality_obj.subjects:
                 self.add_modality(modality_obj)
         if not self.modalities:
-            raise EOFError("Expected Sidecar JSON files in --data_root. Got 0")
+            raise EOFError('Expected Sidecar JSON files in --data_source.'
+                           ' Got 0')
 
-    def parse(self, session_node, filters, bids_layout):
+    def parse(self, session_node: Session,
+              filters: dict, bids_layout: BIDSLayout) -> Session:
+        """
+        Extracts parameters for a run. Adds the new run node to session node,
+        returns modified session node.
+
+        Parameters
+        ----------
+        session_node : MRdataset.base.Session
+            session node to which the run node has to be added
+        filters : dict
+            dictionary defining arguments like subject, session, datatype to
+            extract corresponding files from a BIDS Layout object
+        bids_layout : bids.BIDSLayout
+            data structure which encapsulates the entire BIDS data structure
+
+        Returns
+        -------
+        session_node : MRdataset.base.Session
+            modified session_node which also contains the new run
+        """
         files = bids_layout.get(**filters)
+        parameters = {}
         for file in files:
             filename = file.filename
-            ext = get_ext(file)
-            if ext == '.json':
-                parameters = select_parameters(file.path, ext)
-            elif ext in ['.nii', '.nii.gz']:
-                parameters = select_parameters(file.path, ext)
-            else:
-                raise NotImplementedError(f"Got {ext}, Expects .nii/.json")
-            if parameters:
-                run_node = session_node.get_run(filename)
-                if run_node is None:
-                    run_node = Run(filename)
-                for k, v in parameters.items():
-                    run_node.params[k] = v
-                run_node.echo_time = round(parameters.get('EchoTime', 1.0), 4)
-                session_node.add_run(run_node)
+            parameters[filename] = {}
+            params_from_file = select_parameters(file)
+            parameters[filename].update(params_from_file)
+
+        for filename, params in parameters.items():
+            run_node = session_node.get_run_by_name(filename)
+            if run_node is None:
+                run_node = Run(filename)
+            for k, v in parameters.items():
+                run_node.params[k] = v
+            run_node.echo_time = parameters.get('EchoTime', 1.0)
+            session_node.add_run(run_node)
         return session_node
```

### Comparing `MRdataset-0.1.3/MRdataset/tests/test_MRdataset.py` & `MRdataset-0.1.6/MRdataset/tests/test_MRdataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """Tests for `MRdataset` package."""
 
 import shutil
 
 import hypothesis.strategies as st
 from MRdataset import import_dataset
 from MRdataset.simulate import make_compliant_test_dataset
+from MRdataset.common_dicom import get_csa_props
 from hypothesis import given, settings
 
 
 @settings(max_examples=50, deadline=None)
 @given(st.integers(min_value=0, max_value=10),
        st.floats(allow_nan=False,
                  allow_infinity=False),
@@ -38,7 +39,14 @@
                 for run in session.runs:
                     assert run.params['tr'] == repetition_time
                     assert run.params['echo_train_length'] == echo_train_length
                     assert run.params['flip_angle'] == flip_angle
     assert len(mrd_num_subjects) == num_subjects
     shutil.rmtree(fake_ds_dir)
     return
+
+
+def get_csa_props_test():
+    "CSA header looks funny in Pitt 7T (20221130)"
+    text = "blah = 0x1\nxy\nsAdjData.uiAdjShimMode                = 0x1\na = b"
+    shim_code = get_csa_props("sAdjData.uiAdjShimMode", text)
+    assert shim_code == '0x1'
```

### Comparing `MRdataset-0.1.3/MRdataset/config.py` & `MRdataset-0.1.6/MRdataset/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from functools import lru_cache
+from pathlib import Path
 
 # Constant Dicom Identifiers Used for dataset creation and manipulation
 TAGS = {
     "series_instance_uid": (0x20, 0x0e),
     "sequence": (0x18, 0x20),
     "variant": (0x18, 0x21),
     "patient_name": (0x10, 0x10),
@@ -17,53 +18,48 @@
     "echo_number": (0x18, 0x86),
     "te": [0x18, 0x81],
     "patient_sex": [0x10, 0x40],
     "patient_age": [0x10, 0x1010],
 }
 
 # Constant Paths
-CACHE_DIR = ".mrdataset"
+CACHE_DIR_NAME = ".mrdataset"
+CACHE_DIR = Path.home().resolve() / CACHE_DIR_NAME
+CACHE_DIR.mkdir(exist_ok=True)
+
+MRDS_EXT = '.mrds.pkl'
+VALID_DATASET_STYLES = [
+    'dicom',
+    'bids',
+    'fastbids',
+]
 
-# Constant Dicom Identifiers used for protocol compliance.
-# These are the parameters
-# which are compared in the final report
-# PARAMETER_TAGS = {
-#     "manufacturer": [0x08, 0x70],
-#     "organ": [0x18, 0x15],
-#     "te": [0x18, 0x81],
-#     "tr": [0x18, 0x80],
-#     "b0": [0x18, 0x87],
-#     "flip_angle": [0x18, 0x1314],
-#     "bwpx": [0x18, 0x95],
-#     "echo_train_length": [0x18, 0x0091],
-#     "scanning_sequence": [0x18, 0x20],
-#     "sequence_variant": [0x18, 0x21],
-#     "mr_acquisition_type": [0x18, 0x23],
-#     "phase_encoding_lines": [0x18, 0x89],
-#     "bwp_phase_encode": [0x19, 0x1028],
-#     "phase_encoding_direction": [0x18, 0x1312],
-# }
+VALID_BIDS_EXTENSIONS = ['.json', '.nii', '.nii.gz']
 
 PARAMETER_NAMES = {
     # 'Manufacturer': [0x08, 0x70],
+    'EchoNumbers': [0x18, 0x86],
     'BodyPartExamined': [0x18, 0x15],
     'EchoTime': [0x18, 0x81],
     'RepetitionTime': [0x18, 0x80],
     'MagneticFieldStrength': [0x18, 0x87],
     'FlipAngle': [0x18, 0x1314],
     'PhaseEncodingDirection': [0x18, 0x1312],
     'EchoTrainLength': [0x18, 0x0091],
     'PixelBandwidth': [0x18, 0x95],
     'ScanningSequence': [0x18, 0x20],
     'SequenceVariant': [0x18, 0x21],
     'MRAcquisitionType': [0x18, 0x23],
-    'PhaseEncodingSteps': [0x18, 0x89]
+    'PhaseEncodingSteps': [0x18, 0x89],
+    # 'Model': [0x08, 0x1090],
+    # 'SoftwareVersions': [0x18, 0x1020],
+    # 'InstitutionName': [0x08, 0x0080],
 }
 
-datatypes = [
+VALID_DATATYPES = [
     'anat',
     'beh',
     'dwi',
     'eeg',
     'fmap',
     'func',
     'ieeg',
@@ -99,15 +95,15 @@
     "SP": "spoiled",
     "MP": "MAG prepared",
     "OSP": "oversampling phase",
     "NONE": "no sequence variant"
 }
 
 PAT = {
-    "1": 'None',
+    "1": 'Not Selected',
     "2": 'Grappa',
     "3": 'Sense'
 }
 
 SHIM = {
     "1": 'tune_up',
     "2": 'standard',
@@ -119,37 +115,14 @@
 
 # Suppress duplicated warnings
 @lru_cache(1)
 def warn_once(logger: logging.Logger, msg: str):
     logger.warning(msg)
 
 
-def setup_logger(name, filename):
-    format_string = '%(asctime)s - %(levelname)s - %(message)s'
-    formatter = logging.Formatter(fmt=format_string)
-    handler = logging.StreamHandler()
-    dup_filter = DuplicateFilter()
-    logger = logging.getLogger(name)
-    logger.setLevel(logging.DEBUG)
-    handler.addFilter(dup_filter)
-    handler.setFormatter(formatter)
-    logger.addHandler(handler)
-    return logger
-
-
-class DuplicateFilter(object):
-    def __init__(self):
-        self.msgs = set()
-
-    def filter(self, record):
-        rv = record.msg not in self.msgs
-        self.msgs.add(record.msg)
-        return rv
-
-
 class MRException(Exception):
     """
     Custom error that is raised when some critical properties are not found
     in dicom file
     """
 
     def __init__(self, message, **kwargs):
@@ -172,14 +145,20 @@
 #     pass
 #
 #
 # class NonCompliantSubject(ComplianceException):
 #     """"""
 #     pass
 
+class DatasetEmptyException(MRException):
+    def __init__(self):
+        super().__init__('Expected Sidecar DICOM/JSON files in '
+                         '--data_source. Got 0 DICOM/JSON files.')
+
+
 class ChangingParamsInSeries(MRException):
     """Custom error that is raised when parameter values are different for
     different slices even though the SeriesInstanceUID is same."""
 
     def __init__(self, filepath):
         super().__init__("Expected all dicom slices to have same parameters. "
                          "Got changing parameters : {}".format(filepath))
```

### Comparing `MRdataset-0.1.3/MRdataset/dicom_dataset.py` & `MRdataset-0.1.6/MRdataset/dicom.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,149 +1,157 @@
-import logging
 from pathlib import Path
 
-import dicom2nifti
 import pydicom
 
-from MRdataset import common_dicom
 from MRdataset import config
-from MRdataset.base import Project, Run, Modality, Subject, Session
-from MRdataset.utils import param_difference, files_under_folder
-import warnings
+from MRdataset.base import BaseDataset, Run, Modality, Subject, Session
+from MRdataset.dicom_utils import is_dicom_file, is_valid_inclusion, \
+    get_dicom_modality_tag, is_same_set, parse_imaging_params, \
+    combine_varying_params
+from MRdataset.log import logger
+from MRdataset.utils import param_difference, files_in_path
+from MRdataset.config import DatasetEmptyException
 
 # Module-level logger
-logger = logging.getLogger('root')
+# logger = logging.getLogger('root')
 
 
 # TODO: check what if each variable is None. Apply try catch
-class DicomDataset(Project):
+class DicomDataset(BaseDataset):
     """
     Container to manage properties and issues of a dataset downloaded from
-    XNAT. Expects the data_root to be collection of dicom files, which may
+    XNAT. Expects the data_source to be collection of dicom files, which may
     belong to different subjects, modalities, sessions or runs.
 
     Attributes
     ----------
     name : str
         Identifier/name for the node
-    data_root : str or Path
-        directory containing dataset with dicom files
-    metadata_root : str or Path
-        directory to store cache
+    data_source : Path or str or Iterable
+        directories containing dicom files, supports nested hierarchies
     include_phantom
         Whether to include non-subject scans like localizer, acr/phantom,
         head_scout
     """
 
     def __init__(self,
-                 name='mind',
-                 data_root=None,
-                 metadata_root=None,
+                 data_source=None,
                  include_phantom=False,
-                 reindex=False,
-                 **kwargs):
+                 is_complete=True,
+                 name=None,
+                 **_kwargs):
 
         """
         Parameters
         ----------
         name : str
             an identifier/name for the dataset
-        data_root : Path or str
+        data_source : Path or str or Iterable
             directory containing dicom files, supports nested hierarchies
-        metadata_root : str or Path
-            directory to store cache
         include_phantom : bool
             whether to include localizer/aahead_scout/phantom/acr
-        reindex : bool
-            If true, rejects stored cache and rebuilds index
+        is_complete : bool
+            whether the dataset is complete or partial (default: True)
+
 
         Examples
         --------
-        >>> from MRdataset import dicom_dataset
-        >>> dataset = dicom_dataset.DicomDataset()
+        >>> from MRdataset import dicom
+        >>> dataset = dicom.DicomDataset()
         """
-        super().__init__(name, data_root, metadata_root)
-
+        super().__init__(data_source)
+        self.is_complete = is_complete
         self.include_phantom = include_phantom
-        indexed = self.cache_path.exists()
-        if not indexed or reindex:
-            self.walk()
-            self.save_dataset()
-        else:
-            self.load_dataset()
+        self.name = name
 
     def walk(self):
-        """generates filenames in the directory tree, verifies if it is dicom
+        """
+        Retrieves filenames in the directory tree, verifies if it is dicom
         file, extracts relevant parameters and stores it in project. Creates
-        a desirable hierarchy for a neuroimaging experiment"""
+        a desirable hierarchy for a neuroimaging experiment
+        """
         no_files_found = True
         study_ids_found = set()
 
-        for filepath in files_under_folder(self.data_root):
+        for filepath in files_in_path(self.data_source):
             no_files_found = False
             try:
-                if not dicom2nifti.common.is_dicom_file(filepath):
-                    # logger.warning(
-                    #     "DICOM not found in {}".format(filepath.parent))
+                if not is_dicom_file(filepath):
+                    logger.debug(
+                        "Not a DICOM file : {}".format(filepath))
                     continue
+                # TODO: Read dicom file : 2
                 dicom = pydicom.read_file(filepath, stop_before_pixels=True)
-                if common_dicom.is_valid_inclusion(filepath,
-                                                   dicom,
-                                                   self.include_phantom):
-
-                    # info = common.parse_study_information(dicom)
-                    modality_name = common_dicom.get_dicom_modality_tag(dicom)
-                    modality_obj = self.get_modality(modality_name)
+                if is_valid_inclusion(filepath,
+                                      dicom,
+                                      self.include_phantom):
+
+                    modality_name = get_dicom_modality_tag(dicom)
+                    modality_obj = self.get_modality_by_name(modality_name)
                     if modality_obj is None:
                         modality_obj = Modality(modality_name)
 
                     patient_id = str(dicom.get('PatientID', None))
-                    subject_obj = modality_obj.get_subject(patient_id)
+                    subject_obj = modality_obj.get_subject_by_name(patient_id)
                     if subject_obj is None:
                         subject_obj = Subject(patient_id)
 
                     series_num = str(dicom.get('SeriesNumber', None))
-                    session_node = subject_obj.get_session(series_num)
+                    session_node = subject_obj.get_session_by_name(series_num)
                     if session_node is None:
-                        session_node = Session(series_num,
-                                               Path(filepath).parent)
+                        session_node = Session(series_num)
+
+                    run_name = is_same_set(dicom)
+                    run_node = session_node.get_run_by_name(run_name)
+                    # Cast as int as sometime it may return a MultiValue type
+                    # TODO: check Rembrandt dataset
+                    try:
+                        echo_numbers = int(dicom.get('EchoNumbers', None))
+                    except TypeError as e:
+                        echo_numbers = 1
+                        logger.warning(f'Got {e}')
 
-                    # series_uid = dicom.get('SeriesInstanceUID', None)
-                    # echo_num = dicom.get('EchoNumbers', None)
-                    # if echo_num:
-                    #     run_name = series_uid + '_e' + str(dicom.EchoNumbers)
-                    # else:
-                    #     run_name = series_uid
-                    run_name = common_dicom.isSameSet(dicom)
-                    run_node = session_node.get_run(run_name)
                     if run_node is None:
                         run_node = Run(run_name)
-                        run_node.echo_time = dicom.get('EchoTime', 1.0)
-
-                    dcm_img_params = common_dicom.parse_imaging_params(filepath)
-                    param_diff = param_difference(dcm_img_params, run_node.params)
+                        # Create bins for each echo time. If echo numbers
+                        # is 1, then it is a single echo time, so we put all
+                        # runs to default bin with echo time 1.0. This will not
+                        # affect the echo times on the report. And, if echo
+                        # numbers is greater than 1, then we create bins for
+                        # each differing echo time. Even though the variable
+                        # name is inconsistent, it is not a bug. Trying to make
+                        # as minimal changes as possible.
+                        # TODO: use array type instead of single value for echo
+                        #  time
+                        if echo_numbers > 1:
+                            run_node.echo_time = dicom.get('EchoTime', 1.0)
+                        else:
+                            run_node.echo_time = 1.0
+                    # TODO: dcm_img_params doesnt make sense
+                    dcm_img_params = parse_imaging_params(filepath)
+                    param_diff = param_difference(dcm_img_params,
+                                                  run_node.params)
                     if len(run_node.params) == 0:
                         run_node.params = dcm_img_params.copy()
                     elif param_diff:
-                        param_name = param_diff[0][1]
-                        expect = run_node.params[param_name]
-                        got = dcm_img_params[param_name]
-                        warnings.warn(f"Slices with varying {param_name}"
-                                      f" in {filepath}."
-                                      f" Expected {expect}, Got {got}")
-
+                        run_node.params = combine_varying_params(
+                                            param_diff,
+                                            run_node.params,
+                                            filepath)
                     session_node.add_run(run_node)
                     subject_obj.add_session(session_node)
                     modality_obj.add_subject(subject_obj)
                     self.add_modality(modality_obj)
 
                     # Collect all unique study ids found in DICOM
                     study_ids_found.add(str(dicom.StudyID))
 
             except config.MRException as mrd_exc:
                 logger.exception(mrd_exc)
+            except PermissionError as e:
+                logger.error(e)
             except Exception as exc:
                 raise exc
         if no_files_found:
-            raise EOFError("Read 0 files at {}".format(self.data_root))
+            raise DatasetEmptyException()
         if len(study_ids_found) > 1:
             logger.warning(config.MultipleProjectsInDataset(study_ids_found))
```

### Comparing `MRdataset-0.1.3/MRdataset/cli.py` & `MRdataset-0.1.6/MRdataset/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 """Console script for MRdataset."""
 import argparse
 import sys
 from pathlib import Path
 
 from MRdataset import import_dataset
+from MRdataset.log import logger
 
 
 def main():
     """Console script for MRdataset."""
     parser = argparse.ArgumentParser(
         description='MRdataset : generates dataset for analysis',
         add_help=False)
     required = parser.add_argument_group('required arguments')
     optional = parser.add_argument_group('optional arguments')
 
-    required.add_argument('-d', '--data_root', type=str, required=True,
+    required.add_argument('-d', '--data-source', type=str, required=True,
                           help='directory containing downloaded dataset with '
                                'dicom files, supports nested hierarchies')
-    optional.add_argument('-s', '--style', type=str, default='dicom',
-                          help='choose type of dataset, one of [dicom|other]')
+    optional.add_argument('-f', '--format', type=str, default='dicom',
+                          help='choose type of dataset, expected'
+                               'one of [dicom|bids|pybids]')
     optional.add_argument('-n', '--name', type=str,
                           help='provide a identifier/name for dataset')
     optional.add_argument('-h', '--help', action='help',
                           default=argparse.SUPPRESS,
                           help='show this help message and exit')
-    optional.add_argument('-r', '--reindex', action='store_true',
-                          help='overwrite existing metadata files')
+    optional.add_argument('--is-partial', action='store_true',
+                          help='flag dataset as a partial dataset')
     optional.add_argument('-v', '--verbose', action='store_true',
                           help='allow verbose output on console')
-    optional.add_argument('--include_phantom', action='store_true',
+    optional.add_argument('--include-phantom', action='store_true',
                           help='whether to include phantom, localizer, '
                                'aahead_scout')
-    optional.add_argument('--metadata_root', type=str, required=False,
-                          help='directory to store cache')
-    optional.add_argument('--include_nifti_header', action='store_true',
+    optional.add_argument('--include-nifti-header', action='store_true',
                           help='whether to check nifti headers for compliance,'
-                               'only used when --style==bids')
+                               'only used when --format==bids')
     args = parser.parse_args()
-    if not Path(args.data_root).is_dir():
-        raise OSError('Expected valid directory for --data_root argument, '
-                      'Got {}'.format(args.data_root))
+    if not Path(args.data_source).is_dir():
+        raise OSError('Expected valid directory for --data_source argument, '
+                      f'Got {args.data_source}')
     if args.include_nifti_header:
-        if args.style != 'bids':
-            raise SyntaxError('--include_nifti_header for style=bids')
+        if args.format != 'bids':
+            raise SyntaxError('--include-nifti-header for format=bids')
+    if args.verbose:
+        logger.setLevel('INFO')
+    else:
+        logger.setLevel('WARNING')
 
-    dataset = import_dataset(data_root=args.data_root,
-                             style=args.style,
+    dataset = import_dataset(data_source=args.data_source,
+                             ds_format=args.format,
                              name=args.name,
-                             reindex=args.reindex,
                              include_phantom=args.include_phantom,
                              verbose=args.verbose,
-                             metadata_root=args.metadata_root,
-                             include_nifti_header=args.include_nifti_header)
+                             include_nifti_header=args.include_nifti_header,
+                             is_complete=not args.is_partial)
     return dataset
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     sys.exit(main())  # pragma: no cover
```

### Comparing `MRdataset-0.1.3/MRdataset/simulate.py` & `MRdataset-0.1.6/MRdataset/simulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     src_dir, dest_dir = setup_directories(compl_data_bids)  # noqa
     copyeverything(src_dir, dest_dir)
     dataset_info = defaultdict(set)
 
     layout = BIDSLayout(dest_dir.as_posix())
     subjects = layout.get_subjects()
 
-    for i, modality in enumerate(MRdataset.config.datatypes):
+    for i, modality in enumerate(MRdataset.config.VALID_DATATYPES):
         count = num_noncompliant_subjects[i]
         non_compliant_subjects = set()
         for sub in subjects:
             if count < 1:
                 break
             filters = {'subject': sub,
                        'datatype': modality,
```

### Comparing `MRdataset-0.1.3/MRdataset/common_dicom.py` & `MRdataset-0.1.6/MRdataset/dicom_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,109 @@
-import logging
+""" Utility functions for dicom files """
+import re
 import warnings
 from collections import defaultdict
+from collections.abc import Iterable
 from pathlib import Path
-from typing import Union
+from typing import Union, Optional
 
 import dicom2nifti
 import pydicom
 from MRdataset import config
 from MRdataset import utils
-from collections.abc import Iterable
+from MRdataset.log import logger
+from MRdataset.utils import slugify
 
 with warnings.catch_warnings():
-    warnings.filterwarnings("ignore")
+    warnings.filterwarnings('ignore')
     from nibabel.nicom import csareader
 
 
-logger = logging.getLogger('root')
+# logger = logging.getLogger('root')
+
 
+def is_dicom_file(filename: str):
+    """
+    The first 4 bytes are read from the file. For a valid DICOM file,
+    the bytes should be DICM. Otherwise, it is not a valid DICOM file.
+    Parameters
+    ----------
+    filename : str
+        path to the file
 
-def isSameSet(dicom):
+    Returns
+    -------
+    bool : if the file is a DICOM file
+    """
+    # TODO: Read dicom file : 1
+    with open(filename, 'rb') as file_stream:
+        file_stream.seek(128)
+        data = file_stream.read(4)
+
+    if data == b'DICM':
+        return True
+
+
+def is_same_set(dicom: pydicom.FileDataset) -> str:
+    """
+    Provides a unique id for Series, to which the input dicom file
+    belongs to.
+
+    Parameters
+    ----------
+    dicom : pydicom.FileDataset
+        dicom object returned by pydicom.dcmread or pydicom.read_file
+
+    Returns
+    -------
+    Series identifier to which this DICOM should be added to
+    """
     series_uid = dicom.get('SeriesInstanceUID', None)
-    # echo_num = dicom.get('EchoNumbers', None)
-    echo_time = dicom.get('EchoTime', None)
-    # if echo_num:
-    #     run_name = series_uid + '_e' + str(dicom.EchoNumbers)
-    if echo_time:
-        run_name = series_uid + '_e' + str(dicom.EchoTime)
+    # Convert pydicom.valuerep.MultiValue to int
+    try:
+        echo_num = int(dicom.get('EchoNumbers', None))
+    except TypeError as e:
+        echo_num = 1
+        logger.warning(f'Got {e}')
+    # Need to convert pydicom.valuerep.DSfloat to float
+    # echo_time = float(dicom.get('EchoTime', None))
+    if echo_num > 1:
+        run_name = series_uid + '_en_' + str(echo_num)
     else:
         run_name = series_uid
+    #     run_name = series_uid
+    # else:
+    # else:
+    # run_name = series_uid
     return run_name
 
 
-
-
-def is_valid_inclusion(filename: str,
+def is_valid_inclusion(filepath: str,
                        dicom: pydicom.FileDataset,
                        include_phantom=False) -> bool:
     """
     Function will do some basic checks to see if it is a valid imaging dicom
 
     Parameters
     ----------
-    filename : str or Path
+    filepath : str or Path
         filename for raising the warning
     dicom : pydicom.FileDataset
         dicom object returned by pydicom.dcmread or pydicom.read_file
     include_phantom : bool
         whether to include AAhead_coil/localizer/ACR/Phantom
 
     Returns
     -------
     bool
     """
-    filename = Path(filename).resolve()
+    filepath = Path(filepath).resolve()
 
     if not dicom2nifti.convert_dir._is_valid_imaging_dicom(dicom):
-        logger.info("Invalid file: %s" % filename.parent)
+        logger.info('Invalid file: %s', filepath.parent)
         return False
 
     # if not header_exists(dicom):
     #     logger.error("Header Absent: %s" % filename)
     #     return False
 
     # TODO: revisit whether to include localizer or not,
@@ -69,26 +113,26 @@
     # check quality control subject :  Not present dicom headers
     try:
         series_desc = dicom.get('SeriesDescription', None)
         if series_desc is not None:
             series_desc = series_desc.lower()
             if not include_phantom:
                 if 'local' in series_desc:
-                    logger.info("Localizer: Skipping %s" % filename.parent)
+                    logger.info('Localizer: Skipping %s', filepath.parent)
                     return False
 
                 if 'aahead' in series_desc:
-                    logger.info("AAhead_Scout: Skipping %s" % filename.parent)
-                    return True
+                    logger.info('AAhead_Scout: Skipping %s', filepath.parent)
+                    return False
 
                 if is_phantom(dicom):
-                    logger.info('ACR/Phantom: %s' % filename.parent)
+                    logger.info('ACR/Phantom: %s', filepath.parent)
                     return False
     except AttributeError as e:
-        logger.warning("Series Description not found in %s" % filename)
+        logger.warning('%s :Series Description not found in %s' % (e, filepath))
 
     return True
 
 
 def is_phantom(dicom: pydicom.FileDataset) -> bool:
     """
     Implements a heuristic to detect a phantom. Checks patient's name,
@@ -135,19 +179,20 @@
 
     if property1 is None:
         property1 = dicom.get('SequenceName', None)
     if property1 is None:
         property1 = dicom.get('ProtocolName', None)
     if property1 is None:
         return 'MR_image'
-    ret_value = str(property1.replace(" ", "_"))
+    ret_value = slugify(property1)
     if ret_value:
         return ret_value
     return 'MR_image'
 
+
 # TODO : rename csa
 def header_exists(dicom: pydicom.FileDataset) -> bool:
     """
     Check if the private SIEMENS header exists in the file or not. Some
     parameters like effective_echo_spacing and shim method need the dicom
     header to be present.
 
@@ -169,84 +214,89 @@
         # don't need these values now
         # image_header = \
         csareader.read(image)
         # items = \
         series_header['tags']['MrPhoenixProtocol']['items'][0].split('\n')
         return True
     except Exception as e:
-        # logger.exception("{}. Expects dicom files from Siemens. "
-        #                  "Use --skip_private_header to create report".format(e))
+        logger.info(f'Expects dicom files from Siemens to be able to'
+                    f' read the private header. For other vendors',
+                    f'private header is skipped. '
+                    f'{e} in {dicom.filename}')
+        # "Use --skip_private_header to create report".format(e))
         # raise e
         return False
 
 
 def parse_imaging_params(dicom_path: Union[str, Path]) -> dict:
     """
     Given a filepath to a .dcm file, the function reader DICOM metadata
     and extracts relevant parameter values for checking compliance.
     The parameters are selected if it is present in config.PARAMETER_NAMES
+
     Parameters
     ----------
     dicom_path: str or Path
         filepath for .dcm file
+
     Returns
     -------
     dict
         contains key, value pairs for relevant parameters
+
+    Raises
+    ------
+
     """
     filepath = Path(dicom_path)
     params = defaultdict()
 
     if not filepath.exists():
-        raise OSError("Expected a valid filepath, Got invalid path : {0}\n"
-                      "Consider re-indexing dataset.".format(filepath))
+        raise OSError(f'Expected a valid filepath,Got invalid path : {filepath}'
+                      f'\n. Consider re-indexing dataset.')
 
     try:
+        # TODO: Read dicom file : 3
         dicom = pydicom.dcmread(filepath,
                                 stop_before_pixels=True)
-    except OSError:
+    except OSError as exc:
         raise FileNotFoundError(
-            "Unable to read dicom file from disk : {0}".format(filepath)
-        )
+            f'Unable to read dicom file from disk : {filepath}'
+        ) from exc
 
     for k in config.PARAMETER_NAMES.keys():
-        # try:
         value = get_param_value_by_name(dicom, k)
         # the value should be hashable
         # a dictionary will be used later to count the majority value
         if not isinstance(value, str):
             if isinstance(value, Iterable):
-                value = '_'.join(value)
+                value = '_'.join([str(i) for i in sorted(value)])
             elif not utils.is_hashable(value):
                 value = str(value)
         params[k] = value
-        # except:
-        #     warnings.warn('Unable to parse parameter {} from \n\t{}'
-        #                   ''.format(k, dicom_path))
     is3d = params['MRAcquisitionType'] == '3D'
-    params["is3d"] = is3d
-    params["effective_echo_spacing"] = effective_echo_spacing(dicom)
+    params['is3d'] = is3d
+    params['effective_echo_spacing'] = effective_echo_spacing(dicom)
     if header_exists(dicom):
         csa_values = csa_parser(dicom)
         params['multi_slice_mode'] = csa_values.get('slice_mode', None)
         params['ipat'] = csa_values.get('ipat', None)
         params['shim'] = csa_values.get('shim', None)
-        params["phase_encoding_direction"] = get_phase_encoding(
-                                dicom,
-                                is3d=params['is3d'],
-                                echo_train_length=params['EchoTrainLength'])
+        params['phase_polarity'] = get_phase_polarity(dicom)
+        # params['phase_encoding_direction'] = get_phase_encoding(dicom)
     else:
         params['multi_slice_mode'] = None
         params['ipat'] = None
         params['shim'] = None
-        params['phase_encoding_direction'] = None
+        params['phase_polarity'] = None
+        # params['phase_encoding_direction'] = None
     return params
 
 
-def get_param_value_by_name(dicom, name):
+def get_param_value_by_name(dicom: pydicom.FileDataset, name: str):
     """
     Extracts value from dicom metadata looking up the corresponding HEX tag
     in config.PARAMETER_NAMES
 
     Parameters
     ----------
     dicom : pydicom.FileDataset
@@ -263,15 +313,15 @@
     # TODO: consider name.lower()
     data = dicom.get(config.PARAMETER_NAMES[name], None)
     if data:
         return data.value
     return None
 
 
-def get_header(dicom, name):
+def get_header(dicom: pydicom.FileDataset, name: str):
     """
     Extracts value from dicom headers looking up the corresponding HEX tag
     in config.HEADER_TAGS
 
     Parameters
     ----------
     dicom : pydicom.FileDataset
@@ -287,133 +337,222 @@
     """
     data = dicom.get(config.HEADER_TAGS[name], None)
     if data:
         return data.value
     return None
 
 
-# def get_tags_by_name(dicom, name):
-#     """
-#     Extracts value from dicom metadata looking up the corresponding HEX tag
-#     in config.PARAMETER_NAMES
-#
-#     Parameters
-#     ----------
-#     dicom : pydicom.FileDataset
-#         dicom object read from pydicom.read_file
-#
-#     name : str
-#         parameter name such as MagneticFieldStrength or Manufacturer
-#
-#     Returns
-#     -------
-#     This method return a value for the given key. If key is not available,
-#     then returns default value None.
-#     """
-#     data = dicom.get(config.TAGS[name], None)
-#     if data is None:
-#         return None
-#     return data.value
-
-
-def csa_parser(dicom):
+def csa_parser(dicom: pydicom.FileDataset) -> dict:
     """
     Handles the private CSA header from Siemens formatted raw scanner.
 
     Parameters
     ----------
     dicom : pydicom.FileDataset
         dicom object read from pydicom.read_file
 
     Returns
     -------
     dict
         Contains multi-slice mode, iPAT and shim_mode
 
+    Raises
+    ------
+    AttributeError
+        If CSA header exists but xProtocol string is missing
+
     """
     series_header = csareader.read(get_header(dicom, 'series_header_info'))
     items = utils.safe_get(series_header, 'tags.MrPhoenixProtocol.items')
     if items:
-        text = items[0].split("\n")
+        text = items[0]
     else:
         raise AttributeError('CSA Header exists, but xProtocol is missing')
 
-    start = False
-    end = False
-    props = {}
-    for e in text:
-        if e[:15] == '### ASCCONV END':
-            end = True
-        if start and not end:
-            ele = e.split()
-            if ele[1].strip() == "=":
-                props[ele[0]] = ele[2]
-        if e[:17] == '### ASCCONV BEGIN':
-            start = True
-
-    slice_code = props.get("sKSpace.ucMultiSliceMode", None)
-    slice_mode = config.SLICE_MODE.get(slice_code, None)
-
-    ipat_code = props.get("sPat.ucPATMode", None)
-    ipat = config.PAT.get(ipat_code, None)
-
-    shim_code = props.get("sAdjData.uiAdjShimMode", None)
-    shim = config.SHIM.get(shim_code, None)
+    slice_code = get_csa_props('sKSpace.ucMultiSliceMode', text)
+    slice_mode = config.SLICE_MODE.get(slice_code, slice_code)
+    ipat_code = get_csa_props('sPat.ucPATMode', text)
+    ipat = config.PAT.get(ipat_code, ipat_code)
+    shim_code = get_csa_props('sAdjData.uiAdjShimMode', text)
+    shim = config.SHIM.get(shim_code, shim_code)
 
     return {
         'slice_mode': slice_mode,
         'ipat': ipat,
         'shim': shim
     }
 
 
-def effective_echo_spacing(dicom):
-    # if self.get("echo_train_length") > 1: # Check if etl == pel
-    # check =
-    # (self.get("echo_train_length") == self.get("phase_encoding_lines"))
-    # if not check:
-    # print("PhaseEncodingLines is not equal to EchoTrainLength
-    # : {0}".format(self.filepath))
+def get_csa_props(parameter, corpus):
+    """Extract parameter code from CSA header text
+
+    we want 0x1 from e.g.
+    sAdjData.uiAdjShimMode                = 0x1
+    """
+    index = corpus.find(parameter)
+    if index == -1:
+        return -1
+
+    shift = len(parameter) + 6
+    if index + shift > len(corpus):
+        print(f"#WARNING: {parameter} in CSA too short: '{corpus[index:]}'")
+        return -1
+
+    # 6 chars after parameter text, 3rd value
+    param_val = corpus[index:index + shift]
+    code_parts = re.split('[\t\n]', param_val)
+    if len(code_parts) >= 3:
+        return code_parts[2]
+
+    # if not above, might look like:
+    # sAdjData.uiAdjShimMode                = 0x1
+
+    # this runs multiple times on every dicom
+    # regexp is expensive? don't use unless we need to
+    match = re.search(r'=\s*([^\n]+)', corpus[index:])
+    if match:
+        match = match.groups()[0]
+        # above is also a string. don't worry about conversion?
+        # match = int(match, 0)  # 0x1 -> 1
+        return match
+
+    # couldn't figure out
+    return -1
+
+
+def effective_echo_spacing(dicom: pydicom.FileDataset) -> Optional[float]:
+    """
+    Calculates effective echo spacing in sec.
+    * For Siemens
+    Effective Echo Spacing (s) =
+    (BandwidthPerPixelPhaseEncode * MatrixSizePhase)^-1
+
+    * For Philips
+    echo spacing (msec) =
+     1000*water-fat shift (per pixel)/(water-fat shift(in Hz)*echo_train_length)
+
+    Parameters
+    ----------
+    dicom : pydicom.FileDataset
+        dicom object returned by pydicom.dcmread or pydicom.read_file
 
+    Returns
+    -------
+    float value for effective echo spacing
+    """
     bwp_phase_encode = get_param_value_by_name(dicom, 'PixelBandwidth')
     phase_encoding = get_param_value_by_name(dicom, 'PhaseEncodingSteps')
 
     if (bwp_phase_encode is None) or (phase_encoding is None):
         return None
-    else:
-        try:
-            value = 1000 / (bwp_phase_encode * phase_encoding)
-        except ZeroDivisionError as exc:
-            logger.exception(exc)
-            return None
+    denominator = bwp_phase_encode * phase_encoding
+    if denominator:
+        value = 1000 / denominator
         # Match value to output of dcm2niix
         return value / 1000
+    else:
+        return None
 
 
-def get_phase_encoding(dicom, is3d, echo_train_length):
+def get_phase_polarity(dicom: pydicom.FileDataset) -> Optional[int]:
+    """
+    Get phase polarity from dicom header
+
+    Parameters
+    ----------
+    dicom : pydicom.FileDataset
+        dicom object returned by pydicom.dcmread or pydicom.read_file
+
+    Returns
+    -------
+    int value for phase polarity
+    """
+    image_header = csareader.read(get_header(dicom, 'image_header_info'))
+    phase_value = utils.safe_get(image_header,
+                                 'tags.PhaseEncodingDirectionPositive.items')
+    if phase_value:
+        return phase_value[0]
+    return None
+
+
+def get_phase_encoding(dicom: pydicom.FileDataset) -> Optional[str]:
     """
     https://github.com/rordenlab/dcm2niix/blob/23d087566a22edd4f50e4afe829143cb8f6e6720/console/nii_dicom_batch.cpp
-    https://neurostars.org/t/determining-bids-phaseencodingdirection-from-dicom/612/6 # noqa
-    Following code only for SEIMENS, Look into above links for GE, Philips etc.
+    https://github.com/rordenlab/dcm2niix/issues/652#issuecomment-1323623521
+    https://www.rad.pitt.edu/extract-phase-encoding.html
+                            Polarity
+                    |  1        |   0       |
+    InPlanePED  ROW |  R >> L   |   L >> R  |
+                COL |  A >> P   |   P >> A  |
+
+                            Polarity
+                    |   1   |   0   |
+    InPlanePED  ROW |   i   |   i-  |
+                COL |   j   |   j-  |
+
+    Following code only for Siemens, Look into above links for GE, Philips etc.
+
+    Parameters
+    ----------
+    dicom : pydicom.FileDataset
+        dicom object returned by pydicom.dcmread or pydicom.read_file
+
+    Returns
+    -------
+    string formatted phase encoding direction
     """
     # is_skip = False
     # if is3d:
     #     is_skip = True
     # if echo_train_length > 1:
     #     is_skip = False
     image_header = csareader.read(get_header(dicom, 'image_header_info'))
     phase_value = utils.safe_get(image_header,
                                  'tags.PhaseEncodingDirectionPositive.items')
     if phase_value:
         phase = phase_value[0]
-        ped_value = get_param_value_by_name(dicom, "PhaseEncodingDirection")
+        ped_value = get_param_value_by_name(dicom, 'PhaseEncodingDirection')
         if ped_value in ['ROW', 'COL']:
             ped = ped_value
         else:
             return None
 
-        niftidim = {'COL': 'i', 'ROW': 'j'}
+        nifti_dim = {'COL': 'j', 'ROW': 'i'}
         ped_to_sign = {0: '-', 1: ''}
-        ij = niftidim[ped]
+        ij = nifti_dim[ped]
         sign = ped_to_sign[phase]
-        return '{}{}'.format(ij, sign)
+        return f'{ij}{sign}'
     return None
+
+
+def combine_varying_params(parameter_diff_list, params, filepath):
+    #   If a different slice is read first, it would lead
+    #   to differences in parameters for the run. How to
+    #   reconcile ? For ex. in one case, there was a single
+    #   dcm file with PED, others didn't have this key.
+    #   Depending upon which file is read first, the
+    #   parameters are added to run, which is a serious issue.
+    #   TODO : Can we maintain a list of values, this would make things simple
+    #       especially for multi-echo time modalities. Right now, it has a
+    #       single value for each parameter.
+    # dcm2niix also raises warnings if parameter value varies. For an example
+    # See https://github.com/rordenlab/dcm2niix/blob/bb3a6c35d2bbac6ed95acb2cd0df65f35e79b5fb/console/nii_dicom.cpp#L2352 # noqa
+
+    # If previous value was None, and another dcm file
+    # has a value (not None), replace None in params.
+    for item in parameter_diff_list:
+        if item[0] == 'change':
+            _, parameter_name, [new_value, old_value] = item
+            if new_value is not None:
+                if old_value is None:
+                    params[parameter_name] = new_value
+                else:
+                    logger.warning(f'Slices with varying {parameter_name} '
+                                   f'Expected {old_value}, Got {new_value} in '
+                                   f'{filepath}')
+        elif item[0] == 'add':
+            logger.debug('Not expected. Report event - %s', item[0])
+            for parameter_name, value in item[2]:
+                params[parameter_name] = value
+        else:
+            logger.debug('Not expected. Report event - %s', item[0])
+    return params
```

### Comparing `MRdataset-0.1.3/versioneer.py` & `MRdataset-0.1.6/versioneer.py`

 * *Files identical despite different names*

