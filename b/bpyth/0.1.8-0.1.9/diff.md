# Comparing `tmp/bpyth-0.1.8.tar.gz` & `tmp/bpyth-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpyth-0.1.8.tar", last modified: Tue Feb 21 21:42:09 2023, max compression
+gzip compressed data, was "bpyth-0.1.9.tar", last modified: Wed Jun  7 13:20:35 2023, max compression
```

## Comparing `bpyth-0.1.8.tar` & `bpyth-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-21 21:42:09.917692 bpyth-0.1.8/
--rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 bpyth-0.1.8/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)     2346 2023-02-21 21:42:09.917692 bpyth-0.1.8/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     1925 2023-02-21 21:41:33.000000 bpyth-0.1.8/README.md
--rw-r--r--   0 me        (1000) me        (1000)     1091 2023-02-21 21:41:08.000000 bpyth-0.1.8/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2023-02-21 21:42:09.917692 bpyth-0.1.8/setup.cfg
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-21 21:42:09.841693 bpyth-0.1.8/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-21 21:42:09.917692 bpyth-0.1.8/src/bpyth/
--rw-r--r--   0 me        (1000) me        (1000)      477 2022-09-11 18:58:57.000000 bpyth-0.1.8/src/bpyth/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      198 2023-02-14 22:56:50.000000 bpyth-0.1.8/src/bpyth/__main__.py
--rw-r--r--   0 me        (1000) me        (1000)     3270 2023-01-09 12:11:37.000000 bpyth-0.1.8/src/bpyth/bpyth_files.py
--rw-r--r--   0 me        (1000) me        (1000)     2054 2022-11-06 09:19:24.000000 bpyth-0.1.8/src/bpyth/bpyth_human.py
--rw-r--r--   0 me        (1000) me        (1000)     5129 2023-02-21 07:48:01.000000 bpyth-0.1.8/src/bpyth/bpyth_iterable.py
--rw-r--r--   0 me        (1000) me        (1000)     5216 2022-11-03 16:15:47.000000 bpyth-0.1.8/src/bpyth/bpyth_object_analysis.py
--rw-r--r--   0 me        (1000) me        (1000)     2106 2022-09-09 18:38:17.000000 bpyth-0.1.8/src/bpyth/bpyth_string.py
--rw-r--r--   0 me        (1000) me        (1000)     1402 2022-11-03 15:46:03.000000 bpyth-0.1.8/src/bpyth/bpyth_tools.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-21 21:42:09.917692 bpyth-0.1.8/src/bpyth.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)     2346 2023-02-21 21:42:09.000000 bpyth-0.1.8/src/bpyth.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)      408 2023-02-21 21:42:09.000000 bpyth-0.1.8/src/bpyth.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2023-02-21 21:42:09.000000 bpyth-0.1.8/src/bpyth.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)       46 2023-02-21 21:42:09.000000 bpyth-0.1.8/src/bpyth.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) me        (1000)        6 2023-02-21 21:42:09.000000 bpyth-0.1.8/src/bpyth.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-07 13:20:35.145099 bpyth-0.1.9/
+-rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 bpyth-0.1.9/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)     2346 2023-06-07 13:20:35.145099 bpyth-0.1.9/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)     1925 2023-06-07 13:19:54.000000 bpyth-0.1.9/README.md
+-rw-r--r--   0 me        (1000) me        (1000)     1091 2023-06-07 13:18:45.000000 bpyth-0.1.9/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-07 13:20:35.145099 bpyth-0.1.9/setup.cfg
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-07 13:20:35.097099 bpyth-0.1.9/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-07 13:20:35.141099 bpyth-0.1.9/src/bpyth/
+-rw-r--r--   0 me        (1000) me        (1000)      477 2022-09-11 18:58:57.000000 bpyth-0.1.9/src/bpyth/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)      198 2023-02-14 22:56:50.000000 bpyth-0.1.9/src/bpyth/__main__.py
+-rw-r--r--   0 me        (1000) me        (1000)     3270 2023-04-11 17:07:26.000000 bpyth-0.1.9/src/bpyth/bpyth_files.py
+-rw-r--r--   0 me        (1000) me        (1000)     2054 2022-11-06 09:19:24.000000 bpyth-0.1.9/src/bpyth/bpyth_human.py
+-rw-r--r--   0 me        (1000) me        (1000)     5210 2023-06-07 13:18:23.000000 bpyth-0.1.9/src/bpyth/bpyth_iterable.py
+-rw-r--r--   0 me        (1000) me        (1000)     5216 2022-11-03 16:15:47.000000 bpyth-0.1.9/src/bpyth/bpyth_object_analysis.py
+-rw-r--r--   0 me        (1000) me        (1000)     2106 2022-09-09 18:38:17.000000 bpyth-0.1.9/src/bpyth/bpyth_string.py
+-rw-r--r--   0 me        (1000) me        (1000)     1402 2022-11-03 15:46:03.000000 bpyth-0.1.9/src/bpyth/bpyth_tools.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-07 13:20:35.145099 bpyth-0.1.9/src/bpyth.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)     2346 2023-06-07 13:20:35.000000 bpyth-0.1.9/src/bpyth.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)      408 2023-06-07 13:20:35.000000 bpyth-0.1.9/src/bpyth.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2023-06-07 13:20:35.000000 bpyth-0.1.9/src/bpyth.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)       46 2023-06-07 13:20:35.000000 bpyth-0.1.9/src/bpyth.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) me        (1000)        6 2023-06-07 13:20:35.000000 bpyth-0.1.9/src/bpyth.egg-info/top_level.txt
```

### Comparing `bpyth-0.1.8/LICENSE` & `bpyth-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bpyth-0.1.8/PKG-INFO` & `bpyth-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpyth
-Version: 0.1.8
+Version: 0.1.9
 Summary: Various Python Tools
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/bpyth
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bpyth-0.1.8/README.md` & `bpyth-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bpyth-0.1.8/pyproject.toml` & `bpyth-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pyproject.toml
 
 
 [project]
 name            = "bpyth"
