# Comparing `tmp/krutils-0.20230522.1625.tar.gz` & `tmp/krutils-0.20230607.2237.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230522.1625.tar", last modified: Mon May 22 07:25:33 2023, max compression
+gzip compressed data, was "krutils-0.20230607.2237.tar", last modified: Wed Jun  7 13:37:32 2023, max compression
```

## Comparing `krutils-0.20230522.1625.tar` & `krutils-0.20230607.2237.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 07:25:33.369859 krutils-0.20230522.1625/
--rw-rw-rw-   0        0        0      526 2023-05-22 07:25:33.367850 krutils-0.20230522.1625/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230522.1625/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 07:25:33.278424 krutils-0.20230522.1625/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230522.1625/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230522.1625/krutils/CONST.py
--rw-rw-rw-   0        0        0       94 2023-05-22 07:06:16.000000 krutils-0.20230522.1625/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230522.1625/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0     2704 2023-05-22 07:25:24.000000 krutils-0.20230522.1625/krutils/futils.py
--rw-rw-rw-   0        0        0    12553 2023-05-22 05:02:22.000000 krutils-0.20230522.1625/krutils/logger.py
--rw-rw-rw-   0        0        0    18549 2023-05-22 06:46:23.000000 krutils-0.20230522.1625/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 07:25:33.337909 krutils-0.20230522.1625/krutils.egg-info/
--rw-rw-rw-   0        0        0      526 2023-05-22 07:25:32.000000 krutils-0.20230522.1625/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-05-22 07:25:33.000000 krutils-0.20230522.1625/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 07:25:32.000000 krutils-0.20230522.1625/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-22 07:25:33.000000 krutils-0.20230522.1625/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 07:25:33.000000 krutils-0.20230522.1625/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 07:25:33.370187 krutils-0.20230522.1625/setup.cfg
--rw-rw-rw-   0        0        0      858 2023-05-22 07:25:32.000000 krutils-0.20230522.1625/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 07:25:33.364719 krutils-0.20230522.1625/test/
--rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230522.1625/test/test_futils.py
--rw-rw-rw-   0        0        0      308 2023-05-22 06:46:23.000000 krutils-0.20230522.1625/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:32.883536 krutils-0.20230607.2237/
+-rw-rw-rw-   0        0        0      526 2023-06-07 13:37:32.879955 krutils-0.20230607.2237/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230607.2237/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:32.660365 krutils-0.20230607.2237/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230607.2237/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230607.2237/krutils/CONST.py
+-rw-rw-rw-   0        0        0       94 2023-06-06 15:37:21.000000 krutils-0.20230607.2237/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230607.2237/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0     2721 2023-06-06 09:07:19.000000 krutils-0.20230607.2237/krutils/futils.py
+-rw-rw-rw-   0        0        0    12556 2023-06-06 16:39:50.000000 krutils-0.20230607.2237/krutils/logger.py
+-rw-rw-rw-   0        0        0      669 2023-06-06 17:38:05.000000 krutils-0.20230607.2237/krutils/logger2.py
+-rw-rw-rw-   0        0        0    18583 2023-06-07 13:37:04.000000 krutils-0.20230607.2237/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:32.809781 krutils-0.20230607.2237/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-06-07 13:37:32.000000 krutils-0.20230607.2237/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-07 13:37:32.000000 krutils-0.20230607.2237/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 13:37:32.000000 krutils-0.20230607.2237/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-07 13:37:32.000000 krutils-0.20230607.2237/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 13:37:32.000000 krutils-0.20230607.2237/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 13:37:32.883536 krutils-0.20230607.2237/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-06-07 13:37:30.000000 krutils-0.20230607.2237/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:32.876731 krutils-0.20230607.2237/test/
+-rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230607.2237/test/test_futils.py
+-rw-rw-rw-   0        0        0      370 2023-06-07 13:32:53.000000 krutils-0.20230607.2237/test/test_logger.py
```

### Comparing `krutils-0.20230522.1625/PKG-INFO` & `krutils-0.20230607.2237/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1625
+Version: 0.20230607.2237
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1625/krutils/CONST.py` & `krutils-0.20230607.2237/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1625/krutils/_dbmgr.py` & `krutils-0.20230607.2237/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1625/krutils/futils.py` & `krutils-0.20230607.2237/krutils/futils.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     data_file_path = get_file_path_fr(file_name)
 
     if (data_file_path == None):
         raise Exception('지정한 파일을 찾을 수 없습니다 [{0}]'.format(file_name))
 
     import json
-    with open(data_file_path) as df:
+    with open(data_file_path, encoding='UTF8') as df:
         json_data = json.load(df)
 
     return json_data
```

### Comparing `krutils-0.20230522.1625/krutils/logger.py` & `krutils-0.20230607.2237/krutils/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
             pass
 
 
 
 ######################
 # logger 클래스 메인
 #   1. 설정파일을 찾아 적용한다. 없으면 기본값으로 적용한다.
-class logger(_logging):
+class getlogger(_logging):
     '''
     My favorite log format maker.
     [LEVEL] [TIME] [SOURCE] contents...
 
     sample>
         logger = krutils.logger(__file__)
```

### Comparing `krutils-0.20230522.1625/krutils/utils.py` & `krutils-0.20230607.2237/krutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -692,20 +692,17 @@
     '''krutils.logger() 참고 '''
 
     caller_path = ____file__
 
     if is_empty(caller_path) == True:
         caller_path = __file__
 
-    from krutils import logger
-    return logger(caller_path)
-
-
-
-
+    # from krutils import logger as lgr
+    import logger as lgr
+    return lgr.getlogger(caller_path)
```

### Comparing `krutils-0.20230522.1625/krutils.egg-info/PKG-INFO` & `krutils-0.20230607.2237/krutils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1625
+Version: 0.20230607.2237
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1625/setup.py` & `krutils-0.20230607.2237/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230522.1625",
+    version="0.20230607.2237",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
@@ -18,10 +18,11 @@
     ],
     # package_dir={"": "krutils"},
     # packages=setuptools.find_packages(where="krutils"),
     package_dir={"krutils": "krutils"},
     packages=["krutils"],
     python_requires=">=3.0",
     install_requires=[
-        "PyMySQL>=1.0.3"
+        "PyMySQL>=1.0.3",
+        'python-telegram-bot'
     ]
 )
```

