# Comparing `tmp/podium_api-0.0.8.tar.gz` & `tmp/podium_api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/podium_api-0.0.8.tar", last modified: Sat Sep 23 06:57:33 2017, max compression
+gzip compressed data, was "dist/podium_api-0.0.9.tar", last modified: Thu Nov  9 16:00:21 2017, max compression
```

## Comparing `podium_api-0.0.8.tar` & `podium_api-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 brent     (1000) brent     (1000)        0 2017-09-23 06:57:33.000000 podium_api-0.0.8/
--rw-rw-r--   0 brent     (1000) brent     (1000)       94 2017-07-24 01:05:47.000000 podium_api-0.0.8/README.txt
--rw-rw-r--   0 brent     (1000) brent     (1000)      416 2017-09-23 06:57:33.000000 podium_api-0.0.8/PKG-INFO
-drwxrwxr-x   0 brent     (1000) brent     (1000)        0 2017-09-23 06:57:33.000000 podium_api-0.0.8/podium_api/
--rw-rw-r--   0 brent     (1000) brent     (1000)    12607 2017-09-23 06:39:02.000000 podium_api-0.0.8/podium_api/friendships.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     3059 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/users.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     6551 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/laps.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     1615 2017-09-23 06:39:02.000000 podium_api-0.0.8/podium_api/__init__.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     2797 2017-09-23 06:39:02.000000 podium_api-0.0.8/podium_api/login.py
--rw-rw-r--   0 brent     (1000) brent     (1000)    39377 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/api.py
--rw-rw-r--   0 brent     (1000) brent     (1000)    15988 2017-09-23 06:39:02.000000 podium_api-0.0.8/podium_api/events.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     3253 2017-09-23 06:39:02.000000 podium_api-0.0.8/podium_api/account.py
--rw-rw-r--   0 brent     (1000) brent     (1000)    16489 2017-09-23 06:39:02.000000 podium_api-0.0.8/podium_api/eventdevices.py
-drwxrwxr-x   0 brent     (1000) brent     (1000)        0 2017-09-23 06:57:33.000000 podium_api-0.0.8/podium_api/types/
--rw-rw-r--   0 brent     (1000) brent     (1000)     2570 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/types/paged_response.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     1279 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/types/lap.py
--rw-rw-r--   0 brent     (1000) brent     (1000)       46 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/types/__init__.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     1839 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/types/user.py
--rw-rw-r--   0 brent     (1000) brent     (1000)      867 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/types/redirect.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     1658 2017-09-23 05:19:15.000000 podium_api-0.0.8/podium_api/types/account.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     1132 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/types/device.py
--rw-rw-r--   0 brent     (1000) brent     (1000)      297 2017-09-23 06:39:02.000000 podium_api-0.0.8/podium_api/types/application.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     1252 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/types/friendship.py
--rw-rw-r--   0 brent     (1000) brent     (1000)      585 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/types/exceptions.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     1660 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/types/event.py
--rw-rw-r--   0 brent     (1000) brent     (1000)     1700 2017-09-18 06:12:59.000000 podium_api-0.0.8/podium_api/types/eventdevice.py
--rw-rw-r--   0 brent     (1000) brent     (1000)      911 2017-07-24 01:05:47.000000 podium_api-0.0.8/podium_api/types/token.py
--rw-rw-r--   0 brent     (1000) brent     (1000)    14957 2017-09-23 06:39:02.000000 podium_api-0.0.8/podium_api/devices.py
--rw-rw-r--   0 brent     (1000) brent     (1000)    13832 2017-09-23 06:39:02.000000 podium_api-0.0.8/podium_api/async.py
--rw-rw-r--   0 brent     (1000) brent     (1000)       39 2017-07-24 01:05:47.000000 podium_api-0.0.8/setup.cfg
--rw-rw-r--   0 brent     (1000) brent     (1000)      506 2017-09-23 06:55:33.000000 podium_api-0.0.8/setup.py
+drwxrwxr-x   0 brent     (1000) brent     (1000)        0 2017-11-09 16:00:21.000000 podium_api-0.0.9/
+-rw-rw-r--   0 brent     (1000) brent     (1000)       94 2017-07-24 01:05:47.000000 podium_api-0.0.9/README.txt
+-rw-rw-r--   0 brent     (1000) brent     (1000)      416 2017-11-09 16:00:21.000000 podium_api-0.0.9/PKG-INFO
+drwxrwxr-x   0 brent     (1000) brent     (1000)        0 2017-11-09 16:00:21.000000 podium_api-0.0.9/podium_api/
+-rw-rw-r--   0 brent     (1000) brent     (1000)    12607 2017-09-23 06:39:02.000000 podium_api-0.0.9/podium_api/friendships.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     3059 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/users.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     6551 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/laps.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     1615 2017-09-23 06:39:02.000000 podium_api-0.0.9/podium_api/__init__.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     2797 2017-09-23 06:39:02.000000 podium_api-0.0.9/podium_api/login.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)    39377 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/api.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)    15988 2017-09-23 06:39:02.000000 podium_api-0.0.9/podium_api/events.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     3253 2017-09-23 06:39:02.000000 podium_api-0.0.9/podium_api/account.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)    16489 2017-09-23 06:39:02.000000 podium_api-0.0.9/podium_api/eventdevices.py
+drwxrwxr-x   0 brent     (1000) brent     (1000)        0 2017-11-09 16:00:21.000000 podium_api-0.0.9/podium_api/types/
+-rw-rw-r--   0 brent     (1000) brent     (1000)     2570 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/types/paged_response.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     1279 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/types/lap.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)       46 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/types/__init__.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     1839 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/types/user.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)      867 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/types/redirect.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     1658 2017-09-23 05:19:15.000000 podium_api-0.0.9/podium_api/types/account.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     1132 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/types/device.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)      297 2017-09-23 06:39:02.000000 podium_api-0.0.9/podium_api/types/application.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     1252 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/types/friendship.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)      585 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/types/exceptions.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     1660 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/types/event.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)     1872 2017-11-07 04:03:26.000000 podium_api-0.0.9/podium_api/types/eventdevice.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)      911 2017-07-24 01:05:47.000000 podium_api-0.0.9/podium_api/types/token.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)    14957 2017-09-23 06:39:02.000000 podium_api-0.0.9/podium_api/devices.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)    13832 2017-09-23 06:39:02.000000 podium_api-0.0.9/podium_api/async.py
+-rw-rw-r--   0 brent     (1000) brent     (1000)       39 2017-07-24 01:05:47.000000 podium_api-0.0.9/setup.cfg
+-rw-rw-r--   0 brent     (1000) brent     (1000)      506 2017-11-09 15:59:06.000000 podium_api-0.0.9/setup.py
```

### Comparing `podium_api-0.0.8/podium_api/friendships.py` & `podium_api-0.0.9/podium_api/friendships.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/users.py` & `podium_api-0.0.9/podium_api/users.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/laps.py` & `podium_api-0.0.9/podium_api/laps.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/__init__.py` & `podium_api-0.0.9/podium_api/__init__.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/login.py` & `podium_api-0.0.9/podium_api/login.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/api.py` & `podium_api-0.0.9/podium_api/api.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/events.py` & `podium_api-0.0.9/podium_api/events.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/account.py` & `podium_api-0.0.9/podium_api/account.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/eventdevices.py` & `podium_api-0.0.9/podium_api/eventdevices.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/types/paged_response.py` & `podium_api-0.0.9/podium_api/types/paged_response.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/types/lap.py` & `podium_api-0.0.9/podium_api/types/lap.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/types/user.py` & `podium_api-0.0.9/podium_api/types/user.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/types/redirect.py` & `podium_api-0.0.9/podium_api/types/redirect.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/types/account.py` & `podium_api-0.0.9/podium_api/types/account.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/types/device.py` & `podium_api-0.0.9/podium_api/types/device.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/types/friendship.py` & `podium_api-0.0.9/podium_api/types/friendship.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/types/exceptions.py` & `podium_api-0.0.9/podium_api/types/exceptions.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/types/event.py` & `podium_api-0.0.9/podium_api/types/event.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/types/eventdevice.py` & `podium_api-0.0.9/podium_api/types/eventdevice.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,27 +14,30 @@
 
         **name** (str): Name of device at event. Not always the same as the
         device name.
 
         **device_uri** (str): URI of the device
 
         **laps_uri** (str): URI of lap data.
