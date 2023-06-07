# Comparing `tmp/ICICONSOLE-0.0.6.tar.gz` & `tmp/ICICONSOLE-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-0.0.6.tar", last modified: Wed Jun  7 01:43:22 2023, max compression
+gzip compressed data, was "ICICONSOLE-0.0.7.tar", last modified: Wed Jun  7 02:03:08 2023, max compression
```

## Comparing `ICICONSOLE-0.0.6.tar` & `ICICONSOLE-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 01:43:22.452309 ICICONSOLE-0.0.6/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 01:43:22.451085 ICICONSOLE-0.0.6/ICICONSOLE/
--rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.6/ICICONSOLE/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.6/ICICONSOLE/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)     9136 2023-06-07 01:40:19.000000 ICICONSOLE-0.0.6/ICICONSOLE/__main__.py
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 01:43:22.451964 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43040 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      318 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       28 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-06-07 01:43:22.000000 ICICONSOLE-0.0.6/ICICONSOLE.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.6/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)    43040 2023-06-07 01:43:22.452168 ICICONSOLE-0.0.6/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1808 2023-04-27 22:52:49.000000 ICICONSOLE-0.0.6/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1009 2023-06-07 01:42:58.000000 ICICONSOLE-0.0.6/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-07 01:43:22.452343 ICICONSOLE-0.0.6/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 02:03:08.858268 ICICONSOLE-0.0.7/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 02:03:08.856926 ICICONSOLE-0.0.7/ICICONSOLE/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.7/ICICONSOLE/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.7/ICICONSOLE/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     9214 2023-06-07 01:47:33.000000 ICICONSOLE-0.0.7/ICICONSOLE/__main__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      330 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.7/ICICONSOLE/helpCypher.json
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-07 02:03:08.857869 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      357 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       28 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-06-07 02:03:08.000000 ICICONSOLE-0.0.7/ICICONSOLE.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.7/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-06-07 02:00:37.000000 ICICONSOLE-0.0.7/MANIFEST.in
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43067 2023-06-07 02:03:08.858121 ICICONSOLE-0.0.7/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1843 2023-06-07 01:45:53.000000 ICICONSOLE-0.0.7/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1001 2023-06-07 02:00:45.000000 ICICONSOLE-0.0.7/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-07 02:03:08.858304 ICICONSOLE-0.0.7/setup.cfg
```

### Comparing `ICICONSOLE-0.0.6/ICICONSOLE/BasicCypherCommands.py` & `ICICONSOLE-0.0.7/ICICONSOLE/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.6/ICICONSOLE/__main__.py` & `ICICONSOLE-0.0.7/ICICONSOLE/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,16 +103,19 @@
                 executeCypher = False
             # The command to clear the screen. Has a recursive call to itself so that the user is once again prompted, and the instruction message is still shown.
             case "clear":
                 os.system('cls' if os.name == 'nt' else 'clear')
                 console(graph, pod_id)
                 executeCypher = False
             case "help":
-                helpCypher()
-                executeCypher = False
+                try:
+                    helpCypher()
+                    executeCypher = False
+                except:
+                    pass
             case "all":
                 query = bcc.getAll()
             case "allNames":
                 query = bcc.getAllNames()
             case "oneByName":
                 query = bcc.getOneByName()
             case "allProperty":
```

### Comparing `ICICONSOLE-0.0.6/ICICONSOLE.egg-info/PKG-INFO` & `ICICONSOLE-0.0.7/ICICONSOLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.6
-Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods.
+Version: 0.0.7
+Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -700,14 +700,18 @@
 
 Requires Python 3.10 or higher. You can clone this repository and manually install the requirements, or you can directly install the application from PyPi.
 
 ```shell 
 pip install ICICONSOLE
 ```
 
+```shell
+python -m ICICONSOLE
+```
+
 **OR**
 
 ```shell 
 git clone https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients.git
 ```
 
 ```shell
```

### Comparing `ICICONSOLE-0.0.6/LICENSE` & `ICICONSOLE-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.6/PKG-INFO` & `ICICONSOLE-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.6
-Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods.
+Version: 0.0.7
+Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -700,14 +700,18 @@
 
 Requires Python 3.10 or higher. You can clone this repository and manually install the requirements, or you can directly install the application from PyPi.
 
 ```shell 
 pip install ICICONSOLE
 ```
 
+```shell
+python -m ICICONSOLE
+```
+
 **OR**
 
 ```shell 
 git clone https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients.git
 ```
 
 ```shell
```

### Comparing `ICICONSOLE-0.0.6/README.md` & `ICICONSOLE-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 
 Requires Python 3.10 or higher. You can clone this repository and manually install the requirements, or you can directly install the application from PyPi.
 
 ```shell 
 pip install ICICONSOLE
 ```
 
+```shell
+python -m ICICONSOLE
+```
+
 **OR**
 
 ```shell 
 git clone https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients.git
 ```
 
 ```shell
```

### Comparing `ICICONSOLE-0.0.6/pyproject.toml` & `ICICONSOLE-0.0.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLE"
-version = "0.0.6"
-description = "Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods."
+version = "0.0.7"
+description = "Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["Tapis", "CLI", "Agave", "HPC", "Tapis Pods", "TACC", "Neo4j"]
 dependencies = [
     "tapipy",
     "py2neo",
     "pandas"
 ]
+
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
 Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/ICICONSOLE"
 
 [project.entry-points."ICICONSOLE.__main__"]
-tomatoes = "ICICONSOLE:__main__"
+tomatoes = "ICICONSOLE:__main__"
```

