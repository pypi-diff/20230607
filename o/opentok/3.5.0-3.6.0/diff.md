# Comparing `tmp/opentok-3.5.0.tar.gz` & `tmp/opentok-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opentok-3.5.0.tar", last modified: Tue May  9 16:58:21 2023, max compression
+gzip compressed data, was "dist/opentok-3.6.0.tar", last modified: Wed Jun  7 11:57:44 2023, max compression
```

## Comparing `opentok-3.5.0.tar` & `opentok-3.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-05-09 16:58:21.000000 opentok-3.5.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     1079 2022-09-05 18:13:07.000000 opentok-3.5.0/LICENSE.txt
--rw-r--r--   0 mkahan     (503) staff       (20)    25836 2023-05-09 16:58:21.000000 opentok-3.5.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)    24531 2023-05-09 16:58:09.000000 opentok-3.5.0/README.rst
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok/
--rw-r--r--   0 mkahan     (503) staff       (20)      605 2023-03-14 18:39:57.000000 opentok-3.5.0/opentok/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     7369 2022-10-12 15:29:40.000000 opentok-3.5.0/opentok/archives.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3754 2023-05-09 16:40:54.000000 opentok-3.5.0/opentok/broadcast.py
--rw-r--r--   0 mkahan     (503) staff       (20)     6229 2023-03-14 18:39:57.000000 opentok-3.5.0/opentok/endpoints.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3270 2023-03-14 18:39:57.000000 opentok-3.5.0/opentok/exceptions.py
--rw-r--r--   0 mkahan     (503) staff       (20)    92855 2023-05-09 16:49:47.000000 opentok-3.5.0/opentok/opentok.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1360 2022-10-12 15:29:40.000000 opentok-3.5.0/opentok/render.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2165 2022-09-05 18:13:07.000000 opentok-3.5.0/opentok/session.py
--rw-r--r--   0 mkahan     (503) staff       (20)      446 2022-09-05 18:13:07.000000 opentok-3.5.0/opentok/sip_call.py
--rw-r--r--   0 mkahan     (503) staff       (20)      899 2022-09-05 18:13:07.000000 opentok-3.5.0/opentok/stream.py
--rw-r--r--   0 mkahan     (503) staff       (20)      809 2022-09-05 18:13:07.000000 opentok-3.5.0/opentok/streamlist.py
--rw-r--r--   0 mkahan     (503) staff       (20)      101 2023-05-09 16:49:47.000000 opentok-3.5.0/opentok/version.py
--rw-r--r--   0 mkahan     (503) staff       (20)      680 2023-03-14 18:39:57.000000 opentok-3.5.0/opentok/websocket_audio_connection.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)    25836 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      472 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       39 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        8 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/top_level.txt
--rw-r--r--   0 mkahan     (503) staff       (20)      103 2023-05-09 16:58:21.000000 opentok-3.5.0/setup.cfg
--rw-r--r--   0 mkahan     (503) staff       (20)     2630 2022-10-12 15:29:40.000000 opentok-3.5.0/setup.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-07 11:57:44.000000 opentok-3.6.0/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1079 2022-09-05 18:13:07.000000 opentok-3.6.0/LICENSE.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)    27854 2023-06-07 11:57:44.000000 opentok-3.6.0/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)    26549 2023-06-07 11:57:23.000000 opentok-3.6.0/README.rst
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok/
+-rw-r--r--   0 mkahan     (503) staff       (20)      605 2023-03-14 18:39:57.000000 opentok-3.6.0/opentok/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     7369 2022-10-12 15:29:40.000000 opentok-3.6.0/opentok/archives.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3973 2023-06-06 16:52:09.000000 opentok-3.6.0/opentok/broadcast.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     6229 2023-03-14 18:39:57.000000 opentok-3.6.0/opentok/endpoints.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3270 2023-03-14 18:39:57.000000 opentok-3.6.0/opentok/exceptions.py
+-rw-r--r--   0 mkahan     (503) staff       (20)    96555 2023-06-06 16:56:02.000000 opentok-3.6.0/opentok/opentok.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1360 2022-10-12 15:29:40.000000 opentok-3.6.0/opentok/render.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2165 2022-09-05 18:13:07.000000 opentok-3.6.0/opentok/session.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      446 2022-09-05 18:13:07.000000 opentok-3.6.0/opentok/sip_call.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      899 2022-09-05 18:13:07.000000 opentok-3.6.0/opentok/stream.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      809 2022-09-05 18:13:07.000000 opentok-3.6.0/opentok/streamlist.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      101 2023-06-07 11:40:16.000000 opentok-3.6.0/opentok/version.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      680 2023-03-14 18:39:57.000000 opentok-3.6.0/opentok/websocket_audio_connection.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)    27854 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      472 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       39 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        8 2023-06-07 11:57:44.000000 opentok-3.6.0/opentok.egg-info/top_level.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)      103 2023-06-07 11:57:44.000000 opentok-3.6.0/setup.cfg
+-rw-r--r--   0 mkahan     (503) staff       (20)     2630 2022-10-12 15:29:40.000000 opentok-3.6.0/setup.py
```

### Comparing `opentok-3.5.0/LICENSE.txt` & `opentok-3.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opentok-3.5.0/PKG-INFO` & `opentok-3.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentok
-Version: 3.5.0
+Version: 3.6.0
 Summary: OpenTok server-side SDK
 Home-page: https://github.com/opentok/Opentok-Python-SDK/
 Author: TokBox, Inc.
 Author-email: support@tokbox.com
 License: LICENSE.txt
 Keywords: video chat tokbox tok opentok python media webrtc archiving realtime
 Classifier: Development Status :: 5 - Production/Stable
@@ -88,14 +88,23 @@
   `OpenTok Media Router <https://tokbox.com/developer/guides/create-session/#media-mode>`_
   or attempt to send streams directly between clients. A routed session is required for some
   OpenTok features (such as archiving).
 
 * ``archive_mode`` which specifies whether the session will be automatically archived (``always``)
   or not (``manual``).
 
+* ``archive_name`` which indicates the archive name for all the archives in auto archived session. 
+  A session that begins with archive mode 'always' will be using this archive name for all archives of that session.
+  Passing 'archive_name' with archive mode 'manual' will cause an error response.
+
+* ``archive_resolution`` which indicates the archive resolution for all the archives in auto archived session.
+  Valid values are '640x480', '480x640', '1280x720', '720x1280', '1920x1080' and '1080x1920'.
+  A session that begins with archive mode 'always' will be using this resolution for all archives of that session.
+  Passing 'archive_resolution' with archive mode 'manual' will cause an error response.
+
 * ``e2ee`` which is a boolean. This specifies whether to enable
   `end-to-end encryption <https://tokbox.com/developer/guides/end-to-end-encryption/>`_
   for the OpenTok session.
 
 This method returns a ``Session`` object. Its ``session_id`` attribute is useful when saving to a persistent
 store (such as a database).
 
@@ -108,14 +117,22 @@
   from opentok import MediaModes
   # A session that uses the OpenTok Media Router, which is required for archiving:
   session = opentok.create_session(media_mode=MediaModes.routed)
 
   # An automatically archived session:
   session = opentok.create_session(media_mode=MediaModes.routed, archive_mode=ArchiveModes.always)
 
+  # An automatically archived session with the archive name and resolution specified:
+  session = opentok.create_session(
+    media_mode=MediaModes.routed,
+    archive_mode=ArchiveModes.always,
+    archive_name='my_archive',
+    archive_resolution='1920x1080'
+  )
+
   # A session with a location hint
   session = opentok.create_session(location=u'12.34.56.78')
 
   # Store this session ID in the database
   session_id = session.session_id
 
 Generating Tokens
