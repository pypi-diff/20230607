# Comparing `tmp/dimp-0.9.7.tar.gz` & `tmp/dimp-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimp-0.9.7.tar", last modified: Thu Sep  3 20:28:06 2020, max compression
+gzip compressed data, was "dist/dimp-0.9.8.tar", last modified: Fri Sep  4 17:55:58 2020, max compression
```

## Comparing `dimp-0.9.7.tar` & `dimp-0.9.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-03 20:28:06.000000 dimp-0.9.7/
--rw-r--r--   0 moky       (501) staff       (20)    14512 2020-09-03 20:28:06.000000 dimp-0.9.7/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)    11393 2020-09-02 14:40:35.000000 dimp-0.9.7/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-03 20:28:06.000000 dimp-0.9.7/dimp/
--rw-r--r--   0 moky       (501) staff       (20)     3277 2020-09-02 14:40:35.000000 dimp-0.9.7/dimp/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9212 2020-03-31 04:56:51.000000 dimp-0.9.7/dimp/barrack.py
--rw-r--r--   0 moky       (501) staff       (20)     3040 2020-03-15 07:40:04.000000 dimp-0.9.7/dimp/delegate.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-03 20:28:06.000000 dimp-0.9.7/dimp/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2354 2020-09-02 14:40:35.000000 dimp-0.9.7/dimp/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4766 2020-09-02 14:40:35.000000 dimp-0.9.7/dimp/protocol/command.py
--rw-r--r--   0 moky       (501) staff       (20)     4924 2020-09-02 14:40:35.000000 dimp-0.9.7/dimp/protocol/content.py
--rw-r--r--   0 moky       (501) staff       (20)    13216 2020-09-02 14:40:35.000000 dimp-0.9.7/dimp/protocol/file.py
--rw-r--r--   0 moky       (501) staff       (20)     3754 2020-09-02 14:40:35.000000 dimp-0.9.7/dimp/protocol/forward.py
--rw-r--r--   0 moky       (501) staff       (20)     9618 2020-09-02 14:40:35.000000 dimp-0.9.7/dimp/protocol/group.py
--rw-r--r--   0 moky       (501) staff       (20)     4222 2020-09-02 14:40:35.000000 dimp-0.9.7/dimp/protocol/history.py
--rw-r--r--   0 moky       (501) staff       (20)     4101 2020-09-02 14:40:35.000000 dimp-0.9.7/dimp/protocol/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5683 2020-01-06 14:09:16.000000 dimp-0.9.7/dimp/protocol/profile.py
--rw-r--r--   0 moky       (501) staff       (20)     3112 2020-09-02 14:40:35.000000 dimp-0.9.7/dimp/protocol/text.py
--rw-r--r--   0 moky       (501) staff       (20)    15351 2020-09-03 19:29:23.000000 dimp-0.9.7/dimp/transceiver.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-03 20:28:06.000000 dimp-0.9.7/dimp.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)    14512 2020-09-03 20:28:06.000000 dimp-0.9.7/dimp.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      467 2020-09-03 20:28:06.000000 dimp-0.9.7/dimp.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2020-09-03 20:28:06.000000 dimp-0.9.7/dimp.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       22 2020-09-03 20:28:06.000000 dimp-0.9.7/dimp.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        5 2020-09-03 20:28:06.000000 dimp-0.9.7/dimp.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2020-09-03 20:28:06.000000 dimp-0.9.7/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1119 2020-09-03 20:16:42.000000 dimp-0.9.7/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-04 17:55:58.000000 dimp-0.9.8/
+-rw-r--r--   0 moky       (501) staff       (20)    14512 2020-09-04 17:55:58.000000 dimp-0.9.8/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)    11393 2020-09-02 14:40:35.000000 dimp-0.9.8/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-04 17:55:58.000000 dimp-0.9.8/dimp/
+-rw-r--r--   0 moky       (501) staff       (20)     3458 2020-09-04 14:05:01.000000 dimp-0.9.8/dimp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9212 2020-03-31 04:56:51.000000 dimp-0.9.8/dimp/barrack.py
+-rw-r--r--   0 moky       (501) staff       (20)     3040 2020-03-15 07:40:04.000000 dimp-0.9.8/dimp/delegate.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-04 17:55:58.000000 dimp-0.9.8/dimp/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     3048 2020-09-04 14:02:20.000000 dimp-0.9.8/dimp/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4839 2020-09-04 17:42:08.000000 dimp-0.9.8/dimp/protocol/command.py
+-rw-r--r--   0 moky       (501) staff       (20)     4942 2020-09-04 17:24:20.000000 dimp-0.9.8/dimp/protocol/content.py
+-rw-r--r--   0 moky       (501) staff       (20)    13467 2020-09-04 17:38:46.000000 dimp-0.9.8/dimp/protocol/file.py
+-rw-r--r--   0 moky       (501) staff       (20)     3836 2020-09-04 17:41:08.000000 dimp-0.9.8/dimp/protocol/forward.py
+-rw-r--r--   0 moky       (501) staff       (20)     9618 2020-09-02 14:40:35.000000 dimp-0.9.8/dimp/protocol/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     4295 2020-09-04 17:42:40.000000 dimp-0.9.8/dimp/protocol/history.py
+-rw-r--r--   0 moky       (501) staff       (20)     4163 2020-09-04 17:44:23.000000 dimp-0.9.8/dimp/protocol/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5646 2020-09-04 17:47:58.000000 dimp-0.9.8/dimp/protocol/profile.py
+-rw-r--r--   0 moky       (501) staff       (20)     3160 2020-09-04 17:46:09.000000 dimp-0.9.8/dimp/protocol/text.py
+-rw-r--r--   0 moky       (501) staff       (20)    15692 2020-09-04 13:52:10.000000 dimp-0.9.8/dimp/transceiver.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-04 17:55:58.000000 dimp-0.9.8/dimp.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)    14512 2020-09-04 17:55:58.000000 dimp-0.9.8/dimp.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      467 2020-09-04 17:55:58.000000 dimp-0.9.8/dimp.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2020-09-04 17:55:58.000000 dimp-0.9.8/dimp.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       22 2020-09-04 17:55:58.000000 dimp-0.9.8/dimp.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        5 2020-09-04 17:55:58.000000 dimp-0.9.8/dimp.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2020-09-04 17:55:58.000000 dimp-0.9.8/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1119 2020-09-04 13:27:22.000000 dimp-0.9.8/setup.py
```

### Comparing `dimp-0.9.7/PKG-INFO` & `dimp-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimp
-Version: 0.9.7
+Version: 0.9.8
 Summary: Decentralized Instant Messaging Protocol
 Home-page: https://github.com/dimchat/core-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging Protocol (Python)