-version         = "0.1.8"        
+version         = "0.1.9"        
 
 requires-python = ">=3.8"
 dependencies    = []
 
 authors        = [{ name = "djekra", email = "hopsalla@gmail.com" }]
 description     = "Various Python Tools"
 readme          = "README.md"
```

### Comparing `bpyth-0.1.8/src/bpyth/bpyth_files.py` & `bpyth-0.1.9/src/bpyth/bpyth_files.py`

 * *Files identical despite different names*

### Comparing `bpyth-0.1.8/src/bpyth/bpyth_human.py` & `bpyth-0.1.9/src/bpyth/bpyth_human.py`

 * *Files identical despite different names*

### Comparing `bpyth-0.1.8/src/bpyth/bpyth_iterable.py` & `bpyth-0.1.9/src/bpyth/bpyth_iterable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-from collections        import Counter, defaultdict, Iterable
+
+try:
+  from collections import Iterable
+except:
+    from collections.abc import Iterable
+
+from collections        import Counter, defaultdict
 from functools          import lru_cache
```

### Comparing `bpyth-0.1.8/src/bpyth/bpyth_object_analysis.py` & `bpyth-0.1.9/src/bpyth/bpyth_object_analysis.py`

 * *Files identical despite different names*

### Comparing `bpyth-0.1.8/src/bpyth/bpyth_string.py` & `bpyth-0.1.9/src/bpyth/bpyth_string.py`

 * *Files identical despite different names*

### Comparing `bpyth-0.1.8/src/bpyth/bpyth_tools.py` & `bpyth-0.1.9/src/bpyth/bpyth_tools.py`

 * *Files identical despite different names*

### Comparing `bpyth-0.1.8/src/bpyth.egg-info/PKG-INFO` & `bpyth-0.1.9/src/bpyth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpyth
-Version: 0.1.8
+Version: 0.1.9
 Summary: Various Python Tools
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/bpyth
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

