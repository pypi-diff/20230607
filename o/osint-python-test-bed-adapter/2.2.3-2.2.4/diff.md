# Comparing `tmp/osint-python-test-bed-adapter-2.2.3.tar.gz` & `tmp/osint-python-test-bed-adapter-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-test-bed-adapter-2.2.3.tar", last modified: Thu Jun  1 22:39:50 2023, max compression
+gzip compressed data, was "osint-python-test-bed-adapter-2.2.4.tar", last modified: Wed Jun  7 20:38:14 2023, max compression
```

## Comparing `osint-python-test-bed-adapter-2.2.3.tar` & `osint-python-test-bed-adapter-2.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.3/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1743 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1316 2023-04-06 23:36:33.000000 osint-python-test-bed-adapter-2.2.3/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1743 2023-06-01 22:39:50.000000 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      782 2023-06-01 22:39:50.000000 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-01 22:39:50.000000 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-06-01 22:39:50.000000 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       17 2023-06-01 22:39:50.000000 osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-06-01 22:37:37.000000 osint-python-test-bed-adapter-2.2.3/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1361 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/__init__.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2413 2023-06-01 22:37:01.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/consumer_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1660 2023-03-16 17:49:08.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/heartbeat_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2897 2023-03-16 17:49:08.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/log_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2122 2023-04-06 23:32:08.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/producer_manager.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/options/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/options/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3486 2023-06-01 22:28:40.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/options/test_bed_options.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/services/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-14 11:55:32.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/services/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2065 2023-03-14 12:17:24.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/services/http_server.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-01 22:39:50.616154 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/helpers.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/key.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.374964 osint-python-test-bed-adapter-2.2.4/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.4/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1743 2023-06-07 20:38:14.374964 osint-python-test-bed-adapter-2.2.4/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1316 2023-04-06 23:36:33.000000 osint-python-test-bed-adapter-2.2.4/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.371631 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1743 2023-06-07 20:38:14.000000 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      782 2023-06-07 20:38:14.000000 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-07 20:38:14.000000 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-06-07 20:38:14.000000 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       17 2023-06-07 20:38:14.000000 osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-07 20:38:14.374964 osint-python-test-bed-adapter-2.2.4/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-06-07 20:37:17.000000 osint-python-test-bed-adapter-2.2.4/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.371631 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1361 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/__init__.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.371631 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2413 2023-06-01 22:37:01.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/consumer_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1660 2023-03-16 17:49:08.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/heartbeat_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2999 2023-06-07 19:48:38.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/log_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2122 2023-04-06 23:32:08.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/producer_manager.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.371631 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/options/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/options/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3486 2023-06-01 22:28:40.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/options/test_bed_options.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.371631 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/services/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-14 11:55:32.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/services/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2065 2023-03-14 12:17:24.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/services/http_server.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 20:38:14.374964 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/helpers.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/key.py
```

### Comparing `osint-python-test-bed-adapter-2.2.3/LICENSE` & `osint-python-test-bed-adapter-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.3/PKG-INFO` & `osint-python-test-bed-adapter-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-test-bed-adapter
-Version: 2.2.3
+Version: 2.2.4
 Summary: Python adapter for Kafka
 Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
 Author: TimovdK
 Author-email: timo_kuil@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osint-python-test-bed-adapter-2.2.3/README.md` & `osint-python-test-bed-adapter-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/PKG-INFO` & `osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-test-bed-adapter
-Version: 2.2.3
+Version: 2.2.4
 Summary: Python adapter for Kafka
 Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
 Author: TimovdK
 Author-email: timo_kuil@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osint-python-test-bed-adapter-2.2.3/osint_python_test_bed_adapter.egg-info/SOURCES.txt` & `osint-python-test-bed-adapter-2.2.4/osint_python_test_bed_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.3/setup.py` & `osint-python-test-bed-adapter-2.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="osint-python-test-bed-adapter",
-    version="2.2.3",
+    version="2.2.4",
     author="TimovdK",
     author_email="timo_kuil@hotmail.com",
     description="Python adapter for Kafka",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-adapter",
     include_package_data=True,
