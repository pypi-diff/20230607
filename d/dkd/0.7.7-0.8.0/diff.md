# Comparing `tmp/dkd-0.7.7.tar.gz` & `tmp/dkd-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dkd-0.7.7.tar", last modified: Thu Sep  3 20:27:39 2020, max compression
+gzip compressed data, was "dist/dkd-0.8.0.tar", last modified: Fri Sep  4 17:23:12 2020, max compression
```

## Comparing `dkd-0.7.7.tar` & `dkd-0.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-03 20:27:39.000000 dkd-0.7.7/
--rw-r--r--   0 moky       (501) staff       (20)     7608 2020-09-03 20:27:39.000000 dkd-0.7.7/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     5796 2020-02-06 10:13:12.000000 dkd-0.7.7/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-03 20:27:39.000000 dkd-0.7.7/dkd/
--rw-r--r--   0 moky       (501) staff       (20)     2063 2020-09-02 14:40:23.000000 dkd-0.7.7/dkd/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3784 2020-09-03 18:53:42.000000 dkd-0.7.7/dkd/content.py
--rw-r--r--   0 moky       (501) staff       (20)     8669 2020-09-02 14:40:23.000000 dkd-0.7.7/dkd/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     6002 2020-09-02 15:29:44.000000 dkd-0.7.7/dkd/envelope.py
--rw-r--r--   0 moky       (501) staff       (20)     8585 2020-09-03 19:55:17.000000 dkd-0.7.7/dkd/instant.py
--rw-r--r--   0 moky       (501) staff       (20)     4802 2020-09-02 14:40:23.000000 dkd-0.7.7/dkd/message.py
--rw-r--r--   0 moky       (501) staff       (20)     5395 2020-09-02 14:40:23.000000 dkd-0.7.7/dkd/reliable.py
--rw-r--r--   0 moky       (501) staff       (20)    10632 2020-09-02 14:40:23.000000 dkd-0.7.7/dkd/secure.py
--rw-r--r--   0 moky       (501) staff       (20)     4371 2020-03-02 07:40:32.000000 dkd-0.7.7/dkd/types.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-03 20:27:39.000000 dkd-0.7.7/dkd.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     7608 2020-09-03 20:27:38.000000 dkd-0.7.7/dkd.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      262 2020-09-03 20:27:39.000000 dkd-0.7.7/dkd.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2020-09-03 20:27:38.000000 dkd-0.7.7/dkd.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2020-09-03 20:27:38.000000 dkd-0.7.7/dkd.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2020-09-03 20:27:39.000000 dkd-0.7.7/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      859 2020-09-03 20:15:40.000000 dkd-0.7.7/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-04 17:23:12.000000 dkd-0.8.0/
+-rw-r--r--   0 moky       (501) staff       (20)     7608 2020-09-04 17:23:12.000000 dkd-0.8.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     5796 2020-02-06 10:13:12.000000 dkd-0.8.0/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-04 17:23:12.000000 dkd-0.8.0/dkd/
+-rw-r--r--   0 moky       (501) staff       (20)     2063 2020-09-02 14:40:23.000000 dkd-0.8.0/dkd/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3862 2020-09-04 16:59:41.000000 dkd-0.8.0/dkd/content.py
+-rw-r--r--   0 moky       (501) staff       (20)     8988 2020-09-04 13:05:07.000000 dkd-0.8.0/dkd/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     5235 2020-09-04 17:00:15.000000 dkd-0.8.0/dkd/envelope.py
+-rw-r--r--   0 moky       (501) staff       (20)     9023 2020-09-04 17:08:26.000000 dkd-0.8.0/dkd/instant.py
+-rw-r--r--   0 moky       (501) staff       (20)     4914 2020-09-04 17:10:12.000000 dkd-0.8.0/dkd/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     5797 2020-09-04 13:20:02.000000 dkd-0.8.0/dkd/reliable.py
+-rw-r--r--   0 moky       (501) staff       (20)    11308 2020-09-04 17:10:27.000000 dkd-0.8.0/dkd/secure.py
+-rw-r--r--   0 moky       (501) staff       (20)     5329 2020-09-04 13:24:50.000000 dkd-0.8.0/dkd/types.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-09-04 17:23:12.000000 dkd-0.8.0/dkd.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     7608 2020-09-04 17:23:12.000000 dkd-0.8.0/dkd.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      262 2020-09-04 17:23:12.000000 dkd-0.8.0/dkd.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2020-09-04 17:23:12.000000 dkd-0.8.0/dkd.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2020-09-04 17:23:12.000000 dkd-0.8.0/dkd.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2020-09-04 17:23:12.000000 dkd-0.8.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      859 2020-09-04 12:21:37.000000 dkd-0.8.0/setup.py
```

### Comparing `dkd-0.7.7/PKG-INFO` & `dkd-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkd
-Version: 0.7.7
+Version: 0.8.0
 Summary: A common message module
 Home-page: https://github.com/dimchat/dkd-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Dao Ke Dao (道可道) -- Message Module (Python)
