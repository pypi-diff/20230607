# Comparing `tmp/channel_box-0.5.1.2-py3-none-any.whl.zip` & `tmp/channel_box-0.5.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7333 bytes, number of entries: 10
+Zip file size: 7340 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx       48 b- defN 23-Jun-07 06:56 channel_box/__init__.py
--rw-rw-r--  2.0 unx     5746 b- defN 23-Jun-07 08:07 channel_box/src.py
+-rw-rw-r--  2.0 unx     5724 b- defN 23-Jun-07 09:06 channel_box/src.py
 -rw-rw-r--  2.0 unx        0 b- defN 20-Jul-19 15:17 example/channel/__init__.py
 -rw-rw-r--  2.0 unx      599 b- defN 23-Jun-07 07:55 example/channel/urls.py
 -rw-rw-r--  2.0 unx     6393 b- defN 23-Jun-07 08:13 example/channel/views.py
--rwxr-xr-x  2.0 unx     1094 b- defN 23-Jun-07 08:45 channel_box-0.5.1.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3040 b- defN 23-Jun-07 08:45 channel_box-0.5.1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 08:45 channel_box-0.5.1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-Jun-07 08:45 channel_box-0.5.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      810 b- defN 23-Jun-07 08:45 channel_box-0.5.1.2.dist-info/RECORD
-10 files, 17842 bytes uncompressed, 5943 bytes compressed:  66.7%
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-Jun-07 09:07 channel_box-0.5.1.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3040 b- defN 23-Jun-07 09:07 channel_box-0.5.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 09:07 channel_box-0.5.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jun-07 09:07 channel_box-0.5.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      810 b- defN 23-Jun-07 09:07 channel_box-0.5.1.4.dist-info/RECORD
+10 files, 17820 bytes uncompressed, 5950 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: example/channel/urls.py
 Comment: 
 
 Filename: example/channel/views.py
 Comment: 
 
-Filename: channel_box-0.5.1.2.dist-info/LICENSE
+Filename: channel_box-0.5.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: channel_box-0.5.1.2.dist-info/METADATA
+Filename: channel_box-0.5.1.4.dist-info/METADATA
 Comment: 
 
-Filename: channel_box-0.5.1.2.dist-info/WHEEL
+Filename: channel_box-0.5.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: channel_box-0.5.1.2.dist-info/top_level.txt
+Filename: channel_box-0.5.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: channel_box-0.5.1.2.dist-info/RECORD
+Filename: channel_box-0.5.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## channel_box/src.py

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 import datetime
 import sys
 import os
 import time
 import uuid
 import logging
+from typing import Any
 from enum import Enum
 from starlette.websockets import WebSocket
 
 
 class Channel:
     """ 
     Channel class - active user channel (adapter to starlette.websockets.WebSocket).
@@ -25,16 +26,15 @@
         assert isinstance(encoding, str) and encoding in ["json", "text", "bytes"], "Must be in ['json', 'text', 'bytes']"
         self.websocket = websocket
         self.expires = expires
         self.encoding = encoding
         self.uuid = uuid.uuid4()
         self.created = time.time()
 
-    async def send(self, payload: dict={}) -> None:
-        assert isinstance(payload, dict)
+    async def send(self, payload: Any) -> None:
         if self.encoding == "json":
             try:
                 await self.websocket.send_json(payload)
             except RuntimeError as error:
                 logging.debug(error)  
         elif self.encoding == "text":
             try:
```

## Comparing `channel_box-0.5.1.2.dist-info/LICENSE` & `channel_box-0.5.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `channel_box-0.5.1.2.dist-info/METADATA` & `channel_box-0.5.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: channel-box
-Version: 0.5.1.2
+Version: 0.5.1.4
 Summary: ChannelBox it is a package for Starlette framework that allows you to make named webscoket channels.
 Home-page: https://github.com/Sobolev5/channel-box
 Author: Sobolev Andrey
 Author-email: email.asobolev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `channel_box-0.5.1.2.dist-info/RECORD` & `channel_box-0.5.1.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 channel_box/__init__.py,sha256=IQ6PdTXL75hv4rFxJ0Mjns30mHJIX_UFUp28JwsU6CY,48
-channel_box/src.py,sha256=nENCMuVdy-QfUkpfylmSdQ_etE_RUb0OrstCNqLlyz0,5746
+channel_box/src.py,sha256=vNjWM0H1HFlyO-yBR-hra9MXu2kG8H7-vfGL3qZ-AN0,5724
 example/channel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 example/channel/urls.py,sha256=R_FB2kG6cMHa_OferyJSll7ixYcnIvxqSTKgjuQFmiI,599
 example/channel/views.py,sha256=JS7xGVULStUowWxpm_-x9jEGrZGf37bL_yrKBz2Z8yk,6393
-channel_box-0.5.1.2.dist-info/LICENSE,sha256=BvmWh0aXPp8jrD0GS25NwyJ321UbcQ7KIui9wAmwVD0,1094
-channel_box-0.5.1.2.dist-info/METADATA,sha256=IXZlQ7qrrPva__-ZaxnkzmhNYyMNbABPeFq_4bgoiyM,3040
-channel_box-0.5.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-channel_box-0.5.1.2.dist-info/top_level.txt,sha256=mjnxqFEWVz6Q-V_iwda7dXI5euFqxEJoqnhuKt-k6sI,20
-channel_box-0.5.1.2.dist-info/RECORD,,
+channel_box-0.5.1.4.dist-info/LICENSE,sha256=BvmWh0aXPp8jrD0GS25NwyJ321UbcQ7KIui9wAmwVD0,1094
+channel_box-0.5.1.4.dist-info/METADATA,sha256=IdwDB_MOjLBDX3BbZJI05HAAOolhcBFlhnrWYAlDtYQ,3040
+channel_box-0.5.1.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+channel_box-0.5.1.4.dist-info/top_level.txt,sha256=mjnxqFEWVz6Q-V_iwda7dXI5euFqxEJoqnhuKt-k6sI,20
+channel_box-0.5.1.4.dist-info/RECORD,,
```

