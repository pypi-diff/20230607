# Comparing `tmp/computing-toolbox-0.2.1.tar.gz` & `tmp/computing-toolbox-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computing-toolbox-0.2.1.tar", last modified: Tue Jun  6 02:54:05 2023, max compression
+gzip compressed data, was "computing-toolbox-0.3.0.tar", last modified: Wed Jun  7 08:36:21 2023, max compression
```

## Comparing `computing-toolbox-0.2.1.tar` & `computing-toolbox-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:05.210327 computing-toolbox-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-06 02:54:05.206328 computing-toolbox-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 02:54:05.210327 computing-toolbox-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:05.206328 computing-toolbox-0.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:05.206328 computing-toolbox-0.2.1/src/computing_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:05.206328 computing-toolbox-0.2.1/src/computing_toolbox/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/algorithms/split_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:05.206328 computing-toolbox-0.2.1/src/computing_toolbox/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/gcp/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:05.206328 computing-toolbox-0.2.1/src/computing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/utils/deep_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/utils/es_long_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/utils/http_async_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/utils/http_fake_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/utils/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/utils/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-06 02:53:56.000000 computing-toolbox-0.2.1/src/computing_toolbox/utils/tictoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:05.206328 computing-toolbox-0.2.1/src/computing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-06 02:54:05.000000 computing-toolbox-0.2.1/src/computing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-06 02:54:05.000000 computing-toolbox-0.2.1/src/computing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:54:05.000000 computing-toolbox-0.2.1/src/computing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-06 02:54:05.000000 computing-toolbox-0.2.1/src/computing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-06 02:54:05.000000 computing-toolbox-0.2.1/src/computing_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/computing_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/computing_toolbox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/algorithms/split_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/computing_toolbox/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/gcp/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/gcp/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/computing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/deep_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/es_long_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/http_async_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/http_fake_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 08:36:21.000000 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-07 08:36:21.000000 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:36:21.000000 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 08:36:21.000000 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 08:36:21.000000 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/top_level.txt
```

### Comparing `computing-toolbox-0.2.1/LICENSE` & `computing-toolbox-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.2.1/PKG-INFO` & `computing-toolbox-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.2.1
+Version: 0.3.0
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.2.1/README.md` & `computing-toolbox-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.2.1/pyproject.toml` & `computing-toolbox-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "computing-toolbox"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
   { name="Pedro Mayorga", email="ppmayorga80@gmail.com" },
 ]
 description = "Computing Toolbox for daily computations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `computing-toolbox-0.2.1/src/computing_toolbox/algorithms/split_range.py` & `computing-toolbox-0.3.0/src/computing_toolbox/algorithms/split_range.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.2.1/src/computing_toolbox/gcp/gs.py` & `computing-toolbox-0.3.0/src/computing_toolbox/gcp/gs.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.2.1/src/computing_toolbox/gcp/secret_manager.py` & `computing-toolbox-0.3.0/src/computing_toolbox/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.2.1/src/computing_toolbox/utils/deep_get.py` & `computing-toolbox-0.3.0/src/computing_toolbox/utils/deep_get.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.2.1/src/computing_toolbox/utils/es_long_search.py` & `computing-toolbox-0.3.0/src/computing_toolbox/utils/es_long_search.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.2.1/src/computing_toolbox/utils/http_fake_headers.py` & `computing-toolbox-0.3.0/src/computing_toolbox/utils/http_fake_headers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,35 @@
 """generate fake or random http headers"""
 from fake_headers import Headers
 
+DEFAULT_HEADERS = {
+    'accept':
+    'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
+    'accept-language':
+    'en',
+    'sec-ch-ua':
+    '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
+    'sec-ch-ua-mobile':
+    '?0',
+    'sec-ch-ua-platform':
+    '"macOS"',
+    'sec-fetch-dest':
+    'document',
+    'sec-fetch-mode':
+    'navigate',
+    'sec-fetch-site':
+    'none',
+    'sec-fetch-user':
+    '?1',
+    'upgrade-insecure-requests':
+    '1',
+    'user-agent':
+    'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
+}
+
 
 def generate_fake_headers(authority: str = "",
                           method: str = "get",
                           scheme: str = "https",
                           default_headers: dict or None = None) -> dict:
     """generate a fake headers to be used in requests
 
@@ -18,36 +43,19 @@
     # 1. define a default headers if necessary and make sure all keys are in lowercase
     # 1.1 regular headers from regular arguments
     regular_headers = {
         "authority": authority,
         "method": method,
         "scheme": scheme,
     }
-    #1.2 default headers taken from a real browser or take the default_header from arguments
-    default_headers = {
-        "accept":
-        "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-        "accept-encoding":
-        "gzip, deflate, br",
-        "accept-language":
-        "en-US,en;q=0.9,es;q=0.8",
-        "cache-control":
-        "max-age=0",
-        "sec-fetch-dest":
-        "document",
-        "sec-fetch-mode":
-        "navigate",
-        "sec-fetch-site":
-        "same-origin",
-        "user-agent":
-        "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.4951.54 Safari/537.36"
-    } if default_headers is None else default_headers
-    #1.3 merge regular headers and default headers
+    # 1.2 default headers taken from a real browser or take the default_header from arguments
+    default_headers = DEFAULT_HEADERS if default_headers is None else default_headers
+    # 1.3 merge regular headers and default headers
     default_headers = {**regular_headers, **default_headers}
-    #1.4 make all keys lowercase
+    # 1.4 make all keys lowercase
     default_headers = {k.lower(): v for k, v in default_headers.items()}
 
     # 2. define a fake-header object and generate a random headers
     header = Headers()
     fake_headers = header.generate()
     # 2.1 convert all keys in lower case to be compatible with default headers
     fake_headers = {k.lower(): v for k, v in fake_headers.items()}
```

### Comparing `computing-toolbox-0.2.1/src/computing_toolbox/utils/http_request.py` & `computing-toolbox-0.3.0/src/computing_toolbox/utils/http_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.2.1/src/computing_toolbox/utils/jsonl.py` & `computing-toolbox-0.3.0/src/computing_toolbox/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.2.1/src/computing_toolbox/utils/tictoc.py` & `computing-toolbox-0.3.0/src/computing_toolbox/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.2.1/src/computing_toolbox.egg-info/PKG-INFO` & `computing-toolbox-0.3.0/src/computing_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.2.1
+Version: 0.3.0
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.2.1/src/computing_toolbox.egg-info/SOURCES.txt` & `computing-toolbox-0.3.0/src/computing_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