```

### Comparing `dkd-0.7.7/README.md` & `dkd-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dkd-0.7.7/dkd/__init__.py` & `dkd-0.8.0/dkd/__init__.py`

 * *Files identical despite different names*

### Comparing `dkd-0.7.7/dkd/content.py` & `dkd-0.8.0/dkd/content.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,20 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 import weakref
+from typing import Optional, Generic
 
+from .types import ID
 
-class Content(dict):
+
+class Content(dict, Generic[ID]):
     """This class is for creating message content
 
         Message Content
         ~~~~~~~~~~~~~~~
 
         data format: {
             'type'    : 0x00,            // message type
@@ -59,15 +62,15 @@
         # lazy
         self.__type: int = None
         self.__sn: int = None
         self.__time: int = None
         self.__group = None
 
     @property
-    def delegate(self):  # Optional[MessageDelegate]
+    def delegate(self):  # Optional[MessageDelegate[ID]]:
         if self.__delegate is not None:
             return self.__delegate()
 
     @delegate.setter
     def delegate(self, value):
         if value is None:
             self.__delegate = None
@@ -97,15 +100,15 @@
             else:
                 self.__time = int(time)
         return self.__time
 
     # Group ID/string for group message
     #    if field 'group' exists, it means this is a group message
     @property
-    def group(self):  # Optional[ID]
+    def group(self) -> Optional[ID]:
         if self.__group is None:
             self.__group = self.delegate.identifier(string=self.get('group'))
         return self.__group
 
     @group.setter
     def group(self, value: str):
         if value is None:
```

### Comparing `dkd-0.7.7/dkd/delegate.py` & `dkd-0.8.0/dkd/delegate.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,243 +25,244 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from abc import ABC, abstractmethod
-from typing import Optional
+from typing import Optional, Generic
 
+from .types import ID, KEY
 from .content import Content
 from .instant import InstantMessage
 from .secure import SecureMessage
 from .reliable import ReliableMessage
 
 
 #
 #  Message Delegates
 #
 
-class MessageDelegate(ABC):
+class MessageDelegate(ABC, Generic[ID]):
 
     @abstractmethod
-    def identifier(self, string: str):  # ID
+    def identifier(self, string: str) -> ID:
         """
         Create entity ID with String
 
         :param string: ID string
         :return: ID object
         """
         raise NotImplemented
 
 
-class InstantMessageDelegate(MessageDelegate):
+class InstantMessageDelegate(MessageDelegate[ID], Generic[ID, KEY]):
 
     """ Delegate for InstantMessage """
 
-    def content(self, content: dict) -> Optional[Content]:
+    def content(self, content: dict) -> Optional[Content[ID]]:
         """
         0. Convert Map object to Content object
 
         :param content: message content info
         :return: Content object
         """
         raise NotImplemented
 
     """ Encrypt Content """
 
-    def serialize_content(self, content: Content, key, msg: InstantMessage) -> bytes:
+    def serialize_content(self, content: Content[ID], key: KEY, msg: InstantMessage[ID, KEY]) -> bytes:
         """
         1. Serialize 'message.content' to data (JsON / ProtoBuf / ...)
 
         :param content:  message content
         :param key:      symmetric key
         :param msg:      instant message
         :return:         serialized content data
         """
         raise NotImplemented
 
     @abstractmethod
-    def encrypt_content(self, data: bytes, key, msg: InstantMessage) -> bytes:
+    def encrypt_content(self, data: bytes, key: KEY, msg: InstantMessage[ID, KEY]) -> bytes:
         """
         2. Encrypt content data to 'message.data' with symmetric key
 
         :param data:     serialized data of message.content
         :param key:      symmetric key
         :param msg:      instant message
         :return:         encrypted message content data
         """
         raise NotImplemented
 
     @abstractmethod
-    def encode_data(self, data: bytes, msg: InstantMessage) -> str:
+    def encode_data(self, data: bytes, msg: InstantMessage[ID, KEY]) -> str:
         """
         3. Encode 'message.data' to String (Base64)
 
         :param data:     encrypted content data
         :param msg:      instant message
         :return:         string
         """
         raise NotImplemented
 
     """ Encrypt Key """
 
-    def serialize_key(self, key, msg: InstantMessage) -> Optional[bytes]:
+    def serialize_key(self, key: KEY, msg: InstantMessage[ID, KEY]) -> Optional[bytes]:
         """
         4. Serialize message key to data (JsON / ProtoBuf / ...)
 
         :param key:      symmetric key to be encrypted
         :param msg:      instant message
         :return:         serialized key data
         """
         raise NotImplemented
 
     @abstractmethod
-    def encrypt_key(self, data: bytes, receiver, msg: InstantMessage) -> Optional[bytes]:
+    def encrypt_key(self, data: bytes, receiver: ID, msg: InstantMessage[ID, KEY]) -> Optional[bytes]:
         """
         5. Encrypt key data to 'message.key' with receiver's public key
 
         :param data:     serialized data of symmetric key
         :param receiver: receiver ID
         :param msg:      instant message
         :return:         encrypted key data
         """
         raise NotImplemented
 
     @abstractmethod
-    def encode_key(self, data: bytes, msg: InstantMessage) -> str:
+    def encode_key(self, data: bytes, msg: InstantMessage[ID, KEY]) -> str:
         """
         6. Encode 'message.key' to String (Base64)
 
         :param data:     encrypted key data
         :param msg:      instant message
         :return:         base64 string
         """
         raise NotImplemented
 
 
-class SecureMessageDelegate(MessageDelegate):
+class SecureMessageDelegate(MessageDelegate[ID], Generic[ID, KEY]):
 
     """ Delegate for SecureMessage """
 
     """ Decrypt Key """
 
     @abstractmethod
-    def decode_key(self, key: str, msg: SecureMessage) -> Optional[bytes]:
+    def decode_key(self, key: str, msg: SecureMessage[ID, KEY]) -> Optional[bytes]:
         """
         1. Decode 'message.key' to encrypted symmetric key data
 
         :param key:      base64 string
         :param msg:      secure message
         :return:         encrypted symmetric key data
         """
         raise NotImplemented
 
     @abstractmethod
-    def decrypt_key(self, data: bytes, sender, receiver, msg: SecureMessage) -> Optional[bytes]:
+    def decrypt_key(self, data: bytes, sender: ID, receiver: ID, msg: SecureMessage[ID, KEY]) -> Optional[bytes]:
         """
         2. Decrypt 'message.key' with receiver's private key
 
         :param data:     encrypted symmetric key data
         :param sender:   sender/member ID
         :param receiver: receiver/group ID
         :param msg:      secure message
         :return:         serialized data of symmetric key
         """
         raise NotImplemented
 
-    def deserialize_key(self, data: Optional[bytes], sender, receiver, msg: SecureMessage):  # Optional[KEY]
+    def deserialize_key(self, data: Optional[bytes], sender: ID, receiver: ID, msg: SecureMessage[ID, KEY]):  # KEY
         """
         3. Deserialize message key from data (JsON / ProtoBuf / ...)
 
         :param data:     serialized key data
         :param sender:   sender/member ID
         :param receiver: receiver/group ID
         :param msg:      secure message
         :return:         symmetric key
         """
         raise NotImplemented
 
     """ Decrypt Content """
 
     @abstractmethod
-    def decode_data(self, data: str, msg: SecureMessage) -> Optional[bytes]:
+    def decode_data(self, data: str, msg: SecureMessage[ID, KEY]) -> Optional[bytes]:
         """
         4. Decode 'message.data' to encrypted content data
 
         :param data:     base64 string
         :param msg:      secure message
         :return:         encrypted content data
         """
         raise NotImplemented
 
     @abstractmethod
-    def decrypt_content(self, data: bytes, key, msg: SecureMessage) -> Optional[bytes]:
+    def decrypt_content(self, data: bytes, key: KEY, msg: SecureMessage[ID, KEY]) -> Optional[bytes]:
         """
         5. Decrypt 'message.data' with symmetric key
 
         :param data:     encrypted content data
         :param key:      symmetric key
         :param msg:      secure message
         :return:         serialized data of message content
         """
         raise NotImplemented
 
-    def deserialize_content(self, data: bytes, key, msg: SecureMessage) -> Optional[Content]:
+    def deserialize_content(self, data: bytes, key: KEY, msg: SecureMessage[ID, KEY]) -> Optional[Content[ID]]:
         """
         6. Deserialize message content from data (JsON / ProtoBuf / ...)
 
         :param data:     serialized content data
         :param key:      symmetric key
         :param msg:      secure message
         :return:         message content
         """
         raise NotImplemented
 
     """ Signature """
 
     @abstractmethod
-    def sign_data(self, data: bytes, sender, msg: SecureMessage) -> bytes:
+    def sign_data(self, data: bytes, sender: ID, msg: SecureMessage[ID, KEY]) -> bytes:
         """
         1. Sign 'message.data' with sender's private key
 
         :param data:      encrypted message data
         :param sender:    sender ID
         :param msg:       secure message
         :return:          signature of encrypted message data
         """
         raise NotImplemented
 
     @abstractmethod
-    def encode_signature(self, signature: bytes, msg: SecureMessage) -> str:
+    def encode_signature(self, signature: bytes, msg: SecureMessage[ID, KEY]) -> str:
         """
         2. Encode 'message.signature' to String (Base64)
 
         :param signature: signature of message.data
         :param msg:       secure message
         :return:          string
         """
         raise NotImplemented
 
 
-class ReliableMessageDelegate(SecureMessageDelegate):
+class ReliableMessageDelegate(SecureMessageDelegate[ID, KEY], Generic[ID, KEY]):
 
     @abstractmethod
-    def decode_signature(self, signature: str, msg: ReliableMessage) -> Optional[bytes]:
+    def decode_signature(self, signature: str, msg: ReliableMessage[ID, KEY]) -> Optional[bytes]:
         """
         1. Decode 'message.signature' from String (Base64)
 
         :param signature: base64 string
         :param msg:       reliable message
         :return:          signature data
         """
         raise NotImplemented
 
     @abstractmethod
-    def verify_data_signature(self, data: bytes, signature: bytes, sender, msg: ReliableMessage) -> bool:
+    def verify_data_signature(self, data: bytes, signature: bytes, sender: ID, msg: ReliableMessage[ID, KEY]) -> bool:
         """
         2. Verify the message data and signature with sender's public key
 
         :param data:      message content(encrypted) data
         :param signature: signature of message content(encrypted) data
         :param sender:    sender ID
         :param msg:       reliable message
