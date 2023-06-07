# Comparing `tmp/twint_fork-2.5.1.tar.gz` & `tmp/twint_fork-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twint_fork-2.5.1.tar", last modified: Wed May 10 05:07:37 2023, max compression
+gzip compressed data, was "twint_fork-2.5.2.tar", last modified: Wed Jun  7 09:02:12 2023, max compression
```

## Comparing `twint_fork-2.5.1.tar` & `twint_fork-2.5.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-10 05:07:37.508225 twint_fork-2.5.1/
--rw-r--r--   0 hyi        (502) staff       (20)     1071 2023-03-22 13:37:09.000000 twint_fork-2.5.1/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)       26 2023-03-22 13:37:09.000000 twint_fork-2.5.1/MANIFEST.in
--rw-r--r--   0 hyi        (502) staff       (20)     7665 2023-05-10 05:07:37.507943 twint_fork-2.5.1/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     6853 2023-04-26 08:12:43.000000 twint_fork-2.5.1/README.md
--rw-r--r--   0 hyi        (502) staff       (20)       38 2023-05-10 05:07:37.508269 twint_fork-2.5.1/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)     1815 2023-05-10 05:07:28.000000 twint_fork-2.5.1/setup.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-10 05:07:37.501821 twint_fork-2.5.1/twint/
--rw-r--r--   0 hyi        (502) staff       (20)      808 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       61 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)       64 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/__version__.py
--rw-r--r--   0 hyi        (502) staff       (20)    15324 2023-04-26 06:33:01.000000 twint_fork-2.5.1/twint/cli.py
--rw-r--r--   0 hyi        (502) staff       (20)     2513 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/config.py
--rw-r--r--   0 hyi        (502) staff       (20)     1080 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/datelock.py
--rw-r--r--   0 hyi        (502) staff       (20)     4001 2023-04-26 14:18:09.000000 twint_fork-2.5.1/twint/feed.py
--rw-r--r--   0 hyi        (502) staff       (20)     4464 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/format.py
--rw-r--r--   0 hyi        (502) staff       (20)    11838 2023-04-26 00:44:20.000000 twint_fork-2.5.1/twint/get.py
--rw-r--r--   0 hyi        (502) staff       (20)     8168 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/output.py
--rw-r--r--   0 hyi        (502) staff       (20)    19377 2023-04-26 14:17:01.000000 twint_fork-2.5.1/twint/run.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-10 05:07:37.504830 twint_fork-2.5.1/twint/storage/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2023-03-22 13:37:09.000000 twint_fork-2.5.1/twint/storage/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)    11197 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/storage/db.py
--rw-r--r--   0 hyi        (502) staff       (20)    13379 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/storage/elasticsearch.py
--rw-r--r--   0 hyi        (502) staff       (20)     6307 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/storage/panda.py
--rw-r--r--   0 hyi        (502) staff       (20)     2161 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/storage/write.py
--rw-r--r--   0 hyi        (502) staff       (20)     3493 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/storage/write_meta.py
--rw-r--r--   0 hyi        (502) staff       (20)     3937 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/token.py
--rw-r--r--   0 hyi        (502) staff       (20)     5533 2023-04-25 13:25:39.000000 twint_fork-2.5.1/twint/tweet.py
--rw-r--r--   0 hyi        (502) staff       (20)     5660 2023-04-26 14:18:30.000000 twint_fork-2.5.1/twint/url.py
--rw-r--r--   0 hyi        (502) staff       (20)     1285 2023-04-26 00:44:03.000000 twint_fork-2.5.1/twint/user.py
--rw-r--r--   0 hyi        (502) staff       (20)      622 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/verbose.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-10 05:07:37.507343 twint_fork-2.5.1/twint_fork.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)     7665 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      645 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)       62 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       51 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)      142 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)        6 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/top_level.txt
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-06-07 09:02:12.433922 twint_fork-2.5.2/
+-rw-r--r--   0 hyi        (502) staff       (20)     1071 2023-03-22 13:37:09.000000 twint_fork-2.5.2/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)       26 2023-03-22 13:37:09.000000 twint_fork-2.5.2/MANIFEST.in
+-rw-r--r--   0 hyi        (502) staff       (20)     7665 2023-06-07 09:02:12.433724 twint_fork-2.5.2/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     6853 2023-04-26 08:12:43.000000 twint_fork-2.5.2/README.md
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2023-06-07 09:02:12.433973 twint_fork-2.5.2/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)     1815 2023-06-07 09:01:59.000000 twint_fork-2.5.2/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-06-07 09:02:12.429511 twint_fork-2.5.2/twint/
+-rw-r--r--   0 hyi        (502) staff       (20)      808 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       61 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       64 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/__version__.py
+-rw-r--r--   0 hyi        (502) staff       (20)    15324 2023-04-26 06:33:01.000000 twint_fork-2.5.2/twint/cli.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2513 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/config.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1080 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/datelock.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4000 2023-06-07 09:01:42.000000 twint_fork-2.5.2/twint/feed.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4464 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/format.py
+-rw-r--r--   0 hyi        (502) staff       (20)    11838 2023-04-26 00:44:20.000000 twint_fork-2.5.2/twint/get.py
+-rw-r--r--   0 hyi        (502) staff       (20)     8168 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/output.py
+-rw-r--r--   0 hyi        (502) staff       (20)    19339 2023-05-15 04:57:25.000000 twint_fork-2.5.2/twint/run.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-06-07 09:02:12.431445 twint_fork-2.5.2/twint/storage/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2023-03-22 13:37:09.000000 twint_fork-2.5.2/twint/storage/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)    11197 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/storage/db.py
+-rw-r--r--   0 hyi        (502) staff       (20)    13379 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/storage/elasticsearch.py
+-rw-r--r--   0 hyi        (502) staff       (20)     6307 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/storage/panda.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2161 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/storage/write.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3493 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/storage/write_meta.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3937 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/token.py
+-rw-r--r--   0 hyi        (502) staff       (20)     5533 2023-04-25 13:25:39.000000 twint_fork-2.5.2/twint/tweet.py
+-rw-r--r--   0 hyi        (502) staff       (20)     5610 2023-06-07 06:06:54.000000 twint_fork-2.5.2/twint/url.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1285 2023-04-26 00:44:03.000000 twint_fork-2.5.2/twint/user.py
+-rw-r--r--   0 hyi        (502) staff       (20)      622 2023-04-20 09:29:26.000000 twint_fork-2.5.2/twint/verbose.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-06-07 09:02:12.433463 twint_fork-2.5.2/twint_fork.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)     7665 2023-06-07 09:02:12.000000 twint_fork-2.5.2/twint_fork.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      645 2023-06-07 09:02:12.000000 twint_fork-2.5.2/twint_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       62 2023-06-07 09:02:12.000000 twint_fork-2.5.2/twint_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       51 2023-06-07 09:02:12.000000 twint_fork-2.5.2/twint_fork.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)      142 2023-06-07 09:02:12.000000 twint_fork-2.5.2/twint_fork.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        6 2023-06-07 09:02:12.000000 twint_fork-2.5.2/twint_fork.egg-info/top_level.txt
```

### Comparing `twint_fork-2.5.1/LICENSE` & `twint_fork-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/PKG-INFO` & `twint_fork-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twint_fork
-Version: 2.5.1
+Version: 2.5.2
 Summary: An advanced Twitter scraping & OSINT tool.
 Home-page: https://github.com/yihong0618/twint
 Author: Cody Zacharias, yihong0618
 Author-email: codyzacharias@pm.me, zouzou0208@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `twint_fork-2.5.1/README.md` & `twint_fork-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/setup.py` & `twint_fork-2.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
 setup(
     name=NAME,
-    version="2.5.1",
+    version="2.5.2",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
```

