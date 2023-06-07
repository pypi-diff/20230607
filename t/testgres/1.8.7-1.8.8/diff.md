# Comparing `tmp/testgres-1.8.7.tar.gz` & `tmp/testgres-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgres-1.8.7.tar", last modified: Wed May 10 12:05:11 2023, max compression
+gzip compressed data, was "testgres-1.8.8.tar", last modified: Wed Jun  7 02:32:48 2023, max compression
```

## Comparing `testgres-1.8.7.tar` & `testgres-1.8.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:05:11.636103 testgres-1.8.7/
--rw-rw-r--   0 root         (0) root         (0)     1106 2023-05-10 11:22:06.000000 testgres-1.8.7/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      136 2022-02-22 09:57:57.000000 testgres-1.8.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5753 2023-05-10 12:05:11.636103 testgres-1.8.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5399 2023-05-05 04:23:08.000000 testgres-1.8.7/README.md
--rw-rw-r--   0 root         (0) root         (0)      160 2023-05-10 12:05:11.636103 testgres-1.8.7/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1011 2023-05-10 11:40:41.000000 testgres-1.8.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:05:11.632103 testgres-1.8.7/testgres/
--rw-rw-r--   0 root         (0) root         (0)     1519 2023-05-05 04:23:08.000000 testgres-1.8.7/testgres/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1524 2022-02-22 09:57:57.000000 testgres-1.8.7/testgres/api.py
--rw-rw-r--   0 root         (0) root         (0)     5187 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/backup.py
--rw-rw-r--   0 root         (0) root         (0)     2195 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/cache.py
--rw-rw-r--   0 root         (0) root         (0)     4781 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/config.py
--rw-rw-r--   0 root         (0) root         (0)     3080 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/connection.py
--rw-rw-r--   0 root         (0) root         (0)      819 2022-02-22 09:57:57.000000 testgres-1.8.7/testgres/consts.py
--rw-rw-r--   0 root         (0) root         (0)     1749 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/decorators.py
--rw-rw-r--   0 root         (0) root         (0)      932 2022-02-22 09:57:57.000000 testgres-1.8.7/testgres/defaults.py
--rw-rw-r--   0 root         (0) root         (0)     2451 2023-05-05 04:23:08.000000 testgres-1.8.7/testgres/enums.py
--rw-rw-r--   0 root         (0) root         (0)     1988 2022-02-22 09:57:57.000000 testgres-1.8.7/testgres/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     1428 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/logger.py
--rw-rw-r--   0 root         (0) root         (0)    51631 2023-05-05 10:42:56.000000 testgres-1.8.7/testgres/node.py
--rw-rw-r--   0 root         (0) root         (0)     8225 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/pubsub.py
--rw-rw-r--   0 root         (0) root         (0)     1547 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/standby.py
--rw-rw-r--   0 root         (0) root         (0)     6283 2022-11-09 15:43:39.000000 testgres-1.8.7/testgres/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:05:11.636103 testgres-1.8.7/testgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5753 2023-05-10 12:05:11.000000 testgres-1.8.7/testgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2023-05-10 12:05:11.000000 testgres-1.8.7/testgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 12:05:11.000000 testgres-1.8.7/testgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-10 12:05:11.000000 testgres-1.8.7/testgres.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-10 12:05:11.000000 testgres-1.8.7/testgres.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:05:11.636103 testgres-1.8.7/tests/
--rwxrwxr-x   0 root         (0) root         (0)    34618 2023-05-05 04:23:08.000000 testgres-1.8.7/tests/test_simple.py
+drwxrwxr-x   0 pge       (1003) pge       (1003)        0 2023-06-07 02:32:48.621387 testgres-1.8.8/
+-rw-rw-r--   0 pge       (1003) pge       (1003)     1106 2023-05-10 11:22:06.000000 testgres-1.8.8/LICENSE
+-rw-rw-r--   0 pge       (1003) pge       (1003)      136 2022-02-22 09:57:57.000000 testgres-1.8.8/MANIFEST.in
+-rw-rw-r--   0 pge       (1003) pge       (1003)     7198 2023-06-07 02:32:48.621387 testgres-1.8.8/PKG-INFO
+-rw-rw-r--   0 pge       (1003) pge       (1003)     5399 2023-05-05 04:23:08.000000 testgres-1.8.8/README.md
+-rw-rw-r--   0 pge       (1003) pge       (1003)      160 2023-06-07 02:32:48.621387 testgres-1.8.8/setup.cfg
+-rwxrwxr-x   0 pge       (1003) pge       (1003)     1011 2023-06-07 02:28:30.000000 testgres-1.8.8/setup.py
+drwxrwxr-x   0 pge       (1003) pge       (1003)        0 2023-06-07 02:32:48.621387 testgres-1.8.8/testgres/
+-rw-rw-r--   0 pge       (1003) pge       (1003)     1519 2023-05-05 04:23:08.000000 testgres-1.8.8/testgres/__init__.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     1524 2022-02-22 09:57:57.000000 testgres-1.8.8/testgres/api.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     5187 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/backup.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     2195 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/cache.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     4781 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/config.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     3080 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/connection.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)      819 2022-02-22 09:57:57.000000 testgres-1.8.8/testgres/consts.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     1749 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/decorators.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)      932 2022-02-22 09:57:57.000000 testgres-1.8.8/testgres/defaults.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     2451 2023-05-05 04:23:08.000000 testgres-1.8.8/testgres/enums.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     1988 2022-02-22 09:57:57.000000 testgres-1.8.8/testgres/exceptions.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     1428 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/logger.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)    51775 2023-06-07 02:28:30.000000 testgres-1.8.8/testgres/node.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     8225 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/pubsub.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     1547 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/standby.py
+-rw-rw-r--   0 pge       (1003) pge       (1003)     6360 2023-06-07 02:28:30.000000 testgres-1.8.8/testgres/utils.py
+drwxrwxr-x   0 pge       (1003) pge       (1003)        0 2023-06-07 02:32:48.621387 testgres-1.8.8/testgres.egg-info/
+-rw-rw-r--   0 pge       (1003) pge       (1003)     7198 2023-06-07 02:32:48.000000 testgres-1.8.8/testgres.egg-info/PKG-INFO
+-rw-rw-r--   0 pge       (1003) pge       (1003)      541 2023-06-07 02:32:48.000000 testgres-1.8.8/testgres.egg-info/SOURCES.txt
+-rw-rw-r--   0 pge       (1003) pge       (1003)        1 2023-06-07 02:32:48.000000 testgres-1.8.8/testgres.egg-info/dependency_links.txt
+-rw-rw-r--   0 pge       (1003) pge       (1003)       49 2023-06-07 02:32:48.000000 testgres-1.8.8/testgres.egg-info/requires.txt
+-rw-rw-r--   0 pge       (1003) pge       (1003)        9 2023-06-07 02:32:48.000000 testgres-1.8.8/testgres.egg-info/top_level.txt
+drwxrwxr-x   0 pge       (1003) pge       (1003)        0 2023-06-07 02:32:48.621387 testgres-1.8.8/tests/
+-rwxrwxr-x   0 pge       (1003) pge       (1003)    34618 2023-05-05 04:23:08.000000 testgres-1.8.8/tests/test_simple.py
```

### Comparing `testgres-1.8.7/LICENSE` & `testgres-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/PKG-INFO` & `testgres-1.8.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: testgres
-Version: 1.8.7
-Summary: Testing utility for PostgreSQL and its extensions
-Home-page: https://github.com/postgrespro/testgres
-Author: Ildar Musin
-Author-email: zildermann@gmail.com
-License: PostgreSQL
-Keywords: test,testing,postgresql
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Build Status](https://travis-ci.com/postgrespro/testgres.svg?branch=master)](https://app.travis-ci.com/github/postgrespro/testgres/branches)
 [![codecov](https://codecov.io/gh/postgrespro/testgres/branch/master/graph/badge.svg)](https://codecov.io/gh/postgrespro/testgres)
 [![PyPI version](https://badge.fury.io/py/testgres.svg)](https://badge.fury.io/py/testgres)
 
 [Documentation](https://postgrespro.github.io/testgres/)
 
 # testgres
@@ -189,9 +176,7 @@
 
 ## Authors
 
 [Ildar Musin](https://github.com/zilder)  
 [Dmitry Ivanov](https://github.com/funbringer)  
 [Ildus Kurbangaliev](https://github.com/ildus)  
 [Yury Zhuravlev](https://github.com/stalkerg)  
-
-
```

### Comparing `testgres-1.8.7/setup.py` & `testgres-1.8.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     install_requires.append("ipaddress")
 
 # Get contents of README file
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
-    version='1.8.7',
+    version='1.8.8',
     name='testgres',
     packages=['testgres'],
     description='Testing utility for PostgreSQL and its extensions',
     url='https://github.com/postgrespro/testgres',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='PostgreSQL',
```

### Comparing `testgres-1.8.7/testgres/__init__.py` & `testgres-1.8.8/testgres/__init__.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/api.py` & `testgres-1.8.8/testgres/api.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/backup.py` & `testgres-1.8.8/testgres/backup.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/cache.py` & `testgres-1.8.8/testgres/cache.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/config.py` & `testgres-1.8.8/testgres/config.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/connection.py` & `testgres-1.8.8/testgres/connection.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/consts.py` & `testgres-1.8.8/testgres/consts.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/decorators.py` & `testgres-1.8.8/testgres/decorators.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/defaults.py` & `testgres-1.8.8/testgres/defaults.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/enums.py` & `testgres-1.8.8/testgres/enums.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/exceptions.py` & `testgres-1.8.8/testgres/exceptions.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/logger.py` & `testgres-1.8.8/testgres/logger.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/node.py` & `testgres-1.8.8/testgres/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1589,16 +1589,18 @@
 
     def make_simple(
             self,
             base_dir=None,
             set_replication=False,
             ptrack_enable=False,
             initdb_params=[],
-            pg_options={}):
-
+            pg_options={},
+            checksum=True):
+        if checksum and '--data-checksums' not in initdb_params:
+            initdb_params.append('--data-checksums')
         node = self.make_empty(base_dir)
         node.init(
             initdb_params=initdb_params, allow_streaming=set_replication)
 
         # set major version
         with open(os.path.join(node.data_dir, 'PG_VERSION')) as f:
             node.major_version_str = str(f.read().rstrip())
```

### Comparing `testgres-1.8.7/testgres/pubsub.py` & `testgres-1.8.8/testgres/pubsub.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/standby.py` & `testgres-1.8.8/testgres/standby.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/testgres/utils.py` & `testgres-1.8.8/testgres/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 import port_for
 import subprocess
 import sys
 import tempfile
 
 from contextlib import contextmanager
 from packaging.version import Version
-from distutils.spawn import find_executable
+try:
+    from shutil import which as find_executable
+except ImportError:
+    from distutils.spawn import find_executable
 from six import iteritems
 
 from .config import testgres_config
 from .exceptions import ExecUtilException
 
 # rows returned by PG_CONFIG
 _pg_config_data = {}
```

### Comparing `testgres-1.8.7/testgres.egg-info/SOURCES.txt` & `testgres-1.8.8/testgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testgres-1.8.7/tests/test_simple.py` & `testgres-1.8.8/tests/test_simple.py`

 * *Files identical despite different names*