```

### Comparing `dimp-0.9.7/README.md` & `dimp-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `dimp-0.9.7/dimp/__init__.py` & `dimp-0.9.8/dimp/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 # SOFTWARE.
 # ==============================================================================
 
 from mkm import *
 
 from dkd import *
 
+from .protocol import Envelope, Message, InstantMessage, SecureMessage, ReliableMessage
+from .protocol import InstantMessageDelegate, SecureMessageDelegate, ReliableMessageDelegate
 from .protocol import Content, ForwardContent, TextContent
 from .protocol import FileContent, ImageContent, AudioContent, VideoContent
 from .protocol import Command, HistoryCommand, GroupCommand
 from .protocol import InviteCommand, ExpelCommand, JoinCommand, QuitCommand
 from .protocol import QueryCommand, ResetCommand
 from .protocol import MetaCommand, ProfileCommand
```

### Comparing `dimp-0.9.7/dimp/barrack.py` & `dimp-0.9.8/dimp/barrack.py`

 * *Files identical despite different names*

### Comparing `dimp-0.9.7/dimp/delegate.py` & `dimp-0.9.8/dimp/delegate.py`

 * *Files identical despite different names*

### Comparing `dimp-0.9.7/dimp/protocol/__init__.py` & `dimp-0.9.8/dimp/protocol/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 """
     DIMP - Message Contents & Commands
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Define universal message types as contents and commands
 """
 
+from mkm import ID, SymmetricKey
+import dkd
+
 from .content import Content
 from .forward import ForwardContent
 from .text import TextContent
 from .file import FileContent, ImageContent, AudioContent, VideoContent
 
 from .command import Command
 from .history import HistoryCommand
@@ -46,16 +49,32 @@
 from .group import GroupCommand
 from .group import InviteCommand, ExpelCommand, JoinCommand, QuitCommand
 from .group import QueryCommand, ResetCommand
 
 from .meta import MetaCommand
 from .profile import ProfileCommand
 
+#
+#  Conveniences for Generic
+#
+Envelope = dkd.Envelope[ID]
+Message = dkd.Message[ID, SymmetricKey]
+InstantMessage = dkd.InstantMessage[ID, SymmetricKey]
+SecureMessage = dkd.SecureMessage[ID, SymmetricKey]
+ReliableMessage = dkd.ReliableMessage[ID, SymmetricKey]
+# Delegates
+InstantMessageDelegate = dkd.InstantMessageDelegate[ID, SymmetricKey]
+SecureMessageDelegate = dkd.SecureMessageDelegate[ID, SymmetricKey]
+ReliableMessageDelegate = dkd.ReliableMessageDelegate[ID, SymmetricKey]
+
 
 __all__ = [
+    'Envelope', 'Message', 'InstantMessage', 'SecureMessage', 'ReliableMessage',
+    'InstantMessageDelegate', 'SecureMessageDelegate', 'ReliableMessageDelegate',
+
     'Content', 'ForwardContent', 'TextContent',
     'FileContent', 'ImageContent', 'AudioContent', 'VideoContent',
 
     'Command', 'HistoryCommand', 'GroupCommand',
     'InviteCommand', 'ExpelCommand', 'JoinCommand', 'QuitCommand',
     'QueryCommand', 'ResetCommand',
```

### Comparing `dimp-0.9.7/dimp/protocol/command.py` & `dimp-0.9.8/dimp/protocol/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,18 +100,20 @@
 
         :param content: command info
         :param command: command name
         :param time: command time
         :return: Command object
         """
         if content is None:
