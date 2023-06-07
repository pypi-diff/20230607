# Comparing `tmp/clocky-0.0.6.tar.gz` & `tmp/clocky-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clocky-0.0.6.tar", last modified: Sun Apr  2 00:27:14 2023, max compression
+gzip compressed data, was "clocky-0.0.7.tar", last modified: Wed Jun  7 03:57:49 2023, max compression
```

## Comparing `clocky-0.0.6.tar` & `clocky-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 00:27:14.595583 clocky-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-02 00:26:59.000000 clocky-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-02 00:27:14.595583 clocky-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-02 00:26:59.000000 clocky-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 00:27:14.595583 clocky-0.0.6/clocky/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-02 00:26:59.000000 clocky-0.0.6/clocky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-04-02 00:26:59.000000 clocky-0.0.6/clocky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-02 00:26:59.000000 clocky-0.0.6/clocky/test_clocky.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 00:27:14.595583 clocky-0.0.6/clocky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-02 00:27:14.000000 clocky-0.0.6/clocky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-02 00:27:14.000000 clocky-0.0.6/clocky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 00:27:14.000000 clocky-0.0.6/clocky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-02 00:27:14.000000 clocky-0.0.6/clocky.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-02 00:27:14.000000 clocky-0.0.6/clocky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-02 00:27:14.000000 clocky-0.0.6/clocky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 00:27:14.595583 clocky-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-02 00:26:59.000000 clocky-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:57:49.269091 clocky-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-07 03:57:35.000000 clocky-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-07 03:57:49.269091 clocky-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-07 03:57:35.000000 clocky-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:57:49.269091 clocky-0.0.7/clocky/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 03:57:35.000000 clocky-0.0.7/clocky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-06-07 03:57:35.000000 clocky-0.0.7/clocky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-07 03:57:35.000000 clocky-0.0.7/clocky/test_clocky.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:57:49.269091 clocky-0.0.7/clocky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-07 03:57:49.000000 clocky-0.0.7/clocky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-07 03:57:49.000000 clocky-0.0.7/clocky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:57:49.000000 clocky-0.0.7/clocky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 03:57:49.000000 clocky-0.0.7/clocky.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 03:57:49.000000 clocky-0.0.7/clocky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 03:57:49.000000 clocky-0.0.7/clocky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 03:57:49.269091 clocky-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-07 03:57:35.000000 clocky-0.0.7/setup.py
```

### Comparing `clocky-0.0.6/LICENSE.txt` & `clocky-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clocky-0.0.6/PKG-INFO` & `clocky-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clocky
-Version: 0.0.6
+Version: 0.0.7
 Home-page: http://github.com/csm10495/clocky
 Author: csm10495
 Author-email: csm10495@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
```

### Comparing `clocky-0.0.6/README.md` & `clocky-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `clocky-0.0.6/clocky/__main__.py` & `clocky-0.0.7/clocky/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,19 +174,22 @@
                     except (psutil.NoSuchProcess, psutil.AccessDenied):
                         # process died... thats ok.
                         break
 
                     # reset counter time
                     next_counters_time = time.time() + counter_time_sec
 
-                time.sleep(0.001)
+                # Done to allow a moment of yield
+                time.sleep(.00001)
 
             death_time = time.time()
             exit_code = proc.wait()
-            run_time = death_time - proc.create_time()
+
+            # due to (seemingly) rounding a really fast process could lead to a negative runtime.
+            run_time = max(0, death_time - proc.create_time())
         else:
             print(f"{cmd[0]}: command not found", file=output)
 
             # 127 == command not found
             exit_code = 127
 
     if not quiet and gnu_mode and exit_code != 0:
```

### Comparing `clocky-0.0.6/clocky/test_clocky.py` & `clocky-0.0.7/clocky/test_clocky.py`

 * *Files identical despite different names*

### Comparing `clocky-0.0.6/clocky.egg-info/PKG-INFO` & `clocky-0.0.7/clocky.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clocky
-Version: 0.0.6
+Version: 0.0.7
 Home-page: http://github.com/csm10495/clocky
 Author: csm10495
 Author-email: csm10495@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
```

### Comparing `clocky-0.0.6/setup.py` & `clocky-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import pathlib
 import sys
 
 from setuptools import setup
 
-THIS_FOLDER = pathlib.Path(__file__).parent
-MODULE_FOLDER = THIS_FOLDER / THIS_FOLDER.name
-
-sys.path.append(str(MODULE_FOLDER))
+THIS_FOLDER = pathlib.Path(__file__).parent.resolve()
+MODULE_FOLDER = (THIS_FOLDER / THIS_FOLDER.name).resolve()
 
+sys.path.insert(0, str(MODULE_FOLDER))
 from __init__ import __version__
 
+sys.path.remove(str(MODULE_FOLDER))
+
+
 req = ["psutil"]
 
 setup(
     name="clocky",
     author="csm10495",
     author_email="csm10495@gmail.com",
     url="http://github.com/csm10495/clocky",
```

