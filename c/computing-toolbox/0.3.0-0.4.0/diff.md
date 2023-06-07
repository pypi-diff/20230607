# Comparing `tmp/computing-toolbox-0.3.0.tar.gz` & `tmp/computing-toolbox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computing-toolbox-0.3.0.tar", last modified: Wed Jun  7 08:36:21 2023, max compression
+gzip compressed data, was "computing-toolbox-0.4.0.tar", last modified: Wed Jun  7 09:06:57 2023, max compression
```

## Comparing `computing-toolbox-0.3.0.tar` & `computing-toolbox-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/computing_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/computing_toolbox/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/algorithms/split_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/computing_toolbox/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/gcp/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/computing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/deep_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/es_long_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/http_async_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/http_fake_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-07 08:36:12.000000 computing-toolbox-0.3.0/src/computing_toolbox/utils/tictoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:21.518716 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 08:36:21.000000 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-07 08:36:21.000000 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:36:21.000000 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 08:36:21.000000 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 08:36:21.000000 computing-toolbox-0.3.0/src/computing_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.869333 computing-toolbox-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 09:06:57.869333 computing-toolbox-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:06:57.869333 computing-toolbox-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.865333 computing-toolbox-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.865333 computing-toolbox-0.4.0/src/computing_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.865333 computing-toolbox-0.4.0/src/computing_toolbox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/algorithms/split_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.865333 computing-toolbox-0.4.0/src/computing_toolbox/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/gcp/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/gcp/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.869333 computing-toolbox-0.4.0/src/computing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/deep_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/es_long_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/http_async_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/http_fake_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.865333 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 09:06:57.000000 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-07 09:06:57.000000 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:06:57.000000 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 09:06:57.000000 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 09:06:57.000000 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/top_level.txt
```

### Comparing `computing-toolbox-0.3.0/LICENSE` & `computing-toolbox-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.3.0/PKG-INFO` & `computing-toolbox-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.3.0
+Version: 0.4.0
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.3.0/README.md` & `computing-toolbox-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox/algorithms/split_range.py` & `computing-toolbox-0.4.0/src/computing_toolbox/algorithms/split_range.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox/gcp/gs.py` & `computing-toolbox-0.4.0/src/computing_toolbox/gcp/gs.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox/gcp/secret_manager.py` & `computing-toolbox-0.4.0/src/computing_toolbox/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox/utils/deep_get.py` & `computing-toolbox-0.4.0/src/computing_toolbox/utils/deep_get.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox/utils/es_long_search.py` & `computing-toolbox-0.4.0/src/computing_toolbox/utils/es_long_search.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox/utils/http_async_request.py` & `computing-toolbox-0.4.0/src/computing_toolbox/utils/http_async_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 import aiohttp
 from aiohttp.client_reqrep import ClientResponse
 from tqdm import tqdm
 
 from computing_toolbox.utils.tictoc import tic, toc
 
-HTTP_SUCCESS_SYMBOL = "🟢"
-HTTP_FAILURE_SYMBOL = "⭕️"
-HTTP_ERROR_SYMBOL = "🔴"
+HTTP_SUCCESS_SYMBOL = "🟢"  # for status_code==[2**]
+HTTP_FAILURE_SYMBOL = "⭕️"  # for status_code!=[2**]
+HTTP_ERROR_SYMBOL = "🔴"  # for exceptions or errors
 
 
 @dataclass
 class HttpAsyncResponse:
     """Custom class for the http response (aiohttp has status variable not status_code)"""
     flag: str = ""
     response: ClientResponse or None = None
@@ -315,19 +315,19 @@
         } for r in request_kwargs]
 
         # create a tqdm dictionary if necessary
         self.progress_bar_increment = 1.0 / self.max_attempts
         tqdm_kwargs = {
             **{
                 "desc":
-                f"HttpAsyncRequest.{self.method}x{n_urls}",
+                    f"HttpAsyncRequest.{self.method}x{n_urls}",
                 "total":
-                len(urls),
+                    len(urls),
                 "bar_format":
-                "{l_bar}{bar}| {n:0.1f}/{total_fmt} [{elapsed}<{remaining}, {rate_fmt}{postfix}]"
+                    "{l_bar}{bar}| {n:0.1f}/{total_fmt} [{elapsed}<{remaining}, {rate_fmt}{postfix}]"
             },
             **tqdm_kwargs
         } if tqdm_kwargs is not None else tqdm_kwargs
 
         # return parameters in the same order, now fixed
         return urls, request_kwargs, tqdm_kwargs
 
@@ -421,15 +421,15 @@
         async with aiohttp.ClientSession() as session:
             # A.1 create the list of responses and progress bar
             self.responses_history = [HttpAsyncResponse() for _ in urls]
 
             # A.2create the progress bar if needed
             range_it = range(len(urls))
             self.progress_bar = tqdm(range_it, **
-                                     tqdm_kwargs) if tqdm_kwargs else None
+            tqdm_kwargs) if tqdm_kwargs else None
 
             # A.3 construct the list of tasks to be requested
             tasks = [
                 asyncio.ensure_future(
                     self._request_one(session=session,
                                       method=method,
                                       url=url_k,
```

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox/utils/http_fake_headers.py` & `computing-toolbox-0.4.0/src/computing_toolbox/utils/http_fake_headers.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox/utils/http_request.py` & `computing-toolbox-0.4.0/src/computing_toolbox/utils/http_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox/utils/jsonl.py` & `computing-toolbox-0.4.0/src/computing_toolbox/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox/utils/tictoc.py` & `computing-toolbox-0.4.0/src/computing_toolbox/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox.egg-info/PKG-INFO` & `computing-toolbox-0.4.0/src/computing_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.3.0
+Version: 0.4.0
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.3.0/src/computing_toolbox.egg-info/SOURCES.txt` & `computing-toolbox-0.4.0/src/computing_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