```

### Comparing `dkd-0.7.7/dkd/envelope.py` & `dkd-0.8.0/dkd/envelope.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,53 +26,20 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 import time as time_lib
 import weakref
-from typing import MutableMapping, Iterator
+from typing import Optional, Generic
 
-
-class Dictionary(MutableMapping):
-    """
-        A container sharing the same inner dictionary
-    """
-
-    def __init__(self, dictionary: dict):
-        super().__init__()
-        self.__dictionary = dictionary
-
-    @property
-    def dictionary(self) -> dict:
-        return self.__dictionary
-
-    def __iter__(self) -> Iterator:
-        return iter(self.__dictionary)
-
-    def __len__(self) -> int:
-        return len(self.__dictionary)
-
-    def __setitem__(self, key, value):
-        self.__dictionary[key] = value
-
-    def __getitem__(self, key):
-        return self.__dictionary[key]
-
-    def __delitem__(self, key) -> None:
-        del self.__dictionary[key]
-
-    def get(self, key):
-        return self.__dictionary.get(key)
-
-    def pop(self, key, default=None):
-        return self.__dictionary.pop(key, default)
+from .types import ID, Dictionary
 
 
-class Envelope(Dictionary):
+class Envelope(Dictionary, Generic[ID]):
     """This class is used to create a message envelope
     which contains 'sender', 'receiver' and 'time'
 
         Envelope for message
         ~~~~~~~~~~~~~~~~~~~~
 
         data format: {
@@ -101,41 +68,41 @@
     def __init__(self, envelope: dict):
         if self is envelope:
             # no need to init again
             return
         super().__init__(envelope)
         self.__delegate: weakref.ReferenceType = None
         # lazy
-        self.__sender = None
-        self.__receiver = None
+        self.__sender: ID = None
+        self.__receiver: ID = None
         self.__time: int = None
         # extra info
-        self.__group = None
+        self.__group: ID = None
         self.__type: int = None
 
     @property
-    def delegate(self):  # Optional[MessageDelegate]
+    def delegate(self):  # Optional[MessageDelegate[ID]]:
         if self.__delegate is not None:
             return self.__delegate()
 
     @delegate.setter
     def delegate(self, value):
         if value is None:
             self.__delegate = None
         else:
             self.__delegate = weakref.ref(value)
 
     @property
-    def sender(self):  # ID
+    def sender(self) -> ID:
         if self.__sender is None:
             self.__sender = self.delegate.identifier(string=self['sender'])
         return self.__sender
 
     @property
-    def receiver(self):  # ID
+    def receiver(self) -> ID:
         if self.__receiver is None:
             self.__receiver = self.delegate.identifier(string=self['receiver'])
         return self.__receiver
 
     @property
     def time(self) -> int:
         if self.__time is None:
@@ -150,15 +117,15 @@
         Group ID
         ~~~~~~~~
         when a group message was split/trimmed to a single message
         the 'receiver' will be changed to a member ID, and
         the group ID will be saved as 'group'.
     """
     @property
