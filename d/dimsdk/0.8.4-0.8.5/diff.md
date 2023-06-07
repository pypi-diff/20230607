# Comparing `tmp/dimsdk-0.8.4.tar.gz` & `tmp/dimsdk-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimsdk-0.8.4.tar", last modified: Sat Jan 21 10:24:07 2023, max compression
+gzip compressed data, was "dist/dimsdk-0.8.5.tar", last modified: Wed Jun  7 17:03:46 2023, max compression
```

## Comparing `dimsdk-0.8.4.tar` & `dimsdk-0.8.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-01-21 10:24:07.000000 dimsdk-0.8.4/
--rw-r--r--   0 moky       (501) staff       (20)     1047 2023-01-21 10:24:07.000000 dimsdk-0.8.4/PKG-INFO
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-01-21 10:24:07.000000 dimsdk-0.8.4/dimsdk.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1047 2023-01-21 10:24:07.000000 dimsdk-0.8.4/dimsdk.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      635 2023-01-21 10:24:07.000000 dimsdk-0.8.4/dimsdk.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)       37 2023-01-21 10:24:07.000000 dimsdk-0.8.4/dimsdk.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        7 2023-01-21 10:24:07.000000 dimsdk-0.8.4/dimsdk.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-01-21 10:24:07.000000 dimsdk-0.8.4/dimsdk.egg-info/dependency_links.txt
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-01-21 10:24:07.000000 dimsdk-0.8.4/dimsdk/
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-01-21 10:24:07.000000 dimsdk-0.8.4/dimsdk/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2278 2023-01-20 15:43:54.000000 dimsdk-0.8.4/dimsdk/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4706 2023-01-20 15:57:47.000000 dimsdk-0.8.4/dimsdk/cpu/factory.py
--rw-r--r--   0 moky       (501) staff       (20)     4547 2022-11-18 09:12:37.000000 dimsdk-0.8.4/dimsdk/cpu/customized.py
--rw-r--r--   0 moky       (501) staff       (20)     4059 2022-07-27 14:40:00.000000 dimsdk-0.8.4/dimsdk/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     2490 2022-07-31 12:08:34.000000 dimsdk-0.8.4/dimsdk/cpu/forward.py
--rw-r--r--   0 moky       (501) staff       (20)     3608 2023-01-20 15:57:15.000000 dimsdk-0.8.4/dimsdk/cpu/creator.py
--rw-r--r--   0 moky       (501) staff       (20)     2354 2022-07-31 12:26:10.000000 dimsdk-0.8.4/dimsdk/cpu/array.py
--rw-r--r--   0 moky       (501) staff       (20)     2887 2023-01-20 15:57:25.000000 dimsdk-0.8.4/dimsdk/cpu/base.py
--rw-r--r--   0 moky       (501) staff       (20)     3283 2022-07-27 14:40:39.000000 dimsdk-0.8.4/dimsdk/cpu/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5866 2023-01-20 16:35:59.000000 dimsdk-0.8.4/dimsdk/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7106 2023-01-20 15:59:10.000000 dimsdk-0.8.4/dimsdk/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     8455 2023-01-20 16:12:28.000000 dimsdk-0.8.4/dimsdk/factories.py
--rw-r--r--   0 moky       (501) staff       (20)     2415 2023-01-20 16:00:20.000000 dimsdk-0.8.4/dimsdk/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     8940 2023-01-20 15:58:42.000000 dimsdk-0.8.4/dimsdk/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-01-21 10:24:07.000000 dimsdk-0.8.4/dimsdk/mkm/
--rw-r--r--   0 moky       (501) staff       (20)     4672 2022-10-26 10:14:36.000000 dimsdk-0.8.4/dimsdk/mkm/roles.py
--rw-r--r--   0 moky       (501) staff       (20)     2263 2022-12-11 11:56:55.000000 dimsdk-0.8.4/dimsdk/mkm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6386 2023-01-21 07:20:27.000000 dimsdk-0.8.4/dimsdk/mkm/station.py
--rw-r--r--   0 moky       (501) staff       (20)     1743 2022-10-26 10:03:34.000000 dimsdk-0.8.4/dimsdk/mkm/robot.py
--rw-r--r--   0 moky       (501) staff       (20)     9529 2023-01-20 16:10:30.000000 dimsdk-0.8.4/dimsdk/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     3727 2023-01-20 16:00:13.000000 dimsdk-0.8.4/dimsdk/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     2013 2023-01-20 15:58:25.000000 dimsdk-0.8.4/dimsdk/helper.py
--rw-r--r--   0 moky       (501) staff       (20)     6681 2023-01-20 15:58:38.000000 dimsdk-0.8.4/dimsdk/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     3503 2023-01-20 15:23:28.000000 dimsdk-0.8.4/dimsdk/proc_content.py
--rw-r--r--   0 moky       (501) staff       (20)      556 2021-11-09 09:08:05.000000 dimsdk-0.8.4/README.md
--rw-r--r--   0 moky       (501) staff       (20)     1256 2023-01-20 15:52:28.000000 dimsdk-0.8.4/setup.py
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-01-21 10:24:07.000000 dimsdk-0.8.4/setup.cfg
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:03:46.000000 dimsdk-0.8.5/
+-rw-r--r--   0 moky       (501) staff       (20)     1047 2023-06-07 17:03:46.000000 dimsdk-0.8.5/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      556 2022-12-11 05:05:26.000000 dimsdk-0.8.5/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk/
+-rw-r--r--   0 moky       (501) staff       (20)     5866 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3727 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/ans.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2278 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2354 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/cpu/array.py
+-rw-r--r--   0 moky       (501) staff       (20)     2887 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/cpu/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     3608 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/cpu/creator.py
+-rw-r--r--   0 moky       (501) staff       (20)     4547 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/cpu/customized.py
+-rw-r--r--   0 moky       (501) staff       (20)     4059 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4706 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/cpu/factory.py
+-rw-r--r--   0 moky       (501) staff       (20)     2490 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/cpu/forward.py
+-rw-r--r--   0 moky       (501) staff       (20)     3283 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/cpu/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     2415 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     8342 2023-06-02 04:25:14.000000 dimsdk-0.8.5/dimsdk/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     8548 2023-06-02 04:28:45.000000 dimsdk-0.8.5/dimsdk/factories.py
+-rw-r--r--   0 moky       (501) staff       (20)     2013 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)     6701 2023-06-02 04:55:12.000000 dimsdk-0.8.5/dimsdk/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk/mkm/
+-rw-r--r--   0 moky       (501) staff       (20)     2263 2022-12-12 09:59:21.000000 dimsdk-0.8.5/dimsdk/mkm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     1965 2023-06-01 18:23:20.000000 dimsdk-0.8.5/dimsdk/mkm/robot.py
+-rw-r--r--   0 moky       (501) staff       (20)     4672 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/mkm/roles.py
+-rw-r--r--   0 moky       (501) staff       (20)     6579 2023-06-01 18:25:38.000000 dimsdk-0.8.5/dimsdk/mkm/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     9854 2023-06-02 04:46:51.000000 dimsdk-0.8.5/dimsdk/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     3503 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/proc_content.py
+-rw-r--r--   0 moky       (501) staff       (20)     7030 2023-06-02 04:52:26.000000 dimsdk-0.8.5/dimsdk/processor.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1047 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      635 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       37 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        7 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-07 17:03:46.000000 dimsdk-0.8.5/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1256 2023-06-01 17:05:35.000000 dimsdk-0.8.5/setup.py
```

### Comparing `dimsdk-0.8.4/PKG-INFO` & `dimsdk-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimsdk
-Version: 0.8.4
+Version: 0.8.5
 Summary: Decentralized Instant Messaging SDK
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python SDK)
```

### Comparing `dimsdk-0.8.4/dimsdk.egg-info/PKG-INFO` & `dimsdk-0.8.5/dimsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimsdk
-Version: 0.8.4
+Version: 0.8.5
 Summary: Decentralized Instant Messaging SDK
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python SDK)
```

### Comparing `dimsdk-0.8.4/dimsdk.egg-info/SOURCES.txt` & `dimsdk-0.8.5/dimsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/cpu/__init__.py` & `dimsdk-0.8.5/dimsdk/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/cpu/factory.py` & `dimsdk-0.8.5/dimsdk/cpu/factory.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/cpu/customized.py` & `dimsdk-0.8.5/dimsdk/cpu/customized.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/cpu/document.py` & `dimsdk-0.8.5/dimsdk/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/cpu/forward.py` & `dimsdk-0.8.5/dimsdk/cpu/forward.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/cpu/creator.py` & `dimsdk-0.8.5/dimsdk/cpu/creator.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/cpu/array.py` & `dimsdk-0.8.5/dimsdk/cpu/array.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/cpu/base.py` & `dimsdk-0.8.5/dimsdk/cpu/base.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/cpu/meta.py` & `dimsdk-0.8.5/dimsdk/cpu/meta.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/__init__.py` & `dimsdk-0.8.5/dimsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/processor.py` & `dimsdk-0.8.5/dimsdk/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,28 +93,27 @@
     # Override
     def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         # TODO: override to check broadcast message before calling it
         messenger = self.messenger
         # 1. verify message
         s_msg = messenger.verify_message(msg=msg)
         if s_msg is None:
-            # waiting for sender's meta if not exists
+            # TODO: suspend and waiting for sender's meta if not exists
             return []
         # 2. process message
         responses = messenger.process_secure_message(msg=s_msg, r_msg=msg)
         if responses is None or len(responses) == 0:
             return []
         # 3. sign message
         messages = []
         for res in responses:
             signed = messenger.sign_message(msg=res)
             if signed is not None:
                 messages.append(signed)
         return messages
-        # TODO: override to deliver to the receiver when catch exception "receiver error ..."
 
     # Override
     def process_secure_message(self, msg: SecureMessage, r_msg: ReliableMessage) -> List[SecureMessage]:
         messenger = self.messenger
         # 1. decrypt message
         i_msg = messenger.decrypt_message(msg=msg)
         if i_msg is None:
```

### Comparing `dimsdk-0.8.4/dimsdk/factories.py` & `dimsdk-0.8.5/dimsdk/factories.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from typing import Optional, Any, Dict
 
-from dimp.dkd.factory import FactoryManager
+from dimp.dkd.factory import CommandFactoryManager
 from dimp.msg import MessageEnvelopeFactory, PlainMessageFactory, EncryptedMessageFactory, NetworkMessageFactory
 from dimp import Envelope, InstantMessage, SecureMessage, ReliableMessage
 
 from dimp import ContentType, Content, ContentFactory
 from dimp import Command, CommandFactory, GroupCommand
 
 from dimp import BaseContent
