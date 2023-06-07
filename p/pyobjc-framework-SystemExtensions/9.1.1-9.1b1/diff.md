# Comparing `tmp/pyobjc-framework-SystemExtensions-9.1.1.tar.gz` & `tmp/pyobjc-framework-SystemExtensions-9.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SystemExtensions-9.1.1.tar", last modified: Tue Apr 18 07:43:22 2023, max compression
+gzip compressed data, was "pyobjc-framework-SystemExtensions-9.1b1.tar", last modified: Sun Mar 26 11:42:47 2023, max compression
```

## Comparing `pyobjc-framework-SystemExtensions-9.1.1.tar` & `pyobjc-framework-SystemExtensions-9.1b1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:43:22.910997 pyobjc-framework-SystemExtensions-9.1.1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:43:22.883191 pyobjc-framework-SystemExtensions-9.1.1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:43:22.887157 pyobjc-framework-SystemExtensions-9.1.1/Lib/SystemExtensions/
--rw-r--r--   0 ronald     (501) staff       (20)      781 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1.1/Lib/SystemExtensions/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3219 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.1.1/Lib/SystemExtensions/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:43:22.890352 pyobjc-framework-SystemExtensions-9.1.1/Lib/pyobjc_framework_SystemExtensions.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2136 2023-04-18 07:43:22.000000 pyobjc-framework-SystemExtensions-9.1.1/Lib/pyobjc_framework_SystemExtensions.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      896 2023-04-18 07:43:22.000000 pyobjc-framework-SystemExtensions-9.1.1/Lib/pyobjc_framework_SystemExtensions.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-04-18 07:43:22.000000 pyobjc-framework-SystemExtensions-9.1.1/Lib/pyobjc_framework_SystemExtensions.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:53.000000 pyobjc-framework-SystemExtensions-9.1.1/Lib/pyobjc_framework_SystemExtensions.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-04-18 07:43:22.000000 pyobjc-framework-SystemExtensions-9.1.1/Lib/pyobjc_framework_SystemExtensions.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       17 2023-04-18 07:43:22.000000 pyobjc-framework-SystemExtensions-9.1.1/Lib/pyobjc_framework_SystemExtensions.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SystemExtensions-9.1.1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1.1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:43:22.892582 pyobjc-framework-SystemExtensions-9.1.1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1174 2021-10-18 19:38:40.000000 pyobjc-framework-SystemExtensions-9.1.1/Modules/_SystemExtensions.m
--rw-r--r--   0 ronald     (501) staff       (20)      298 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1.1/Modules/_SystemExtensions_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-SystemExtensions-9.1.1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12944 2023-04-15 08:26:49.000000 pyobjc-framework-SystemExtensions-9.1.1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1925 2023-04-18 07:43:22.910512 pyobjc-framework-SystemExtensions-9.1.1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:43:22.893692 pyobjc-framework-SystemExtensions-9.1.1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1.1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3446 2022-06-25 20:07:35.000000 pyobjc-framework-SystemExtensions-9.1.1/PyObjCTest/test_systemextensions.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:43:22.895033 pyobjc-framework-SystemExtensions-9.1.1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      803 2021-10-25 15:33:38.000000 pyobjc-framework-SystemExtensions-9.1.1/metadata/SystemExtensions.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       48 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1.1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:43:22.909801 pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    10275 2021-07-30 09:00:38.000000 pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10540 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8360 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8412 2021-03-21 10:08:23.000000 pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10276 2021-07-30 09:00:38.000000 pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10541 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SystemExtensions-9.1.1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-04-18 07:43:22.911093 pyobjc-framework-SystemExtensions-9.1.1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1201 2023-04-17 07:58:01.000000 pyobjc-framework-SystemExtensions-9.1.1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:47.001840 pyobjc-framework-SystemExtensions-9.1b1/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.968315 pyobjc-framework-SystemExtensions-9.1b1/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.979992 pyobjc-framework-SystemExtensions-9.1b1/Lib/SystemExtensions/
+-rw-r--r--   0 ronald     (501) staff       (20)      781 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/SystemExtensions/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3219 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/SystemExtensions/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.988848 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2136 2023-03-26 11:42:46.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      896 2023-03-26 11:42:46.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:42:46.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:53.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:42:46.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-03-26 11:42:46.000000 pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SystemExtensions-9.1b1/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.991454 pyobjc-framework-SystemExtensions-9.1b1/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1174 2021-10-18 19:38:40.000000 pyobjc-framework-SystemExtensions-9.1b1/Modules/_SystemExtensions.m
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/Modules/_SystemExtensions_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-SystemExtensions-9.1b1/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-SystemExtensions-9.1b1/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1925 2023-03-26 11:42:47.001532 pyobjc-framework-SystemExtensions-9.1b1/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.993501 pyobjc-framework-SystemExtensions-9.1b1/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3446 2022-06-25 20:07:35.000000 pyobjc-framework-SystemExtensions-9.1b1/PyObjCTest/test_systemextensions.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:46.995272 pyobjc-framework-SystemExtensions-9.1b1/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      803 2021-10-25 15:33:38.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/SystemExtensions.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       48 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:42:47.000928 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    10275 2021-07-30 09:00:38.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10540 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8360 2020-11-30 18:45:15.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8412 2021-03-21 10:08:23.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10276 2021-07-30 09:00:38.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10541 2022-02-24 08:47:17.000000 pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SystemExtensions-9.1b1/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:42:47.001936 pyobjc-framework-SystemExtensions-9.1b1/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1201 2023-03-25 14:20:32.000000 pyobjc-framework-SystemExtensions-9.1b1/setup.py
```

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/Lib/SystemExtensions/__init__.py` & `pyobjc-framework-SystemExtensions-9.1b1/Lib/SystemExtensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/Lib/SystemExtensions/_metadata.py` & `pyobjc-framework-SystemExtensions-9.1b1/Lib/SystemExtensions/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/Lib/pyobjc_framework_SystemExtensions.egg-info/PKG-INFO` & `pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SystemExtensions
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework SystemExtensions on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SystemExtensions
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/Lib/pyobjc_framework_SystemExtensions.egg-info/SOURCES.txt` & `pyobjc-framework-SystemExtensions-9.1b1/Lib/pyobjc_framework_SystemExtensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/License.txt` & `pyobjc-framework-SystemExtensions-9.1b1/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/Modules/_SystemExtensions.m` & `pyobjc-framework-SystemExtensions-9.1b1/Modules/_SystemExtensions.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/Modules/pyobjc-api.h` & `pyobjc-framework-SystemExtensions-9.1b1/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/Modules/pyobjc-compat.h` & `pyobjc-framework-SystemExtensions-9.1b1/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/PKG-INFO` & `pyobjc-framework-SystemExtensions-9.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SystemExtensions
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework SystemExtensions on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SystemExtensions
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/PyObjCTest/test_systemextensions.py` & `pyobjc-framework-SystemExtensions-9.1b1/PyObjCTest/test_systemextensions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/metadata/SystemExtensions.fwinfo` & `pyobjc-framework-SystemExtensions-9.1b1/metadata/SystemExtensions.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-SystemExtensions-9.1b1/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/pyobjc_setup.py` & `pyobjc-framework-SystemExtensions-9.1b1/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SystemExtensions-9.1.1/setup.py` & `pyobjc-framework-SystemExtensions-9.1b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 and (Objective-)C frameworks
 """
 
 import os
 
 from pyobjc_setup import Extension, setup
 
-VERSION = "9.1.1"
+VERSION = "9.1b1"
 
 setup(
     name="pyobjc-framework-SystemExtensions",
     description="Wrappers for the framework SystemExtensions on macOS",
     min_os_level="10.15",
     packages=["SystemExtensions"],
     ext_modules=[
```

