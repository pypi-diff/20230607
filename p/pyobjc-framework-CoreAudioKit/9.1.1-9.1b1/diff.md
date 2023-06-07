# Comparing `tmp/pyobjc-framework-CoreAudioKit-9.1.1.tar.gz` & `tmp/pyobjc-framework-CoreAudioKit-9.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreAudioKit-9.1.1.tar", last modified: Tue Apr 18 07:23:14 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreAudioKit-9.1b1.tar", last modified: Sun Mar 26 11:19:38 2023, max compression
```

## Comparing `pyobjc-framework-CoreAudioKit-9.1.1.tar` & `pyobjc-framework-CoreAudioKit-9.1b1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:23:14.176549 pyobjc-framework-CoreAudioKit-9.1.1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:23:14.104953 pyobjc-framework-CoreAudioKit-9.1.1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:23:14.116346 pyobjc-framework-CoreAudioKit-9.1.1/Lib/CoreAudioKit/
--rw-r--r--   0 ronald     (501) staff       (20)      740 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/Lib/CoreAudioKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2363 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1.1/Lib/CoreAudioKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:23:14.130548 pyobjc-framework-CoreAudioKit-9.1.1/Lib/pyobjc_framework_CoreAudioKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2110 2023-04-18 07:23:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/Lib/pyobjc_framework_CoreAudioKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1015 2023-04-18 07:23:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/Lib/pyobjc_framework_CoreAudioKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-04-18 07:23:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/Lib/pyobjc_framework_CoreAudioKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:41.000000 pyobjc-framework-CoreAudioKit-9.1.1/Lib/pyobjc_framework_CoreAudioKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       83 2023-04-18 07:23:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/Lib/pyobjc_framework_CoreAudioKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-04-18 07:23:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/Lib/pyobjc_framework_CoreAudioKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreAudioKit-9.1.1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:23:14.132854 pyobjc-framework-CoreAudioKit-9.1.1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      835 2021-10-18 19:38:40.000000 pyobjc-framework-CoreAudioKit-9.1.1/Modules/_CoreAudioKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      192 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/Modules/_CoreAudioKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreAudioKit-9.1.1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12944 2023-04-15 08:26:49.000000 pyobjc-framework-CoreAudioKit-9.1.1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1899 2023-04-18 07:23:14.176162 pyobjc-framework-CoreAudioKit-9.1.1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:23:14.135907 pyobjc-framework-CoreAudioKit-9.1.1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      222 2022-06-25 20:07:08.000000 pyobjc-framework-CoreAudioKit-9.1.1/PyObjCTest/test_aucustomviewpersistentdata.py
--rw-r--r--   0 ronald     (501) staff       (20)      649 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1.1/PyObjCTest/test_augenericview.py
--rw-r--r--   0 ronald     (501) staff       (20)      596 2021-03-21 10:08:22.000000 pyobjc-framework-CoreAudioKit-9.1.1/PyObjCTest/test_auviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/PyObjCTest/test_canetworkbrowserwindowcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-CoreAudioKit-9.1.1/PyObjCTest/test_coreaudiokit.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:23:14.141397 pyobjc-framework-CoreAudioKit-9.1.1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1456 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/metadata/CoreAudioKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:23:14.175563 pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     9033 2021-07-30 09:00:37.000000 pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9110 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8821 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9034 2021-03-21 10:08:22.000000 pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9034 2021-07-30 09:00:37.000000 pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9111 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreAudioKit-9.1.1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-04-18 07:23:14.176654 pyobjc-framework-CoreAudioKit-9.1.1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1369 2023-04-17 07:57:59.000000 pyobjc-framework-CoreAudioKit-9.1.1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.705790 pyobjc-framework-CoreAudioKit-9.1b1/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.598741 pyobjc-framework-CoreAudioKit-9.1b1/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.645573 pyobjc-framework-CoreAudioKit-9.1b1/Lib/CoreAudioKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      740 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/CoreAudioKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2363 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/CoreAudioKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.655877 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2110 2023-03-26 11:19:38.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1015 2023-03-26 11:19:38.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:19:38.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:41.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       83 2023-03-26 11:19:38.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:19:38.000000 pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreAudioKit-9.1b1/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.671203 pyobjc-framework-CoreAudioKit-9.1b1/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      835 2021-10-18 19:38:40.000000 pyobjc-framework-CoreAudioKit-9.1b1/Modules/_CoreAudioKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      192 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/Modules/_CoreAudioKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreAudioKit-9.1b1/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreAudioKit-9.1b1/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1899 2023-03-26 11:19:38.705281 pyobjc-framework-CoreAudioKit-9.1b1/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.690986 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      222 2022-06-25 20:07:08.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_aucustomviewpersistentdata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      649 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_augenericview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      596 2021-03-21 10:08:22.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_auviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_canetworkbrowserwindowcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_coreaudiokit.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.693392 pyobjc-framework-CoreAudioKit-9.1b1/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1456 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/CoreAudioKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:19:38.703688 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     9033 2021-07-30 09:00:37.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9110 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8821 2020-11-30 18:45:14.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9034 2021-03-21 10:08:22.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9034 2021-07-30 09:00:37.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9111 2022-02-24 08:47:16.000000 pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreAudioKit-9.1b1/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:19:38.705903 pyobjc-framework-CoreAudioKit-9.1b1/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1369 2023-03-25 14:20:30.000000 pyobjc-framework-CoreAudioKit-9.1b1/setup.py
```

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/Lib/CoreAudioKit/__init__.py` & `pyobjc-framework-CoreAudioKit-9.1b1/Lib/CoreAudioKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/Lib/CoreAudioKit/_metadata.py` & `pyobjc-framework-CoreAudioKit-9.1b1/Lib/CoreAudioKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/Lib/pyobjc_framework_CoreAudioKit.egg-info/PKG-INFO` & `pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreAudioKit
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework CoreAudioKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreAudioKit
 Platform: MacOS X
```

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/Lib/pyobjc_framework_CoreAudioKit.egg-info/SOURCES.txt` & `pyobjc-framework-CoreAudioKit-9.1b1/Lib/pyobjc_framework_CoreAudioKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/License.txt` & `pyobjc-framework-CoreAudioKit-9.1b1/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/Modules/_CoreAudioKit.m` & `pyobjc-framework-CoreAudioKit-9.1b1/Modules/_CoreAudioKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreAudioKit-9.1b1/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreAudioKit-9.1b1/Modules/pyobjc-compat.h`

 * *Files 1% similar despite different names*

```diff
@@ -301,18 +301,14 @@
 #define MAC_OS_X_VERSION_13_2 130200
 #endif
 
 #ifndef MAC_OS_X_VERSION_13_3
 #define MAC_OS_X_VERSION_13_3 130300
 #endif
 
