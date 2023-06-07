# Comparing `tmp/twitter-api-client-0.9.1.tar.gz` & `tmp/twitter-api-client-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.9.1.tar", last modified: Tue Jun  6 22:13:57 2023, max compression
+gzip compressed data, was "twitter-api-client-0.9.2.tar", last modified: Wed Jun  7 19:09:27 2023, max compression
```

## Comparing `twitter-api-client-0.9.1.tar` & `twitter-api-client-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 22:13:57.017467 twitter-api-client-0.9.1/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.1/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 22:13:57.017467 twitter-api-client-0.9.1/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-06 22:13:57.017467 twitter-api-client-0.9.1/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-06 22:13:31.000000 twitter-api-client-0.9.1/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 22:13:57.016467 twitter-api-client-0.9.1/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.1/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    23524 2023-06-06 19:05:18.000000 twitter-api-client-0.9.1/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28299 2023-06-06 19:05:18.000000 twitter-api-client-0.9.1/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.9.1/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    28285 2023-06-06 22:07:05.000000 twitter-api-client-0.9.1/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     6123 2023-06-06 19:05:18.000000 twitter-api-client-0.9.1/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9683 2023-06-06 20:42:23.000000 twitter-api-client-0.9.1/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 22:13:57.017467 twitter-api-client-0.9.1/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 22:13:57.000000 twitter-api-client-0.9.1/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-06 22:13:57.000000 twitter-api-client-0.9.1/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-06 22:13:57.000000 twitter-api-client-0.9.1/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-06 22:13:57.000000 twitter-api-client-0.9.1/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-06 22:13:57.000000 twitter-api-client-0.9.1/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:09:27.282779 twitter-api-client-0.9.2/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.2/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 19:09:27.281779 twitter-api-client-0.9.2/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-07 19:09:27.282779 twitter-api-client-0.9.2/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-07 19:04:37.000000 twitter-api-client-0.9.2/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:09:27.281779 twitter-api-client-0.9.2/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.2/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    23524 2023-06-06 19:05:18.000000 twitter-api-client-0.9.2/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28698 2023-06-07 18:37:17.000000 twitter-api-client-0.9.2/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7382 2023-06-07 19:06:40.000000 twitter-api-client-0.9.2/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    33429 2023-06-07 19:04:37.000000 twitter-api-client-0.9.2/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     6123 2023-06-06 19:05:18.000000 twitter-api-client-0.9.2/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-07 19:04:37.000000 twitter-api-client-0.9.2/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:09:27.281779 twitter-api-client-0.9.2/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 19:09:27.000000 twitter-api-client-0.9.2/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-07 19:09:27.000000 twitter-api-client-0.9.2/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-07 19:09:27.000000 twitter-api-client-0.9.2/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-07 19:09:27.000000 twitter-api-client-0.9.2/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-07 19:09:27.000000 twitter-api-client-0.9.2/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.9.1/LICENSE` & `twitter-api-client-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.1/PKG-INFO` & `twitter-api-client-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.1
+Version: 0.9.2
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.9.1/setup.py` & `twitter-api-client-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.9.1",
+    version="0.9.2",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
```

### Comparing `twitter-api-client-0.9.1/twitter/account.py` & `twitter-api-client-0.9.2/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.1/twitter/constants.py` & `twitter-api-client-0.9.2/twitter/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,26 @@
         LOGGER_NAME: {
             'handlers': ['console', 'file'],
             'level': 'DEBUG',
         }
     }
 }
 
+ID_MAP = {
+    'Followers': '^user-\d+$',
+    'Following': '^user-\d+$',
+    'UserTweets': '^tweet-\d+$',
+    'Likes': '^tweet-\d+$',
+    'UserMedia': '^tweet-\d+$',
+    'TweetsAndReplies': '^profile-conversation-\d+-tweet-\d+$',
+    'TweetDetail': '^conversationthread-\d+-tweet-\d+$',  # if another key after tweet-\d+, it's an ad
+    'Retweeters': '^user-\d+$',
+    'Favoriters': '^user-\d+$'
+}
+
 
 @dataclass
 class SpaceCategory:
     Top = 'Top'
     Live = 'Live'
     Upcoming = 'Upcoming'
```

### Comparing `twitter-api-client-0.9.1/twitter/login.py` & `twitter-api-client-0.9.2/twitter/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
-import time
 
 from httpx import Client
+
 from .constants import GREEN, YELLOW, RED, BOLD, RESET
 from .util import find_key  # ,get_confirmation_code, get_inbox, init_protonmail_session
 
 
 def update_token(client: Client, key: str, url: str, **kwargs) -> Client:
     caller_name = sys._getframe(1).f_code.co_name
     try:
@@ -158,21 +158,21 @@
             "password": password,
             "guest_token": None,
             "flow_token": None,
         },
         headers={
             'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
             'content-type': 'application/json',
-            'user-agent': 'Mozilla/5.0 (Linux; Android 11; Nokia G20) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.88 Mobile Safari/537.36',
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
             'x-twitter-active-user': 'yes',
             'x-twitter-client-language': 'en',
         })
 
     # client.protonmail = kwargs.get('protonmail')
 
     client = execute_login_flow(client)
-    if kwargs.get('debug', True):
+    if kwargs.get('debug'):
         if not client or client.cookies.get('flow_errors') == 'true':
             print(f'[{RED}error{RESET}] {BOLD}{username}{RESET} login failed')
         else:
             print(f'[{GREEN}success{RESET}] {BOLD}{username}{RESET} login success')
     return client
```

### Comparing `twitter-api-client-0.9.1/twitter/search.py` & `twitter-api-client-0.9.2/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.1/twitter/util.py` & `twitter-api-client-0.9.2/twitter/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from urllib.parse import urlsplit, urlencode, urlunsplit, parse_qs, quote
 
 import orjson
 # import protonmail
 from httpx import Response, Client
 
-from .constants import GREEN, MAGENTA, RED, RESET
+from .constants import GREEN, MAGENTA, RED, RESET, ID_MAP
 
 
 def init_session():
     client = Client(headers={
         'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
         'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
     }, follow_redirects=True)
@@ -200,14 +200,19 @@
         color = GREEN
     elif 300 <= status < 400:
         color = MAGENTA
     elif 400 <= status < 600:
         color = RED
     return f'[{color}{status}{RESET}]'
 
+
+def get_ids(data: list | dict, operation: tuple) -> set:
+    expr = ID_MAP[operation[-1]]
+    return {k for k in find_key(data, 'entryId') if re.search(expr, k)}
+
 # def init_protonmail_session(email: str, password: str) -> protonmail.api.Session:
 #     """
 #     Create an authenticated Proton Mail session
 #
 #     @param email: your email. Can also use username
 #     @param password: your password
 #     @return: Proton Mail Session object
```

### Comparing `twitter-api-client-0.9.1/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.9.2/twitter_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.1
+Version: 0.9.2
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

