# Comparing `tmp/python-eigen-ingenuity-0.4.7.3.tar.gz` & `tmp/python-eigen-ingenuity-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-eigen-ingenuity-0.4.7.3.tar", last modified: Mon May 22 10:03:07 2023, max compression
+gzip compressed data, was "python-eigen-ingenuity-0.4.8.tar", last modified: Wed Jun  7 12:12:42 2023, max compression
```

## Comparing `python-eigen-ingenuity-0.4.7.3.tar` & `python-eigen-ingenuity-0.4.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-22 10:03:07.479429 python-eigen-ingenuity-0.4.7.3/
--rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.3/LICENSE
--rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.7.3/MANIFEST.in
--rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-05-22 10:03:07.479150 python-eigen-ingenuity-0.4.7.3/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.3/README.md
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-22 10:03:07.477090 python-eigen-ingenuity-0.4.7.3/eigeningenuity/
--rw-r--r--   0 berhic     (501) staff       (20)     1203 2023-04-06 15:03:48.000000 python-eigen-ingenuity-0.4.7.3/eigeningenuity/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)    16232 2023-05-18 14:59:11.000000 python-eigen-ingenuity-0.4.7.3/eigeningenuity/assetmodel.py
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-22 10:03:07.477867 python-eigen-ingenuity-0.4.7.3/eigeningenuity/core/
--rw-r--r--   0 berhic     (501) staff       (20)     7715 2023-04-06 10:18:46.000000 python-eigen-ingenuity-0.4.7.3/eigeningenuity/core/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.3/eigeningenuity/core/debug.py
--rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.7.3/eigeningenuity/elastic.py
--rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.7.3/eigeningenuity/events.py
--rw-r--r--   0 berhic     (501) staff       (20)    36274 2023-05-22 10:02:52.000000 python-eigen-ingenuity-0.4.7.3/eigeningenuity/historian.py
--rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.7.3/eigeningenuity/smartdash.py
--rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.7.3/eigeningenuity/sql.py
--rw-r--r--   0 berhic     (501) staff       (20)    12181 2023-05-18 15:50:36.000000 python-eigen-ingenuity-0.4.7.3/eigeningenuity/util.py
--rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.3/pyproject.toml
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-22 10:03:07.478881 python-eigen-ingenuity-0.4.7.3/python_eigen_ingenuity.egg-info/
--rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-05-22 10:03:07.000000 python-eigen-ingenuity-0.4.7.3/python_eigen_ingenuity.egg-info/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)      551 2023-05-22 10:03:07.000000 python-eigen-ingenuity-0.4.7.3/python_eigen_ingenuity.egg-info/SOURCES.txt
--rw-r--r--   0 berhic     (501) staff       (20)        1 2023-05-22 10:03:07.000000 python-eigen-ingenuity-0.4.7.3/python_eigen_ingenuity.egg-info/dependency_links.txt
--rw-r--r--   0 berhic     (501) staff       (20)       24 2023-05-22 10:03:07.000000 python-eigen-ingenuity-0.4.7.3/python_eigen_ingenuity.egg-info/requires.txt
--rw-r--r--   0 berhic     (501) staff       (20)       15 2023-05-22 10:03:07.000000 python-eigen-ingenuity-0.4.7.3/python_eigen_ingenuity.egg-info/top_level.txt
--rw-r--r--   0 berhic     (501) staff       (20)       38 2023-05-22 10:03:07.479483 python-eigen-ingenuity-0.4.7.3/setup.cfg
--rw-r--r--   0 berhic     (501) staff       (20)      691 2023-05-22 09:58:25.000000 python-eigen-ingenuity-0.4.7.3/setup.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.729014 python-eigen-ingenuity-0.4.8/
+-rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/LICENSE
+-rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.8/MANIFEST.in
+-rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-06-07 12:12:42.728734 python-eigen-ingenuity-0.4.8/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/README.md
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.727292 python-eigen-ingenuity-0.4.8/eigeningenuity/
+-rw-r--r--   0 berhic     (501) staff       (20)     1205 2023-05-23 15:38:30.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)    16232 2023-05-18 14:59:11.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/assetmodel.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.727647 python-eigen-ingenuity-0.4.8/eigeningenuity/core/
+-rw-r--r--   0 berhic     (501) staff       (20)     7741 2023-05-23 15:25:59.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/core/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/core/debug.py
+-rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/elastic.py
+-rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/events.py
+-rw-r--r--   0 berhic     (501) staff       (20)    36274 2023-05-24 08:12:38.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/historian.py
+-rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/smartdash.py
+-rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/sql.py
+-rw-r--r--   0 berhic     (501) staff       (20)    15067 2023-06-07 12:09:52.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/util.py
+-rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/pyproject.toml
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.728508 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/
+-rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)      551 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/SOURCES.txt
+-rw-r--r--   0 berhic     (501) staff       (20)        1 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/dependency_links.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       24 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/requires.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       15 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/top_level.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       38 2023-06-07 12:12:42.729074 python-eigen-ingenuity-0.4.8/setup.cfg
+-rw-r--r--   0 berhic     (501) staff       (20)      689 2023-06-07 12:12:34.000000 python-eigen-ingenuity-0.4.8/setup.py
```

### Comparing `python-eigen-ingenuity-0.4.7.3/LICENSE` & `python-eigen-ingenuity-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.3/PKG-INFO` & `python-eigen-ingenuity-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.7.3
+Version: 0.4.8
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.7.3/README.md` & `python-eigen-ingenuity-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.3/eigeningenuity/__init__.py` & `python-eigen-ingenuity-0.4.8/eigeningenuity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 from eigeningenuity.assetmodel import get_assetmodel
 from eigeningenuity.smartdash import get_smartdash
 from eigeningenuity.sql import get_sql
 
 from eigeningenuity.core import *
 
 __all__ = ["get_historian", "get_assetmodel", "get_elastic", "get_sql", "get_eventlog", "get_smartdash", "list_historians", "get_default_historian_name", "EigenServer"]
