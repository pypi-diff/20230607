# Comparing `tmp/skyflow-1.8.1.tar.gz` & `tmp/skyflow-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyflow-1.8.1.tar", last modified: Fri Mar 17 12:32:25 2023, max compression
+gzip compressed data, was "skyflow-1.9.0.tar", last modified: Wed Jun  7 11:54:49 2023, max compression
```

## Comparing `skyflow-1.8.1.tar` & `skyflow-1.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:32:25.483512 skyflow-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-17 12:32:11.000000 skyflow-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-17 12:32:25.483512 skyflow-1.8.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-03-17 12:32:11.000000 skyflow-1.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 12:32:25.483512 skyflow-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-17 12:32:22.000000 skyflow-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:32:25.479512 skyflow-1.8.1/skyflow/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:32:25.479512 skyflow-1.8.1/skyflow/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/errors/_skyflow_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:32:25.479512 skyflow-1.8.1/skyflow/service_account/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/service_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/service_account/_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/service_account/_validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:32:25.483512 skyflow-1.8.1/skyflow/vault/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/vault/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/vault/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/vault/_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/vault/_detokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/vault/_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/vault/_get_by_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/vault/_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/vault/_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-03-17 12:32:11.000000 skyflow-1.8.1/skyflow/vault/_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:32:25.479512 skyflow-1.8.1/skyflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-17 12:32:25.000000 skyflow-1.8.1/skyflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-17 12:32:25.000000 skyflow-1.8.1/skyflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 12:32:25.000000 skyflow-1.8.1/skyflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-17 12:32:25.000000 skyflow-1.8.1/skyflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-17 12:32:25.000000 skyflow-1.8.1/skyflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 11:54:36.000000 skyflow-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-07 11:54:49.768780 skyflow-1.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-06-07 11:54:36.000000 skyflow-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 11:54:49.768780 skyflow-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-07 11:54:46.000000 skyflow-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/skyflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/skyflow/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/errors/_skyflow_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/skyflow/service_account/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/service_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/service_account/_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/service_account/_validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/skyflow/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_get_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-07 11:54:36.000000 skyflow-1.9.0/skyflow/vault/_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:54:49.768780 skyflow-1.9.0/skyflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-07 11:54:49.000000 skyflow-1.9.0/skyflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 11:54:49.000000 skyflow-1.9.0/skyflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:54:49.000000 skyflow-1.9.0/skyflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 11:54:49.000000 skyflow-1.9.0/skyflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 11:54:49.000000 skyflow-1.9.0/skyflow.egg-info/top_level.txt
```

### Comparing `skyflow-1.8.1/LICENSE` & `skyflow-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skyflow-1.8.1/PKG-INFO` & `skyflow-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyflow
-Version: 1.8.1
+Version: 1.9.0
 Summary: Skyflow SDK for the Python programming language
 Home-page: https://github.com/skyflowapi/skyflow-python/
 Author: Skyflow
 Author-email: service-ops@skyflow.com
 License: LICENSE
 Requires-Python: >=3.7
 License-File: LICENSE
```

### Comparing `skyflow-1.8.1/README.rst` & `skyflow-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `skyflow-1.8.1/setup.py` & `skyflow-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 	Copyright (c) 2022 Skyflow, Inc.
 '''
 from setuptools import setup, find_packages
 import sys
 
 if sys.version_info < (3, 7):
     raise RuntimeError("skyflow requires Python 3.7+")
-current_version = '1.8.1'
+current_version = '1.9.0'
 
 setup(
     name='skyflow',
     version=current_version,
     author='Skyflow',
     author_email='service-ops@skyflow.com',
     packages=find_packages(where='.', exclude=['test*']),
```

### Comparing `skyflow-1.8.1/skyflow/_utils.py` & `skyflow-1.9.0/skyflow/_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 '''
 	Copyright (c) 2022 Skyflow, Inc.
 '''
 import urllib.parse
 import logging
 from enum import Enum
+import platform
+import sys
+from version import SDK_VERSION
 
 skyflowLog = logging.getLogger('skyflow')
 skyflowLog.setLevel(logging.ERROR)
 
 supported_content_types = {
     "JSON": 'application/json',
     "PLAINTEXT": 'text/plain',
@@ -123,7 +126,35 @@
     '''
     depth, outStr = 0, ''
     for x in parents:
         s = "[%s]" if depth > 0 or isinstance(x, int) else "%s"
         outStr += s % str(x)
         depth += 1
     return outStr
