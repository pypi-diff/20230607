# Comparing `tmp/prefai-0.0.2.tar.gz` & `tmp/prefai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefai-0.0.2.tar", last modified: Mon Jun  5 21:22:20 2023, max compression
+gzip compressed data, was "prefai-0.0.3.tar", last modified: Wed Jun  7 06:52:27 2023, max compression
```

## Comparing `prefai-0.0.2.tar` & `prefai-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-05 21:22:20.503586 prefai-0.0.2/
--rw-r--r--   0 bjaros     (501) staff       (20)     1079 2023-06-01 06:14:59.000000 prefai-0.0.2/LICENSE.txt
--rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-05 21:22:20.503379 prefai-0.0.2/PKG-INFO
--rw-r--r--   0 bjaros     (501) staff       (20)     1238 2023-06-03 22:24:22.000000 prefai-0.0.2/README.md
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-05 21:22:20.502080 prefai-0.0.2/prefai/
--rw-r--r--   0 bjaros     (501) staff       (20)       46 2023-05-31 03:58:40.000000 prefai-0.0.2/prefai/__init__.py
--rw-r--r--   0 bjaros     (501) staff       (20)     4290 2023-06-05 21:09:53.000000 prefai-0.0.2/prefai/client.py
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-05 21:22:20.502792 prefai-0.0.2/prefai.egg-info/
--rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-05 21:22:20.000000 prefai-0.0.2/prefai.egg-info/PKG-INFO
--rw-r--r--   0 bjaros     (501) staff       (20)      207 2023-06-05 21:22:20.000000 prefai-0.0.2/prefai.egg-info/SOURCES.txt
--rw-r--r--   0 bjaros     (501) staff       (20)        1 2023-06-05 21:22:20.000000 prefai-0.0.2/prefai.egg-info/dependency_links.txt
--rw-r--r--   0 bjaros     (501) staff       (20)        7 2023-06-05 21:22:20.000000 prefai-0.0.2/prefai.egg-info/top_level.txt
--rw-r--r--   0 bjaros     (501) staff       (20)       38 2023-06-05 21:22:20.503643 prefai-0.0.2/setup.cfg
--rw-r--r--   0 bjaros     (501) staff       (20)      710 2023-06-05 21:10:13.000000 prefai-0.0.2/setup.py
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-05 21:22:20.502915 prefai-0.0.2/tests/
--rw-r--r--   0 bjaros     (501) staff       (20)     3204 2023-06-03 22:24:22.000000 prefai-0.0.2/tests/test_client.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-07 06:52:27.715684 prefai-0.0.3/
+-rw-r--r--   0 bjaros     (501) staff       (20)     1079 2023-06-01 06:14:59.000000 prefai-0.0.3/LICENSE.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-07 06:52:27.715519 prefai-0.0.3/PKG-INFO
+-rw-r--r--   0 bjaros     (501) staff       (20)     1238 2023-06-03 22:24:22.000000 prefai-0.0.3/README.md
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-07 06:52:27.714136 prefai-0.0.3/prefai/
+-rw-r--r--   0 bjaros     (501) staff       (20)       46 2023-05-31 03:58:40.000000 prefai-0.0.3/prefai/__init__.py
+-rw-r--r--   0 bjaros     (501) staff       (20)     5880 2023-06-07 06:48:49.000000 prefai-0.0.3/prefai/client.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-07 06:52:27.714983 prefai-0.0.3/prefai.egg-info/
+-rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-07 06:52:27.000000 prefai-0.0.3/prefai.egg-info/PKG-INFO
+-rw-r--r--   0 bjaros     (501) staff       (20)      207 2023-06-07 06:52:27.000000 prefai-0.0.3/prefai.egg-info/SOURCES.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)        1 2023-06-07 06:52:27.000000 prefai-0.0.3/prefai.egg-info/dependency_links.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)        7 2023-06-07 06:52:27.000000 prefai-0.0.3/prefai.egg-info/top_level.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)       38 2023-06-07 06:52:27.715734 prefai-0.0.3/setup.cfg
+-rw-r--r--   0 bjaros     (501) staff       (20)      710 2023-06-07 06:50:21.000000 prefai-0.0.3/setup.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-07 06:52:27.715122 prefai-0.0.3/tests/
+-rw-r--r--   0 bjaros     (501) staff       (20)     3204 2023-06-03 22:24:22.000000 prefai-0.0.3/tests/test_client.py
```

### Comparing `prefai-0.0.2/LICENSE.txt` & `prefai-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prefai-0.0.2/PKG-INFO` & `prefai-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefai
-Version: 0.0.2
+Version: 0.0.3
 Summary: A brief description of your package
 Home-page: http://github.com/prefai/pythonclient
 Author: Bobby Jaros
 Author-email: bobby@pref.ai
 License: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prefai-0.0.2/README.md` & `prefai-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `prefai-0.0.2/prefai/client.py` & `prefai-0.0.3/prefai/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 class PrefaiTimeoutError(PrefaiError):
     pass
 
 class PrefaiClient:
     _api_base_url = 'https://api.pref.ai'
+    # _api_base_url = 'http://127.0.0.1:8000'
 
     def __init__(self, api_key: str = None):
         if api_key:
             self.api_key = api_key
         else:
             self.api_key = os.getenv('PREFAI_API_KEY')
 
@@ -93,15 +94,15 @@
 
 
     def retrieve_records(self,
         user_action: str,
         context: Optional[str] = None,
         user_email: Optional[str] = None,
         user_id: Optional[str] = None,
-        max_num_results: Optional[int] = 3,
+        max_results: Optional[int] = 3,
         min_similarity: Optional[float] = None,
     ) -> Dict:
 
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
@@ -110,15 +111,60 @@
             response = requests.post(
                 f"{self._api_base_url}/v1/records/retrieve",
                 json={
                     "context": context,
                     "user_action": user_action,
                     "user_email": user_email,
                     "user_id": user_id,
-                    "max_num_results": max_num_results,
+                    "max_results": max_results,
+                    "min_similarity": min_similarity,
+                },
+                headers=headers,
+                timeout=5
+            )
+
+            response.raise_for_status()
+            json_response = response.json()
+
+            return json_response
+
+        except requests.exceptions.Timeout:
+            raise PrefaiTimeoutError("Request timed out")
+
+        except requests.HTTPError as http_err:
+            response_content = response.content.decode()
+            if response_content:
+                response_dict = json.loads(response_content)
+                if 'detail' in response_dict:
+                    raise PrefaiError(f"Request failed: {http_err}. Reason: {response_dict['detail']}")
+            raise PrefaiError(f"Request failed: {http_err}")
+
+    def retrieve_prompt(self,
+        user_action: str,
+        context: Optional[str] = None,
+        user_email: Optional[str] = None,
+        user_id: Optional[str] = None,
+        max_tokens: Optional[int] = 300,
+        min_similarity: Optional[float] = None,
+    ) -> Dict:
+
+        headers = {
+            "Authorization": f"Bearer {self.api_key}",
+            "Content-Type": "application/json",
+        }
+
+        try:
+            response = requests.post(
+                f"{self._api_base_url}/v1/records/retrieve-prompt",
+                json={
+                    "context": context,
+                    "user_action": user_action,
+                    "user_email": user_email,
+                    "user_id": user_id,
+                    "max_tokens": max_tokens,
                     "min_similarity": min_similarity,
                 },
                 headers=headers,
                 timeout=5
             )
 
             response.raise_for_status()
```

### Comparing `prefai-0.0.2/prefai.egg-info/PKG-INFO` & `prefai-0.0.3/prefai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefai
-Version: 0.0.2
+Version: 0.0.3
 Summary: A brief description of your package
 Home-page: http://github.com/prefai/pythonclient
 Author: Bobby Jaros
 Author-email: bobby@pref.ai
 License: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prefai-0.0.2/setup.py` & `prefai-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="prefai",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     author="Bobby Jaros",
     author_email="bobby@pref.ai",
     description="A brief description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="http://github.com/prefai/pythonclient",
```

### Comparing `prefai-0.0.2/tests/test_client.py` & `prefai-0.0.3/tests/test_client.py`

 * *Files identical despite different names*

