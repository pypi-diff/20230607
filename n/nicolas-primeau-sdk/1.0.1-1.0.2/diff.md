# Comparing `tmp/nicolas-primeau-sdk-1.0.1.tar.gz` & `tmp/nicolas-primeau-sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicolas-primeau-sdk-1.0.1.tar", last modified: Wed Jun  7 00:02:59 2023, max compression
+gzip compressed data, was "nicolas-primeau-sdk-1.0.2.tar", last modified: Wed Jun  7 00:06:18 2023, max compression
```

## Comparing `nicolas-primeau-sdk-1.0.1.tar` & `nicolas-primeau-sdk-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:02:59.789252 nicolas-primeau-sdk-1.0.1/
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     1063 2023-06-06 23:55:38.000000 nicolas-primeau-sdk-1.0.1/LICENSE.txt
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      304 2023-06-07 00:02:59.789252 nicolas-primeau-sdk-1.0.1/PKG-INFO
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     3194 2023-06-06 23:22:06.000000 nicolas-primeau-sdk-1.0.1/README.md
-drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:02:59.789252 nicolas-primeau-sdk-1.0.1/nicolas_primeau_sdk.egg-info/
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      304 2023-06-07 00:02:59.000000 nicolas-primeau-sdk-1.0.1/nicolas_primeau_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      946 2023-06-07 00:02:59.000000 nicolas-primeau-sdk-1.0.1/nicolas_primeau_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)        1 2023-06-07 00:02:59.000000 nicolas-primeau-sdk-1.0.1/nicolas_primeau_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)       72 2023-06-07 00:02:59.000000 nicolas-primeau-sdk-1.0.1/nicolas_primeau_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)       17 2023-06-07 00:02:59.000000 nicolas-primeau-sdk-1.0.1/nicolas_primeau_sdk.egg-info/requires.txt
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)       16 2023-06-07 00:02:59.000000 nicolas-primeau-sdk-1.0.1/nicolas_primeau_sdk.egg-info/top_level.txt
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)       50 2023-06-06 17:04:47.000000 nicolas-primeau-sdk-1.0.1/pyproject.toml
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)       79 2023-06-07 00:02:59.793252 nicolas-primeau-sdk-1.0.1/setup.cfg
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      726 2023-06-07 00:02:31.000000 nicolas-primeau-sdk-1.0.1/setup.py
-drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:02:59.789252 nicolas-primeau-sdk-1.0.1/src/
-drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:02:59.789252 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-06 18:36:59.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/__init__.py
-drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:02:59.789252 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/cli/
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-06 21:04:03.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/cli/__init__.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     2142 2023-06-06 23:47:16.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/cli/cli_client.py
-drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:02:59.789252 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/components/
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-06 17:22:08.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/components/__init__.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      957 2023-06-06 21:51:20.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/components/base.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     1114 2023-06-06 23:47:16.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/components/client.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     3256 2023-06-06 23:51:43.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/components/requests.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      850 2023-06-06 23:47:16.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/config.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      789 2023-06-06 23:47:16.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/exceptions.py
-drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:02:59.789252 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/resources/
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-06 19:15:54.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/resources/__init__.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     1272 2023-06-06 19:58:56.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/resources/adapters.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      589 2023-06-06 22:01:23.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/resources/base.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     1163 2023-06-06 23:47:49.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/resources/movies.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     1268 2023-06-06 23:47:49.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/resources/quotes.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      437 2023-06-06 23:44:46.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/sdk.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      161 2023-06-06 18:42:26.000000 nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/utils.py
-drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:02:59.789252 nicolas-primeau-sdk-1.0.1/test/
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      860 2023-06-06 23:47:16.000000 nicolas-primeau-sdk-1.0.1/test/test_config.py
--rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     3559 2023-06-06 23:47:33.000000 nicolas-primeau-sdk-1.0.1/test/test_sdk.py
+drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:06:18.072636 nicolas-primeau-sdk-1.0.2/
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     1063 2023-06-06 23:55:38.000000 nicolas-primeau-sdk-1.0.2/LICENSE.txt
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      304 2023-06-07 00:06:18.072636 nicolas-primeau-sdk-1.0.2/PKG-INFO
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     3194 2023-06-06 23:22:06.000000 nicolas-primeau-sdk-1.0.2/README.md
+drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:06:18.068636 nicolas-primeau-sdk-1.0.2/nicolas_primeau_sdk.egg-info/
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      304 2023-06-07 00:06:18.000000 nicolas-primeau-sdk-1.0.2/nicolas_primeau_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      946 2023-06-07 00:06:18.000000 nicolas-primeau-sdk-1.0.2/nicolas_primeau_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)        1 2023-06-07 00:06:18.000000 nicolas-primeau-sdk-1.0.2/nicolas_primeau_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)       72 2023-06-07 00:06:18.000000 nicolas-primeau-sdk-1.0.2/nicolas_primeau_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)       17 2023-06-07 00:06:18.000000 nicolas-primeau-sdk-1.0.2/nicolas_primeau_sdk.egg-info/requires.txt
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)       16 2023-06-07 00:06:18.000000 nicolas-primeau-sdk-1.0.2/nicolas_primeau_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)       50 2023-06-06 17:04:47.000000 nicolas-primeau-sdk-1.0.2/pyproject.toml
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)       79 2023-06-07 00:06:18.072636 nicolas-primeau-sdk-1.0.2/setup.cfg
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      726 2023-06-07 00:05:16.000000 nicolas-primeau-sdk-1.0.2/setup.py
+drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:06:18.068636 nicolas-primeau-sdk-1.0.2/src/
+drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:06:18.068636 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-06 18:36:59.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/__init__.py
+drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:06:18.072636 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/cli/
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-06 21:04:03.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/cli/__init__.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     2107 2023-06-07 00:04:35.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/cli/cli_client.py
+drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:06:18.072636 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/components/
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-06 17:22:08.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/components/__init__.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      957 2023-06-06 21:51:20.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/components/base.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     1114 2023-06-06 23:47:16.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/components/client.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     3256 2023-06-06 23:51:43.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/components/requests.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      850 2023-06-06 23:47:16.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/config.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      789 2023-06-06 23:47:16.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/exceptions.py
+drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:06:18.072636 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/resources/
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-06 19:15:54.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/resources/__init__.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     1272 2023-06-06 19:58:56.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/resources/adapters.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      589 2023-06-06 22:01:23.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/resources/base.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     1163 2023-06-06 23:47:49.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/resources/movies.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     1268 2023-06-06 23:47:49.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/resources/quotes.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      437 2023-06-06 23:44:46.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/sdk.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      161 2023-06-06 18:42:26.000000 nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/utils.py
+drwxrwxr-x   0 nprimeau  (1000) nprimeau  (1000)        0 2023-06-07 00:06:18.072636 nicolas-primeau-sdk-1.0.2/test/
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)      860 2023-06-06 23:47:16.000000 nicolas-primeau-sdk-1.0.2/test/test_config.py
+-rw-rw-r--   0 nprimeau  (1000) nprimeau  (1000)     3559 2023-06-06 23:47:33.000000 nicolas-primeau-sdk-1.0.2/test/test_sdk.py
```

### Comparing `nicolas-primeau-sdk-1.0.1/LICENSE.txt` & `nicolas-primeau-sdk-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/README.md` & `nicolas-primeau-sdk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/nicolas_primeau_sdk.egg-info/SOURCES.txt` & `nicolas-primeau-sdk-1.0.2/nicolas_primeau_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/setup.py` & `nicolas-primeau-sdk-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 _SCRIPT_PATH = pathlib.Path("./scripts")
 setup(
     name='nicolas-primeau-sdk',
     author="Nicolas Primeau",
     author_email="nicolas.primeau@gmail.com",
     description="Description",
-    version='1.0.1',
+    version='1.0.2',
     python_requires=">=3.10.0",
     install_requires=[
         'requests>=2.31.0',
     ],
-    download_url="https://github.com/Nixon-/nicolas.primeau-SDK/archive/refs/tags/1.0.1.tar.gz",
+    download_url="https://github.com/Nixon-/nicolas.primeau-SDK/archive/refs/tags/1.0.2.tar.gz",
     packages=setuptools.find_packages(where="./src"),
     package_dir={'the_one_api_sdk': 'src/the_one_api_sdk'},
     entry_points={
         'console_scripts': [
             'the-one-api-sdk = the_one_api_sdk.cli.cli_client:main'
         ]
     },
```

### Comparing `nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/cli/cli_client.py` & `nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/cli/cli_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import pprint
 
-from the_one_api_sdk import components
+from the_one_api_sdk import sdk
 
 
 class UnknownCommand(Exception):
     pass
 
 
 class InvalidCommand(Exception):
@@ -42,28 +42,28 @@
         case _:
             raise UnknownCommand(args.command)
 
 
 def handle_movie_command(args):
     match args.subcommand:
         case "list":
-            for movie in components.TheOneApiSdk().movies.list(limit=args.limit):
+            for movie in sdk.TheOneApiSdk().movies.list(limit=args.limit):
                 pprint.pprint(movie)
         case "get":
             if not args.movie_id:
                 raise InvalidCommand("Movie ID must be specified")
-            pprint.pprint(components.TheOneApiSdk().movies(args.movie_id).fetch())
+            pprint.pprint(sdk.TheOneApiSdk().movies(args.movie_id).fetch())
         case _:
             raise UnknownCommand(args.subcommand)
 
 
 def handle_quotes_command(args):
     match args.subcommand:
         case "list":
-            for quote in components.TheOneApiSdk().quotes.list(movie_id=args.movie_id, limit=args.limit):
+            for quote in sdk.TheOneApiSdk().quotes.list(movie_id=args.movie_id, limit=args.limit):
                 pprint.pprint(quote)
         case "get":
             if not args.quote_id:
                 raise InvalidCommand("Quote ID must be specified")
-            pprint.pprint(components.TheOneApiSdk().quotes(args.quote_id).fetch())
+            pprint.pprint(sdk.TheOneApiSdk().quotes(args.quote_id).fetch())
         case _:
             raise UnknownCommand(args.subcommand)
```

### Comparing `nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/components/base.py` & `nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/components/base.py`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/components/client.py` & `nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/components/client.py`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/components/requests.py` & `nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/components/requests.py`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/config.py` & `nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/config.py`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/exceptions.py` & `nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/resources/adapters.py` & `nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/resources/adapters.py`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/resources/base.py` & `nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/resources/base.py`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/resources/movies.py` & `nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/resources/movies.py`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/src/the_one_api_sdk/resources/quotes.py` & `nicolas-primeau-sdk-1.0.2/src/the_one_api_sdk/resources/quotes.py`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/test/test_config.py` & `nicolas-primeau-sdk-1.0.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `nicolas-primeau-sdk-1.0.1/test/test_sdk.py` & `nicolas-primeau-sdk-1.0.2/test/test_sdk.py`

 * *Files identical despite different names*