-            # create empty content
-            content = {}
-        # set content type: 'Command'
-        if 'type' not in content:
+            # create empty content with type
+            content = {
+                'type': ContentType.Command
+            }
+        elif 'type' not in content:
+            # set content type: 'Command'
             content['type'] = ContentType.Command
         # set command name
         if command is not None:
             content['command'] = command
         # new Command(dict)
         return super().new(content=content, time=time)
```

### Comparing `dimp-0.9.7/dimp/protocol/content.py` & `dimp-0.9.8/dimp/protocol/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,28 @@
 # SOFTWARE.
 # ==============================================================================
 
 from typing import Union
 import time as time_lib
 import random
 
+from mkm import ID
+
 from dkd import ContentType
 from dkd import Content as DKDContent
 
 
 def random_positive_integer():
     """
     :return: random integer greater than 0
     """
     return random.randint(1, 2**32-1)
 
 
-class Content(DKDContent):
+class Content(DKDContent[ID]):
     """This class is for creating message content
 
         Message Content
         ~~~~~~~~~~~~~~~
 
         data format: {
             'type'    : 0x00,            // message type
@@ -84,15 +86,15 @@
         # subclass or default Content(dict)
         return super().__new__(cls, content)
 
     #
     #   Factory
     #
     @classmethod
-    def new(cls, content: dict=None, content_type: Union[ContentType, int, None]=0, time: int=0):
+    def new(cls, content: dict=None, content_type: Union[ContentType, int]=0, time: int=0):
         """
         Create message content with 'type' & 'sn' (serial number)
 
         :param content:      content info, if empty then create a new one with 'type'
         :param content_type: content type, if not empty then set into content
         :param time:         message time
         :return: Content object
```

### Comparing `dimp-0.9.7/dimp/protocol/file.py` & `dimp-0.9.8/dimp/protocol/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,18 +135,18 @@
             self.__password = SymmetricKey(self.get('password'))
         return self.__password
 
     @password.setter
     def password(self, key: dict):
         if key is None:
             self.pop('password', None)
