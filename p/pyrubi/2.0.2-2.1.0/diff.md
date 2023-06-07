# Comparing `tmp/pyrubi-2.0.2.tar.gz` & `tmp/pyrubi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubi-2.0.2.tar", last modified: Mon Apr 24 17:39:36 2023, max compression
+gzip compressed data, was "pyrubi-2.1.0.tar", last modified: Wed Jun  7 14:39:14 2023, max compression
```

## Comparing `pyrubi-2.0.2.tar` & `pyrubi-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:36.299052 pyrubi-2.0.2/
--rw-rw-rw-   0        0        0     1747 2023-04-24 17:39:36.298052 pyrubi-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      927 2023-04-24 17:38:54.000000 pyrubi-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:36.260890 pyrubi-2.0.2/pyrubi/
--rw-rw-rw-   0        0        0      246 2023-04-24 17:38:16.000000 pyrubi-2.0.2/pyrubi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:36.270668 pyrubi-2.0.2/pyrubi/cryption/
--rw-rw-rw-   0        0        0     1194 2023-02-10 12:30:31.000000 pyrubi-2.0.2/pyrubi/cryption/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:36.271672 pyrubi-2.0.2/pyrubi/handler/
--rw-rw-rw-   0        0        0     1544 2023-04-16 13:37:06.000000 pyrubi-2.0.2/pyrubi/handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:36.273672 pyrubi-2.0.2/pyrubi/maker/
--rw-rw-rw-   0        0        0     2885 2023-04-20 11:49:58.000000 pyrubi-2.0.2/pyrubi/maker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:36.274671 pyrubi-2.0.2/pyrubi/message/
--rw-rw-rw-   0        0        0     4687 2023-04-20 12:26:50.000000 pyrubi-2.0.2/pyrubi/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:36.284788 pyrubi-2.0.2/pyrubi/methods/
--rw-rw-rw-   0        0        0    43171 2023-04-24 16:52:37.000000 pyrubi-2.0.2/pyrubi/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:36.286929 pyrubi-2.0.2/pyrubi/servers/
--rw-rw-rw-   0        0        0      334 2023-03-08 18:29:05.000000 pyrubi-2.0.2/pyrubi/servers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:36.297053 pyrubi-2.0.2/pyrubi/tools/
--rw-rw-rw-   0        0        0     4361 2023-03-09 12:00:43.000000 pyrubi-2.0.2/pyrubi/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:36.269015 pyrubi-2.0.2/pyrubi.egg-info/
--rw-rw-rw-   0        0        0     1747 2023-04-24 17:39:36.000000 pyrubi-2.0.2/pyrubi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-04-24 17:39:36.000000 pyrubi-2.0.2/pyrubi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 17:39:36.000000 pyrubi-2.0.2/pyrubi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-04-24 17:39:36.000000 pyrubi-2.0.2/pyrubi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 17:39:36.000000 pyrubi-2.0.2/pyrubi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 17:39:36.299052 pyrubi-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1140 2023-04-24 17:39:02.000000 pyrubi-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.662299 pyrubi-2.1.0/
+-rw-rw-rw-   0        0        0     2204 2023-06-07 14:39:14.662299 pyrubi-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1404 2023-06-07 14:35:32.000000 pyrubi-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.622603 pyrubi-2.1.0/pyrubi/
+-rw-rw-rw-   0        0        0      246 2023-06-07 14:36:26.000000 pyrubi-2.1.0/pyrubi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.646796 pyrubi-2.1.0/pyrubi/cryption/
+-rw-rw-rw-   0        0        0     1194 2023-02-10 12:30:31.000000 pyrubi-2.1.0/pyrubi/cryption/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.647798 pyrubi-2.1.0/pyrubi/handler/
+-rw-rw-rw-   0        0        0     1243 2023-06-07 06:58:02.000000 pyrubi-2.1.0/pyrubi/handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.649004 pyrubi-2.1.0/pyrubi/maker/
+-rw-rw-rw-   0        0        0     3164 2023-06-07 09:01:39.000000 pyrubi-2.1.0/pyrubi/maker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.655895 pyrubi-2.1.0/pyrubi/message/
+-rw-rw-rw-   0        0        0     4687 2023-04-20 12:26:50.000000 pyrubi-2.1.0/pyrubi/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.657895 pyrubi-2.1.0/pyrubi/methods/
+-rw-rw-rw-   0        0        0    43655 2023-06-07 09:00:36.000000 pyrubi-2.1.0/pyrubi/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.659127 pyrubi-2.1.0/pyrubi/servers/
+-rw-rw-rw-   0        0        0      334 2023-05-26 15:37:31.000000 pyrubi-2.1.0/pyrubi/servers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.660136 pyrubi-2.1.0/pyrubi/tools/
+-rw-rw-rw-   0        0        0     7027 2023-06-07 09:00:54.000000 pyrubi-2.1.0/pyrubi/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.638957 pyrubi-2.1.0/pyrubi.egg-info/
+-rw-rw-rw-   0        0        0     2204 2023-06-07 14:39:14.000000 pyrubi-2.1.0/pyrubi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-06-07 14:39:14.000000 pyrubi-2.1.0/pyrubi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:39:14.000000 pyrubi-2.1.0/pyrubi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-07 14:39:14.000000 pyrubi-2.1.0/pyrubi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-07 14:39:14.000000 pyrubi-2.1.0/pyrubi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:39:14.662299 pyrubi-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1083 2023-06-07 13:59:20.000000 pyrubi-2.1.0/setup.py
```

### Comparing `pyrubi-2.0.2/PKG-INFO` & `pyrubi-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,83 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.0.2
-Summary: This is a powerful library for building self robots in Rubika
+Version: 2.1.0
+Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
-Keywords: rubika,rubino,pyrubi,pyrubika,rubika bot,rubika library,rubx,rubika-bot,rubika-lib,bot,self bot,rubika.ir
+Keywords: rubika,rubino,pyrubi,pyrubika,rubx,rubika.ir,bot,chat
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: ~=3.7
+Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.0.2</h1>
+<h1>Pyrubi 2.1.0</h1>
 
