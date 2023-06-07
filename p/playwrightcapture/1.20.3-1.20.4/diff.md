# Comparing `tmp/playwrightcapture-1.20.3.tar.gz` & `tmp/playwrightcapture-1.20.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.20.3.tar", max compression
+gzip compressed data, was "playwrightcapture-1.20.4.tar", max compression
```

## Comparing `playwrightcapture-1.20.3.tar` & `playwrightcapture-1.20.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.3/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.3/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.3/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    36341 2023-06-06 14:46:46.974833 playwrightcapture-1.20.3/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.3/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.3/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.3/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1809 2023-06-06 14:57:04.241971 playwrightcapture-1.20.3/pyproject.toml
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 playwrightcapture-1.20.3/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.4/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.4/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.4/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    36479 2023-06-07 12:40:02.326124 playwrightcapture-1.20.4/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.4/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.4/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.4/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1828 2023-06-07 12:42:00.258731 playwrightcapture-1.20.4/pyproject.toml
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.4/PKG-INFO
```

### Comparing `playwrightcapture-1.20.3/LICENSE` & `playwrightcapture-1.20.4/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.3/README.md` & `playwrightcapture-1.20.4/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.3/playwrightcapture/capture.py` & `playwrightcapture-1.20.4/playwrightcapture/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,34 +166,36 @@
 
     @http_credentials.setter
     def http_credentials(self, credentials: Optional[Dict[str, str]]) -> None:
         if not credentials:
             return
         if 'username' in credentials and 'password' in credentials:
             self._http_credentials = {'username': credentials['username'],
-                                      'password': credentials['password'],
-                                      'origin': credentials.get('origin')}
+                                      'password': credentials['password']}
+            if 'origin' in credentials:
+                self._http_credentials['origin'] = credentials['origin']
         else:
             raise InvalidPlaywrightParameter(f'At least a username and a password are required in the credentials: {credentials}')
 
     def set_http_credentials(self, username: str, password: str, origin: Optional[str]=None) -> None:
         self._http_credentials = {'username': username, 'password': password, 'origin': origin}
 
     @property
     def geolocation(self) -> 'Geolocation':
         return self._geolocation
 
     @geolocation.setter
-    def geolocation(self, geolocation: Optional[Dict[str, float]]) -> None:
+    def geolocation(self, geolocation: Optional[Dict[str, Union[str, int, float]]]) -> None:
         if not geolocation:
             return
         if 'latitude' in geolocation and 'longitude' in geolocation:
-            self._geolocation = {'latitude': geolocation['latitude'],
-                                 'longitude': geolocation['longitude'],
-                                 'accuracy': geolocation.get('accuracy')}
+            self._geolocation = {'latitude': float(geolocation['latitude']),
+                                 'longitude': float(geolocation['longitude'])}
+            if 'accuracy' in geolocation:
+                self._geolocation['accuracy'] = float(geolocation['accuracy'])
         else:
             raise InvalidPlaywrightParameter(f'At least a latitude and a longitude are required in the geolocation: {geolocation}')
 
     @property
     def cookies(self) -> List['SetCookieParam']:
         return self._cookies
 
@@ -283,19 +285,19 @@
             self._headers[name] = value
 
     @property
     def viewport(self) -> Optional['ViewportSize']:
         return self._viewport
 
     @viewport.setter
-    def viewport(self, viewport: Optional[Dict[str, int]]) -> None:
+    def viewport(self, viewport: Optional[Dict[str, Union[str, int]]]) -> None:
         if not viewport:
             return
         if 'width' in viewport and 'height' in viewport:
-            self._viewport = {'width': viewport['width'], 'height': viewport['height']}
+            self._viewport = {'width': int(viewport['width']), 'height': int(viewport['height'])}
         else:
             raise InvalidPlaywrightParameter(f'A viewport must have a height and a width - {viewport}')
 
     @property
     def user_agent(self) -> str:
         return self._user_agent
```

### Comparing `playwrightcapture-1.20.3/playwrightcapture/helpers.py` & `playwrightcapture-1.20.4/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.3/pyproject.toml` & `playwrightcapture-1.20.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.20.3"
+version = "1.20.4"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -26,14 +26,15 @@
 beautifulsoup4 = "^4.12.2"
 w3lib = "^2.1.1"
 lxml = "^4.9.2"
 requests = {version = "^2.31.0", optional = true}
 pydub = {version = "^0.25.1", optional = true}
 SpeechRecognition = {version = "^3.10.0", optional = true}
 pytz = {"version" = "^2023.3", python = "<3.9"}
+tzdata = "^2023.3"
 
 [tool.poetry.extras]
 recaptcha = ["requests", "pydub", "SpeechRecognition"]
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `playwrightcapture-1.20.3/PKG-INFO` & `playwrightcapture-1.20.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.20.3
+Version: 1.20.4
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -23,14 +23,15 @@
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: playwright (>=1.34.0,<2.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "recaptcha"
 Requires-Dist: pytz (>=2023.3,<2024.0) ; python_version < "3.9"
 Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "recaptcha"
+Requires-Dist: tzdata (>=2023.3,<2024.0)
 Requires-Dist: w3lib (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/Lookyloo/PlaywrightCapture
 Description-Content-Type: text/markdown
 
 # Playwright Capture
 
 Simple replacement for [splash](https://github.com/scrapinghub/splash) using [playwright](https://github.com/microsoft/playwright-python).
```

