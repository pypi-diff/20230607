# Comparing `tmp/pyobjc-framework-EventKit-9.1.1.tar.gz` & `tmp/pyobjc-framework-EventKit-9.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-EventKit-9.1.1.tar", last modified: Tue Apr 18 07:27:05 2023, max compression
+gzip compressed data, was "pyobjc-framework-EventKit-9.1b1.tar", last modified: Sun Mar 26 11:23:37 2023, max compression
```

## Comparing `pyobjc-framework-EventKit-9.1.1.tar` & `pyobjc-framework-EventKit-9.1b1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:27:05.306617 pyobjc-framework-EventKit-9.1.1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-EventKit-9.1.1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:27:05.239400 pyobjc-framework-EventKit-9.1.1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:27:05.243620 pyobjc-framework-EventKit-9.1.1/Lib/EventKit/
--rw-r--r--   0 ronald     (501) staff       (20)      693 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1.1/Lib/EventKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    11435 2022-06-15 11:57:00.000000 pyobjc-framework-EventKit-9.1.1/Lib/EventKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:27:05.246342 pyobjc-framework-EventKit-9.1.1/Lib/pyobjc_framework_EventKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2129 2023-04-18 07:27:05.000000 pyobjc-framework-EventKit-9.1.1/Lib/pyobjc_framework_EventKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1250 2023-04-18 07:27:05.000000 pyobjc-framework-EventKit-9.1.1/Lib/pyobjc_framework_EventKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-04-18 07:27:05.000000 pyobjc-framework-EventKit-9.1.1/Lib/pyobjc_framework_EventKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:02.000000 pyobjc-framework-EventKit-9.1.1/Lib/pyobjc_framework_EventKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-04-18 07:27:05.000000 pyobjc-framework-EventKit-9.1.1/Lib/pyobjc_framework_EventKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-04-18 07:27:05.000000 pyobjc-framework-EventKit-9.1.1/Lib/pyobjc_framework_EventKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1.1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1918 2023-04-18 07:27:05.306290 pyobjc-framework-EventKit-9.1.1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:27:05.271146 pyobjc-framework-EventKit-9.1.1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      677 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekalarm.py
--rw-r--r--   0 ronald     (501) staff       (20)     1234 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekcalendar.py
--rw-r--r--   0 ronald     (501) staff       (20)      563 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekcalendaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)     2944 2022-06-15 11:57:00.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekerror.py
--rw-r--r--   0 ronald     (501) staff       (20)     1223 2022-02-24 08:47:16.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekevent.py
--rw-r--r--   0 ronald     (501) staff       (20)     3359 2022-02-24 08:47:16.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekeventstore.py
--rw-r--r--   0 ronald     (501) staff       (20)      448 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekobject.py
--rw-r--r--   0 ronald     (501) staff       (20)     1575 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekparticipant.py
--rw-r--r--   0 ronald     (501) staff       (20)      891 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekrecurrencerule.py
--rw-r--r--   0 ronald     (501) staff       (20)      682 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekreminder.py
--rw-r--r--   0 ronald     (501) staff       (20)     1067 2022-06-15 11:57:00.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_eksource.py
--rw-r--r--   0 ronald     (501) staff       (20)     6451 2022-02-24 08:47:16.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ektypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      536 2021-07-30 09:00:37.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekvirtualconferenceprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_eventkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      309 2021-10-18 19:38:40.000000 pyobjc-framework-EventKit-9.1.1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:27:05.272453 pyobjc-framework-EventKit-9.1.1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     3986 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1.1/metadata/EventKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1.1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-04-18 07:27:05.304877 pyobjc-framework-EventKit-9.1.1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    80431 2021-07-30 09:00:37.000000 pyobjc-framework-EventKit-9.1.1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    81347 2022-02-24 08:47:16.000000 pyobjc-framework-EventKit-9.1.1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    82940 2022-06-15 11:57:00.000000 pyobjc-framework-EventKit-9.1.1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    64684 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    72253 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    73106 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    37403 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    80432 2021-07-30 09:00:37.000000 pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    81348 2022-02-24 08:47:16.000000 pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    82941 2022-06-15 11:57:00.000000 pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-EventKit-9.1.1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-04-18 07:27:05.306714 pyobjc-framework-EventKit-9.1.1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      660 2023-04-17 07:57:59.000000 pyobjc-framework-EventKit-9.1.1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:37.152015 pyobjc-framework-EventKit-9.1b1/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-EventKit-9.1b1/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:37.106054 pyobjc-framework-EventKit-9.1b1/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:37.113244 pyobjc-framework-EventKit-9.1b1/Lib/EventKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      693 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1b1/Lib/EventKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11435 2022-06-15 11:57:00.000000 pyobjc-framework-EventKit-9.1b1/Lib/EventKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:37.116546 pyobjc-framework-EventKit-9.1b1/Lib/pyobjc_framework_EventKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2129 2023-03-26 11:23:37.000000 pyobjc-framework-EventKit-9.1b1/Lib/pyobjc_framework_EventKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1250 2023-03-26 11:23:37.000000 pyobjc-framework-EventKit-9.1b1/Lib/pyobjc_framework_EventKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:23:37.000000 pyobjc-framework-EventKit-9.1b1/Lib/pyobjc_framework_EventKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:02.000000 pyobjc-framework-EventKit-9.1b1/Lib/pyobjc_framework_EventKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:23:37.000000 pyobjc-framework-EventKit-9.1b1/Lib/pyobjc_framework_EventKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:23:37.000000 pyobjc-framework-EventKit-9.1b1/Lib/pyobjc_framework_EventKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1b1/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1918 2023-03-26 11:23:37.151531 pyobjc-framework-EventKit-9.1b1/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:37.129984 pyobjc-framework-EventKit-9.1b1/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      677 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekalarm.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1234 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekcalendar.py
+-rw-r--r--   0 ronald     (501) staff       (20)      563 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekcalendaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2944 2022-06-15 11:57:00.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1223 2022-02-24 08:47:16.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3359 2022-02-24 08:47:16.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekeventstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      448 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1575 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekparticipant.py
+-rw-r--r--   0 ronald     (501) staff       (20)      891 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekrecurrencerule.py
+-rw-r--r--   0 ronald     (501) staff       (20)      682 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekreminder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1067 2022-06-15 11:57:00.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_eksource.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6451 2022-02-24 08:47:16.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ektypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      536 2021-07-30 09:00:37.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekvirtualconferenceprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_eventkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      309 2021-10-18 19:38:40.000000 pyobjc-framework-EventKit-9.1b1/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:37.131229 pyobjc-framework-EventKit-9.1b1/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     3986 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1b1/metadata/EventKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1b1/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:37.149575 pyobjc-framework-EventKit-9.1b1/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    80431 2021-07-30 09:00:37.000000 pyobjc-framework-EventKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    81347 2022-02-24 08:47:16.000000 pyobjc-framework-EventKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    82940 2022-06-15 11:57:00.000000 pyobjc-framework-EventKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    64684 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    72253 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    73106 2021-03-21 10:08:22.000000 pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    37403 2020-11-30 18:45:14.000000 pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    80432 2021-07-30 09:00:37.000000 pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    81348 2022-02-24 08:47:16.000000 pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    82941 2022-06-15 11:57:00.000000 pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-EventKit-9.1b1/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:23:37.152123 pyobjc-framework-EventKit-9.1b1/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      660 2023-03-25 14:20:31.000000 pyobjc-framework-EventKit-9.1b1/setup.py
```

### Comparing `pyobjc-framework-EventKit-9.1.1/LICENSE.txt` & `pyobjc-framework-EventKit-9.1b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/Lib/EventKit/__init__.py` & `pyobjc-framework-EventKit-9.1b1/Lib/EventKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/Lib/EventKit/_metadata.py` & `pyobjc-framework-EventKit-9.1b1/Lib/EventKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/Lib/pyobjc_framework_EventKit.egg-info/PKG-INFO` & `pyobjc-framework-EventKit-9.1b1/Lib/pyobjc_framework_EventKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-EventKit
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework Accounts on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,EventKit
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-EventKit-9.1.1/Lib/pyobjc_framework_EventKit.egg-info/SOURCES.txt` & `pyobjc-framework-EventKit-9.1b1/Lib/pyobjc_framework_EventKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PKG-INFO` & `pyobjc-framework-EventKit-9.1b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-EventKit
-Version: 9.1.1
+Version: 9.1b1
 Summary: Wrappers for the framework Accounts on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,EventKit
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekalarm.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekalarm.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekcalendar.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekcalendar.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekcalendaritem.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekcalendaritem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekerror.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekevent.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekeventstore.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekeventstore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekparticipant.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekparticipant.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekrecurrencerule.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekrecurrencerule.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekreminder.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekreminder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_eksource.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_eksource.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ektypes.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ektypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/PyObjCTest/test_ekvirtualconferenceprovider.py` & `pyobjc-framework-EventKit-9.1b1/PyObjCTest/test_ekvirtualconferenceprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/metadata/EventKit.fwinfo` & `pyobjc-framework-EventKit-9.1b1/metadata/EventKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-EventKit-9.1b1/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-EventKit-9.1b1/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-EventKit-9.1b1/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-EventKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/pyobjc_setup.py` & `pyobjc-framework-EventKit-9.1b1/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-EventKit-9.1.1/setup.py` & `pyobjc-framework-EventKit-9.1b1/setup.py`

 * *Files 17% similar despite different names*

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
     name="pyobjc-framework-EventKit",
     description="Wrappers for the framework Accounts on macOS",
     min_os_level="10.8",
     packages=["EventKit"],
     version=VERSION,
```

