# Comparing `tmp/autosubmitconfigparser-1.0.32.tar.gz` & `tmp/autosubmitconfigparser-1.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmitconfigparser-1.0.32.tar", last modified: Wed Jun  7 12:24:11 2023, max compression
+gzip compressed data, was "autosubmitconfigparser-1.0.33.tar", last modified: Wed Jun  7 14:00:53 2023, max compression
```

## Comparing `autosubmitconfigparser-1.0.32.tar` & `autosubmitconfigparser-1.0.33.tar`

### file list

```diff
@@ -1,51 +1,34 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.839842 autosubmitconfigparser-1.0.32/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      187 2023-02-08 10:33:31.000000 autosubmitconfigparser-1.0.32/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-09-23 10:01:03.000000 autosubmitconfigparser-1.0.32/CHANGELOG
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.32/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-06-07 12:24:11.839842 autosubmitconfigparser-1.0.32/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.32/README.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        6 2023-06-07 12:12:55.000000 autosubmitconfigparser-1.0.32/VERSION
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmitconfigparser-1.0.32/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      162 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/__pycache__/__init__.cpython-37.pyc
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      169 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4469 2023-06-06 08:56:07.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    75347 2023-06-06 08:56:07.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/basicconfig.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   104405 2023-06-07 12:09:09.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/configcommon.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/autosubmit-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/autosubmit.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/expdef-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/expdef.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/git-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/jobs-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/jobs.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/local-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/platforms-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/platforms.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      275 2023-06-07 12:06:41.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/yamlparser.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.835842 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-06-07 12:24:11.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1525 2023-06-07 12:24:11.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-06-07 12:24:11.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      305 2023-06-07 12:24:11.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-06-07 12:24:11.000000 autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/top_level.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      591 2023-06-07 12:12:55.000000 autosubmitconfigparser-1.0.32/environment.yml
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.839842 autosubmitconfigparser-1.0.32/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.32/log/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 12:24:11.839842 autosubmitconfigparser-1.0.32/log/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      143 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.32/log/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12336 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.32/log/__pycache__/log.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.32/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.32/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      416 2023-06-07 12:12:55.000000 autosubmitconfigparser-1.0.32/requeriments.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-06-07 12:24:11.839842 autosubmitconfigparser-1.0.32/setup.cfg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1465 2023-06-07 12:12:55.000000 autosubmitconfigparser-1.0.32/setup.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1254 2023-01-31 09:30:38.000000 autosubmitconfigparser-1.0.32/test_config.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.33/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2123 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.33/README.md
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/autosubmitconfigparser/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:48:23.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:49:24.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/__init__.py
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/basicconfig.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   104405 2023-06-07 13:56:15.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/configcommon.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/autosubmit-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/autosubmit.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/expdef-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/expdef.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/git-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/jobs-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/jobs.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/local-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/platforms-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/platforms.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      275 2023-06-07 12:06:41.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/yamlparser.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2123 2023-06-07 14:00:52.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1029 2023-06-07 14:00:53.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-06-07 14:00:52.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      338 2023-06-07 14:00:52.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-06-07 14:00:53.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/top_level.txt
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.33/log/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.33/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.33/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/setup.cfg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1499 2023-06-07 14:00:30.000000 autosubmitconfigparser-1.0.33/setup.py
```

### Comparing `autosubmitconfigparser-1.0.32/PKG-INFO` & `autosubmitconfigparser-1.0.33/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.32
+Version: 1.0.33
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
+License: UNKNOWN
 Keywords: climate,weather,workflow,HPC
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 
 Simple library that allows to read the data of an Autosubmit experiment.
@@ -56,7 +58,9 @@
 # This is a sample text with a placeholder expid
 
 # delete samples
 os.remove("as_sample.txt")
 os.remove("as_sample_parsed.txt")
 ```
 
+
+
```

### Comparing `autosubmitconfigparser-1.0.32/README.md` & `autosubmitconfigparser-1.0.33/README.md`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/basicconfig.py` & `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/basicconfig.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/configcommon.py` & `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/configcommon.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/expdef-dummy.yml` & `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/expdef-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/expdef.yml` & `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/expdef.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/jobs-dummy.yml` & `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/jobs-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/jobs.yml` & `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/jobs.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/platforms-dummy.yml` & `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/platforms-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.32/autosubmitconfigparser/config/files/platforms.yml` & `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/platforms.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.32/autosubmitconfigparser.egg-info/PKG-INFO` & `autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.32
+Version: 1.0.33
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
+License: UNKNOWN
 Keywords: climate,weather,workflow,HPC
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 
 Simple library that allows to read the data of an Autosubmit experiment.
@@ -56,7 +58,9 @@
 # This is a sample text with a placeholder expid
 
 # delete samples
 os.remove("as_sample.txt")
 os.remove("as_sample_parsed.txt")
 ```
 
+
+
```

### Comparing `autosubmitconfigparser-1.0.32/log/fd_show.py` & `autosubmitconfigparser-1.0.33/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.32/log/log.py` & `autosubmitconfigparser-1.0.33/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.32/setup.py` & `autosubmitconfigparser-1.0.33/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autosubmitconfigparser",
-    version="1.0.32",
+    version="1.0.33",
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
-    install_requires=['packaging>19', 'six>=1.10.0', 'configobj>=5.0.6', 'argparse>=1.4.0', 'python-dateutil>=2.8.2',
+    install_requires=['ruamel.yaml==0.17.31','ruamel.yaml.clib==0.2.7','packaging>19', 'six>=1.10.0', 'configobj>=5.0.6', 'argparse>=1.4.0', 'python-dateutil>=2.8.2',
                        'pyparsing>=3.0.7',
                       'mock>=4.0.3', 'portalocker>=2.3.2', 'networkx>=2.6.3', 'requests>=2.27.1',
                       'bscearth.utils>=0.5.2', 'cryptography>=36.0.1', 'setuptools>=60.8.2',
-                      'pip>=22.0.3', 'ruamel.yaml', 'pythondialog', 'pytest', 'nose', 'coverage', 'PyNaCl>=1.4.0',
+                      'pip>=22.0.3', 'pythondialog', 'pytest', 'nose', 'coverage', 'PyNaCl>=1.4.0',
                       'Pygments'],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: POSIX :: Linux"
     ],
```