+        
+        **avatar_uri** (str): URI of the device avatar
 
     """
 
     def __init__(self, eventdevice_id, uri, channels, name, device_uri,
-                 laps_uri, user_uri, event_uri):
+                 laps_uri, user_uri, event_uri, avatar_uri):
         self.eventdevice_id = eventdevice_id
         self.uri = uri
         self.channels = channels
         self.name = name
         self.device_uri = device_uri
         self.laps_uri = laps_uri
         self.user_uri = user_uri
         self.event_uri = event_uri
+        self.avatar_uri = avatar_uri
 
 
 
 def get_eventdevice_from_json(json):
     """
     Returns a PodiumEventDevice object from the json dict received from
     podium api.
@@ -47,8 +50,9 @@
     """
     return PodiumEventDevice(json['id'], json['URI'],
                              json.get('channels', []),
                              json.get('name', None),
                              json.get('device_uri', None),
                              json.get('laps_uri', None),
                              json.get('user_uri', None),
-                             json.get('event_uri', None))
+                             json.get('event_uri', None),
+                             json.get('avatar', None))
```

### Comparing `podium_api-0.0.8/podium_api/types/token.py` & `podium_api-0.0.9/podium_api/types/token.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/devices.py` & `podium_api-0.0.9/podium_api/devices.py`

 * *Files identical despite different names*

### Comparing `podium_api-0.0.8/podium_api/async.py` & `podium_api-0.0.9/podium_api/async.py`

 * *Files identical despite different names*

