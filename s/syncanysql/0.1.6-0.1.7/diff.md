# Comparing `tmp/syncanysql-0.1.6.tar.gz` & `tmp/syncanysql-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.1.6.tar", last modified: Fri Jun  2 10:53:06 2023, max compression
+gzip compressed data, was "syncanysql-0.1.7.tar", last modified: Wed Jun  7 03:06:08 2023, max compression
```

## Comparing `syncanysql-0.1.6.tar` & `syncanysql-0.1.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:06.264278 syncanysql-0.1.6/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.1.6/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4346 2023-06-02 10:53:06.266279 syncanysql-0.1.6/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3019 2023-05-30 02:47:03.000000 syncanysql-0.1.6/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-06-02 10:53:06.276278 syncanysql-0.1.6/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2007 2023-05-31 04:54:20.000000 syncanysql-0.1.6/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:04.549981 syncanysql-0.1.6/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8803 2023-06-02 04:45:20.000000 syncanysql-0.1.6/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:05.242668 syncanysql-0.1.6/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3127 2023-06-02 03:47:10.000000 syncanysql-0.1.6/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11327 2023-06-01 07:50:12.000000 syncanysql-0.1.6/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      722 2023-05-26 03:56:52.000000 syncanysql-0.1.6/syncanysql/calculaters/env_variable_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      406 2023-05-30 02:50:43.000000 syncanysql-0.1.6/syncanysql/calculaters/generate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:05.667392 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      384 2023-05-29 03:23:56.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10475 2023-05-27 08:55:29.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2982 2023-06-01 03:41:52.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/logical_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6764 2023-05-29 05:01:09.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3880 2023-06-02 03:47:10.000000 syncanysql-0.1.6/syncanysql/calculaters/window_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   194908 2023-06-02 06:40:14.000000 syncanysql-0.1.6/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13459 2023-05-27 14:11:29.000000 syncanysql-0.1.6/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      298 2023-06-02 03:32:36.000000 syncanysql-0.1.6/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8503 2023-06-02 04:45:20.000000 syncanysql-0.1.6/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4167 2023-06-02 04:35:38.000000 syncanysql-0.1.6/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.6/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7050 2023-06-02 04:45:20.000000 syncanysql-0.1.6/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:06.212462 syncanysql-0.1.6/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.6/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.6/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1601 2023-06-02 04:37:49.000000 syncanysql-0.1.6/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.6/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4120 2023-06-02 04:35:38.000000 syncanysql-0.1.6/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    23727 2023-06-02 04:45:20.000000 syncanysql-0.1.6/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2886 2023-06-02 04:37:49.000000 syncanysql-0.1.6/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2139 2023-06-02 04:37:49.000000 syncanysql-0.1.6/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1217 2023-06-02 04:37:49.000000 syncanysql-0.1.6/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      754 2023-05-08 04:04:28.000000 syncanysql-0.1.6/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-05-30 01:57:39.000000 syncanysql-0.1.6/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:04.862815 syncanysql-0.1.6/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4346 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1311 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.6/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      395 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-06-02 10:53:03.000000 syncanysql-0.1.6/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:08.292360 syncanysql-0.1.7/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.1.7/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4346 2023-06-07 03:06:08.294380 syncanysql-0.1.7/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3019 2023-05-30 02:47:03.000000 syncanysql-0.1.7/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-06-07 03:06:08.305385 syncanysql-0.1.7/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2007 2023-06-03 11:38:53.000000 syncanysql-0.1.7/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:06.367979 syncanysql-0.1.7/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8803 2023-06-02 04:45:20.000000 syncanysql-0.1.7/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:07.124383 syncanysql-0.1.7/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3127 2023-06-02 03:47:10.000000 syncanysql-0.1.7/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11914 2023-06-05 06:10:11.000000 syncanysql-0.1.7/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      722 2023-05-26 03:56:52.000000 syncanysql-0.1.7/syncanysql/calculaters/env_variable_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      406 2023-05-30 02:50:43.000000 syncanysql-0.1.7/syncanysql/calculaters/generate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-06-05 09:23:36.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:07.639358 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      384 2023-05-29 03:23:56.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11491 2023-06-05 09:30:11.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6174 2023-06-05 06:10:11.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3208 2023-06-05 06:10:11.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/logical_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5153 2023-06-05 06:10:11.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6867 2023-06-05 06:30:27.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4291 2023-06-05 06:10:11.000000 syncanysql-0.1.7/syncanysql/calculaters/window_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   189228 2023-06-06 05:45:39.000000 syncanysql-0.1.7/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13459 2023-05-27 14:11:29.000000 syncanysql-0.1.7/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      298 2023-06-02 03:32:36.000000 syncanysql-0.1.7/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8503 2023-06-02 04:45:20.000000 syncanysql-0.1.7/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4167 2023-06-02 04:35:38.000000 syncanysql-0.1.7/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.7/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7050 2023-06-02 04:45:20.000000 syncanysql-0.1.7/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:08.243361 syncanysql-0.1.7/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.7/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.7/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1601 2023-06-02 04:37:49.000000 syncanysql-0.1.7/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.7/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4120 2023-06-02 04:35:38.000000 syncanysql-0.1.7/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    25444 2023-06-04 04:46:30.000000 syncanysql-0.1.7/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2886 2023-06-02 04:37:49.000000 syncanysql-0.1.7/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2139 2023-06-02 04:37:49.000000 syncanysql-0.1.7/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1217 2023-06-02 04:37:49.000000 syncanysql-0.1.7/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3805 2023-06-05 04:41:14.000000 syncanysql-0.1.7/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-06-03 05:28:09.000000 syncanysql-0.1.7/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:06.723362 syncanysql-0.1.7/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4346 2023-06-07 03:06:04.000000 syncanysql-0.1.7/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1311 2023-06-07 03:06:05.000000 syncanysql-0.1.7/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-06-07 03:06:04.000000 syncanysql-0.1.7/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-06-07 03:06:04.000000 syncanysql-0.1.7/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.7/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      395 2023-06-07 03:06:04.000000 syncanysql-0.1.7/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-06-07 03:06:04.000000 syncanysql-0.1.7/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.1.6/LICENSE` & `syncanysql-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/PKG-INFO` & `syncanysql-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.1.6/README.md` & `syncanysql-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/setup.py` & `syncanysql-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.1.6"
+version = "0.1.7"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -34,15 +34,15 @@
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(exclude=['*tests*']),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
         "sqlglot>=11.5.5,<12",
-        "syncany>=0.2.12",
+        "syncany>=0.2.13",
         'Pygments>=2.14.0',
         'prompt-toolkit>=3.0.36',
         "rich>=9.11.1",
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
         "pymysql": ['PyMySQL>=0.8.1'],
```

### Comparing `syncanysql-0.1.6/syncanysql/__init__.py` & `syncanysql-0.1.7/syncanysql/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/calculaters/__init__.py` & `syncanysql-0.1.7/syncanysql/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/calculaters/aggregate_calculater.py` & `syncanysql-0.1.7/syncanysql/calculaters/aggregate_calculater.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
 # 2023/3/21
 # create by: snower
 
 from syncany.calculaters.calculater import Calculater
+from syncany.filters import IntFilter, FloatFilter, ArrayFilter
+from ..utils import ensure_number, ensure_int
 
 
 class AggregateKeyCalculater(Calculater):
     def calculate(self, *args):
         if len(args) == 1:
-            return args[0]
+            return tuple(args[0]) if isinstance(args[0], list) else args[0]
         return args
 
 
 class AggregateCalculater(Calculater):
     def __init__(self, *args, **kwargs):
         super(AggregateCalculater, self).__init__(*args, **kwargs)
         
@@ -69,14 +71,16 @@
             if state_value is None:
                 return 1
             try:
                 return int(state_value) + 1
             except:
                 return state_value
 
+    def get_final_filter(self):
+        return IntFilter.default()
 
 class AggregateDistinctCountCalculater(StateAggregateCalculater):
     def aggregate(self, state_value, data_value):
         if data_value is None:
             return state_value
         if state_value is None:
             try:
@@ -108,33 +112,35 @@
         return state_value | data_value
 
     def final_value(self, state_value):
         if state_value is None:
             return 0
         return len(state_value)
 
+    def get_final_filter(self):
+        return IntFilter.default()
+
 
 class AggregateSumCalculater(AggregateCalculater):
     def aggregate(self, state_value, data_value):
         try:
-            return state_value + data_value
+            if isinstance(data_value, (int, float)):
+                return state_value + data_value
+            return state_value + ensure_number(data_value)
         except:
             if data_value is None:
                 return state_value or 0
             if state_value is None:
-                return data_value
-            try:
-                if isinstance(state_value, (int, float)):
-                    return state_value + type(state_value)(data_value)
-                try:
-                    return int(state_value) + int(data_value)
-                except:
-                    return float(state_value) + float(data_value)
-            except:
-                return state_value
+                if isinstance(data_value, (int, float)):
+                    return data_value
+                return ensure_number(data_value)
+            return state_value
+
+    def get_final_filter(self):
+        return FloatFilter.default()
 
 
 class AggregateMaxCalculater(AggregateCalculater):
     def aggregate(self, state_value, data_value):
         try:
             return max(state_value, data_value)
         except:
