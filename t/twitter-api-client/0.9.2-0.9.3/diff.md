# Comparing `tmp/twitter-api-client-0.9.2.tar.gz` & `tmp/twitter-api-client-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.9.2.tar", last modified: Wed Jun  7 19:09:27 2023, max compression
+gzip compressed data, was "twitter-api-client-0.9.3.tar", last modified: Wed Jun  7 19:13:36 2023, max compression
```

## Comparing `twitter-api-client-0.9.2.tar` & `twitter-api-client-0.9.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:09:27.282779 twitter-api-client-0.9.2/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.2/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 19:09:27.281779 twitter-api-client-0.9.2/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-07 19:09:27.282779 twitter-api-client-0.9.2/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-07 19:04:37.000000 twitter-api-client-0.9.2/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:09:27.281779 twitter-api-client-0.9.2/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.2/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    23524 2023-06-06 19:05:18.000000 twitter-api-client-0.9.2/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28698 2023-06-07 18:37:17.000000 twitter-api-client-0.9.2/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7382 2023-06-07 19:06:40.000000 twitter-api-client-0.9.2/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    33429 2023-06-07 19:04:37.000000 twitter-api-client-0.9.2/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     6123 2023-06-06 19:05:18.000000 twitter-api-client-0.9.2/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-07 19:04:37.000000 twitter-api-client-0.9.2/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:09:27.281779 twitter-api-client-0.9.2/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 19:09:27.000000 twitter-api-client-0.9.2/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-07 19:09:27.000000 twitter-api-client-0.9.2/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-07 19:09:27.000000 twitter-api-client-0.9.2/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-07 19:09:27.000000 twitter-api-client-0.9.2/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-07 19:09:27.000000 twitter-api-client-0.9.2/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:13:36.051248 twitter-api-client-0.9.3/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.3/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 19:13:36.051248 twitter-api-client-0.9.3/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-07 19:13:36.051248 twitter-api-client-0.9.3/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-07 19:13:05.000000 twitter-api-client-0.9.3/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:13:36.051248 twitter-api-client-0.9.3/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.3/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    23528 2023-06-07 19:13:05.000000 twitter-api-client-0.9.3/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28698 2023-06-07 18:37:17.000000 twitter-api-client-0.9.3/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7382 2023-06-07 19:06:40.000000 twitter-api-client-0.9.3/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    33429 2023-06-07 19:04:37.000000 twitter-api-client-0.9.3/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     6127 2023-06-07 19:13:05.000000 twitter-api-client-0.9.3/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-07 19:04:37.000000 twitter-api-client-0.9.3/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-07 19:13:36.051248 twitter-api-client-0.9.3/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-07 19:13:36.000000 twitter-api-client-0.9.3/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-07 19:13:36.000000 twitter-api-client-0.9.3/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-07 19:13:36.000000 twitter-api-client-0.9.3/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-07 19:13:36.000000 twitter-api-client-0.9.3/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-07 19:13:36.000000 twitter-api-client-0.9.3/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.9.2/LICENSE` & `twitter-api-client-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.2/PKG-INFO` & `twitter-api-client-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.2
+Version: 0.9.3
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.9.2/setup.py` & `twitter-api-client-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.9.2",
+    version="0.9.3",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
```

### Comparing `twitter-api-client-0.9.2/twitter/account.py` & `twitter-api-client-0.9.3/twitter/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     except ImportError as e:
         ...
 
 
 class Account:
 
     def __init__(self, email: str = None, username: str = None, password: str = None, session: Client = None, **kwargs):
-        self.logger = self.init_logger(kwargs.get('log_config', False))
-        self.session = self.validate_session(email, username, password, session, **kwargs)
+        self.logger = self._init_logger(kwargs.get('log_config', False))
+        self.session = self._validate_session(email, username, password, session, **kwargs)
         self.save = kwargs.get('save', True)
         self.debug = kwargs.get('debug', 0)
         self.gql_api = 'https://twitter.com/i/api/graphql'
         self.v1_api = 'https://api.twitter.com/1.1'
 
     def gql(self, method: str, operation: tuple, variables: dict, features: dict = Operation.default_features) -> dict:
         qid, op = operation
