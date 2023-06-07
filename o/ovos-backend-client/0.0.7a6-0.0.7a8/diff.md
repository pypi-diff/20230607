# Comparing `tmp/ovos-backend-client-0.0.7a6.tar.gz` & `tmp/ovos-backend-client-0.0.7a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-backend-client-0.0.7a6.tar", last modified: Sat May  6 22:28:01 2023, max compression
+gzip compressed data, was "ovos-backend-client-0.0.7a8.tar", last modified: Wed Jun  7 10:49:24 2023, max compression
```

## Comparing `ovos-backend-client-0.0.7a6.tar` & `ovos-backend-client-0.0.7a8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:01.174351 ovos-backend-client-0.0.7a6/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-06 22:28:01.174351 ovos-backend-client-0.0.7a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:01.170351 ovos-backend-client-0.0.7a6/ovos_backend_client/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:01.174351 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22979 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/ovos.py
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/personal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/selene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-06 22:27:51.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:01.174351 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-06 22:28:00.000000 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-06 22:28:01.000000 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 22:28:00.000000 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 22:28:00.000000 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 22:28:00.000000 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 22:28:01.174351 ovos-backend-client-0.0.7a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:49:24.042743 ovos-backend-client-0.0.7a8/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 10:49:24.042743 ovos-backend-client-0.0.7a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:49:24.038743 ovos-backend-client-0.0.7a8/ovos_backend_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:49:24.042743 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/ovos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/personal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/selene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:49:24.038743 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 10:49:24.000000 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-07 10:49:24.000000 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:49:24.000000 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 10:49:24.000000 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 10:49:24.000000 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:49:24.042743 ovos-backend-client-0.0.7a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/setup.py
```

### Comparing `ovos-backend-client-0.0.7a6/README.md` & `ovos-backend-client-0.0.7a8/README.md`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/api.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/api.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/__init__.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/base.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/backends/base.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/offline.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/backends/offline.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from uuid import uuid4
 
 import requests
 from json_database import JsonStorageXDG
 from ovos_config.config import Configuration
 from ovos_config.config import update_mycroft_config
 from ovos_plugin_manager.stt import OVOSSTTFactory, get_stt_config
+from ovos_utils import timed_lru_cache
 from ovos_utils.log import LOG
 from ovos_utils.network_utils import get_external_ip
 from ovos_utils.smtp_utils import send_smtp
 
 from ovos_backend_client.backends.base import AbstractBackend, BackendType
 from ovos_backend_client.database import BackendDatabase
 from ovos_backend_client.identity import IdentityManager
@@ -21,14 +22,15 @@
 class OfflineBackend(AbstractBackend):
 
     def __init__(self, url="127.0.0.1", version="v1", identity_file=None, credentials=None):
         super().__init__(url, version, identity_file, BackendType.OFFLINE, credentials)
         self.stt = None
 
     # OWM API
+    @timed_lru_cache(seconds=600)  # cache results for 10 mins
     def owm_get_weather(self, lat_lon=None, lang="en-us", units="metric"):
         """Issue an API call and map the return value into a weather report
 
         Args:
             units (str): metric or imperial measurement units
             lat_lon (tuple): the geologic (latitude, longitude) of the weather location
         """
@@ -41,14 +43,15 @@
             "lat": lat, "lon": lon,
             "appid": self.credentials["owm"]
         }
         url = "https://api.openweathermap.org/data/2.5/onecall"
         response = self.get(url, params=params)
         return response.json()
 
+    @timed_lru_cache(seconds=600)  # cache results for 10 mins
     def owm_get_current(self, lat_lon=None, lang="en-us", units="metric"):
         """Issue an API call and map the return value into a weather report
 
         Args:
             units (str): metric or imperial measurement units
             lat_lon (tuple): the geologic (latitude, longitude) of the weather location
         """
@@ -61,14 +64,15 @@
             "lat": lat, "lon": lon,
             "appid": self.credentials["owm"]
         }
         url = "https://api.openweathermap.org/data/2.5/weather"
         response = self.get(url, params=params)
         return response.json()
 
+    @timed_lru_cache(seconds=600)  # cache results for 10 mins
     def owm_get_hourly(self, lat_lon=None, lang="en-us", units="metric"):
         """Issue an API call and map the return value into a weather report
 
         Args:
             units (str): metric or imperial measurement units
             lat_lon (tuple): the geologic (latitude, longitude) of the weather location
         """
@@ -81,14 +85,15 @@
             "lat": lat, "lon": lon,
             "appid": self.credentials["owm"]
         }
         url = "https://api.openweathermap.org/data/2.5/forecast"
         response = self.get(url, params=params)
         return response.json()
 
+    @timed_lru_cache(seconds=600)  # cache results for 10 mins
     def owm_get_daily(self, lat_lon=None, lang="en-us", units="metric"):
         """Issue an API call and map the return value into a weather report
 
         Args:
             units (str): metric or imperial measurement units
             lat_lon (tuple): the geologic (latitude, longitude) of the weather location
         """
@@ -102,38 +107,41 @@
             "appid": self.credentials["owm"]
         }
         url = "https://api.openweathermap.org/data/2.5/forecast/daily"
         response = self.get(url, params=params)
         return response.json()
 
     # Wolfram Alpha Api
+    @timed_lru_cache(seconds=600)  # cache results for 10 mins
     def wolfram_spoken(self, query, units="metric", lat_lon=None, optional_params=None):
         optional_params = optional_params or {}
         if not lat_lon:
             lat_lon = self._get_lat_lon(**optional_params)
         params = {'i': query,
                   "geolocation": "{},{}".format(*lat_lon),
                   'units': units,
                   **optional_params}
         url = 'https://api.wolframalpha.com/v1/spoken'
         params["appid"] = self.credentials["wolfram"]
         return self.get(url, params=params).text
 
+    @timed_lru_cache(seconds=600)  # cache results for 10 mins
     def wolfram_simple(self, query, units="metric", lat_lon=None, optional_params=None):
         optional_params = optional_params or {}
         if not lat_lon:
             lat_lon = self._get_lat_lon(**optional_params)
         params = {'i': query,
                   "geolocation": "{},{}".format(*lat_lon),
                   'units': units,
                   **optional_params}
         url = 'https://api.wolframalpha.com/v1/simple'
         params["appid"] = self.credentials["wolfram"]
         return self.get(url, params=params).text
 
+    @timed_lru_cache(seconds=600)  # cache results for 10 mins
     def wolfram_full_results(self, query, units="metric", lat_lon=None, optional_params=None):
         """Wrapper for the WolframAlpha Full Results v2 API.
         https://products.wolframalpha.com/api/documentation/
         Pods of interest
         - Input interpretation - Wolfram's determination of what is being asked about.
         - Name - primary name of
         """
@@ -149,14 +157,15 @@
                   **optional_params}
         url = 'https://api.wolframalpha.com/v2/query'
         params["appid"] = self.credentials["wolfram"]
         data = self.get(url, params=params)
         return data.json()
 
     # Geolocation Api
+    @timed_lru_cache(seconds=600)  # cache results for 10 mins
     def geolocation_get(self, location):
         """Call the geolocation endpoint.
 
         Args:
             location (str): the location to lookup (e.g. Kansas City Missouri)
 
         Returns:
@@ -166,46 +175,53 @@
         data = self.get(url, params={"q": location, "format": "json", "limit": 1}).json()[0]
         lat = data.get("lat")
         lon = data.get("lon")
 
         if lat and lon:
             return self.reverse_geolocation_get(lat, lon)
 
-        url = "https://nominatim.openstreetmap.org/details.php?osmtype=W&osmid=38210407&format=json"
+        url = "https://nominatim.openstreetmap.org/details.php"
         details = self.get(url, params={"osmid": data['osm_id'], "osmtype": data['osm_type'][0].upper(),
                                         "format": "json"}).json()
+
         # if no addresstags are present for the location an empty list is sent instead of a dict
-        if not details.get("addresstags"):
-            details["addresstags"] = dict()
+        tags = details.get("addresstags") or {}
 
+        place_type = details["extratags"].get("linked_place") or details.get("category") or data.get(
+            "type") or data.get("class")
+        name = details["localname"] or details["names"].get("name") or details["names"].get("official_name") or data[
+            "display_name"]
+        cc = details["country_code"] or tags.get("country") or details["extratags"].get('ISO3166-1:alpha2') or ""
+        # TODO - lang support, official name is reported in various langs
         location = {
+            "address": data["display_name"],
             "city": {
-                "code": details.get("addresstags", {}).get("postcode") or \
-                        details.get("calculated_postcode") or "",
-                "name": details.get("localname"),
+                "code": tags.get("postcode") or
+                        details["calculated_postcode"] or "",
+                "name": name if place_type == "city" else "",
                 "state": {
-                    "code": details.get("addresstags", {}).get("state_code") or \
-                            details.get("calculated_postcode") or "",
-                    "name": details.get("addresstags", {}).get("state") or \
-                            data.get("display_name", "").split(", ")[0] or "",
+                    "code": tags.get("state_code") or
+                            details["calculated_postcode"] or "",
+                    "name": name if place_type == "state" else tags.get("state"),
                     "country": {
-                        "code": details.get("country_code", "").upper() or \
-                                details.get("addresstags", {}).get("country") or "",
-                        "name": data.get("display_name", "").split(", ")[-1]
+                        "code": cc.upper(),
+                        "name": name if place_type == "country" else ""  # TODO - country code to name
                     }
                 }
             },
             "coordinate": {
                 "latitude": lat,
                 "longitude": lon
             }
         }
-
+        if "timezone" not in location:
+            location["timezone"] = self._get_timezone(lon=lon, lat=lat)
         return location
 
+    @timed_lru_cache(seconds=600)  # cache results for 10 mins
     def reverse_geolocation_get(self, lat, lon):
         """Call the reverse geolocation endpoint.
 
         Args:
             lat (float): latitude
             lon (float): longitude
 
@@ -235,21 +251,23 @@
                         "name": address.get("country") or "",
                     }
                 }
             },
             "coordinate": {
                 "latitude": details.get("lat") or lat,
                 "longitude": details.get("lon") or lon
-            },
-            "timezone": self._get_timezone(lat=details.get("lat") or lat,
-                                           lon=details.get("lon") or lon)
+            }
         }
-
+        if "timezone" not in location:
+            location["timezone"] = self._get_timezone(
+                lat=details.get("lat") or lat,
+                lon=details.get("lon") or lon)
         return location
 
+    @timed_lru_cache(seconds=600)  # cache results for 10 mins
     def ip_geolocation_get(self, ip):
         """Call the geolocation endpoint.
 
         Args:
             ip (str): the ip address to lookup
 
         Returns:
@@ -560,18 +578,17 @@
 
         Args:
             audio (bytes): The recorded audio, as in a FLAC file
             language (str): A BCP-47 language code, e.g. "en-US"
             limit (int): Maximum alternate transcriptions
 
        """
-        from speech_recognition import Recognizer, AudioFile
-
         if self.stt is None:
             self.load_stt_plugin(lang=language)
+        from speech_recognition import AudioFile, Recognizer
         with NamedTemporaryFile() as fp:
             fp.write(audio)
             with AudioFile(fp.name) as source:
                 audio = Recognizer().record(source)
         tx = self.stt.execute(audio, language)
         if isinstance(tx, str):
             tx = [tx]
```

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/ovos.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/backends/ovos.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/personal.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/backends/personal.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/selene.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/backends/selene.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/cloud.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/cloud.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/config.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/config.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/database.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/database.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/identity.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/identity.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/pairing.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/pairing.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client/settings.py` & `ovos-backend-client-0.0.7a8/ovos_backend_client/settings.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/SOURCES.txt` & `ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a6/setup.py` & `ovos-backend-client-0.0.7a8/setup.py`

 * *Files identical despite different names*

