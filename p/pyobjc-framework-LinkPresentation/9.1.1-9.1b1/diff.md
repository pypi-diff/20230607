# Comparing `tmp/pyobjc-framework-LinkPresentation-9.1.1.tar.gz` & `tmp/pyobjc-framework-LinkPresentation-9.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-LinkPresentation-9.1.1.tar", last modified: Tue Apr 18 07:31:51 2023, max compression
+gzip compressed data, was "pyobjc-framework-LinkPresentation-9.1b1.tar", last modified: Sun Mar 26 11:28:08 2023, max compression
```

## Comparing `pyobjc-framework-LinkPresentation-9.1.1.tar` & `pyobjc-framework-LinkPresentation-9.1b1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:51.133955 pyobjc-framework-LinkPresentation-9.1.1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:51.111174 pyobjc-framework-LinkPresentation-9.1.1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:51.115259 pyobjc-framework-LinkPresentation-9.1.1/Lib/LinkPresentation/
--rw-r--r--   0 ronald     (501) staff       (20)      744 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1.1/Lib/LinkPresentation/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2045 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.1.1/Lib/LinkPresentation/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:51.118397 pyobjc-framework-LinkPresentation-9.1.1/Lib/pyobjc_framework_LinkPresentation.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2136 2023-04-18 07:31:51.000000 pyobjc-framework-LinkPresentation-9.1.1/Lib/pyobjc_framework_LinkPresentation.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      947 2023-04-18 07:31:51.000000 pyobjc-framework-LinkPresentation-9.1.1/Lib/pyobjc_framework_LinkPresentation.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-04-18 07:31:51.000000 pyobjc-framework-LinkPresentation-9.1.1/Lib/pyobjc_framework_LinkPresentation.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:14.000000 pyobjc-framework-LinkPresentation-9.1.1/Lib/pyobjc_framework_LinkPresentation.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-04-18 07:31:51.000000 pyobjc-framework-LinkPresentation-9.1.1/Lib/pyobjc_framework_LinkPresentation.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       17 2023-04-18 07:31:51.000000 pyobjc-framework-LinkPresentation-9.1.1/Lib/pyobjc_framework_LinkPresentation.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LinkPresentation-9.1.1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1.1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1925 2023-04-18 07:31:51.133639 pyobjc-framework-LinkPresentation-9.1.1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:51.121327 pyobjc-framework-LinkPresentation-9.1.1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1.1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      216 2022-04-11 08:03:15.000000 pyobjc-framework-LinkPresentation-9.1.1/PyObjCTest/test_linkpresentation.py
--rw-r--r--   0 ronald     (501) staff       (20)      484 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.1.1/PyObjCTest/test_lperror.py
--rw-r--r--   0 ronald     (501) staff       (20)      561 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.1.1/PyObjCTest/test_lplinkmetadata.py
--rw-r--r--   0 ronald     (501) staff       (20)      823 2021-06-10 09:09:03.000000 pyobjc-framework-LinkPresentation-9.1.1/PyObjCTest/test_lpmetadataprovider.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:51.122990 pyobjc-framework-LinkPresentation-9.1.1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      896 2021-06-10 09:09:03.000000 pyobjc-framework-LinkPresentation-9.1.1/metadata/LinkPresentation.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       48 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1.1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:31:51.132993 pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    10808 2021-07-30 09:00:38.000000 pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10871 2022-02-24 08:47:16.000000 pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10929 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     9843 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10123 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10809 2021-07-30 09:00:38.000000 pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10872 2022-02-24 08:47:16.000000 pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10930 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LinkPresentation-9.1.1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-04-18 07:31:51.134050 pyobjc-framework-LinkPresentation-9.1.1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      763 2023-04-17 07:58:00.000000 pyobjc-framework-LinkPresentation-9.1.1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.932053 pyobjc-framework-LinkPresentation-9.1b1/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.909463 pyobjc-framework-LinkPresentation-9.1b1/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.914031 pyobjc-framework-LinkPresentation-9.1b1/Lib/LinkPresentation/
+-rw-r--r--   0 ronald     (501) staff       (20)      744 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/LinkPresentation/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2045 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/LinkPresentation/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.916965 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2136 2023-03-26 11:28:08.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      947 2023-03-26 11:28:08.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:28:08.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:14.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:28:08.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-03-26 11:28:08.000000 pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-LinkPresentation-9.1b1/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1b1/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1925 2023-03-26 11:28:08.931744 pyobjc-framework-LinkPresentation-9.1b1/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.920094 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      216 2022-04-11 08:03:15.000000 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_linkpresentation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      484 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_lperror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      561 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_lplinkmetadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      823 2021-06-10 09:09:03.000000 pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_lpmetadataprovider.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.921636 pyobjc-framework-LinkPresentation-9.1b1/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      896 2021-06-10 09:09:03.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/LinkPresentation.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       48 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:08.931161 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    10808 2021-07-30 09:00:38.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10871 2022-02-24 08:47:16.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10929 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     9843 2020-11-30 18:45:15.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10123 2021-03-21 10:08:22.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10809 2021-07-30 09:00:38.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10872 2022-02-24 08:47:16.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10930 2023-02-19 10:50:35.000000 pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-LinkPresentation-9.1b1/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:08.932164 pyobjc-framework-LinkPresentation-9.1b1/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      763 2023-03-25 14:20:31.000000 pyobjc-framework-LinkPresentation-9.1b1/setup.py
```

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/Lib/LinkPresentation/__init__.py` & `pyobjc-framework-LinkPresentation-9.1b1/Lib/LinkPresentation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/Lib/LinkPresentation/_metadata.py` & `pyobjc-framework-LinkPresentation-9.1b1/Lib/LinkPresentation/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/Lib/pyobjc_framework_LinkPresentation.egg-info/PKG-INFO` & `pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LinkPresentation
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework LinkPresentation on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LinkPresentation
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/Lib/pyobjc_framework_LinkPresentation.egg-info/SOURCES.txt` & `pyobjc-framework-LinkPresentation-9.1b1/Lib/pyobjc_framework_LinkPresentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/License.txt` & `pyobjc-framework-LinkPresentation-9.1b1/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/PKG-INFO` & `pyobjc-framework-LinkPresentation-9.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-LinkPresentation
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework LinkPresentation on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,LinkPresentation
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/PyObjCTest/test_lplinkmetadata.py` & `pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_lplinkmetadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/PyObjCTest/test_lpmetadataprovider.py` & `pyobjc-framework-LinkPresentation-9.1b1/PyObjCTest/test_lpmetadataprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/metadata/LinkPresentation.fwinfo` & `pyobjc-framework-LinkPresentation-9.1b1/metadata/LinkPresentation.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-LinkPresentation-9.1b1/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/pyobjc_setup.py` & `pyobjc-framework-LinkPresentation-9.1b1/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-LinkPresentation-9.1.1/setup.py` & `pyobjc-framework-LinkPresentation-9.1b1/setup.py`

 * *Files 13% similar despite different names*

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
     name="pyobjc-framework-LinkPresentation",
     description="Wrappers for the framework LinkPresentation on macOS",
     min_os_level="10.15",
     packages=["LinkPresentation"],
     version=VERSION,
```

