# Comparing `tmp/pyobjc-framework-AudioVideoBridging-9.1.1.tar.gz` & `tmp/pyobjc-framework-AudioVideoBridging-9.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-AudioVideoBridging-9.1.1.tar", last modified: Tue Apr 18 07:19:44 2023, max compression
+gzip compressed data, was "pyobjc-framework-AudioVideoBridging-9.1b1.tar", last modified: Sun Mar 26 11:14:50 2023, max compression
```

## Comparing `pyobjc-framework-AudioVideoBridging-9.1.1.tar` & `pyobjc-framework-AudioVideoBridging-9.1b1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:19:44.617964 pyobjc-framework-AudioVideoBridging-9.1.1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:19:44.547314 pyobjc-framework-AudioVideoBridging-9.1.1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:19:44.557859 pyobjc-framework-AudioVideoBridging-9.1.1/Lib/AudioVideoBridging/
--rw-r--r--   0 ronald     (501) staff       (20)      741 2021-07-31 09:51:58.000000 pyobjc-framework-AudioVideoBridging-9.1.1/Lib/AudioVideoBridging/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    20866 2022-10-18 09:53:23.000000 pyobjc-framework-AudioVideoBridging-9.1.1/Lib/AudioVideoBridging/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:19:44.561609 pyobjc-framework-AudioVideoBridging-9.1.1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2143 2023-04-18 07:19:44.000000 pyobjc-framework-AudioVideoBridging-9.1.1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1178 2023-04-18 07:19:44.000000 pyobjc-framework-AudioVideoBridging-9.1.1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-04-18 07:19:44.000000 pyobjc-framework-AudioVideoBridging-9.1.1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 09:24:48.000000 pyobjc-framework-AudioVideoBridging-9.1.1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-04-18 07:19:44.000000 pyobjc-framework-AudioVideoBridging-9.1.1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       19 2023-04-18 07:19:44.000000 pyobjc-framework-AudioVideoBridging-9.1.1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AudioVideoBridging-9.1.1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1.1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1932 2023-04-18 07:19:44.617291 pyobjc-framework-AudioVideoBridging-9.1.1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:19:44.574257 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       14 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      220 2022-04-11 08:03:15.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_audiovideobridging.py
--rw-r--r--   0 ronald     (501) staff       (20)     1577 2022-06-25 20:17:48.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avb17221acmpinterface.py
--rw-r--r--   0 ronald     (501) staff       (20)     1846 2022-06-25 20:15:55.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avb17221aecpinterface.py
--rw-r--r--   0 ronald     (501) staff       (20)      345 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avb17221entity.py
--rw-r--r--   0 ronald     (501) staff       (20)     1224 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avb17221entitydiscovery.py
--rw-r--r--   0 ronald     (501) staff       (20)     5424 2022-06-25 08:59:06.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avb17221entitydiscoverydelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      408 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avbcentralmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)    26182 2022-10-18 09:53:23.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avbconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)      250 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avbinterface.py
--rw-r--r--   0 ronald     (501) staff       (20)      465 2022-06-24 15:44:31.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avbipaddress.py
--rw-r--r--   0 ronald     (501) staff       (20)      544 2021-07-31 10:10:13.000000 pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avbmacaddress.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:19:44.575864 pyobjc-framework-AudioVideoBridging-9.1.1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2362 2022-06-24 15:45:30.000000 pyobjc-framework-AudioVideoBridging-9.1.1/metadata/AudioVideoBridging.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       52 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1.1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:19:44.593087 pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    80989 2021-08-14 10:34:11.000000 pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    76859 2022-02-24 08:47:16.000000 pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    86067 2022-10-18 09:53:23.000000 pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    80990 2021-08-14 10:34:11.000000 pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    76860 2022-02-24 08:47:16.000000 pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    86068 2022-10-18 09:53:23.000000 pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AudioVideoBridging-9.1.1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-04-18 07:19:44.618073 pyobjc-framework-AudioVideoBridging-9.1.1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      722 2023-04-17 07:57:58.000000 pyobjc-framework-AudioVideoBridging-9.1.1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:50.138914 pyobjc-framework-AudioVideoBridging-9.1b1/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:50.072332 pyobjc-framework-AudioVideoBridging-9.1b1/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:50.080562 pyobjc-framework-AudioVideoBridging-9.1b1/Lib/AudioVideoBridging/
+-rw-r--r--   0 ronald     (501) staff       (20)      741 2021-07-31 09:51:58.000000 pyobjc-framework-AudioVideoBridging-9.1b1/Lib/AudioVideoBridging/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    20866 2022-10-18 09:53:23.000000 pyobjc-framework-AudioVideoBridging-9.1b1/Lib/AudioVideoBridging/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:50.088803 pyobjc-framework-AudioVideoBridging-9.1b1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2143 2023-03-26 11:14:50.000000 pyobjc-framework-AudioVideoBridging-9.1b1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1178 2023-03-26 11:14:50.000000 pyobjc-framework-AudioVideoBridging-9.1b1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:14:50.000000 pyobjc-framework-AudioVideoBridging-9.1b1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2021-07-30 09:24:48.000000 pyobjc-framework-AudioVideoBridging-9.1b1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:14:50.000000 pyobjc-framework-AudioVideoBridging-9.1b1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2023-03-26 11:14:50.000000 pyobjc-framework-AudioVideoBridging-9.1b1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AudioVideoBridging-9.1b1/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1b1/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1932 2023-03-26 11:14:50.138434 pyobjc-framework-AudioVideoBridging-9.1b1/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:50.121117 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      220 2022-04-11 08:03:15.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_audiovideobridging.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1577 2022-06-25 20:17:48.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avb17221acmpinterface.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1846 2022-06-25 20:15:55.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avb17221aecpinterface.py
+-rw-r--r--   0 ronald     (501) staff       (20)      345 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avb17221entity.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1224 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avb17221entitydiscovery.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5424 2022-06-25 08:59:06.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avb17221entitydiscoverydelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      408 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avbcentralmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)    26182 2022-10-18 09:53:23.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avbconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)      250 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avbinterface.py
+-rw-r--r--   0 ronald     (501) staff       (20)      465 2022-06-24 15:44:31.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avbipaddress.py
+-rw-r--r--   0 ronald     (501) staff       (20)      544 2021-07-31 10:10:13.000000 pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avbmacaddress.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:50.123817 pyobjc-framework-AudioVideoBridging-9.1b1/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2362 2022-06-24 15:45:30.000000 pyobjc-framework-AudioVideoBridging-9.1b1/metadata/AudioVideoBridging.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       52 2021-07-30 09:00:37.000000 pyobjc-framework-AudioVideoBridging-9.1b1/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:50.136503 pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    80989 2021-08-14 10:34:11.000000 pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    76859 2022-02-24 08:47:16.000000 pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    86067 2022-10-18 09:53:23.000000 pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    80990 2021-08-14 10:34:11.000000 pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    76860 2022-02-24 08:47:16.000000 pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    86068 2022-10-18 09:53:23.000000 pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AudioVideoBridging-9.1b1/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:14:50.139024 pyobjc-framework-AudioVideoBridging-9.1b1/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      722 2023-03-25 14:20:30.000000 pyobjc-framework-AudioVideoBridging-9.1b1/setup.py
```

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/Lib/AudioVideoBridging/__init__.py` & `pyobjc-framework-AudioVideoBridging-9.1b1/Lib/AudioVideoBridging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/Lib/AudioVideoBridging/_metadata.py` & `pyobjc-framework-AudioVideoBridging-9.1b1/Lib/AudioVideoBridging/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/PKG-INFO` & `pyobjc-framework-AudioVideoBridging-9.1b1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AudioVideoBridging
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework AudioVideoBridging on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AudioVideoBridging
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/SOURCES.txt` & `pyobjc-framework-AudioVideoBridging-9.1b1/Lib/pyobjc_framework_AudioVideoBridging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/License.txt` & `pyobjc-framework-AudioVideoBridging-9.1b1/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/PKG-INFO` & `pyobjc-framework-AudioVideoBridging-9.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AudioVideoBridging
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework AudioVideoBridging on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AudioVideoBridging
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avb17221acmpinterface.py` & `pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avb17221acmpinterface.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avb17221aecpinterface.py` & `pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avb17221aecpinterface.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avb17221entitydiscovery.py` & `pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avb17221entitydiscovery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avb17221entitydiscoverydelegate.py` & `pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avb17221entitydiscoverydelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avbconstants.py` & `pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avbconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/PyObjCTest/test_avbmacaddress.py` & `pyobjc-framework-AudioVideoBridging-9.1b1/PyObjCTest/test_avbmacaddress.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/metadata/AudioVideoBridging.fwinfo` & `pyobjc-framework-AudioVideoBridging-9.1b1/metadata/AudioVideoBridging.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-AudioVideoBridging-9.1b1/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/pyobjc_setup.py` & `pyobjc-framework-AudioVideoBridging-9.1b1/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AudioVideoBridging-9.1.1/setup.py` & `pyobjc-framework-AudioVideoBridging-9.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 from pyobjc_setup import setup
 
-VERSION = "9.1.1"
+VERSION = "9.1b1"
 
 setup(
     name="pyobjc-framework-AudioVideoBridging",
     description="Wrappers for the framework AudioVideoBridging on macOS",
     min_os_level="10.8",
     packages=["AudioVideoBridging"],
     version=VERSION,
```