-    def group(self):  # Optional[ID]
+    def group(self) -> Optional[ID]:
         if self.__group is None:
             self.__group = self.delegate.identifier(string=self.get('group'))
         return self.__group
 
     @group.setter
     def group(self, value: str):
         if value is None:
```

### Comparing `dkd-0.7.7/dkd/instant.py` & `dkd-0.8.0/dkd/instant.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,26 +24,26 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-import time as time_lib
 import weakref
-from typing import Optional
+from typing import Union, Optional, Generic
 
+from .types import ID, KEY
 from .envelope import Envelope
 from .content import Content
 from .message import Message
 
-import dkd  # dkd.SecureMessage
+import dkd  # dkd.InstantMessageDelegate, dkd.SecureMessage
 
 
-class InstantMessage(Message):
+class InstantMessage(Message[ID, KEY], Generic[ID, KEY]):
     """
         Instant Message
         ~~~~~~~~~~~~~~~
 
         data format: {
             //-- envelope
             sender   : "moki@xxx",
@@ -73,20 +73,22 @@
     def __init__(self, msg: dict):
         if self is msg:
             # no need to init again
             return
         super().__init__(msg)
         self.__delegate: weakref.ReferenceType = None
         # lazy
-        self.__content: Content = None
+        self.__content: Content[ID] = None
 
     @property
-    def content(self) -> Content:
+    def content(self) -> Content[ID]:
         if self.__content is None:
-            self.__content = self.delegate.content(self['content'])
+            delegate = self.delegate
+            assert isinstance(delegate, dkd.InstantMessageDelegate), 'instant delegate error: %s' % delegate
+            self.__content = delegate.content(self['content'])
         return self.__content
 
     @property
     def delegate(self):  # Optional[InstantMessageDelegate]
         return self.envelope.delegate
 
     @delegate.setter
@@ -98,15 +100,15 @@
     def time(self) -> Optional[int]:
         value = self.content.time
         if value > 0:
             return value
         return self.envelope.time
 
     @property
-    def group(self):  # ID
+    def group(self) -> ID:
         return self.content.group
 
     @property
     def type(self) -> Optional[int]:
         return self.content.type
 
     """