-            self.__password = None
         else:
             self['password'] = key
-            self.__password = SymmetricKey(key)
+        # lazy load
+        self.__password = None
 
     #
     #   Factories
     #
     @classmethod
     def new(cls, content: dict=None, data: bytes=None, filename: str=None):
         """
@@ -154,18 +154,20 @@
 
         :param content:  content info
         :param data:     file data
         :param filename: file name
         :return: FileContent object
         """
         if content is None:
-            # create empty content
-            content = {}
-        # set content type: 'File'
-        if 'type' not in content:
+            # create empty content with type
+            content = {
+                'type': ContentType.File
+            }
+        elif 'type' not in content:
+            # set content type: 'File'
             content['type'] = ContentType.File
         # set file data
         if data is not None:
             content['data'] = Base64.encode(data)
         # set filename
         if filename is not None:
             content['filename'] = filename
@@ -253,18 +255,20 @@
         :param content:   content info
         :param data:      image data
         :param thumbnail: thumbnail data
         :param filename:  image filename
         :return: ImageContent object
         """
         if content is None:
-            # create empty content
-            content = {}
-        # set content type: 'Image'
-        if 'type' not in content:
+            # create empty content with type
+            content = {
+                'type': ContentType.Image
+            }
+        elif 'type' not in content:
+            # set content type: 'Image'
             content['type'] = ContentType.Image
         # set thumbnail data
         if thumbnail is not None:
             content['thumbnail'] = Base64.encode(thumbnail)
         # new ImageContent(dict)
         return super().new(content=content, data=data, filename=filename)
 
@@ -330,18 +334,20 @@
         :param content:  content info
         :param data:     audio data
         :param text:     Automatic Speech Recognition
         :param filename: audio filename
         :return: AudioContent object
         """
         if content is None:
-            # create empty content
-            content = {}
-        # set content type: 'Audio'
-        if 'type' not in content:
+            # create empty content with type
+            content = {
+                'type': ContentType.Audio
+            }
+        elif 'type' not in content:
+            # set content type: 'Audio'
             content['type'] = ContentType.Audio
         # set ASR text
         if text is not None:
             content['text'] = text
         # new AudioContent(dict)
         return super().new(content=content, data=data, filename=filename)
 
@@ -414,18 +420,20 @@
         :param content:  content info
         :param data:     video data
         :param snapshot: snapshot data
         :param filename: video filename
         :return: VideoContent object
         """
         if content is None:
-            # create empty content
-            content = {}
-        # set content type: 'Video'
-        if 'type' not in content:
+            # create empty content with type
+            content = {
+                'type': ContentType.Video
+            }
+        elif 'type' not in content:
+            # set content type: 'Video'
             content['type'] = ContentType.Video
         # set snapshot data
         if snapshot is not None:
             content['snapshot'] = Base64.encode(snapshot)
         # new VideoContent(dict)
         return super().new(content=content, data=data, filename=filename)
```

### Comparing `dimp-0.9.7/dimp/protocol/forward.py` & `dimp-0.9.8/dimp/protocol/forward.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
+from mkm import ID, SymmetricKey
+
 from dkd import ContentType
 from dkd import ReliableMessage
 
 from .content import Content
 
 
 class ForwardContent(Content):
@@ -65,44 +67,45 @@
 
     def __init__(self, content: dict):
         if self is content:
             # no need to init again
             return
         super().__init__(content)
         # lazy
-        self.__forward: ReliableMessage = None
+        self.__forward = None
 
     #
     #   forward (top-secret message)
     #
     @property
-    def message(self) -> ReliableMessage:
+    def message(self) -> ReliableMessage[ID, SymmetricKey]:
         if self.__forward is None:
-            self.__forward = ReliableMessage(self.get('forward'))
+            self.__forward = ReliableMessage[ID, SymmetricKey](self.get('forward'))
         return self.__forward
 
     @message.setter
     def message(self, value: dict):
         if value is None:
             self.pop('forward', None)
         else:
             self['forward'] = value
-        self.__forward = value
+        # lazy load
+        self.__forward = None
 
     #
     #   Factory
     #
     @classmethod
-    def new(cls, content: dict=None, message: ReliableMessage=None, time: int=0):
+    def new(cls, content: dict=None, message: dict=None, time: int=0):
         """
         Create forward message content with 'forward' (top-secret) message
 
         :param content: content info
