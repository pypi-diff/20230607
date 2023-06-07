# Comparing `tmp/chatai-stream-0.0.2.tar.gz` & `tmp/chatai-stream-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-stream-0.0.2.tar", last modified: Tue Jun  6 12:57:24 2023, max compression
+gzip compressed data, was "chatai-stream-0.0.3.tar", last modified: Wed Jun  7 14:57:23 2023, max compression
```

## Comparing `chatai-stream-0.0.2.tar` & `chatai-stream-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 12:57:24.373233 chatai-stream-0.0.2/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 11:25:30.000000 chatai-stream-0.0.2/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-06 12:57:24.373233 chatai-stream-0.0.2/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8103 2023-06-06 12:52:21.000000 chatai-stream-0.0.2/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-06 12:57:24.373233 chatai-stream-0.0.2/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1162 2023-06-06 12:52:21.000000 chatai-stream-0.0.2/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 12:57:24.373233 chatai-stream-0.0.2/src/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1582 2023-06-06 12:52:21.000000 chatai-stream-0.0.2/src/ChatAIStream.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       51 2023-06-06 12:52:21.000000 chatai-stream-0.0.2/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 12:57:24.373233 chatai-stream-0.0.2/src/chatai_stream.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-06 12:57:24.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      306 2023-06-06 12:57:24.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 12:57:24.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 12:52:21.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       44 2023-06-06 12:57:24.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       22 2023-06-06 12:57:24.000000 chatai-stream-0.0.2/src/chatai_stream.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 14:57:23.756641 chatai-stream-0.0.3/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 11:25:30.000000 chatai-stream-0.0.3/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-07 14:57:23.756641 chatai-stream-0.0.3/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8103 2023-06-06 12:52:21.000000 chatai-stream-0.0.3/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-07 14:57:23.756641 chatai-stream-0.0.3/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1162 2023-06-07 14:34:45.000000 chatai-stream-0.0.3/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 14:57:23.756641 chatai-stream-0.0.3/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1610 2023-06-07 14:17:02.000000 chatai-stream-0.0.3/src/ChatAIStream.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       51 2023-06-07 14:35:24.000000 chatai-stream-0.0.3/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 14:57:23.756641 chatai-stream-0.0.3/src/chatai_stream.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-07 14:57:23.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      306 2023-06-07 14:57:23.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-07 14:57:23.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 12:52:21.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       44 2023-06-07 14:57:23.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       22 2023-06-07 14:57:23.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/top_level.txt
```

### Comparing `chatai-stream-0.0.2/LICENSE` & `chatai-stream-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-stream-0.0.2/PKG-INFO` & `chatai-stream-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-stream
-Version: 0.0.2
+Version: 0.0.3
 Summary: ChatGPT reacts YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStream
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-stream-0.0.2/README.md` & `chatai-stream-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `chatai-stream-0.0.2/setup.py` & `chatai-stream-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-stream",
-    version="0.0.2",
+    version="0.0.3",
     license="MIT",
     description="ChatGPT reacts YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-stream-0.0.2/src/ChatAIStream.py` & `chatai-stream-0.0.3/src/ChatAIStream.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
 import threading
 from typing import Callable
 from dataclasses import dataclass
 import StreamChatAgent as sca
 import ChatAIAgent as ca
 
-
 streamParams = sca.params
+userMessage = ca.userMessage
 aiParams = ca.params
 
 @dataclass
 class params():
   stream_params: streamParams
   ai_params: aiParams
```

### Comparing `chatai-stream-0.0.2/src/chatai_stream.egg-info/PKG-INFO` & `chatai-stream-0.0.3/src/chatai_stream.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-stream
-Version: 0.0.2
+Version: 0.0.3
 Summary: ChatGPT reacts YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStream
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