@@ -119,15 +121,15 @@
             | time     |  ->  | time     |
             |          |      |          |
             | content  |      | data     |  1. data = encrypt(content, PW)
             +----------+      | key/keys |  2. key  = encrypt(PW, receiver.PK)
                               +----------+
     """
 
-    def encrypt(self, password, members: list=None):  # -> Optional[dkd.SecureMessage]:
+    def encrypt(self, password: KEY, members: list=None):  # -> Optional[dkd.SecureMessage]:
         """
         Encrypt message content with password(symmetric key)
 
         :param password: A symmetric key for encrypting message content
         :param members:  If this is a group message, get all members here
         :return: SecureMessage object
         """
@@ -139,21 +141,22 @@
             # personal message
             msg = self.__encrypt_key(password=password)
         else:
             # group message
             msg = self.__encrypt_keys(password=password, members=members)
 
         # 3. pack message
-        return dkd.SecureMessage(msg)
+        return dkd.SecureMessage[ID, KEY](msg)
 
-    def __encrypt_key(self, password) -> Optional[dict]:
+    def __encrypt_key(self, password: KEY) -> Optional[dict]:
         # 1. encrypt 'message.content' to 'message.data'
         msg = self.__prepare_data(password=password)
         # 2. encrypt symmetric key(password) to 'message.key'
         delegate = self.delegate
+        assert isinstance(delegate, dkd.InstantMessageDelegate), 'instant delegate error: %s' % delegate
         # 2.1. serialize symmetric key
         key = delegate.serialize_key(key=password, msg=self)
         if key is None:
             # A) broadcast message has no key
             # B) reused key
             return msg
         # 2.2. encrypt symmetric key data
@@ -165,19 +168,20 @@
         # 2.3. encode encrypted key data
         base64 = delegate.encode_key(data=data, msg=self)
         assert base64 is not None, 'failed to encode key data: %s' % data
         # 2.4. insert as 'key'
         msg['key'] = base64
         return msg
 
-    def __encrypt_keys(self, password, members: list) -> dict:
+    def __encrypt_keys(self, password: KEY, members: list) -> dict:
         # 1. encrypt 'message.content' to 'message.data'
         msg = self.__prepare_data(password=password)
         # 2. encrypt symmetric key(password) to 'message.key'
         delegate = self.delegate
+        assert isinstance(delegate, dkd.InstantMessageDelegate), 'instant delegate error: %s' % delegate
         # 2.1. serialize symmetric key
         key = delegate.serialize_key(key=password, msg=self)
         if key is None:
             # A) broadcast message has no key
             # B) reused key
             return msg
         # encrypt key data to 'message.keys'
@@ -196,16 +200,17 @@
             # 2.4. insert to 'message.keys' with member ID
             keys[member] = base64
             count += 1
         if count > 0:
             msg['keys'] = keys
         return msg
 
-    def __prepare_data(self, password) -> dict:
+    def __prepare_data(self, password: KEY) -> dict:
         delegate = self.delegate
+        assert isinstance(delegate, dkd.InstantMessageDelegate), 'instant delegate error: %s' % delegate
         # 1. serialize message content
         data = delegate.serialize_content(content=self.content, key=password, msg=self)
         assert data is not None, 'failed to serialize content: %s' % self.content
         # 2. encrypt content data with password
         data = delegate.encrypt_content(data=data, key=password, msg=self)
         assert data is not None, 'failed to encrypt content with key: %s' % password
         # 3. encode encrypted data
@@ -217,25 +222,19 @@
         msg['data'] = base64
         return msg
 
     #
     #  Factory
     #
     @classmethod
-    def new(cls, content: Content, envelope: Envelope=None,
-            sender: str=None, receiver: str=None, time: int=0):
-        if envelope:
-            # share the same dictionary with envelope object
+    def new(cls, content: dict, envelope: Union[Envelope, dict]=None,
+            sender: str=None, receiver: str=None, time: int=0):  # InstantMessage
+        # message will share the same dictionary with envelope object
+        if isinstance(envelope, Envelope):
             msg = envelope.dictionary
-            msg['content'] = content
+        elif isinstance(envelope, dict):
+            msg = envelope
         else:
-            assert sender is not None and receiver is not None, 'sender/receiver error'
-            if time == 0:
-                time = int(time_lib.time())
-            # build instant message info
-            msg = {
-                'sender': sender,
-                'receiver': receiver,
-                'time': time,
-                'content': content,
-            }
+            envelope = Envelope.new(sender=sender, receiver=receiver, time=time)
+            msg = envelope.dictionary
+        msg['content'] = content
         return cls(msg)
```

### Comparing `dkd-0.7.7/dkd/message.py` & `dkd-0.8.0/dkd/message.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,20 +44,23 @@
                                                +--------------+
         Algorithm:
             data      = password.encrypt(content)
             key       = receiver.public_key.encrypt(password)
             signature = sender.private_key.sign(data)
 """
 
