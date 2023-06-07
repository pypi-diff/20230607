# Comparing `tmp/cgsubmit-1.0.0.tar.gz` & `tmp/cgsubmit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgsubmit-1.0.0.tar", last modified: Tue Jun  6 21:55:39 2023, max compression
+gzip compressed data, was "cgsubmit-1.0.1.tar", last modified: Wed Jun  7 19:39:12 2023, max compression
```

## Comparing `cgsubmit-1.0.0.tar` & `cgsubmit-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:55:39.297069 cgsubmit-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 21:55:22.000000 cgsubmit-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-06 21:55:39.297069 cgsubmit-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-06 21:55:22.000000 cgsubmit-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:55:39.293069 cgsubmit-1.0.0/cgsubmit/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 21:55:22.000000 cgsubmit-1.0.0/cgsubmit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-06 21:55:22.000000 cgsubmit-1.0.0/cgsubmit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:55:39.297069 cgsubmit-1.0.0/cgsubmit/api/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 21:55:22.000000 cgsubmit-1.0.0/cgsubmit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-06 21:55:22.000000 cgsubmit-1.0.0/cgsubmit/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:55:39.297069 cgsubmit-1.0.0/cgsubmit/games/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 21:55:22.000000 cgsubmit-1.0.0/cgsubmit/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-06 21:55:22.000000 cgsubmit-1.0.0/cgsubmit/games/games.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:55:39.297069 cgsubmit-1.0.0/cgsubmit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-06 21:55:39.000000 cgsubmit-1.0.0/cgsubmit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-06 21:55:39.000000 cgsubmit-1.0.0/cgsubmit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:55:39.000000 cgsubmit-1.0.0/cgsubmit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 21:55:39.000000 cgsubmit-1.0.0/cgsubmit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-06 21:55:22.000000 cgsubmit-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 21:55:39.297069 cgsubmit-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-06 21:55:22.000000 cgsubmit-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:12.439548 cgsubmit-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-07 19:38:55.000000 cgsubmit-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-07 19:39:12.439548 cgsubmit-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-07 19:38:55.000000 cgsubmit-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:12.439548 cgsubmit-1.0.1/cgsubmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 19:38:55.000000 cgsubmit-1.0.1/cgsubmit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-07 19:38:55.000000 cgsubmit-1.0.1/cgsubmit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:12.439548 cgsubmit-1.0.1/cgsubmit/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 19:38:55.000000 cgsubmit-1.0.1/cgsubmit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 19:38:55.000000 cgsubmit-1.0.1/cgsubmit/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:12.439548 cgsubmit-1.0.1/cgsubmit/games/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 19:38:55.000000 cgsubmit-1.0.1/cgsubmit/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-07 19:38:55.000000 cgsubmit-1.0.1/cgsubmit/games/games.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:12.439548 cgsubmit-1.0.1/cgsubmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-07 19:39:12.000000 cgsubmit-1.0.1/cgsubmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-07 19:39:12.000000 cgsubmit-1.0.1/cgsubmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:39:12.000000 cgsubmit-1.0.1/cgsubmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 19:39:12.000000 cgsubmit-1.0.1/cgsubmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 19:39:12.000000 cgsubmit-1.0.1/cgsubmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-07 19:38:55.000000 cgsubmit-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:39:12.439548 cgsubmit-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-07 19:38:55.000000 cgsubmit-1.0.1/setup.py
```

### Comparing `cgsubmit-1.0.0/LICENSE` & `cgsubmit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.0/PKG-INFO` & `cgsubmit-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Analyse your submit in codingame competitions.
 Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Author: FrequentlyMissedDeadlines
 Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +28,20 @@
 [![Version](https://img.shields.io/pypi/pyversions/cgsubmit)](https://pypi.org/project/cgsubmit)
 [![codecov](https://codecov.io/gh/FrequentlyMissedDeadlines/cgsubmit/branch/main/graph/badge.svg)](https://codecov.io/github/FrequentlyMissedDeadlines/cgsubmit?branch=main)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/cgsubmit)
 # codingame-submit
 A tool to analyze the results of your submits in codingame competitions and save a lot of time.
 
+It will automatically:
+- retrieve all the games you lost by timeout (code too slow, or runtime error). Fixing these issues should always be your number 1 priority.
+- sort the game you lost by biggest score difference. This way you can easily focus on the games you totally lost as there might be some cases you don't handle properly or you have bugs.
+
+![](Doc/output.png)
+
 ## Installation
 ```
 pip install cgsubmit
 ```
 
 ## Usage
 ### Getting your test session handle
@@ -45,9 +51,9 @@
 1. open the IDE of the game you are playing in your browser (for example [https://www.codingame.com/ide/puzzle/spring-challenge-2023-ants](https://www.codingame.com/ide/puzzle/spring-challenge-2023-ants))
 2. open the Developer Tools (F12)
 3. look for this query and get the `handle` value: ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/handle.png)
 
 ### Run
 
 ```
-python -m cgsubmit your-test-session-handle
+python -m cgsubmit -t your-test-session-handle
 ```
```

### Comparing `cgsubmit-1.0.0/cgsubmit/__main__.py` & `cgsubmit-1.0.1/cgsubmit/__main__.py`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.0/cgsubmit/api/api.py` & `cgsubmit-1.0.1/cgsubmit/api/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import requests
 
 class Api:
     def __init__(self, test_session_handle):
-        self.session = requests.Session()
         self.test_session_handle = test_session_handle
     
     def get_all_battles(self):
-        r = self.session.post('https://www.codingame.com/services/gamesPlayersRanking/findLastBattlesByTestSessionHandle',
+        r = requests.post('https://www.codingame.com/services/gamesPlayersRanking/findLastBattlesByTestSessionHandle',
                           data='[' + self.test_session_handle + ', null]', headers = {'Content-type': 'application/json'})
         
         if r.status_code == 200:
             return r.json()
         else:
             raise Exception('Unable to retrieve last battles: ' + str(r))
     
     def get_lost_games(self, losts):
-        return [self.session.post('https://www.codingame.com/services/gameResultRemoteService/findByGameId', data='[' + str(id) + ', null]', headers = {'Content-type': 'application/json'}).json() for id in losts]
+        return [requests.post('https://www.codingame.com/services/gameResultRemoteService/findByGameId', data='[' + str(id) + ', null]', headers = {'Content-type': 'application/json'}).json() for id in losts]
```

### Comparing `cgsubmit-1.0.0/cgsubmit/games/games.py` & `cgsubmit-1.0.1/cgsubmit/games/games.py`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.0/cgsubmit.egg-info/PKG-INFO` & `cgsubmit-1.0.1/cgsubmit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Analyse your submit in codingame competitions.
 Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Author: FrequentlyMissedDeadlines
 Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +28,20 @@
 [![Version](https://img.shields.io/pypi/pyversions/cgsubmit)](https://pypi.org/project/cgsubmit)
 [![codecov](https://codecov.io/gh/FrequentlyMissedDeadlines/cgsubmit/branch/main/graph/badge.svg)](https://codecov.io/github/FrequentlyMissedDeadlines/cgsubmit?branch=main)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/cgsubmit)
 # codingame-submit
 A tool to analyze the results of your submits in codingame competitions and save a lot of time.
 
+It will automatically:
+- retrieve all the games you lost by timeout (code too slow, or runtime error). Fixing these issues should always be your number 1 priority.
+- sort the game you lost by biggest score difference. This way you can easily focus on the games you totally lost as there might be some cases you don't handle properly or you have bugs.
+
+![](Doc/output.png)
+
 ## Installation
 ```
 pip install cgsubmit
 ```
 
 ## Usage
 ### Getting your test session handle
@@ -45,9 +51,9 @@
 1. open the IDE of the game you are playing in your browser (for example [https://www.codingame.com/ide/puzzle/spring-challenge-2023-ants](https://www.codingame.com/ide/puzzle/spring-challenge-2023-ants))
 2. open the Developer Tools (F12)
 3. look for this query and get the `handle` value: ![](https://raw.githubusercontent.com/FrequentlyMissedDeadlines/cgsubmit/main/Doc/handle.png)
 
 ### Run
 
 ```
-python -m cgsubmit your-test-session-handle
+python -m cgsubmit -t your-test-session-handle
 ```
```

### Comparing `cgsubmit-1.0.0/setup.py` & `cgsubmit-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_namespace_packages
 from os.path import abspath, dirname, join
 
 # Fetches the content from README.md
 # This will be used for the "long_description" field.
 README_MD = open(join(dirname(abspath(__file__)), "README.md")).read()
 
+with open('requirements.txt') as f:
+    required = f.read().splitlines()
+
 setup(
     name="cgsubmit",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_namespace_packages(include=['cgsubmit', 'cgsubmit.*'], exclude=['*.tests*']),
     description="Analyse your submit in codingame competitions.",
     long_description=README_MD,
     long_description_content_type="text/markdown",
     url="https://github.com/FrequentlyMissedDeadlines/cgsubmit",
     author="FrequentlyMissedDeadlines",
     author_email="FrequentlyMissedDeadlines+cgsubmit@gmail.com",
@@ -26,12 +29,13 @@
         "Topic :: Software Development",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11"
     ],
+    install_requires=required,
     project_urls={
         'Bug Reports': 'https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues',
         'Source': 'https://github.com/FrequentlyMissedDeadlines/cgsubmit',
-    },
+    }
 )
```

