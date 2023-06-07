# Comparing `tmp/autosubmitconfigparser-1.0.31.tar.gz` & `tmp/autosubmitconfigparser-1.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmitconfigparser-1.0.31.tar", last modified: Thu Jun  1 13:53:37 2023, max compression
+gzip compressed data, was "autosubmitconfigparser-1.0.32.tar", last modified: Wed Jun  7 12:24:11 2023, max compression
```

## Comparing `autosubmitconfigparser-1.0.31.tar` & `autosubmitconfigparser-1.0.32.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-01 13:53:37.571846 autosubmitconfigparser-1.0.31/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      187 2023-02-08 10:33:31.000000 autosubmitconfigparser-1.0.31/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-09-23 10:01:03.000000 autosubmitconfigparser-1.0.31/CHANGELOG
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.31/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-06-01 13:53:37.571846 autosubmitconfigparser-1.0.31/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.31/README.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        6 2023-06-01 13:40:36.000000 autosubmitconfigparser-1.0.31/VERSION
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmitconfigparser-1.0.31/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-01 13:53:37.563846 autosubmitconfigparser-1.0.31/autosubmitconfigparser/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-01 13:53:37.567846 autosubmitconfigparser-1.0.31/autosubmitconfigparser/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      162 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/__pycache__/__init__.cpython-37.pyc
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-01 13:53:37.567846 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-01 13:53:37.567846 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      169 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4469 2023-05-15 08:55:06.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    75347 2023-05-16 10:32:31.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/basicconfig.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   100818 2023-06-01 13:35:42.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/configcommon.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-01 13:53:37.567846 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/autosubmit-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/autosubmit.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/expdef-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/expdef.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/git-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/jobs-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/jobs.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/local-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/platforms-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/platforms.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      408 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/yamlparser.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-01 13:53:37.567846 autosubmitconfigparser-1.0.31/autosubmitconfigparser.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-06-01 13:53:37.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1525 2023-06-01 13:53:37.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-06-01 13:53:37.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      314 2023-06-01 13:53:37.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-06-01 13:53:37.000000 autosubmitconfigparser-1.0.31/autosubmitconfigparser.egg-info/top_level.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      600 2023-05-05 11:20:51.000000 autosubmitconfigparser-1.0.31/environment.yml
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-01 13:53:37.567846 autosubmitconfigparser-1.0.31/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.31/log/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-01 13:53:37.571846 autosubmitconfigparser-1.0.31/log/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      143 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.31/log/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12336 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.31/log/__pycache__/log.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.31/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.31/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      425 2023-05-05 11:20:51.000000 autosubmitconfigparser-1.0.31/requeriments.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-06-01 13:53:37.571846 autosubmitconfigparser-1.0.31/setup.cfg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1474 2023-06-01 13:40:36.000000 autosubmitconfigparser-1.0.31/setup.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1254 2023-01-31 09:30:38.000000 autosubmitconfigparser-1.0.31/test_config.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.839842 autosubmitconfigparser-1.0.32/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      187 2023-02-08 10:33:31.000000 autosubmitconfigparser-1.0.32/.gitignore
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-09-23 10:01:03.000000 autosubmitconfigparser-1.0.32/CHANGELOG
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.32/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-06-07 12:24:11.839842 autosubmitconfigparser-1.0.32/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.32/README.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        6 2023-06-07 12:12:55.000000 autosubmitconfigparser-1.0.32/VERSION
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmitconfigparser-1.0.32/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      162 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/__pycache__/__init__.cpython-37.pyc
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      169 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4469 2023-06-06 08:56:07.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    75347 2023-06-06 08:56:07.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/basicconfig.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   104405 2023-06-07 12:09:09.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/configcommon.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/autosubmit-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/autosubmit.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/expdef-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/expdef.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/git-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/jobs-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/jobs.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/local-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/platforms-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/platforms.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      275 2023-06-07 12:06:41.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/yamlparser.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-06-07 12:24:11.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1525 2023-06-07 12:24:11.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-06-07 12:24:11.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      305 2023-06-07 12:24:11.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-06-07 12:24:11.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/top_level.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      591 2023-06-07 12:12:55.000000 autosubmitconfigparser-1.0.32/environment.yml
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.839842 autosubmitconfigparser-1.0.32/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.32/log/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.839842 autosubmitconfigparser-1.0.32/log/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      143 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.32/log/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12336 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.32/log/__pycache__/log.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.32/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.32/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      416 2023-06-07 12:12:55.000000 autosubmitconfigparser-1.0.32/requeriments.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-06-07 12:24:11.839842 autosubmitconfigparser-1.0.32/setup.cfg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1465 2023-06-07 12:12:55.000000 autosubmitconfigparser-1.0.32/setup.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1254 2023-01-31 09:30:38.000000 autosubmitconfigparser-1.0.32/test_config.py
```

### Comparing `autosubmitconfigparser-1.0.31/PKG-INFO` & `autosubmitconfigparser-1.0.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.31
+Version: 1.0.32
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 Keywords: climate,weather,workflow,HPC
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `autosubmitconfigparser-1.0.31/README.md` & `autosubmitconfigparser-1.0.32/README.md`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/basicconfig.py` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/basicconfig.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/configcommon.py` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/configcommon.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 import shutil
 import numbers
 