### Comparing `twint_fork-2.5.1/twint/__init__.py` & `twint_fork-2.5.2/twint/__init__.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/cli.py` & `twint_fork-2.5.2/twint/cli.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/config.py` & `twint_fork-2.5.2/twint/config.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/datelock.py` & `twint_fork-2.5.2/twint/datelock.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/feed.py` & `twint_fork-2.5.2/twint/feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 class NoMoreTweetsException(Exception):
     def __init__(self, msg):
         super().__init__(msg)
 
 
 def Follow(response):
-
     follows = loads(response)
     follow = follows["users"]
     logme.debug(__name__ + ":Follow")
     cursor = follows["next_cursor_str"]
 
     return follow, cursor
```

### Comparing `twint_fork-2.5.1/twint/format.py` & `twint_fork-2.5.2/twint/format.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/get.py` & `twint_fork-2.5.2/twint/get.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/output.py` & `twint_fork-2.5.2/twint/output.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/run.py` & `twint_fork-2.5.2/twint/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
                             time.sleep(1)
                         if favorite_err_cnt == 5:
                             print("Favorite page could not be fetched")
                     if not self.count % 40:
                         time.sleep(5)
                 elif self.config.Followers or self.config.Following:
                     self.feed, self.init = feed.Follow(response)
-                    print(self.count)
                     if not self.count % 40:
                         time.sleep(5)
                 elif self.config.Profile or self.config.TwitterSearch:
                     try:
                         # track the max_id if we need to continue
                         # ticky to make slef.feed to empty
                         # TODO