-        :param message: top-secret message
-        :param time: message time
+        :param message: top-secret message (ReliableMessage)
+        :param time:    message time
         :return: ForwardMessage object
         """
         if content is None:
             # create empty content
             content = {}
         # set 'forward' message
         if message is not None:
```

### Comparing `dimp-0.9.7/dimp/protocol/group.py` & `dimp-0.9.8/dimp/protocol/group.py`

 * *Files identical despite different names*

### Comparing `dimp-0.9.7/dimp/protocol/history.py` & `dimp-0.9.8/dimp/protocol/history.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,18 +114,20 @@
 
         :param content: command info
         :param command: command name
         :param time: command time
         :return: HistoryCommand object
         """
         if content is None:
-            # create empty content
-            content = {}
-        # set content type: 'History'
-        if 'type' not in content:
+            # create empty content with type
+            content = {
+                'type': ContentType.History
+            }
+        elif 'type' not in content:
+            # set content type: 'History'
             content['type'] = ContentType.History
         # new HistoryCommand(dict)
         return super().new(content, command=command, time=time)
 
 
 # register content class with type
 Content.register(content_type=ContentType.History, content_class=HistoryCommand)
```

### Comparing `dimp-0.9.7/dimp/protocol/meta.py` & `dimp-0.9.8/dimp/protocol/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,42 +98,44 @@
             self.__meta = Meta(self.get('meta'))
         return self.__meta
 
     #
     #   Factories
     #
     @classmethod
-    def new(cls, content: dict=None, identifier: ID=None, meta: Meta=None):
+    def new(cls, content: dict=None, identifier: str=None, meta: dict=None):
         """
         Create meta command for entity
 
         :param content:    command info
         :param identifier: entity ID
         :param meta:       meta info
         :return: MetaCommand object
         """
         if content is None:
             # create empty content
-            content = {}
-        # set command name: 'meta'
-        if 'command' not in content:
+            content = {
+                'command': Command.META
+            }
+        elif 'command' not in content:
+            # set command name: 'meta'
             content['command'] = Command.META
         # set entity ID
         if identifier is not None:
             content['ID'] = identifier
         # set entity meta
         if meta is not None:
             content['meta'] = meta
         # new MetaCommand(dict)
         return super().new(content=content)
 
     @classmethod
-    def query(cls, identifier: ID):
+    def query(cls, identifier: str):
         return cls.new(identifier=identifier)
 
     @classmethod
-    def response(cls, identifier: ID, meta: Meta):
+    def response(cls, identifier: str, meta: dict):
         return cls.new(identifier=identifier, meta=meta)
 
 
 # register command class
 Command.register(command=Command.META, command_class=MetaCommand)
```

### Comparing `dimp-0.9.7/dimp/protocol/profile.py` & `dimp-0.9.8/dimp/protocol/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     1. contains 'ID' only, means query profile for ID
     2. contains 'profile' and 'signature' (must match), means reply
 """
 
 from typing import Optional
 
-from mkm import ID, Meta, Profile
+from mkm import Profile
 
 from .command import Command
 from .meta import MetaCommand
 
 
 class ProfileCommand(MetaCommand):
     """
@@ -123,45 +123,46 @@
     def signature(self) -> Optional[str]:
         return self.get('signature')
 
     #
     #   Factories
     #
     @classmethod
-    def new(cls, content: dict=None, identifier: ID=None, meta: Meta=None, profile: Profile=None, signature: str=None):
+    def new(cls, content: dict=None, identifier: str=None, meta: dict=None, profile: dict=None, signature: str=None):
         """
         Create profile command for entity
 
         :param content:    command info
         :param identifier: entity ID
         :param meta:       entity meta
         :param profile:    entity profile
         :param signature:  old profile's signature for querying
         :return: ProfileCommand object
         """
         if content is None:
