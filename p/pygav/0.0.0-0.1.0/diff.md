# Comparing `tmp/pygav-0.0.0.tar.gz` & `tmp/pygav-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygav-0.0.0.tar", last modified: Sat Jun  4 22:48:08 2022, max compression
+gzip compressed data, was "pygav-0.1.0.tar", last modified: Wed Jun  7 16:17:28 2023, max compression
```

## Comparing `pygav-0.0.0.tar` & `pygav-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2022-06-04 22:48:08.270329 pygav-0.0.0/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      483 2022-06-04 21:24:31.000000 pygav-0.0.0/LICENSE
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1032 2022-06-04 22:48:08.270329 pygav-0.0.0/PKG-INFO
--rw-rw-r--   0 ngav      (1000) ngav      (1000)       31 2022-06-04 21:29:35.000000 pygav-0.0.0/README.md
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      704 2022-06-04 22:47:28.000000 pygav-0.0.0/pyproject.toml
--rw-rw-r--   0 ngav      (1000) ngav      (1000)       38 2022-06-04 22:48:08.270329 pygav-0.0.0/setup.cfg
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2022-06-04 22:48:08.266329 pygav-0.0.0/src/
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2022-06-04 22:48:08.270329 pygav-0.0.0/src/pygav/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)        0 2022-06-04 19:41:44.000000 pygav-0.0.0/src/pygav/__init__.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      167 2022-06-04 20:48:32.000000 pygav-0.0.0/src/pygav/utils.py
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2022-06-04 22:48:08.270329 pygav-0.0.0/src/pygav.egg-info/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1032 2022-06-04 22:48:07.000000 pygav-0.0.0/src/pygav.egg-info/PKG-INFO
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      237 2022-06-04 22:48:08.000000 pygav-0.0.0/src/pygav.egg-info/SOURCES.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)        1 2022-06-04 22:48:08.000000 pygav-0.0.0/src/pygav.egg-info/dependency_links.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)       25 2022-06-04 22:48:08.000000 pygav-0.0.0/src/pygav.egg-info/requires.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)        6 2022-06-04 22:48:08.000000 pygav-0.0.0/src/pygav.egg-info/top_level.txt
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-07 16:17:28.645563 pygav-0.1.0/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      483 2022-06-04 21:24:31.000000 pygav-0.1.0/LICENSE
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1437 2023-06-07 16:17:28.641563 pygav-0.1.0/PKG-INFO
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      437 2023-06-07 10:34:10.000000 pygav-0.1.0/README.md
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-07 16:17:28.641563 pygav-0.1.0/pygav/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)        0 2022-06-04 19:41:44.000000 pygav-0.1.0/pygav/__init__.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1406 2023-06-07 16:15:36.000000 pygav-0.1.0/pygav/data.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      715 2023-06-07 10:49:39.000000 pygav-0.1.0/pygav/utils.py
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-07 16:17:28.641563 pygav-0.1.0/pygav.egg-info/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1437 2023-06-07 16:17:28.000000 pygav-0.1.0/pygav.egg-info/PKG-INFO
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      243 2023-06-07 16:17:28.000000 pygav-0.1.0/pygav.egg-info/SOURCES.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)        1 2023-06-07 16:17:28.000000 pygav-0.1.0/pygav.egg-info/dependency_links.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)       82 2023-06-07 16:17:28.000000 pygav-0.1.0/pygav.egg-info/requires.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)        6 2023-06-07 16:17:28.000000 pygav-0.1.0/pygav.egg-info/top_level.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      788 2023-06-07 16:16:18.000000 pygav-0.1.0/pyproject.toml
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)       38 2023-06-07 16:17:28.645563 pygav-0.1.0/setup.cfg
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-07 16:17:28.641563 pygav-0.1.0/tests/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      258 2023-06-07 10:51:03.000000 pygav-0.1.0/tests/test_utils.py
```

### Comparing `pygav-0.0.0/pyproject.toml` & `pygav-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygav"
-version = "0.0.0"
+version = "0.1.0"
 description = "Useful stuff"
 readme = "README.md"
 authors = [{ name = "Nikos Gavalas", email = "ngavalas@protonmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
 ]
 keywords = ["utilities"]
-dependencies = []
+dependencies = [
+  "pandas >= 2.0.2, < 3",
+  "matplotlib >= 3.7.1, < 4",
+  "seaborn >= 0.12.2, < 1"
+]
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = ["pytest", "pytest-cov"]
 
 [project.urls]
 Homepage = "https://github.com/nikosgavalas/pygav"
```

