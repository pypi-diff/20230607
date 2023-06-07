# Comparing `tmp/cgsubmit-1.0.2.tar.gz` & `tmp/cgsubmit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgsubmit-1.0.2.tar", last modified: Wed Jun  7 19:51:53 2023, max compression
+gzip compressed data, was "cgsubmit-1.0.3.tar", last modified: Wed Jun  7 19:57:15 2023, max compression
```

## Comparing `cgsubmit-1.0.2.tar` & `cgsubmit-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:51:53.386436 cgsubmit-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-07 19:51:31.000000 cgsubmit-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-07 19:51:53.386436 cgsubmit-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-07 19:51:31.000000 cgsubmit-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:51:53.382436 cgsubmit-1.0.2/cgsubmit/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 19:51:31.000000 cgsubmit-1.0.2/cgsubmit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-07 19:51:31.000000 cgsubmit-1.0.2/cgsubmit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:51:53.382436 cgsubmit-1.0.2/cgsubmit/api/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 19:51:31.000000 cgsubmit-1.0.2/cgsubmit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 19:51:31.000000 cgsubmit-1.0.2/cgsubmit/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:51:53.386436 cgsubmit-1.0.2/cgsubmit/games/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 19:51:31.000000 cgsubmit-1.0.2/cgsubmit/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-07 19:51:31.000000 cgsubmit-1.0.2/cgsubmit/games/games.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:51:53.382436 cgsubmit-1.0.2/cgsubmit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-07 19:51:53.000000 cgsubmit-1.0.2/cgsubmit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-07 19:51:53.000000 cgsubmit-1.0.2/cgsubmit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:51:53.000000 cgsubmit-1.0.2/cgsubmit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 19:51:53.000000 cgsubmit-1.0.2/cgsubmit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 19:51:53.000000 cgsubmit-1.0.2/cgsubmit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-07 19:51:31.000000 cgsubmit-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:51:53.386436 cgsubmit-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-07 19:51:31.000000 cgsubmit-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:57:15.010894 cgsubmit-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-07 19:56:57.000000 cgsubmit-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-07 19:57:15.010894 cgsubmit-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-07 19:56:57.000000 cgsubmit-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:57:15.010894 cgsubmit-1.0.3/cgsubmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 19:56:57.000000 cgsubmit-1.0.3/cgsubmit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-07 19:56:57.000000 cgsubmit-1.0.3/cgsubmit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:57:15.010894 cgsubmit-1.0.3/cgsubmit/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 19:56:57.000000 cgsubmit-1.0.3/cgsubmit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 19:56:57.000000 cgsubmit-1.0.3/cgsubmit/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:57:15.010894 cgsubmit-1.0.3/cgsubmit/games/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 19:56:57.000000 cgsubmit-1.0.3/cgsubmit/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-07 19:56:57.000000 cgsubmit-1.0.3/cgsubmit/games/games.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:57:15.010894 cgsubmit-1.0.3/cgsubmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-07 19:57:14.000000 cgsubmit-1.0.3/cgsubmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-07 19:57:14.000000 cgsubmit-1.0.3/cgsubmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:57:14.000000 cgsubmit-1.0.3/cgsubmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 19:57:14.000000 cgsubmit-1.0.3/cgsubmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 19:57:14.000000 cgsubmit-1.0.3/cgsubmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-07 19:56:57.000000 cgsubmit-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:57:15.010894 cgsubmit-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-07 19:56:57.000000 cgsubmit-1.0.3/setup.py
```

### Comparing `cgsubmit-1.0.2/LICENSE` & `cgsubmit-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.2/PKG-INFO` & `cgsubmit-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.0.2
+Version: 1.0.3
 Summary: Analyse your submit in codingame competitions.
 Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Author: FrequentlyMissedDeadlines
 Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Classifier: Programming Language :: Python :: 3
@@ -33,14 +33,15 @@
 A tool to analyze the results of your submits in codingame competitions and save a lot of time.
 
 It will automatically:
 - retrieve all the games you lost by timeout (code too slow, or runtime error). Fixing these issues should always be your number 1 priority.
 - sort the game you lost by biggest score difference. This way you can easily focus on the games you totally lost as there might be some cases you don't handle properly or you have bugs.
 
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/output.png)
+![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/Codingame.png)
 
 ## Installation
 ```
 pip install cgsubmit
 ```
 
 ## Usage
```

### Comparing `cgsubmit-1.0.2/README.md` & `cgsubmit-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 A tool to analyze the results of your submits in codingame competitions and save a lot of time.
 
 It will automatically:
 - retrieve all the games you lost by timeout (code too slow, or runtime error). Fixing these issues should always be your number 1 priority.
 - sort the game you lost by biggest score difference. This way you can easily focus on the games you totally lost as there might be some cases you don't handle properly or you have bugs.
 
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/output.png)
+![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/Codingame.png)
 
 ## Installation
 ```
 pip install cgsubmit
 ```
 
 ## Usage
```

### Comparing `cgsubmit-1.0.2/cgsubmit/__main__.py` & `cgsubmit-1.0.3/cgsubmit/__main__.py`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.2/cgsubmit/api/api.py` & `cgsubmit-1.0.3/cgsubmit/api/api.py`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.2/cgsubmit/games/games.py` & `cgsubmit-1.0.3/cgsubmit/games/games.py`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.2/cgsubmit.egg-info/PKG-INFO` & `cgsubmit-1.0.3/cgsubmit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.0.2
+Version: 1.0.3
 Summary: Analyse your submit in codingame competitions.
 Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Author: FrequentlyMissedDeadlines
 Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Classifier: Programming Language :: Python :: 3
@@ -33,14 +33,15 @@
 A tool to analyze the results of your submits in codingame competitions and save a lot of time.
 
 It will automatically:
 - retrieve all the games you lost by timeout (code too slow, or runtime error). Fixing these issues should always be your number 1 priority.
 - sort the game you lost by biggest score difference. This way you can easily focus on the games you totally lost as there might be some cases you don't handle properly or you have bugs.
 
 ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/output.png)
+![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/Codingame.png)
 
 ## Installation
 ```
 pip install cgsubmit
 ```
 
 ## Usage
```

### Comparing `cgsubmit-1.0.2/setup.py` & `cgsubmit-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 README_MD = open(join(dirname(abspath(__file__)), "README.md")).read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="cgsubmit",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_namespace_packages(include=['cgsubmit', 'cgsubmit.*'], exclude=['*.tests*']),
     description="Analyse your submit in codingame competitions.",
     long_description=README_MD,
     long_description_content_type="text/markdown",
     url="https://github.com/FrequentlyMissedDeadlines/cgsubmit",
     author="FrequentlyMissedDeadlines",
     author_email="FrequentlyMissedDeadlines+cgsubmit@gmail.com",
```