@@ -177,50 +183,46 @@
         return min(state_value, data_value)
 
 
 class AggregateAvgCalculater(StateAggregateCalculater):
     def aggregate(self, state_value, data_value):
         try:
             state_value["count_value"] += 1
-            state_value["sum_value"] += data_value
+            if isinstance(data_value, (int, float)):
+                state_value["sum_value"] += data_value
+            else:
+                state_value["sum_value"] += ensure_number(data_value)
             return state_value
         except:
             if data_value is None:
                 return state_value
             if state_value is None:
                 if data_value is None:
                     return None
-                return {"count_value": 1, "sum_value": data_value}
-            try:
-                if isinstance(state_value["sum_value"], (int, float)):
-                    state_value["count_value"] += 1
-                    state_value["sum_value"] += type(state_value["sum_value"])(data_value)
-                    return state_value
-                try:
-                    return {"count_value": state_value["count_value"] + 1,
-                            "sum_value": int(state_value["sum_value"]) + int(data_value)}
-                except:
-                    return {"count_value": state_value["count_value"] + 1,
-                            "sum_value": float(state_value["sum_value"]) + float(data_value)}
-            except:
-                return state_value
+                if isinstance(data_value, (int, float)):
+                    return {"count_value": 1, "sum_value": data_value}
+                return {"count_value": 1, "sum_value": ensure_number(data_value)}
+            return state_value
 
     def reduce(self, state_value, data_value):
         if data_value is None:
             return state_value
         if state_value is None:
             return data_value
         return {"count_value": state_value["count_value"] + data_value["count_value"],
                 "sum_value": state_value["sum_value"] + data_value["sum_value"]}
 
     def final_value(self, state_value):
         if state_value is None:
             return 0
         return state_value["sum_value"] / state_value["count_value"]
 
+    def get_final_filter(self):
+        return FloatFilter.default()
+
 
 class AggregateGroupConcatCalculater(StateAggregateCalculater):
     def aggregate(self, state_value, data_value):
         if data_value is None:
             return state_value
         if state_value is None:
             return [str(data_value)]
@@ -257,14 +259,17 @@
         return state_value + data_value
 
     def final_value(self, state_value):
         if state_value is None:
             return []
         return state_value
 
+    def get_final_filter(self):
+        return FloatFilter.default()
+
 
 class AggregateGroupUniqArrayCalculater(StateAggregateCalculater):
     def aggregate(self, state_value, data_value):
         if data_value is None:
             return state_value
         if state_value is None:
             try:
@@ -290,54 +295,72 @@
         return state_value | data_value
 
     def final_value(self, state_value):
         if state_value is None:
             return []
         return list(state_value)
 
+    def get_final_filter(self):
+        return ArrayFilter.default()
+
 
 class AggregateGroupBitAndCalculater(AggregateCalculater):
     def aggregate(self, state_value, data_value):
         if data_value is None:
             return state_value
         if state_value is None:
             return data_value
-        return state_value & data_value
+        if isinstance(data_value, int):
+            return state_value & data_value
+        return state_value & ensure_int(data_value)
 
     def reduce(self, state_value, data_value):
         if data_value is None:
             return state_value
         if state_value is None:
             return data_value
         return state_value & data_value
 
+    def get_final_filter(self):
+        return IntFilter.default()
+
 
 class AggregateGroupBitOrCalculater(AggregateCalculater):
     def aggregate(self, state_value, data_value):
         if data_value is None:
             return state_value
         if state_value is None:
             return data_value
-        return state_value | data_value
+        if isinstance(data_value, int):
+            return state_value | data_value
+        return state_value | ensure_int(data_value)
 
     def reduce(self, state_value, data_value):
         if data_value is None:
             return state_value
         if state_value is None:
             return data_value
         return state_value | data_value
 
+    def get_final_filter(self):
+        return IntFilter.default()
+
 
 class AggregateGroupBitXorCalculater(AggregateCalculater):
     def aggregate(self, state_value, data_value):
         if data_value is None:
             return state_value
         if state_value is None:
             return data_value
-        return state_value ^ data_value
+        if isinstance(data_value, int):
+            return state_value ^ data_value
+        return state_value ^ ensure_int(data_value)
 
     def reduce(self, state_value, data_value):
         if data_value is None:
             return state_value
         if state_value is None:
             return data_value
         return state_value ^ data_value
+
+    def get_final_filter(self):
+        return IntFilter.default()
```

### Comparing `syncanysql-0.1.6/syncanysql/calculaters/env_variable_calculater.py` & `syncanysql-0.1.7/syncanysql/calculaters/env_variable_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/datetime_funcs.py` & `syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/datetime_funcs.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # create by: snower
 
 import re
 import time
 import datetime
 import pytz
 from syncany.utils import get_timezone, parse_datetime
+from syncany.calculaters import typing_filter
 
 TIMEDELTA_UNITS = {"YEAR": 365 * 24 * 60 * 60, "QUARTER": 90 * 24 * 60 * 60, "MONTH": 30 * 24 * 60 * 60,
                    "WEEK": 7 * 24 * 60 * 60, "DAY": 24 * 60 * 60, "HOUR": 3600, "MINUTE": 60, "SECOND": 1,
                    "MICROSECOND": 1}
 TIME_INTERVAL_RE = re.compile('^(\d{4}?\-)?(\d+?\-)?(\d+?\s)?(\d+?:)?(\d+?)?(:\d+)?(\.\d+)?$')
 
 def calculate_datetime(dt, interval, is_sub=False):
@@ -47,45 +48,53 @@
             continue
         dt = calculate(units[i], int(values[i].replace("-", "").replace(".", "").replace(":", "")))
         if not dt:
             return None
     return dt
 
 
+@typing_filter(datetime.datetime)
 def mysql_currenttimestamp():
     return datetime.datetime.now(tz=get_timezone())
 
+@typing_filter(datetime.date)
 def mysql_curdate():
     return datetime.date.today()
 
+@typing_filter(datetime.date)
 def mysql_currentdate():
     return datetime.date.today()
 
+@typing_filter(datetime.time)
 def mysql_curtime():
     dt = datetime.datetime.now(tz=get_timezone())
     return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond)
 
+@typing_filter(datetime.time)
 def mysql_currenttime():
     dt = datetime.datetime.now(tz=get_timezone())
     return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond)
 
+@typing_filter(datetime.datetime)
 def mysql_sysdate():
     return datetime.datetime.now(tz=get_timezone())
 