```

### Comparing `twint_fork-2.5.1/twint/storage/db.py` & `twint_fork-2.5.2/twint/storage/db.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/storage/elasticsearch.py` & `twint_fork-2.5.2/twint/storage/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/storage/panda.py` & `twint_fork-2.5.2/twint/storage/panda.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/storage/write.py` & `twint_fork-2.5.2/twint/storage/write.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/storage/write_meta.py` & `twint_fork-2.5.2/twint/storage/write_meta.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/token.py` & `twint_fork-2.5.2/twint/token.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/tweet.py` & `twint_fork-2.5.2/twint/tweet.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/url.py` & `twint_fork-2.5.2/twint/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import datetime
 from sys import platform
 import logging as logme
 from urllib.parse import urlencode
 from urllib.parse import quote
 
 mobile = "https://mobile.twitter.com"
-base = "https://api.twitter.com/2/search/adaptive.json"
 base = "https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name"
 
 
 def _sanitizeQuery(_url, params):
     _serialQuery = ""
     _serialQuery = urlencode(params, quote_via=quote)
     _serialQuery = _url + "?" + _serialQuery
@@ -69,25 +68,26 @@
 
 async def Search(config, init):
     logme.debug(__name__ + ":Search")
     url = base
     tweet_count = 100 if not config.Limit else config.Limit
     q = ""
     params = [
+        ("from", config.Username),
         ("include_can_media_tag", "1"),
         ("include_ext_alt_text", "true"),
         ("include_quote_count", "true"),
         ("include_reply_count", "1"),
         ("tweet_mode", "extended"),
         ("include_entities", "true"),
         ("include_user_entities", "true"),
         ("include_ext_media_availability", "true"),
         ("send_error_codes", "true"),
         ("simple_quoted_tweet", "true"),
-        ("count", tweet_count),
+        ("count", 99),
         ("query_source", "typed_query"),
         ("spelling_corrections", "1"),
         ("ext", "mediaStats%2ChighlightedLabel"),
         (
             "tweet_search_mode",
             "live",
         ),  # this can be handled better, maybe take an argument and set it then
@@ -125,17 +125,17 @@
         q += " exclude:links"
     if config.Source:
         q += f' source:"{config.Source}"'
     q = q.strip()
     params.append(("q", q))
     _serialQuery = _sanitizeQuery(url, params)
     if init != -1:
-        url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={config.Username}&count=200&max_id={init}"
+        url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={config.Username}&max_id={init}"
     else:
-        url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={config.Username}&count=200"
+        url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={config.Username}"
     return url, params, _serialQuery
 
 
 def SearchProfile(config, init=None):
     logme.debug(__name__ + ":SearchProfile")
     _url = "https://api.twitter.com/2/timeline/profile/{user_id}.json".format(
         user_id=config.User_id
```

### Comparing `twint_fork-2.5.1/twint/user.py` & `twint_fork-2.5.2/twint/user.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint/verbose.py` & `twint_fork-2.5.2/twint/verbose.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.1/twint_fork.egg-info/PKG-INFO` & `twint_fork-2.5.2/twint_fork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twint-fork
-Version: 2.5.1
+Version: 2.5.2
 Summary: An advanced Twitter scraping & OSINT tool.
 Home-page: https://github.com/yihong0618/twint
 Author: Cody Zacharias, yihong0618
 Author-email: codyzacharias@pm.me, zouzou0208@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `twint_fork-2.5.1/twint_fork.egg-info/SOURCES.txt` & `twint_fork-2.5.2/twint_fork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

