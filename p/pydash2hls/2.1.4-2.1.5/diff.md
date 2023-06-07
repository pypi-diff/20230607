# Comparing `tmp/pydash2hls-2.1.4.tar.gz` & `tmp/pydash2hls-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash2hls-2.1.4.tar", last modified: Tue Jun  6 18:37:39 2023, max compression
+gzip compressed data, was "pydash2hls-2.1.5.tar", last modified: Wed Jun  7 11:32:08 2023, max compression
```

## Comparing `pydash2hls-2.1.4.tar` & `pydash2hls-2.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 18:37:39.335865 pydash2hls-2.1.4/
--rw-rw-rw-   0        0        0    35823 2023-06-06 11:16:08.000000 pydash2hls-2.1.4/LICENSE
--rw-rw-rw-   0        0        0     3389 2023-06-06 18:37:39.335865 pydash2hls-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2463 2023-06-06 11:16:08.000000 pydash2hls-2.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 18:37:39.303737 pydash2hls-2.1.4/pydash2hls/
--rw-rw-rw-   0        0        0       59 2023-06-06 18:22:52.000000 pydash2hls-2.1.4/pydash2hls/__init__.py
--rw-rw-rw-   0        0        0    11315 2023-06-06 18:21:39.000000 pydash2hls-2.1.4/pydash2hls/converter.py
--rw-rw-rw-   0        0        0      469 2023-06-06 11:16:08.000000 pydash2hls-2.1.4/pydash2hls/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-06 18:37:39.335865 pydash2hls-2.1.4/pydash2hls.egg-info/
--rw-rw-rw-   0        0        0     3389 2023-06-06 18:37:39.000000 pydash2hls-2.1.4/pydash2hls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-06 18:37:39.000000 pydash2hls-2.1.4/pydash2hls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 18:37:39.000000 pydash2hls-2.1.4/pydash2hls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-06 18:37:39.000000 pydash2hls-2.1.4/pydash2hls.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 18:37:39.000000 pydash2hls-2.1.4/pydash2hls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 18:37:39.335865 pydash2hls-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1152 2023-06-06 17:59:10.000000 pydash2hls-2.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 18:37:39.335865 pydash2hls-2.1.4/test/
--rw-rw-rw-   0        0        0      865 2023-06-06 18:20:13.000000 pydash2hls-2.1.4/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:32:08.840283 pydash2hls-2.1.5/
+-rw-rw-rw-   0        0        0    35823 2023-06-07 10:10:12.000000 pydash2hls-2.1.5/LICENSE
+-rw-rw-rw-   0        0        0     3389 2023-06-07 11:32:08.840283 pydash2hls-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2463 2023-06-07 10:10:12.000000 pydash2hls-2.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 11:32:08.820124 pydash2hls-2.1.5/pydash2hls/
+-rw-rw-rw-   0        0        0       59 2023-06-07 10:57:16.000000 pydash2hls-2.1.5/pydash2hls/__init__.py
+-rw-rw-rw-   0        0        0    11896 2023-06-07 11:07:38.000000 pydash2hls-2.1.5/pydash2hls/converter.py
+-rw-rw-rw-   0        0        0      469 2023-06-07 10:10:12.000000 pydash2hls-2.1.5/pydash2hls/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:32:08.838293 pydash2hls-2.1.5/pydash2hls.egg-info/
+-rw-rw-rw-   0        0        0     3389 2023-06-07 11:32:08.000000 pydash2hls-2.1.5/pydash2hls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-07 11:32:08.000000 pydash2hls-2.1.5/pydash2hls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 11:32:08.000000 pydash2hls-2.1.5/pydash2hls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-07 11:32:08.000000 pydash2hls-2.1.5/pydash2hls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 11:32:08.000000 pydash2hls-2.1.5/pydash2hls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 11:32:08.840283 pydash2hls-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-06-07 11:30:23.000000 pydash2hls-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:32:08.839284 pydash2hls-2.1.5/test/
+-rw-rw-rw-   0        0        0      865 2023-06-07 10:10:12.000000 pydash2hls-2.1.5/test/test.py
```

### Comparing `pydash2hls-2.1.4/LICENSE` & `pydash2hls-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydash2hls-2.1.4/PKG-INFO` & `pydash2hls-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash2hls
-Version: 2.1.4
+Version: 2.1.5
 Summary: Python library for converting DASH manifest files to HLS format.
 Home-page: https://github.com/hyugogirubato/pydash2hls
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: manifest,hls,m3u8,dash
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydash2hls-2.1.4/README.md` & `pydash2hls-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pydash2hls-2.1.4/pydash2hls/converter.py` & `pydash2hls-2.1.5/pydash2hls/converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
 import base64
+import re
+from collections import Counter
 from pathlib import Path
 from typing import Optional
 
 import requests
 import xmltodict
 
 from pydash2hls.exceptions import InvalidFileContent, InvalidPath, InvalidProfile, MissingRemoteUrl
