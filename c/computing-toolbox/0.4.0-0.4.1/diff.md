# Comparing `tmp/computing-toolbox-0.4.0.tar.gz` & `tmp/computing-toolbox-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computing-toolbox-0.4.0.tar", last modified: Wed Jun  7 09:06:57 2023, max compression
+gzip compressed data, was "computing-toolbox-0.4.1.tar", last modified: Wed Jun  7 18:59:30 2023, max compression
```

## Comparing `computing-toolbox-0.4.0.tar` & `computing-toolbox-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.869333 computing-toolbox-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 09:06:57.869333 computing-toolbox-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:06:57.869333 computing-toolbox-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.865333 computing-toolbox-0.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.865333 computing-toolbox-0.4.0/src/computing_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.865333 computing-toolbox-0.4.0/src/computing_toolbox/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/algorithms/split_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.865333 computing-toolbox-0.4.0/src/computing_toolbox/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/gcp/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.869333 computing-toolbox-0.4.0/src/computing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/deep_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/es_long_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    21692 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/http_async_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/http_fake_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-07 09:06:46.000000 computing-toolbox-0.4.0/src/computing_toolbox/utils/tictoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:06:57.865333 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 09:06:57.000000 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-07 09:06:57.000000 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:06:57.000000 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 09:06:57.000000 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 09:06:57.000000 computing-toolbox-0.4.0/src/computing_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.971042 computing-toolbox-0.4.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.971042 computing-toolbox-0.4.1/src/computing_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/src/computing_toolbox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/algorithms/split_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/src/computing_toolbox/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/gcp/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/gcp/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/src/computing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/deep_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/es_long_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/http_async_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/http_fake_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 18:59:30.000000 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-07 18:59:30.000000 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:59:30.000000 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 18:59:30.000000 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 18:59:30.000000 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/top_level.txt
```

### Comparing `computing-toolbox-0.4.0/LICENSE` & `computing-toolbox-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.0/PKG-INFO` & `computing-toolbox-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.4.0
+Version: 0.4.1
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.4.0/README.md` & `computing-toolbox-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox/algorithms/split_range.py` & `computing-toolbox-0.4.1/src/computing_toolbox/algorithms/split_range.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox/gcp/gs.py` & `computing-toolbox-0.4.1/src/computing_toolbox/gcp/gs.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox/gcp/secret_manager.py` & `computing-toolbox-0.4.1/src/computing_toolbox/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox/utils/deep_get.py` & `computing-toolbox-0.4.1/src/computing_toolbox/utils/deep_get.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox/utils/es_long_search.py` & `computing-toolbox-0.4.1/src/computing_toolbox/utils/es_long_search.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox/utils/http_async_request.py` & `computing-toolbox-0.4.1/src/computing_toolbox/utils/http_async_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from collections import Counter
 from dataclasses import dataclass, field
 
 import aiohttp
 from aiohttp.client_reqrep import ClientResponse
 from tqdm import tqdm
 
+from computing_toolbox.utils.deep_get import deep_get
 from computing_toolbox.utils.tictoc import tic, toc
 
 HTTP_SUCCESS_SYMBOL = "🟢"  # for status_code==[2**]
 HTTP_FAILURE_SYMBOL = "⭕️"  # for status_code!=[2**]
 HTTP_ERROR_SYMBOL = "🔴"  # for exceptions or errors
 
 
@@ -283,31 +284,38 @@
                     timeout: float or list[float] = 5,
                     allow_redirects: bool or list[bool] = True,
                     proxies: dict or list[dict] or None = None,
                     request_kwargs: dict or None = None,
                     tqdm_kwargs: dict or None = None):
         """fix parameters from `request` method, used only before `request` method is executed"""
         n_urls = len(urls)
+
         # fix null values -> list
         params = self._expand_to_list(params, n_urls)
         headers = self._expand_to_list(headers, n_urls)
         timeout = self._expand_to_list(timeout, n_urls)
         allow_redirects = self._expand_to_list(allow_redirects, n_urls)
         proxies = self._expand_to_list(proxies, n_urls)
 