+from typing import Generic
+
+from .types import ID, KEY
 from .envelope import Envelope
 
 import dkd  # dkd.InstantMessage, dkd.ReliableMessage
 
 
-class Message(dict):
+class Message(dict, Generic[ID, KEY]):
     """This class is used to create a message
     with the envelope fields, such as 'sender', 'receiver', and 'time'
 
         Message with Envelope
         ~~~~~~~~~~~~~~~~~~~~~
         Base classes for messages
 
@@ -80,64 +83,64 @@
         :return: Message object
         """
         if msg is None:
             return None
         elif cls is Message:
             if 'content' in msg:
                 # this should be an instant message
-                return dkd.InstantMessage.__new__(dkd.InstantMessage, msg)
+                return dkd.InstantMessage.__new__(dkd.InstantMessage[ID, KEY], msg)
             if 'signature' in msg:
                 # this should be a reliable message
-                return dkd.ReliableMessage.__new__(dkd.ReliableMessage, msg)
+                return dkd.ReliableMessage.__new__(dkd.ReliableMessage[ID, KEY], msg)
             if 'data' in msg:
                 # this should be a secure message
-                return dkd.SecureMessage.__new__(dkd.SecureMessage, msg)
+                return dkd.SecureMessage.__new__(dkd.SecureMessage[ID, KEY], msg)
             if isinstance(msg, Message):
                 # return Message object directly
                 return msg
         # subclass or default Message(dict)
         return super().__new__(cls, msg)
 
     def __init__(self, msg: dict):
         if self is msg:
             # no need to init again
             return
         super().__init__(msg)
         # lazy
-        self.__envelope: Envelope = None
+        self.__envelope: Envelope[ID] = None
 
     @property
-    def envelope(self) -> Envelope:
+    def envelope(self) -> Envelope[ID]:
         if self.__envelope is None:
             # let envelope share the same dictionary with message
-            self.__envelope = Envelope(self)
+            self.__envelope = Envelope[ID](self)
         return self.__envelope
 
     @property
     def delegate(self):  # Optional[MessageDelegate]
         return self.envelope.delegate
 
     @delegate.setter
     def delegate(self, value):
         self.envelope.delegate = value
 
     # --------
 
     @property
-    def sender(self):  # ID
+    def sender(self) -> ID:
         return self.envelope.sender
 
     @property
-    def receiver(self):  # ID
+    def receiver(self) -> ID:
         return self.envelope.receiver
 
     @property
     def time(self) -> int:
         return self.envelope.time
 
     @property
-    def group(self):  # ID
+    def group(self) -> ID:
         return self.envelope.group
 
     @property
     def type(self) -> int:
         return self.envelope.type
```

### Comparing `dkd-0.7.7/dkd/reliable.py` & `dkd-0.8.0/dkd/reliable.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,20 +24,23 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-from typing import Optional
+from typing import Optional, Generic
 
+from .types import ID, KEY
 from .secure import SecureMessage
 
+import dkd  # dkd.ReliableMessageDelegate
 
-class ReliableMessage(SecureMessage):
+
+class ReliableMessage(SecureMessage[ID, KEY], Generic[ID, KEY]):
     """This class is used to sign the SecureMessage
     It contains a 'signature' field which signed with sender's private key
 
         Instant Message signed by an asymmetric key
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
         data format: {
@@ -81,15 +84,17 @@
         self.__signature = None
 
     @property
     def signature(self) -> bytes:
         if self.__signature is None:
             base64 = self.get('signature')
             assert base64 is not None, 'signature of reliable message cannot be empty: %s' % self
-            self.__signature = self.delegate.decode_signature(signature=base64, msg=self)
+            delegate = self.delegate
+            assert isinstance(delegate, dkd.ReliableMessageDelegate), 'reliable delegate error: %s' % delegate
+            self.__signature = delegate.decode_signature(signature=base64, msg=self)
         return self.__signature
 
     """
         Sender's Meta
         ~~~~~~~~~~~~~
         Extends for the first message package of 'Handshake' protocol.
     """
@@ -131,27 +136,29 @@
             |          |      |          |
             | data     |      | data     |  1. verify(data, signature, sender.PK)
             | key/keys |      | key/keys |
             | signature|      +----------+
             +----------+
     """
 