-> Pyrubi is a powerful and easy library for building self bots in Rubika
+> Pyrubi is a powerful and easy library for building self Bots in Rubika
 
+<style>
+    .image {
+        border-radius: 12px
+    }
+    h1 {
+        text-align: center;
+        color: dodgerblue;
+        font-size: 25px;
+        border-radius: 3px
+    }
+    a{
+        margin: 1px;
+        color: white;
+        background-image: linear-gradient(to right, rgb(0, 89, 255), rgb(0, 166, 255));
+        font-size: 18px;
+        border-radius: 3px
+    }
+</style>
+
+<p align='center'>
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.1.0' width='356' class="image">
+</p>
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.0.2' width='356'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
+    <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
 
 <hr>
 
 **Example:**
 ``` python
 from pyrubi import Bot, Message
 
-bot = Bot('TOKEN')
+bot = Bot("TOKEN")
 
-for msg in bot.on_message():
-    m = Message(msg)
+for update in bot.on_message():
+    message = Message(update)
     if m.text() == 'Hello':
-        bot.send_text(m.chat_id(), 'Hello from Pyrubi Library', m.message_id())
+        bot.send_text(message.chat_id(), "``Hello`` **from** __Pyrubi__ ~~Library~~, --I'm Ali--.", message.message_id())
 ```
 
 <hr>
 
 ### Features:
     
-- *Fast* : **The minimum request time is 0.07 seconds and the maximum request time is 0.3 seconds**
-- *Easy* : **All methods and features are designed as easy and optimal as possible**
-- *Powerful* : **While the library is simple, it has high speed and features that make your work easier and faster**
+- **Fast** : *The requests are very fast.*
+
+- **Easy** : *All methods and features are designed as easy and optimal as possible*
+
+- **Powerful** : *While the library is simple, it has high speed and features that make your work easier and faster*
+
 
 <hr>
 