+@typing_filter(datetime.date)
 def mysql_date(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     if isinstance(dt, datetime.datetime):
         return datetime.date(dt.year, dt.month, dt.day)
     if isinstance(dt, datetime.date):
         return dt
     return None
 
+@typing_filter(datetime.datetime)
 def mysql_datetime(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     if isinstance(dt, datetime.datetime):
         return dt
@@ -93,205 +102,232 @@
         return datetime.datetime(dt.year, dt.month, dt.day, tzinfo=get_timezone())
     if isinstance(dt, datetime.time):
         now = datetime.datetime.now(tz=get_timezone())
         return datetime.datetime(now.year, now.month, now.day, dt.hour, dt.minute,
                                  dt.second, dt.microsecond, tzinfo=get_timezone())
     return None
 
+@typing_filter(datetime.time)
 def mysql_time(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     if isinstance(dt, datetime.time):
         return dt
     if isinstance(dt, datetime.datetime):
         return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond, tzinfo=get_timezone())
     if isinstance(dt, datetime.date):
         return datetime.time(tzinfo=get_timezone())
     return None
 
+@typing_filter(int)
 def mysql_unix_timestamp(dt=None):
     if dt is None:
         return int(time.time())
     return int(time.mktime(dt.utctimetuple()))
 
+@typing_filter(datetime.datetime)
 def mysql_from_unixtime(t):
     if t is None:
         return None
     return datetime.datetime.utcfromtimestamp(t).replace(tzinfo=pytz.UTC).astimezone(tz=get_timezone())
 
+@typing_filter(int)
 def mysql_month(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return dt.month
 
+@typing_filter(str)
 def mysql_monthname(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return dt.strftime("%b")
 
+@typing_filter(str)
 def mysql_dayname(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return dt.strftime("%A")
 
+@typing_filter(int)
 def mysql_dayofweek(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return dt.weekday() + 1
 
+@typing_filter(int)
 def mysql_week(dt, mod=None):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return int(dt.strftime("%W" if str(mod) == "1" else "%U"))
 
+@typing_filter(int)
 def mysql_yearweek(dt, mod=None):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return int(dt.strftime("%Y%W" if str(mod) == "1" else "%Y%U"))
 
+@typing_filter(int)
 def mysql_dayofyear(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return int(dt.strftime("%j"))
 
+@typing_filter(int)
 def mysql_dayofmonth(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return dt.day
 
+@typing_filter(int)
 def mysql_year(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return dt.year
 
+@typing_filter(int)
 def mysql_time_to_sec(dt):
     if dt is None:
         return None
     st = parse_datetime("2000-01-01 00:00:00", None, get_timezone())
     if isinstance(dt, str):
         dt = parse_datetime("2000-01-01 " + dt, None, get_timezone())
     return int((dt - st).total_seconds())
 
+@typing_filter(str)
 def mysql_sec_to_time(t):
     if t is None:
         return None
     st = parse_datetime("2000-01-01 00:00:00", None, get_timezone())
     return (st + datetime.timedelta(seconds=t)).strftime("%H:%M:%S")
 
+@typing_filter(datetime.datetime)
 def mysql_dateadd(dt, i):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     if isinstance(i, (int, float)) or (isinstance(i, str) and i.isdigit()):
         return dt + datetime.timedelta(days=int(i))
     return calculate_datetime(dt, i, False)
 
+@typing_filter(datetime.datetime)
 def mysql_adddate(dt, i):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     if isinstance(i, (int, float)) or (isinstance(i, str) and i.isdigit()):
         return dt + datetime.timedelta(days=int(i))
     return calculate_datetime(dt, i, False)
 
+@typing_filter(datetime.datetime)
 def mysql_datesub(dt, i):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     if isinstance(i, (int, float)) or (isinstance(i, str) and i.isdigit()):
         return dt - datetime.timedelta(days=int(i))
     return calculate_datetime(dt, i, True)
 
+@typing_filter(datetime.datetime)
 def mysql_subdate(dt, i):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     if isinstance(i, (int, float)) or (isinstance(i, str) and i.isdigit()):
         return dt - datetime.timedelta(days=int(i))
     return calculate_datetime(dt, i, True)
 
+@typing_filter(datetime.datetime)
 def mysql_addtime(dt, i):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     if isinstance(i, (int, float)) or (isinstance(i, str) and i.isdigit()):
         return dt + datetime.timedelta(days=int(i))
     return calculate_datetime(dt, i, False)
 
+@typing_filter(datetime.datetime)
 def mysql_subtime(dt, i):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     if isinstance(i, (int, float)) or (isinstance(i, str) and i.isdigit()):
         return dt - datetime.timedelta(days=int(i))
     return calculate_datetime(dt, i, True)
 
+@typing_filter(int)
 def mysql_datediff(dt1, dt2):
     if dt1 is None or dt2 is None:
         return None
     if isinstance(dt1, (int, float, str)):
         dt1 = parse_datetime(str(dt1), None, get_timezone())
     if isinstance(dt2, (int, float, str)):
         dt2 = parse_datetime(str(dt2), None, get_timezone())
     return int((dt2 - dt1).total_seconds() / 86400)
 
+@typing_filter(str)
 def mysql_date_format(dt, f):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return dt.strftime(f.replace("%v", "%V"))
 
+@typing_filter(str)
 def mysql_time_format(dt, f):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime("2000-01-01 " + str(dt), None, get_timezone())
     return dt.strftime(f.replace("%v", "%V"))
 
+@typing_filter(int)
 def mysql_weekday(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return dt.weekday()
 
+@typing_filter(datetime.date)
 def mysql_utc_date():
     dt = datetime.datetime.utcnow()
     return datetime.date(dt.year, dt.month, dt.day)
 
+@typing_filter(datetime.time)
 def mysql_utc_time():
     dt = datetime.datetime.utcnow()
     return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond)
 
+@typing_filter(datetime.datetime)
 def mysql_utc_timestamp():
     dt = datetime.datetime.utcnow()
     return dt.replace(tzinfo=pytz.UTC)
 
 
 funcs = {key[6:]: value for key, value in globals().items() if key.startswith("mysql_")}
```

### Comparing `syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 # 2023/3/14
 # create by: snower
 
 import json
+from syncany.calculaters import typing_filter
 
 
 def parse_json_path(json_path):
     if not json_path:
         return []
     try:
         dot_index = json_path.index(".")
@@ -83,14 +84,15 @@
             if json_path_key not in json_data:
                 return None
             json_data = json_data[json_path_key]
         return json_data
     return get_value(json_data, parse_json_path(json_path))
 
 
+@typing_filter(int)
 def mysql_json_contains(target, candidate, path):
     if isinstance(target, str):
         try:
             target = json.loads(target)
         except:
             pass
     if isinstance(candidate, str):
@@ -98,14 +100,15 @@
             candidate = json.loads(candidate)
         except:
             pass
     target_value = get_json_path_value(target, path)
     return 1 if target_value == candidate else 0
 
 
+@typing_filter(int)
 def mysql_json_contains_path(json_doc, one_or_all, *paths):
     if isinstance(json_doc, str):
         try:
             json_doc = json.loads(json_doc)
         except:
             pass
     if not one_or_all:
@@ -127,15 +130,15 @@
         except:
             pass
     results = []
     for path in paths:
         results.append(get_json_path_value(json_doc, path))
     return results[0] if len(paths) == 1 else results
 
-
+@typing_filter(int)
 def mysql_json_depth(json_doc):
     if isinstance(json_doc, str):
         try:
             json_doc = json.loads(json_doc)
         except:
             pass
     def get_depth(json_doc):
@@ -145,40 +148,43 @@
             return max((get_depth(json_value) for json_value in json_doc)) + 1
         if isinstance(json_doc, dict):
             return max((get_depth(json_value) for json_value in json_doc.values())) + 1
         return 1
     return get_depth(json_doc)
 
 
+@typing_filter(list)
 def mysql_json_keys(json_doc, path=None):
     if isinstance(json_doc, str):
         try:
             json_doc = json.loads(json_doc)
         except:
             pass
     if path:
         json_doc = get_json_path_value(json_doc, path)
     if not isinstance(json_doc, dict):
         return []
     return list(json_doc.keys())
 
 
+@typing_filter(int)
 def mysql_json_length(json_doc, path=None):
     if isinstance(json_doc, str):
         try:
             json_doc = json.loads(json_doc)
         except:
             pass
     if path:
         json_doc = get_json_path_value(json_doc, path)
     if not isinstance(json_doc, (list, dict)):
         return 0
     return len(json_doc)
 
 
+@typing_filter(int)
 def mysql_json_valid(val):
     if isinstance(val, str):
         try:
             json.loads(val)
             return 1
         except:
             return 0
```

### Comparing `syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/logical_funcs.py` & `syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/logical_funcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,99 @@
 # -*- coding: utf-8 -*-
 # 2023/5/29
 # create by: snower
 
-from .number_funcs import ensure_number
-from .string_funcs import ensure_str
+from syncany.calculaters import typing_filter
+from ...utils import ensure_number, ensure_str
 
+@typing_filter(int)
 def mysql_eq(a, b):
     if a is None or b is None:
         return None
     if isinstance(a, (int, float, bool)) or isinstance(b, (int, float, bool)):
         return 1 if ensure_number(a) == ensure_number(b) else 0
     if isinstance(a, str) or isinstance(b, str):
         return 1 if ensure_str(a) == ensure_str(b) else 0
     return 1 if a == b else 0
 
+@typing_filter(int)
 def mysql_neq(a, b):
     if a is None or b is None:
         return None
     if isinstance(a, (int, float, bool)) or isinstance(b, (int, float, bool)):
         return 1 if ensure_number(a) != ensure_number(b) else 0
     if isinstance(a, str) or isinstance(b, str):
         return 1 if ensure_str(a) != ensure_str(b) else 0
     return 1 if a != b else 0
 
+@typing_filter(int)
 def mysql_gt(a, b):
     if a is None or b is None:
         return None
     if isinstance(a, (int, float, bool)) or isinstance(b, (int, float, bool)):
         return 1 if ensure_number(a) > ensure_number(b) else 0
     if isinstance(a, str) or isinstance(b, str):
         return 1 if ensure_str(a) > ensure_str(b) else 0
     return 1 if a > b else 0
 
+@typing_filter(int)
 def mysql_gte(a, b):
     if a is None or b is None:
         return None
     if isinstance(a, (int, float, bool)) or isinstance(b, (int, float, bool)):
         return 1 if ensure_number(a) >= ensure_number(b) else 0
     if isinstance(a, str) or isinstance(b, str):
         return 1 if ensure_str(a) >= ensure_str(b) else 0
     return 1 if a >= b else 0
 
+@typing_filter(int)
 def mysql_lt(a, b):
     if a is None or b is None:
         return None
     if isinstance(a, (int, float, bool)) or isinstance(b, (int, float, bool)):
         return 1 if ensure_number(a) < ensure_number(b) else 0
     if isinstance(a, str) or isinstance(b, str):
         return 1 if ensure_str(a) < ensure_str(b) else 0
     return 1 if a < b else 0
 
+@typing_filter(int)
 def mysql_lte(a, b):
     if a is None or b is None:
         return None
     if isinstance(a, (int, float, bool)) or isinstance(b, (int, float, bool)):
         return 1 if ensure_number(a) <= ensure_number(b) else 0
     if isinstance(a, str) or isinstance(b, str):
         return 1 if ensure_str(a) <= ensure_str(b) else 0
     return 1 if a <= b else 0
 
+@typing_filter(int)
 def mysql_in(a, b):
     if a is None:
         return None
     hs_none = False
     for v in b:
         if b is None:
             hs_none = True
             continue
         if mysql_eq(a, v):
             return 1
     return None if hs_none else 0
 
+@typing_filter(int)
 def mysql_not(a):
     if a is None:
         return None
     return 1 if not a else 0
 
+@typing_filter(int)
 def mysql_is(a, b):
     if a is None or b is None:
         return 1 if a is b else 0
     return mysql_eq(a, b)
 
+@typing_filter(int)
 def mysql_is_not(a, b):
     if a is None or b is None:
         return 0 if a is b else 1
     return mysql_neq(a, b)
 
 funcs = {key[6:]: value for key, value in globals().items() if key.startswith("mysql_")}
```

### Comparing `syncanysql-0.1.6/syncanysql/calculaters/mysql_funcs/string_funcs.py` & `syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/string_funcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,282 +1,306 @@
 # -*- coding: utf-8 -*-
 # 2023/3/2
 # create by: snower
 
-import datetime
 import socket
 import base64
 import binascii
+from syncany.calculaters import typing_filter
+from ...utils import ensure_str
 
-def ensure_str(x):
-    if isinstance(x, str):
-        return x
-    if x is None:
-        raise ValueError('value is None')
-    if not x:
-        return '0'
-    if x is True:
-        return '1'
-    if isinstance(x, bytes):
-        return x.decode("utf-8")
-    if isinstance(x, datetime.date):
-        if isinstance(x, datetime.datetime):
-            return x.strftime("%Y-%m-%d %H:%M:%S")
-        return x.strftime("%Y-%m-%d")
-    if isinstance(x, datetime.time):
-        return x.strftime("%H:%M:%S")
-    return str(x)
-
+@typing_filter(str)
 def mysql_bin(x):
     if isinstance(x, (int, float)):
         return bin(int(x))
     if x is None:
         return None
     if x is True:
         return bin(1)
     if not x:
         return bin(0)
     return bin(x)
 
+@typing_filter(str)
 def mysql_hex(x):
     if isinstance(x, (int, float)):
         return hex(int(x))
     if x is None:
         return None
     if x is True:
         return hex(1)
     if not x:
         return hex(0)
     return binascii.b2a_hex(x.encode("utf-8")).decode("utf-8")
 
+@typing_filter(str)
 def mysql_unhex(x):
     if x is None:
         return None
     return binascii.a2b_hex(ensure_str(x))
 
+@typing_filter(str)
 def mysql_oct(x):
     if x is None:
         return None
     return oct(x)[2:]
 
+@typing_filter(int)
 def mysql_ord(x):
     if x is None:
         return None
     return ord(ensure_str(x))
 
+@typing_filter(str)
 def mysql_ascii(s):
     if s is None:
         return None
     return sum([ord(c) for c in ensure_str(s)])
 
+@typing_filter(str)
 def mysql_char(*args):
     return "".join([chr(arg) for arg in args])
 
+@typing_filter(int)
 def mysql_bit_length(s):
     if s is None:
         return None
     return len(s.encode("utf-8")) * 8
 
+@typing_filter(int)
 def mysql_length(s):
     if s is None:
         return None
     return len(s.encode("utf-8"))
 
+@typing_filter(int)
 def mysql_char_length(s):
     if s is None:
         return None
     return len(ensure_str(s))
 
+@typing_filter(int)
 def mysql_character_length(s):
     if s is None:
         return None
     return len(ensure_str(s))
 
+@typing_filter(str)
 def mysql_concat(*args):
     return "".join(ensure_str(arg) for arg in args)
 
+@typing_filter(str)
 def mysql_concat_ws(sep, *args):
     return sep.join(ensure_str(arg) for arg in args)
 
+@typing_filter(str)
 def mysql_insert(s1, x, l, s2):
     s1, s2 = ensure_str(s1), ensure_str(s2)
     return s1[: x - 1] + s2 + s1[x + l - 1:]
 
+@typing_filter(str)
 def mysql_lower(s):
     if s is None:
         return None
     return ensure_str(s).lower()
 
+@typing_filter(str)
 def mysql_upper(s):
     if s is None:
         return None
     return ensure_str(s).upper()
 
+@typing_filter(str)
 def mysql_ucase(s):
     if s is None:
         return None
     return ensure_str(s).upper()
 
+@typing_filter(str)
 def mysql_left(s, x):
     if s is None:
         return None
     return ensure_str(s)[:x]
 
+@typing_filter(str)
 def mysql_right(s, x):
     if s is None:
         return None
     return ensure_str(s)[-x:]
 
+@typing_filter(str)
 def mysql_trim(s):
     if s is None:
         return None
     return ensure_str(s).strip()
 
+@typing_filter(str)
 def mysql_elt(n, *args):
     return args[n - 1] if n < len(args) else None
 
+@typing_filter(int)
 def mysql_field(s, *args):
     if s is None:
         return None
     try:
         return args.index(s) + 1
     except ValueError:
         return 0
 
+@typing_filter(int)
 def mysql_find_in_set(s, ss):
     if s is None:
         return None
     try:
         return ensure_str(ss).split(",").index(s) + 1
     except ValueError:
         return 0
 
+@typing_filter(str)
 def mysql_replace(s, s1, s2):
     if s is None:
         return None
     return ensure_str(s).replace(s1, s2)
 
+@typing_filter(str)
 def mysql_substring(s, n, l=None):
     if s is None:
         return None
     s = ensure_str(s)
     if isinstance(l, int):
         return s[n - 1: n + l - 1]
     return s[n - 1:]
 
+@typing_filter(str)
 def mysql_substr(s, n, l=None):
     if s is None:
         return None
     s = ensure_str(s)
     if isinstance(l, int):
         return s[n - 1: n + l - 1]
     return s[n - 1:]
 
+@typing_filter(str)
 def mysql_substring_index(s, d, c):
     if s is None:
         return None
     s, d = ensure_str(s), ensure_str(d)
     if c < 0:
         return d.join(s.split(d)[-c:])
     return d.join(s.split(d)[:c])
 
+@typing_filter(str)
 def mysql_repeat(s, c):
     if s is None:
         return None
     return ensure_str(s) * c
 
+@typing_filter(str)
 def mysql_reverse(s):
     if s is None:
         return None
     return ensure_str(s)[::-1]
 
+@typing_filter(int)
 def mysql_strcmp(s1, s2):
     if s1 is None or s2 is None:
         return None
     s1, s2 = ensure_str(s1), ensure_str(s2)
     return 0 if s1 == s2 else (-1 if s1 < s2 else 1)
 
+@typing_filter(int)
 def mysql_startswith(s1, s2):
     if s1 is None or s2 is None:
         return None
     s1, s2 = ensure_str(s1), ensure_str(s2)
     return 1 if s1.startswith(s2) else 0
 
+@typing_filter(int)
 def mysql_endswith(s1, s2):
     if s1 is None or s2 is None:
         return None
     s1, s2 = ensure_str(s1), ensure_str(s2)
     return 1 if s1.endswith(s2) else 0
 
+@typing_filter(int)
 def mysql_contains(s1, s2):
     if s1 is None or s2 is None:
         return None
     try:
         return 1 if s2 in s1 else 0
     except:
         s1, s2 = ensure_str(s1), ensure_str(s2)
         return 1 if s2 in s1 else 0
 
+@typing_filter(int)
 def mysql_crc32(s):
     if s is None:
         return None
     import zlib
     return zlib.crc32(s)
 
+@typing_filter(str)
 def mysql_from_base64(s):
     if s is None:
         return None
     return base64.b64decode(s.encode("utf-8")).decode("utf-8")
 
+@typing_filter(str)
 def mysql_to_base64(s):
     if s is None:
         return None
     return base64.b64encode(s.encode("utf-8")).decode("utf-8")
 
+@typing_filter(str)
 def mysql_inet4_aton(s):
     if s is None:
         return None
     try:
         return binascii.b2a_hex(socket.inet_aton(s)).decode("utf-8")
     except:
         return None
 
+@typing_filter(str)
 def mysql_inet4_ntoa(b):
     if b is None:
         return None
     try:
         return socket.inet_ntoa(b)
     except:
         return None
 
+@typing_filter(int)
 def mysql_is_ipv4(s):
     if s is None:
         return None
     try:
         socket.inet_aton(s)
         return 1
     except:
         return 0
 
+@typing_filter(str)
 def mysql_inet6_aton(s):
     if s is None:
         return None
     try:
         return binascii.b2a_hex(socket.inet_pton(socket.AF_INET6, s)).decode("utf-8")
     except:
         return None
 
+@typing_filter(str)
 def mysql_inet6_ntoa(b):
     if b is None:
         return None
     try:
         return socket.inet_ntop(socket.AF_INET6, b)
     except:
         return None
 
+@typing_filter(int)
 def mysql_is_ipv6(s):
     if s is None:
         return None
     try:
         socket.inet_pton(socket.AF_INET6, s)
         return 1
     except:
```

### Comparing `syncanysql-0.1.6/syncanysql/calculaters/window_calculater.py` & `syncanysql-0.1.7/syncanysql/calculaters/window_calculater.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 # 2023/6/1
 # create by: snower
 
 from syncany.calculaters.calculater import Calculater
+from syncany.filters import IntFilter, FloatFilter
 from ..errors import SyncanySqlExecutorException
 
 
 class WindowAggregateCalculater(Calculater):
     def __init__(self, *args, **kwargs):
         super(WindowAggregateCalculater, self).__init__(*args, **kwargs)
 
@@ -45,14 +46,17 @@
         return super(WindowStateAggregateCalculater, self).calculate(*args)
 
 
 class WindowStateAggregateRowNumberCalculater(WindowAggregateCalculater):
     def order_aggregate(self, state_value, data_value, context):
         return context.current_index + 1
 
+    def get_final_filter(self):
+        return IntFilter.default()
+
 
 class WindowStateAggregateRankCalculater(WindowStateAggregateCalculater):
     def order_aggregate(self, state_value, data_value, context):
         order_value = context.order_value
         if state_value is None:
             return {"order_value": order_value, "rank": 1, "row_number": 1}
         state_value["row_number"] += 1
@@ -61,14 +65,17 @@
         return state_value
 
     def final_value(self, state_value):
         if state_value is None:
             return 1
         return state_value["rank"]
 
+    def get_final_filter(self):
+        return IntFilter.default()
+
 
 class WindowStateAggregateDenseRankCalculater(WindowStateAggregateCalculater):
     def order_aggregate(self, state_value, data_value, context):
         order_value = context.order_value
         if state_value is None:
             return {"order_value": order_value, "rank": 1}
         if order_value != state_value["order_value"]:
@@ -76,14 +83,17 @@
         return state_value
 
     def final_value(self, state_value):
         if state_value is None:
             return 1
         return state_value["rank"]
 
+    def get_final_filter(self):
+        return IntFilter.default()
+
 
 class WindowStateAggregatePercentRankCalculater(WindowStateAggregateCalculater):
     def order_aggregate(self, state_value, data_value, context):
         order_value = context.order_value
         if state_value is None:
             return {"order_value": order_value, "rank": 1, "row_number": 1}
         state_value["row_number"] += 1
@@ -94,13 +104,19 @@
     def final_value(self, state_value):
         if state_value is None:
             return 1
         if state_value["row_number"] <= 1:
             return 0
         return state_value["rank"] - 1 / state_value["row_number"] - 1
 
+    def get_final_filter(self):
+        return FloatFilter.default()
+
 
 class WindowStateAggregateCumeDistCalculater(WindowAggregateCalculater):
     def order_aggregate(self, state_value, data_value, context):
         if not context.datas:
             return 0
         return context.current_index + 1 / len(context.datas) + 1
+
+    def get_final_filter(self):
+        return FloatFilter.default()
```

### Comparing `syncanysql-0.1.6/syncanysql/compiler.py` & `syncanysql-0.1.7/syncanysql/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,25 +417,14 @@
             if aggregate_expressions:
                 self.compile_aggregate_column(calculate_expression, config, arguments, primary_table, column_alias,
                                               group_expression, aggregate_expressions, join_tables)
                 continue
             self.compile_select_calculate_column(calculate_expression, config, arguments, primary_table, column_alias,
                                                  join_tables)
 
-        distinct_expression = expression.args.get("distinct")
-        if distinct_expression and not config.get("aggregate", {}).get("distinct_keys"):
-            if not isinstance(config["schema"], dict):
-                raise SyncanySqlCompileException('error distinct, select columns is unknown, related sql "%s"' % self.to_sql(expression))
-            if "aggregate" not in config:
-                config["aggregate"] = copy.deepcopy(DEAULT_AGGREGATE)
-            for name, column in config["schema"].items():
-                if name in config["aggregate"]["schema"]:
-                    continue
-                config["aggregate"]["distinct_keys"].append(copy.deepcopy(column))
-
         where_expression = expression.args.get("where")
         if where_expression and isinstance(where_expression, sqlglot_expressions.Where):
             where_condition = self.compile_where_condition(where_expression.args["this"], config, arguments, primary_table, join_tables)
             if where_condition:
                 if not config["intercepts"]:
                     config["intercepts"] = [["#const", 1], ["#const", 1]]
                 config["intercepts"][0] = where_condition
@@ -462,22 +451,37 @@
             offset_expression, limit_expression = expression.args.get("limit"), expression.args.get("offset")
         else:
             offset_expression, limit_expression = None, expression.args.get("limit")
         if limit_expression:
             offset_value = max(int(offset_expression.args["expression"].args["this"]), 0) if offset_expression else 0
             limit_value = max(int(limit_expression.args["expression"].args["this"]), 1)
             if limit_value > 0:
-                if config["intercepts"] or (config.get("aggregate") and config["aggregate"]["schema"]) \
+                if config["intercepts"] or (config.get("aggregate") and (config["aggregate"]["schema"]
+                                                                         or config["aggregate"]["window_schema"])) \
                         or config["pipelines"] or offset_value > 0:
                     config["pipelines"].append([">>@array::slice", "$.*|array", offset_value, offset_value + limit_value])
                 else:
                     arguments["@limit"] = limit_value
 
         if group_expression and ("aggregate" not in config or not config["aggregate"] or not config["aggregate"]["schema"]):
             self.compile_group_column(group_expression, config, arguments, primary_table, join_tables)
+        distinct_expression = expression.args.get("distinct")
+        if distinct_expression and ("aggregate" not in config or not config["aggregate"] or not config["aggregate"]["schema"]):
+            if not group_expression:
+                self.compile_distinct_column(expression, config, arguments, primary_table, join_tables)
+            else:
+                if not isinstance(config["schema"], dict):
+                    raise SyncanySqlCompileException(
+                        'error distinct, select columns is unknown, related sql "%s"' % self.to_sql(expression))
+                if "aggregate" not in config:
+                    config["aggregate"] = copy.deepcopy(DEAULT_AGGREGATE)
+                for name, column in config["schema"].items():
+                    if name in config["aggregate"]["schema"]:
+                        continue
+                    config["aggregate"]["distinct_keys"].append(copy.deepcopy(column))
         if not from_expression and not primary_table["outputer_primary_keys"] and isinstance(config["schema"], dict):
             for column_alias in config["schema"]:
                 if not column_alias.isidentifier():
                     continue
                 primary_table["outputer_primary_keys"] = [column_alias]
                 break
         config["input"] = "".join(["&.", primary_table["db"], ".", primary_table["name"], "::",
@@ -951,26 +955,58 @@
                 column_alias = list(config["schema"].keys())[0]
             else:
                 raise SyncanySqlCompileException('error group by, unknown column, related sql "%s"' % self.to_sql(expression))
         group_column = self.compile_aggregate_key(expression, config, arguments, primary_table, join_tables)
         if "aggregate" not in config:
             config["aggregate"] = copy.deepcopy(DEAULT_AGGREGATE)
         aggregate_column = {
-            "key": group_column,
+            "key": group_column[0] if len(group_column) == 1 else ["#make", group_column, [":@aggregate_key", "$.*"]],
+            "value": config["schema"][column_alias],
+            "calculate": "$$.value",
+            "aggregate": [":#aggregate", "$.key", "$$.value"],
+            "reduce": "$$." + column_alias,
+            "final_value": None
+        }
+        config["schema"][column_alias] = ["#make", {
+            "key": copy.deepcopy(aggregate_column["key"]),
+            "value": copy.deepcopy(aggregate_column["value"])
+        }, [":#aggregate", "$.key", "$$.value"]]
+        config["aggregate"]["key"] = copy.deepcopy(aggregate_column["key"])
+        config["aggregate"]["schema"][column_alias] = aggregate_column
+
+    def compile_distinct_column(self, expression, config, arguments, primary_table, join_tables):
+        column_alias = None
+        if primary_table["outputer_primary_keys"]:
+            if isinstance(config["schema"], dict) and primary_table["outputer_primary_keys"][0] in config["schema"]:
+                column_alias = primary_table["outputer_primary_keys"][0]
+        if not column_alias:
+            if isinstance(config["schema"], dict) and config["schema"]:
+                column_alias = list(config["schema"].keys())[0]
+            else:
+                raise SyncanySqlCompileException('error group by, unknown column, related sql "%s"' % self.to_sql(expression))
+        if "aggregate" not in config:
+            config["aggregate"] = copy.deepcopy(DEAULT_AGGREGATE)
+        group_column = []
+        for select_name, select_column in config["schema"].items():
+            if select_name in config["aggregate"]["schema"] or select_name in config["aggregate"]["window_schema"]:
+                continue
+            group_column.append(copy.deepcopy(select_column))
+        aggregate_column = {
+            "key": group_column[0] if len(group_column) == 1 else ["#make", group_column, [":@aggregate_key", "$.*"]],
             "value": config["schema"][column_alias],
             "calculate": "$$.value",
             "aggregate": [":#aggregate", "$.key", "$$.value"],
             "reduce": "$$." + column_alias,
             "final_value": None
         }
         config["schema"][column_alias] = ["#make", {
-            "key": copy.deepcopy(group_column),
-            "value": copy.deepcopy(config["schema"][column_alias])
+            "key": copy.deepcopy(aggregate_column["key"]),
+            "value": copy.deepcopy(aggregate_column["value"])
         }, [":#aggregate", "$.key", "$$.value"]]
-        config["aggregate"]["key"] = copy.deepcopy(group_column)
+        config["aggregate"]["key"] = copy.deepcopy(aggregate_column["key"])
         config["aggregate"]["schema"][column_alias] = aggregate_column
 
     def compile_aggregate_column(self, expression, config, arguments, primary_table, column_alias, group_expression,
                                  aggregate_expressions, join_tables):
         group_column = self.compile_aggregate_key(group_expression, config, arguments, primary_table, join_tables)
         aggregate_value_expressions = []
         for i in range(len(aggregate_expressions)):
@@ -993,66 +1029,62 @@
             aggregate_value_expressions.append(value_expressions)
 
         if "aggregate" not in config:
             config["aggregate"] = copy.deepcopy(DEAULT_AGGREGATE)
         if len(aggregate_expressions) == 1 and aggregate_expressions[0] is expression:
             value_column = self.compile_aggregate_value(aggregate_expressions[0], config, arguments, primary_table, join_tables,
                                                         aggregate_value_expressions[0])
-            if value_column and len(value_column) == 2:
-                value_column = value_column[1]
             aggregate_calculate, reduce_calculate, final_calculate = self.compile_aggregate_calculate(aggregate_expressions[0])
             aggregate_column = {
-                "key": group_column,
-                "value": value_column,
+                "key": group_column[0] if len(group_column) == 1 else ["#make", group_column, [":@aggregate_key", "$.*"]],
+                "value": value_column[0] if len(value_column) == 1 else ["#make", value_column],
                 "calculate": [aggregate_calculate, "$." + column_alias, "$$.value"],
                 "aggregate": [":#aggregate", "$.key", [aggregate_calculate, "$." + column_alias, "$$.value"]],
                 "reduce": [reduce_calculate, "$." + column_alias, "$$." + column_alias],
                 "final_value": [final_calculate, "$." + column_alias] if final_calculate else None
             }
         else:
             value_column, calculate_column, reduce_column = ["#make", {}], ["#make", {}], ["#make", {}]
             for i in range(len(aggregate_expressions)):
                 aggregate_value_key = "value_%d" % id(aggregate_expressions[i])
                 aggregate_value_column = self.compile_aggregate_value(aggregate_expressions[i], config, arguments, primary_table,
                                                                       join_tables, aggregate_value_expressions[i])
-                if aggregate_value_column and len(aggregate_value_column) == 2:
-                    aggregate_value_column = aggregate_value_column[1]
                 aggregate_calculate, reduce_calculate, final_calculate = self.compile_aggregate_calculate(aggregate_expressions[i])
-                value_column[1][aggregate_value_key] = aggregate_value_column
+                value_column[1][aggregate_value_key] = aggregate_value_column[0] if len(aggregate_value_column) == 1 else ["#make", aggregate_value_column]
                 calculate_column[1][aggregate_value_key] = [aggregate_calculate, "$." + column_alias + "." + aggregate_value_key,
                                                             "$$.value." + aggregate_value_key]
                 reduce_column[1][aggregate_value_key] = [reduce_calculate, "$." + column_alias + "." + aggregate_value_key,
                                                          "$$." + column_alias + "." + aggregate_value_key]
                 setattr(aggregate_expressions[i], "syncany_valuer",
                         [final_calculate, "$." + column_alias + "." + aggregate_value_key]
                         if final_calculate else ("$." + column_alias + "." + aggregate_value_key))
             self.compile_select_calculate_column(expression, config, arguments, primary_table, column_alias,
                                                  join_tables, False)
             aggregate_column = {
-                "key": group_column,
+                "key": group_column[0] if len(group_column) == 1 else ["#make", group_column, [":@aggregate_key", "$.*"]],
                 "value": value_column,
                 "calculate": calculate_column,
                 "aggregate": [":#aggregate", "$.key", copy.deepcopy(calculate_column)],
                 "reduce": reduce_column,
                 "final_value": config["schema"][column_alias]
             }
 
         config["schema"][column_alias] = ["#make", {
-            "key": copy.deepcopy(group_column),
-            "value": copy.deepcopy(value_column),
+            "key": copy.deepcopy(aggregate_column["key"]),
+            "value": copy.deepcopy(aggregate_column["value"]),
         }, copy.deepcopy(aggregate_column["aggregate"])]
         config["aggregate"]["key"] = copy.deepcopy(aggregate_column["key"])
         config["aggregate"]["schema"][column_alias] = aggregate_column
         primary_table["select_columns"][column_alias] = expression
 
     def compile_aggregate_key(self, expression, config, arguments, primary_table, join_tables):
         if not expression:
-            return ["@aggregate_key", ["#const", "__k_g__"]]
+            return [["#const", "__k_g__"]]
 
-        group_column = ["@aggregate_key"]
+        group_column = []
         for group_expression in expression.args["expressions"]:
             if self.is_column(group_expression, config, arguments):
                 group_expression_column = self.parse_column(group_expression, config, arguments)
                 if isinstance(config["schema"], dict) and not group_expression_column["table_name"] \
                         and group_expression_column["column_name"] in config["schema"]:
                     group_column.append(config["schema"][group_expression_column["column_name"]])
                     continue
@@ -1083,19 +1115,19 @@
             group_column.append(self.compile_join_column(group_expression, config, arguments, primary_table,
                                                          calculate_column, column_join_tables))
         return group_column
 
     def compile_aggregate_value(self, expression, config, arguments, primary_table, join_tables, value_expressions):
         if isinstance(expression, sqlglot_expressions.Count) and isinstance(expression.args["this"],
                                                                             sqlglot_expressions.Star):
-            return ["@make", ["#const", 0]]
+            return [["#const", 0]]
         if not value_expressions:
-            return ["@make", ["#const", None]]
+            return [["#const", None]]
 
-        value_column = ["@make"]
+        value_column = []
         for value_expression in value_expressions:
             calculate_fields = []
             self.parse_calculate(value_expression, config, arguments, primary_table, calculate_fields)
             calculate_fields = [calculate_field for calculate_field in calculate_fields if calculate_field["table_name"]
                                 and calculate_field["table_name"] != primary_table["table_name"]]
             if not calculate_fields:
                 value_column.append(self.compile_calculate(value_expression, config, arguments, primary_table, []))
@@ -1176,35 +1208,35 @@
 
             partition_column = self.compile_window_key(window_expressions[i].args["partition_by"], config, arguments,
                                                        primary_table, join_tables) if window_expressions[i].args.get("partition_by") else None
             order_column = self.compile_window_order(window_expressions[i].args["order"], config, arguments,
                                                      primary_table, join_tables) if window_expressions[i].args.get("order") else None
             value_column = self.compile_window_value(window_expressions[i].args["this"], config, arguments, primary_table,
                                                      join_tables, value_expressions) if value_expressions else None
-            if value_column and len(value_column) == 2:
-                value_column = value_column[1]
             is_window_aggregate_calculate, aggregate_calculate, final_calculate = self.compile_window_calculate(window_expressions[i])
             partition_calculate = "$.partition_key" if partition_column is not None else None
             order_calculate = {"valuer": "$.order_key", "orders": order_column["orders"]} if order_column is not None else None
             value_calculate = "$.value" if value_column is not None else None
             if is_window_aggregate_calculate:
                 aggregate_calculate = [":#partition", partition_calculate, order_calculate, value_calculate,
                                        [aggregate_calculate, "$.state", "$.value", "$.context"]]
             else:
                 aggregate_calculate = [":#partition", partition_calculate, order_calculate, value_calculate,
                                        [aggregate_calculate, "$.state", "$.value"]]
             if final_calculate:
                 aggregate_calculate.append([":" + final_calculate, "$.*"])
             window_aggregate_column = ["#make", {}, aggregate_calculate]
             if partition_column is not None:
-                window_aggregate_column[1]["partition_key"] = partition_column
+                window_aggregate_column[1]["partition_key"] = partition_column[0] \
+                    if len(partition_column) == 1 else ["#make", partition_column, [":@aggregate_key", "$.*"]]
             if order_column is not None:
-                window_aggregate_column[1]["order_key"] = order_column["valuer"]
+                window_aggregate_column[1]["order_key"] = order_column["valuer"][0] \
+                    if len(order_column["valuer"]) == 1 else ["#make", order_column["valuer"], [":@aggregate_key", "$.*"]]
             if value_column is not None:
-                window_aggregate_column[1]["value"] = value_column
+                window_aggregate_column[1]["value"] = value_column[0] if len(value_column) == 1 else ["#make", value_column]
 
             if len(window_expressions) > 1:
                 aggregate_column_alias = "__window_aggregate_value_%d__" % id(window_expressions[i])
                 config["schema"][aggregate_column_alias] = window_aggregate_column
                 setattr(window_expressions[i], "syncany_valuer", "$." + aggregate_column_alias)
                 if not isinstance(config["aggregate"]["window_schema"][column_alias]["aggregate"], dict):
                     config["aggregate"]["window_schema"][column_alias]["aggregate"] = {}
@@ -1216,17 +1248,17 @@
         if len(window_expressions) > 1:
             self.compile_select_calculate_column(expression, config, arguments, primary_table, column_alias, join_tables, False)
             config["aggregate"]["window_schema"][column_alias]["final_value"] = config["schema"].pop(column_alias, None)
         primary_table["select_columns"][column_alias] = expression
 
     def compile_window_key(self, expressions, config, arguments, primary_table, join_tables):
         if not expressions:
-            return ["@aggregate_key", ["#const", "__k_g__"]]
+            return [["#const", "__k_g__"]]
 
-        key_column = ["@aggregate_key"]
+        key_column = []
         for expression in expressions:
             if self.is_column(expression, config, arguments):
                 key_expression_column = self.parse_column(expression, config, arguments)
                 if isinstance(config["schema"], dict) and not key_expression_column["table_name"] \
                         and key_expression_column["column_name"] in config["schema"]:
                     key_column.append(config["schema"][key_expression_column["column_name"]])
                     continue
@@ -1265,19 +1297,19 @@
             value_order_expressions.append(order_expression.args["this"])
         return {"valuer": self.compile_window_key(value_order_expressions, config, arguments,
                                                   primary_table, join_tables), "orders": orders}
 
     def compile_window_value(self, expression, config, arguments, primary_table, join_tables, value_expressions):
         if isinstance(expression, sqlglot_expressions.Count) and isinstance(expression.args["this"],
                                                                             sqlglot_expressions.Star):
-            return ["@make", ["#const", 0]]
+            return [["#const", 0]]
         if not value_expressions:
-            return ["@make", ["#const", None]]
+            return [["#const", None]]
 
-        value_column = ["@make"]
+        value_column = []
         for value_expression in value_expressions:
             calculate_fields = []
             self.parse_calculate(value_expression, config, arguments, primary_table, calculate_fields)
             calculate_fields = [calculate_field for calculate_field in calculate_fields if calculate_field["table_name"]
                                 and calculate_field["table_name"] != primary_table["table_name"]]
             if not calculate_fields:
                 value_column.append(self.compile_calculate(value_expression, config, arguments, primary_table, []))
@@ -1380,15 +1412,20 @@
                     config["defines"][define_name] = self.compile_calculate(expression.args["expressions"][0], config, arguments, primary_table, column_join_tables, join_index)
                 return ["#call", define_name, "$.*"]
 
             if calculater_name not in ("add", "sub", "mul", "div", "mod") and is_mysql_func(calculater_name):
                 column = ["@mysql::" + calculater_name]
             else:
                 if calculater_name[:8] == "convert_":
-                    column = ["@" + calculater_name + "|" + calculater_name[8:]]
+                    if calculater_name[8:] in self.TYPE_FILTERS:
+                        calculater_name = "convert_" + self.TYPE_FILTERS[calculater_name[8:]]
+                    if calculater_name.startswith("convert_str"):
+                        column = ["@convert_string|str"]
+                    else:
+                        column = ["@" + calculater_name + "|" + calculater_name[8:]]
                 else:
                     calculater_modules = calculater_name.split("$")
                     column = ["@" + calculater_modules[0] + (("::" + ".".join(calculater_modules[1:])) if len(calculater_modules) >= 2 else "")]
             for arg_expression in expression.args.get("expressions", []):
                 if self.is_const(arg_expression, config, arguments):
                     column.append(self.compile_const(arg_expression, config, arguments,
                                                      self.parse_const(arg_expression, config, arguments)))
@@ -1413,14 +1450,16 @@
                 typing_filter = "float"
             elif to_type in sqlglot_expressions.DataType.INTEGER_TYPES:
                 typing_filter = "int"
             elif to_type == sqlglot_expressions.DataType.Type.DATE:
                 typing_filter = "date"
             elif to_type in sqlglot_expressions.DataType.TEMPORAL_TYPES:
                 typing_filter = "datetime"
+            elif to_type == sqlglot_expressions.DataType.Type.TIME:
+                typing_filter = "time"
             elif to_type == sqlglot_expressions.DataType.TEXT_TYPES:
                 typing_filter = "str"
             else:
                 typing_filter = None
             value_column = self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
             if typing_filter:
                 return ["#if", ["#const", 1], value_column, None, ":$.*|" + typing_filter]
@@ -2432,28 +2471,14 @@
             if join_expression.side and join_expression.side.lower() == "right":
                 expression = self.optimize_rewrite_right_join(expression, config, arguments)
                 break
         for join_expression in expression.args["joins"]:
             if join_expression.kind and join_expression.kind.lower() == "inner":
                 expression = self.optimize_rewrite_inner_join(expression, config, arguments)
                 break
-
-        if len(expression.args["expressions"]) == 1:
-            if isinstance(expression.args["expressions"][0], sqlglot_expressions.Star):
-                return expression
-        aggregate_expressions = []
-        for select_expression in expression.args["expressions"]:
-            if isinstance(select_expression, sqlglot_expressions.Alias):
-                self.parse_aggregate(select_expression.args["this"], config, arguments, aggregate_expressions)
-                self.parse_window_aggregate(select_expression.args["this"], config, arguments, aggregate_expressions)
-            else:
-                self.parse_aggregate(select_expression, config, arguments, aggregate_expressions)
-                self.parse_window_aggregate(select_expression, config, arguments, aggregate_expressions)
-        if aggregate_expressions or expression.args.get("group"):
-            expression = self.optimize_rewrite_aggregate(expression, config, arguments, aggregate_expressions)
         return expression
 
     def optimize_rewrite_multi_select(self, expression, config, arguments, from_expression):
         primary_table = self.optimize_rewrite_parse_table(expression, config, arguments,
                                                           expression.args["from"].expressions[0])
         if not primary_table["table_name"]:
             return expression
@@ -2665,106 +2690,14 @@
         if limit_expression:
             offset_value = max(int(offset_expression.args["expression"].args["this"]), 0) if offset_expression else 0
             limit_value = max(int(limit_expression.args["expression"].args["this"]), 1)
             sql.append(
                 ("LIMIT %d, %d" % (offset_value, limit_value)) if offset_value > 0 else ("LIMIT %d" % limit_value))
         return maybe_parse(" ".join(sql), dialect=CompilerDialect)
 
-    def optimize_rewrite_aggregate(self, expression, config, arguments, aggregate_expressions):
-        primary_table = self.optimize_rewrite_parse_table(expression, config, arguments,
-                                                          expression.args["from"].expressions[0])
-        if not primary_table["table_name"]:
-            return expression
-        aggregate_calculate_fields = []
-        for aggregate_expression in aggregate_expressions:
-            self.parse_calculate(aggregate_expression, config, arguments, primary_table, aggregate_calculate_fields)
-        aggregate_calculate_fields = [calculate_field for calculate_field in aggregate_calculate_fields
-                                      if calculate_field["table_name"] and calculate_field["table_name"] != primary_table["table_name"]]
-        if not aggregate_calculate_fields:
-            if not expression.args.get("group"):
-                return expression
-            group_calculate_fields = []
-            for group_expression in expression.args["group"].args["expressions"]:
-                self.parse_calculate(group_expression, config, arguments, primary_table, group_calculate_fields)
-            group_calculate_fields = [calculate_field for calculate_field in group_calculate_fields
-                                      if calculate_field["table_name"] and calculate_field["table_name"] != primary_table["table_name"]]
-            if not group_calculate_fields:
-                return expression
-
-        sub_sql = ["SELECT"]
-        calculate_fields, sub_columns = [], []
-        for select_expression in expression.args["expressions"]:
-            if isinstance(select_expression, sqlglot_expressions.Column) \
-                    and isinstance(select_expression.args.get("this"), sqlglot_expressions.Star):
-                sub_columns.append(str(select_expression))
-            else:
-                self.parse_calculate(select_expression, config, arguments, primary_table, calculate_fields)
-        if expression.args.get("group"):
-            for group_expression in expression.args["group"].args["expressions"]:
-                self.parse_calculate(group_expression, config, arguments, primary_table, calculate_fields)
-        if expression.args.get("order"):
-            for order_expression in expression.args["order"].args["expressions"]:
-                self.parse_calculate(order_expression.args["this"], config, arguments, primary_table, calculate_fields)
-        for calculate_field in calculate_fields:
-            if not calculate_field["table_name"] and primary_table["table_name"] and primary_table["table_alias"]:
-                continue
-            if calculate_field["table_name"] and calculate_field["table_name"] != primary_table["table_name"]:
-                sub_column = "%s as `%s__%s`" % (str(calculate_field["expression"]),
-                                                 calculate_field["table_name"].replace(".", "__"),
-                                                 calculate_field["column_name"])
-            else:
-                sub_column = "%s as `%s`" % (str(calculate_field["expression"]), calculate_field["column_name"])
-            if sub_column not in sub_columns:
-                sub_columns.append(sub_column)
-        sub_sql.append(", ".join(sub_columns))
-        sub_sql.append(str(expression.args["from"]))
-        for join_expression in expression.args["joins"]:
-            sub_sql.append(str(join_expression))
-        if expression.args.get("where"):
-            sub_sql.append(str(expression.args["where"]))
-
-        subquery_name = "__subquery_" + str(uuid.uuid1().int)
-        sql = ["SELECT"]
-        if expression.args.get("distinct"):
-            sql.append(str(self.optimize_rewrite_except_table(expression.args["distinct"],
-                                                              config, arguments, primary_table)))
-        select_sql = []
-        for select_expression in expression.args["expressions"]:
-            if isinstance(select_expression, sqlglot_expressions.Alias):
-                select_sql.append(str(self.optimize_rewrite_except_table(select_expression, config, arguments, primary_table)))
-                continue
-            if isinstance(select_expression, sqlglot_expressions.Column):
-                if isinstance(select_expression.args.get("this"), sqlglot_expressions.Star):
-                    if (subquery_name + ".*") not in select_sql:
-                        select_sql.insert(0, subquery_name + ".*")
-                    continue
-                select_column_name = self.parse_column(select_expression, config, arguments)["column_name"]
-            else:
-                select_column_name = str(select_expression)
-            select_sql.append("%s as `%s`" %
-                              (str(self.optimize_rewrite_except_table(select_expression, config, arguments, primary_table)),
-                               select_column_name))
-        sql.append(", ".join(select_sql))
-        sql.append("FROM (%s) %s" % (" ".join(sub_sql), subquery_name))
-        if expression.args.get("group"):
-            sql.append(str(self.optimize_rewrite_except_table(expression.args["group"], config, arguments, primary_table)))
-        if expression.args.get("having"):
-            sql.append(str(expression.args["having"]))
-        if expression.args.get("order"):
-            sql.append(str(self.optimize_rewrite_except_table(expression.args["order"], config, arguments, primary_table)))
-        if expression.args.get("offset"):
-            offset_expression, limit_expression = expression.args.get("limit"), expression.args.get("offset")
-        else:
-            offset_expression, limit_expression = None, expression.args.get("limit")
-        if limit_expression:
-            offset_value = max(int(offset_expression.args["expression"].args["this"]), 0) if offset_expression else 0
-            limit_value = max(int(limit_expression.args["expression"].args["this"]), 1)
-            sql.append(("LIMIT %d, %d" % (offset_value, limit_value)) if offset_value > 0 else ("LIMIT %d" % limit_value))
-        return maybe_parse(" ".join(sql), dialect=CompilerDialect)
-
     def optimize_rewrite_parse_table(self, expression, config, arguments, table_expression):
         table = {"table_name": None, "table_alias": None, "columns": {}}
         if isinstance(table_expression, sqlglot_expressions.Table):
             table.update(self.parse_table(table_expression, config, arguments))
         elif isinstance(table_expression, sqlglot_expressions.Subquery):
             if "alias" not in table_expression.args:
                 return table
@@ -2812,37 +2745,14 @@
                 return
             on_expressions.append(condition_expression)
             for calculate_field in calculate_fields:
                 related_tables.add(calculate_field["table_name"])
         else:
             calcuate_expressions.append(condition_expression)
 
-    def optimize_rewrite_except_table(self, expression, config, arguments, primary_table):
-        def parse_except_table(arg_expression):
-            if not isinstance(arg_expression, sqlglot_expressions.Expression):
-                return arg_expression
-            if isinstance(arg_expression, sqlglot_expressions.Column):
-                column = self.parse_column(arg_expression, config, arguments)
-                if column["table_name"] and column["table_name"] != primary_table["table_name"]:
-                    arg_expression.args["this"].args["this"] = "%s__%s" % (
-                        column["table_name"].replace(".", "__"), column["column_name"])
-                if arg_expression.args.get("db"):
-                    arg_expression.args["db"] = None
-                if arg_expression.args.get("table"):
-                    arg_expression.args["table"] = None
-                return arg_expression
-            for child_arg_expression in arg_expression.args.values():
-                if isinstance(child_arg_expression, list):
-                    for child_item_arg_expression in child_arg_expression:
-                        parse_except_table(child_item_arg_expression)
-                else:
-                    parse_except_table(child_arg_expression)
-            return arg_expression
-        return parse_except_table(expression)
-
     def to_sql(self, expression_sql):
         if not isinstance(expression_sql, str):
             expression_sql = str(expression_sql)
         parser = SqlParser(expression_sql)
         segments = []
         last_start_index, last_end_index = 0, 0
         while True:
```

### Comparing `syncanysql-0.1.6/syncanysql/config.py` & `syncanysql-0.1.7/syncanysql/config.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/executor.py` & `syncanysql-0.1.7/syncanysql/executor.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/main.py` & `syncanysql-0.1.7/syncanysql/main.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/parser.py` & `syncanysql-0.1.7/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/prompt.py` & `syncanysql-0.1.7/syncanysql/prompt.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/taskers/delete.py` & `syncanysql-0.1.7/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/taskers/execute.py` & `syncanysql-0.1.7/syncanysql/taskers/execute.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/taskers/explain.py` & `syncanysql-0.1.7/syncanysql/taskers/explain.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/taskers/into.py` & `syncanysql-0.1.7/syncanysql/taskers/into.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/taskers/query.py` & `syncanysql-0.1.7/syncanysql/taskers/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -237,42 +237,61 @@
             "orders": [],
             "pipelines": [],
             "options": {},
             "dependencys": [],
             "states": [],
         })
 
-        group_column = ["@aggregate_key"] if not aggregate["key"] else copy.deepcopy(aggregate["key"])
-        group_column.extend(aggregate["distinct_keys"])
+        is_multi_group_key = True
+        if not aggregate["key"]:
+            if len(aggregate["distinct_keys"]) == 1:
+                group_column, is_multi_group_key = aggregate["distinct_keys"][0], False
+            else:
+                group_column = ["#make", aggregate["distinct_keys"], [":@aggregate_key", "$.*"]]
+        elif isinstance(aggregate["key"], list) and aggregate["key"][0] == "#make":
+            group_column = copy.deepcopy(aggregate["key"])
+            group_column[1].extend(aggregate["distinct_keys"])
+        else:
+            group_column = ["#make", [copy.deepcopy(aggregate["key"])] + aggregate["distinct_keys"], [":@aggregate_key", "$.*"]]
         distinct_aggregate = copy.deepcopy(DEAULT_AGGREGATE)
         for key, column in tuple(self.config["schema"].items()):
             if key in aggregate["distinct_aggregates"]:
                 config["schema"][key] = ["#make", {
-                    "key": "$._aggregate_distinct_key_",
+                    "key": ["@aggregate_key", "$._aggregate_distinct_key_"] if is_multi_group_key else "$._aggregate_distinct_key_",
                     "value": "$." + key
                 }, aggregate["schema"][key]["aggregate"]]
                 self.config["schema"][key] = aggregate["schema"][key]["value"]
             elif key in aggregate["schema"]:
                 self.config["schema"][key] = ["#make", {
-                    "key": group_column,
+                    "key": copy.deepcopy(group_column),
                     "value": aggregate["schema"][key]["value"]
                 }, aggregate["schema"][key]["aggregate"]]
                 distinct_aggregate["schema"][key] = copy.deepcopy(aggregate["schema"][key])
                 distinct_aggregate["schema"][key]["final_value"] = None
-                config["schema"][key] = ["#aggregate", "$._aggregate_distinct_key_", aggregate["schema"][key]["reduce"]]
+                if is_multi_group_key:
+                    config["schema"][key] = ["#aggregate", ["@aggregate_key", "$._aggregate_distinct_key_"],
+                                             aggregate["schema"][key]["reduce"]]
+                else:
+                    config["schema"][key] = ["#aggregate", "$._aggregate_distinct_key_", aggregate["schema"][key]["reduce"]]
             elif where_schema and key in where_schema:
                 continue
             else:
                 config["schema"][key] = "$." + key
 
         if aggregate["key"]:
             self.config["schema"]["_aggregate_distinct_key_"] = aggregate["key"]
-            aggregate["key"] = "$._aggregate_distinct_key_"
-        self.config["schema"]["_aggregate_distinct_aggregate_key_"] = ["#aggregate", group_column, ["#const", 0]]
-        distinct_aggregate["key"] = group_column
+            if is_multi_group_key:
+                aggregate["key"] = ["@aggregate_key", "$._aggregate_distinct_key_"]
+            else:
+                aggregate["key"] = "$._aggregate_distinct_key_"
+        self.config["schema"]["_aggregate_distinct_aggregate_key_"] = ["#make", {
+            "key": copy.deepcopy(group_column),
+            "value": ["#const", 0]
+        }, [":#aggregate", "$.key", "$$.value"]]
+        distinct_aggregate["key"] = copy.deepcopy(group_column)
         distinct_aggregate["schema"]["_aggregate_distinct_aggregate_key_"] = {
             "key": group_column,
             "value": ["#const", 0],
             "calculate": ["#const", 0],
             "aggregate": [":#aggregate", "$.key", ["#const", 0]],
             "reduce": ["#const", 0],
             "final_value": None
@@ -306,17 +325,27 @@
             "schema": {},
             "orders": [],
             "pipelines": [],
             "options": {},
             "dependencys": [],
             "states": [],
         })
+
+        is_multi_group_key = False
+        if isinstance(aggregate["key"], list):
+            if aggregate["key"] and aggregate["key"][0] == "@aggregate_key":
+                is_multi_group_key = True
+            elif len(aggregate["key"]) == 3 and aggregate["key"][0] == "#make" and aggregate["key"][2][0] == ":@aggregate_key":
+                is_multi_group_key = True
         for key, column in self.config["schema"].items():
             if key in aggregate["schema"]:
-                config["schema"][key] = ["#aggregate", "$._aggregate_key_", aggregate["schema"][key]["reduce"]]
+                if is_multi_group_key:
+                    config["schema"][key] = ["#aggregate", ["@aggregate_key", "$._aggregate_key_"], aggregate["schema"][key]["reduce"]]
+                else:
+                    config["schema"][key] = ["#aggregate", "$._aggregate_key_", aggregate["schema"][key]["reduce"]]
             else:
                 config["schema"][key] = "$." + key
         if aggregate["key"]:
             config["schema"]["_aggregate_key_"] = "$._aggregate_key_"
             self.config["schema"]["_aggregate_key_"] = aggregate["key"]
         config["aggregate"] = aggregate
         config["where_schema"] = where_schema
```

### Comparing `syncanysql-0.1.6/syncanysql/taskers/set.py` & `syncanysql-0.1.7/syncanysql/taskers/set.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/taskers/show.py` & `syncanysql-0.1.7/syncanysql/taskers/show.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql/taskers/use.py` & `syncanysql-0.1.7/syncanysql/taskers/use.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.6/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.1.7/syncanysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.1.6/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.1.7/syncanysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

