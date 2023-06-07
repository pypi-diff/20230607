# Comparing `tmp/replicator-cli-0.0.6.tar.gz` & `tmp/replicator-cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicator-cli-0.0.6.tar", last modified: Wed Jun  7 19:20:55 2023, max compression
+gzip compressed data, was "replicator-cli-0.0.7.tar", last modified: Wed Jun  7 19:24:45 2023, max compression
```

## Comparing `replicator-cli-0.0.6.tar` & `replicator-cli-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-06-07 19:20:55.914887 replicator-cli-0.0.6/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     1091 2023-06-07 16:04:30.000000 replicator-cli-0.0.6/LICENSE
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2398 2023-06-07 19:20:55.914887 replicator-cli-0.0.6/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2005 2023-06-07 16:04:30.000000 replicator-cli-0.0.6/README.md
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       17 2023-06-07 16:09:14.000000 replicator-cli-0.0.6/meta.py
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      969 2023-06-07 18:23:00.000000 replicator-cli-0.0.6/notifier.py
--rwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)     3666 2023-06-07 19:17:09.000000 replicator-cli-0.0.6/replicator.py
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-06-07 19:20:55.914887 replicator-cli-0.0.6/replicator_cli.egg-info/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2398 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      290 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       39 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/entry_points.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/requires.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       25 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/top_level.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-06-07 19:20:55.914887 replicator-cli-0.0.6/setup.cfg
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      981 2023-06-07 16:06:48.000000 replicator-cli-0.0.6/setup.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-06-07 19:24:45.973139 replicator-cli-0.0.7/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     1091 2023-06-07 16:04:30.000000 replicator-cli-0.0.7/LICENSE
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2398 2023-06-07 19:24:45.973139 replicator-cli-0.0.7/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2005 2023-06-07 16:04:30.000000 replicator-cli-0.0.7/README.md
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       17 2023-06-07 19:24:31.000000 replicator-cli-0.0.7/meta.py
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      969 2023-06-07 19:23:44.000000 replicator-cli-0.0.7/notifier.py
+-rwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)     3666 2023-06-07 19:23:44.000000 replicator-cli-0.0.7/replicator.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-06-07 19:24:45.973139 replicator-cli-0.0.7/replicator_cli.egg-info/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2398 2023-06-07 19:24:45.000000 replicator-cli-0.0.7/replicator_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      290 2023-06-07 19:24:45.000000 replicator-cli-0.0.7/replicator_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-06-07 19:24:45.000000 replicator-cli-0.0.7/replicator_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       46 2023-06-07 19:24:45.000000 replicator-cli-0.0.7/replicator_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-06-07 19:24:45.000000 replicator-cli-0.0.7/replicator_cli.egg-info/requires.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       25 2023-06-07 19:24:45.000000 replicator-cli-0.0.7/replicator_cli.egg-info/top_level.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-06-07 19:24:45.973139 replicator-cli-0.0.7/setup.cfg
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      988 2023-06-07 19:24:01.000000 replicator-cli-0.0.7/setup.py
```

### Comparing `replicator-cli-0.0.6/LICENSE` & `replicator-cli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `replicator-cli-0.0.6/PKG-INFO` & `replicator-cli-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicator-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: Task runner for backups
 Home-page: https://github.com/vitonsky/replicator
 Author: Robert Vitonsky
 Author-email: rob@vitonsky.net
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `replicator-cli-0.0.6/README.md` & `replicator-cli-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `replicator-cli-0.0.6/notifier.py` & `replicator-cli-0.0.7/notifier.py`

 * *Files identical despite different names*

### Comparing `replicator-cli-0.0.6/replicator.py` & `replicator-cli-0.0.7/replicator.py`

 * *Files identical despite different names*

### Comparing `replicator-cli-0.0.6/replicator_cli.egg-info/PKG-INFO` & `replicator-cli-0.0.7/replicator_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicator-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: Task runner for backups
 Home-page: https://github.com/vitonsky/replicator
 Author: Robert Vitonsky
 Author-email: rob@vitonsky.net
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `replicator-cli-0.0.6/setup.py` & `replicator-cli-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     python_requires='>=3.7',
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
     entry_points = '''
         [console_scripts]
-        replicator=app:cli
+        replicator=replicator:cli
     '''
 )
```