@@ -80,21 +80,21 @@
 class GeneralCommandFactory(ContentFactory, CommandFactory):
 
     def __init__(self):
         super().__init__()
 
     # Override
     def parse_content(self, content: Dict[str, Any]) -> Optional[Content]:
-        gf = FactoryManager.general_factory
+        gf = CommandFactoryManager.general_factory
         name = gf.get_cmd(content=content)
         # get factory by command name
-        factory = gf.get_command_factory(cmd=name)
+        factory = None if name is None else gf.get_command_factory(cmd=name)
         if factory is None:
             # check for group command
-            if 'group' in content:
+            if 'group' in content and name != 'group':
                 factory = gf.get_command_factory(cmd='group')
             if factory is None:
                 factory = self
         return factory.parse_command(content=content)
 
     # Override
     def parse_command(self, content: Dict[str, Any]) -> Optional[Command]:
@@ -108,18 +108,18 @@
         return BaseHistoryCommand(content=content)
 
 
 class GroupCommandFactory(HistoryCommandFactory):
 
     # Override
     def parse_content(self, content: Dict[str, Any]) -> Optional[Content]:
-        gf = FactoryManager.general_factory
+        gf = CommandFactoryManager.general_factory
         name = gf.get_cmd(content=content)
         # get factory by command name