-            # create empty content
-            content = {}
-        # set command name: 'profile'
-        if 'command' not in content:
+            # create empty content with command name
+            content = {
+                'command': Command.PROFILE
+            }
+        elif 'command' not in content:
+            # set command name: 'profile'
             content['command'] = Command.PROFILE
         # set profile info
         if profile is not None:
-            assert profile.identifier == identifier, 'profile ID error: %s, %s' % (profile, identifier)
             # TODO: upgrade to v1.1 later
             content['profile'] = profile.get('data')
             content['signature'] = profile.get('signature')
         elif signature is not None:
             content['signature'] = signature
         return super().new(content=content, identifier=identifier, meta=meta)
 
     @classmethod
-    def query(cls, identifier: ID, signature: str=None):
+    def query(cls, identifier: str, signature: str=None):
         return cls.new(identifier=identifier, signature=signature)
 
     @classmethod
-    def response(cls, identifier: ID, profile: Profile, meta: Meta=None):
+    def response(cls, identifier: str, profile: dict, meta: dict=None):
         return cls.new(identifier=identifier, meta=meta, profile=profile)
 
 
 # register command class
 Command.register(command=Command.PROFILE, command_class=ProfileCommand)
```

### Comparing `dimp-0.9.7/dimp/protocol/text.py` & `dimp-0.9.8/dimp/protocol/text.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,17 +87,19 @@
         :param content: content info
         :param text: message
         :param time: message time
         :return: TextContent object
         """
         if content is None:
             # create empty content
-            content = {}
-        # set text
-        if text is not None:
+            content = {
+                'text': text
+            }
+        elif text is not None:
+            # set text
             content['text'] = text
         # new
         return super().new(content=content, content_type=ContentType.Text, time=time)
 
 
 # register content class with type
 Content.register(content_type=ContentType.Text, content_class=TextContent)
```

### Comparing `dimp-0.9.7/dimp/transceiver.py` & `dimp-0.9.8/dimp/transceiver.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 import json
 import weakref
 from typing import Optional
 
 from mkm import Base64
 from mkm import SymmetricKey, ID
 
-from dkd import Message
-from dkd import InstantMessage, SecureMessage, ReliableMessage
-from dkd import InstantMessageDelegate, ReliableMessageDelegate
+from .protocol import Message
+from .protocol import InstantMessage, SecureMessage, ReliableMessage
+from .protocol import InstantMessageDelegate, ReliableMessageDelegate
 
 from .protocol import Content, Command
 from .delegate import EntityDelegate, CipherKeyDelegate
 
 
 class Transceiver(InstantMessageDelegate, ReliableMessageDelegate):
 
@@ -154,15 +154,15 @@
         group = self.__overt_group(content=msg.content)
         if group is None:
             # personal message or (group) command
             password = self.__password(sender=sender, receiver=receiver)
         else:
             # group message (excludes group command)
             password = self.__password(sender=sender, receiver=group)
-        assert isinstance(password, dict), 'password error: %s' % password
+        assert isinstance(password, SymmetricKey), 'password error: %s' % password
 
         assert msg.content is not None, 'message content empty: %s' % msg
         # 2. encrypt 'content' to 'data' for receiver/group members
         if receiver.is_group:
             # group message
             grp = self.barrack.group(identifier=receiver)
             s_msg = msg.encrypt(password=password, members=grp.members)
@@ -248,31 +248,34 @@
         return msg.decrypt()
         # TODO: check top-secret message
         #       (do it by application)
 
     #
     #   MessageDelegate
     #
+
     def identifier(self, string: str) -> ID:
         return self.barrack.identifier(string=string)
 
     #
     #   InstantMessageDelegate
     #
+
     def content(self, content: dict) -> Optional[Content]:
         body = Content(content)
         body.delegate = self
         return body
 
     def serialize_content(self, content: Content, key: SymmetricKey, msg: InstantMessage) -> bytes:
         # NOTICE: check attachment for File/Image/Audio/Video message content
         #         before serialize content, this job should be do in subclass
         string = json.dumps(content)
         return string.encode('utf-8')
 
+    # noinspection PyUnusedLocal,PyMethodMayBeStatic
     def encrypt_content(self, data: bytes, key: SymmetricKey, msg: InstantMessage) -> bytes:
         return key.encrypt(data=data)
 
     def encode_data(self, data: bytes, msg: InstantMessage) -> str:
         if self.__is_broadcast_message(msg=msg):
             # broadcast message content will not be encrypted (just encoded to JsON),
             # so no need to encode to Base64 here
@@ -298,19 +301,21 @@
         assert not self.__is_broadcast_message(msg=msg), 'broadcast message has no key: %s' % msg
         # encode to Base64
         return Base64.encode(data)
 
     #
     #   SecureMessageDelegate
     #
+
     def decode_key(self, key: str, msg: SecureMessage) -> Optional[bytes]:
         assert not self.__is_broadcast_message(msg=msg), 'broadcast message has no key'
         # decode from Base64
         return Base64.decode(key)
 
+    # noinspection PyUnusedLocal
     def decrypt_key(self, data: bytes, sender: ID, receiver: ID, msg: SecureMessage) -> Optional[bytes]:
         assert not self.__is_broadcast_message(msg=msg), 'broadcast message has no key'
         # decrypt key data with the receiver's private key
         user = self.barrack.user(identifier=msg.receiver)
         assert user is not None, 'failed to create local user: %s' % msg.receiver
         return user.decrypt(data=data)
 
@@ -334,14 +339,15 @@
     def decode_data(self, data: str, msg: SecureMessage) -> Optional[bytes]:
         if self.__is_broadcast_message(msg=msg):
             # broadcast message content will not be encrypted (just encoded to JsON),
             # so return the string data directly
             return data.encode('utf-8')
         return Base64.decode(data)
 
+    # noinspection PyUnusedLocal,PyMethodMayBeStatic
     def decrypt_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[bytes]:
         return key.decrypt(data)
 
     def deserialize_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[Content]:
         string = data.decode('utf-8')
         dictionary = json.loads(string)
         # TODO: translate short keys
@@ -361,25 +367,30 @@
                 # group message (excludes group command)
                 # cache the key with direction (sender -> group)
                 self.key_cache.cache_cipher_key(key=key, sender=msg.sender, receiver=group)
         # NOTICE: check attachment for File/Image/Audio/Video message content
         #         after deserialize content, this job should be do in subclass
         return content
 
+    # noinspection PyUnusedLocal
     def sign_data(self, data: bytes, sender: ID, msg: SecureMessage) -> bytes:
         user = self.barrack.user(identifier=sender)
         assert user is not None, 'failed to sign with sender: %s' % sender
         return user.sign(data)
 
+    # noinspection PyUnusedLocal,PyMethodMayBeStatic
     def encode_signature(self, signature: bytes, msg: SecureMessage) -> str:
         return Base64.encode(signature)
 
     #
     #   ReliableMessageDelegate
     #
+
+    # noinspection PyUnusedLocal,PyMethodMayBeStatic
     def decode_signature(self, signature: str, msg: ReliableMessage) -> Optional[bytes]:
         return Base64.decode(signature)
 
+    # noinspection PyUnusedLocal
     def verify_data_signature(self, data: bytes, signature: bytes, sender: ID, msg: ReliableMessage) -> bool:
         contact = self.barrack.user(identifier=sender)
         assert contact is not None, 'failed to verify signature for sender: %s' % sender
         return contact.verify(data=data, signature=signature)
```

### Comparing `dimp-0.9.7/dimp.egg-info/PKG-INFO` & `dimp-0.9.8/dimp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimp
-Version: 0.9.7
+Version: 0.9.8
 Summary: Decentralized Instant Messaging Protocol
 Home-page: https://github.com/dimchat/core-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging Protocol (Python)
```

### Comparing `dimp-0.9.7/setup.py` & `dimp-0.9.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     This is a new protocol designed for instant messaging (IM).
     The software provides accounts(user identity recognition) and
     communications between accounts safely by end-to-end encryption.
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '0.9.7'
+__version__ = '0.9.8'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
@@ -32,11 +32,11 @@
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'dkd>=0.7.7',
+        'dkd>=0.8.0',
         'mkm>=0.9.3',
     ]
 )
```

