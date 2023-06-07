# Comparing `tmp/revChatGPT-6.1.1.tar.gz` & `tmp/revChatGPT-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.1.1.tar", last modified: Wed Jun  7 16:33:19 2023, max compression
+gzip compressed data, was "revChatGPT-6.1.2.tar", last modified: Wed Jun  7 17:13:41 2023, max compression
```

## Comparing `revChatGPT-6.1.1.tar` & `revChatGPT-6.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    52598 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.256803 revChatGPT-6.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    54723 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 17:13:41.000000 revChatGPT-6.1.2/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:13:41.260803 revChatGPT-6.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-07 17:13:12.000000 revChatGPT-6.1.2/tests/test_recipient.py
```

### Comparing `revChatGPT-6.1.1/LICENSE` & `revChatGPT-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.1/PKG-INFO` & `revChatGPT-6.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.1.1
+Version: 6.1.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.1.1/README.md` & `revChatGPT-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.1/setup.py` & `revChatGPT-6.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.1.1",
+    version="6.1.2",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.1.1/src/revChatGPT/V1.py` & `revChatGPT-6.1.2/src/revChatGPT/V1.py`

 * *Files 4% similar despite different names*

```diff
@@ -708,35 +708,58 @@
         self.__check_response(response)
         if encoding is not None:
             response.encoding = encoding
         return response.json()
 
     def share_conversation(
         self,
+        title: str = None,
         convo_id: str = None,
         node_id: str = None,
         anonymous: bool = True,
     ) -> str:
         """
         Creates a share link to a conversation
         :param convo_id: UUID of conversation
         :param node_id: UUID of node
 
         Returns:
             str: A URL to the shared link
         """
+        convo_id = convo_id or self.conversation_id
+        node_id = node_id or self.parent_id
+        headers = {
+            "Content-Type": "application/json",
+            "origin": "https://chat.openai.com",
+            "referer": f"https://chat.openai.com/c/{convo_id}",
+        }
+        # First create the share
         payload = {
-            "conversation_id": convo_id or self.conversation_id,
-            "current_node_id": node_id or self.parent_id,
+            "conversation_id": convo_id,
+            "current_node_id": node_id,
             "is_anonymous": anonymous,
         }
         url = f"{self.base_url}share/create"
-        response = self.session.post(url, data=json.dumps(payload))
+        response = self.session.post(url, data=json.dumps(payload), headers=headers)
+        self.__check_response(response)
+        share_url = response.json().get("share_url")
+        # Then patch the share to make public
+        share_id = response.json().get("share_id")
+        url = f"{self.base_url}share/{share_id}"
+        payload = {
+            "share_id": share_id,
+            "highlighted_message_id": node_id,
+            "title": title or response.json().get("title", "New chat"),
+            "is_public": True,
+            "is_visible": True,
+            "is_anonymous": True,
+        }
+        response = self.session.patch(url, data=json.dumps(payload), headers=headers)
         self.__check_response(response)
-        return response.json().get("share_url")
+        return share_url
 
     @logger(is_timed=True)
     def gen_title(self, convo_id: str, message_id: str) -> str:
         """
         Generate title for conversation
         """
         response = self.session.post(
@@ -1195,35 +1218,66 @@
             response.encoding = encoding
             await self.__check_response(response)
             return json.loads(response.text)
         return None
 
     async def share_conversation(
         self,
+        title: str = None,
         convo_id: str = None,
         node_id: str = None,
         anonymous: bool = True,
     ) -> str:
         """
         Creates a share link to a conversation
         :param convo_id: UUID of conversation
         :param node_id: UUID of node
 
         Returns:
             str: A URL to the shared link
         """
+        convo_id = convo_id or self.conversation_id
+        node_id = node_id or self.parent_id
+        headers = {
+            "Content-Type": "application/json",
+            "origin": "https://chat.openai.com",
+            "referer": f"https://chat.openai.com/c/{convo_id}",
+        }
+        # First create the share
         payload = {
-            "conversation_id": convo_id or self.conversation_id,
-            "current_node_id": node_id or self.parent_id,
+            "conversation_id": convo_id,
+            "current_node_id": node_id,
             "is_anonymous": anonymous,
         }
         url = f"{self.base_url}share/create"
-        response = await self.session.post(url, data=json.dumps(payload))
+        response = await self.session.post(
+            url,
+            data=json.dumps(payload),
+            headers=headers,
+        )
+        await self.__check_response(response)
+        share_url = response.json().get("share_url")
+        # Then patch the share to make public
+        share_id = response.json().get("share_id")
+        url = f"{self.base_url}share/{share_id}"
+        payload = {
+            "share_id": share_id,
+            "highlighted_message_id": node_id,
+            "title": title or response.json().get("title", "New chat"),
+            "is_public": True,
+            "is_visible": True,
+            "is_anonymous": True,
+        }
+        response = await self.session.patch(
+            url,
+            data=json.dumps(payload),
+            headers=headers,
+        )
         await self.__check_response(response)
-        return response.json().get("share_url")
+        return share_url
 
     async def gen_title(self, convo_id: str, message_id: str) -> None:
         """
         Generate title for conversation
         """
         url = f"{self.base_url}conversation/gen_title/{convo_id}"
         response = await self.session.post(
@@ -1330,14 +1384,15 @@
             !help - Show this message
             !reset - Forget the current conversation
             !config - Show the current configuration
             !plugins - Show the current plugins
             !switch x - Switch to plugin x. Need to reset the conversation to ativate the plugin.
             !rollback x - Rollback the conversation (x being the number of messages to rollback)
             !setconversation - Changes the conversation
+            !share - Creates a share link to the current conversation
             !exit - Exit this program
             """,
             )
         elif command == "!reset":
             chatbot.reset_chat()
             print("Chat session successfully reset.")
         elif command == "!config":
@@ -1371,14 +1426,16 @@
             prev_text = ""
             for data in chatbot.continue_write():
                 message = data["message"][len(prev_text) :]
                 print(message, end="", flush=True)
                 prev_text = data["message"]
             print(bcolors.ENDC)
             print()
+        elif command.startswith("!share"):
+            print(f"Conversation shared at {chatbot.share_conversation()}")
         elif command == "!exit":
             if isinstance(chatbot.session, httpx.AsyncClient):
                 chatbot.session.aclose()
             exit()
         else:
             return False
         return True
@@ -1391,14 +1448,15 @@
             "!config",
             "!rollback",
             "!exit",
             "!setconversation",
             "!continue",
             "!plugins",
             "!switch",
+            "!share",
         ],
     )
     print()
     try:
         result = {}
         while True:
             print(f"{bcolors.OKBLUE + bcolors.BOLD}You: {bcolors.ENDC}")
```

### Comparing `revChatGPT-6.1.1/src/revChatGPT/V3.py` & `revChatGPT-6.1.2/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.1/src/revChatGPT/__init__.py` & `revChatGPT-6.1.2/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.1/src/revChatGPT/__main__.py` & `revChatGPT-6.1.2/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.1/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.1.2/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.1/src/revChatGPT/typings.py` & `revChatGPT-6.1.2/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.1/src/revChatGPT/utils.py` & `revChatGPT-6.1.2/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.1/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.1.2/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.1.1
+Version: 6.1.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.1.1/tests/test_recipient.py` & `revChatGPT-6.1.2/tests/test_recipient.py`

 * *Files identical despite different names*