-    def verify(self) -> Optional[SecureMessage]:
+    def verify(self) -> Optional[SecureMessage[ID, KEY]]:
         """
         Verify the message.data with signature
 
         :return: SecureMessage object if signature matched
         """
         data = self.data
         if data is None:
             raise ValueError('failed to decode content data: %s' % self)
         signature = self.signature
         if signature is None:
             raise ValueError('failed to decode message signature: %s' % self)
         # 1. verify data signature
-        if self.delegate.verify_data_signature(data=data, signature=signature, sender=self.sender, msg=self):
+        delegate = self.delegate
+        assert isinstance(delegate, dkd.ReliableMessageDelegate), 'reliable delegate error: %s' % delegate
+        if delegate.verify_data_signature(data=data, signature=signature, sender=self.sender, msg=self):
             # 2. pack message
             msg = self.copy()
             msg.pop('signature')  # remove 'signature'
-            return SecureMessage(msg)
+            return SecureMessage[ID, KEY](msg)
         # else:
         #     raise ValueError('Signature error: %s' % self)
```

### Comparing `dkd-0.7.7/dkd/secure.py` & `dkd-0.8.0/dkd/secure.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,23 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-from typing import Optional
+from typing import Optional, Generic
 
+from .types import ID, KEY
 from .message import Message
 
-import dkd  # dkd.InstantMessage, dkd.ReliableMessage
+import dkd  # dkd.SecureMessageDelegate, dkd.InstantMessage, dkd.ReliableMessage
 
 
-class SecureMessage(Message):
+class SecureMessage(Message[ID, KEY], Generic[ID, KEY]):
     """Instant Message encrypted by a symmetric key
 
         Secure Message
         ~~~~~~~~~~~~~~
 
         data format: {
             //-- envelope
@@ -64,15 +65,15 @@
         """
         if msg is None:
             return None
         elif cls is SecureMessage:
             if 'signature' in msg:
                 # this should be a reliable message
                 # noinspection PyTypeChecker
-                return dkd.ReliableMessage.__new__(dkd.ReliableMessage, msg)
+                return dkd.ReliableMessage.__new__(dkd.ReliableMessage[ID, KEY], msg)
             elif isinstance(msg, SecureMessage):
                 # return SecureMessage object directly
                 return msg
         # subclass or SecureMessage(dict)
         return super().__new__(cls, msg)
 
     def __init__(self, msg: dict):
@@ -86,28 +87,32 @@
         self.__keys: dict = None
 
     @property
     def data(self) -> bytes:
         if self.__data is None:
             base64 = self.get('data')
             assert base64 is not None, 'secure message data cannot be empty'
-            self.__data = self.delegate.decode_data(data=base64, msg=self)
+            delegate = self.delegate
+            assert isinstance(delegate, dkd.SecureMessageDelegate), 'secure delegate error: %s' % delegate
+            self.__data = delegate.decode_data(data=base64, msg=self)
         return self.__data
 
     @property
     def encrypted_key(self) -> Optional[bytes]:
         if self.__key is None:
             base64 = self.get('key')
             if base64 is None:
                 # check 'keys'
                 keys = self.encrypted_keys
                 if keys is not None:
                     base64 = keys.get(self.receiver)
             if base64 is not None:
-                self.__key = self.delegate.decode_key(key=base64, msg=self)
+                delegate = self.delegate
+                assert isinstance(delegate, dkd.SecureMessageDelegate), 'secure delegate error: %s' % delegate
+                self.__key = delegate.decode_key(key=base64, msg=self)
         return self.__key
 
     @property
     def encrypted_keys(self) -> Optional[dict]:
         if self.__keys is None:
             self.__keys = self.get('keys')
         return self.__keys
@@ -122,15 +127,15 @@
             | time     |  ->  | time     |
             |          |      |          |  1. PW      = decrypt(key, receiver.SK)
             | data     |      | content  |  2. content = decrypt(data, PW)
             | key/keys |      +----------+
             +----------+
     """
 
-    def decrypt(self) -> Optional[dkd.InstantMessage]:
+    def decrypt(self) -> Optional[dkd.InstantMessage[ID, KEY]]:
         """
         Decrypt message data to plaintext content
 
         :return: InstantMessage object
         """
         sender = self.sender
         group = self.group
@@ -140,14 +145,15 @@
             receiver = self.receiver
         else:
             # group message
             receiver = group
 
         # 1. decrypt 'message.key' to symmetric key
         delegate = self.delegate
+        assert isinstance(delegate, dkd.SecureMessageDelegate), 'secure delegate error: %s' % delegate
         # 1.1. decode encrypted key data
         key = self.encrypted_key
         # 1.2. decrypt key data
         if key is not None:
             key = delegate.decrypt_key(data=key, sender=sender, receiver=receiver, msg=self)
             if key is None:
                 raise AssertionError('failed to decrypt key in msg: %s' % self)
@@ -179,15 +185,15 @@
 
         # 3. pack message
         msg = self.copy()
         msg.pop('key', None)
         msg.pop('keys', None)
         msg.pop('data')
         msg['content'] = content
-        return dkd.InstantMessage(msg)
+        return dkd.InstantMessage[ID, KEY](msg)
 
     """
         Sign the Secure Message to Reliable Message
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
             +----------+      +----------+
             | sender   |      | sender   |
