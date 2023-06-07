# Comparing `tmp/openmodule_commands-11.1.0rc4.tar.gz` & `tmp/openmodule_commands-11.1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule_commands-11.1.0rc4.tar", last modified: Tue Jun  6 13:05:01 2023, max compression
+gzip compressed data, was "openmodule_commands-11.1.0rc5.tar", last modified: Wed Jun  7 07:49:39 2023, max compression
```

## Comparing `openmodule_commands-11.1.0rc4.tar` & `openmodule_commands-11.1.0rc5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 13:05:01.503665 openmodule_commands-11.1.0rc4/
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     6035 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/ChangeLog
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-06 13:05:01.503665 openmodule_commands-11.1.0rc4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-06 13:04:48.000000 openmodule_commands-11.1.0rc4/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 13:05:01.503665 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      232 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-06-06 13:05:01.503665 openmodule_commands-11.1.0rc4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-06 13:04:48.000000 openmodule_commands-11.1.0rc4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-06-06 13:04:48.000000 openmodule_commands-11.1.0rc4/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:49:39.644661 openmodule_commands-11.1.0rc5/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-07 07:49:39.000000 openmodule_commands-11.1.0rc5/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     5904 2023-06-07 07:49:39.000000 openmodule_commands-11.1.0rc5/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-07 07:49:39.644661 openmodule_commands-11.1.0rc5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-07 07:49:27.000000 openmodule_commands-11.1.0rc5/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:49:39.644661 openmodule_commands-11.1.0rc5/openmodule_commands.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-07 07:49:39.000000 openmodule_commands-11.1.0rc5/openmodule_commands.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-07 07:49:39.000000 openmodule_commands-11.1.0rc5/openmodule_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 07:49:39.000000 openmodule_commands-11.1.0rc5/openmodule_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2023-06-07 07:49:39.000000 openmodule_commands-11.1.0rc5/openmodule_commands.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 07:49:39.000000 openmodule_commands-11.1.0rc5/openmodule_commands.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-07 07:49:39.000000 openmodule_commands-11.1.0rc5/openmodule_commands.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-07 07:49:39.000000 openmodule_commands-11.1.0rc5/openmodule_commands.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-06-07 07:49:39.644661 openmodule_commands-11.1.0rc5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-07 07:49:27.000000 openmodule_commands-11.1.0rc5/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-06-07 07:49:27.000000 openmodule_commands-11.1.0rc5/translate.py
```

### Comparing `openmodule_commands-11.1.0rc4/ChangeLog` & `openmodule_commands-11.1.0rc5/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+v11.1.0.rc5
+-----------
+
+* again no language set in testing
+
 v11.1.0.rc4
 -----------
 
 * arivo-schedule in public pip
 * use temporary arivo-schedule package
 
 v11.1.0.rc3
@@ -148,23 +153,21 @@
 * known issues and migrations written
 * do not write default Legacy-0 matching scheme to disk if not existing but use StringIO instead
 * Fixed get\_gateway\_states returning an empty IoState if the given Gateway was offline for 5 seconds. Added method descriptions to all callable IoListener methods
 * Added last\_timestamp to IoState. Renamed get\_state in IoListener to get\_io\_state. it now returns an IoState with all values 0. Added is\_pin\_valid, get\_gateway\_states and is\_gateway\_valid to IoListener. Added testcases for changes/new additions
 * Added Test case for SigTERM signal
 * Added a SigTERM interrupt handler, that simply raises a KeyboardInterrupt(). The handler is set in init\_openmodule and can be told not to start by setting catch\_sigterm=False at method call. The two arguments the signal hanlder receives (signal number, frame stack) are ignored (using \*\_)
 * added raise\_handler\_errors bool to IoListener for listener.handler exceptions moved message = message.dict() to just before listener calls
-* Added OpenModuleModel as inheritance to IoState and moved it to models/io.py
 
 v8.0.1
 ------
 
 * fixed loading empty yamls fixes rpc server not logging info in debug log
 
 v8.0.0
 ------
 
 * fix in ci job
 * drop support for python 3.7
 * cleanup and docs
 * testcases for the new test method
 * better logging for rpc requests, and added a function to the test framework to receive rpc responses async
-* moved config yaml path guesser to separate function, removed GUID again because its not a great idea after all
```

### Comparing `openmodule_commands-11.1.0rc4/PKG-INFO` & `openmodule_commands-11.1.0rc5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule_commands
-Version: 11.1.0rc4
+Version: 11.1.0rc5
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.1.0rc4/__init__.py` & `openmodule_commands-11.1.0rc5/__init__.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/PKG-INFO` & `openmodule_commands-11.1.0rc5/openmodule_commands.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule-commands
-Version: 11.1.0rc4
+Version: 11.1.0rc5
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.1.0rc4/setup.cfg` & `openmodule_commands-11.1.0rc5/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc4/setup.py` & `openmodule_commands-11.1.0rc5/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc4/translate.py` & `openmodule_commands-11.1.0rc5/translate.py`

 * *Files identical despite different names*

