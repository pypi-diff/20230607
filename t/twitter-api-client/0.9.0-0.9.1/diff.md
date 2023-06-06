# Comparing `tmp/twitter-api-client-0.9.0.tar.gz` & `tmp/twitter-api-client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.9.0.tar", last modified: Tue Jun  6 20:45:14 2023, max compression
+gzip compressed data, was "twitter-api-client-0.9.1.tar", last modified: Tue Jun  6 22:13:57 2023, max compression
```

## Comparing `twitter-api-client-0.9.0.tar` & `twitter-api-client-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 20:45:14.449000 twitter-api-client-0.9.0/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.0/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 20:45:14.449000 twitter-api-client-0.9.0/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-06 20:45:14.449000 twitter-api-client-0.9.0/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-06 20:43:37.000000 twitter-api-client-0.9.0/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 20:45:14.448000 twitter-api-client-0.9.0/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.0/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    23524 2023-06-06 19:05:18.000000 twitter-api-client-0.9.0/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28299 2023-06-06 19:05:18.000000 twitter-api-client-0.9.0/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.9.0/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    28214 2023-06-06 20:39:28.000000 twitter-api-client-0.9.0/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     6123 2023-06-06 19:05:18.000000 twitter-api-client-0.9.0/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9683 2023-06-06 20:42:23.000000 twitter-api-client-0.9.0/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 20:45:14.449000 twitter-api-client-0.9.0/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 20:45:14.000000 twitter-api-client-0.9.0/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-06 20:45:14.000000 twitter-api-client-0.9.0/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-06 20:45:14.000000 twitter-api-client-0.9.0/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-06 20:45:14.000000 twitter-api-client-0.9.0/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-06 20:45:14.000000 twitter-api-client-0.9.0/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 22:13:57.017467 twitter-api-client-0.9.1/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.1/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 22:13:57.017467 twitter-api-client-0.9.1/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-06 22:13:57.017467 twitter-api-client-0.9.1/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-06 22:13:31.000000 twitter-api-client-0.9.1/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 22:13:57.016467 twitter-api-client-0.9.1/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.1/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    23524 2023-06-06 19:05:18.000000 twitter-api-client-0.9.1/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28299 2023-06-06 19:05:18.000000 twitter-api-client-0.9.1/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.9.1/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    28285 2023-06-06 22:07:05.000000 twitter-api-client-0.9.1/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     6123 2023-06-06 19:05:18.000000 twitter-api-client-0.9.1/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9683 2023-06-06 20:42:23.000000 twitter-api-client-0.9.1/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 22:13:57.017467 twitter-api-client-0.9.1/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 22:13:57.000000 twitter-api-client-0.9.1/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-06 22:13:57.000000 twitter-api-client-0.9.1/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-06 22:13:57.000000 twitter-api-client-0.9.1/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-06 22:13:57.000000 twitter-api-client-0.9.1/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-06 22:13:57.000000 twitter-api-client-0.9.1/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.9.0/LICENSE` & `twitter-api-client-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.0/PKG-INFO` & `twitter-api-client-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.9.0/setup.py` & `twitter-api-client-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.9.0",
+    version="0.9.1",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
```

### Comparing `twitter-api-client-0.9.0/twitter/account.py` & `twitter-api-client-0.9.1/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.0/twitter/constants.py` & `twitter-api-client-0.9.1/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.0/twitter/login.py` & `twitter-api-client-0.9.1/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.0/twitter/scraper.py` & `twitter-api-client-0.9.1/twitter/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,14 +289,15 @@
             return {
                 'space': key['rest_id'],
                 'chat': chat,
                 'info': info,
             }
 
         async def process():
+            (self.out_path / 'raw').mkdir(parents=True, exist_ok=True)
             limits = Limits(max_connections=100, max_keepalive_connections=10)
             headers = self.session.headers if self.guest else get_headers(self.session)
             cookies = self.session.cookies
             async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
                 tasks = (get(c, key) for key in keys)
                 if self.pbar:
                     return await tqdm_asyncio.gather(*tasks, desc='Downloading chat data')
```

### Comparing `twitter-api-client-0.9.0/twitter/search.py` & `twitter-api-client-0.9.1/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.0/twitter/util.py` & `twitter-api-client-0.9.1/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.0/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.9.1/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

