# Comparing `tmp/bahire-hasab-0.2.7.tar.gz` & `tmp/bahire-hasab-0.2.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bahire-hasab-0.2.7.tar", last modified: Wed Jun  7 07:45:21 2023, max compression
+gzip compressed data, was "bahire-hasab-0.2.7a0.tar", last modified: Wed Jun  7 07:52:17 2023, max compression
```

## Comparing `bahire-hasab-0.2.7.tar` & `bahire-hasab-0.2.7a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:21.651998 bahire-hasab-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-07 07:45:21.651998 bahire-hasab-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 07:45:21.651998 bahire-hasab-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:21.647998 bahire-hasab-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:21.651998 bahire-hasab-0.2.7/src/bahire_hasab/
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/src/bahire_hasab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/src/bahire_hasab/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:21.651998 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-07 07:45:21.000000 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-07 07:45:21.000000 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:45:21.000000 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 07:45:21.000000 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 07:45:21.000000 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:52:17.038201 bahire-hasab-0.2.7a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-07 07:52:17.034201 bahire-hasab-0.2.7a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 07:52:17.038201 bahire-hasab-0.2.7a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:52:17.034201 bahire-hasab-0.2.7a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:52:17.034201 bahire-hasab-0.2.7a0/src/bahire_hasab/
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/src/bahire_hasab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/src/bahire_hasab/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:52:17.034201 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-07 07:52:17.000000 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-07 07:52:17.000000 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:52:17.000000 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 07:52:17.000000 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 07:52:17.000000 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/top_level.txt
```

### Comparing `bahire-hasab-0.2.7/LICENSE` & `bahire-hasab-0.2.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.7/PKG-INFO` & `bahire-hasab-0.2.7a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.2.7
+Version: 0.2.7a0
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.7 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.7a0 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

### Comparing `bahire-hasab-0.2.7/README.md` & `bahire-hasab-0.2.7a0/README.md`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.7/setup.py` & `bahire-hasab-0.2.7a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("./README.md", "r") as file:
     long_description = file.read()
 setup(
     name="bahire-hasab",
     author="Hundera Awoke",
-    version="0.2.7",
+    version="0.2.7a",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="hunderaweke@gmail.com",
     url="https://github.com/hunderaweke/bahire-hasab",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=[],
```

### Comparing `bahire-hasab-0.2.7/src/bahire_hasab/__init__.py` & `bahire-hasab-0.2.7a0/src/bahire_hasab/__init__.py`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.7/src/bahire_hasab/__main__.py` & `bahire-hasab-0.2.7a0/src/bahire_hasab/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         action="store_true",
     )
     parser.add_argument(
         '-l',
         '--log-level',
         help="Loglever setter for the cli.",
         choices=['debug', 'info', 'warning', 'error', 'critical'],
-        default='info'
+        default='info',
     )
     args: argparse.Namespace = parser.parse_args()
 
     log_level = args.log_level.upper()
     
     logging.basicConfig(format='%(asctime)s | %(funcName)s | %(message)s ', datefmt='%d-%b-%y %H:%M:%S', level=log_level)
 
@@ -170,15 +170,14 @@
         year.beale_hamsa,
         year.tsome_hawaryat,
         year.tsome_dhnet,
     ]
     table = zip(name, value)
     # --------------------------------------------
     if args.all:
-        logger.debug('showing table')
         print(tabulate(table, headers=heading,tablefmt="simple_grid"));
  
     for a, m in zip(arguments, methods):
         if getattr(args, a):
             print(getattr(year, m))
```

### Comparing `bahire-hasab-0.2.7/src/bahire_hasab.egg-info/PKG-INFO` & `bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.2.7
+Version: 0.2.7a0
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.7 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.7a0 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