-
 import os
 import re
 import subprocess
 import traceback
 import json
 import ruamel.yaml as yaml
 from .basicconfig import BasicConfig
@@ -48,23 +47,26 @@
     Class to handle experiment configuration coming from file or database
 
     :param expid: experiment identifier
     :type expid: str
     """
 
     def __init__(self, expid, basic_config=BasicConfig, parser_factory=YAMLParserFactory()):
+        self.data_changed = False
         self.ignore_undefined_platforms = False
         self.ignore_file_path = False
         self.expid = expid
         self.basic_config = basic_config
         self.basic_config.read()
         self.parser_factory = parser_factory
         self.experiment_data = {}
+        self.last_experiment_data = {}
         self.data_loops = list()
 
+
         self.current_loaded_files = dict()
         self.conf_folder_yaml = Path(BasicConfig.LOCAL_ROOT_DIR, expid, "conf")
 
         self.wrong_config = defaultdict(list)
         self.warn_config = defaultdict(list)
         self.dynamic_variables = list()
         self.starter_conf = dict()
@@ -1216,15 +1218,20 @@
 
             jobs_in_wrapper = wrapper_values.get('JOBS_IN_WRAPPER',"")
             if "&" in jobs_in_wrapper:
                 jobs_in_wrapper = jobs_in_wrapper.split("&")
             else:
                 jobs_in_wrapper = jobs_in_wrapper.split(" ")
             for section in jobs_in_wrapper:
-                platform_name = self.jobs_data[section].get('PLATFORM',"").upper()
+                try:
+                    platform_name = self.jobs_data[section].get('PLATFORM',"").upper()
+                except:
+                    self.wrong_config["WRAPPERS"] += [[wrapper_name,
+                                                      "JOBS_IN_WRAPPER contains non-defined jobs.  parameter is invalid"]]
+                    continue
                 if platform_name == "":
                     platform_name = self.get_platform().upper()
                 if platform_name == "LOCAL":
                     continue
                 if not self.is_valid_jobs_in_wrapper(wrapper_values):
                     self.wrong_config["WRAPPERS"] += [[wrapper_name,
                                                       "JOBS_IN_WRAPPER contains non-defined jobs.  parameter is invalid"]]
@@ -1333,33 +1340,28 @@
         :return:
         """
         # This is a recursive call
         current_data_pre,current_data_post = self.load_custom_config(current_data, filenames_to_load)
         # Unifies all pre and post data of the current pre or post data. Think of it as a tree with two branches that needs to be unified at each level
         return self.substitute_dynamic_variables(self.unify_conf(self.unify_conf(current_data_pre,current_data),current_data_post))
 
-    def reload(self,force_load=False,only_experiment_data = False):
+    def reload(self,force_load=False,only_experiment_data = False,save= False):
         """
         Reloads the configuration files
         :param force_load: If True, reloads all the files, if False, reloads only the modified files
         """
         # Check if the files have been modified or if they need a reload
         files_to_reload = []
         # Reload only the files that have been modified
-        for yaml_name,last_known_modtime in self.current_loaded_files.items():
-            if Path(yaml_name).stat().st_mtime > last_known_modtime:
-                files_to_reload.append(yaml_name)
-        #  TODO What we should really reload? right now is all files , hard to track the changes in files with custom_config of custom_config
-        #if (len(self.current_loaded_files) > 0 and len(files_to_reload) > 0) and not force_load:
-        #    self.experiment_data = self.load_config_folder(self.experiment_data,files_to_reload)
-        # Check if reload is allowed, new parameter # TODO doc users may want to change configuration without affecting to the current autosubmit run
-        if ( len(files_to_reload) > 0 and self.experiment_data.get("CONFIG", {}).get("RELOAD_WHILE_RUNNING", True) ) or len(self.current_loaded_files) == 0 or force_load:
+        self.load_last_run() # from unified conf if any.
+        # Only reload the data if there are changes or there is no data loaded yet
+        if force_load or (self.data_changed and self.experiment_data.get("CONFIG", {}).get("RELOAD_WHILE_RUNNING", True)):
+            files_to_reload = self.current_loaded_files.keys()
+        if len(files_to_reload) > 0 or len(self.current_loaded_files) == 0 :
             # Load all the files starting from the $expid/conf folder
