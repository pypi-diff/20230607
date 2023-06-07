# Comparing `tmp/twitter-api-client-0.9.3.tar.gz` & `tmp/twitter-api-client-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.9.3.tar", last modified: Wed Jun  7 19:13:36 2023, max compression
+gzip compressed data, was "twitter-api-client-0.9.4.tar", last modified: Wed Jun  7 20:58:11 2023, max compression
```

## Comparing `twitter-api-client-0.9.3.tar` & `twitter-api-client-0.9.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:13:36.051248 twitter-api-client-0.9.3/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.3/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 19:13:36.051248 twitter-api-client-0.9.3/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-07 19:13:36.051248 twitter-api-client-0.9.3/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-07 19:13:05.000000 twitter-api-client-0.9.3/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:13:36.051248 twitter-api-client-0.9.3/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.3/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    23528 2023-06-07 19:13:05.000000 twitter-api-client-0.9.3/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28698 2023-06-07 18:37:17.000000 twitter-api-client-0.9.3/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7382 2023-06-07 19:06:40.000000 twitter-api-client-0.9.3/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    33429 2023-06-07 19:04:37.000000 twitter-api-client-0.9.3/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     6127 2023-06-07 19:13:05.000000 twitter-api-client-0.9.3/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-07 19:04:37.000000 twitter-api-client-0.9.3/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:13:36.051248 twitter-api-client-0.9.3/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 19:13:36.000000 twitter-api-client-0.9.3/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-07 19:13:36.000000 twitter-api-client-0.9.3/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-07 19:13:36.000000 twitter-api-client-0.9.3/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-07 19:13:36.000000 twitter-api-client-0.9.3/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-07 19:13:36.000000 twitter-api-client-0.9.3/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 20:58:11.738655 twitter-api-client-0.9.4/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.4/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 20:58:11.738655 twitter-api-client-0.9.4/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-07 20:58:11.739655 twitter-api-client-0.9.4/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-07 20:57:15.000000 twitter-api-client-0.9.4/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 20:58:11.738655 twitter-api-client-0.9.4/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.4/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    23528 2023-06-07 19:13:05.000000 twitter-api-client-0.9.4/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28740 2023-06-07 20:57:15.000000 twitter-api-client-0.9.4/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7382 2023-06-07 19:06:40.000000 twitter-api-client-0.9.4/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    33428 2023-06-07 20:57:15.000000 twitter-api-client-0.9.4/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     6127 2023-06-07 19:13:05.000000 twitter-api-client-0.9.4/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-07 19:04:37.000000 twitter-api-client-0.9.4/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 20:58:11.738655 twitter-api-client-0.9.4/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 20:58:11.000000 twitter-api-client-0.9.4/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-07 20:58:11.000000 twitter-api-client-0.9.4/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-07 20:58:11.000000 twitter-api-client-0.9.4/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-07 20:58:11.000000 twitter-api-client-0.9.4/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-07 20:58:11.000000 twitter-api-client-0.9.4/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.9.3/LICENSE` & `twitter-api-client-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.3/PKG-INFO` & `twitter-api-client-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.3
+Version: 0.9.4
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.9.3/setup.py` & `twitter-api-client-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.9.3",
+    version="0.9.4",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
```

### Comparing `twitter-api-client-0.9.3/twitter/account.py` & `twitter-api-client-0.9.4/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.3/twitter/constants.py` & `twitter-api-client-0.9.4/twitter/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 ID_MAP = {
     'Followers': '^user-\d+$',
     'Following': '^user-\d+$',
     'UserTweets': '^tweet-\d+$',
     'Likes': '^tweet-\d+$',
     'UserMedia': '^tweet-\d+$',
+    'TweetResultByRestId': '^tweet-\d+$',
     'TweetsAndReplies': '^profile-conversation-\d+-tweet-\d+$',
     'TweetDetail': '^conversationthread-\d+-tweet-\d+$',  # if another key after tweet-\d+, it's an ad
     'Retweeters': '^user-\d+$',
     'Favoriters': '^user-\d+$'
 }
```

### Comparing `twitter-api-client-0.9.3/twitter/login.py` & `twitter-api-client-0.9.4/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.3/twitter/scraper.py` & `twitter-api-client-0.9.4/twitter/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,16 +558,16 @@
             res = []
             ids = set()
         else:
             try:
                 r = await self._query(client, operation, **kwargs)
                 initial_data = r.json()
                 res = [r]
-                ids = get_ids(initial_data, operation)
-                # ids = set(find_key(initial_data, 'rest_id'))  # todo
+                # ids = get_ids(initial_data, operation) # todo
+                ids = set(find_key(initial_data, 'rest_id'))
                 cursor = get_cursor(initial_data)
             except Exception as e:
                 self.logger.error('Failed to get initial pagination data', e)
                 return
         while (dups < DUP_LIMIT) and cursor:
             prev_len = len(ids)
             if prev_len >= limit:
@@ -575,16 +575,16 @@
             try:
                 r = await self._query(client, operation, cursor=cursor, **kwargs)
                 data = r.json()
             except Exception as e:
                 self.logger.error(f'Failed to get pagination data\n{e}')
                 return
             cursor = get_cursor(data)
-            ids |= get_ids(data, operation)
-            # ids |= set(find_key(data, 'rest_id')) # todo
+            # ids |= get_ids(data, operation) # todo
+            ids |= set(find_key(data, 'rest_id'))
             if self.debug:
                 self.logger.debug(f'Unique results: {len(ids)}\tcursor: {cursor}')
             if prev_len == len(ids):
                 dups += 1
             res.append(r)
         if is_resuming:
             return res, cursor
```

### Comparing `twitter-api-client-0.9.3/twitter/search.py` & `twitter-api-client-0.9.4/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.3/twitter/util.py` & `twitter-api-client-0.9.4/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.3/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.9.4/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.3
+Version: 0.9.4
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