-# Rubika : @pyrubika
+## Rubika : @pyrubika
 
 ### Install or Update:
 
 ``` bash
 pip install -U pyrubi
 ```
```

#### html2text {}

```diff
@@ -1,25 +1,27 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.0.2 Summary: This is a powerful
-library for building self robots in Rubika Home-page: https://github.com/
-AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email: ali.ganji.za@gmail.com
-Keywords: rubika,rubino,pyrubi,pyrubika,rubika bot,rubika library,rubx,rubika-
-bot,rubika-lib,bot,self bot,rubika.ir Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: License :: OSI Approved ::
-MIT License Requires-Python: ~=3.7 Description-Content-Type: text/markdown
-****** Pyrubi 2.0.2 ******
-> Pyrubi is a powerful and easy library for building self bots in Rubika
-                         [Pyrubi Library 2.0.2] GitHub
+Metadata-Version: 2.1 Name: pyrubi Version: 2.1.0 Summary: This is a powerful
+and easy library for building self Bots in Rubika Home-page: https://
+github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
+ali.ganji.za@gmail.com Keywords:
+rubika,rubino,pyrubi,pyrubika,rubx,rubika.ir,bot,chat Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: MIT License Requires-Python: ~=3.6 Description-Content-Type: text/
+markdown
+****** Pyrubi 2.1.0 ******
+> Pyrubi is a powerful and easy library for building self Bots in Rubika
+                            [Pyrubi Library 2.1.0]
+                               GitHub Documents
 ===============================================================================
-**Example:** ``` python from pyrubi import Bot, Message bot = Bot('TOKEN') for
-msg in bot.on_message(): m = Message(msg) if m.text() == 'Hello': bot.send_text
-(m.chat_id(), 'Hello from Pyrubi Library', m.message_id()) ```
+**Example:** ``` python from pyrubi import Bot, Message bot = Bot("TOKEN") for
+update in bot.on_message(): message = Message(update) if m.text() == 'Hello':
+bot.send_text(message.chat_id(), "``Hello`` **from** __Pyrubi__ ~~Library~~, --
+I'm Ali--.", message.message_id()) ```
 ===============================================================================
-### Features: - *Fast* : **The minimum request time is 0.07 seconds and the
-maximum request time is 0.3 seconds** - *Easy* : **All methods and features are
-designed as easy and optimal as possible** - *Powerful* : **While the library
-is simple, it has high speed and features that make your work easier and
-faster**
+### Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
+methods and features are designed as easy and optimal as possible* -
+**Powerful** : *While the library is simple, it has high speed and features
+that make your work easier and faster*
 ===============================================================================
-# Rubika : @pyrubika ### Install or Update: ``` bash pip install -U pyrubi ```
+## Rubika : @pyrubika ### Install or Update: ``` bash pip install -U pyrubi ```
```

### Comparing `pyrubi-2.0.2/pyrubi/cryption/__init__.py` & `pyrubi-2.1.0/pyrubi/cryption/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.0.2/pyrubi/handler/__init__.py` & `pyrubi-2.1.0/pyrubi/handler/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 from websocket import create_connection
 from json import dumps, loads
 from ..servers import get_server
 from ..cryption import cryption
-
 class handler:
 
-    def __init__(self, auth):
-        # self.server = get_server('socket')
+    def __init__(self, auth, methods):
+        self.server = get_server('socket')
         self.crypto = cryption(auth)
         self.auth = auth
+        self.methods = methods
+        self.hs_data = {
+            'api_version': '5',
+            'auth': auth,
+            'method': 'handShake'
+        }
         del auth
+        del methods
     
     def hand_shake(self):
         print('connecting to the web socket...')