-            if len(files_to_reload) > 0:
-                Log.result(f"Reloading configuration files, due a change in the following files: {files_to_reload}")
             starter_conf = {}
             self.current_loaded_files = {} # reset loaded files
             for filename in self.get_yaml_filenames_to_load(self.conf_folder_yaml):
                 starter_conf = self.unify_conf(starter_conf, self.load_config_file(starter_conf, Path(filename)))
             starter_conf = self.load_common_parameters(starter_conf)
             starter_conf = self.substitute_dynamic_variables(starter_conf)
             self.starter_conf = starter_conf
@@ -1370,34 +1372,105 @@
                 non_minimal_files[str(filename)] = Path(filename).stat().st_mtime
                 non_minimal_conf = self.unify_conf(non_minimal_conf, self.load_config_file(non_minimal_conf, Path(filename)))
             non_minimal_conf = self.load_common_parameters(non_minimal_conf)
             non_minimal_conf = self.substitute_dynamic_variables(non_minimal_conf, max_deep=25)
             # Start loading the custom config files
             # Gets the files to load
             filenames_to_load = self.parse_custom_conf_directive(starter_conf.get("DEFAULT",{}).get("CUSTOM_CONFIG",None))
-            #debug
             if not only_experiment_data:
                 # Loads all configuration associated with the project data "pre"
                 custom_conf_pre = self.load_custom_config_section({}, filenames_to_load["PRE"])
                 # Loads all configuration associated with the user data "post"
                 self.experiment_data = self.load_custom_config_section(self.unify_conf(custom_conf_pre,non_minimal_conf),filenames_to_load["POST"])
             else:
                 self.experiment_data = starter_conf
             self.experiment_data = self.substitute_dynamic_variables(self.experiment_data, max_deep=25)
             ###
             self.current_loaded_files.update(non_minimal_files)
             if "AS_TEMP" in self.experiment_data.keys():
                 del self.experiment_data["AS_TEMP"]
             # IF expid and hpcarch are not defined, use the ones from the minimal.yml file
             self.deep_add_missing_starter_conf(self.experiment_data,starter_conf)
-
             self.experiment_data = self.substitute_dynamic_variables(self.experiment_data)
             self.experiment_data = self.normalize_variables(self.experiment_data)
-            pass
+    def load_last_run(self):
+        self.metadata_folder = Path(self.conf_folder_yaml) / "metadata"
+        if not self.metadata_folder.exists():
+            os.makedirs(self.metadata_folder)
+            os.chmod(self.metadata_folder, 0o775)
+        if not os.access(self.metadata_folder, os.W_OK):
+            print(f"WARNING: Can't save the experiment data into {self.metadata_folder}, no write permissions")
+        else:
+            # Load data from last run
+            if (Path(self.metadata_folder) / "experiment_data.yml").exists():
+                with open(Path(self.metadata_folder) / "experiment_data.yml", 'r') as stream:
+                    self.last_experiment_data = yaml.load(stream)
+                self.data_changed = self.quick_deep_diff(self.experiment_data, self.last_experiment_data)
+            else:
+                self.last_experiment_data = {}
+    def save(self):
+        """
+        Saves the experiment data into the experiment_folder/conf/metadata folder as a yaml file
+        :return: True if the data has changed, False otherwise
+        """
+        changed = False
+        # check if the folder exists and we have write permissions, if folder doesn't exist create it with rwx/rwx/r-x permissions
+        # metadata folder is inside the experiment folder / conf folder / metadata folder
+        # If this function is called before load_last_run, we need to load the last run
+        if len(self.last_experiment_data) > 0:
+            self.load_last_run()
+        if self.data_changed:
+            # Backup the old file
+            if (Path(self.metadata_folder) / "experiment_data.yml").exists():
+                shutil.copy(Path(self.metadata_folder) / "experiment_data.yml", Path(self.metadata_folder) / "experiment_data.yml.bak")
+            with open(Path(self.metadata_folder) / "experiment_data.yml", 'w') as stream:
+                yaml.dump(self.experiment_data, stream, default_flow_style=False)
+            print(f"Saving experiment data into {self.metadata_folder}")
+        else:
+            print(f"Experiment data has not changed, no save is needed")
+        return self.data_changed
+    def detailed_deep_diff(self, current_data, last_run_data, differences={}):
+        """
+        Returns a dictionary with for each key, the difference between the current configuration and the last_run_data
+        :param current_data: dictionary with the current data
+        :param last_run_data: dictionary with the last_run_data data
+        :return: differences: dictionary
+        """
+        for key, val in current_data.items():
+            if isinstance(val, collections.abc.Mapping):
+                if key not in last_run_data.keys():
+                    differences[key] = val
+                else:
+                    self.detailed_deep_diff(last_run_data[key], val, differences)
+            else:
+                if key not in last_run_data.keys() or last_run_data[key] != val:
+                    differences[key] = val
+        return differences
+
+    def quick_deep_diff(self, current_data, last_run_data, changed = False):
+        """
+        Returns if there is any difference between the current configuration and the stored one
+        :param last_run_data: dictionary with the stored data
+        :return: changed: boolean, True if the configuration has changed
+        """
 
