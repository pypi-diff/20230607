# Comparing `tmp/channel_box-0.4.0-py3-none-any.whl.zip` & `tmp/channel_box-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,12 @@
-Zip file size: 8227 bytes, number of entries: 14
--rw-rw-r--  2.0 unx       83 b- defN 21-Oct-17 15:36 channel_box/__init__.py
--rw-rw-r--  2.0 unx     5140 b- defN 22-Sep-15 12:35 channel_box/channel_box.py
--rw-rw-r--  2.0 unx        0 b- defN 20-Jul-19 09:12 example/__init__.py
--rw-rw-r--  2.0 unx      318 b- defN 22-Sep-15 12:22 example/app.py
--rw-rw-r--  2.0 unx       18 b- defN 22-Sep-15 12:32 example/settings.py
--rw-rw-r--  2.0 unx      968 b- defN 22-Sep-15 12:31 example/setup.py
+Zip file size: 7320 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx       48 b- defN 23-Jun-07 06:56 channel_box/__init__.py
+-rw-rw-r--  2.0 unx     5746 b- defN 23-Jun-07 08:07 channel_box/src.py
 -rw-rw-r--  2.0 unx        0 b- defN 20-Jul-19 15:17 example/channel/__init__.py
--rw-rw-r--  2.0 unx      597 b- defN 22-Sep-15 11:32 example/channel/urls.py
--rw-rw-r--  2.0 unx     5947 b- defN 22-Sep-15 12:38 example/channel/views.py
--rw-r--r--  2.0 unx     1094 b- defN 22-Sep-15 12:44 channel_box-0.4.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2771 b- defN 22-Sep-15 12:44 channel_box-0.4.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Sep-15 12:44 channel_box-0.4.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 22-Sep-15 12:44 channel_box-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1097 b- defN 22-Sep-15 12:44 channel_box-0.4.0.dist-info/RECORD
-14 files, 18145 bytes uncompressed, 6401 bytes compressed:  64.7%
+-rw-rw-r--  2.0 unx      599 b- defN 23-Jun-07 07:55 example/channel/urls.py
+-rw-rw-r--  2.0 unx     6393 b- defN 23-Jun-07 08:13 example/channel/views.py
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-Jun-07 08:22 channel_box-0.5.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3054 b- defN 23-Jun-07 08:22 channel_box-0.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 08:22 channel_box-0.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jun-07 08:22 channel_box-0.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      800 b- defN 23-Jun-07 08:22 channel_box-0.5.1.dist-info/RECORD
+10 files, 17846 bytes uncompressed, 5950 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,43 +1,31 @@
 Filename: channel_box/__init__.py
 Comment: 
 
-Filename: channel_box/channel_box.py
-Comment: 
-
-Filename: example/__init__.py
-Comment: 
-
-Filename: example/app.py
-Comment: 
-
-Filename: example/settings.py
-Comment: 
-
-Filename: example/setup.py
+Filename: channel_box/src.py
 Comment: 
 
 Filename: example/channel/__init__.py
 Comment: 
 
 Filename: example/channel/urls.py
 Comment: 
 
 Filename: example/channel/views.py
 Comment: 
 
-Filename: channel_box-0.4.0.dist-info/LICENSE
+Filename: channel_box-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: channel_box-0.4.0.dist-info/METADATA
+Filename: channel_box-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: channel_box-0.4.0.dist-info/WHEEL
+Filename: channel_box-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: channel_box-0.4.0.dist-info/top_level.txt
+Filename: channel_box-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: channel_box-0.4.0.dist-info/RECORD
+Filename: channel_box-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## channel_box/__init__.py

```diff
@@ -1,2 +1,3 @@
-from .channel_box import ChannelBoxEndpoint
-from .channel_box import channel_box
+from .src import (
+    Channel, ChannelBox
+)
```

## example/channel/urls.py