+
+def getMetrics():
+    ''' fetch metrics
+    '''
+    sdk_name_version = "skyflow-python@" + SDK_VERSION
+
+    try:
+        sdk_client_device_model = platform.node()
+    except Exception:
+        sdk_client_device_model = ""
+
+    try:
+        sdk_client_os_details = sys.platform
+    except Exception:
+        sdk_client_os_details = ""
+
+    try:
+        sdk_runtime_details = sys.version
+    except Exception:
+        sdk_runtime_details = ""
+
+    details_dic = {
+        'sdk_name_version': sdk_name_version,
+        'sdk_client_device_model': sdk_client_device_model,
+        'sdk_client_os_details': sdk_client_os_details,
+        'sdk_runtime_details': "Python " + sdk_runtime_details,
+    }
+    return details_dic
```

### Comparing `skyflow-1.8.1/skyflow/errors/_skyflow_errors.py` & `skyflow-1.9.0/skyflow/errors/_skyflow_errors.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.8.1/skyflow/service_account/_token.py` & `skyflow-1.9.0/skyflow/service_account/_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 '''
 import json
 import jwt
 import datetime
 import requests
 from warnings import warn
 from collections import namedtuple
-from skyflow._utils import log_info, InterfaceName, InfoMessages
+from skyflow._utils import log_info, InterfaceName, InfoMessages, getMetrics
 
 
 from skyflow.errors._skyflow_errors import *
 
 ResponseToken = namedtuple('ResponseToken', ['AccessToken', 'TokenType'])
 interface = InterfaceName.GENERATE_BEARER_TOKEN
 
@@ -122,15 +122,16 @@
     except Exception as e:
         raise SkyflowError(SkyflowErrorCodes.INVALID_INPUT,
                            SkyflowErrorMessages.JWT_INVALID_FORMAT, interface=interface)
 
 
 def sendRequestWithToken(url, token):
     headers = {
-        "content-type": "application/json"
+        "content-type": "application/json",
+        "sky-metadata": json.dumps(getMetrics())
     }
     payload = {
         "grant_type": "urn:ietf:params:oauth:grant-type:jwt-bearer",
         "assertion":  token
     }
     try:
         response = requests.post(url=url, json=payload, headers=headers)
```

### Comparing `skyflow-1.8.1/skyflow/service_account/_validity.py` & `skyflow-1.9.0/skyflow/service_account/_validity.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.8.1/skyflow/vault/_client.py` & `skyflow-1.9.0/skyflow/vault/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 '''
 	Copyright (c) 2022 Skyflow, Inc.
 '''
+import json
 import types
 import requests
 from ._insert import getInsertRequestBody, processResponse, convertResponse
 from ._update import sendUpdateRequests, createUpdateResponseBody
 from ._config import Configuration
 from ._config import InsertOptions, ConnectionConfig, UpdateOptions
 from ._connection import createRequest
 from ._detokenize import sendDetokenizeRequests, createDetokenizeResponseBody
 from ._get_by_id import sendGetByIdRequests, createGetResponseBody
 from ._get import sendGetRequests
 import asyncio
 from skyflow.errors._skyflow_errors import SkyflowError, SkyflowErrorCodes, SkyflowErrorMessages
-from skyflow._utils import log_info, InfoMessages, InterfaceName
+from skyflow._utils import log_info, InfoMessages, InterfaceName, getMetrics
 from ._token import tokenProviderWrapper
 
 
 class Client:
     def __init__(self, config: Configuration):
 
         interface = InterfaceName.CLIENT.value
@@ -48,15 +49,16 @@
         self._checkConfig(interface)
 
         jsonBody = getInsertRequestBody(records, options)
         requestURL = self._get_complete_vault_url()
         self.storedToken = tokenProviderWrapper(
             self.storedToken, self.tokenProvider, interface)
         headers = {
-            "Authorization": "Bearer " + self.storedToken
+            "Authorization": "Bearer " + self.storedToken,
+            "sky-metadata": json.dumps(getMetrics())
         }
 
         response = requests.post(requestURL, data=jsonBody, headers=headers)
         processedResponse = processResponse(response)
         result = convertResponse(records, processedResponse, options.tokens)
 
         log_info(InfoMessages.INSERT_DATA_SUCCESS.value, interface)
@@ -127,14 +129,16 @@
         self.storedToken = tokenProviderWrapper(
             self.storedToken, self.tokenProvider, interface)
         request = createRequest(config)
 
         if not 'X-Skyflow-Authorization'.lower() in request.headers:
             request.headers['x-skyflow-authorization'] = self.storedToken
 
+        request.headers['sky-metadata'] = json.dumps(getMetrics())
+
         response = session.send(request)
         session.close()
         return processResponse(response, interface=interface)
 
     def _checkConfig(self, interface):
         '''
             Performs basic check on the given client config