+        if changed:
+            return True
+        for key, val in current_data.items():
+            if isinstance(val, collections.abc.Mapping):
+                if key not in last_run_data.keys():
+                    changed = True
+                    break
+                else:
+                    changed = self.quick_deep_diff(last_run_data[key], val, changed)
+            else:
+                if key not in last_run_data.keys() or last_run_data[key] != val:
+                    changed = True
+                    break
+        return changed
     def deep_add_missing_starter_conf(self,experiment_data,starter_conf):
         """
         Add the missing keys from starter_conf to experiment_data
         :param experiment_data:
         :param starter_conf:
         :return:
         """
```

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/expdef-dummy.yml` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/expdef-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/expdef.yml` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/expdef.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/jobs-dummy.yml` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/jobs-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/jobs.yml` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/jobs.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/platforms-dummy.yml` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/platforms-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser/config/files/platforms.yml` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/platforms.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser.egg-info/PKG-INFO` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.31
+Version: 1.0.32
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 Keywords: climate,weather,workflow,HPC
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `autosubmitconfigparser-1.0.31/autosubmitconfigparser.egg-info/SOURCES.txt` & `autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/environment.yml` & `autosubmitconfigparser-1.0.32/environment.yml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   - portalocker>=2.3.2
   - requests>=2.27.1
   - bscearth.utils>=0.5.2
   - cryptography>=36.0.1
   - setuptools>=60.8.2
   - six>=1.10.0
   - xlib>=0.21
-  - ruamel.yaml==0.17.21
+  - ruamel.yaml
   - pythondialog
   - pytest
   - nose
   - coverage
   - requests
   - configobj
```

### Comparing `autosubmitconfigparser-1.0.31/log/__pycache__/log.cpython-37.pyc` & `autosubmitconfigparser-1.0.32/log/__pycache__/log.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/log/fd_show.py` & `autosubmitconfigparser-1.0.32/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/log/log.py` & `autosubmitconfigparser-1.0.32/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.31/setup.py` & `autosubmitconfigparser-1.0.32/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autosubmitconfigparser",
-    version="1.0.31",
+    version="1.0.32",
     author="Daniel Beltran Mora",
     author_email="daniel.beltran@bsc.es",
     description="An utility library that allows to read an Autosubmit 4 experiment configuration.",
     keywords=['climate', 'weather', 'workflow', 'HPC'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git",
     include_package_data=True,
     package_data={'files': ['autosubmitconfigparser/conf/files/*']},
     packages=setuptools.find_packages(),
     install_requires=['packaging>19', 'six>=1.10.0', 'configobj>=5.0.6', 'argparse>=1.4.0', 'python-dateutil>=2.8.2',
                        'pyparsing>=3.0.7',
                       'mock>=4.0.3', 'portalocker>=2.3.2', 'networkx>=2.6.3', 'requests>=2.27.1',
                       'bscearth.utils>=0.5.2', 'cryptography>=36.0.1', 'setuptools>=60.8.2',
-                      'pip>=22.0.3', 'ruamel.yaml==0.17.21', 'pythondialog', 'pytest', 'nose', 'coverage', 'PyNaCl>=1.4.0',
+                      'pip>=22.0.3', 'ruamel.yaml', 'pythondialog', 'pytest', 'nose', 'coverage', 'PyNaCl>=1.4.0',
                       'Pygments'],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: POSIX :: Linux"
     ],
```

### Comparing `autosubmitconfigparser-1.0.31/test_config.py` & `autosubmitconfigparser-1.0.32/test_config.py`

 * *Files identical despite different names*

