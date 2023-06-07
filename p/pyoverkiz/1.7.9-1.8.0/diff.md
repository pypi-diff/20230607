# Comparing `tmp/pyoverkiz-1.7.9.tar.gz` & `tmp/pyoverkiz-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoverkiz-1.7.9.tar", max compression
+gzip compressed data, was "pyoverkiz-1.8.0.tar", max compression
```

## Comparing `pyoverkiz-1.7.9.tar` & `pyoverkiz-1.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1073 2023-05-19 12:25:35.025662 pyoverkiz-1.7.9/LICENSE
--rw-r--r--   0        0        0     3319 2023-05-19 12:25:35.025662 pyoverkiz-1.7.9/README.md
--rw-r--r--   0        0        0        0 2023-05-19 12:25:35.037662 pyoverkiz-1.7.9/pyoverkiz/__init__.py
--rw-r--r--   0        0        0    30963 2023-05-19 12:25:35.037662 pyoverkiz-1.7.9/pyoverkiz/client.py
--rw-r--r--   0        0        0     3917 2023-05-19 12:25:35.037662 pyoverkiz-1.7.9/pyoverkiz/const.py
--rw-r--r--   0        0        0      220 2023-05-19 12:25:35.037662 pyoverkiz-1.7.9/pyoverkiz/enums/__init__.py
--rw-r--r--   0        0        0     8866 2023-05-19 12:25:35.037662 pyoverkiz-1.7.9/pyoverkiz/enums/command.py
--rw-r--r--   0        0        0     1888 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/execution.py
--rw-r--r--   0        0        0     2945 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/gateway.py
--rw-r--r--   0        0        0    17241 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/general.py
--rw-r--r--   0        0        0     2141 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/measured_value_type.py
--rw-r--r--   0        0        0     1052 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/protocol.py
--rw-r--r--   0        0        0    14019 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/state.py
--rw-r--r--   0        0        0    18302 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/ui.py
--rw-r--r--   0        0        0     1642 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/exceptions.py
--rw-r--r--   0        0        0    24495 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/models.py
--rw-r--r--   0        0        0     1869 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/obfuscate.py
--rw-r--r--   0        0        0        0 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/py.typed
--rw-r--r--   0        0        0      518 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/types.py
--rw-r--r--   0        0        0      987 2023-05-19 12:25:52.457677 pyoverkiz-1.7.9/pyproject.toml
--rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 pyoverkiz-1.7.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-07 19:12:22.663895 pyoverkiz-1.8.0/LICENSE
+-rw-r--r--   0        0        0     3319 2023-06-07 19:12:22.663895 pyoverkiz-1.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 19:12:22.675895 pyoverkiz-1.8.0/pyoverkiz/__init__.py
+-rw-r--r--   0        0        0    31572 2023-06-07 19:12:22.675895 pyoverkiz-1.8.0/pyoverkiz/client.py
+-rw-r--r--   0        0        0     3917 2023-06-07 19:12:22.675895 pyoverkiz-1.8.0/pyoverkiz/const.py
+-rw-r--r--   0        0        0      220 2023-06-07 19:12:22.675895 pyoverkiz-1.8.0/pyoverkiz/enums/__init__.py
+-rw-r--r--   0        0        0     8866 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/command.py
+-rw-r--r--   0        0        0     1888 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/execution.py
+-rw-r--r--   0        0        0     2945 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/gateway.py
+-rw-r--r--   0        0        0    17241 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/general.py
+-rw-r--r--   0        0        0     2141 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/measured_value_type.py
+-rw-r--r--   0        0        0     1052 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/protocol.py
+-rw-r--r--   0        0        0    14019 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/state.py
+-rw-r--r--   0        0        0    18346 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/ui.py
+-rw-r--r--   0        0        0     1774 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/exceptions.py
+-rw-r--r--   0        0        0    24495 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/models.py
+-rw-r--r--   0        0        0     1869 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/obfuscate.py
+-rw-r--r--   0        0        0        0 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/py.typed
+-rw-r--r--   0        0        0      518 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/types.py
+-rw-r--r--   0        0        0      987 2023-06-07 19:12:46.656016 pyoverkiz-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 pyoverkiz-1.8.0/PKG-INFO
```

### Comparing `pyoverkiz-1.7.9/LICENSE` & `pyoverkiz-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/README.md` & `pyoverkiz-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyoverkiz/client.py` & `pyoverkiz-1.8.0/pyoverkiz/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     MaintenanceException,
     MissingAuthorizationTokenException,
     NexityBadCredentialsException,
     NexityServiceException,
     NoRegisteredEventListenerException,
     NotAuthenticatedException,
     NotSuchTokenException,