-        factory = gf.get_command_factory(cmd=name)
+        factory = None if name is None else gf.get_command_factory(cmd=name)
         if factory is None:
             factory = self
         return factory.parse_command(content=content)
 
     # Override
     def parse_command(self, content: Dict[str, Any]) -> Optional[Command]:
         return BaseGroupCommand(content=content)
```

### Comparing `dimsdk-0.8.4/dimsdk/delegate.py` & `dimsdk-0.8.5/dimsdk/delegate.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/packer.py` & `dimsdk-0.8.5/dimsdk/packer.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,30 +41,36 @@
 
 
 class MessagePacker(TwinsHelper, Packer):
 
     # Override
     def overt_group(self, content: Content) -> Optional[ID]:
         group = content.group
-        if group is not None:
-            if group.is_broadcast:
-                # broadcast message is always overt
-                return group
-            if isinstance(content, Command):
-                # group command should be sent to each member directly, so
-                # don't expose group ID
-                return None
+        if group is None:
+            return None
+        elif group.is_broadcast:
+            # broadcast message is always overt
+            return group
+        elif isinstance(content, Command):
+            # group command should be sent to each member directly, so
+            # don't expose group ID
+            return None
+        else:
             return group
 
     #
     #   InstantMessage -> SecureMessage -> ReliableMessage -> Data
     #
 
     # Override
     def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
+        # TODO: check receiver before calling this, make sure the visa.key exists;
+        #       otherwise, suspend this message for waiting receiver's visa/meta;
+        #       if receiver is a group, query all members' visa too!
+
         messenger = self.messenger
         # check message delegate
         if msg.delegate is None:
             msg.delegate = messenger
 
         sender = msg.sender
         receiver = msg.receiver
@@ -96,34 +102,38 @@
             assert password is not None, 'failed to get group msg key: %s -> %s' % (sender, group)
 
         # 2. encrypt 'content' to 'data' for receiver/group members
         if receiver.is_group:
             # group message
             facebook = self.facebook
             grp = facebook.group(identifier=receiver)
-            if grp is None:
-                # group not ready
-                # TODO: suspend this message for waiting group's meta
-                return None
+            # a station will never send group message, so here must be a client;
+            # and the client messenger should check the group's meta & members
+            # before encrypting message, so we can trust that the group can be
+            # created and its members MUST exist here.
+            assert grp is not None, 'group not ready: %s' % receiver
+            # if grp is None:
+            #     # TODO: suspend this message for waiting group's meta
+            #     return None
             members = grp.members
-            if members is None or len(members) == 0:
-                # group members not found
-                # TODO: suspend this message for waiting group's membership
-                return None
+            assert len(members) > 0, 'group members not found: %s' % receiver
+            # if members is None or len(members) == 0:
+            #     # TODO: suspend this message for waiting group's membership
+            #     return None
             s_msg = msg.encrypt(password=password, members=grp.members)
         else:
             # personal message (or split group message)
             s_msg = msg.encrypt(password=password)
         if s_msg is None:
             # public key for encryption not found
             # TODO: suspend this message for waiting receiver's meta
             return None
 
         # overt group ID
-        if group is not None and receiver != group:
+        if group is not None and group != receiver:
             # NOTICE: this help the receiver knows the group ID
             #         when the group message separated to multi-messages,
             #         if don't want the others know you are the group members,
             #         remove it.
             s_msg.envelope.group = group
 
         # NOTICE: copy content type to envelope
@@ -147,60 +157,64 @@
 
     #
     #   Data -> ReliableMessage -> SecureMessage -> InstantMessage
     #
 
     def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
         js = utf8_decode(data=data)
