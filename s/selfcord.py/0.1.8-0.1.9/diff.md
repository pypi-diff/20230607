# Comparing `tmp/selfcord.py-0.1.8.tar.gz` & `tmp/selfcord.py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.1.8.tar", last modified: Tue May 30 16:51:20 2023, max compression
+gzip compressed data, was "selfcord.py-0.1.9.tar", last modified: Thu Jun  1 19:05:19 2023, max compression
```

## Comparing `selfcord.py-0.1.8.tar` & `selfcord.py-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.274997 selfcord.py-0.1.8/selfcord/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.274997 selfcord.py-0.1.8/selfcord/api/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14582 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.274997 selfcord.py-0.1.8/selfcord/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/voice/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)    22236 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/selfcord/models/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/selfcord/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.274997 selfcord.py-0.1.8/selfcord.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-30 16:51:20.000000 selfcord.py-0.1.8/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-30 16:51:20.000000 selfcord.py-0.1.8/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:51:20.000000 selfcord.py-0.1.8/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 16:51:20.000000 selfcord.py-0.1.8/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 16:51:20.000000 selfcord.py-0.1.8/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.860261 selfcord.py-0.1.9/selfcord/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.864261 selfcord.py-0.1.9/selfcord/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21938 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.864261 selfcord.py-0.1.9/selfcord/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/voice/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22255 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/selfcord/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/selfcord/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.860261 selfcord.py-0.1.9/selfcord.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-01 19:05:19.000000 selfcord.py-0.1.9/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-01 19:05:19.000000 selfcord.py-0.1.9/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:05:19.000000 selfcord.py-0.1.9/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 19:05:19.000000 selfcord.py-0.1.9/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 19:05:19.000000 selfcord.py-0.1.9/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/tests/test_commands.py
```

### Comparing `selfcord.py-0.1.8/PKG-INFO` & `selfcord.py-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.8 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.9 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
```

### Comparing `selfcord.py-0.1.8/README.md` & `selfcord.py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/api/errors.py` & `selfcord.py-0.1.9/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/api/events.py` & `selfcord.py-0.1.9/selfcord/api/events.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 from __future__ import annotations
 
 import asyncio
 import time
 from time import perf_counter
 from typing import TYPE_CHECKING
 
-from ..models import (Client, DMChannel, GroupChannel, Guild, Message,
-                      TextChannel, User, VoiceChannel)
+from aioconsole import aprint
+
+from ..models import (
+    Client,
+    DMChannel,
+    GroupChannel,
+    Guild,
+    Message,
+    TextChannel,
+    User,
+    VoiceChannel,
+)
 from ..models.role import Role
 from ..utils import logging
 from .voice import Voice
 
 if TYPE_CHECKING:
     from ..bot import Bot
     from .http import http
@@ -302,14 +312,38 @@
             if role.get("guild_id") == guild.id:
                 for role in guild.roles:
                     if role.get("id") == role.id:
                         await self.bot.emit("role_delete", role)
                         guild.roles.remove(role)
                         return
 
+    async def handle_call_update(self, data: dict, user: Client, http: http):
+        channel = self.bot.get_channel(data["channel_id"])
+        region = data.get("region")
+        if isinstance(channel, DMChannel):
+            users = channel.recipient
+        elif isinstance(channel, GroupChannel):
+            users = channel.recipients
+
+        await self.bot.emit("call_update", channel, users, region)
+
+    async def handle_call_create(self, data: dict, user: Client, http: http):
+        channel = self.bot.get_channel(data["channel_id"])
+        region = data.get("region")
+        if isinstance(channel, DMChannel):
+            users = channel.recipient
+        elif isinstance(channel, GroupChannel):
+            users = channel.recipients
+
+        await self.bot.emit("call_create", channel, users, region)
+
+    async def handle_call_delete(self, data: dict, user: Client, http: http):
+        channel = self.bot.get_channel(data["channel_id"])
+        await self.bot.emit("call_delete", channel)
+
     async def handle_voice_state_update(self, data: dict, user: Client, http: http):
         """Handles the voice state updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
```

### Comparing `selfcord.py-0.1.8/selfcord/api/gateway.py` & `selfcord.py-0.1.9/selfcord/api/gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,15 +458,14 @@
         Args:
             payload (dict): Valid payload to send to the gateway
         """
         await self.ws.send(json.dumps(payload))
 
     async def reconnect(self, seq: int):
         """Reconnect to discord gateway"""
-        print(self.bot.resume_url)
         self.ws = await websockets.connect(
             f"{self.bot.resume_url}?encoding=json&v=9&compress=zlib-stream"
         )
         payload = {
             "op": 6,
             "d": {"token": self.token, "session_id": self.bot.session_id, "seq": seq},
         }
```

### Comparing `selfcord.py-0.1.8/selfcord/api/http.py` & `selfcord.py-0.1.9/selfcord/api/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,23 @@
             "Sec-Fetch-Site": "same-origin",
             "origin": "https://discord.com",
             "x-debug-options": "logGatewayEvents,logOverlayEvents,logAnalyticsEvents,bugReporterEnabled",
             "x-fingerprint": self.fingerprint,
             "TE": "trailers",
         }
 
-        async with ClientSession(headers=headers) as session:
+        async with ClientSession(
+            timeout=aiohttp.ClientTimeout(
+                total=10000, connect=10000, sock_read=10000, sock_connect=10000
+            ),
+            connector=aiohttp.TCPConnector(
+                limit=0, limit_per_host=0, ttl_dns_cache=300
+            ),
+            headers=headers,
+        ) as session:
             request = getattr(session, method)
             while True:
                 async with request(url, *args, **kwargs) as resp:
                     if self.debug:
                         log.debug(f"Sent Request URL: {url} Payload: {args} {kwargs}")
 
                     if resp.status == 429:
```

### Comparing `selfcord.py-0.1.8/selfcord/api/voice/voice.py` & `selfcord.py-0.1.9/selfcord/api/voice/voice.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/bot.py` & `selfcord.py-0.1.9/selfcord/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .api import Activity, gateway, http
 from .models import (
     Client,
     DMChannel,
     GroupChannel,
     Guild,
     InteractionUtil,
+    Option,
     Search,
     SlashCommand,
     TextChannel,
     User,
     VoiceChannel,
 )
 from .utils import (
@@ -364,15 +365,15 @@
             log.error(f"Failed to load extension events\n{error}")
 
     async def trigger_slash(
         self,
         command: SlashCommand,
         channel_id: str,
         bot_id: str,
-        value: list[str] | None = None,
+        value: list[str | None] | None = None,
         option: list[Option] | None = None,
         guild_id: str | None = None,
     ):
         interaction = InteractionUtil(self, self.http)
         await interaction.trigger_slash(
             command, channel_id, bot_id, value, option, guild_id
         )
```

### Comparing `selfcord.py-0.1.8/selfcord/models/channel.py` & `selfcord.py-0.1.9/selfcord/models/channel.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/models/client.py` & `selfcord.py-0.1.9/selfcord/models/client.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/models/emoji.py` & `selfcord.py-0.1.9/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/models/guild.py` & `selfcord.py-0.1.9/selfcord/models/guild.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/models/interactions.py` & `selfcord.py-0.1.9/selfcord/models/interactions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import json
 import random
 import string
 import time
 from itertools import zip_longest
 from typing import TYPE_CHECKING
 
 from aioconsole import aprint
@@ -127,51 +128,63 @@
         )
 
     async def trigger_slash(
         self,
         command: SlashCommand,
         channel_id: str,
         bot_id: str,
-        value: list[str] | None = None,
+        value: list[str | None] | None = None,
         option: list[Option] | None = None,
         guild_id: str | None = None,
     ):
+        nonce = int(time.time())
         payload = {
             "type": 2,
             "application_id": bot_id,
             "channel_id": channel_id,
-            "nonce": f"{int(time.time())}",
+            "nonce": nonce,
             "session_id": self.bot.session_id,
         }
         if guild_id is not None:
             payload.update({"guild_id": guild_id})
 
         data = {
             "version": command.version,
             "id": command.id,
             "name": command.name,
             "type": command.type,
             "options": [],
             "application_command": command.raw_data,
+            "attachments": [],
         }
+        if value is not None:
+            last_val = value[-1]
         if option is not None:
             dic = {"options": []}
-            for opt, value in zip_longest(option, value):
-                dic["options"].append(
-                    {
-                        "name": opt.name,
-                        "type": opt.type,
-                        "value": value,
-                    }
-                )
+            last_opt = option[-1]
+            for index, (opt, value) in enumerate(zip_longest(option, value)):
+                if index == 0:
+                    if value is None:
+                        dic["options"].append(
+                            {"name": opt.name, "type": opt.type, "options": []}
+                        )
+                    else:
+                        dic["options"].append(
+                            {"name": opt.name, "type": opt.type, "value": value}
+                        )
+                elif value is not None:
+                    for opten in dic["options"]:
+                        opten["options"].append(
+                            {"name": opt.name, "type": opt.type, "value": value}
+                        )
 
             data.update(dic)
-        payload.update(data)
+        payload.update({"data": data})
         randstr = "".join(random.sample(string.ascii_letters + string.digits, k=16))
         boundary_val = f"----WebkitFormBoundary{randstr}"
-        req_data = f'--{boundary_val}\r\nContent-Disposition: form-data; name="payload_json"\r\n\r\n{payload}\r\n--{boundary_val}'
+        req_data = f'--{boundary_val}\r\nContent-Disposition: form-data; name="payload_json"\r\n\r\n{json.dumps(payload)}\r\n--{boundary_val}--'
         await self.http.request(
             "post",
             "/interactions",
             headers={"content-type": f"multipart/form-data; boundary={boundary_val}"},
             data=req_data,
         )
```

### Comparing `selfcord.py-0.1.8/selfcord/models/member.py` & `selfcord.py-0.1.9/selfcord/models/member.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/models/message.py` & `selfcord.py-0.1.9/selfcord/models/message.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/models/permission.py` & `selfcord.py-0.1.9/selfcord/models/permission.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/models/role.py` & `selfcord.py-0.1.9/selfcord/models/role.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/models/user.py` & `selfcord.py-0.1.9/selfcord/models/user.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/models/webhook.py` & `selfcord.py-0.1.9/selfcord/models/webhook.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/utils/command.py` & `selfcord.py-0.1.9/selfcord/utils/command.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord/utils/logging.py` & `selfcord.py-0.1.9/selfcord/utils/logging.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.1.9/selfcord.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.8 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.9 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
```

### Comparing `selfcord.py-0.1.8/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.1.9/selfcord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.8/setup.py` & `selfcord.py-0.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                 "selfcord",
                 "selfcord.api",
                 "selfcord.utils",
                 "selfcord.models",
                 "selfcord.api.voice",
             ]
         ),
-        version="0.1.8",
+        version="0.1.9",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell",
         extras_require={"voice": ["pynacl==1.5.0", "opuslib==3.0.1"]},
         license="MIT",
         install_requires=[
             "aiohttp==3.7.4.post0",
```

