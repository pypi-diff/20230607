# Comparing `tmp/google-civic-information-api-0.1.1.tar.gz` & `tmp/google-civic-information-api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-civic-information-api-0.1.1.tar", last modified: Tue Jun  6 15:39:05 2023, max compression
+gzip compressed data, was "google-civic-information-api-1.0.0.tar", last modified: Wed Jun  7 12:54:00 2023, max compression
```

## Comparing `google-civic-information-api-0.1.1.tar` & `google-civic-information-api-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:39:05.550370 google-civic-information-api-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/src/google_civic_information_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/src/google_civic_information_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/src/google_civic_information_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/src/google_civic_information_api/divisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/src/google_civic_information_api/elections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/src/google_civic_information_api/representatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-06 15:39:05.000000 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-06 15:39:05.000000 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:39:05.000000 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 15:39:05.000000 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 15:39:05.000000 google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:39:05.554370 google-civic-information-api-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/tests/test_divisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/tests/test_elections.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-06 15:38:56.000000 google-civic-information-api-0.1.1/tests/test_representatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:00.344624 google-civic-information-api-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-07 12:53:49.000000 google-civic-information-api-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-07 12:54:00.344624 google-civic-information-api-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-07 12:53:49.000000 google-civic-information-api-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-07 12:53:49.000000 google-civic-information-api-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:54:00.344624 google-civic-information-api-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:00.340624 google-civic-information-api-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:00.340624 google-civic-information-api-1.0.0/src/google_civic_information_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:49.000000 google-civic-information-api-1.0.0/src/google_civic_information_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-07 12:53:49.000000 google-civic-information-api-1.0.0/src/google_civic_information_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-07 12:53:49.000000 google-civic-information-api-1.0.0/src/google_civic_information_api/divisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-07 12:53:49.000000 google-civic-information-api-1.0.0/src/google_civic_information_api/elections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-07 12:53:49.000000 google-civic-information-api-1.0.0/src/google_civic_information_api/representatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:00.344624 google-civic-information-api-1.0.0/src/google_civic_information_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-07 12:54:00.000000 google-civic-information-api-1.0.0/src/google_civic_information_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-07 12:54:00.000000 google-civic-information-api-1.0.0/src/google_civic_information_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:54:00.000000 google-civic-information-api-1.0.0/src/google_civic_information_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 12:54:00.000000 google-civic-information-api-1.0.0/src/google_civic_information_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 12:54:00.000000 google-civic-information-api-1.0.0/src/google_civic_information_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:00.344624 google-civic-information-api-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-07 12:53:49.000000 google-civic-information-api-1.0.0/tests/test_divisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-07 12:53:49.000000 google-civic-information-api-1.0.0/tests/test_elections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-07 12:53:49.000000 google-civic-information-api-1.0.0/tests/test_representatives.py
```

### Comparing `google-civic-information-api-0.1.1/LICENSE` & `google-civic-information-api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-civic-information-api-0.1.1/pyproject.toml` & `google-civic-information-api-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [build-system]
 requires = ["setuptools>=67.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "google-civic-information-api"
-version = "0.1.1"
+version = "1.0.0"
 description = "A python wrapper for Google's Civic Information API"
 readme = "README.md"
 authors = [{ name = "Matthew Mathur"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
-    "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["civic-information-api"]
 dependencies = [
     "requests >= 2.1.0",
 ]
 requires-python = ">=3.7"
```

### Comparing `google-civic-information-api-0.1.1/src/google_civic_information_api/elections.py` & `google-civic-information-api-1.0.0/src/google_civic_information_api/elections.py`

 * *Files identical despite different names*

### Comparing `google-civic-information-api-0.1.1/src/google_civic_information_api/representatives.py` & `google-civic-information-api-1.0.0/src/google_civic_information_api/representatives.py`

 * *Files identical despite different names*

### Comparing `google-civic-information-api-0.1.1/src/google_civic_information_api.egg-info/SOURCES.txt` & `google-civic-information-api-1.0.0/src/google_civic_information_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-civic-information-api-0.1.1/tests/test_divisions.py` & `google-civic-information-api-1.0.0/tests/test_divisions.py`

 * *Files identical despite different names*

### Comparing `google-civic-information-api-0.1.1/tests/test_elections.py` & `google-civic-information-api-1.0.0/tests/test_elections.py`

 * *Files identical despite different names*

### Comparing `google-civic-information-api-0.1.1/tests/test_representatives.py` & `google-civic-information-api-1.0.0/tests/test_representatives.py`

 * *Files identical despite different names*

