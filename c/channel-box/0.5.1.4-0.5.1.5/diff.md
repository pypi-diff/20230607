# Comparing `tmp/channel_box-0.5.1.4-py3-none-any.whl.zip` & `tmp/channel_box-0.5.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7340 bytes, number of entries: 10
+Zip file size: 7342 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx       48 b- defN 23-Jun-07 06:56 channel_box/__init__.py
 -rw-rw-r--  2.0 unx     5724 b- defN 23-Jun-07 09:06 channel_box/src.py
 -rw-rw-r--  2.0 unx        0 b- defN 20-Jul-19 15:17 example/channel/__init__.py
 -rw-rw-r--  2.0 unx      599 b- defN 23-Jun-07 07:55 example/channel/urls.py
 -rw-rw-r--  2.0 unx     6393 b- defN 23-Jun-07 08:13 example/channel/views.py
--rwxr-xr-x  2.0 unx     1094 b- defN 23-Jun-07 09:07 channel_box-0.5.1.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3040 b- defN 23-Jun-07 09:07 channel_box-0.5.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 09:07 channel_box-0.5.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-Jun-07 09:07 channel_box-0.5.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      810 b- defN 23-Jun-07 09:07 channel_box-0.5.1.4.dist-info/RECORD
-10 files, 17820 bytes uncompressed, 5950 bytes compressed:  66.6%
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-Jun-07 09:09 channel_box-0.5.1.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3045 b- defN 23-Jun-07 09:09 channel_box-0.5.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 09:09 channel_box-0.5.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jun-07 09:09 channel_box-0.5.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      810 b- defN 23-Jun-07 09:09 channel_box-0.5.1.5.dist-info/RECORD
+10 files, 17825 bytes uncompressed, 5952 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: example/channel/urls.py
 Comment: 
 
 Filename: example/channel/views.py
 Comment: 
 
-Filename: channel_box-0.5.1.4.dist-info/LICENSE
+Filename: channel_box-0.5.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: channel_box-0.5.1.4.dist-info/METADATA
+Filename: channel_box-0.5.1.5.dist-info/METADATA
 Comment: 
 
-Filename: channel_box-0.5.1.4.dist-info/WHEEL
+Filename: channel_box-0.5.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: channel_box-0.5.1.4.dist-info/top_level.txt
+Filename: channel_box-0.5.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: channel_box-0.5.1.4.dist-info/RECORD
+Filename: channel_box-0.5.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `channel_box-0.5.1.4.dist-info/LICENSE` & `channel_box-0.5.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `channel_box-0.5.1.4.dist-info/METADATA` & `channel_box-0.5.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: channel-box
-Version: 0.5.1.4
+Version: 0.5.1.5
 Summary: ChannelBox it is a package for Starlette framework that allows you to make named webscoket channels.
 Home-page: https://github.com/Sobolev5/channel-box
 Author: Sobolev Andrey
 Author-email: email.asobolev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -63,14 +63,15 @@
 
 ## Setup channel 
 ```python
 from starlette.endpoints import WebSocketEndpoint
 from channel_box import Channel, ChannelBox
 
 class WsChatEndpoint(WebSocketEndpoint):
+    
     async def on_connect(self, websocket):
         group_name = websocket.query_params.get("group_name")  # group name */ws?group_name=MyChat
         if group_name:
             channel = Channel(websocket, expires=60*60, encoding="json") # define user channel
             channel = await ChannelBox.channel_add(group_name, channel) # add channel to named group
         await websocket.accept()
```

## Comparing `channel_box-0.5.1.4.dist-info/RECORD` & `channel_box-0.5.1.5.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 channel_box/__init__.py,sha256=IQ6PdTXL75hv4rFxJ0Mjns30mHJIX_UFUp28JwsU6CY,48
 channel_box/src.py,sha256=vNjWM0H1HFlyO-yBR-hra9MXu2kG8H7-vfGL3qZ-AN0,5724
 example/channel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 example/channel/urls.py,sha256=R_FB2kG6cMHa_OferyJSll7ixYcnIvxqSTKgjuQFmiI,599
 example/channel/views.py,sha256=JS7xGVULStUowWxpm_-x9jEGrZGf37bL_yrKBz2Z8yk,6393
-channel_box-0.5.1.4.dist-info/LICENSE,sha256=BvmWh0aXPp8jrD0GS25NwyJ321UbcQ7KIui9wAmwVD0,1094
-channel_box-0.5.1.4.dist-info/METADATA,sha256=IdwDB_MOjLBDX3BbZJI05HAAOolhcBFlhnrWYAlDtYQ,3040
-channel_box-0.5.1.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-channel_box-0.5.1.4.dist-info/top_level.txt,sha256=mjnxqFEWVz6Q-V_iwda7dXI5euFqxEJoqnhuKt-k6sI,20
-channel_box-0.5.1.4.dist-info/RECORD,,
+channel_box-0.5.1.5.dist-info/LICENSE,sha256=BvmWh0aXPp8jrD0GS25NwyJ321UbcQ7KIui9wAmwVD0,1094
+channel_box-0.5.1.5.dist-info/METADATA,sha256=wlCq-at3L5u7EKja64dqbDrcG1RhYwI5BipRcWLzZx8,3045
+channel_box-0.5.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+channel_box-0.5.1.5.dist-info/top_level.txt,sha256=mjnxqFEWVz6Q-V_iwda7dXI5euFqxEJoqnhuKt-k6sI,20
+channel_box-0.5.1.5.dist-info/RECORD,,
```