```

### Comparing `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/__init__.py` & `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/consumer_manager.py` & `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/consumer_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/heartbeat_manager.py` & `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/heartbeat_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/log_manager.py` & `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/log_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from ..options.test_bed_options import TestBedOptions
-from .producer_manager import ProducerManager
-from ..utils.helpers import Helpers
-from enum import Enum
-from datetime import datetime
 import copy
 import json
 import time
+from datetime import datetime
+from enum import Enum
 
+from .producer_manager import ProducerManager
+from ..options.test_bed_options import TestBedOptions
+from ..utils.helpers import Helpers
 
 
 class BColors:
     OKBLUE = '\033[94m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
     ENDC = '\033[0m'
@@ -21,25 +21,25 @@
 
 
 def timestamp():
     return datetime.today().strftime('%Y-%m-%d %H:%M:%S')
 
 
 def LogLevelToType(level):
-    if (level == LogLevel.Sill):
+    if level == LogLevel.Sill:
         return 'SILLY'
-    elif (level == LogLevel.Debug):
+    elif level == LogLevel.Debug:
         return 'DEBUG'
-    elif (level == LogLevel.Info):
+    elif level == LogLevel.Info:
         return 'INFO'
-    elif (level == LogLevel.Warn):
+    elif level == LogLevel.Warn:
         return 'WARN'
-    elif (level == LogLevel.Error):
+    elif level == LogLevel.Error:
         return 'ERROR'
-    elif (level == LogLevel.Critical):
+    elif level == LogLevel.Critical:
         return 'CRITICAL'
 
 
 class LogLevel(Enum):
     Sill = 0,
     Debug = 1,
     Info = 2,
@@ -74,33 +74,34 @@
     def error(self, msg):
         self.log(LogLevel.Error, msg)
 
     def critical(self, msg):
         self.log(LogLevel.Critical, msg)
 
     def log(self, level: LogLevel, msg):
-        if (not isinstance(msg, str)):
+        if not isinstance(msg, str):
             msg = json.dumps(msg)
 
         # Send to console
-        if (level == LogLevel.Sill):
+        if level == LogLevel.Sill:
             print(f'{BColors.OKBLUE}{timestamp()}: Silly: {msg}{BColors.ENDC}')
-        elif (level == LogLevel.Debug):
+        elif level == LogLevel.Debug:
             print(f'{BColors.OKBLUE}{timestamp()}: Debug: {msg}{BColors.ENDC}')
-        elif (level == LogLevel.Info):
+        elif level == LogLevel.Info:
             print(f'{BColors.OKBLUE}{timestamp()}: Info: {msg}{BColors.ENDC}')
-        elif (level == LogLevel.Warn):
+        elif level == LogLevel.Warn:
             print(f'{BColors.WARNING}{timestamp()}: Warning: {msg}{BColors.ENDC}')
-        elif (level == LogLevel.Error):
+        elif level == LogLevel.Error:
             print(f'{BColors.FAIL}{timestamp()}: Error: {msg}{BColors.ENDC}')
-        elif (level == LogLevel.Critical):
+        elif level == LogLevel.Critical:
             print(f'{BColors.FAIL}{timestamp()}: Critical: {msg}{BColors.ENDC}')
 
-        # Send to Kafka
-        payload = {
-            "id": self.options.consumer_group,
-            "level": LogLevelToType(level),
-            "dateTimeSent": current_milli_time(),
-            "log": msg
-        }
-        message = [payload]
-        self.kafka_log_producer.send_messages(message)
+        if level == LogLevel.Error or level == LogLevel.Critical or level == LogLevel.Warn:
+            # Send to Kafka
+            payload = {
+                "id": self.options.consumer_group,
+                "level": LogLevelToType(level),
+                "dateTimeSent": current_milli_time(),
+                "log": msg
+            }
+            message = [payload]
+            self.kafka_log_producer.send_messages(message)
```

### Comparing `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/kafka/producer_manager.py` & `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/kafka/producer_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/options/test_bed_options.py` & `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/options/test_bed_options.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/services/http_server.py` & `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/services/http_server.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/helpers.py` & `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.3/test_bed_adapter/utils/key.py` & `osint-python-test-bed-adapter-2.2.4/test_bed_adapter/utils/key.py`

 * *Files identical despite different names*