-        ws = create_connection('wss://jsocket1.iranlms.ir:80/')
-        ws.send(
-            dumps(
-                {
-                    'api_version': '5',
-                    'auth': self.auth,
-                    'method': 'handShake'
-                }
-            )
-        )
+        ws = create_connection(self.server)
+        self.methods.get_me()
+        ws.send(dumps(self.hs_data))
         print('connected !')
         while True:
             try:
                 recv = loads(ws.recv())
-                if recv != {"status":"OK","status_det":"OK"}:
+                if recv != {"status":"OK", "status_det":"OK"}:
                     if recv['type'] == 'messenger':
                         yield loads(self.crypto.decrypt(recv['data_enc']))
             except:
-                print('There was a problem connecting to the web socket. Reconnecting...')
+                ws.close()
                 del ws
                 ws = create_connection(self.server)
-                ws.send(
-                    dumps(
-                        {
-                            'api_version': '5',
-                            'auth': self.auth,
-                            'method': 'handShake'
-                        }
-                    )
-                )
-                print('connected !')
+                self.methods.get_me()
+                ws.send(dumps(self.hs_data))
                 continue
```

### Comparing `pyrubi-2.0.2/pyrubi/maker/__init__.py` & `pyrubi-2.1.0/pyrubi/maker/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from ..servers import get_server
 from urllib3 import PoolManager
 from json import dumps, loads
 from requests import  post
 
 class maker:
     
-    def __init__(self, auth):
+    def __init__(self, auth, methods):
         self.auth = auth
         self.crypto = cryption(auth)
         self.http = PoolManager()
         self.server = get_server('api')
+        self.methods = methods
         self.req_clients = {
             'web': {
                 'app_name':'Main',
                 'app_version':'4.2.0',
                 'platform':'Web',
                 'package':'web.rubika.ir',
                 'lang_code':'fa'
@@ -39,34 +40,39 @@
                         'method': method,
                         'input': data,
                         'client': self.req_clients['web']
                     }
                 )
             )
         }
-        result = self.http.request(
-            'POST',
-            self.server,
-            body = dumps(data).encode(),
-            headers = {'Cookie': 'Pyrubi Library'}
-        )
-        result = loads(self.crypto.decrypt(loads(result.data.decode('utf-8'))['data_enc']))
-        if result['status'] == 'OK':
-            return result['data']
-        elif result['status'] in ['ERROR_GENERIC', 'ERROR_ACTION']:
-            for i in [
-                ('INVALID_AUTH', 'The Auth entered is invalid !'),
-                ('NOT_REGISTERED', 'Method input is not registered !'),
-                ('INVALID_INPUT', 'Invalid method input !'),
-                ('TOO_REQUESTS', 'Too much request ! Your account has been temporarily suspended.')
-            ]:
-                if result['status_det'] == i[0]:
-                    raise IndexError(i[1])
-                else:
-                    continue
+        trying = 0
+        while True:
+            result = self.http.request(
+                'POST',
+                self.server,
+                body = dumps(data).encode(),
+            )
+            result = loads(self.crypto.decrypt(loads(result.data.decode('utf-8'))['data_enc']))
+            if result['status'] == 'OK':
+                return result['data']
+            elif result['status'] in ['ERROR_GENERIC', 'ERROR_ACTION']:
+                if result['status_det'] == 'INVALID_AUTH':
+                    if trying < 3:
+                        self.methods.get_me()
+                        trying += 1
+                        continue
+                    raise ConnectionError('The Auth entered is invalid !')
+                for i in [
+                    ('NOT_REGISTERED', 'Method input is not registered !'),
+                    ('INVALID_INPUT', 'Invalid method input !'),
+                    ('TOO_REQUESTS', 'Too much request ! Your account has been suspended.')
+                ]: 
+                    if result['status_det'] == i[0]:
+                        raise ConnectionError(i[1])
+            continue
 
     def _upload(self, url, data, headers):
         while True:
             req = post(url=url, data=data, headers=headers)
             if req.status_code != 200:
                 print('This file cannot be uploaded ! Trying to upload again ...')
                 continue
