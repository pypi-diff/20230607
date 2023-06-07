# Comparing `tmp/sqlsprinkler_python_GT3CH1-0.0.7-py3-none-any.whl.zip` & `tmp/sqlsprinkler_python_GT3CH1-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5717 bytes, number of entries: 9
+Zip file size: 5747 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      107 b- defN 23-May-03 22:05 sqlsprinkler/__init__.py
 -rw-r--r--  2.0 unx      222 b- defN 23-May-03 22:30 sqlsprinkler/api.py
--rw-r--r--  2.0 unx     7383 b- defN 23-Jun-07 00:02 sqlsprinkler/system.py
--rw-r--r--  2.0 unx     3845 b- defN 23-Jun-04 21:39 sqlsprinkler/zone.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-07 00:09 sqlsprinkler_python_GT3CH1-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      830 b- defN 23-Jun-07 00:09 sqlsprinkler_python_GT3CH1-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 00:09 sqlsprinkler_python_GT3CH1-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-07 00:09 sqlsprinkler_python_GT3CH1-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      791 b- defN 23-Jun-07 00:09 sqlsprinkler_python_GT3CH1-0.0.7.dist-info/RECORD
-9 files, 14351 bytes uncompressed, 4333 bytes compressed:  69.8%
+-rw-r--r--  2.0 unx     7383 b- defN 23-Jun-07 00:17 sqlsprinkler/system.py
+-rw-r--r--  2.0 unx     4361 b- defN 23-Jun-07 00:20 sqlsprinkler/zone.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-07 00:21 sqlsprinkler_python_GT3CH1-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      830 b- defN 23-Jun-07 00:21 sqlsprinkler_python_GT3CH1-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 00:21 sqlsprinkler_python_GT3CH1-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-07 00:21 sqlsprinkler_python_GT3CH1-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      791 b- defN 23-Jun-07 00:21 sqlsprinkler_python_GT3CH1-0.0.8.dist-info/RECORD
+9 files, 14867 bytes uncompressed, 4363 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: sqlsprinkler/system.py
 Comment: 
 
 Filename: sqlsprinkler/zone.py
 Comment: 
 
-Filename: sqlsprinkler_python_GT3CH1-0.0.7.dist-info/LICENSE
+Filename: sqlsprinkler_python_GT3CH1-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: sqlsprinkler_python_GT3CH1-0.0.7.dist-info/METADATA
+Filename: sqlsprinkler_python_GT3CH1-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: sqlsprinkler_python_GT3CH1-0.0.7.dist-info/WHEEL
+Filename: sqlsprinkler_python_GT3CH1-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: sqlsprinkler_python_GT3CH1-0.0.7.dist-info/top_level.txt
+Filename: sqlsprinkler_python_GT3CH1-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlsprinkler_python_GT3CH1-0.0.7.dist-info/RECORD
+Filename: sqlsprinkler_python_GT3CH1-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlsprinkler/system.py

```diff
@@ -68,15 +68,15 @@
         """
         Updates the system.
         :return: None
         """
         self.zones = self._fetch_zones()
         self._update_system_state()
 
-    async def update_async(self):
+    async def async_update(self):
         """
         Fetches the zones from the hostname.
         :return: A list of zones.
         """
         url = "{}/{}".format(self.hostname,API.ZONE_INFO_URL)
         zone_list = []
         async with aiohttp.ClientSession() as session:
@@ -102,33 +102,33 @@
 
     def turn_on(self):
         self.set_system_state(True)
 
     def turn_off(self):
         self.set_system_state(False)
 
-    async def turn_on_async(self)
-        self.set_system_state_async(True)
+    async def async_turn_on(self)
+        self.async_set_system_state(True)
 
-    async def turn_on_async(self)
-        self.set_system_state_async(False)
+    async def async_turn_on(self)
+        self.async_set_system_state(False)
 
     def set_system_state(self, state: bool) -> None:
         """
         Sets the system state.
         :param state: The state to set.
         :return: None
         """
         url = "{}/{}".format(self.hostname,API.SYSTEM_STATE_URL)
         request = self.session.put(url, json={"system_enabled": state})
         if request.status_code != 200:
             raise Exception(f"Failed to set system state {state}")
         self._update_system_state()
 
-    async def set_system_state_async(self,state: bool) -> None:
+    async def async_set_system_state(self,state: bool) -> None:
         url = "{}/{}".format(self.hostname,API.SYSTEM_STATE_URL)
         json={"system_enabled": state}
         async with aiohttp.ClientSession() as session:
             async with session.post(url,json) as response:
                 status = await response.status_code
                 if status_code != 200:
                     raise Exception(f"Failed to set system state {state}")
```

