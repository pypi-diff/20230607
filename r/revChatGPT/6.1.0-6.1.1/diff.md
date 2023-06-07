# Comparing `tmp/revChatGPT-6.1.0.tar.gz` & `tmp/revChatGPT-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.1.0.tar", last modified: Tue Jun  6 16:24:18 2023, max compression
+gzip compressed data, was "revChatGPT-6.1.1.tar", last modified: Wed Jun  7 16:33:19 2023, max compression
```

## Comparing `revChatGPT-6.1.0.tar` & `revChatGPT-6.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.593769 revChatGPT-6.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    51072 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 16:24:18.000000 revChatGPT-6.1.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:24:18.597769 revChatGPT-6.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-06 16:23:42.000000 revChatGPT-6.1.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    52598 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 16:33:19.000000 revChatGPT-6.1.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:19.360266 revChatGPT-6.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-07 16:32:51.000000 revChatGPT-6.1.1/tests/test_recipient.py
```

### Comparing `revChatGPT-6.1.0/LICENSE` & `revChatGPT-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.0/PKG-INFO` & `revChatGPT-6.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.1.0
+Version: 6.1.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.1.0/README.md` & `revChatGPT-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.0/setup.py` & `revChatGPT-6.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.1.0",
+    version="6.1.1",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.1.0/src/revChatGPT/V1.py` & `revChatGPT-6.1.1/src/revChatGPT/V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -706,14 +706,38 @@
         url = f"{self.base_url}conversation/{convo_id}"
         response = self.session.get(url)
         self.__check_response(response)
         if encoding is not None:
             response.encoding = encoding
         return response.json()
 
+    def share_conversation(
+        self,
+        convo_id: str = None,
+        node_id: str = None,
+        anonymous: bool = True,
+    ) -> str:
+        """
+        Creates a share link to a conversation
+        :param convo_id: UUID of conversation
+        :param node_id: UUID of node
+
+        Returns:
+            str: A URL to the shared link
+        """
+        payload = {
+            "conversation_id": convo_id or self.conversation_id,
+            "current_node_id": node_id or self.parent_id,
+            "is_anonymous": anonymous,
+        }
+        url = f"{self.base_url}share/create"
+        response = self.session.post(url, data=json.dumps(payload))
+        self.__check_response(response)
+        return response.json().get("share_url")
+
     @logger(is_timed=True)
     def gen_title(self, convo_id: str, message_id: str) -> str:
         """
         Generate title for conversation
         """
         response = self.session.post(
             f"{self.base_url}conversation/gen_title/{convo_id}",
@@ -833,19 +857,19 @@
         log.debug("Sending the payload")
 
         cid, pid = data["conversation_id"], data["parent_message_id"]
         model, message = None, ""
 
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
-        async with self.session.post(
+        async with self.session.stream(
+            "POST",
             url=f"{self.base_url}conversation",
             data=json.dumps(data),
             timeout=timeout,
-            stream=True,
         ) as response:
             await self.__check_response(response)
 
             finish_details = None
             async for line in response.aiter_lines():
                 # remove b' and ' at the beginning and end and ignore case
                 line = str(line)[2:-1]
@@ -990,15 +1014,15 @@
                         print("Conversation unavailable")
                 else:
                     await self.__map_conversations()
             if conversation_id in self.conversation_mapping:
                 parent_id = self.conversation_mapping[conversation_id]
             else:
                 print(
-                    "Warning: Invalid conversation_id provided, treat as a new conversation"
+                    "Warning: Invalid conversation_id provided, treat as a new conversation",
                 )
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
 
         data = {
             "action": "next",
             "messages": messages,
@@ -1169,14 +1193,38 @@
         response = await self.session.get(url)
         if encoding is not None:
             response.encoding = encoding
             await self.__check_response(response)
             return json.loads(response.text)
         return None
 
+    async def share_conversation(
+        self,
+        convo_id: str = None,
+        node_id: str = None,
+        anonymous: bool = True,
+    ) -> str:
+        """
+        Creates a share link to a conversation
+        :param convo_id: UUID of conversation
+        :param node_id: UUID of node
+
+        Returns:
+            str: A URL to the shared link
+        """
+        payload = {
+            "conversation_id": convo_id or self.conversation_id,
+            "current_node_id": node_id or self.parent_id,
+            "is_anonymous": anonymous,
+        }
+        url = f"{self.base_url}share/create"
+        response = await self.session.post(url, data=json.dumps(payload))
+        await self.__check_response(response)
+        return response.json().get("share_url")
+
     async def gen_title(self, convo_id: str, message_id: str) -> None:
         """
         Generate title for conversation
         """
         url = f"{self.base_url}conversation/gen_title/{convo_id}"
         response = await self.session.post(
             url,
```

### Comparing `revChatGPT-6.1.0/src/revChatGPT/V3.py` & `revChatGPT-6.1.1/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.0/src/revChatGPT/__init__.py` & `revChatGPT-6.1.1/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.0/src/revChatGPT/__main__.py` & `revChatGPT-6.1.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.1.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.0/src/revChatGPT/typings.py` & `revChatGPT-6.1.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.0/src/revChatGPT/utils.py` & `revChatGPT-6.1.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.1.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.1.0
+Version: 6.1.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.1.0/tests/test_recipient.py` & `revChatGPT-6.1.1/tests/test_recipient.py`

 * *Files identical despite different names*

