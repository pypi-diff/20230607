# Comparing `tmp/ensta-0.6.tar.gz` & `tmp/ensta-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-0.6.tar", last modified: Tue Jun  6 16:22:41 2023, max compression
+gzip compressed data, was "ensta-0.7.tar", last modified: Wed Jun  7 07:14:19 2023, max compression
```

## Comparing `ensta-0.6.tar` & `ensta-0.7.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:22:41.162260 ensta-0.6/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1687 2023-06-06 16:22:41.162260 ensta-0.6/PKG-INFO
--rw-rw-rw-   0        0        0      964 2023-06-06 15:54:53.000000 ensta-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 16:22:41.146643 ensta-0.6/ensta/
--rw-rw-rw-   0        0        0    15625 2023-06-06 16:22:21.000000 ensta-0.6/ensta/Guest.py
--rw-rw-rw-   0        0        0     6399 2023-06-06 16:22:15.000000 ensta-0.6/ensta/Host.py
--rw-rw-rw-   0        0        0       58 2023-06-06 15:20:49.000000 ensta-0.6/ensta/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-06-06 16:22:15.000000 ensta-0.6/ensta/commons.py
--rw-rw-rw-   0        0        0      217 2023-06-05 12:51:10.000000 ensta-0.6/ensta/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:22:41.162260 ensta-0.6/ensta.egg-info/
--rw-rw-rw-   0        0        0     1687 2023-06-06 16:22:41.000000 ensta-0.6/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-06-06 16:22:41.000000 ensta-0.6/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:22:41.000000 ensta-0.6/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 16:22:41.000000 ensta-0.6/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 16:22:41.000000 ensta-0.6/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-06 16:22:41.162260 ensta-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-06-06 16:22:35.000000 ensta-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:14:19.310845 ensta-0.7/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     1687 2023-06-07 07:14:19.310845 ensta-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2023-06-06 15:54:53.000000 ensta-0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 07:14:19.295461 ensta-0.7/ensta/
+-rw-rw-rw-   0        0        0    15661 2023-06-07 07:12:11.000000 ensta-0.7/ensta/Guest.py
+-rw-rw-rw-   0        0        0     6447 2023-06-07 07:11:41.000000 ensta-0.7/ensta/Host.py
+-rw-rw-rw-   0        0        0       60 2023-06-07 07:03:08.000000 ensta-0.7/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:14:19.310845 ensta-0.7/ensta.egg-info/
+-rw-rw-rw-   0        0        0     1687 2023-06-07 07:14:19.000000 ensta-0.7/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-07 07:14:19.000000 ensta-0.7/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 07:14:19.000000 ensta-0.7/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 07:14:19.000000 ensta-0.7/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 07:14:19.000000 ensta-0.7/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-07 07:14:19.310845 ensta-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-06-07 07:01:57.000000 ensta-0.7/setup.py
```

### Comparing `ensta-0.6/LICENSE.txt` & `ensta-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-0.6/PKG-INFO` & `ensta-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 0.6
+Version: 0.7
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v0.1.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
```

### Comparing `ensta-0.6/README.md` & `ensta-0.7/README.md`

 * *Files identical despite different names*

### Comparing `ensta-0.6/ensta/Guest.py` & `ensta-0.7/ensta/Guest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from json import JSONDecodeError
 import base64
 import random
 import requests
 import requests.cookies
-import commons
+from .lib import update_session, update_homepage_source, update_app_id, refresh_csrf_token
 
 
 class Guest:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     csrf_token: str = None
 
     def __init__(self):
-        commons.update_session(self)
-        commons.update_homepage_source(self)
-        commons.update_app_id(self)
+        update_session(self)
+        update_homepage_source(self)
+        update_app_id(self)
 
     def username_availability(self, username: str):
         username = username.strip().lower().replace(" ", "")
-        commons.refresh_csrf_token(self)
+        refresh_csrf_token(self)
         preferred_color_scheme = random.choice(["light", "dark"])
         body_json = {
             "email": f"{username}@{self.csrf_token}.com",
             "username": username,
             "first_name": username.capitalize(),
             "opt_into_one_tap": False
         }
@@ -68,15 +68,15 @@
             else:
                 return {"success": False, "available": None, "suggestions": []}
         except JSONDecodeError:
             return {"success": False, "available": None, "suggestions": []}
 
     def profile_info(self, username: str):
         username = username.strip().lower().replace(" ", "")
-        commons.refresh_csrf_token(self)
+        refresh_csrf_token(self)
         preferred_color_scheme = random.choice(["light", "dark"])
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": preferred_color_scheme,
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
             "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
```

### Comparing `ensta-0.6/ensta/Host.py` & `ensta-0.7/ensta/Host.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import requests
 import requests.cookies
 from json import JSONDecodeError
 import random
 import string
-from Guest import Guest
-import commons
-import exceptions
+from .Guest import Guest
+from .lib import update_session, update_homepage_source, update_app_id, refresh_csrf_token
+from .lib import AuthenticationError, NetworkError
 
 
 class Host:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     preferred_color_scheme: str = "dark"
     x_ig_www_claim: str = None
     csrf_token: str = None
     guest: Guest = None
 
     def __init__(self, session_id: str):
         self.x_ig_www_claim = "hmac." + "".join(random.choices(string.ascii_letters + string.digits + "_-", k=48))
-        commons.update_session(self)
-        commons.update_homepage_source(self)
-        commons.update_app_id(self)
+        update_session(self)
+        update_homepage_source(self)
+        update_app_id(self)
         self.guest = Guest()
 
         self.request_session.cookies.set("sessionid", session_id)
 
         if not self.is_authenticated():
-            raise exceptions.AuthenticationError("Either User ID or Session ID is not valid.")
+            raise AuthenticationError("Either User ID or Session ID is not valid.")
 
     def update_homepage_source(self):
         temp_homepage_source = requests.get("https://www.instagram.com/").text.strip()
 
         if temp_homepage_source != "":
             self.homepage_source = temp_homepage_source
         else:
-            raise exceptions.NetworkError("Couldn't load instagram homepage.")
+            raise NetworkError("Couldn't load instagram homepage.")
 
     def is_authenticated(self):
-        commons.refresh_csrf_token(self)
+        refresh_csrf_token(self)
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
             "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
             "sec-ch-ua-mobile": "?0",
@@ -66,15 +66,15 @@
             http_response.json()
             return True
         except JSONDecodeError:
             return False
 
     def follow_user_id(self, user_id: str | int):
         user_id = str(user_id).strip()
-        commons.refresh_csrf_token(self)
+        refresh_csrf_token(self)
         random_referer_username = "".join(random.choices(string.ascii_lowercase, k=6))
         body_json = {
             "container_module": "profile",
             "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
             "user_id": user_id
         }
         request_headers = {
```

### Comparing `ensta-0.6/ensta.egg-info/PKG-INFO` & `ensta-0.7/ensta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 0.6
+Version: 0.7
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v0.1.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
```

### Comparing `ensta-0.6/setup.py` & `ensta-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="ensta",
     packages=["ensta"],
-    version="0.6",
+    version="0.7",
     license="MIT",
     description="Simple & Up-to-date Instagram API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
```