+        # fix proxies for aiohttp (because this class use a string proxy representation)
+        proxies = [
+            deep_get(p, ["https"], deep_get(p, ["http"], None)) if isinstance(
+                p, dict) else p for p in proxies
+        ]
+
         # set default kwargs for request
         request_kwargs = request_kwargs if request_kwargs is not None else {}
         request_kwargs = self._expand_to_list(request_kwargs, n_urls)
         request_kwargs = [{
             **{
                 "params": p,
                 "headers": h,
                 "timeout": t,
                 "allow_redirects": a,
-                "proxies": x,
+                "proxy": x,
             },
             **r
         } for r, p, h, t, a, x in zip(request_kwargs, params, headers, timeout,
                                       allow_redirects, proxies)]
         # filter not defined params
         request_kwargs = [{
             k: v
@@ -315,19 +323,19 @@
         } for r in request_kwargs]
 
         # create a tqdm dictionary if necessary
         self.progress_bar_increment = 1.0 / self.max_attempts
         tqdm_kwargs = {
             **{
                 "desc":
-                    f"HttpAsyncRequest.{self.method}x{n_urls}",
+                f"HttpAsyncRequest.{self.method}x{n_urls}",
                 "total":
-                    len(urls),
+                len(urls),
                 "bar_format":
-                    "{l_bar}{bar}| {n:0.1f}/{total_fmt} [{elapsed}<{remaining}, {rate_fmt}{postfix}]"
+                "{l_bar}{bar}| {n:0.1f}/{total_fmt} [{elapsed}<{remaining}, {rate_fmt}{postfix}]"
             },
             **tqdm_kwargs
         } if tqdm_kwargs is not None else tqdm_kwargs
 
         # return parameters in the same order, now fixed
         return urls, request_kwargs, tqdm_kwargs
 
@@ -421,15 +429,15 @@
         async with aiohttp.ClientSession() as session:
             # A.1 create the list of responses and progress bar
             self.responses_history = [HttpAsyncResponse() for _ in urls]
 
             # A.2create the progress bar if needed
             range_it = range(len(urls))
             self.progress_bar = tqdm(range_it, **
-            tqdm_kwargs) if tqdm_kwargs else None
+                                     tqdm_kwargs) if tqdm_kwargs else None
 
             # A.3 construct the list of tasks to be requested
             tasks = [
                 asyncio.ensure_future(
                     self._request_one(session=session,
                                       method=method,
                                       url=url_k,
```

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox/utils/http_fake_headers.py` & `computing-toolbox-0.4.1/src/computing_toolbox/utils/http_fake_headers.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox/utils/http_request.py` & `computing-toolbox-0.4.1/src/computing_toolbox/utils/http_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,49 +106,53 @@
         # filter not defined params
         default_request_kwargs = {
             k: v
             for k, v in default_request_kwargs.items() if v is not None
         }
 
         tqdm_default_kwargs = {
-            "desc": f"HttpRequest.{self.method}({url})",
+            "desc": f"HttpRequest.{self.method} Attempts:",
             "total": self.max_attempts
         }
         tqdm_default_kwargs = {
             **tqdm_default_kwargs,
             **tqdm_kwargs
         } if tqdm_kwargs is not None else tqdm_default_kwargs
 
         range_it = range(self.max_attempts)
-        attempt_iterator = tqdm(
-            range_it, **
-            tqdm_default_kwargs) if tqdm_kwargs is not None else range_it
+        attempt_iterator = range_it if tqdm_kwargs is None else tqdm(
+            range_it, **tqdm_default_kwargs)
 
         self.errors = []
         success = False
         response = None
         postfix_str = "⚪️"
+        break_flag = False
         for k in attempt_iterator:
+            if break_flag:
+                break
+
             self.attempts = k + 1
             if tqdm_kwargs is not None:
                 if len(self.errors) > 0:
                     postfix_str = f"🔴x{len(self.errors)}"
                     attempt_iterator.set_postfix_str(postfix_str)
 
             try:
                 response = requests.request(method, url,
                                             **default_request_kwargs)
                 if 200 <= response.status_code < 300:
                     success = True
+                    break_flag = True
                     if tqdm_kwargs is not None:
                         postfix_str += "→🟢"
                         attempt_iterator.set_postfix_str(postfix_str)
                         attempt_iterator.update()
-                    break
-                # if not break <-> not success then add an error
+
+                # if not break <-> not success, then add an error
                 self.errors.append(
                     ValueError(
                         f"failed request at attempt {k + 1} with status_code:{response.status_code}"
                     ))
             except Exception as error:
                 self.errors.append(f"{error}")
                 if self.rnd_sleep_interval:
```

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox/utils/jsonl.py` & `computing-toolbox-0.4.1/src/computing_toolbox/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox/utils/tictoc.py` & `computing-toolbox-0.4.1/src/computing_toolbox/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox.egg-info/PKG-INFO` & `computing-toolbox-0.4.1/src/computing_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.4.0
+Version: 0.4.1
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.4.0/src/computing_toolbox.egg-info/SOURCES.txt` & `computing-toolbox-0.4.1/src/computing_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