```diff
@@ -1,20 +1,20 @@
 from starlette.routing import Route
 from starlette.routing import WebSocketRoute
 
-from .views import Channel
+from .views import WsChatEndpoint
 from .views import Chat
 from .views import Message
-from .views import Channels
-from .views import ChannelsFlush
+from .views import Groups
+from .views import GroupsFlush
 from .views import History
 from .views import HistoryFlush
 
 routes = [
-    WebSocketRoute("/chat_ws", Channel),
+    WebSocketRoute("/chat_ws", WsChatEndpoint),
     Route("/", endpoint=Chat),
     Route("/message", endpoint=Message),
-    Route("/channels", endpoint=Channels),
-    Route("/channels-flush", endpoint=ChannelsFlush),
+    Route("/groups", endpoint=Groups),
+    Route("/groups-flush", endpoint=GroupsFlush),
     Route("/history", endpoint=History),
     Route("/history-flush", endpoint=HistoryFlush),
 ]
```

## example/channel/views.py

```diff
@@ -1,59 +1,63 @@
+import json
 from simple_print import sprint
 from jinja2 import Template
-from channel_box import channel_box
-from channel_box import ChannelBoxEndpoint
+from channel_box import Channel
+from channel_box import ChannelBox
+from starlette.endpoints import WebSocketEndpoint
 from starlette.responses import JSONResponse
 from starlette.endpoints import HTTPEndpoint
 from starlette.responses import HTMLResponse
-from settings import HOST
+from settings import SOCKET
 
-class Channel(ChannelBoxEndpoint):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.expires = 16000
-        self.encoding = "json"
+
+class WsChatEndpoint(WebSocketEndpoint):
 
     async def on_connect(self, websocket):
-        sprint('user_connected', c="green", p=True)
-        channel_name = websocket.query_params.get("channel_name", "MySimpleChat")  # channel name */ws?channel_name=MySimpleChat
-        await self.channel_get_or_create(channel_name, websocket) 
+        sprint('Channel.on_connect', c="green")
+        group_name = websocket.query_params.get("group_name")  # group name */ws?group_name=MyChat
+        if group_name:
+            channel = Channel(websocket, expires=60*60, encoding="json") # define user channel
+            status = await ChannelBox.channel_add(group_name, channel) # add channel to named group
         await websocket.accept()
 
     async def on_receive(self, websocket, data):
+        sprint(f'Channel.on_receive data [{data}]', c="green")
+        data = json.loads(data)
         message = data["message"]
         username = data["username"]     
+
         if message.strip():
             payload = {
                 "username": username,
                 "message": message,
             }
-            await self.channel_send(payload, history=True)
-
+            group_name = websocket.query_params.get("group_name")
+            if group_name:
+                await ChannelBox.group_send(group_name, payload, history=True)
 
 html_text = """
 <!DOCTYPE html>
 <html>
     <head>
-        <title>MySimpleChat channel (open in different browsers)</title>
+        <title>MyChat group (open in different browsers)</title>
         <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
     </head>
     <body>
-        <div class="container mt-4">
-            
+        <div class="container mt-4">        
             <div class="card">
                 <div class="card-header">
-                    <h5 class="mt-2">MySimpleChat channel (open in different browsers)</h5>
-                    <h5>channel-box == 0.4.0</h5>
+                    <h5 class="mt-2">MyChat group (open in different browsers)</h5>
+                    <h5>channel-box == 0.5.0</h5>
                     <ul>
-                        <li><a href="http://{{ host }}/message" target="_blank">Send message from another view</a></li>
-                        <li><a href="http://{{ host }}/channels" target="_blank">Show channels</a></li>
-                        <li><a href="http://{{ host }}/channels-flush" target="_blank">Flush channels</a></li>
-                        <li><a href="http://{{ host }}/history" target="_blank">Show history</a></li>
-                        <li><a href="http://{{ host }}/history-flush" target="_blank">Flush history</a></li>
+                        <li><a href="http://{{ SOCKET }}/message" target="_blank">Send message from another view</a></li>
+                        <li><a href="http://{{ SOCKET }}/groups" target="_blank">Show groups</a></li>
+                        <li><a href="http://{{ SOCKET }}/groups-flush" target="_blank">Flush groups</a></li>
+                        <li><a href="http://{{ SOCKET }}/history" target="_blank">Show history</a></li>
+                        <li><a href="http://{{ SOCKET }}/history-flush" target="_blank">Flush history</a></li>
                     </ul>
                 </div>
                 <div class"card-body">   
                     <div class="p-3">                 
                         <form onsubmit="sendMessage(event)">
                             <div class="mb-3">
                                 <label for="username" class="form-label">Username</label>
@@ -69,17 +73,17 @@
                     <div class="p-3"> 
                         <div id="messages">
                         </div>
                     </div>
                 </div>
             </div>
             <script>
-                var ws = new WebSocket("wss://{{ host }}/chat_ws?channel_name=MySimpleChat"); 
+                var ws = new WebSocket("ws://{{ SOCKET }}/chat_ws?group_name=MyChat"); 
                 ws.onopen = function(event) {
-                    console.log('Connected to websocket. Channel MySimpleChat is open now.')
+                    console.log('Connected to websocket. Channel MyChat is open now.')
                 };
                 ws.onmessage = function(event) {
                     console.log('Message received %s', event.data)
                     var messages = document.getElementById('messages');
                     var message = document.createElement('div');
                     var data = JSON.parse(event.data);
                     message.innerHTML = `<strong>${data.username} :</strong> ${data.message}`;
@@ -99,39 +103,45 @@
             </script>
         </div>
     </body>
 </html>
 """
 
 class Chat(HTTPEndpoint):
-    async def get(self, request):   
+    async def get(self, request):  
+        sprint('Chat.get', c="green")    
         template = Template(html_text)      
-        return HTMLResponse(template.render(host=HOST))
+        return HTMLResponse(template.render(SOCKET=SOCKET))
 
 class Message(HTTPEndpoint):
-    async def get(self, request):     
-        await channel_box.channel_send(channel_name="MySimpleChat", payload={"username": "Message HTTPEndpoint", "message": "hello from Message"}, history=True)   
+    async def get(self, request):   
+        sprint('Message.get', c="green")          
+        await ChannelBox.group_send(group_name="MyChat", payload={"username": "Any part of your code", "message": "Hello World"}, history=True)   
         return JSONResponse({"message": "success"})
 
-class Channels(HTTPEndpoint):
-    async def get(self, request):                 
-        channels = await channel_box.channels()
-        return HTMLResponse(f"{channels}")
-
-class ChannelsFlush(HTTPEndpoint):
-    async def get(self, request):   
-        await channel_box.channels_flush()            
+class Groups(HTTPEndpoint):
+    async def get(self, request):  
+        sprint('Groups.get', c="green")                 
+        groups = await ChannelBox.groups()
+        return HTMLResponse(f"{groups}")
+
+class GroupsFlush(HTTPEndpoint):
+    async def get(self, request): 
+        sprint('GroupsFlush.get', c="green")    
+        await ChannelBox.groups_flush()            
         return JSONResponse({"flush": "success"})   
 
 class History(HTTPEndpoint):
-    async def get(self, request):      
-        history = await channel_box.history()
+    async def get(self, request):   
+        sprint('History.get', c="green")   
+        history = await ChannelBox.history()
         return HTMLResponse(f"{history}")
 
 class HistoryFlush(HTTPEndpoint):
     async def get(self, request):  
-        await channel_box.history_flush()             
+        sprint('HistoryFlush.get', c="green")
+        await ChannelBox.history_flush()             
         return JSONResponse({"flush": "success"})
```

## Comparing `channel_box-0.4.0.dist-info/LICENSE` & `channel_box-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