```

### Comparing `pyrubi-2.0.2/pyrubi/message/__init__.py` & `pyrubi-2.1.0/pyrubi/message/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.0.2/pyrubi/methods/__init__.py` & `pyrubi-2.1.0/pyrubi/methods/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 from ..cryption import cryption
 from ..tools import tools
 from ..message import message
 from ..maker import maker
 from ..handler import handler
-from requests import post
+from requests import session
 from urllib3 import PoolManager
 from random import choice, randint
 from time import time
 from pathlib import Path
-from json import dumps, loads
 
 class methods:
 
     def __init__(self, auth):
         self.auth = auth
-        self.hs = handler(auth).hand_shake
-        self.method = maker(auth).method
+        self.hs = handler(auth, self).hand_shake
+        self.method = maker(auth, self).method
         self.crypto = cryption(auth)
         self.http = PoolManager()
         self.got_messages_update = []
-        self.filters = {
-            'chat_filter': [],
-            'message_filter': []
-        }
         del auth
 
-    def add_filter(self, chat_filter = [], message_filter = []):
-        self.filters['chat_filter'] = chat_filter
-        self.filters['message_filter'] = message_filter
 
-    def on_message(self):
+    def on_message(self, chat_filter=[], message_filter=[]):
         for recv in self.hs():
-            if 'chat_updates' in recv and not message(recv).chat_type() in self.filters['chat_filter'] and not message(recv).message_type() in self.filters['message_filter']:
+            if 'chat_updates' in recv and not message(recv).chat_type() in chat_filter and not message(recv).message_type() in message_filter:
                 yield recv
             else:
                 continue
 
-    def get_chats_update(self, save_message_ids=True):
+    def get_chats_update(self, chat_filter=[], message_filter=[], save_message_ids=True):
         while True:
-            chats_update = self.method('getChatsUpdates', {'state': round(time()) - 100})['chats'][0]
-            if not message(chats_update).chat_type() in self.filters['chat_filter'] and not message(chats_update).message_type() in self.filters['message_filter']:
-                if save_message_ids:
-                    if not message(chats_update).message_id() in self.got_messages_update:
-                        self.got_messages_update.append(message(chats_update).message_id())
+            try:
+                chats_update = self.method('getChatsUpdates', {'state': round(time()) - 200})['chats'][0]
+                if not message(chats_update).chat_type() in chat_filter and not message(chats_update).message_type() in message_filter:
+                    if save_message_ids:
+                        if not message(chats_update).message_id() in self.got_messages_update:
+                            self.got_messages_update.append(message(chats_update).message_id())
+                            yield chats_update
+                    else:
                         yield chats_update
-                else:
-                    yield chats_update
+            except IndexError:
+                continue
+
+    def get_chats_update2(self):
+        return self.method('getChatsUpdates', {'state': round(time()) - 200})['chats']
 
-    def send_text(self, chat_id, custom_text, message_id = None):
-        metadata = tools.check_metadata(custom_text)
+    def send_text(self, chat_id, text, message_id = None):
+        metadata = tools.check_metadata(text)
         data = {
             'object_guid': chat_id,
             'rnd': str(randint(10000000, 999999999)),
-            'text': metadata[1].strip(),
+            'text': metadata[1].strip() if metadata[1] != None else '????',
             'reply_to_message_id': message_id,
         }
         if metadata[0] != []:
             data['metadata'] = {'meta_data_parts': metadata[0]}
         return self.method('sendMessage', data)
 