@@ -203,24 +209,26 @@
     def sign(self):  # -> dkd.ReliableMessage:
         """
         Sign the message.data with sender's private key
 
         :return: ReliableMessage object
         """
         data = self.data
+        delegate = self.delegate
+        assert isinstance(delegate, dkd.SecureMessageDelegate), 'secure delegate error: %s' % delegate
         # 1. sign message.data
-        signature = self.delegate.sign_data(data=data, sender=self.sender, msg=self)
+        signature = delegate.sign_data(data=data, sender=self.sender, msg=self)
         assert signature is not None, 'failed to sign message: %s' % self
         # 2. encode signature
-        base64 = self.delegate.encode_signature(signature=signature, msg=self)
+        base64 = delegate.encode_signature(signature=signature, msg=self)
         assert base64 is not None, 'failed to encode signature: %s' % signature
         # 3. pack message
         msg = self.copy()
         msg['signature'] = base64
-        return dkd.ReliableMessage(msg)
+        return dkd.ReliableMessage[ID, KEY](msg)
 
     """
         Split/Trim group message
         ~~~~~~~~~~~~~~~~~~~~~~~~
         
         for each members, get key from 'keys' and replace 'receiver' to member ID
     """
@@ -257,21 +265,21 @@
             key = keys.get(member)
             if key is None:
                 msg.pop('key', None)
             else:
                 msg['key'] = key
             # 4. pack message
             if reliable:
-                messages.append(dkd.ReliableMessage(msg))
+                messages.append(dkd.ReliableMessage[ID, KEY](msg))
             else:
-                messages.append(SecureMessage(msg))
+                messages.append(SecureMessage[ID, KEY](msg))
         # OK
         return messages
 
-    def trim(self, member: str):  # -> SecureMessage
+    def trim(self, member: ID):  # -> SecureMessage
         """
         Trim the group message for a member
 
         :param member: Member ID
         :return:       A SecureMessage object drop all irrelevant keys to the member
         """
         msg = self.copy()
@@ -290,10 +298,10 @@
             # it will not be equal to the member of course,
             # so move 'receiver' to 'group'
             msg['group'] = self.receiver
         # replace receiver
         msg['receiver'] = member
         # repack
         if 'signature' in msg:
-            return dkd.ReliableMessage(msg)
+            return dkd.ReliableMessage[ID, KEY](msg)
         else:
-            return SecureMessage(msg)
+            return SecureMessage[ID, KEY](msg)
```

### Comparing `dkd-0.7.7/dkd/types.py` & `dkd-0.8.0/dkd/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from enum import IntEnum
+from typing import TypeVar, MutableMapping, Iterator
+
+
+# generics
+ID = TypeVar('ID', str, object)
+KEY = TypeVar('KEY', dict, object)
 
 
 class ContentType(IntEnum):
     """
         @enum DKDContentType
 
         @abstract A flag to indicate what kind of message content this is.
@@ -100,7 +106,42 @@
     SplitBill = 0x49     # 0100 1001 (Split the bill)
 
     Command = 0x88     # 1000 1000
     History = 0x89     # 1000 1001 (Entity history command)
 
     # top-secret message forward by proxy (Service Provider)
     Forward = 0xFF  # 1111 1111
+
+
+class Dictionary(MutableMapping):
+    """
+        A container sharing the same inner dictionary
+    """
+
+    def __init__(self, dictionary: dict):
+        super().__init__()
+        self.__dictionary = dictionary
+
+    @property
+    def dictionary(self) -> dict:
+        return self.__dictionary
+
+    def __iter__(self) -> Iterator:
+        return iter(self.__dictionary)
+
+    def __len__(self) -> int:
+        return len(self.__dictionary)
+
+    def __setitem__(self, key, value):
+        self.__dictionary[key] = value
+
+    def __getitem__(self, key):
+        return self.__dictionary[key]
+
+    def __delitem__(self, key) -> None:
+        del self.__dictionary[key]
+
+    def get(self, key):
+        return self.__dictionary.get(key)
+
+    def pop(self, key, default=None):
+        return self.__dictionary.pop(key, default)
```

### Comparing `dkd-0.7.7/dkd.egg-info/PKG-INFO` & `dkd-0.8.0/dkd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkd
-Version: 0.7.7
+Version: 0.8.0
 Summary: A common message module
 Home-page: https://github.com/dimchat/dkd-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Dao Ke Dao (道可道) -- Message Module (Python)
```

### Comparing `dkd-0.7.7/setup.py` & `dkd-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~~~~~~~~
 
     Common Message Module for decentralized instant messaging
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '0.7.7'
+__version__ = '0.8.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
```

