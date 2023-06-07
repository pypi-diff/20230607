# Comparing `tmp/agxclick-0.1.28.tar.gz` & `tmp/agxclick-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agxclick-0.1.28.tar", max compression
+gzip compressed data, was "agxclick-0.1.29.tar", max compression
```

## Comparing `agxclick-0.1.28.tar` & `agxclick-0.1.29.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    10433 2023-06-07 08:50:39.313818 agxclick-0.1.28/README.md
--rw-r--r--   0        0        0      495 2023-06-07 08:52:00.360874 agxclick-0.1.28/pyproject.toml
--rw-r--r--   0        0        0      649 2022-06-02 06:39:22.620436 agxclick-0.1.28/src/agxclick/__init__.py
--rw-r--r--   0        0        0     2348 2022-06-02 06:39:22.622000 agxclick-0.1.28/src/agxclick/agx_application.py
--rw-r--r--   0        0        0      264 2022-06-16 12:35:01.202788 agxclick-0.1.28/src/agxclick/application_step_listener.py
--rw-r--r--   0        0        0     1647 2023-06-07 07:32:08.110496 agxclick-0.1.28/src/agxclick/brick_reader.py
--rw-r--r--   0        0        0     2379 2022-06-02 06:39:22.625681 agxclick-0.1.28/src/agxclick/brick_utils.py
--rw-r--r--   0        0        0    10140 2023-06-07 07:32:08.110706 agxclick-0.1.28/src/agxclick/click_application.py
--rw-r--r--   0        0        0     9778 2023-06-07 07:32:08.110907 agxclick-0.1.28/src/agxclick/click_event_listener.py
--rw-r--r--   0        0        0    10192 2023-06-07 07:32:08.111099 agxclick-0.1.28/src/agxclick/click_robot.py
--rw-r--r--   0        0        0      736 2022-06-02 06:39:22.629400 agxclick-0.1.28/src/agxclick/graphics_throttler.py
--rw-r--r--   0        0        0     1319 2021-11-17 10:51:45.931702 agxclick-0.1.28/src/agxclick/keyboard_listener.py
--rw-r--r--   0        0        0    10279 2023-06-07 07:32:08.111672 agxclick-0.1.28/src/agxclick/message_factory.py
--rw-r--r--   0        0        0     1230 2023-06-07 07:32:08.111855 agxclick-0.1.28/src/agxclick/reset_batch_listener.py
--rw-r--r--   0        0        0      348 2022-06-02 06:39:22.631892 agxclick-0.1.28/src/agxclick/wallclock.py
--rw-r--r--   0        0        0    11031 1970-01-01 00:00:00.000000 agxclick-0.1.28/PKG-INFO
+-rw-r--r--   0        0        0    10433 2023-06-07 08:50:39.313818 agxclick-0.1.29/README.md
+-rw-r--r--   0        0        0      495 2023-06-07 09:26:12.304609 agxclick-0.1.29/pyproject.toml
+-rw-r--r--   0        0        0      649 2022-06-02 06:39:22.620436 agxclick-0.1.29/src/agxclick/__init__.py
+-rw-r--r--   0        0        0     2348 2022-06-02 06:39:22.622000 agxclick-0.1.29/src/agxclick/agx_application.py
+-rw-r--r--   0        0        0      264 2022-06-16 12:35:01.202788 agxclick-0.1.29/src/agxclick/application_step_listener.py
+-rw-r--r--   0        0        0     1647 2023-06-07 07:32:08.110496 agxclick-0.1.29/src/agxclick/brick_reader.py
+-rw-r--r--   0        0        0     2379 2022-06-02 06:39:22.625681 agxclick-0.1.29/src/agxclick/brick_utils.py
+-rw-r--r--   0        0        0    10140 2023-06-07 07:32:08.110706 agxclick-0.1.29/src/agxclick/click_application.py
+-rw-r--r--   0        0        0     9778 2023-06-07 07:32:08.110907 agxclick-0.1.29/src/agxclick/click_event_listener.py
+-rw-r--r--   0        0        0    10192 2023-06-07 07:32:08.111099 agxclick-0.1.29/src/agxclick/click_robot.py
+-rw-r--r--   0        0        0      736 2022-06-02 06:39:22.629400 agxclick-0.1.29/src/agxclick/graphics_throttler.py
+-rw-r--r--   0        0        0     1319 2021-11-17 10:51:45.931702 agxclick-0.1.29/src/agxclick/keyboard_listener.py
+-rw-r--r--   0        0        0    10279 2023-06-07 07:32:08.111672 agxclick-0.1.29/src/agxclick/message_factory.py
+-rw-r--r--   0        0        0     1230 2023-06-07 07:32:08.111855 agxclick-0.1.29/src/agxclick/reset_batch_listener.py
+-rw-r--r--   0        0        0      348 2022-06-02 06:39:22.631892 agxclick-0.1.29/src/agxclick/wallclock.py
+-rw-r--r--   0        0        0    11081 1970-01-01 00:00:00.000000 agxclick-0.1.29/PKG-INFO
```

### Comparing `agxclick-0.1.28/README.md` & `agxclick-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/src/agxclick/__init__.py` & `agxclick-0.1.29/src/agxclick/__init__.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/src/agxclick/agx_application.py` & `agxclick-0.1.29/src/agxclick/agx_application.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/src/agxclick/brick_reader.py` & `agxclick-0.1.29/src/agxclick/brick_reader.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/src/agxclick/brick_utils.py` & `agxclick-0.1.29/src/agxclick/brick_utils.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/src/agxclick/click_application.py` & `agxclick-0.1.29/src/agxclick/click_application.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/src/agxclick/click_event_listener.py` & `agxclick-0.1.29/src/agxclick/click_event_listener.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/src/agxclick/click_robot.py` & `agxclick-0.1.29/src/agxclick/click_robot.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/src/agxclick/graphics_throttler.py` & `agxclick-0.1.29/src/agxclick/graphics_throttler.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/src/agxclick/keyboard_listener.py` & `agxclick-0.1.29/src/agxclick/keyboard_listener.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/src/agxclick/message_factory.py` & `agxclick-0.1.29/src/agxclick/message_factory.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/src/agxclick/reset_batch_listener.py` & `agxclick-0.1.29/src/agxclick/reset_batch_listener.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.28/PKG-INFO` & `agxclick-0.1.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: agxclick
-Version: 0.1.28
+Version: 0.1.29
 Summary: Controller to AGX using pClick messaging
 Home-page: https://github.com/algoryx/click-mirror
 License: Apache-2.0
 Author: Algoryx Simulation
 Author-email: contact@algoryx.se
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: agxBrick (>=0.5.7)
 Requires-Dist: pClick (>=0.1.35)
 Project-URL: Repository, https://github.com/algoryx/click-mirror
 Description-Content-Type: text/markdown
 
 # AgxClick
```