-    def reply(self, data, custom_text):
+    def reply(self, data, text):
         msg = message(data)
         return self.send_text(
             msg.chat_id(),
-            custom_text,
-            msg.message_id()
+            text,
+            msg.message_id(),
         )
 
     def send_image(self, chat_id, file, caption = None, message_id = None, thumbnail = None):
         req = self.upload_file(file)
         file_data = req[0]
         url_data = req[1]
         size = tools.get_image_size(file if str(type(file)) == "<class 'bytes'>" else open(file,'rb').read() if not url_data else url_data.data)
@@ -158,15 +156,15 @@
         metadata = tools.check_metadata(caption)
         data = {
             'file_inline': {
                 'dc_id': file_data['dc_id'],
                 'file_id': file_data['id'],
                 'type': 'Voice',
                 'file_name': f'Pyrubi {randint(1, 100)}.ogg' if url_data or str(type(file)) == "<class 'bytes'>" else file,
-                'size': str(len(url_data.data)) if url_data else str(Path(file).stat().st_size),
+                'size': str(len(url_data.data)) if url_data else str(len(file)) if str(type(file)) == "<class 'bytes'>" else str(Path(file).stat().st_size),
                 'time': 1 if url_data or str(type(file)) == "<class 'bytes'>" else int(tools.get_voice_duration(open(file,'rb').read()) if time == None else time) * 1000,
                 'mime': 'ogg',
                 'access_hash_rec': req[2],
             },
             'object_guid': chat_id,
             'rnd': str(randint(100000,999999999)),
             'reply_to_message_id': message_id,
@@ -763,15 +761,15 @@
             {
                 'phone': f'98{tools.parse_phone_number(phone_number)}',
                 'first_name': first_name,
                 'last_name': last_name
             }
         )
 
