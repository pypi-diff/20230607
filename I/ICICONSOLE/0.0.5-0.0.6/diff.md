# Comparing `tmp/ICICONSOLE-0.0.5.tar.gz` & `tmp/ICICONSOLE-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-0.0.5.tar", last modified: Thu Apr 27 22:53:25 2023, max compression
+gzip compressed data, was "ICICONSOLE-0.0.6.tar", last modified: Wed Jun  7 01:43:22 2023, max compression
```

## Comparing `ICICONSOLE-0.0.5.tar` & `ICICONSOLE-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:53:25.051113 ICICONSOLE-0.0.5/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:53:25.049755 ICICONSOLE-0.0.5/ICICONSOLE/
--rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.5/ICICONSOLE/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.5/ICICONSOLE/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)     9045 2023-04-27 22:38:06.000000 ICICONSOLE-0.0.5/ICICONSOLE/__main__.py
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:53:25.050741 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43040 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      318 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       28 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.5/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43040 2023-04-27 22:53:25.050963 ICICONSOLE-0.0.5/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1808 2023-04-27 22:52:49.000000 ICICONSOLE-0.0.5/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1009 2023-04-27 22:51:50.000000 ICICONSOLE-0.0.5/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-04-27 22:53:25.051151 ICICONSOLE-0.0.5/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 01:43:22.452309 ICICONSOLE-0.0.6/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 01:43:22.451085 ICICONSOLE-0.0.6/ICICONSOLE/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.6/ICICONSOLE/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.6/ICICONSOLE/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     9136 2023-06-07 01:40:19.000000 ICICONSOLE-0.0.6/ICICONSOLE/__main__.py
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 01:43:22.451964 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43040 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      318 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       28 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.6/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43040 2023-06-07 01:43:22.452168 ICICONSOLE-0.0.6/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1808 2023-04-27 22:52:49.000000 ICICONSOLE-0.0.6/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1009 2023-06-07 01:42:58.000000 ICICONSOLE-0.0.6/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-07 01:43:22.452343 ICICONSOLE-0.0.6/setup.cfg
```

### Comparing `ICICONSOLE-0.0.5/ICICONSOLE/BasicCypherCommands.py` & `ICICONSOLE-0.0.6/ICICONSOLE/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.5/ICICONSOLE/__main__.py` & `ICICONSOLE-0.0.6/ICICONSOLE/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from getpass import getpass
 # This is how we actually connect to TAPIS and get the required information to connect to a Pod
 from tapipy.tapis import Tapis
 # These are to clear the screen
 import os
 import signal
 import json
+import pkg_resources
+
 try:
     from . import BasicCypherCommands as bcc
 except:
     import BasicCypherCommands as bcc
 
 # Recording login time
 start = time.time()
@@ -62,16 +64,17 @@
     print("-" * len(message))
 
 # Welcome message, formatted with the heavyFormat function
 heavyFormat("Welcome to ICICONSOLE. Login to get started. ")
 
 # Loads help for cypher commands
 def helpCypher():
+    json_path = pkg_resources.resource_filename(__name__, 'helpCypher.json')
     print("\n")
-    with open('helpCypher.json') as f:
+    with open(json_path) as f:
         help_data = json.load(f)
     for key, value in help_data.items():
         print(key + ' : ' + value + '\n')
 
 # The console function is the actual cypher console that you see after logging in and choosing a pod.
 # The console allows you to type in cypher, and run it on the Neo4j pod you are connected to.
 # The console function needs to parameters: a Neo4j graph object, and a pod id.
```

### Comparing `ICICONSOLE-0.0.5/ICICONSOLE.egg-info/PKG-INFO` & `ICICONSOLE-0.0.6/ICICONSOLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.5
+Version: 0.0.6
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ICICONSOLE-0.0.5/LICENSE` & `ICICONSOLE-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.5/PKG-INFO` & `ICICONSOLE-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.5
+Version: 0.0.6
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ICICONSOLE-0.0.5/README.md` & `ICICONSOLE-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.5/pyproject.toml` & `ICICONSOLE-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLE"
-version = "0.0.5"
+version = "0.0.6"
 description = "Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

