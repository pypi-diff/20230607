# Comparing `tmp/jintonic-0.2.5.tar.gz` & `tmp/jintonic-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jintonic-0.2.5.tar", last modified: Wed Jun  7 20:07:38 2023, max compression
+gzip compressed data, was "jintonic-0.2.6.tar", last modified: Wed Jun  7 20:09:43 2023, max compression
```

## Comparing `jintonic-0.2.5.tar` & `jintonic-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:38.937713 jintonic-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-07 20:07:07.000000 jintonic-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-07 20:07:38.937713 jintonic-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-07 20:07:07.000000 jintonic-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 20:07:07.000000 jintonic-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:07.000000 jintonic-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:07:38.937713 jintonic-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:38.933713 jintonic-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:38.933713 jintonic-0.2.5/src/jintonic/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-07 20:07:07.000000 jintonic-0.2.5/src/jintonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 20:07:07.000000 jintonic-0.2.5/src/jintonic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-07 20:07:07.000000 jintonic-0.2.5/src/jintonic/chords.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-07 20:07:07.000000 jintonic-0.2.5/src/jintonic/harmonics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-06-07 20:07:07.000000 jintonic-0.2.5/src/jintonic/intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-06-07 20:07:07.000000 jintonic-0.2.5/src/jintonic/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-07 20:07:07.000000 jintonic-0.2.5/src/jintonic/primes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15260 2023-06-07 20:07:07.000000 jintonic-0.2.5/src/jintonic/scales.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:38.937713 jintonic-0.2.5/src/jintonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-07 20:07:38.000000 jintonic-0.2.5/src/jintonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 20:07:38.000000 jintonic-0.2.5/src/jintonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:07:38.000000 jintonic-0.2.5/src/jintonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 20:07:38.000000 jintonic-0.2.5/src/jintonic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 20:07:38.000000 jintonic-0.2.5/src/jintonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:09:43.451309 jintonic-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-07 20:08:57.000000 jintonic-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-07 20:09:43.447309 jintonic-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-07 20:08:57.000000 jintonic-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 20:08:57.000000 jintonic-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:08:57.000000 jintonic-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:09:43.451309 jintonic-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:09:43.447309 jintonic-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:09:43.447309 jintonic-0.2.6/src/jintonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-07 20:08:57.000000 jintonic-0.2.6/src/jintonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 20:08:57.000000 jintonic-0.2.6/src/jintonic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-07 20:08:57.000000 jintonic-0.2.6/src/jintonic/chords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-07 20:08:57.000000 jintonic-0.2.6/src/jintonic/harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-06-07 20:08:57.000000 jintonic-0.2.6/src/jintonic/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-06-07 20:08:57.000000 jintonic-0.2.6/src/jintonic/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-07 20:08:57.000000 jintonic-0.2.6/src/jintonic/primes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15260 2023-06-07 20:08:57.000000 jintonic-0.2.6/src/jintonic/scales.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:09:43.447309 jintonic-0.2.6/src/jintonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-07 20:09:43.000000 jintonic-0.2.6/src/jintonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 20:09:43.000000 jintonic-0.2.6/src/jintonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:09:43.000000 jintonic-0.2.6/src/jintonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 20:09:43.000000 jintonic-0.2.6/src/jintonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 20:09:43.000000 jintonic-0.2.6/src/jintonic.egg-info/top_level.txt
```

### Comparing `jintonic-0.2.5/LICENSE` & `jintonic-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.5/PKG-INFO` & `jintonic-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jintonic
-Version: 0.2.5
+Version: 0.2.6
 Summary: Utilities for computer assisted composition in just intonation
 Author: Ismail Negm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `jintonic-0.2.5/README.md` & `jintonic-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.5/pyproject.toml` & `jintonic-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.5/src/jintonic/chords.py` & `jintonic-0.2.6/src/jintonic/chords.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.5/src/jintonic/harmonics.py` & `jintonic-0.2.6/src/jintonic/harmonics.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.5/src/jintonic/intervals.py` & `jintonic-0.2.6/src/jintonic/intervals.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.5/src/jintonic/lattice.py` & `jintonic-0.2.6/src/jintonic/lattice.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.5/src/jintonic/primes.py` & `jintonic-0.2.6/src/jintonic/primes.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.5/src/jintonic/scales.py` & `jintonic-0.2.6/src/jintonic/scales.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.5/src/jintonic.egg-info/PKG-INFO` & `jintonic-0.2.6/src/jintonic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jintonic
-Version: 0.2.5
+Version: 0.2.6
 Summary: Utilities for computer assisted composition in just intonation
 Author: Ismail Negm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