-__version__ = pkg_resources.require("python-eigen-ingenuity")[0].version
+# __version__ = pkg_resources.require("python-eigen-ingenuity")[0].version
```

### Comparing `python-eigen-ingenuity-0.4.7.3/eigeningenuity/assetmodel.py` & `python-eigen-ingenuity-0.4.8/eigeningenuity/assetmodel.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.3/eigeningenuity/core/__init__.py` & `python-eigen-ingenuity-0.4.8/eigeningenuity/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 argument, falling back on the environment variable EIGENSERVER.
 This may either be in the form of a URL (http://foo:8087/) or a
 hostname, or hostname:port combination. If no variable is set, it defaults
 to http://localhost:8080/
 """
 
 import sys, os
-from eigeningenuity.util import _do_eigen_json_request, EigenException, RemoteServerException, serverTimeToPythonTime
+from eigeningenuity.util import _do_eigen_json_request, EigenException, RemoteServerException, serverTimeToPythonTime, _authenticate_azure_user
 
 _INSTANCE = None
 class EigenServer (object):
     def __init__(self, name:str = None, disableSsl = False):
         """Takes the base URL for the Eigen Ingenuity server.
         """
         if name is None:
```

### Comparing `python-eigen-ingenuity-0.4.7.3/eigeningenuity/core/debug.py` & `python-eigen-ingenuity-0.4.8/eigeningenuity/core/debug.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.3/eigeningenuity/elastic.py` & `python-eigen-ingenuity-0.4.8/eigeningenuity/elastic.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.3/eigeningenuity/events.py` & `python-eigen-ingenuity-0.4.8/eigeningenuity/events.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.3/eigeningenuity/historian.py` & `python-eigen-ingenuity-0.4.8/eigeningenuity/historian.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.3/eigeningenuity/smartdash.py` & `python-eigen-ingenuity-0.4.8/eigeningenuity/smartdash.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.3/eigeningenuity/sql.py` & `python-eigen-ingenuity-0.4.8/eigeningenuity/sql.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.3/eigeningenuity/util.py` & `python-eigen-ingenuity-0.4.8/eigeningenuity/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,98 @@
 
-import sys, os, json, time, requests, csv
+import sys, os, json, time, requests, csv, msal, atexit
 from datetime import datetime
 import pandas as pd
 from collections import ChainMap
 from urllib.parse import urlsplit, quote as urlquote
 
 from requests.exceptions import ConnectionError
 
 from eigeningenuity.core.debug import _debug
 
+def _authenticate_azure_user(baseurl):
+    cache = msal.SerializableTokenCache()
+
+    if not os.path.exists(os.path.dirname(__file__) + '/.azure'):
+        os.mkdir(os.path.dirname(__file__) + "/.azure")
+    if os.path.exists(os.path.dirname(__file__) + "/.azure/token_cache.bin"):
+        cache.deserialize(open(os.path.dirname(__file__) + "/.azure/token_cache.bin", "r").read())
+    atexit.register(lambda:
+        open(os.path.dirname(__file__) + "/.azure/token_cache.bin", "w").write(cache.serialize())
+        if cache.has_state_changed else None
+        )
+
+    client_id = os.environ["CLIENTID"]
+    tenant_id = os.environ["TENANTID"]
+    authority = f'https://login.microsoftonline.com/{tenant_id}'
+    scope=[f"{baseurl}/user_impersonation"]
+
+    app = msal.PublicClientApplication(
+        client_id=client_id,
+        authority=authority,
+        token_cache=cache
+    )
+
+    result=None
+
+    # We now check the cache to see
+    # whether we already have some accounts that the end user already used to sign in before.
+    accounts = app.get_accounts()
+    if accounts:
+        account = 0
+        # If so, you could then somehow display these accounts and let end user choose
+        if len(accounts) >= 2:
+            print("Found Multiple Users in Cache")
+            while True:
+                for idx,a in enumerate(accounts):
+                    print(f'{idx}: {a["username"]}')
+                try:
+                    account = int(input("Enter the number of the account you want to use:\n"))
+                    if account not in list(range(len(accounts))):
+                        print("That is not a valid option!")
+                    else:
+                        break
+                except:
+                    print("That is not a valid option!")
+
+        # Assuming the end user chose this one
+        chosen = accounts[account]
+        # Now let's try to find a token in cache for this account
+        result = app.acquire_token_silent(scope, account=chosen)
+
+
+    if not result:
+        # So no suitable token exists in cache. Let's get a new one from Azure AD.
+        # result = app.ACQUIRE_TOKEN_INTERACTIVE(flow)
+        result = app.acquire_token_interactive(scope)
+
+    if "access_token" in result:
+        access_token = (result["access_token"])  # Yay!
+    else:
+        print(result.get("error"))
+        print(result.get("error_description"))
+        print(result.get("correlation_id"))  # You may need this when reporting a bug
+
+    # Make requests to the Java API using the obtained access token
+    return {
+        'Authorization': f'Bearer {access_token}',
+        'Accept': 'application/json',
+        'Content-Type': 'application/json'
+    }
+
+
 def _do_eigen_json_request(requesturl,**params):
 
+    headers = {}
+
+    
+
+    if os.getenv("TENANTID") and os.getenv("CLIENTID"):
+        headers = _authenticate_azure_user('/'.join(requesturl.split("/")[0:3]))
+
     if params:
         if "?" in requesturl:
             sep = "&"
         else:
             sep = "?"
 
         for k,v in params.items():
@@ -28,21 +106,20 @@
                         else:
                             e = str(e)
                     requesturl += sep + urlquote(k) + "=" + urlquote(e.encode("UTF8"))
 
                     sep = "&"
 
 
-
     _debug("DEBUG",requesturl)
     if 'DEBUG' in os.environ and os.environ['DEBUG']:
         print("DEBUG: [" + requesturl + "]", file=sys.stderr)
 
     try:
-        data = requests.get(requesturl, verify=False)
+        data = requests.get(requesturl, headers=headers, verify=False)
     except ConnectionError as e:
         # sys.tracebacklimit = 0
         raise EigenException("No Response from ingenuity instance at https://" + requesturl.split("/")[2] + ". Please check this is correct url and that the instance is currently running") from None
 
 
     if data.text.startswith("ERROR:"):
         if "UNKNOWN TAG" in data.text:
@@ -55,15 +132,15 @@
             ret = data.json()
         except ValueError:
             ret = data.text
 
     return ret
 
 def _do_eigen_post_request(posturl,data):
-    requests.post(posturl,data, verify=False)
+    requests.post(posturl,data, headers=False)
     pass
 
 def is_list(x):
     return type(x) in (list, tuple, set)
 
 def force_list(x):
     if is_list(x):
```

### Comparing `python-eigen-ingenuity-0.4.7.3/python_eigen_ingenuity.egg-info/PKG-INFO` & `python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.7.3
+Version: 0.4.8
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.7.3/python_eigen_ingenuity.egg-info/SOURCES.txt` & `python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.3/setup.py` & `python-eigen-ingenuity-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README = (HERE / "README.md").read_text()
 
 pkgname = 'python-eigen-ingenuity'
 
 # Invoke setup
 setup(
     name=pkgname,
-    version='0.4.7.3',
+    version='0.4.8',
     author='Murray Callander',
     author_email='info@eigen.co',
     url='https://www.eigen.co/',
     description="A python library used to query data from the Eigen Ingenuity system",
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages("."),
```

