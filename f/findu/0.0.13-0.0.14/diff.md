# Comparing `tmp/findu-0.0.13.tar.gz` & `tmp/findu-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findu-0.0.13.tar", max compression
+gzip compressed data, was "findu-0.0.14.tar", max compression
```

## Comparing `findu-0.0.13.tar` & `findu-0.0.14.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0      483 2023-06-07 04:32:01.441958 findu-0.0.13/findu/__init__.py
--rw-r--r--   0        0        0      562 2023-04-16 06:26:44.829145 findu-0.0.13/findu/__main__.py
--rw-r--r--   0        0        0    32712 2023-06-07 04:19:34.717509 findu-0.0.13/findu/findu.py
--rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.13/findu/findu2.py
--rw-r--r--   0        0        0     7211 2023-06-04 14:22:33.985163 findu-0.0.13/findu/jack.txt
--rw-r--r--   0        0        0     1363 2023-06-04 14:06:36.562095 findu-0.0.13/findu/markhoo.txt
--rw-r--r--   0        0        0     8894 2023-04-16 06:26:44.830142 findu-0.0.13/findu/notify.py
--rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.13/findu/resources/data.json
--rw-r--r--   0        0        0     3201 2023-04-16 06:26:44.832137 findu-0.0.13/findu/result.py
--rw-r--r--   0        0        0     9242 2023-04-16 06:26:44.834132 findu-0.0.13/findu/sites.py
--rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.13/findu/tests/__init__.py
--rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.13/findu/tests/all.py
--rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.13/findu/tests/base.py
--rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.13/findu/tests/test_multiple_usernames.py
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.13/findu/translations/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.13/findu/translations/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.13/findu/translations/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.13/LICENSE
--rw-r--r--   0        0        0     1594 2023-06-07 04:33:28.965360 findu-0.0.13/pyproject.toml
--rw-r--r--   0        0        0    10885 2023-06-04 14:32:59.022396 findu-0.0.13/README.md
--rw-r--r--   0        0        0    12314 1970-01-01 00:00:00.000000 findu-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0      483 2023-06-07 04:32:01.441958 findu-0.0.14/findu/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-07 04:38:01.851778 findu-0.0.14/findu/__main__.py
+-rw-r--r--   0        0        0    32739 2023-06-07 04:55:06.206294 findu-0.0.14/findu/findu.py
+-rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.14/findu/findu2.py
+-rw-r--r--   0        0        0     8895 2023-06-07 04:54:06.964355 findu-0.0.14/findu/notify.py
+-rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.14/findu/resources/data.json
+-rw-r--r--   0        0        0     3203 2023-06-07 04:54:23.272209 findu-0.0.14/findu/result.py
+-rw-r--r--   0        0        0     9244 2023-06-07 04:54:40.419398 findu-0.0.14/findu/sites.py
+-rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.14/findu/tests/__init__.py
+-rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.14/findu/tests/all.py
+-rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.14/findu/tests/base.py
+-rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.14/findu/tests/test_multiple_usernames.py
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.14/findu/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.14/findu/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.14/findu/translations/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.14/LICENSE
+-rw-r--r--   0        0        0     1594 2023-06-07 04:43:00.752822 findu-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0    10885 2023-06-04 14:32:59.022396 findu-0.0.14/README.md
+-rw-r--r--   0        0        0    12314 1970-01-01 00:00:00.000000 findu-0.0.14/PKG-INFO
```

### Comparing `findu-0.0.13/findu/findu.py` & `findu-0.0.14/findu/findu.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from time import monotonic
 
 import requests
 
 from requests_futures.sessions import FuturesSession
 from torrequest import TorRequest
-from result import QueryStatus
-from result import QueryResult
-from notify import QueryNotifyPrint
-from sites import SitesInformation
+from .result import QueryStatus
+from .result import QueryResult
+from .notify import QueryNotifyPrint
+from .sites import SitesInformation
 from colorama import init
 
 module_name = "Find U: Find Usernames Across Social Networks"