@@ -553,29 +553,29 @@
     def _add_alt_text(self, media_id: int, text: str) -> Response:
         params = {"media_id": media_id, "alt_text": {"text": text}}
         url = f'{self.v1_api}/media/metadata/create.json'
         r = self.session.post(url, headers=get_headers(self.session), json=params)
         return r
 
     @staticmethod
-    def init_logger(cfg: dict) -> Logger:
+    def _init_logger(cfg: dict) -> Logger:
         if cfg:
             logging.config.dictConfig(cfg)
         else:
             logging.config.dictConfig(LOGGER_CONFIG)
 
         # Set level of all other loggers to ERROR
         for name in logging.root.manager.loggerDict:
             if name != LOGGER_NAME:
                 logging.getLogger(name).setLevel(logging.ERROR)
 
         return logging.getLogger(LOGGER_NAME)
 
     @staticmethod
-    def validate_session(*args, **kwargs):
+    def _validate_session(*args, **kwargs):
         email, username, password, session = args
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
             # authenticated session provided
             return session
         if not session:
             # no session provided, login to authenticate
             return login(email, username, password, **kwargs)
```

### Comparing `twitter-api-client-0.9.2/twitter/constants.py` & `twitter-api-client-0.9.3/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.2/twitter/login.py` & `twitter-api-client-0.9.3/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.2/twitter/scraper.py` & `twitter-api-client-0.9.3/twitter/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.2/twitter/search.py` & `twitter-api-client-0.9.3/twitter/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         uvloop.install()
     except ImportError as e:
         ...
 
 
 class Search:
     def __init__(self, email: str = None, username: str = None, password: str = None, session: Client = None, **kwargs):
-        self.logger = self.init_logger(kwargs.get('log_config', False))
-        self.session = self.validate_session(email, username, password, session, **kwargs)
+        self.logger = self._init_logger(kwargs.get('log_config', False))
+        self.session = self._validate_session(email, username, password, session, **kwargs)
         self.api = 'https://api.twitter.com/2/search/adaptive.json?'
         self.save = kwargs.get('save', True)
         self.debug = kwargs.get('debug', 0)
 
     def run(self, *args, out: str = 'data', **kwargs):
         out_path = self.make_output_dirs(out)
         if kwargs.get('latest', False):
@@ -131,29 +131,29 @@
         p = Path(f'{path}')
         (p / 'raw').mkdir(parents=True, exist_ok=True)
         (p / 'processed').mkdir(parents=True, exist_ok=True)
         (p / 'final').mkdir(parents=True, exist_ok=True)
         return p
 
     @staticmethod
-    def init_logger(cfg: dict) -> Logger:
+    def _init_logger(cfg: dict) -> Logger:
         if cfg:
             logging.config.dictConfig(cfg)
         else:
             logging.config.dictConfig(LOGGER_CONFIG)
 
         # Set level of all other loggers to ERROR
         for name in logging.root.manager.loggerDict:
             if name != LOGGER_NAME:
                 logging.getLogger(name).setLevel(logging.ERROR)
 
         return logging.getLogger(LOGGER_NAME)
 
     @staticmethod
-    def validate_session(*args, **kwargs):
+    def _validate_session(*args, **kwargs):
         email, username, password, session = args
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
             # authenticated session provided
             return session
         if not session:
             # no session provided, log-in to authenticate
             return login(email, username, password, **kwargs)
```

### Comparing `twitter-api-client-0.9.2/twitter/util.py` & `twitter-api-client-0.9.3/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.2/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.9.3/twitter_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.2
+Version: 0.9.3
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

