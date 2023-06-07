# Comparing `tmp/osim_utils-0.4.2.tar.gz` & `tmp/osim_utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osim_utils-0.4.2.tar", max compression
+gzip compressed data, was "osim_utils-0.5.0.tar", max compression
```

## Comparing `osim_utils-0.4.2.tar` & `osim_utils-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.4.2/README.md
--rw-r--r--   0        0        0     1446 2023-05-08 15:34:27.529473 osim_utils-0.4.2/osim_utils/clients/crossref.py
--rw-r--r--   0        0        0     6886 2023-05-03 10:56:19.733447 osim_utils-0.4.2/osim_utils/clients/epmc.py
--rw-r--r--   0        0        0     4130 2023-05-03 16:19:44.648513 osim_utils-0.4.2/osim_utils/clients/openalex.py
--rw-r--r--   0        0        0     2539 2023-05-09 15:21:33.775514 osim_utils-0.4.2/osim_utils/clients/sherpa.py
--rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.4.2/osim_utils/common.py
--rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.4.2/osim_utils/constants.py
--rw-r--r--   0        0        0     1515 2023-05-03 13:04:39.071924 osim_utils-0.4.2/osim_utils/decorators.py
--rw-r--r--   0        0        0      716 2023-05-05 17:07:41.792972 osim_utils-0.4.2/osim_utils/exceptions.py
--rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.4.2/osim_utils/logger.py
--rw-r--r--   0        0        0      408 2023-05-09 15:24:42.422598 osim_utils-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 osim_utils-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.5.0/README.md
+-rw-r--r--   0        0        0     1446 2023-05-08 15:34:27.529473 osim_utils-0.5.0/osim_utils/clients/crossref.py
+-rw-r--r--   0        0        0     1732 2023-06-07 12:22:25.951705 osim_utils-0.5.0/osim_utils/clients/embl_data_warehouse.py
+-rw-r--r--   0        0        0     5470 2023-06-07 12:06:24.954904 osim_utils-0.5.0/osim_utils/clients/epmc.py
+-rw-r--r--   0        0        0     4130 2023-05-03 16:19:44.648513 osim_utils-0.5.0/osim_utils/clients/openalex.py
+-rw-r--r--   0        0        0     2539 2023-06-07 09:08:46.139525 osim_utils-0.5.0/osim_utils/clients/sherpa.py
+-rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.5.0/osim_utils/common.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.5.0/osim_utils/constants.py
+-rw-r--r--   0        0        0     1497 2023-06-07 12:06:24.960205 osim_utils-0.5.0/osim_utils/decorators.py
+-rw-r--r--   0        0        0      769 2023-06-07 12:00:54.184987 osim_utils-0.5.0/osim_utils/exceptions.py
+-rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.5.0/osim_utils/logger.py
+-rw-r--r--   0        0        0      408 2023-06-07 12:34:32.461580 osim_utils-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 osim_utils-0.5.0/PKG-INFO
```

### Comparing `osim_utils-0.4.2/osim_utils/clients/crossref.py` & `osim_utils-0.5.0/osim_utils/clients/crossref.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.4.2/osim_utils/clients/epmc.py` & `osim_utils-0.5.0/osim_utils/clients/epmc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,15 @@
 import functools
 import json
 import requests
 from osim_utils.logger import get_logger
 
 from http import HTTPStatus
 import osim_utils.exceptions as exc
-
-
-# region decorators
-def check_response(*args):
-    """
-    Checks that a call to a EuropePMC API client method returned an expected status code.
-    Raises an AssertionError if the returned status code is unexpected.
-
-    Args:
-        *args (tuple): status codes that should NOT lead to an
-            exception
-
-    Returns:
-        The response of the decorated method
-    """
-
-    def decorator(func):
-        @functools.wraps(func)
-        def wrapper(*inner_args, **kwargs):
-            response = func(*inner_args, **kwargs)
-            assert response.status_code in args, (
-                f"API call initiated by {func.__module__}.{func.__name__} "
-                f"returned error: {response.content}"
-            )
-            return response
-
-        return wrapper
-
-    return decorator
-
-
-def process_response(func):
-    """
-    Processes the response of a call to a EuropePMC API client method
-    so that only the body of the response is decoded form json and returned
-
-    Returns:
-        The json-decoded body of the response of the decorated method
-    """
-
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        response = func(*args, **kwargs)
-        try:
-            return response.json()
-        except json.JSONDecodeError:
-            raise exc.ApiClientError(
-                f"API call initiated by {func.__module__}.{func.__name__} "
-                f"failed with error: {response.text}"
-            )
-
-    return wrapper
-
-
-# endregion
+from osim_utils.decorators import check_response, process_response
 
 
 class EpmcClient:
     """
     API client for EuropePMC Articles REST API
     (https://europepmc.org/RestfulWebService)
     """
```

### Comparing `osim_utils-0.4.2/osim_utils/clients/openalex.py` & `osim_utils-0.5.0/osim_utils/clients/openalex.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.4.2/osim_utils/clients/sherpa.py` & `osim_utils-0.5.0/osim_utils/clients/sherpa.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.4.2/osim_utils/decorators.py` & `osim_utils-0.5.0/osim_utils/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 
 import osim_utils.exceptions as exc
 
 
 def check_response(*args):
     """
-    Checks that a call to a EuropePMC API client method returned an expected status code.
+    Checks that a call to an API client method returned an expected status code.
     Raises an AssertionError if the returned status code is unexpected.
 
     Args:
         *args (tuple): status codes that should NOT lead to an
             exception
 
     Returns:
@@ -30,15 +30,15 @@
         return wrapper
 
     return decorator
 
 
 def process_response(func):
     """
-    Processes the response of a call to a EuropePMC API client method
+    Processes the response of a call to an API client method
     so that only the body of the response is decoded form json and returned
 
     Returns:
         The json-decoded body of the response of the decorated method
     """
 
     @functools.wraps(func)
```

### Comparing `osim_utils-0.4.2/osim_utils/exceptions.py` & `osim_utils-0.5.0/osim_utils/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     pass
 
 
 class ApiClientError(DetailedError):
     pass
 
 
+class AuthenticationError(DetailedError):
+    pass
+
+
 class DuplicateValueError(DetailedError):
     pass
 
 
 class DataValidationError(DetailedError):
     pass
```

### Comparing `osim_utils-0.4.2/osim_utils/logger.py` & `osim_utils-0.5.0/osim_utils/logger.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.4.2/PKG-INFO` & `osim_utils-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osim-utils
-Version: 0.4.2
+Version: 0.5.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