-__version__ = "0.0.11"
+__version__ = "0.0.14"
 
 
 class SherlockFuturesSession(FuturesSession):
     def request(self, method, url, hooks=None, *args, **kwargs):
         """Request URL.
 
         This extends the FuturesSession request method to calculate a response
@@ -567,27 +567,27 @@
 
     args = parser.parse_args()
 
     # If the user presses CTRL-C, exit gracefully without throwing errors
     signal.signal(signal.SIGINT, handler)
 
     # Check for newer version of Sherlock. If it exists, let the user know about it
-    try:
-        r = requests.get(
-            "https://raw.githubusercontent.com/sherlock-project/sherlock/master/sherlock/sherlock.py")
-
-        remote_version = str(re.findall('__version__ = "(.*)"', r.text)[0])
-        local_version = __version__
-
-        if remote_version != local_version:
-            print("Update Available!\n" +
-                  f"You are running version {local_version}. Version {remote_version} is available at https://github.com/sherlock-project/sherlock")
-
-    except Exception as error:
-        print(f"A problem occurred while checking for an update: {error}")
+    # try:
+    #     r = requests.get(
+    #         "https://raw.githubusercontent.com/sherlock-project/sherlock/master/sherlock/sherlock.py")
+    #
+    #     remote_version = str(re.findall('__version__ = "(.*)"', r.text)[0])
+    #     local_version = __version__
+    #
+    #     if remote_version != local_version:
+    #         print("Update Available!\n" +
+    #               f"You are running version {local_version}. Version {remote_version} is available at https://github.com/markhoo/findu")
+    #
+    # except Exception as error:
+    #     print(f"A problem occurred while checking for an update: {error}")
 
     # Argument check
     # TODO regex check on args.proxy
     if args.tor and (args.proxy is not None):
         raise Exception("Tor and Proxy cannot be set at the same time.")
 
     # Make prompts
```

### Comparing `findu-0.0.13/findu/findu2.py` & `findu-0.0.14/findu/findu2.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.13/findu/notify.py` & `findu-0.0.14/findu/notify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Sherlock Notify Module
 
 This module defines the objects for notifying the caller about the
 results of queries.
 """
-from result import QueryStatus
+from .result import QueryStatus
 from colorama import Fore, Style
 import webbrowser
 
 # Global variable to count the number of results.
 globvar = 0
```

### Comparing `findu-0.0.13/findu/resources/data.json` & `findu-0.0.14/findu/resources/data.json`

 * *Files identical despite different names*

### Comparing `findu-0.0.13/findu/result.py` & `findu-0.0.14/findu/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self                   -- This object.
 
         Return Value:
         Nicely formatted string to get information about this object.
         """
         return self.value
 
+
 class QueryResult():
     """Query Result Object.
 
     Describes result of query about a given username.
     """
     def __init__(self, username, site_name, site_url_user, status,
                  query_time=None, context=None):
```

### Comparing `findu-0.0.13/findu/sites.py` & `findu-0.0.14/findu/sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 This module supports storing information about websites.
 This is the raw data that will be used to search for usernames.
 """
 import json
 import requests
 import secrets
 
+
 class SiteInformation:
     def __init__(self, name, url_home, url_username_format, username_claimed,
                 information, is_nsfw, username_unclaimed=secrets.token_urlsafe(10)):
         """Create Site Information Object.
 
         Contains information about a specific website.
```

### Comparing `findu-0.0.13/findu/tests/all.py` & `findu-0.0.14/findu/tests/all.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.13/findu/tests/base.py` & `findu-0.0.14/findu/tests/base.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.13/findu/tests/test_multiple_usernames.py` & `findu-0.0.14/findu/tests/test_multiple_usernames.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.13/LICENSE` & `findu-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `findu-0.0.13/pyproject.toml` & `findu-0.0.14/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findu"
-version = "0.0.13"
+version = "0.0.14"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/findu"
 repository = "https://github.com/MarkHoo/findu"
 classifiers = [
```

### Comparing `findu-0.0.13/README.md` & `findu-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `findu-0.0.13/PKG-INFO` & `findu-0.0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findu
-Version: 0.0.13
+Version: 0.0.14
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/findu
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