-    def get_chat_folders(self):
+    def get_folders(self):
         return self.method('getFolders', {})
 
     def get_suggested_folders(self):
         return self.method('getSuggestedFolders', {})
 
     def add_chat_folder(self, folder_name, exclude_chat_ids = [], exclude_chat_types = [], include_chat_ids = [], include_chat_types = [], add_to_top = True, folder_id = ''):
         data = dict(
@@ -833,54 +831,72 @@
         return self.method(
             'verifyRecoveryEmail',
             {
                 'password': current_password,
                 'code': verification_code
             }            
         )
+    
+    def get_sticker_sets(self):
+        return self.method('getMyStickerSets', {})
 
     def get_me(self):
-        return loads(
-            self.http.request(
-                'POST',
-                'https://messengerg2c1.iranlms.ir',
-                body=dumps(
-                    {
-                        'data': {},
-                        'method': 'getUser',
-                        'api_version': '2',
-                        'auth': self.auth,
-                        'client': {
-                            'app_name': 'Mian',
-                            'package': 'm.rubika.ir',
-                            'app_version': '1.2.1',
-                            'platform': 'PWA'
-                        }
-                    },
-                ),
-                headers = {'Cookie': 'Pyrubi Library'}
-            ).data.decode('utf-8')
-        )['data']['user']
+        session().close()
+        return session().post(
+            'https://messengerg2c1.iranlms.ir',
+            json={
+                "data":{},
+                "method":"getUser",
+                "api_version":"2",
+                "auth": self.auth,
+                "Messenger":{
+                    "app_name":"Main",
+                    "package":"m.rubika.ir",
+                    "app_version":"1.2.1",
+                    "platform":"PWA"
+                }
+            },
+            headers = {
+                'referer': 'https://web.rubika.ir/',
+            }
+        ).json()
     
     def get_base_info(self):
-        return post(
+        return session().post(
             'https://servicesbase.iranlms.ir/',
             json={
                 'method':'getBaseInfo',
                 'api_version':'0',
                 'data':{},
                 'auth': self.auth,
                 'client':{
                     'app_name':'Main',
                     'app_version':'4.2.0',
                     'platform':'PWA',
                     'package':'web.rubika.ir'
                 }
             }
         ).json()
+    
+    def get_tag_list(self):
+        return session().post(
+            'https://services3.iranlms.ir/',
+            json={
+                'method':'getTagList',
+                'api_version':'0',
+                'data':{'taglist_id': 'new_vod'},
+                'auth': self.auth,
+                'client':{
+                    'app_name':'Main',
+                    'app_version':'4.2.0',
+                    'platform':'PWA',
+                    'package':'web.rubika.ir'
+                }
+            }
+        ).json()
 
     def edit_profile(self, **kwargs):
         """
         parameters : first_name, last_name, bio, username
         """
         if 'username' in list(kwargs.keys()):
             return self.method(
@@ -964,15 +980,15 @@
             }
         ), url_data
 
     def upload_file(self, file):
         req = self.request_file(file)
         file_data = req[0]
         url_data = req[1]
-        upload = maker(self.auth)._upload
+        upload = maker(self.auth, self)._upload
         bytef = url_data.data if url_data else file if str(type(file)) == "<class 'bytes'>" else open(file,'rb').read()
         size = str(len(url_data.data)) if url_data else str(len(file)) if str(type(file)) == "<class 'bytes'>" else str(Path(file).stat().st_size)
         url = file_data['upload_url']
         header = {
             'auth': self.auth,
             'Host': file_data['upload_url'].replace('https://','').replace('/UploadFile.ashx',''),
             'chunk-size': size,
```

### Comparing `pyrubi-2.0.2/pyrubi.egg-info/PKG-INFO` & `pyrubi-2.1.0/pyrubi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,83 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.0.2
-Summary: This is a powerful library for building self robots in Rubika
+Version: 2.1.0
+Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
-Keywords: rubika,rubino,pyrubi,pyrubika,rubika bot,rubika library,rubx,rubika-bot,rubika-lib,bot,self bot,rubika.ir
+Keywords: rubika,rubino,pyrubi,pyrubika,rubx,rubika.ir,bot,chat
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: ~=3.7
+Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.0.2</h1>
+<h1>Pyrubi 2.1.0</h1>
 
-> Pyrubi is a powerful and easy library for building self bots in Rubika
+> Pyrubi is a powerful and easy library for building self Bots in Rubika
 
+<style>
+    .image {
+        border-radius: 12px
+    }
+    h1 {
+        text-align: center;
+        color: dodgerblue;
+        font-size: 25px;
+        border-radius: 3px
+    }
+    a{
+        margin: 1px;
+        color: white;
+        background-image: linear-gradient(to right, rgb(0, 89, 255), rgb(0, 166, 255));
+        font-size: 18px;
+        border-radius: 3px
+    }
+</style>
+
+<p align='center'>
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.1.0' width='356' class="image">
+</p>
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.0.2' width='356'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
+    <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
 
 <hr>
 
 **Example:**
 ``` python
 from pyrubi import Bot, Message
 
-bot = Bot('TOKEN')
+bot = Bot("TOKEN")
 
-for msg in bot.on_message():
-    m = Message(msg)
+for update in bot.on_message():
+    message = Message(update)
     if m.text() == 'Hello':
-        bot.send_text(m.chat_id(), 'Hello from Pyrubi Library', m.message_id())
+        bot.send_text(message.chat_id(), "``Hello`` **from** __Pyrubi__ ~~Library~~, --I'm Ali--.", message.message_id())
 ```
 
 <hr>
 
 ### Features:
     
-- *Fast* : **The minimum request time is 0.07 seconds and the maximum request time is 0.3 seconds**
-- *Easy* : **All methods and features are designed as easy and optimal as possible**
-- *Powerful* : **While the library is simple, it has high speed and features that make your work easier and faster**
+- **Fast** : *The requests are very fast.*
+
+- **Easy** : *All methods and features are designed as easy and optimal as possible*
+
+- **Powerful** : *While the library is simple, it has high speed and features that make your work easier and faster*
+
 
 <hr>
 
-# Rubika : @pyrubika
+## Rubika : @pyrubika
 
 ### Install or Update:
 
 ``` bash
 pip install -U pyrubi
 ```
```

#### html2text {}

```diff
@@ -1,25 +1,27 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.0.2 Summary: This is a powerful
-library for building self robots in Rubika Home-page: https://github.com/
-AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email: ali.ganji.za@gmail.com
-Keywords: rubika,rubino,pyrubi,pyrubika,rubika bot,rubika library,rubx,rubika-
-bot,rubika-lib,bot,self bot,rubika.ir Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: License :: OSI Approved ::
-MIT License Requires-Python: ~=3.7 Description-Content-Type: text/markdown
-****** Pyrubi 2.0.2 ******
-> Pyrubi is a powerful and easy library for building self bots in Rubika
-                         [Pyrubi Library 2.0.2] GitHub
+Metadata-Version: 2.1 Name: pyrubi Version: 2.1.0 Summary: This is a powerful
+and easy library for building self Bots in Rubika Home-page: https://
+github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
+ali.ganji.za@gmail.com Keywords:
+rubika,rubino,pyrubi,pyrubika,rubx,rubika.ir,bot,chat Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: MIT License Requires-Python: ~=3.6 Description-Content-Type: text/
+markdown
+****** Pyrubi 2.1.0 ******
+> Pyrubi is a powerful and easy library for building self Bots in Rubika
+                            [Pyrubi Library 2.1.0]
+                               GitHub Documents
 ===============================================================================
-**Example:** ``` python from pyrubi import Bot, Message bot = Bot('TOKEN') for
-msg in bot.on_message(): m = Message(msg) if m.text() == 'Hello': bot.send_text
-(m.chat_id(), 'Hello from Pyrubi Library', m.message_id()) ```
+**Example:** ``` python from pyrubi import Bot, Message bot = Bot("TOKEN") for
+update in bot.on_message(): message = Message(update) if m.text() == 'Hello':
+bot.send_text(message.chat_id(), "``Hello`` **from** __Pyrubi__ ~~Library~~, --
+I'm Ali--.", message.message_id()) ```
 ===============================================================================
-### Features: - *Fast* : **The minimum request time is 0.07 seconds and the
-maximum request time is 0.3 seconds** - *Easy* : **All methods and features are
-designed as easy and optimal as possible** - *Powerful* : **While the library
-is simple, it has high speed and features that make your work easier and
-faster**
+### Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
+methods and features are designed as easy and optimal as possible* -
+**Powerful** : *While the library is simple, it has high speed and features
+that make your work easier and faster*
 ===============================================================================
-# Rubika : @pyrubika ### Install or Update: ``` bash pip install -U pyrubi ```
+## Rubika : @pyrubika ### Install or Update: ``` bash pip install -U pyrubi ```
```

### Comparing `pyrubi-2.0.2/setup.py` & `pyrubi-2.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pyrubi',
-    version = '2.0.2',
+    version = '2.1.0',
     author='Ali Ganji zadeh',
     author_email = 'ali.ganji.za@gmail.com',
-    description = 'This is a powerful library for building self robots in Rubika',
-    keywords = ['rubika', 'rubino', 'pyrubi', 'pyrubika', 'rubika bot', 'rubika library', 'rubx', 'rubika-bot', 'rubika-lib', 'bot', 'self bot', 'rubika.ir'],
+    description = 'This is a powerful and easy library for building self Bots in Rubika',
+    keywords = ['rubika', 'rubino', 'pyrubi', 'pyrubika', 'rubx', 'rubika.ir', 'bot', 'chat'],
     long_description = open("README.md", encoding="utf-8").read(),
-    python_requires="~=3.7",
+    python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/AliGanji1/pyrubi',
     packages = find_packages(),
     install_requires = ['pycryptodome', 'websocket-client', 'requests', 'aiohttp', 'urllib3', 'pillow', 'mutagen', 'tinytag'],
     classifiers = [
     	"Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

