# Comparing `tmp/actipy-2.0.3.post2.tar.gz` & `tmp/actipy-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actipy-2.0.3.post2.tar", last modified: Wed Apr 19 19:21:20 2023, max compression
+gzip compressed data, was "actipy-2.0.4.tar", last modified: Wed Jun  7 13:58:04 2023, max compression
```

## Comparing `actipy-2.0.3.post2.tar` & `actipy-2.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:20.644297 actipy-2.0.3.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-19 19:21:20.644297 actipy-2.0.3.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:21:20.644297 actipy-2.0.3.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:20.644297 actipy-2.0.3.post2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:20.644297 actipy-2.0.3.post2/src/actipy/
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-19 19:21:10.000000 actipy-2.0.3.post2/src/actipy/ActigraphReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/src/actipy/ActigraphReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-19 19:21:10.000000 actipy-2.0.3.post2/src/actipy/AxivityReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/src/actipy/AxivityReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-19 19:21:10.000000 actipy-2.0.3.post2/src/actipy/GENEActivReader.class
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/src/actipy/GENEActivReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-19 19:21:10.000000 actipy-2.0.3.post2/src/actipy/NpyWriter.class
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/src/actipy/NpyWriter.java
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/src/actipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 19:21:20.644297 actipy-2.0.3.post2/src/actipy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/src/actipy/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/src/actipy/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:20.644297 actipy-2.0.3.post2/src/actipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-19 19:21:20.000000 actipy-2.0.3.post2/src/actipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-19 19:21:20.000000 actipy-2.0.3.post2/src/actipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:21:20.000000 actipy-2.0.3.post2/src/actipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-19 19:21:20.000000 actipy-2.0.3.post2/src/actipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 19:21:20.000000 actipy-2.0.3.post2/src/actipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-19 19:21:05.000000 actipy-2.0.3.post2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:04.769765 actipy-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-07 13:57:51.000000 actipy-2.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-07 13:57:51.000000 actipy-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-07 13:58:04.769765 actipy-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-07 13:57:51.000000 actipy-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-07 13:57:51.000000 actipy-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:58:04.769765 actipy-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-07 13:57:51.000000 actipy-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:04.765765 actipy-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:04.769765 actipy-2.0.4/src/actipy/
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-07 13:57:55.000000 actipy-2.0.4/src/actipy/ActigraphReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/ActigraphReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-07 13:57:55.000000 actipy-2.0.4/src/actipy/AxivityReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/AxivityReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-07 13:57:55.000000 actipy-2.0.4/src/actipy/GENEActivReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/GENEActivReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-07 13:57:55.000000 actipy-2.0.4/src/actipy/NpyWriter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/NpyWriter.java
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-07 13:58:04.769765 actipy-2.0.4/src/actipy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-07 13:57:51.000000 actipy-2.0.4/src/actipy/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:04.769765 actipy-2.0.4/src/actipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-07 13:58:04.000000 actipy-2.0.4/src/actipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-07 13:58:04.000000 actipy-2.0.4/src/actipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:58:04.000000 actipy-2.0.4/src/actipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-07 13:58:04.000000 actipy-2.0.4/src/actipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 13:58:04.000000 actipy-2.0.4/src/actipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-07 13:57:51.000000 actipy-2.0.4/versioneer.py
```

### Comparing `actipy-2.0.3.post2/LICENSE.md` & `actipy-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/PKG-INFO` & `actipy-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actipy
-Version: 2.0.3.post2
+Version: 2.0.4
 Summary: Python package to process wearable accelerometer data
 Home-page: https://github.com/OxWearables/actipy
 Download-URL: https://github.com/OxWearables/actipy
 Author: Shing Chan, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
```

### Comparing `actipy-2.0.3.post2/README.md` & `actipy-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/pyproject.toml` & `actipy-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/setup.py` & `actipy-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         "dev": [
             "flake8",
             "autopep8",
             "ipython",
             "ipdb",
             "memory-profiler",
             "twine",
+            "tomli",
         ],
         "docs": [
             "sphinx>=4.2",
             "sphinx_rtd_theme>=1.0",
             "readthedocs-sphinx-search>=0.1",
             "docutils<0.18",
         ]
```

### Comparing `actipy-2.0.3.post2/src/actipy/ActigraphReader.class` & `actipy-2.0.4/src/actipy/ActigraphReader.class`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/src/actipy/ActigraphReader.java` & `actipy-2.0.4/src/actipy/ActigraphReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/src/actipy/AxivityReader.class` & `actipy-2.0.4/src/actipy/AxivityReader.class`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/src/actipy/AxivityReader.java` & `actipy-2.0.4/src/actipy/AxivityReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/src/actipy/GENEActivReader.class` & `actipy-2.0.4/src/actipy/GENEActivReader.class`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/src/actipy/GENEActivReader.java` & `actipy-2.0.4/src/actipy/GENEActivReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/src/actipy/NpyWriter.class` & `actipy-2.0.4/src/actipy/NpyWriter.class`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/src/actipy/NpyWriter.java` & `actipy-2.0.4/src/actipy/NpyWriter.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/src/actipy/processing.py` & `actipy-2.0.4/src/actipy/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,11 +413,11 @@
 
 
 def npy2df(data):
     """ Convert a numpy structured array to pandas dataframe. Also parse time
     and set as index. This function will avoid copies whenever possible. """
 
     t = pd.to_datetime(data['time'], unit='ms')
-    columns = [c for c in ['x', 'y', 'z', 'T'] if c in data.dtype.names]
+    columns = [c for c in ['x', 'y', 'z', 'temperature'] if c in data.dtype.names]
     data = pd.DataFrame({c: data[c] for c in columns}, index=t, copy=False)
 
     return data
```

### Comparing `actipy-2.0.3.post2/src/actipy/reader.py` & `actipy-2.0.4/src/actipy/reader.py`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/src/actipy.egg-info/PKG-INFO` & `actipy-2.0.4/src/actipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actipy
-Version: 2.0.3.post2
+Version: 2.0.4
 Summary: Python package to process wearable accelerometer data
 Home-page: https://github.com/OxWearables/actipy
 Download-URL: https://github.com/OxWearables/actipy
 Author: Shing Chan, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
```

### Comparing `actipy-2.0.3.post2/src/actipy.egg-info/SOURCES.txt` & `actipy-2.0.4/src/actipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post2/versioneer.py` & `actipy-2.0.4/versioneer.py`

 * *Files identical despite different names*