## sqlsprinkler/zone.py

```diff
@@ -1,11 +1,10 @@
 from dataclasses import field, dataclass
 
 import requests
-import asyncio
 import aiohttp
 from sqlsprinkler import API
 
 
 @dataclass
 class Zone:
     """ This class represents a SQL Sprinkler zone. """
@@ -41,17 +40,29 @@
 
     def update(self) -> None:
         """
         Updates the state of the zone.
         :return: None
         """
         # send request to API_ZONE_INFO_URL with ID
-        asyncio.run(self.async_update())
+        url = "{}/{}/{}".format(self.host, API.ZONE_INFO_URL, self.id)
+        response = self.session.get(url)
+        if response.status_code != 200:
+            raise Exception("Failed to update zone {}".format(self.id))
+        response = response.json()                     
+        self.name = response['name']
+        self.gpio = response['gpio']
+        self.time = response['time']
+        self.enabled = response['enabled']
+        self.auto_off = response['auto_off']
+        self.system_order = response['system_order']
+        self.state = response['state']
+
 
-    async def update_async(self) -> None:
+    async def async_update(self) -> None:
         url = "{}/{}/{}".format(self.host, API.ZONE_INFO_URL, self.id)
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as request:
                 response = await request.json()
                 self.name = response['name']
                 self.gpio = response['gpio']
                 self.time = response['time']
```

## Comparing `sqlsprinkler_python_GT3CH1-0.0.7.dist-info/LICENSE` & `sqlsprinkler_python_GT3CH1-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sqlsprinkler_python_GT3CH1-0.0.7.dist-info/METADATA` & `sqlsprinkler_python_GT3CH1-0.0.8.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsprinkler-python-GT3CH1
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python library to control a SQLSprinkler system
 Home-page: https://github.com/GT3CH1/sqlsprinkler_python
 Author: Gavin Pease
 Author-email: gavinpease@gmail.com
 Project-URL: Bug Tracker, https://github.com/GT3CH1/sqlsprinkler_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `sqlsprinkler_python_GT3CH1-0.0.7.dist-info/RECORD` & `sqlsprinkler_python_GT3CH1-0.0.8.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 sqlsprinkler/__init__.py,sha256=pg952RebeeOzsYtyrA6QNAcY7886d4juHUrda7PbdXQ,107
 sqlsprinkler/api.py,sha256=EWjPjHy5locZtRQF26JNm31z6mLTRgLksycXpmBB_7M,222
-sqlsprinkler/system.py,sha256=DQ685b35UFTd6F_9bgBZ475n2rO6g-elWvWB1bsk6OI,7383
-sqlsprinkler/zone.py,sha256=NoeH4zuwWM1RSQOERXMjSN6jaCYR6VAz1rUSwxNSfSM,3845
-sqlsprinkler_python_GT3CH1-0.0.7.dist-info/LICENSE,sha256=L6YQEZortlWlNmb1Zl8feSk4ifo39dg0KTiZjVK-6h8,1068
-sqlsprinkler_python_GT3CH1-0.0.7.dist-info/METADATA,sha256=XfCARrygZoBmKeLAPR62hqHWh0GDDWwpIFJfXzs7DRA,830
-sqlsprinkler_python_GT3CH1-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sqlsprinkler_python_GT3CH1-0.0.7.dist-info/top_level.txt,sha256=UOpJrwrCTBjFX_uKBfS9EYYRgMrSpV56d8Jqg9oBX_o,13
-sqlsprinkler_python_GT3CH1-0.0.7.dist-info/RECORD,,
+sqlsprinkler/system.py,sha256=SzCdhcfxDPcE7Y0LTSwKc78x5-0jqE35VYUzOuURKQU,7383
+sqlsprinkler/zone.py,sha256=7XH-gm6Y33PVQIDYE8H8eE7GbYUIsQRu0MwkUPcRAjU,4361
+sqlsprinkler_python_GT3CH1-0.0.8.dist-info/LICENSE,sha256=L6YQEZortlWlNmb1Zl8feSk4ifo39dg0KTiZjVK-6h8,1068
+sqlsprinkler_python_GT3CH1-0.0.8.dist-info/METADATA,sha256=8HxN1eo7qGzcInxNTLkCmANHVRPlkFh3-zyZEbwSdOs,830
+sqlsprinkler_python_GT3CH1-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sqlsprinkler_python_GT3CH1-0.0.8.dist-info/top_level.txt,sha256=UOpJrwrCTBjFX_uKBfS9EYYRgMrSpV56d8Jqg9oBX_o,13
+sqlsprinkler_python_GT3CH1-0.0.8.dist-info/RECORD,,
```

