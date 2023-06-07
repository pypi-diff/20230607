# Comparing `tmp/pclick-0.1.27.tar.gz` & `tmp/pclick-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pclick-0.1.27.tar", max compression
+gzip compressed data, was "pclick-0.1.29.tar", max compression
```

## Comparing `pclick-0.1.27.tar` & `pclick-0.1.29.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2021-10-20 11:00:43.860801 pclick-0.1.27/README.md
--rw-r--r--   0        0        0      482 2023-06-07 08:00:37.647996 pclick-0.1.27/pyproject.toml
--rw-r--r--   0        0        0    10259 2023-06-07 07:32:08.130569 pclick-0.1.27/src/pclick/Messaging_pb2.py
--rw-r--r--   0        0        0      527 2022-12-20 09:23:53.909558 pclick-0.1.27/src/pclick/__init__.py
--rw-r--r--   0        0        0     1087 2022-09-09 16:13:16.831909 pclick-0.1.27/src/pclick/client.py
--rw-r--r--   0        0        0        0 2021-10-15 12:09:20.013250 pclick-0.1.27/src/pclick/demo/__init__.py
--rw-r--r--   0        0        0      159 2022-10-24 11:54:24.274468 pclick-0.1.27/src/pclick/demo/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2022-06-20 06:44:26.841227 pclick-0.1.27/src/pclick/demo/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3457 2023-05-31 11:34:14.381785 pclick-0.1.27/src/pclick/demo/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0     3461 2023-05-22 14:26:39.207729 pclick-0.1.27/src/pclick/demo/__pycache__/client.cpython-39.pyc
--rw-r--r--   0        0        0     2898 2022-09-13 13:14:55.794124 pclick-0.1.27/src/pclick/demo/__pycache__/client_shared.cpython-39.pyc
--rw-r--r--   0        0        0     2990 2022-09-12 15:08:46.858446 pclick-0.1.27/src/pclick/demo/__pycache__/pub_demo_server.cpython-39.pyc
--rw-r--r--   0        0        0     3081 2023-05-31 09:24:47.280850 pclick-0.1.27/src/pclick/demo/__pycache__/server.cpython-310.pyc
--rw-r--r--   0        0        0     3076 2023-05-22 14:12:21.319547 pclick-0.1.27/src/pclick/demo/__pycache__/server.cpython-39.pyc
--rw-r--r--   0        0        0     1652 2022-09-13 13:14:55.791524 pclick-0.1.27/src/pclick/demo/__pycache__/sub_demo_client.cpython-39.pyc
--rw-r--r--   0        0        0     4566 2023-06-07 07:32:08.131103 pclick-0.1.27/src/pclick/demo/client.py
--rw-r--r--   0        0        0     3767 2023-06-07 07:32:08.131614 pclick-0.1.27/src/pclick/demo/server.py
--rw-r--r--   0        0        0     2014 2021-10-20 09:58:12.229791 pclick-0.1.27/src/pclick/message_proto_helpers.py
--rw-r--r--   0        0        0     2537 2023-06-07 07:32:08.132121 pclick-0.1.27/src/pclick/server.py
--rw-r--r--   0        0        0     1715 1970-01-01 00:00:00.000000 pclick-0.1.27/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-10-20 11:00:43.860801 pclick-0.1.29/README.md
+-rw-r--r--   0        0        0      476 2023-06-07 09:25:24.359356 pclick-0.1.29/pyproject.toml
+-rw-r--r--   0        0        0    10259 2023-06-07 07:32:08.130569 pclick-0.1.29/src/pclick/Messaging_pb2.py
+-rw-r--r--   0        0        0      527 2022-12-20 09:23:53.909558 pclick-0.1.29/src/pclick/__init__.py
+-rw-r--r--   0        0        0     1087 2022-09-09 16:13:16.831909 pclick-0.1.29/src/pclick/client.py
+-rw-r--r--   0        0        0        0 2021-10-15 12:09:20.013250 pclick-0.1.29/src/pclick/demo/__init__.py
+-rw-r--r--   0        0        0      159 2022-10-24 11:54:24.274468 pclick-0.1.29/src/pclick/demo/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2022-06-20 06:44:26.841227 pclick-0.1.29/src/pclick/demo/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3457 2023-05-31 11:34:14.381785 pclick-0.1.29/src/pclick/demo/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0        0        0     3461 2023-05-22 14:26:39.207729 pclick-0.1.29/src/pclick/demo/__pycache__/client.cpython-39.pyc
+-rw-r--r--   0        0        0     2898 2022-09-13 13:14:55.794124 pclick-0.1.29/src/pclick/demo/__pycache__/client_shared.cpython-39.pyc
+-rw-r--r--   0        0        0     2990 2022-09-12 15:08:46.858446 pclick-0.1.29/src/pclick/demo/__pycache__/pub_demo_server.cpython-39.pyc
+-rw-r--r--   0        0        0     3081 2023-05-31 09:24:47.280850 pclick-0.1.29/src/pclick/demo/__pycache__/server.cpython-310.pyc
+-rw-r--r--   0        0        0     3076 2023-05-22 14:12:21.319547 pclick-0.1.29/src/pclick/demo/__pycache__/server.cpython-39.pyc
+-rw-r--r--   0        0        0     1652 2022-09-13 13:14:55.791524 pclick-0.1.29/src/pclick/demo/__pycache__/sub_demo_client.cpython-39.pyc
+-rw-r--r--   0        0        0     4566 2023-06-07 07:32:08.131103 pclick-0.1.29/src/pclick/demo/client.py
+-rw-r--r--   0        0        0     3767 2023-06-07 07:32:08.131614 pclick-0.1.29/src/pclick/demo/server.py
+-rw-r--r--   0        0        0     2014 2021-10-20 09:58:12.229791 pclick-0.1.29/src/pclick/message_proto_helpers.py
+-rw-r--r--   0        0        0     2537 2023-06-07 07:32:08.132121 pclick-0.1.29/src/pclick/server.py
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 pclick-0.1.29/PKG-INFO
```

### Comparing `pclick-0.1.27/README.md` & `pclick-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/Messaging_pb2.py` & `pclick-0.1.29/src/pclick/Messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/__init__.py` & `pclick-0.1.29/src/pclick/__init__.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/client.py` & `pclick-0.1.29/src/pclick/client.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/demo/__pycache__/client.cpython-310.pyc` & `pclick-0.1.29/src/pclick/demo/__pycache__/client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/demo/__pycache__/client.cpython-39.pyc` & `pclick-0.1.29/src/pclick/demo/__pycache__/client.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/demo/__pycache__/client_shared.cpython-39.pyc` & `pclick-0.1.29/src/pclick/demo/__pycache__/client_shared.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/demo/__pycache__/pub_demo_server.cpython-39.pyc` & `pclick-0.1.29/src/pclick/demo/__pycache__/pub_demo_server.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/demo/__pycache__/server.cpython-310.pyc` & `pclick-0.1.29/src/pclick/demo/__pycache__/server.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/demo/__pycache__/server.cpython-39.pyc` & `pclick-0.1.29/src/pclick/demo/__pycache__/server.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/demo/__pycache__/sub_demo_client.cpython-39.pyc` & `pclick-0.1.29/src/pclick/demo/__pycache__/sub_demo_client.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/demo/client.py` & `pclick-0.1.29/src/pclick/demo/client.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/demo/server.py` & `pclick-0.1.29/src/pclick/demo/server.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/message_proto_helpers.py` & `pclick-0.1.29/src/pclick/message_proto_helpers.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/src/pclick/server.py` & `pclick-0.1.29/src/pclick/server.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.27/PKG-INFO` & `pclick-0.1.29/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pclick
-Version: 0.1.27
+Version: 0.1.29
 Summary: Controller to AGX messaging
-Home-page: https://git.algoryx.se/algoryx/external/click
+Home-page: https://github.com/algoryx/click-mirror
 License: Apache-2.0
 Author: Algoryx Simulation
 Author-email: contact@algoryx.se
-Requires-Python: >=3.8,<3.10
+Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: protobuf (==3.17.1)
 Requires-Dist: pyzmq (==22.3.0)
-Project-URL: Repository, https://git.algoryx.se/algoryx/external/click
+Project-URL: Repository, https://github.com/algoryx/click-mirror
 Description-Content-Type: text/markdown
 
 # Click
 
 The main idea behind click is to enable a non-Brick controller talking to a Brick enabled AGX Simulation in way configurable by Brick.
 The name comes from the sound two Bricks makes when connected.
```