```

### Comparing `skyflow-1.8.1/skyflow/vault/_config.py` & `skyflow-1.9.0/skyflow/vault/_config.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.8.1/skyflow/vault/_connection.py` & `skyflow-1.9.0/skyflow/vault/_connection.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.8.1/skyflow/vault/_detokenize.py` & `skyflow-1.9.0/skyflow/vault/_detokenize.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 '''
 	Copyright (c) 2022 Skyflow, Inc.
 '''
 from skyflow.errors._skyflow_errors import SkyflowError, SkyflowErrorCodes, SkyflowErrorMessages
 import asyncio
 from aiohttp import ClientSession, request
 import json
-from skyflow._utils import InterfaceName
+from ._config import RedactionType
+from skyflow._utils import InterfaceName, getMetrics
 
 interface = InterfaceName.DETOKENIZE.value
 
 
 def getDetokenizeRequestBody(data):
     try:
         token = data["token"]
     except KeyError:
         raise SkyflowError(SkyflowErrorCodes.INVALID_INPUT,
-                           SkyflowErrorMessages.TOKEN_KEY_ERROR, interface=interface)
+                            SkyflowErrorMessages.TOKEN_KEY_ERROR, interface=interface)
     if not isinstance(token, str):
         tokenType = str(type(token))
         raise SkyflowError(SkyflowErrorCodes.INVALID_INPUT, SkyflowErrorMessages.INVALID_TOKEN_TYPE.value % (
             tokenType), interface=interface)
+
+    if "redaction" in data:
+        if not isinstance(data["redaction"], RedactionType):
+            redactionType = str(type(data["redaction"]))
+            raise SkyflowError(SkyflowErrorCodes.INVALID_INPUT, SkyflowErrorMessages.INVALID_REDACTION_TYPE.value % (
+            redactionType), interface=interface)
+        else:
+            redactionType =  data["redaction"]
+    else:
+        redactionType = RedactionType.PLAIN_TEXT
+
     requestBody = {"detokenizationParameters": []}
     requestBody["detokenizationParameters"].append({
-        "token": token})
+        "token": token,
+        "redaction": redactionType.value
+        })
     return requestBody
 
 
 async def sendDetokenizeRequests(data, url, token):
 
     tasks = []
 
@@ -35,24 +49,25 @@
     except KeyError:
         raise SkyflowError(SkyflowErrorCodes.INVALID_INPUT,
                            SkyflowErrorMessages.RECORDS_KEY_ERROR, interface=interface)
     if not isinstance(records, list):
         recordsType = str(type(records))
         raise SkyflowError(SkyflowErrorCodes.INVALID_INPUT, SkyflowErrorMessages.INVALID_RECORDS_TYPE.value % (
             recordsType), interface=interface)
-
     validatedRecords = []
     for record in records:
         requestBody = getDetokenizeRequestBody(record)
         jsonBody = json.dumps(requestBody)
         validatedRecords.append(jsonBody)
     async with ClientSession() as session:
         for record in validatedRecords:
             headers = {
-                "Authorization": "Bearer " + token
+                "Authorization": "Bearer " + token,
+                "sky-metadata": json.dumps(getMetrics())
+
             }
             task = asyncio.ensure_future(post(url, record, headers, session))
             tasks.append(task)
         await asyncio.gather(*tasks)
         await session.close()
     return tasks
```

### Comparing `skyflow-1.8.1/skyflow/vault/_get.py` & `skyflow-1.9.0/skyflow/vault/_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 '''
 	Copyright (c) 2022 Skyflow, Inc.
 '''
+import json
 from skyflow.errors._skyflow_errors import SkyflowError, SkyflowErrorCodes, SkyflowErrorMessages
 import asyncio
 from aiohttp import ClientSession
 from ._config import RedactionType