-#ifndef MAC_OS_X_VERSION_13_4
-#define MAC_OS_X_VERSION_13_4 130400
-#endif
-
 /*
  *
  * End of Cocoa definitions
  *
  */
 
 /*
```

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/PKG-INFO` & `pyobjc-framework-CoreAudioKit-9.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreAudioKit
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework CoreAudioKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreAudioKit
 Platform: MacOS X
```

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/PyObjCTest/test_augenericview.py` & `pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_augenericview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/PyObjCTest/test_auviewcontroller.py` & `pyobjc-framework-CoreAudioKit-9.1b1/PyObjCTest/test_auviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/metadata/CoreAudioKit.fwinfo` & `pyobjc-framework-CoreAudioKit-9.1b1/metadata/CoreAudioKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreAudioKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/pyobjc_setup.py` & `pyobjc-framework-CoreAudioKit-9.1b1/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreAudioKit-9.1.1/setup.py` & `pyobjc-framework-CoreAudioKit-9.1b1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Distutils doesn't understand '.mm' as an extension
 #
 import distutils.unixccompiler
 import os
 
 from pyobjc_setup import Extension, setup
 
-VERSION = "9.1.1"
+VERSION = "9.1b1"
 
 
 distutils.unixccompiler.UnixCCompiler.src_extensions.append(".mm")
 
 setup(
     name="pyobjc-framework-CoreAudioKit",
     description="Wrappers for the framework CoreAudioKit on macOS",
```

