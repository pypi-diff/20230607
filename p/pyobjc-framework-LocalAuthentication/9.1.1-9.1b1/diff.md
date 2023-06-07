# Comparing `tmp/pyobjc-framework-LocalAuthentication-9.1.1.tar.gz` & `tmp/pyobjc-framework-LocalAuthentication-9.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-LocalAuthentication-9.1.1.tar", last modified: Tue Apr 18 07:31:56 2023, max compression
+gzip compressed data, was "pyobjc-framework-LocalAuthentication-9.1b1.tar", last modified: Sun Mar 26 11:28:13 2023, max compression
```

## Comparing `pyobjc-framework-LocalAuthentication-9.1.1.tar` & `pyobjc-framework-LocalAuthentication-9.1b1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:56.124880 pyobjc-framework-LocalAuthentication-9.1.1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LocalAuthentication-9.1.1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:56.090510 pyobjc-framework-LocalAuthentication-9.1.1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:56.094861 pyobjc-framework-LocalAuthentication-9.1.1/Lib/LocalAuthentication/
--rw-r--r--   0 ronald     (501) staff       (20)      754 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1.1/Lib/LocalAuthentication/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    13511 2022-07-08 16:02:54.000000 pyobjc-framework-LocalAuthentication-9.1.1/Lib/LocalAuthentication/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:56.097601 pyobjc-framework-LocalAuthentication-9.1.1/Lib/pyobjc_framework_LocalAuthentication.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2174 2023-04-18 07:31:56.000000 pyobjc-framework-LocalAuthentication-9.1.1/Lib/pyobjc_framework_LocalAuthentication.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1163 2023-04-18 07:31:56.000000 pyobjc-framework-LocalAuthentication-9.1.1/Lib/pyobjc_framework_LocalAuthentication.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-04-18 07:31:56.000000 pyobjc-framework-LocalAuthentication-9.1.1/Lib/pyobjc_framework_LocalAuthentication.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:25.000000 pyobjc-framework-LocalAuthentication-9.1.1/Lib/pyobjc_framework_LocalAuthentication.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       82 2023-04-18 07:31:56.000000 pyobjc-framework-LocalAuthentication-9.1.1/Lib/pyobjc_framework_LocalAuthentication.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       20 2023-04-18 07:31:56.000000 pyobjc-framework-LocalAuthentication-9.1.1/Lib/pyobjc_framework_LocalAuthentication.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1.1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1963 2023-04-18 07:31:56.124465 pyobjc-framework-LocalAuthentication-9.1.1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:56.115529 pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     5435 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_lacontext.py
--rw-r--r--   0 ronald     (501) staff       (20)     3091 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_laerror.py
--rw-r--r--   0 ronald     (501) staff       (20)     1056 2022-06-27 12:41:12.000000 pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_laprivatekey.py
--rw-r--r--   0 ronald     (501) staff       (20)     3018 2022-06-15 11:57:00.000000 pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_lapublicdefines.py
--rw-r--r--   0 ronald     (501) staff       (20)      869 2022-06-27 11:34:54.000000 pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_lapublickey.py
--rw-r--r--   0 ronald     (501) staff       (20)      957 2022-07-08 16:02:54.000000 pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_laright.py
--rw-r--r--   0 ronald     (501) staff       (20)     1005 2022-06-15 11:57:00.000000 pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_larightstore.py
--rw-r--r--   0 ronald     (501) staff       (20)      293 2022-06-15 11:57:00.000000 pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_lasecret.py
--rw-r--r--   0 ronald     (501) staff       (20)      222 2022-04-11 08:03:15.000000 pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_localauthentication.py
--rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-LocalAuthentication-9.1.1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:56.116797 pyobjc-framework-LocalAuthentication-9.1.1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     4332 2022-07-08 16:02:54.000000 pyobjc-framework-LocalAuthentication-9.1.1/metadata/LocalAuthentication.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       54 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1.1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:56.123244 pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    11257 2021-08-04 10:01:04.000000 pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11502 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    33053 2022-07-08 16:02:54.000000 pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     3188 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10364 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11033 2021-03-21 10:08:22.000000 pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11258 2021-08-04 10:01:04.000000 pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    11503 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    33054 2022-07-08 16:02:54.000000 pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LocalAuthentication-9.1.1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-04-18 07:31:56.124992 pyobjc-framework-LocalAuthentication-9.1.1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      777 2023-04-17 07:58:00.000000 pyobjc-framework-LocalAuthentication-9.1.1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:13.505479 pyobjc-framework-LocalAuthentication-9.1b1/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LocalAuthentication-9.1b1/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:13.452473 pyobjc-framework-LocalAuthentication-9.1b1/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:13.460902 pyobjc-framework-LocalAuthentication-9.1b1/Lib/LocalAuthentication/
+-rw-r--r--   0 ronald     (501) staff       (20)      754 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1b1/Lib/LocalAuthentication/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13511 2022-07-08 16:02:54.000000 pyobjc-framework-LocalAuthentication-9.1b1/Lib/LocalAuthentication/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:13.469150 pyobjc-framework-LocalAuthentication-9.1b1/Lib/pyobjc_framework_LocalAuthentication.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2174 2023-03-26 11:28:13.000000 pyobjc-framework-LocalAuthentication-9.1b1/Lib/pyobjc_framework_LocalAuthentication.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1163 2023-03-26 11:28:13.000000 pyobjc-framework-LocalAuthentication-9.1b1/Lib/pyobjc_framework_LocalAuthentication.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:28:13.000000 pyobjc-framework-LocalAuthentication-9.1b1/Lib/pyobjc_framework_LocalAuthentication.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:25.000000 pyobjc-framework-LocalAuthentication-9.1b1/Lib/pyobjc_framework_LocalAuthentication.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       82 2023-03-26 11:28:13.000000 pyobjc-framework-LocalAuthentication-9.1b1/Lib/pyobjc_framework_LocalAuthentication.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       20 2023-03-26 11:28:13.000000 pyobjc-framework-LocalAuthentication-9.1b1/Lib/pyobjc_framework_LocalAuthentication.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1b1/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1963 2023-03-26 11:28:13.505156 pyobjc-framework-LocalAuthentication-9.1b1/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:13.480343 pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5435 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_lacontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3091 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_laerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1056 2022-06-27 12:41:12.000000 pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_laprivatekey.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3018 2022-06-15 11:57:00.000000 pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_lapublicdefines.py
+-rw-r--r--   0 ronald     (501) staff       (20)      869 2022-06-27 11:34:54.000000 pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_lapublickey.py
+-rw-r--r--   0 ronald     (501) staff       (20)      957 2022-07-08 16:02:54.000000 pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_laright.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1005 2022-06-15 11:57:00.000000 pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_larightstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      293 2022-06-15 11:57:00.000000 pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_lasecret.py
+-rw-r--r--   0 ronald     (501) staff       (20)      222 2022-04-11 08:03:15.000000 pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_localauthentication.py
+-rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-LocalAuthentication-9.1b1/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:13.482776 pyobjc-framework-LocalAuthentication-9.1b1/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     4332 2022-07-08 16:02:54.000000 pyobjc-framework-LocalAuthentication-9.1b1/metadata/LocalAuthentication.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       54 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1b1/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:13.503788 pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    11257 2021-08-04 10:01:04.000000 pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11502 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    33053 2022-07-08 16:02:54.000000 pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     3188 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10364 2020-11-30 18:45:15.000000 pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11033 2021-03-21 10:08:22.000000 pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11258 2021-08-04 10:01:04.000000 pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    11503 2022-02-24 08:47:16.000000 pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    33054 2022-07-08 16:02:54.000000 pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LocalAuthentication-9.1b1/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:13.505577 pyobjc-framework-LocalAuthentication-9.1b1/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      777 2023-03-25 14:20:31.000000 pyobjc-framework-LocalAuthentication-9.1b1/setup.py
```

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/LICENSE.txt` & `pyobjc-framework-LocalAuthentication-9.1b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/Lib/LocalAuthentication/__init__.py` & `pyobjc-framework-LocalAuthentication-9.1b1/Lib/LocalAuthentication/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/Lib/LocalAuthentication/_metadata.py` & `pyobjc-framework-LocalAuthentication-9.1b1/Lib/LocalAuthentication/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/Lib/pyobjc_framework_LocalAuthentication.egg-info/PKG-INFO` & `pyobjc-framework-LocalAuthentication-9.1b1/Lib/pyobjc_framework_LocalAuthentication.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LocalAuthentication
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework LocalAuthentication on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LocalAuthentication
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/Lib/pyobjc_framework_LocalAuthentication.egg-info/SOURCES.txt` & `pyobjc-framework-LocalAuthentication-9.1b1/Lib/pyobjc_framework_LocalAuthentication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/PKG-INFO` & `pyobjc-framework-LocalAuthentication-9.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LocalAuthentication
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework LocalAuthentication on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LocalAuthentication
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_lacontext.py` & `pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_lacontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_laerror.py` & `pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_laerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_laprivatekey.py` & `pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_laprivatekey.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_lapublicdefines.py` & `pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_lapublicdefines.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_lapublickey.py` & `pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_lapublickey.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_laright.py` & `pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_laright.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/PyObjCTest/test_larightstore.py` & `pyobjc-framework-LocalAuthentication-9.1b1/PyObjCTest/test_larightstore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/metadata/LocalAuthentication.fwinfo` & `pyobjc-framework-LocalAuthentication-9.1b1/metadata/LocalAuthentication.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-LocalAuthentication-9.1b1/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/pyobjc_setup.py` & `pyobjc-framework-LocalAuthentication-9.1b1/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LocalAuthentication-9.1.1/setup.py` & `pyobjc-framework-LocalAuthentication-9.1b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
 from pyobjc_setup import setup
 
-VERSION = "9.1.1"
+VERSION = "9.1b1"
 
 setup(
     name="pyobjc-framework-LocalAuthentication",
     description="Wrappers for the framework LocalAuthentication on macOS",
     min_os_level="10.10",
     packages=["LocalAuthentication"],
     version=VERSION,
```