+        assert js is not None, 'message data error: %d' % len(data)
         dictionary = json_decode(string=js)
         # TODO: translate short keys
         #       'S' -> 'sender'
         #       'R' -> 'receiver'
         #       'W' -> 'time'
         #       'T' -> 'type'
         #       'G' -> 'group'
         #       ------------------
         #       'D' -> 'data'
         #       'V' -> 'signature'
         #       'K' -> 'key'
         #       ------------------
         #       'M' -> 'meta'
+        #       'P' -> 'visa'
         return ReliableMessage.parse(msg=dictionary)
 
     def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
-        # TODO: make sure meta exists before verifying message
+        # TODO: make sure sender's meta exists before verifying message
         facebook = self.facebook
         sender = msg.sender
         # [Meta Protocol]
         meta = msg.meta
         if meta is not None:
             facebook.save_meta(meta=meta, identifier=sender)
         # [Visa Protocol]
         visa = msg.visa
         if visa is not None:
             facebook.save_document(document=visa)
         # check message delegate
         if msg.delegate is None:
             msg.delegate = self.messenger
         #
-        # TODO: check [Meta Protocol]
-        #       make sure the sender's meta exists
-        #       (do in by application)
+        # NOTICE: check [Visa Protocol] before calling this
+        #       make sure the sender's meta(visa) exists
+        #       (do it by application)
         #
         assert msg.signature is not None, 'message signature cannot be empty: %s' % msg
         # verify 'data' with 'signature'
         return msg.verify()
 
     def decrypt_message(self, msg: SecureMessage) -> Optional[InstantMessage]:
-        # TODO: make sure private key (decrypt key) exists before decrypting message
+        # TODO: check receiver before calling this, make sure you are the receiver,
+        #       or you are a member of the group when this is a group message,
+        #       so that you will have a private key (decrypt key) to decrypt it.
         facebook = self.facebook
         receiver = msg.receiver
         user = facebook.select_user(receiver=receiver)
         if user is None:
-            # current users not match
+            # local users not match
             trimmed = None
         elif receiver.is_group:
             # trim group message
             trimmed = msg.trim(member=user.identifier)
         else:
             trimmed = msg
         if trimmed is None:
```

### Comparing `dimsdk-0.8.4/dimsdk/mkm/roles.py` & `dimsdk-0.8.5/dimsdk/mkm/roles.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/mkm/__init__.py` & `dimsdk-0.8.5/dimsdk/mkm/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/mkm/station.py` & `dimsdk-0.8.5/dimsdk/mkm/station.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,20 @@
             doc = self.document(doc_type='*')
             if doc is not None:
                 value = doc.get_property('port')
                 if value is not None:
                     self.__port = int(value)
         return self.__port
 
+    @property
+    def provider(self) -> Optional[ID]:
+        doc = self.document(doc_type='*')
+        if doc is not None:
+            return ID.parse(identifier=doc.get_property(key='ISP'))
+
 
 class ServiceProvider(BaseGroup):
 
     def __init__(self, identifier: ID):
         super().__init__(identifier=identifier)
         assert identifier.type == EntityType.ISP, 'Service Provider ID type error: %s' % identifier
```

### Comparing `dimsdk-0.8.4/dimsdk/mkm/robot.py` & `dimsdk-0.8.5/dimsdk/mkm/robot.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,16 +29,24 @@
 # ==============================================================================
 
 """
     Bot User
     ~~~~~~~~
 """
 
+from typing import Optional
+
 from dimp import ID, EntityType
 from dimp import BaseUser
 
 
 class Bot(BaseUser):
 
     def __init__(self, identifier: ID):
         super().__init__(identifier=identifier)
         assert identifier.type == EntityType.BOT, 'Bot ID type error: %s' % identifier
