# Comparing `tmp/krutils-0.20230607.2310.tar.gz` & `tmp/krutils-0.20230607.2323.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230607.2310.tar", last modified: Wed Jun  7 14:10:40 2023, max compression
+gzip compressed data, was "krutils-0.20230607.2323.tar", last modified: Wed Jun  7 14:23:32 2023, max compression
```

## Comparing `krutils-0.20230607.2310.tar` & `krutils-0.20230607.2323.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:10:40.577160 krutils-0.20230607.2310/
--rw-rw-rw-   0        0        0      526 2023-06-07 14:10:40.573058 krutils-0.20230607.2310/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230607.2310/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 14:10:40.483016 krutils-0.20230607.2310/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230607.2310/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230607.2310/krutils/CONST.py
--rw-rw-rw-   0        0        0       94 2023-06-06 15:37:21.000000 krutils-0.20230607.2310/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230607.2310/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0     2721 2023-06-06 09:07:19.000000 krutils-0.20230607.2310/krutils/futils.py
--rw-rw-rw-   0        0        0    12556 2023-06-06 16:39:50.000000 krutils-0.20230607.2310/krutils/logger.py
--rw-rw-rw-   0        0        0      669 2023-06-06 17:38:05.000000 krutils-0.20230607.2310/krutils/logger2.py
--rw-rw-rw-   0        0        0    18583 2023-06-07 14:10:35.000000 krutils-0.20230607.2310/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:10:40.563510 krutils-0.20230607.2310/krutils.egg-info/
--rw-rw-rw-   0        0        0      526 2023-06-07 14:10:40.000000 krutils-0.20230607.2310/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-07 14:10:40.000000 krutils-0.20230607.2310/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:10:40.000000 krutils-0.20230607.2310/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-07 14:10:40.000000 krutils-0.20230607.2310/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 14:10:40.000000 krutils-0.20230607.2310/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 14:10:40.578624 krutils-0.20230607.2310/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-06-07 14:10:38.000000 krutils-0.20230607.2310/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:10:40.571921 krutils-0.20230607.2310/test/
--rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230607.2310/test/test_futils.py
--rw-rw-rw-   0        0        0      235 2023-06-07 13:45:35.000000 krutils-0.20230607.2310/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:23:32.339423 krutils-0.20230607.2323/
+-rw-rw-rw-   0        0        0      526 2023-06-07 14:23:32.330326 krutils-0.20230607.2323/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230607.2323/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 14:23:32.249174 krutils-0.20230607.2323/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230607.2323/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230607.2323/krutils/CONST.py
+-rw-rw-rw-   0        0        0       94 2023-06-06 15:37:21.000000 krutils-0.20230607.2323/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230607.2323/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0     2721 2023-06-06 09:07:19.000000 krutils-0.20230607.2323/krutils/futils.py
+-rw-rw-rw-   0        0        0    12556 2023-06-06 16:39:50.000000 krutils-0.20230607.2323/krutils/logger.py
+-rw-rw-rw-   0        0        0      669 2023-06-06 17:38:05.000000 krutils-0.20230607.2323/krutils/logger2.py
+-rw-rw-rw-   0        0        0    18188 2023-06-07 14:23:27.000000 krutils-0.20230607.2323/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:23:32.300323 krutils-0.20230607.2323/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-06-07 14:23:31.000000 krutils-0.20230607.2323/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-07 14:23:32.000000 krutils-0.20230607.2323/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:23:31.000000 krutils-0.20230607.2323/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-07 14:23:31.000000 krutils-0.20230607.2323/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 14:23:31.000000 krutils-0.20230607.2323/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:23:32.340349 krutils-0.20230607.2323/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-06-07 14:23:30.000000 krutils-0.20230607.2323/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:23:32.319668 krutils-0.20230607.2323/test/
+-rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230607.2323/test/test_futils.py
+-rw-rw-rw-   0        0        0      235 2023-06-07 13:45:35.000000 krutils-0.20230607.2323/test/test_logger.py
```

### Comparing `krutils-0.20230607.2310/PKG-INFO` & `krutils-0.20230607.2323/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230607.2310
+Version: 0.20230607.2323
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230607.2310/krutils/CONST.py` & `krutils-0.20230607.2323/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.2310/krutils/_dbmgr.py` & `krutils-0.20230607.2323/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.2310/krutils/futils.py` & `krutils-0.20230607.2323/krutils/futils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.2310/krutils/logger.py` & `krutils-0.20230607.2323/krutils/logger.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.2310/krutils/logger2.py` & `krutils-0.20230607.2323/krutils/logger2.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.2310/krutils/utils.py` & `krutils-0.20230607.2323/krutils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -681,36 +681,14 @@
 # }
 
 
 
 
 
 
-##########################################
-##      LOGGING
-##########################################
-def logger(____file__):
-    '''krutils.logger() 참고 '''
-
-    caller_path = ____file__
-
-    if is_empty(caller_path) == True:
-        caller_path = __file__
-
-    # from krutils import logger as lgr
-    import logger as lgr
-    return lgr.getlogger(caller_path)
-
-
-
-
-
-
-
-
```

### Comparing `krutils-0.20230607.2310/krutils.egg-info/PKG-INFO` & `krutils-0.20230607.2323/krutils.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230607.2310
+Version: 0.20230607.2323
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230607.2310/setup.py` & `krutils-0.20230607.2323/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230607.2310",
+    version="0.20230607.2323",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```