@@ -447,14 +464,16 @@
   session_id = 'SESSIONID'
   options = {
     'layout': {
       'type': 'custom',
       'stylesheet': 'the layout stylesheet (only used with type == custom)'
     },
     'maxDuration': 5400,
+    'hasAudio': True
+    'hasVideo': True
     'outputs': {
       'hls': {},
       'rtmp': [{
         'id': 'foo',
         'serverUrl': 'rtmp://myfooserver/myfooapp',
         'streamName': 'myfoostream'
       }, {
@@ -503,14 +522,45 @@
   }
 
   broadcast = opentok.start_broadcast(session_id, options)
   
 To enable multiple simultaneous broadcasts on the same session, specify a unique value for the 
 ``multiBroadcastTag`` parameter in ``options`` when calling the ``opentok.start_broadcast`` method.
 
+You can broadcast only audio, or only video, for a stream by setting ``hasAudio`` or ``hasVideo``
+to ``False`` as required. These fields are ``True`` by default.
+
+.. code:: python
+
+  session_id = 'SESSIONID'
+  options = {
+    'layout': {
+      'type': 'custom',
+      'stylesheet': 'the layout stylesheet (only used with type == custom)'
+    },
+    'maxDuration': 5400,
+    'hasAudio': True
+    'hasVideo': False
+    'outputs': {
+      'hls': {},
+      'rtmp': [{
+        'id': 'foo',
+        'serverUrl': 'rtmp://myfooserver/myfooapp',
+        'streamName': 'myfoostream'
+      }, {
+        'id': 'bar',
+        'serverUrl': 'rtmp://mybarserver/mybarapp',
+        'streamName': 'mybarstream'
+      }]
+    },
+    'resolution': '640x480'
+  }
+
+  broadcast = opentok.start_broadcast(session_id, options)
+
 You can stop a started Broadcast using the ``opentok.stop_broadcast(broadcast_id)`` method.
 
 .. code:: python
 
   # getting the ID from a broadcast object
   broadcast_id = broadcast.id
 
@@ -666,14 +716,23 @@
   
   digits = '12345'
   opentok.play_dtmf(session_id, digits)
 
   # To a specific connection
   opentok.play_dtmf(session_id, connection_id, digits)
 
+Appending to the User Agent
+---------------------------
+
+You can append a string to the user agent that is sent with requests:
+
+.. code:: python
+
+  opentok.append_to_user_agent('my-appended-string')
+
 Samples
 -------
 
 There are two sample applications included in this repository. To get going as fast as possible, clone the whole
 repository and follow the Walkthroughs:
 
 - `HelloWorld <sample/HelloWorld/README.md>`_
```

### Comparing `opentok-3.5.0/README.rst` & `opentok-3.6.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,23 @@
   `OpenTok Media Router <https://tokbox.com/developer/guides/create-session/#media-mode>`_
   or attempt to send streams directly between clients. A routed session is required for some
   OpenTok features (such as archiving).
 
 * ``archive_mode`` which specifies whether the session will be automatically archived (``always``)
   or not (``manual``).
 
+* ``archive_name`` which indicates the archive name for all the archives in auto archived session. 
+  A session that begins with archive mode 'always' will be using this archive name for all archives of that session.
+  Passing 'archive_name' with archive mode 'manual' will cause an error response.
+
+* ``archive_resolution`` which indicates the archive resolution for all the archives in auto archived session.
+  Valid values are '640x480', '480x640', '1280x720', '720x1280', '1920x1080' and '1080x1920'.
+  A session that begins with archive mode 'always' will be using this resolution for all archives of that session.
+  Passing 'archive_resolution' with archive mode 'manual' will cause an error response.
+
 * ``e2ee`` which is a boolean. This specifies whether to enable
   `end-to-end encryption <https://tokbox.com/developer/guides/end-to-end-encryption/>`_
   for the OpenTok session.
 
 This method returns a ``Session`` object. Its ``session_id`` attribute is useful when saving to a persistent
 store (such as a database).
 
@@ -78,14 +87,22 @@
   from opentok import MediaModes
   # A session that uses the OpenTok Media Router, which is required for archiving:
   session = opentok.create_session(media_mode=MediaModes.routed)
 
   # An automatically archived session:
   session = opentok.create_session(media_mode=MediaModes.routed, archive_mode=ArchiveModes.always)
 
+  # An automatically archived session with the archive name and resolution specified:
+  session = opentok.create_session(
+    media_mode=MediaModes.routed,
+    archive_mode=ArchiveModes.always,
+    archive_name='my_archive',
+    archive_resolution='1920x1080'
+  )
+
   # A session with a location hint
   session = opentok.create_session(location=u'12.34.56.78')
 
   # Store this session ID in the database
   session_id = session.session_id
 
 Generating Tokens
@@ -417,14 +434,16 @@
   session_id = 'SESSIONID'
   options = {
     'layout': {
       'type': 'custom',
       'stylesheet': 'the layout stylesheet (only used with type == custom)'
     },
     'maxDuration': 5400,
+    'hasAudio': True
+    'hasVideo': True
     'outputs': {
       'hls': {},
       'rtmp': [{
         'id': 'foo',
         'serverUrl': 'rtmp://myfooserver/myfooapp',
         'streamName': 'myfoostream'
       }, {
@@ -473,14 +492,45 @@
   }
 
   broadcast = opentok.start_broadcast(session_id, options)
   
 To enable multiple simultaneous broadcasts on the same session, specify a unique value for the 
 ``multiBroadcastTag`` parameter in ``options`` when calling the ``opentok.start_broadcast`` method.
 
+You can broadcast only audio, or only video, for a stream by setting ``hasAudio`` or ``hasVideo``
+to ``False`` as required. These fields are ``True`` by default.
+
+.. code:: python
+
+  session_id = 'SESSIONID'
+  options = {
+    'layout': {
+      'type': 'custom',
+      'stylesheet': 'the layout stylesheet (only used with type == custom)'
+    },
+    'maxDuration': 5400,
+    'hasAudio': True
+    'hasVideo': False
+    'outputs': {
+      'hls': {},
+      'rtmp': [{
+        'id': 'foo',
+        'serverUrl': 'rtmp://myfooserver/myfooapp',
+        'streamName': 'myfoostream'
+      }, {
+        'id': 'bar',
+        'serverUrl': 'rtmp://mybarserver/mybarapp',
+        'streamName': 'mybarstream'
+      }]
+    },
+    'resolution': '640x480'
+  }
+
+  broadcast = opentok.start_broadcast(session_id, options)
+
 You can stop a started Broadcast using the ``opentok.stop_broadcast(broadcast_id)`` method.
 
 .. code:: python
 
   # getting the ID from a broadcast object
   broadcast_id = broadcast.id
 
@@ -636,14 +686,23 @@
   
   digits = '12345'
   opentok.play_dtmf(session_id, digits)
 
   # To a specific connection
   opentok.play_dtmf(session_id, connection_id, digits)
 
+Appending to the User Agent
+---------------------------
+
+You can append a string to the user agent that is sent with requests:
+
+.. code:: python
+
+  opentok.append_to_user_agent('my-appended-string')
+
 Samples
 -------
 
 There are two sample applications included in this repository. To get going as fast as possible, clone the whole
 repository and follow the Walkthroughs:
 
 - `HelloWorld <sample/HelloWorld/README.md>`_
```

### Comparing `opentok-3.5.0/opentok/__init__.py` & `opentok-3.6.0/opentok/__init__.py`

 * *Files identical despite different names*

### Comparing `opentok-3.5.0/opentok/archives.py` & `opentok-3.6.0/opentok/archives.py`

 * *Files identical despite different names*

### Comparing `opentok-3.5.0/opentok/broadcast.py` & `opentok-3.6.0/opentok/broadcast.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
     :ivar resolution:
         The resolution of the broadcast (either "640x480", "1280x720", "1920x1080", "480x640", "720x1280", or "1920x1080").
         
     :ivar status:
         The status of the broadcast.
 
+    :ivar hasAudio:
+        Whether the broadcast has audio.
+
+    :ivar hasVideo:
+        Whether the broadcast has video.
+
     :ivar broadcastUrls:
         An object containing details about the HLS and RTMP broadcasts.
         
         If you specified an HLS endpoint, the object includes an hls property, which is set to the URL for the HLS broadcast. 
         Note this HLS broadcast URL points to an index file, an .M3U8-formatted playlist that contains a list of URLs 
         to .ts media segment files (MPEG-2 transport stream files).
         While the URLs of both the playlist index file and media segment files are provided as soon as the HTTP response
@@ -59,23 +65,25 @@
 
     def __init__(self, kwargs):
         self.id = kwargs.get("id")
         self.sessionId = kwargs.get("sessionId")
         self.projectId = kwargs.get("projectId")
         self.createdAt = kwargs.get("createdAt")
         self.updatedAt = kwargs.get("updatedAt")
+        self.hasAudio = kwargs.get("hasAudio")
+        self.hasVideo = kwargs.get("hasVideo")
         self.resolution = kwargs.get("resolution")
         self.status = kwargs.get("status")
         self.broadcastUrls = kwargs.get("broadcastUrls")
         self.stream_mode = kwargs.get("streamMode", BroadcastStreamModes.auto)
         self.streams = kwargs.get("streams")
 
     def json(self):
         """
-        Returns a JSON representation of the broadcast
+        Returns a JSON representation of the broadcast.
         """
         return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
 
 class BroadcastStreamModes(Enum):
     """"List of valid settings for the stream_mode parameter of the OpenTok.start_broadcast()
     method."""
```

### Comparing `opentok-3.5.0/opentok/endpoints.py` & `opentok-3.6.0/opentok/endpoints.py`

 * *Files identical despite different names*

### Comparing `opentok-3.5.0/opentok/exceptions.py` & `opentok-3.6.0/opentok/exceptions.py`

 * *Files identical despite different names*

### Comparing `opentok-3.5.0/opentok/opentok.py` & `opentok-3.6.0/opentok/opentok.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime  # generate_token
-from typing import List, Optional # imports List, Optional type hint
+from typing import List, Optional  # imports List, Optional type hint
 import calendar  # generate_token
 import base64  # generate_token
 import random  # generate_token
 import time  # generate_token
 import hmac  # _sign_string
 import hashlib
 from typing import List  # use for type hinting
@@ -46,15 +46,15 @@
     GetStreamError,
     ForceDisconnectError,
     SipDialError,
     SetStreamClassError,
     BroadcastError,
     DTMFError,
     InvalidWebSocketOptionsError,
-    InvalidMediaModeError  
+    InvalidMediaModeError,
 )
 
 
 class Roles(Enum):
     """List of valid roles for a token."""
 
     subscriber = u("subscriber")
@@ -86,16 +86,26 @@
 
     manual = u("manual")
     """The session will be manually archived."""
     always = u("always")
     """The session will be automatically archived."""
 
 
+valid_archive_resolutions = {
+    "640x480",
+    "480x640",
+    "1280x720",
+    "720x1280",
+    "1920x1080",
+    "1080x1920",
+}
+
 logger = logging.getLogger("opentok")
 
+
 class Client(object):
 
     """Use this SDK to create tokens and interface with the server-side portion
     of the Opentok API.
     """
 
     TOKEN_SENTINEL = "T1=="
@@ -111,14 +121,17 @@
     ):
         self.api_key = str(api_key)
         self.api_secret = api_secret
         self.timeout = timeout
         self._proxies = None
         self.endpoints = Endpoints(api_url, self.api_key)
         self._app_version = __version__ if app_version == None else app_version
+        self._user_agent = (
+            f"OpenTok-Python-SDK/{self.app_version} python/{platform.python_version()}"
+        )
         # JWT custom claims - Default values
         self._jwt_livetime = 3  # In minutes
 
     @property
     def proxies(self):
         return self._proxies
 
@@ -131,14 +144,21 @@
         return self._app_version
 
     @app_version.setter
     def app_version(self, value):
         self._app_version = value
 
     @property
+    def user_agent(self):
+        return self._user_agent
+
+    def append_to_user_agent(self, value):
+        self._user_agent = self._user_agent + value
+
+    @property
     def jwt_livetime(self):
         return self._jwt_livetime
 
     @jwt_livetime.setter
     def jwt_livetime(self, minutes):
         self._jwt_livetime = minutes
 
@@ -297,14 +317,16 @@
         return token
 
     def create_session(
         self,
         location=None,
         media_mode=MediaModes.relayed,
         archive_mode=ArchiveModes.manual,
+        archive_name=None,
+        archive_resolution=None,
         e2ee=False,
     ):
         """
         Creates a new OpenTok session and returns the session ID, which uniquely identifies
         the session.
 
         For example, when using the OpenTok JavaScript library, use the session ID when calling the
@@ -352,14 +374,24 @@
         :param String archive_mode: Whether the session is automatically archived
             (ArchiveModes.always) or not (ArchiveModes.manual). By default,
             the setting is ArchiveModes.manual, and you must call the
             start_archive() method of the OpenTok object to start archiving. To archive the session
             (either automatically or not), you must set the media_mode parameter to
             MediaModes.routed.
 
+        :param String archive_name: Indicates the archive name for all the archives in auto archived session.
+            A session that begins with archive mode 'always' will be using this archive name for all archives of that session.
+            Passing 'archive_name' with archive mode 'manual' will cause an error response.
+
+        :param String archive_resolution:
+            Indicates the archive resolution for all the archives in auto archived session.
+            Valid values are '640x480', '480x640', '1280x720', '720x1280', '1920x1080' and '1080x1920'.
+            A session that begins with archive mode 'always' will be using this resolution for all archives of that session.
+            Passing 'archive_resolution' with archive mode 'manual' will cause an error response.
+
         :param String location: An IP address that the OpenTok servers will use to
             situate the session in its global network. If you do not set a location hint,
             the OpenTok servers will be based on the first client connecting to the session.
 
          :param Boolean e2ee: Whether to enable end-to-end encryption for a routed session
              (see https://tokbox.com/developer/guides/end-to-end-encryption/).
 
@@ -382,16 +414,42 @@
             )
         if archive_mode == ArchiveModes.always and media_mode != MediaModes.routed:
             raise OpenTokException(
                 u(
                     "A session with always archive mode must also have the routed media mode."
                 )
             )
+
+        if archive_name is not None:
+            if archive_mode == ArchiveModes.manual:
+                raise OpenTokException(
+                    "You cannot specify a value for archive_name with archive mode: manual."
+                )
+            if not 1 <= len(archive_name) <= 80:
+                raise OpenTokException(
+                    "archive_name must be between 1 and 80 characters in length."
+                )
+
+        if archive_resolution is not None:
+            if archive_mode == ArchiveModes.manual:
+                raise OpenTokException(
+                    "You cannot specify a value for archive_resolution with archive mode: manual."
+                )
+            if archive_resolution not in valid_archive_resolutions:
+                raise OpenTokException(
+                    f"archive_resolution must be one of the allowed values: {valid_archive_resolutions}."
+                )
+
         options[u("p2p.preference")] = media_mode.value
         options[u("archiveMode")] = archive_mode.value
+        if archive_name is not None:
+            options[("archiveName")] = archive_name
+        if archive_resolution is not None:
+            options[("archiveResolution")] = archive_resolution
+
         if location:
             # validate IP address
             try:
                 inet_aton(location)
             except:
                 raise OpenTokException(
                     u(
@@ -437,15 +495,15 @@
                         error.attributes["code"].value,
                         error.firstChild.attributes["message"].value,
                     )
                 )
 
             session_id = (
                 dom.getElementsByTagName("session_id")[0].childNodes[0].nodeValue
-            )            
+            )
             return Session(
                 self,
                 session_id,
                 location=location,
                 media_mode=media_mode,
                 archive_mode=archive_mode,
                 e2ee=e2ee,
@@ -491,15 +549,15 @@
         has_audio=True,
         has_video=True,
         name=None,
         output_mode=OutputModes.composed,
         stream_mode=StreamModes.auto,
         resolution=None,
         layout=None,
-        multi_archive_tag=None
+        multi_archive_tag=None,
     ):
         """
         Starts archiving an OpenTok session.
 
         Clients must be actively connected to the OpenTok session for you to successfully start
         recording an archive.
 
@@ -542,21 +600,21 @@
             set 'type' to 'bestFit'
 
         :param StreamModes stream_mode (Optional): Determines the archive stream handling mode.
         Set this to StreamModes.auto (the default) to have streams added automatically. Set this to
         StreamModes.manual to explicitly select streams to include in the the archive, using the
         OpenTok.add_archive_stream() and OpenTok.remove_archive_stream() methods.
 
-        :param String multi_archive_tag (Optional): Set this to support recording multiple archives for the same 
-        session simultaneously. Set this to a unique string for each simultaneous archive of an ongoing session. 
-        You must also set this option when manually starting an archive that is automatically archived. 
-        Note that the multiArchiveTag value is not included in the response for the methods to list archives and 
-        retrieve archive information. If you do not specify a unique multi_archive_tag, you can only record one archive 
-        at a time for a given session. 
-        For more information, see simultaneous archives: https://tokbox.com/developer/guides/archiving/#simultaneous-archives. 
+        :param String multi_archive_tag (Optional): Set this to support recording multiple archives for the same
+        session simultaneously. Set this to a unique string for each simultaneous archive of an ongoing session.
+        You must also set this option when manually starting an archive that is automatically archived.
+        Note that the multiArchiveTag value is not included in the response for the methods to list archives and
+        retrieve archive information. If you do not specify a unique multi_archive_tag, you can only record one archive
+        at a time for a given session.
+        For more information, see simultaneous archives: https://tokbox.com/developer/guides/archiving/#simultaneous-archives.
 
         :rtype: The Archive object, which includes properties defining the archive,
           including the archive ID.
         """
         if not isinstance(output_mode, OutputModes):
             raise OpenTokException(
                 u("Cannot start archive, {0} is not a valid output mode").format(
@@ -575,25 +633,25 @@
             "name": name,
             "sessionId": session_id,
             "hasAudio": has_audio,
             "hasVideo": has_video,
             "outputMode": output_mode.value,
             "resolution": resolution,
             "streamMode": stream_mode.value,
-            "multiArchiveTag": multi_archive_tag
+            "multiArchiveTag": multi_archive_tag,
         }
 
         if layout is not None:
-            payload['layout'] = layout
+            payload["layout"] = layout
 
         logger.debug(
             "POST to %r with params %r, headers %r, proxies %r",
             self.endpoints.archive_url(),
             json.dumps(payload),
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.post(
             self.endpoints.get_archive_url(),
             data=json.dumps(payload),
             headers=self.get_json_headers(),
@@ -631,15 +689,15 @@
         @param [String] archive_id The archive ID of the archive you want to stop recording.
 
         :rtype: The Archive object corresponding to the archive being stopped.
         """
         logger.debug(
             "POST to %r with headers %r, proxies %r",
             self.endpoints.archive_url(archive_id) + "/stop",
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.post(
             self.endpoints.get_archive_url(archive_id) + "/stop",
             headers=self.get_json_headers(),
             proxies=self.proxies,
@@ -666,15 +724,15 @@
         removes the archive file, making it unavailable for download.
 
         :param String archive_id: The archive ID of the archive to be deleted.
         """
         logger.debug(
             "DELETE to %r with headers %r, proxies %r",
             self.endpoints.archive_url(archive_id),
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.delete(
             self.endpoints.get_archive_url(archive_id),
             headers=self.get_json_headers(),
             proxies=self.proxies,
@@ -696,15 +754,15 @@
         :param String archive_id: The archive ID.
 
         :rtype: The Archive object.
         """
         logger.debug(
             "GET to %r with headers %r, proxies %r",
             self.endpoints.archive_url(archive_id),
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.get(
             self.endpoints.get_archive_url(archive_id),
             headers=self.get_json_headers(),
             proxies=self.proxies,
@@ -742,15 +800,15 @@
             params["sessionId"] = session_id
 
         endpoint = self.endpoints.get_archive_url() + "?" + urlencode(params)
 
         logger.debug(
             "GET to %r with headers %r, proxies %r",
             endpoint,
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.get(
             endpoint,
             headers=self.get_json_headers(),
             proxies=self.proxies,
@@ -774,17 +832,16 @@
         return self.get_archives(offset, count, session_id)
 
     def add_archive_stream(
         self,
         archive_id: str,
         stream_id: str,
         has_audio: bool = True,
-        has_video: bool = True
-        ) -> requests.Response:
-
+        has_video: bool = True,
+    ) -> requests.Response:
         """
         This method will add streams to the archive with addStream for new participant(choosing audio, video or both).
 
         :param String archive_id: the ID of the archive that will be updated
         :param String stream_id: the id of the stream that will get added to the archive
         :param Boolean has_audio: if set to True, an audio track will be inserted to the archive.
           has_audio is an optional parameter that is set to True by default. If you set both
@@ -792,19 +849,15 @@
           an error.
         :param Boolean has_video: if set to True, a video track will be inserted to the archive.
           has_video is an optional parameter that is set to True by default.
         """
 
         endpoint = self.endpoints.get_archive_stream(archive_id)
 
-        streams = {
-            "hasAudio": has_audio,
-            "hasVideo": has_video,
-            "addStream": stream_id
-        }
+        streams = {"hasAudio": has_audio, "hasVideo": has_video, "addStream": stream_id}
 
         response = requests.patch(
             endpoint,
             data=json.dumps(streams),
             headers=self.get_json_headers(),
             proxies=self.proxies,
             timeout=self.timeout,
@@ -822,33 +875,35 @@
             You specify an invalid resolution value.
             The outputMode property is set to "individual" and you set the resolution property and (which is not supported in individual stream archives).
             """
             raise RequestError(response.json().get("message"))
         elif response.status_code == 404:
             raise NotFoundError("Archive or Stream not found")
         elif response.status_code == 405:
-            raise ArchiveStreamModeError("Your archive is configured with a streamMode that does not support stream manipulation.")
+            raise ArchiveStreamModeError(
+                "Your archive is configured with a streamMode that does not support stream manipulation."
+            )
         elif response.status_code == 409:
             raise ArchiveError(response.json().get("message"))
         else:
             raise RequestError("An unexpected error occurred", response.status_code)
 
-    def remove_archive_stream(self, archive_id: str, stream_id: str) -> requests.Response:
+    def remove_archive_stream(
+        self, archive_id: str, stream_id: str
+    ) -> requests.Response:
         """
         This method will remove streams from the archive with removeStream.
 
         :param String archive_id: the ID of the archive that will be updated
         :param String stream_id: the ID of the stream that will get added to the archive
         """
 
         endpoint = self.endpoints.get_archive_stream(archive_id)
 
-        streams = {
-            "removeStream": stream_id
-        }
+        streams = {"removeStream": stream_id}
 
         response = requests.patch(
             endpoint,
             data=json.dumps(streams),
             headers=self.get_json_headers(),
             proxies=self.proxies,
             timeout=self.timeout,
@@ -866,22 +921,22 @@
             You specify an invalid resolution value.
             The outputMode property is set to "individual" and you set the resolution property and (which is not supported in individual stream archives).
             """
             raise RequestError(response.json().get("message"))
         elif response.status_code == 404:
             raise NotFoundError("Archive or Stream not found")
         elif response.status_code == 405:
-            raise ArchiveStreamModeError("Your archive is configured with a streamMode that does not support stream manipulation.")
+            raise ArchiveStreamModeError(
+                "Your archive is configured with a streamMode that does not support stream manipulation."
+            )
         elif response.status_code == 409:
             raise ArchiveError(response.json().get("message"))
         else:
             raise RequestError("An unexpected error occurred", response.status_code)
 
-
-
     def send_signal(self, session_id, payload, connection_id=None):
         """
         Send signals to all participants in an active OpenTok session or to a specific client
         connected to that session.
 
         :param String session_id: The session ID of the OpenTok session that receives the signal
 
@@ -893,15 +948,15 @@
         the signal is sent to the specified client. Otherwise, the signal is sent to all clients
         connected to the session
         """
         logger.debug(
             "POST to %r with params %r, headers %r, proxies %r",
             self.endpoints.signaling_url(session_id, connection_id),
             json.dumps(payload),
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.post(
             self.endpoints.get_signaling_url(session_id, connection_id),
             data=json.dumps(payload),
             headers=self.get_json_headers(),
@@ -948,15 +1003,15 @@
         -layoutClassList: It's an array of the layout classes for the stream
         """
         endpoint = self.endpoints.get_stream_url(session_id, stream_id)
 
         logger.debug(
             "GET to %r with headers %r, proxies %r",
             endpoint,
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.get(
             endpoint,
             headers=self.get_json_headers(),
             proxies=self.proxies,
@@ -985,15 +1040,15 @@
         -items: List of the Stream objects
         """
         endpoint = self.endpoints.get_stream_url(session_id)
 
         logger.debug(
             "GET to %r with headers %r, proxies %r",
             endpoint,
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.get(
             endpoint,
             headers=self.get_json_headers(),
             proxies=self.proxies,
@@ -1023,15 +1078,15 @@
         :param String connection_id: The connection ID of the client that will be disconnected
         """
         endpoint = self.endpoints.force_disconnect_url(session_id, connection_id)
 
         logger.debug(
             "DELETE to %r with headers %r, proxies %r",
             endpoint,
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.delete(
             endpoint,
             headers=self.get_json_headers(),
             proxies=self.proxies,
@@ -1051,15 +1106,17 @@
         elif response.status_code == 404:
             raise ForceDisconnectError(
                 "The client specified by the connectionId property is not connected to the session."
             )
         else:
             raise RequestError("An unexpected error occurred", response.status_code)
 
-    def set_archive_layout(self, archive_id, layout_type, stylesheet=None, screenshare_type=None):
+    def set_archive_layout(
+        self, archive_id, layout_type, stylesheet=None, screenshare_type=None
+    ):
         """
         Use this method to change the layout of videos in an OpenTok archive
 
         :param String archive_id: The ID of the archive that will be updated
 
         :param String layout_type: The layout type for the archive. Valid values are:
         'bestFit', 'custom', 'horizontalPresentation', 'pip' and 'verticalPresentation'
@@ -1083,15 +1140,15 @@
 
         endpoint = self.endpoints.set_archive_layout_url(archive_id)
 
         logger.debug(
             "PUT to %r with params %r, headers %r, proxies %r",
             endpoint,
             json.dumps(payload),
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.put(
             endpoint,
             data=json.dumps(payload),
             headers=self.get_json_headers(),
@@ -1212,15 +1269,15 @@
 
         endpoint = self.endpoints.dial_url()
 
         logger.debug(
             "POST to %r with params %r, headers %r, proxies %r",
             endpoint,
             json.dumps(payload),
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.post(
             endpoint,
             data=json.dumps(payload),
             headers=self.get_json_headers(),
@@ -1266,15 +1323,15 @@
 
         endpoint = self.endpoints.set_stream_class_lists_url(session_id)
 
         logger.debug(
             "PUT to %r with params %r, headers %r, proxies %r",
             endpoint,
             json.dumps(items_payload),
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.put(
             endpoint,
             data=json.dumps(items_payload),
             headers=self.get_json_headers(),
@@ -1290,25 +1347,31 @@
                 "is invalid JSON. It may also indicate that you passed in invalid layout options."
             )
         elif response.status_code == 403:
             raise AuthError("Authentication error.")
         else:
             raise RequestError("OpenTok server error.", response.status_code)
 
-    def start_broadcast(self, session_id, options, stream_mode=BroadcastStreamModes.auto):
+    def start_broadcast(
+        self, session_id, options, stream_mode=BroadcastStreamModes.auto
+    ):
         """
         Use this method to start a live streaming broadcast for an OpenTok session. This broadcasts
         the session to an HLS (HTTP live streaming) or to RTMP streams. To successfully start
         broadcasting a session, at least one client must be connected to the session. You can only
         start live streaming for sessions that use the OpenTok Media Router (with the media mode set
         to routed); you cannot use live streaming with sessions that have the media mode set to
         relayed
 
         :param String session_id: The session ID of the OpenTok session you want to broadcast
 
+        :param Boolean optional hasAudio: Whether the stream is broadcast with audio.
+
+        :param Boolean optional hasVideo: Whether the stream is broadcast with video.
+
         :param Dictionary options, with the following properties:
 
             Dictionary 'layout' optional: Specify this to assign the initial layout type for the
             broadcast.
 
                 String 'type': Type of layout. Valid values for the layout property are "bestFit" (best fit),
                 "custom" (custom), "horizontalPresentation" (horizontal presentation), "pip" (picture-in-picture),
@@ -1350,50 +1413,53 @@
                         'streamName': 'mybarstream'
                     }]
                 }
 
             String 'resolution' optional: The resolution of the broadcast, either "640x480"
             (SD, the default) or "1280x720" (HD)
 
-            String 'multiBroadcastTag' optional: Set this to support multiple broadcasts for the same session simultaneously. 
-            Set this to a unique string for each simultaneous broadcast of an ongoing session. 
-            Note that the multiBroadcastTag value is not included in the response for the methods to list live streaming 
-            broadcasts and get information about a live streaming broadcast. 
-            For more information, see https://tokbox.com/developer/guides/broadcast/live-streaming#simultaneous-broadcasts. 
+            String 'multiBroadcastTag' optional: Set this to support multiple broadcasts for the same session simultaneously.
+            Set this to a unique string for each simultaneous broadcast of an ongoing session.
+            Note that the multiBroadcastTag value is not included in the response for the methods to list live streaming
+            broadcasts and get information about a live streaming broadcast.
+            For more information, see https://tokbox.com/developer/guides/broadcast/live-streaming#simultaneous-broadcasts.
 
         :param BroadcastStreamModes stream_mode (Optional): Determines the broadcast stream handling mode.
         Set this to BroadcastStreamModes.auto (the default) to have streams added automatically. Set this to
         BroadcastStreamModes.manual to explicitly select streams to include in the the broadcast, using the
         OpenTok.add_broadcast_stream() and OpenTok.remove_broadcast_stream() methods.
 
-        :rtype A Broadcast object, which contains information of the broadcast: id, sessionId
+        :rtype A Broadcast object, which contains information of the broadcast: id, sessionId,
         projectId, createdAt, updatedAt, resolution, status and broadcastUrls
         """
 
-        if 'hls' in options['outputs']:
-            if 'lowLatency' in options['outputs']['hls'] and 'dvr' in options['outputs']['hls']:
-                if options['outputs']['hls']['lowLatency'] == True and options['outputs']['hls']['dvr'] == True:
+        if "hls" in options["outputs"]:
+            if (
+                "lowLatency" in options["outputs"]["hls"]
+                and "dvr" in options["outputs"]["hls"]
+            ):
+                if (
+                    options["outputs"]["hls"]["lowLatency"] == True
+                    and options["outputs"]["hls"]["dvr"] == True
+                ):
                     raise BroadcastHLSOptionsError(
                         'HLS options "lowLatency" and "dvr" cannot both be set to "True".'
-                        )
+                    )
 
-        payload = {
-                    "sessionId": session_id,
-                    "streamMode": stream_mode.value
-                  }
+        payload = {"sessionId": session_id, "streamMode": stream_mode.value}
 
         payload.update(options)
 
         endpoint = self.endpoints.broadcast_url()
 
         logger.debug(
             "POST to %r with params %r, headers %r, proxies %r",
             endpoint,
             json.dumps(payload),
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.post(
             endpoint,
             data=json.dumps(payload),
             headers=self.get_json_headers(),
@@ -1428,15 +1494,15 @@
         """
 
         endpoint = self.endpoints.broadcast_url(broadcast_id, stop=True)
 
         logger.debug(
             "POST to %r with headers %r, proxies %r",
             endpoint,
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.post(
             endpoint,
             headers=self.get_json_headers(),
             proxies=self.proxies,
@@ -1461,17 +1527,16 @@
             raise RequestError("OpenTok server error.", response.status_code)
 
     def add_broadcast_stream(
         self,
         broadcast_id: str,
         stream_id: str,
         has_audio: bool = True,
-        has_video: bool = True
-        ) -> requests.Response:
-
+        has_video: bool = True,
+    ) -> requests.Response:
         """
         This method will add streams to the broadcast with addStream for new participant(choosing audio, video or both).
 
         :param String broadcast_id: the ID of the broadcast that will be updated
         :param String stream_id: the id of the stream that will get added to the broadcast
         :param Boolean has_audio: if set to True, an audio track will be inserted to the broadcast.
           has_audio is an optional parameter that is set to True by default. If you set both
@@ -1479,19 +1544,15 @@
           an error.
         :param Boolean has_video: if set to True, a video track will be inserted to the broadcast.
           has_video is an optional parameter that is set to True by default.
         """
 
         endpoint = self.endpoints.get_broadcast_stream(broadcast_id)
 
-        streams = {
-            "hasAudio": has_audio,
-            "hasVideo": has_video,
-            "addStream": stream_id
-        }
+        streams = {"hasAudio": has_audio, "hasVideo": has_video, "addStream": stream_id}
 
         response = requests.patch(
             endpoint,
             data=json.dumps(streams),
             headers=self.get_json_headers(),
             proxies=self.proxies,
             timeout=self.timeout,
@@ -1505,34 +1566,35 @@
                 "invalid JSON. It may also indicate that you passed in invalid layout options. "
                 "Or you have exceeded the limit of five simultaneous RTMP streams for an OpenTok "
                 "session. Or you specified and invalid resolution."
             )
         elif response.status_code == 403:
             raise AuthError("Authentication error.")
         elif response.status_code == 405:
-            raise BroadcastStreamModeError("Your broadcast is configured with a streamMode that does not support stream manipulation.")
+            raise BroadcastStreamModeError(
+                "Your broadcast is configured with a streamMode that does not support stream manipulation."
+            )
         elif response.status_code == 409:
             raise BroadcastError("The broadcast has already started for the session.")
         else:
             raise RequestError("OpenTok server error.", response.status_code)
 
-
-    def remove_broadcast_stream(self, broadcast_id: str, stream_id: str) -> requests.Response:
+    def remove_broadcast_stream(
+        self, broadcast_id: str, stream_id: str
+    ) -> requests.Response:
         """
         This method will remove streams from the broadcast with removeStream.
 
         :param String broadcast_id: the ID of the broadcast that will be updated
         :param String stream_id: the id of the stream that will get added to the broadcast
         """
 
         endpoint = self.endpoints.get_broadcast_stream(broadcast_id)
 
-        streams = {
-            "removeStream": stream_id
-        }
+        streams = {"removeStream": stream_id}
 
         response = requests.patch(
             endpoint,
             data=json.dumps(streams),
             headers=self.get_json_headers(),
             proxies=self.proxies,
             timeout=self.timeout,
@@ -1546,21 +1608,22 @@
                 "invalid JSON. It may also indicate that you passed in invalid layout options. "
                 "Or you have exceeded the limit of five simultaneous RTMP streams for an OpenTok "
                 "session. Or you specified and invalid resolution."
             )
         elif response.status_code == 403:
             raise AuthError("Authentication error.")
         elif response.status_code == 405:
-            raise BroadcastStreamModeError("Your broadcast is configured with a streamMode that does not support stream manipulation.")
+            raise BroadcastStreamModeError(
+                "Your broadcast is configured with a streamMode that does not support stream manipulation."
+            )
         elif response.status_code == 409:
             raise BroadcastError("The broadcast has already started for the session.")
         else:
             raise RequestError("OpenTok server error.", response.status_code)
 
-
     def get_broadcast(self, broadcast_id):
         """
         Use this method to get details on a broadcast that is in-progress.
 
         :param String broadcast_id: The ID of the broadcast you want to stop
 
         :rtype A Broadcast object, which contains information of the broadcast: id, sessionId
@@ -1568,15 +1631,15 @@
         """
 
         endpoint = self.endpoints.broadcast_url(broadcast_id)
 
         logger.debug(
             "GET to %r with headers %r, proxies %r",
             endpoint,
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.get(
             endpoint,
             headers=self.get_json_headers(),
             proxies=self.proxies,
@@ -1593,15 +1656,17 @@
         elif response.status_code == 403:
             raise AuthError("Authentication error.")
         elif response.status_code == 409:
             raise BroadcastError("No matching broadcast found (with the specified ID).")
         else:
             raise RequestError("OpenTok server error.", response.status_code)
 
-    def set_broadcast_layout(self, broadcast_id, layout_type, stylesheet=None, screenshare_type=None):
+    def set_broadcast_layout(
+        self, broadcast_id, layout_type, stylesheet=None, screenshare_type=None
+    ):
         """
         Use this method to change the layout type of a live streaming broadcast
 
         :param String broadcast_id: The ID of the broadcast that will be updated
 
         :param String layout_type: The layout type for the broadcast. Valid values are:
         'bestFit', 'custom', 'horizontalPresentation', 'pip' and 'verticalPresentation'
@@ -1625,15 +1690,15 @@
 
         endpoint = self.endpoints.broadcast_url(broadcast_id, layout=True)
 
         logger.debug(
             "PUT to %r with params %r, headers %r, proxies %r",
             endpoint,
             json.dumps(payload),
-            self.json_headers(),
+            self.get_json_headers(),
             self.proxies,
         )
 
         response = requests.put(
             endpoint,
             data=json.dumps(payload),
             headers=self.get_json_headers(),
@@ -1649,35 +1714,44 @@
                 "invalid JSON. It may also indicate that you passed in invalid layout options."
             )
         elif response.status_code == 403:
             raise AuthError("Authentication error.")
         else:
             raise RequestError("OpenTok server error.", response.status_code)
 
-    def start_render(self, session_id, opentok_token, url, max_duration=7200, resolution="1280x720", status_callback_url=None, properties: dict = None):
+    def start_render(
+        self,
+        session_id,
+        opentok_token,
+        url,
+        max_duration=7200,
+        resolution="1280x720",
+        status_callback_url=None,
+        properties: dict = None,
+    ):
         """
-        Starts an Experience Composer for the specified OpenTok session.
-        For more information, see the
-       `Experience Composer developer guide <https://tokbox.com/developer/guides/experience-composer>`_.
-
-        :param String 'session_id': The session ID of the OpenTok session that will include the Experience Composer stream.
-        :param String 'opentok_token': A valid OpenTok token with a Publisher role and (optionally) connection data to be associated with the output stream.
-        :param String 'url': A publically reachable URL controlled by the customer and capable of generating the content to be rendered without user intervention.
-        :param Integer 'maxDuration' Optional: The maximum time allowed for the Experience Composer, in seconds. After this time, it is stopped automatically, if it is still running. The maximum value is 36000 (10 hours), the minimum value is 60 (1 minute), and the default value is 7200 (2 hours). When the Experience Composer ends, its stream is unpublished and an event is posted to the callback URL, if configured in the Account Portal.
-        :param String 'resolution' Optional: The resolution of the Experience Composer, either "640x480" (SD landscape), "480x640" (SD portrait), "1280x720" (HD landscape), "720x1280" (HD portrait), "1920x1080" (FHD landscape), or "1080x1920" (FHD portrait). By default, this resolution is "1280x720" (HD landscape, the default).
-        :param Dictionary 'properties' Optional: Initial configuration of Publisher properties for the composed output stream.
-            String name Optional: The name of the composed output stream which will be published to the session. The name must have a minimum length of 1 and a maximum length of 200.
+         Starts an Experience Composer for the specified OpenTok session.
+         For more information, see the
+        `Experience Composer developer guide <https://tokbox.com/developer/guides/experience-composer>`_.
+
+         :param String 'session_id': The session ID of the OpenTok session that will include the Experience Composer stream.
+         :param String 'opentok_token': A valid OpenTok token with a Publisher role and (optionally) connection data to be associated with the output stream.
+         :param String 'url': A publically reachable URL controlled by the customer and capable of generating the content to be rendered without user intervention.
+         :param Integer 'maxDuration' Optional: The maximum time allowed for the Experience Composer, in seconds. After this time, it is stopped automatically, if it is still running. The maximum value is 36000 (10 hours), the minimum value is 60 (1 minute), and the default value is 7200 (2 hours). When the Experience Composer ends, its stream is unpublished and an event is posted to the callback URL, if configured in the Account Portal.
+         :param String 'resolution' Optional: The resolution of the Experience Composer, either "640x480" (SD landscape), "480x640" (SD portrait), "1280x720" (HD landscape), "720x1280" (HD portrait), "1920x1080" (FHD landscape), or "1080x1920" (FHD portrait). By default, this resolution is "1280x720" (HD landscape, the default).
+         :param Dictionary 'properties' Optional: Initial configuration of Publisher properties for the composed output stream.
+             String name Optional: The name of the composed output stream which will be published to the session. The name must have a minimum length of 1 and a maximum length of 200.
         """
         payload = {
             "sessionId": session_id,
             "token": opentok_token,
             "url": url,
             "maxDuration": max_duration,
             "resolution": resolution,
-            "properties": properties
+            "properties": properties,
         }
 
         logger.debug(
             "POST to %r with params %r, headers %r, proxies %r",
             self.endpoints.get_render_url(),
             json.dumps(payload),
             self.get_json_headers(),
@@ -1707,15 +1781,15 @@
             raise RequestError("An unexpected error occurred", response.status_code)
 
     def get_render(self, render_id):
         """
         This method allows you to see the status of a render, which can be one of the following:
             ['starting', 'started', 'stopped', 'failed']
 
-        :param String 'render_id': The ID of a specific render. 
+        :param String 'render_id': The ID of a specific render.
         """
         logger.debug(
             "GET to %r with headers %r, proxies %r",
             self.endpoints.get_render_url(render_id=render_id),
             self.get_json_headers(),
             self.proxies,
         )
@@ -1740,15 +1814,15 @@
         else:
             raise RequestError("An unexpected error occurred", response.status_code)
 
     def stop_render(self, render_id):
         """
         This method stops a render.
 
-        :param String 'render_id': The ID of a specific render. 
+        :param String 'render_id': The ID of a specific render.
         """
         logger.debug(
             "DELETE to %r with headers %r, proxies %r",
             self.endpoints.get_render_url(render_id=render_id),
             self.get_headers(),
             self.proxies,
         )
@@ -1774,15 +1848,15 @@
             raise RequestError("An unexpected error occurred", response.status_code)
 
     def list_renders(self, offset=0, count=50):
         """
         List existing renders associated with the project's API key.
 
         :param Integer 'offset' Optional: Start offset in the list of existing renders.
-        :param Integer 'count' Optional: Number of renders to retrieve, starting at 'offset'. 
+        :param Integer 'count' Optional: Number of renders to retrieve, starting at 'offset'.
         """
 
         query_params = {"offset": offset, "count": count}
 
         logger.debug(
             "GET to %r with headers %r, params %r, proxies %r",
             self.endpoints.get_render_url(),
@@ -1806,32 +1880,34 @@
                 "Invalid request. This response may indicate that data in your request is invalid JSON. Or it may indicate that you do not pass in a session ID."
             )
         elif response.status_code == 403:
             raise AuthError("You passed in an invalid OpenTok API key or JWT token.")
         else:
             raise RequestError("An unexpected error occurred", response.status_code)
 
-    def connect_audio_to_websocket(self, session_id: str, opentok_token: str, websocket_options: dict):
+    def connect_audio_to_websocket(
+        self, session_id: str, opentok_token: str, websocket_options: dict
+    ):
         """
         Connects audio streams to a specified WebSocket URI.
         For more information, see the `Audio Connector developer guide <https://tokbox.com/developer/guides/audio-streamer/>`.
 
         :param String 'session_id': The OpenTok session ID that includes the OpenTok streams you want to include in the WebSocket stream. The Audio Connector feature is only supported in routed sessions (sessions that use the OpenTok Media Router).
         :param String 'opentok_token': The OpenTok token to be used for the Audio Connector connection to the OpenTok session.
         :param Dictionary 'websocket_options': Included options for the WebSocket.
             String 'uri': A publicly reachable WebSocket URI to be used for the destination of the audio stream (such as "wss://example.com/ws-endpoint").
             List 'streams' Optional: A list of stream IDs for the OpenTok streams you want to include in the WebSocket audio. If you omit this property, all streams in the session will be included.
             Dictionary 'headers' Optional: An object of key-value pairs of headers to be sent to your WebSocket server with each message, with a maximum length of 512 bytes.
         """
         self.validate_websocket_options(websocket_options)
-        
+
         payload = {
             "sessionId": session_id,
             "token": opentok_token,
-            "websocket": websocket_options
+            "websocket": websocket_options,
         }
 
         logger.debug(
             "POST to %r with params %r, headers %r, proxies %r",
             self.endpoints.get_audio_connector_url(),
             json.dumps(payload),
             self.get_json_headers(),
@@ -1854,23 +1930,27 @@
             You did not pass in a session ID or you pass in an invalid session ID.
             You specified an invalid value for input parameters.
             """
             raise RequestError(response.json().get("message"))
         elif response.status_code == 403:
             raise AuthError("You passed in an invalid OpenTok API key or JWT token.")
         elif response.status_code == 409:
-            raise InvalidMediaModeError("Only routed sessions are allowed to initiate Audio Connector WebSocket connections.")
+            raise InvalidMediaModeError(
+                "Only routed sessions are allowed to initiate Audio Connector WebSocket connections."
+            )
         else:
             raise RequestError("An unexpected error occurred", response.status_code)
 
     def validate_websocket_options(self, options):
         if type(options) is not dict:
-            raise InvalidWebSocketOptionsError('Must pass WebSocket options as a dictionary.')
-        if 'uri' not in options:
-            raise InvalidWebSocketOptionsError('Provide a WebSocket URI.')
+            raise InvalidWebSocketOptionsError(
+                "Must pass WebSocket options as a dictionary."
+            )
+        if "uri" not in options:
+            raise InvalidWebSocketOptionsError("Provide a WebSocket URI.")
 
     def _sign_string(self, string, secret):
         return hmac.new(
             secret.encode("utf-8"), string.encode("utf-8"), hashlib.sha1
         ).hexdigest()
 
     def _create_jwt_auth_header(self):
@@ -1880,20 +1960,18 @@
             "iat": int(time.time()),  # current time in unix time (seconds)
             "exp": int(time.time())
             + (60 * self._jwt_livetime),  # 3 minutes in the future (seconds)
             "jti": "{0}".format(0, random.random()),
         }
 
         return jwt.encode(payload, self.api_secret, algorithm="HS256")
-        
-
-    def mute_all(self,
-                session_id: str,
-                excludedStreamIds: Optional[List[str]]) -> requests.Response:
 
+    def mute_all(
+        self, session_id: str, excludedStreamIds: Optional[List[str]]
+    ) -> requests.Response:
         """
         Mutes all streams in an OpenTok session.
 
         You can include an optional list of streams IDs to exclude from being muted.
 
         In addition to existing streams, any streams that are published after the call to
         this method are published with audio muted. You can remove the mute state of a session
@@ -1906,67 +1984,76 @@
         """
 
         options = {}
         url = self.endpoints.get_mute_all_url(session_id)
 
         try:
             if excludedStreamIds:
-                options = {'active': True, 'excludedStreams': excludedStreamIds }
+                options = {"active": True, "excludedStreams": excludedStreamIds}
             else:
-                options = {'active': True, 'excludedStreams': []}
+                options = {"active": True, "excludedStreams": []}
 
-            response = requests.post(url, headers=self.get_headers(), data=json.dumps(options))
+            response = requests.post(
+                url, headers=self.get_headers(), data=json.dumps(options)
+            )
 
             if response:
                 return response
             elif response.status_code == 400:
-                raise GetStreamError("Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID.")
+                raise GetStreamError(
+                    "Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID."
+                )
             elif response.status_code == 403:
                 raise AuthError("Failed to mute, invalid credentials.")
             elif response.status_code == 404:
                 raise NotFoundError("The session or a stream is not found.")
         except Exception as e:
             raise OpenTokException(
-                ("There was an error thrown by the OpenTok SDK, please check that your session_id {0} and excludedStreamIds (if exists) {1} are valid").format(
-                    session_id, excludedStreamIds))
-
+                (
+                    "There was an error thrown by the OpenTok SDK, please check that your session_id {0} and excludedStreamIds (if exists) {1} are valid"
+                ).format(session_id, excludedStreamIds)
+            )
 
     def disable_force_mute(self, session_id: str) -> requests.Response:
         """
         Disables the active mute state of the session. After you call this method, new streams
         published to the session will no longer have audio muted.
 
         After you call the mute_all() method, any streams published after
         the call are published with audio muted. Call the OpenTok.disable_force_mute() method
         to remove the mute state of a session, so that new published streams are not
         automatically muted.
 
         :param session_id The session ID.
         """
 
-        options = {'active': False}
+        options = {"active": False}
         url = self.endpoints.get_mute_all_url(session_id)
 
-        response = requests.post(url, headers=self.get_headers(), data=json.dumps(options))
-
+        response = requests.post(
+            url, headers=self.get_headers(), data=json.dumps(options)
+        )
 
         try:
             if response:
-                    return response
+                return response
             elif response.status_code == 400:
-                raise GetStreamError("Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID.")
+                raise GetStreamError(
+                    "Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID."
+                )
             elif response.status_code == 403:
                 raise AuthError("Failed to mute, invalid credentials.")
             elif response.status_code == 404:
                 raise NotFoundError("The session or a stream is not found.")
         except Exception as e:
             raise OpenTokException(
-                ("There was an error thrown by the OpenTok SDK, please check that your session_id {0} is valid").format(
-                    session_id))
-
+                (
+                    "There was an error thrown by the OpenTok SDK, please check that your session_id {0} is valid"
+                ).format(session_id)
+            )
 
     def mute_stream(self, session_id: str, stream_id: str) -> requests.Response:
         """
         Mutes a single stream in an OpenTok session.
 
         :param session_id The session ID.
 
@@ -1976,28 +2063,33 @@
         try:
             if stream_id:
                 url = self.endpoints.get_stream_url(session_id, stream_id) + "/mute"
 
             response = requests.post(url, headers=self.get_headers())
 
             if response:
-                    return response
+                return response
             elif response.status_code == 400:
-                raise GetStreamError("Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID.")
+                raise GetStreamError(
+                    "Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID."
+                )
             elif response.status_code == 403:
                 raise AuthError("Failed to mute, invalid credentials.")
             elif response.status_code == 404:
                 raise NotFoundError("Mute not found")
         except Exception as e:
             raise OpenTokException(
-                ("There was an error thrown by the OpenTok SDK, please check that your session_id {0} and stream_id {1} are valid").format(
-                    session_id, stream_id))
-
+                (
+                    "There was an error thrown by the OpenTok SDK, please check that your session_id {0} and stream_id {1} are valid"
+                ).format(session_id, stream_id)
+            )
 
-    def play_dtmf(self, session_id: str, connection_id: str, digits: str, options: dict = {}) -> requests.Response:
+    def play_dtmf(
+        self, session_id: str, connection_id: str, digits: str, options: dict = {}
+    ) -> requests.Response:
         """
         Plays a DTMF string into a session or to a specific connection
 
         :param session_id The ID of the OpenTok session that the participant being called
         will join
 
         :param connection_id An optional parameter used to send the DTMF tones to a specific
@@ -2013,27 +2105,39 @@
             if not connection_id:
                 url = self.endpoints.get_dtmf_all_url(session_id)
                 payload = {"digits": digits}
             else:
                 url = self.endpoints.get_dtmf_specific_url(session_id, connection_id)
                 payload = {"digits": digits}
 
-            response = requests.post(url, headers=self.get_json_headers(), data=json.dumps(payload))
+            response = requests.post(
+                url, headers=self.get_json_headers(), data=json.dumps(payload)
+            )
 
             if response.status_code == 200:
                 return response
             elif response.status_code == 400:
-                raise DTMFError("One of the properties digits, sessionId or connectionId is invalid.")
+                raise DTMFError(
+                    "One of the properties digits, sessionId or connectionId is invalid."
+                )
             elif response.status_code == 403:
-                raise AuthError("Failed to create session, invalid credentials. Please check your OpenTok API Key or JSON web token")
+                raise AuthError(
+                    "Failed to create session, invalid credentials. Please check your OpenTok API Key or JSON web token"
+                )
             elif response.status_code == 404:
-                raise NotFoundError("The session does not exists or the client specified by the connection_id is not connected to the session")
+                raise NotFoundError(
+                    "The session does not exists or the client specified by the connection_id is not connected to the session"
+                )
         except Exception as e:
             raise OpenTokException(
-                (f"There was an error thrown by the OpenTok SDK, please check that your session_id: {session_id}, connection_id (if exists): {connection_id} and digits: {digits} are valid"))
+                (
+                    f"There was an error thrown by the OpenTok SDK, please check that your session_id: {session_id}, connection_id (if exists): {connection_id} and digits: {digits} are valid"
+                )
+            )
+
 
 class OpenTok(Client):
     def __init__(
         self,
         api_key,
         api_secret,
         api_url="https://api.opentok.com",
@@ -2046,21 +2150,20 @@
             stacklevel=2,
         )
         super(OpenTok, self).__init__(
             api_key,
             api_secret,
             api_url=api_url,
             timeout=timeout,
-            app_version=app_version
+            app_version=app_version,
         )
 
-    def mute_all(self,
-                session_id: str,
-                excludedStreamIds: Optional[List[str]]) -> requests.Response:
-
+    def mute_all(
+        self, session_id: str, excludedStreamIds: Optional[List[str]]
+    ) -> requests.Response:
         """
         Mutes all streams in an OpenTok session.
         You can include an optional list of streams IDs to exclude from being muted.
         In addition to existing streams, any streams that are published after the call to
         this method are published with audio muted. You can remove the mute state of a session
         by calling the OpenTok.disableForceMute() method.
         :param session_id The session ID
@@ -2069,65 +2172,74 @@
         """
 
         options = {}
         url = self.endpoints.get_mute_all_url(session_id)
 
         try:
             if excludedStreamIds:
-                options = {'active': True, 'excludedStreams': excludedStreamIds }
+                options = {"active": True, "excludedStreams": excludedStreamIds}
             else:
-                options = {'active': True, 'excludedStreams': []}
+                options = {"active": True, "excludedStreams": []}
 
-            response = requests.post(url, headers=self.get_headers(), data=json.dumps(options))
+            response = requests.post(
+                url, headers=self.get_headers(), data=json.dumps(options)
+            )
 
             if response:
                 return response
             elif response.status_code == 400:
-                raise GetStreamError("Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID.")
+                raise GetStreamError(
+                    "Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID."
+                )
             elif response.status_code == 403:
                 raise AuthError("Failed to mute, invalid credentials.")
             elif response.status_code == 404:
                 raise NotFoundError("The session or a stream is not found.")
         except Exception as e:
             raise OpenTokException(
-                ("There was an error thrown by the OpenTok SDK, please check that your session_id {0} and excludedStreamIds (if exists) {1} are valid").format(
-                    session_id, excludedStreamIds))
-
+                (
+                    "There was an error thrown by the OpenTok SDK, please check that your session_id {0} and excludedStreamIds (if exists) {1} are valid"
+                ).format(session_id, excludedStreamIds)
+            )
 
     def disable_force_mute(self, session_id: str) -> requests.Response:
         """
         Disables the active mute state of the session. After you call this method, new streams
         published to the session will no longer have audio muted.
         After you call the mute_all() method, any streams published after
         the call are published with audio muted. Call the OpenTok.disable_force_mute() method
         to remove the mute state of a session, so that new published streams are not
         automatically muted.
         :param session_id The session ID.
         """
 
-        options = {'active': False}
+        options = {"active": False}
         url = self.endpoints.get_mute_all_url(session_id)
 
-        response = requests.post(url, headers=self.get_headers(), data=json.dumps(options))
-
+        response = requests.post(
+            url, headers=self.get_headers(), data=json.dumps(options)
+        )
 
         try:
             if response:
-                    return response
+                return response
             elif response.status_code == 400:
-                raise GetStreamError("Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID.")
+                raise GetStreamError(
+                    "Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID."
+                )
             elif response.status_code == 403:
                 raise AuthError("Failed to mute, invalid credentials.")
             elif response.status_code == 404:
                 raise NotFoundError("The session or a stream is not found.")
         except Exception as e:
             raise OpenTokException(
-                ("There was an error thrown by the OpenTok SDK, please check that your session_id {0} is valid").format(
-                    session_id))
-
+                (
+                    "There was an error thrown by the OpenTok SDK, please check that your session_id {0} is valid"
+                ).format(session_id)
+            )
 
     def mute_stream(self, session_id: str, stream_id: str) -> requests.Response:
         """
         Mutes a single stream in an OpenTok session.
         :param session_id The session ID.
         :param stream_id The stream ID.
         """
@@ -2135,28 +2247,33 @@
         try:
             if stream_id:
                 url = self.endpoints.get_stream_url(session_id, stream_id) + "/mute"
 
             response = requests.post(url, headers=self.get_headers())
 
             if response:
-                    return response
+                return response
             elif response.status_code == 400:
-                raise GetStreamError("Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID.")
+                raise GetStreamError(
+                    "Invalid request. This response may indicate that data in your request data is invalid JSON. Or it may indicate that you do not pass in a session ID or you passed in an invalid stream ID."
+                )
             elif response.status_code == 403:
                 raise AuthError("Failed to mute, invalid credentials.")
             elif response.status_code == 404:
                 raise NotFoundError("Mute not found")
         except Exception as e:
             raise OpenTokException(
-                ("There was an error thrown by the OpenTok SDK, please check that your session_id {0} and stream_id {1} are valid").format(
-                    session_id, stream_id))
-
+                (
+                    "There was an error thrown by the OpenTok SDK, please check that your session_id {0} and stream_id {1} are valid"
+                ).format(session_id, stream_id)
+            )
 
-    def play_dtmf(self, session_id: str, connection_id: str, digits: str, options: dict = {}) -> requests.Response:
+    def play_dtmf(
+        self, session_id: str, connection_id: str, digits: str, options: dict = {}
+    ) -> requests.Response:
         """
         Plays a DTMF string into a session or to a specific connection
         :param session_id The ID of the OpenTok session that the participant being called
         will join
         :param connection_id An optional parameter used to send the DTMF tones to a specific
         connectoiin in a session.
         :param digits DTMF digits to play
@@ -2168,20 +2285,31 @@
             if not connection_id:
                 url = self.endpoints.get_dtmf_all_url(session_id)
                 payload = {"digits": digits}
             else:
                 url = self.endpoints.get_dtmf_specific_url(session_id, connection_id)
                 payload = {"digits": digits}
 
-            response = requests.post(url, headers=self.get_json_headers(), data=json.dumps(payload))
+            response = requests.post(
+                url, headers=self.get_json_headers(), data=json.dumps(payload)
+            )
 
             if response.status_code == 200:
                 return response
             elif response.status_code == 400:
-                raise DTMFError("One of the properties digits, sessionId or connectionId is invalid.")
+                raise DTMFError(
+                    "One of the properties digits, sessionId or connectionId is invalid."
+                )
             elif response.status_code == 403:
-                raise AuthError("Failed to create session, invalid credentials. Please check your OpenTok API Key or JSON web token")
+                raise AuthError(
+                    "Failed to create session, invalid credentials. Please check your OpenTok API Key or JSON web token"
+                )
             elif response.status_code == 404:
-                raise NotFoundError("The session does not exists or the client specified by the connection_id is not connected to the session")
+                raise NotFoundError(
+                    "The session does not exists or the client specified by the connection_id is not connected to the session"
+                )
         except Exception as e:
             raise OpenTokException(
-                (f"There was an error thrown by the OpenTok SDK, please check that your session_id: {session_id}, connection_id (if exists): {connection_id} and digits: {digits} are valid"))
+                (
+                    f"There was an error thrown by the OpenTok SDK, please check that your session_id: {session_id}, connection_id (if exists): {connection_id} and digits: {digits} are valid"
+                )
+            )
```

### Comparing `opentok-3.5.0/opentok/render.py` & `opentok-3.6.0/opentok/render.py`

 * *Files identical despite different names*

### Comparing `opentok-3.5.0/opentok/session.py` & `opentok-3.6.0/opentok/session.py`

 * *Files identical despite different names*

### Comparing `opentok-3.5.0/opentok/stream.py` & `opentok-3.6.0/opentok/stream.py`

 * *Files identical despite different names*

### Comparing `opentok-3.5.0/opentok/streamlist.py` & `opentok-3.6.0/opentok/streamlist.py`

 * *Files identical despite different names*

### Comparing `opentok-3.5.0/opentok/websocket_audio_connection.py` & `opentok-3.6.0/opentok/websocket_audio_connection.py`

 * *Files identical despite different names*

### Comparing `opentok-3.5.0/opentok.egg-info/PKG-INFO` & `opentok-3.6.0/opentok.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentok
-Version: 3.5.0
+Version: 3.6.0
 Summary: OpenTok server-side SDK
 Home-page: https://github.com/opentok/Opentok-Python-SDK/
 Author: TokBox, Inc.
 Author-email: support@tokbox.com
 License: LICENSE.txt
 Keywords: video chat tokbox tok opentok python media webrtc archiving realtime
 Classifier: Development Status :: 5 - Production/Stable
@@ -88,14 +88,23 @@
   `OpenTok Media Router <https://tokbox.com/developer/guides/create-session/#media-mode>`_
   or attempt to send streams directly between clients. A routed session is required for some
   OpenTok features (such as archiving).
 
 * ``archive_mode`` which specifies whether the session will be automatically archived (``always``)
   or not (``manual``).
 
+* ``archive_name`` which indicates the archive name for all the archives in auto archived session. 
+  A session that begins with archive mode 'always' will be using this archive name for all archives of that session.
+  Passing 'archive_name' with archive mode 'manual' will cause an error response.
+
+* ``archive_resolution`` which indicates the archive resolution for all the archives in auto archived session.
+  Valid values are '640x480', '480x640', '1280x720', '720x1280', '1920x1080' and '1080x1920'.
+  A session that begins with archive mode 'always' will be using this resolution for all archives of that session.
+  Passing 'archive_resolution' with archive mode 'manual' will cause an error response.
+
 * ``e2ee`` which is a boolean. This specifies whether to enable
   `end-to-end encryption <https://tokbox.com/developer/guides/end-to-end-encryption/>`_
   for the OpenTok session.
 
 This method returns a ``Session`` object. Its ``session_id`` attribute is useful when saving to a persistent
 store (such as a database).
 
@@ -108,14 +117,22 @@
   from opentok import MediaModes
   # A session that uses the OpenTok Media Router, which is required for archiving:
   session = opentok.create_session(media_mode=MediaModes.routed)
 
   # An automatically archived session:
   session = opentok.create_session(media_mode=MediaModes.routed, archive_mode=ArchiveModes.always)
 
+  # An automatically archived session with the archive name and resolution specified:
+  session = opentok.create_session(
+    media_mode=MediaModes.routed,
+    archive_mode=ArchiveModes.always,
+    archive_name='my_archive',
+    archive_resolution='1920x1080'
+  )
+
   # A session with a location hint
   session = opentok.create_session(location=u'12.34.56.78')
 
   # Store this session ID in the database
   session_id = session.session_id
 
 Generating Tokens
@@ -447,14 +464,16 @@
   session_id = 'SESSIONID'
   options = {
     'layout': {
       'type': 'custom',
       'stylesheet': 'the layout stylesheet (only used with type == custom)'
     },
     'maxDuration': 5400,
+    'hasAudio': True
+    'hasVideo': True
     'outputs': {
       'hls': {},
       'rtmp': [{
         'id': 'foo',
         'serverUrl': 'rtmp://myfooserver/myfooapp',
         'streamName': 'myfoostream'
       }, {
@@ -503,14 +522,45 @@
   }
 
   broadcast = opentok.start_broadcast(session_id, options)
   
 To enable multiple simultaneous broadcasts on the same session, specify a unique value for the 
 ``multiBroadcastTag`` parameter in ``options`` when calling the ``opentok.start_broadcast`` method.
 
+You can broadcast only audio, or only video, for a stream by setting ``hasAudio`` or ``hasVideo``
+to ``False`` as required. These fields are ``True`` by default.
+
+.. code:: python
+
+  session_id = 'SESSIONID'
+  options = {
+    'layout': {
+      'type': 'custom',
+      'stylesheet': 'the layout stylesheet (only used with type == custom)'
+    },
+    'maxDuration': 5400,
+    'hasAudio': True
+    'hasVideo': False
+    'outputs': {
+      'hls': {},
+      'rtmp': [{
+        'id': 'foo',
+        'serverUrl': 'rtmp://myfooserver/myfooapp',
+        'streamName': 'myfoostream'
+      }, {
+        'id': 'bar',
+        'serverUrl': 'rtmp://mybarserver/mybarapp',
+        'streamName': 'mybarstream'
+      }]
+    },
+    'resolution': '640x480'
+  }
+
+  broadcast = opentok.start_broadcast(session_id, options)
+
 You can stop a started Broadcast using the ``opentok.stop_broadcast(broadcast_id)`` method.
 
 .. code:: python
 
   # getting the ID from a broadcast object
   broadcast_id = broadcast.id
 
@@ -666,14 +716,23 @@
   
   digits = '12345'
   opentok.play_dtmf(session_id, digits)
 
   # To a specific connection
   opentok.play_dtmf(session_id, connection_id, digits)
 
+Appending to the User Agent
+---------------------------
+
+You can append a string to the user agent that is sent with requests:
+
+.. code:: python
+
+  opentok.append_to_user_agent('my-appended-string')
+
 Samples
 -------
 
 There are two sample applications included in this repository. To get going as fast as possible, clone the whole
 repository and follow the Walkthroughs:
 
 - `HelloWorld <sample/HelloWorld/README.md>`_
```

### Comparing `opentok-3.5.0/setup.py` & `opentok-3.6.0/setup.py`

 * *Files identical despite different names*