+
+    @property
+    def provider(self) -> Optional[ID]:
+        doc = self.document(doc_type='*')
+        if doc is not None:
+            return ID.parse(identifier=doc.get_property(key='ICP'))
```

### Comparing `dimsdk-0.8.4/dimsdk/facebook.py` & `dimsdk-0.8.5/dimsdk/facebook.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,108 +97,69 @@
 
         :param document: entity document
         :return: True on success
         """
         raise NotImplemented
 
     #
-    #   Group Members
-    #
-    @abstractmethod
-    def save_members(self, members: List[ID], identifier: ID) -> bool:
-        """
-        Save members of group
-
-        :param members:    member ID list
-        :param identifier: group ID
-        :return: True on success
-        """
-        raise NotImplemented
-
-    #
     #   Document checking
     #
     def check_document(self, document: Document) -> bool:
         """
         Checking document
 
         :param document: entity document
         :return: True on accepted
         """
         identifier = document.identifier
-        if identifier is None:
-            return False
         # NOTICE: if this is a bulletin document for group,
         #             verify it with the group owner's meta.key
         #         else (this is a visa document for user)
         #             verify it with the user's meta.key
         if identifier.is_group:
-            # check by owner
+            # check by group owner's meta.key
             owner = self.owner(identifier=identifier)
-            if owner is None:
-                if identifier.type == EntityType.GROUP:
-                    # NOTICE: if this is a polylogue profile
-                    #             verify it with the founder's meta.key
-                    #             (which equals to the group's meta.key)
-                    meta = self.meta(identifier=identifier)
-                else:
-                    # FIXME: owner not found for this group
-                    return False
-            else:
+            if owner is not None:
                 meta = self.meta(identifier=owner)
+            elif identifier.type == EntityType.GROUP:
+                # NOTICE: if this is a polylogue profile
+                #             verify it with the founder's meta.key
+                #             (which equals to the group's meta.key)
+                meta = self.meta(identifier=identifier)
+            else:
+                # FIXME: owner not found for this group
+                return False
         else:
+            # check by user's meta.key
             meta = self.meta(identifier=identifier)
         if meta is not None:
             return document.verify(public_key=meta.key)
 
-    # group membership
-
-    def is_founder(self, member: ID, group: ID) -> bool:
-        # check member's public key with group's meta.key
-        g_meta = self.meta(identifier=group)
-        assert g_meta is not None, 'failed to get meta for group: %s' % group
-        u_meta = self.meta(identifier=member)
-        assert u_meta is not None, 'failed to get meta for member: %s' % member
-        return Meta.match_key(meta=g_meta, key=u_meta.key)
-
-    def is_owner(self, member: ID, group: ID) -> bool:
-        if group.type == EntityType.GROUP:
-            # this is a polylogue
-            return self.is_founder(member=member, group=group)
-        raise AssertionError('only Polylogue so far')
-
+    # protected
     def create_user(self, identifier: ID) -> Optional[User]:
-        if identifier.is_broadcast:
-            # create user 'anyone@anywhere'
-            return BaseUser(identifier=identifier)
-        # make sure meta exists
-        assert self.meta(identifier) is not None, 'failed to get meta for user: %s' % identifier
         # TODO: make sure visa key exists before calling this
-        u_type = identifier.type
+        network = identifier.type
         # check user type
-        if u_type == EntityType.STATION:
-            # TODO: get station address before create it
+        if network == EntityType.STATION:
+            # TODO: get station ip,port before create it
             # return Station(identifier=identifier, host='0.0.0.0', port=0)
             return Station(identifier=identifier)
-        elif u_type == EntityType.BOT:
+        elif network == EntityType.BOT:
             return Bot(identifier=identifier)
-        # raise TypeError('unsupported user type: %s' % u_type)
+        # general user, or 'anyone@anywhere'
         return BaseUser(identifier=identifier)
 
+    # protected
     def create_group(self, identifier: ID) -> Optional[Group]:
-        if identifier.is_broadcast:
-            # create group 'everyone@everywhere'
-            return BaseGroup(identifier=identifier)
-        # make sure meta exists
-        assert self.meta(identifier) is not None, 'failed to get meta for group: %s' % identifier
-        g_type = identifier.type
+        # TODO: make group meta exists before calling this
+        network = identifier.type
         # check group type
-        if g_type == EntityType.ISP:
+        if network == EntityType.ISP:
             return ServiceProvider(identifier=identifier)
-        # raise TypeError('unsupported group type: %s' % g_type)
+        # general group, or 'everyone@everywhere'
         return BaseGroup(identifier=identifier)
 
     @property
     @abstractmethod
     def local_users(self) -> List[User]:
         """
         Get all local users (for decrypting received message)