+    OverkizException,
+    ServiceUnavailableException,
     SessionAndBearerInSameRequestException,
     SomfyBadCredentialsException,
     SomfyServiceException,
     TooManyAttemptsBannedException,
     TooManyConcurrentRequestsException,
     TooManyExecutionsException,
     TooManyRequestsException,
@@ -798,22 +800,35 @@
         if response.status in [200, 204]:
             return
 
         try:
             result = await response.json(content_type=None)
         except JSONDecodeError as error:
             result = await response.text()
-            if "Server is down for maintenance" in result:
+
+            if "is down for maintenance" in result:
                 raise MaintenanceException("Server is down for maintenance") from error
-            raise Exception(
+
+            if response.status == 503:
+                raise ServiceUnavailableException(result) from error
+
+            raise OverkizException(
                 f"Unknown error while requesting {response.url}. {response.status} - {result}"
             ) from error
 
         if result.get("errorCode"):
-            message = result.get("error")
+            # Error messages between cloud and local Overkiz servers can be slightly different
+            # To make it easier to have a strict match for these errors, we remove the double quotes and the period at the end.
+
+            if message := result.get("error"):
+                message = message.strip(
+                    '".'
+                )  # Change to .removesuffix when Python 3.8 support is dropped
+            else:
+                message = ""  # An error message can have an empty (None) message
 
             # {"errorCode": "AUTHENTICATION_ERROR",
             # "error": "Too many requests, try again later : login with xxx@xxx.tld"}
             if "Too many requests" in message:
                 raise TooManyRequestsException(message)
 
             # {"errorCode": "AUTHENTICATION_ERROR", "error": "Bad credentials"}
@@ -821,15 +836,15 @@
                 raise BadCredentialsException(message)
 
             # {"errorCode": "RESOURCE_ACCESS_DENIED", "error": "Not authenticated"}
             if message == "Not authenticated":
                 raise NotAuthenticatedException(message)
 
             # {"error":"Missing authorization token.","errorCode":"RESOURCE_ACCESS_DENIED"}
-            if message == "Missing authorization token.":
+            if message == "Missing authorization token":
                 raise MissingAuthorizationTokenException(message)
 
             # {"error": "Server busy, please try again later. (Too many executions)"}
             if message == "Server busy, please try again later. (Too many executions)":
                 raise TooManyExecutionsException(message)
 
             # {"error": "UNSUPPORTED_OPERATION", "error": "No such command : ..."}
@@ -847,38 +862,36 @@
             # {"errorCode": "RESOURCE_ACCESS_DENIED",  "error": "too many concurrent requests"}
             if message == "too many concurrent requests":
                 raise TooManyConcurrentRequestsException(message)
 
             if message == "Cannot use JSESSIONID and bearer token in same request":
                 raise SessionAndBearerInSameRequestException(message)
 
-            if (
-                message
-                == "Too many attempts with an invalid token, temporarily banned."
-            ):
+            if message == "Too many attempts with an invalid token, temporarily banned":
                 raise TooManyAttemptsBannedException(message)
 
             if "Invalid token : " in message:
                 raise InvalidTokenException(message)
 
             if "Not such token with UUID: " in message:
                 raise NotSuchTokenException(message)
 
             if "Unknown user :" in message:
                 raise UnknownUserException(message)
 
             # {"error":"Unknown object.","errorCode":"UNSPECIFIED_ERROR"}
-            if message == "Unknown object.":
+            if message == "Unknown object":
                 raise UnknownObjectException(message)
 
             # {'errorCode': 'RESOURCE_ACCESS_DENIED', 'error': 'Access denied to gateway #1234-5678-1234 for action ADD_TOKEN'}
             if "Access denied to gateway" in message:
                 raise AccessDeniedToGatewayException(message)
 
-        raise Exception(message if message else result)
+        # General Overkiz exception
+        raise OverkizException(result)
 
     async def _refresh_token_if_expired(self) -> None:
         """Check if token is expired and request a new one."""
         if (
             self._expires_in
             and self._refresh_token
             and self._expires_in <= datetime.datetime.now()
```

### Comparing `pyoverkiz-1.7.9/pyoverkiz/const.py` & `pyoverkiz-1.8.0/pyoverkiz/const.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyoverkiz/enums/command.py` & `pyoverkiz-1.8.0/pyoverkiz/enums/command.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyoverkiz/enums/execution.py` & `pyoverkiz-1.8.0/pyoverkiz/enums/execution.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyoverkiz/enums/gateway.py` & `pyoverkiz-1.8.0/pyoverkiz/enums/gateway.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyoverkiz/enums/general.py` & `pyoverkiz-1.8.0/pyoverkiz/enums/general.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyoverkiz/enums/measured_value_type.py` & `pyoverkiz-1.8.0/pyoverkiz/enums/measured_value_type.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyoverkiz/enums/protocol.py` & `pyoverkiz-1.8.0/pyoverkiz/enums/protocol.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyoverkiz/enums/state.py` & `pyoverkiz-1.8.0/pyoverkiz/enums/state.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyoverkiz/enums/ui.py` & `pyoverkiz-1.8.0/pyoverkiz/enums/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
     )
     CUMULATIVE_GAS_CONSUMPTION_SENSOR = "CumulativeGasConsumptionSensor"
     CUMULATIVE_THERMAL_ENERGY_CONSUMPTION_SENSOR = (
         "CumulativeThermalEnergyConsumptionSensor"
     )
     CUMULATIVE_WATER_CONSUMPTION_SENSOR = "CumulativeWaterConsumptionSensor"
     CURTAIN_TRACK_UNO = "CurtainTrackUno"
+    CYCLIC_GARAGE_DOOR = "CyclicGarageDoor"
     CYCLIC_GENERIC = "CyclicGeneric"
     DHW_SET_POINT = "DHWSetPoint"
     DE_DIETRICH_BOILER = "DeDietrichBoiler"
     DE_DIETRICH_DHW = "DeDietrichDHW"
     DE_DIETRICH_HEATING_CIRCUIT = "DeDietrichHeatingCircuit"
     DE_DIETRICH_MODBUS_GATEWAY = "DeDietrichModbusGateway"
     DE_DIETRICH_SWIMMING_POOL = "DeDietrichSwimmingPool"
```

### Comparing `pyoverkiz-1.7.9/pyoverkiz/exceptions.py` & `pyoverkiz-1.8.0/pyoverkiz/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 class BaseOverkizException(Exception):
     pass
 
 
+class OverkizException(BaseOverkizException):
+    pass
+
+
 class BadCredentialsException(BaseOverkizException):
     pass
 
 
 class InvalidCommandException(BaseOverkizException):
     pass
 
@@ -22,15 +26,19 @@
     pass
 
 
 class TooManyConcurrentRequestsException(BaseOverkizException):
     pass
 
 
-class MaintenanceException(BaseOverkizException):
+class ServiceUnavailableException(BaseOverkizException):
+    pass
+
+
+class MaintenanceException(ServiceUnavailableException):
     pass
 
 
 class MissingAuthorizationTokenException(BaseOverkizException):
     pass
```

### Comparing `pyoverkiz-1.7.9/pyoverkiz/models.py` & `pyoverkiz-1.8.0/pyoverkiz/models.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyoverkiz/obfuscate.py` & `pyoverkiz-1.8.0/pyoverkiz/obfuscate.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyoverkiz/types.py` & `pyoverkiz-1.8.0/pyoverkiz/types.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.9/pyproject.toml` & `pyoverkiz-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyoverkiz"
-version = "1.7.9"
+version = "1.8.0"
 description = "Async Python client to interact with internal OverKiz API (e.g. used by Somfy TaHoma)."
 authors = ["Mick Vleeshouwer", "Vincent Le Bourlot", "Thibaut Etienne"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/iMicknl/python-overkiz-api"
 repository = "https://github.com/iMicknl/python-overkiz-api"
 packages = [
@@ -20,15 +20,15 @@
 attrs = ">=21.2,<24.0"
 boto3 = "^1.18.59"
 warrant-lite = "^1.0.4"
 
 [tool.poetry.dev-dependencies]
 tox = "^3.28"
 pytest = "^7.3"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 pre-commit = "^2.21"
 black = {version = "^22.12", allow-prereleases = true}
 pylint = "^2.13.9"
 isort = "^5.11.5"
 mypy = "^1.3"
 flake8 = "^5.0.4"
 pyupgrade = "^3.3.2"
```

### Comparing `pyoverkiz-1.7.9/PKG-INFO` & `pyoverkiz-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoverkiz
-Version: 1.7.9
+Version: 1.8.0
 Summary: Async Python client to interact with internal OverKiz API (e.g. used by Somfy TaHoma).
 Home-page: https://github.com/iMicknl/python-overkiz-api
 License: MIT
 Author: Mick Vleeshouwer
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyoverkiz Version: 1.7.9 Summary: Async Python
+Metadata-Version: 2.1 Name: pyoverkiz Version: 1.8.0 Summary: Async Python
 client to interact with internal OverKiz API (e.g. used by Somfy TaHoma). Home-
 page: https://github.com/iMicknl/python-overkiz-api License: MIT Author: Mick
 Vleeshouwer Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

