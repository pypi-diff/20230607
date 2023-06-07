# Comparing `tmp/jittok-0.0.5.tar.gz` & `tmp/jittok-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jittok-0.0.5.tar", last modified: Fri Apr 21 15:07:01 2023, max compression
+gzip compressed data, was "jittok-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jittok-0.0.5.tar` & `jittok-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,22 @@
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.189279 jittok-0.0.5/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     1073 2022-10-23 11:33:34.000000 jittok-0.0.5/LICENSE
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     1369 2023-04-21 15:07:01.189279 jittok-0.0.5/PKG-INFO
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     1067 2023-03-20 14:04:49.000000 jittok-0.0.5/README.md
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.185279 jittok-0.0.5/jittok/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      233 2023-04-21 15:05:21.000000 jittok-0.0.5/jittok/__init__.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       30 2023-02-14 13:34:36.000000 jittok-0.0.5/jittok/__main__.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      497 2023-02-14 13:34:36.000000 jittok-0.0.5/jittok/cli.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      233 2022-11-08 13:52:24.000000 jittok-0.0.5/jittok/core.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       36 2022-11-08 13:52:24.000000 jittok-0.0.5/jittok/exceptions.py
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.185279 jittok-0.0.5/jittok/jpaddress/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      123 2023-03-24 14:39:08.000000 jittok-0.0.5/jittok/jpaddress/__init__.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     6525 2023-03-24 14:39:08.000000 jittok-0.0.5/jittok/jpaddress/core.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      150 2023-03-24 14:39:08.000000 jittok-0.0.5/jittok/jpaddress/exceptions.py
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.185279 jittok-0.0.5/jittok/jpdatetime/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       51 2023-03-20 14:04:49.000000 jittok-0.0.5/jittok/jpdatetime/__init__.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     1832 2023-03-20 14:04:49.000000 jittok-0.0.5/jittok/jpdatetime/core.py
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.189279 jittok-0.0.5/jittok/jptext/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      303 2023-03-02 13:14:13.000000 jittok-0.0.5/jittok/jptext/__init__.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      422 2023-02-14 13:34:36.000000 jittok-0.0.5/jittok/jptext/cli.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     6389 2023-04-21 15:02:22.000000 jittok-0.0.5/jittok/jptext/core.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      146 2023-02-13 12:57:35.000000 jittok-0.0.5/jittok/jptext/exceptions.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)        0 2023-02-15 00:21:42.000000 jittok-0.0.5/jittok/py.typed
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.185279 jittok-0.0.5/jittok.egg-info/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     1369 2023-04-21 15:07:01.000000 jittok-0.0.5/jittok.egg-info/PKG-INFO
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      576 2023-04-21 15:07:01.000000 jittok-0.0.5/jittok.egg-info/SOURCES.txt
--rw-rw-r--   0 osoken    (1000) osoken    (1000)        1 2023-04-21 15:07:01.000000 jittok-0.0.5/jittok.egg-info/dependency_links.txt
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       81 2023-04-21 15:07:01.000000 jittok-0.0.5/jittok.egg-info/requires.txt
--rw-rw-r--   0 osoken    (1000) osoken    (1000)        7 2023-04-21 15:07:01.000000 jittok-0.0.5/jittok.egg-info/top_level.txt
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       38 2023-04-21 15:07:01.189279 jittok-0.0.5/setup.cfg
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     1164 2023-03-24 15:17:43.000000 jittok-0.0.5/setup.py
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.189279 jittok-0.0.5/tests/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     1600 2023-02-14 13:34:36.000000 jittok-0.0.5/tests/test_cli.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      253 2023-02-14 13:34:36.000000 jittok-0.0.5/tests/test_core.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       98 2022-10-31 11:27:53.000000 jittok-0.0.5/tests/test_package.py
+-rw-r--r--   0        0        0     1073 2023-06-07 13:44:22.368995 jittok-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1067 2023-06-07 13:44:22.368995 jittok-0.0.6/README.md
+-rw-r--r--   0        0        0      105 2023-06-07 14:26:06.210881 jittok-0.0.6/jittok/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/__main__.py
+-rw-r--r--   0        0        0       18 2023-06-07 14:31:40.795395 jittok-0.0.6/jittok/_version.py
+-rw-r--r--   0        0        0      163 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/blob/__init__.py
+-rw-r--r--   0        0        0     1042 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/blob/core.py
+-rw-r--r--   0        0        0      497 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/cli.py
+-rw-r--r--   0        0        0      233 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/core.py
+-rw-r--r--   0        0        0       36 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/exceptions.py
+-rw-r--r--   0        0        0      123 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/jpaddress/__init__.py
+-rw-r--r--   0        0        0     6525 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/jpaddress/core.py
+-rw-r--r--   0        0        0      150 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/jpaddress/exceptions.py
+-rw-r--r--   0        0        0       51 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/jpdatetime/__init__.py
+-rw-r--r--   0        0        0     1832 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/jpdatetime/core.py
+-rw-r--r--   0        0        0      303 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/jptext/__init__.py
+-rw-r--r--   0        0        0      422 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/jptext/cli.py
+-rw-r--r--   0        0        0     6389 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/jptext/core.py
+-rw-r--r--   0        0        0      146 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/jptext/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:44:22.368995 jittok-0.0.6/jittok/py.typed
+-rw-r--r--   0        0        0     1003 2023-06-07 14:26:06.210881 jittok-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 jittok-0.0.6/PKG-INFO
```

### Comparing `jittok-0.0.5/LICENSE` & `jittok-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jittok-0.0.5/PKG-INFO` & `jittok-0.0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: jittok
-Version: 0.0.5
-Summary: Swiss Army Knife-like toolbox for data processing
-Home-page: https://github.com/osoken/jittok
-Author: osoken
-Author-email: osoken.devel@outlook.jp
-License: MIT
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # jittok
 
 `jittok` is a Swiss Army Knife-like toolbox for data processing.
 
 ## Installation
 
 ```
```

### Comparing `jittok-0.0.5/jittok/jpaddress/core.py` & `jittok-0.0.6/jittok/jpaddress/core.py`

 * *Files identical despite different names*

### Comparing `jittok-0.0.5/jittok/jpdatetime/core.py` & `jittok-0.0.6/jittok/jpdatetime/core.py`

 * *Files identical despite different names*

### Comparing `jittok-0.0.5/jittok/jptext/core.py` & `jittok-0.0.6/jittok/jptext/core.py`

 * *Files identical despite different names*