@@ -213,36 +174,45 @@
     #     users = self.local_users
     #     if users is not None and len(users) > 0:
     #         return users[0]
 
     def select_user(self, receiver: ID) -> Optional[User]:
         """ Select local user for receiver """
         users = self.local_users
-        assert users is not None and len(users) > 0, 'local users should not be empty'
-        if receiver.is_broadcast:
+        if users is None or len(users) == 0:
+            assert False, 'local users should not be empty'
+            # return None
+        elif receiver.is_broadcast:
+            # broadcast message can decrypt by anyone, so just return current user
             return users[0]
-        if receiver.is_group:
-            # group message (recipient not designated)
-            members = self.members(identifier=receiver)
-            if members is None or len(members) == 0:
-                # TODO: group not ready, waiting for group info
-                return None
-            for item in users:
-                assert isinstance(item, User), 'local user error: %s' % item
-                if item.identifier in members:
-                    # DISCUSS: set this item to be current user?
-                    return item
-        else:
+        elif receiver.is_user:
             # 1. personal message
             # 2. split group message
             for item in users:
-                assert isinstance(item, User), 'local user error: %s' % item
                 if item.identifier == receiver:
                     # DISCUSS: set this item to be current user?
                     return item
+            # not mine?
+            return None
+        # group message (recipient not designated)
+        assert receiver.is_group, 'receiver error: %s' % receiver
+        # the messenger will check group info before decrypting message,
+        # so we can trust that the group's meta & members MUST exist here.
+        grp = self.group(identifier=receiver)
+        assert grp is not None, 'group not ready: %s' % receiver
+        # if grp is None:
+        #     return None
+        members = grp.members
+        assert len(members) > 0, 'members not found: %s' % receiver
+        # if members is None or len(members) == 0:
+        #     return None
+        for item in users:
+            if item.identifier in members:
+                # DISCUSS: set this item to be current user?
+                return item
 
     #
     #   Entity Delegate
     #
 
     # Override
     def user(self, identifier: ID) -> Optional[User]:
```

### Comparing `dimsdk-0.8.4/dimsdk/ans.py` & `dimsdk-0.8.5/dimsdk/ans.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/helper.py` & `dimsdk-0.8.5/dimsdk/helper.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/dimsdk/messenger.py` & `dimsdk-0.8.5/dimsdk/messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,20 @@
 
     # Override
     def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
         delegate = self.packer
         return delegate.encrypt_message(msg=msg)
 
     # Override
-    def sign_message(self, msg: SecureMessage) -> ReliableMessage:
+    def sign_message(self, msg: SecureMessage) -> Optional[ReliableMessage]:
         delegate = self.packer
         return delegate.sign_message(msg=msg)
 
     # Override
-    def serialize_message(self, msg: ReliableMessage) -> bytes:
+    def serialize_message(self, msg: ReliableMessage) -> Optional[bytes]:
         delegate = self.packer
         return delegate.serialize_message(msg=msg)
 
     # Override
     def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
         delegate = self.packer
         return delegate.deserialize_message(data=data)
```

### Comparing `dimsdk-0.8.4/dimsdk/proc_content.py` & `dimsdk-0.8.5/dimsdk/proc_content.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/README.md` & `dimsdk-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.4/setup.py` & `dimsdk-0.8.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.8.4'
+__version__ = '0.8.5'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -37,12 +37,12 @@
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'dimp>=0.12.6',
-        'dkd>=0.12.6',
-        'mkm>=0.12.6',
+        'dimp>=0.12.8',
+        'dkd>=0.12.7',
+        'mkm>=0.12.7',
     ]
 )
```