-from skyflow._utils import InterfaceName
+from skyflow._utils import InterfaceName, getMetrics
 from ._get_by_id import get
 
 interface = InterfaceName.GET.value
 
 def getGetRequestBody(data):
     ids = None
     if "ids" in data:
@@ -79,15 +80,16 @@
     validatedRecords = []
     for record in records:
         ids, table, redaction, columnName, columnValues = getGetRequestBody(record)
         validatedRecords.append((ids, table, redaction, columnName, columnValues))
     async with ClientSession() as session:
         for record in validatedRecords:
             headers = {
-                "Authorization": "Bearer " + token
+                "Authorization": "Bearer " + token,
+                "sky-metadata": json.dumps(getMetrics())
             }
             params = {"redaction": redaction}
             if ids is not None:
                 params["skyflow_ids"] = ids
             if columnName is not None:
                 params["column_name"] = columnName
                 params["column_values"] = columnValues
```

### Comparing `skyflow-1.8.1/skyflow/vault/_get_by_id.py` & `skyflow-1.9.0/skyflow/vault/_get_by_id.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 	Copyright (c) 2022 Skyflow, Inc.
 '''
 from skyflow.errors._skyflow_errors import SkyflowError, SkyflowErrorCodes, SkyflowErrorMessages
 import asyncio
 from aiohttp import ClientSession
 import json
 from ._config import RedactionType
-from skyflow._utils import InterfaceName
+from skyflow._utils import InterfaceName, getMetrics
 
 interface = InterfaceName.GET_BY_ID.value
 
 
 def getGetByIdRequestBody(data):
     try:
         ids = data["ids"]
@@ -62,15 +62,16 @@
     validatedRecords = []
     for record in records:
         ids, table, redaction = getGetByIdRequestBody(record)
         validatedRecords.append((ids, table, redaction))
     async with ClientSession() as session:
         for record in validatedRecords:
             headers = {
-                "Authorization": "Bearer " + token
+                "Authorization": "Bearer " + token,
+                "sky-metadata": json.dumps(getMetrics())
             }
             params = {"skyflow_ids": record[0], "redaction": record[2]}
             task = asyncio.ensure_future(
                 get(url, headers, params, session, record[1]))
             tasks.append(task)
         await asyncio.gather(*tasks)
         await session.close()
```

### Comparing `skyflow-1.8.1/skyflow/vault/_insert.py` & `skyflow-1.9.0/skyflow/vault/_insert.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.8.1/skyflow/vault/_token.py` & `skyflow-1.9.0/skyflow/vault/_token.py`

 * *Files identical despite different names*

### Comparing `skyflow-1.8.1/skyflow/vault/_update.py` & `skyflow-1.9.0/skyflow/vault/_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 	Copyright (c) 2022 Skyflow, Inc.
 '''
 import json
 
 import asyncio
 from skyflow.errors._skyflow_errors import SkyflowError, SkyflowErrorCodes, SkyflowErrorMessages
 from ._insert import getTableAndFields
-from skyflow._utils import InterfaceName
+from skyflow._utils import InterfaceName, getMetrics
 from aiohttp import ClientSession
 from ._config import UpdateOptions
 
 interface = InterfaceName.UPDATE.value
 
 async def sendUpdateRequests(data,options: UpdateOptions,url,token):
     tasks = []
@@ -36,15 +36,16 @@
                 "record": {
                     "fields": record["fields"]
                 },
                 "tokenization": options.tokens
             }
             reqBody = json.dumps(reqBody)
             headers = {
-                "Authorization": "Bearer " + token
+                "Authorization": "Bearer " + token,
+                "sky-metadata": json.dumps(getMetrics())
             }
             task = asyncio.ensure_future(put(recordUrl, reqBody, headers, session))
             tasks.append(task)
         await asyncio.gather(*tasks)
         await session.close()
     return tasks
```

### Comparing `skyflow-1.8.1/skyflow.egg-info/PKG-INFO` & `skyflow-1.9.0/skyflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyflow
-Version: 1.8.1
+Version: 1.9.0
 Summary: Skyflow SDK for the Python programming language
 Home-page: https://github.com/skyflowapi/skyflow-python/
 Author: Skyflow
 Author-email: service-ops@skyflow.com
 License: LICENSE
 Requires-Python: >=3.7
 License-File: LICENSE
```

### Comparing `skyflow-1.8.1/skyflow.egg-info/SOURCES.txt` & `skyflow-1.9.0/skyflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