@@ -18,16 +20,23 @@
             "widevine": "cenc:pssh",
             "playready": "mspr:pro",
             "license": "ms:laurl"
         }
 
         for key, value in keys.items():
             if value in protection:
+                scheme_id = re.sub(r'[^0-9a-f]', "", protection.get("@schemeIdUri", "").replace("urn:uuid:", "").lower())
+                if scheme_id == "edef8ba979d64acea3c827dcd51d21ed":
+                    key = "widevine"
+                elif scheme_id == "9a04f07998404286ab92e65be0885f95":
+                    key = "playready"
+
                 item = protection[value]
-                drm[key] = item if isinstance(item, str) else item["#text"]
+                item = item if isinstance(item, str) else item["#text"]
+                drm[key] = item.lower() if key == "kid" else item
     return drm
 
 
 class Converter:
 
     def __init__(self, mdp_srt: str, mdp_dict: dict, url: str = None):
         self.mdp_srt = mdp_srt
@@ -86,23 +95,23 @@
 
                 # Representations
                 representations = adaptation["Representation"]
                 representations = representations if isinstance(representations, list) else [representations]
 
                 for representation in representations:
                     mime_type = self._get_key(adaptation, representation, "@mimeType") or ("video/mp4" if "avc" in representation["@codecs"] else "audio/m4a")
-                    start_with_sap = self._get_key(adaptation, representation, "@startWithSAP") or "1"
+                    start_with_sap = (self._get_key(adaptation, representation, "@startWithSAP") or "1") == "1"
                     if "video" not in mime_type and "audio" not in mime_type:
                         continue
 
                     profile = {
-                        "id": representation["@id"],
+                        "id": representation.get("@id") or adaptation.get("@id"),
                         "mimeType": mime_type,
-                        "codecs": representation["@codecs"],
-                        "bandwidth": int(representation["@bandwidth"]),
+                        "codecs": representation.get("@codecs") or adaptation.get("@codecs"),
+                        "bandwidth": int(representation.get("@bandwidth") or adaptation.get("@bandwidth")),
                         "startWithSAP": start_with_sap
                     }
                     if "audio" in profile["mimeType"] or "@audioSamplingRate" in representation:
                         profile["audioSamplingRate"] = representation.get("@audioSamplingRate")
                     else:
                         profile["width"] = int(representation["@width"])
                         profile["height"] = int(representation["@height"])
@@ -206,20 +215,20 @@
                         if not self.profiles[index]["drm"]:
                             self.profiles[index]["drm"] = profile["drm"]
                         self.profiles[index]["fragments"] = profile["fragments"]
 
     def build_hls(self, profile_id: str, licence: str = None) -> str:
         profile = self._get_profile(profile_id)
         sequence = 0 if len(profile["fragments"]) == 1 else 1
-        duration = int(max([float(f["extinf"]) for f in profile["fragments"]]))
+        duration, _ = Counter([float(f["extinf"]) for f in profile["fragments"]]).most_common(1)[0]
         hls = [
             "#EXTM3U",
             "#EXT-X-VERSION:6",
             f"#EXT-X-MEDIA-SEQUENCE:{sequence}",
-            f"#EXT-X-TARGETDURATION:{duration}",
+            f"#EXT-X-TARGETDURATION:{int(duration)}",
             "#EXT-X-PLAYLIST-TYPE:VOD",
             "#EXT-X-ALLOW-CACHE:YES",
         ]
 
         if licence:
             kid, key = licence.split(":")
             key_uri = "data:text/plain;base64," + base64.b64encode(bytes.fromhex(key)).decode("utf-8")
```

### Comparing `pydash2hls-2.1.4/pydash2hls.egg-info/PKG-INFO` & `pydash2hls-2.1.5/pydash2hls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash2hls
-Version: 2.1.4
+Version: 2.1.5
 Summary: Python library for converting DASH manifest files to HLS format.
 Home-page: https://github.com/hyugogirubato/pydash2hls
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: manifest,hls,m3u8,dash
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydash2hls-2.1.4/setup.py` & `pydash2hls-2.1.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pydash2hls",
-    version="2.1.4",
+    version="2.1.5",
     author="hyugogirubato",
     author_email="hyugogirubato@gmail.com",
     description="Python library for converting DASH manifest files to HLS format.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hyugogirubato/pydash2hls",
     packages=find_packages(),
     license="GPL-3.0-only",
-    keywords=["manifest", "hls", "m3u8", "dash"],
+    keywords=[
+        "manifest",
+        "hls",
+        "m3u8",
+        "dash"
+    ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Utilities"
     ],
-    install_requires=["requests", "xmltodict"],
+    install_requires=[
+        "requests",
+        "xmltodict"
+    ],
     python_requires=">=3.7"
 )
```

### Comparing `pydash2hls-2.1.4/test/test.py` & `pydash2hls-2.1.5/test/test.py`

 * *Files identical despite different names*

