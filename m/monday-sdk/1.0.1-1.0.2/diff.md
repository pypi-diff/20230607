# Comparing `tmp/monday_sdk-1.0.1.tar.gz` & `tmp/monday_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monday_sdk-1.0.1.tar", max compression
+gzip compressed data, was "monday_sdk-1.0.2.tar", max compression
```

## Comparing `monday_sdk-1.0.1.tar` & `monday_sdk-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1089 2023-06-07 00:26:52.038137 monday_sdk-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-05-08 16:00:48.272318 monday_sdk-1.0.1/monday_sdk/__init__.py
--rw-r--r--   0        0        0     2239 2023-06-07 00:14:15.237710 monday_sdk-1.0.1/monday_sdk/authentication.py
--rw-r--r--   0        0        0      514 2023-06-07 00:14:23.454810 monday_sdk-1.0.1/monday_sdk/graphql_loader.py
--rw-r--r--   0        0        0     3031 2023-06-07 00:14:49.820809 monday_sdk-1.0.1/monday_sdk/monday.py
--rw-r--r--   0        0        0      700 2023-06-07 00:26:13.629056 monday_sdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       29 2023-06-07 00:12:01.661191 monday_sdk-1.0.1/README.md
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 monday_sdk-1.0.1/setup.py
--rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 monday_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-07 00:26:52.038137 monday_sdk-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      499 2023-06-07 13:59:00.004287 monday_sdk-1.0.2/monday_sdk/__init__.py
+-rw-r--r--   0        0        0     2716 2023-06-07 14:47:27.857230 monday_sdk-1.0.2/monday_sdk/authentication.py
+-rw-r--r--   0        0        0      837 2023-06-07 14:19:23.747742 monday_sdk-1.0.2/monday_sdk/graphql_loader.py
+-rw-r--r--   0        0        0     3792 2023-06-07 14:48:23.344238 monday_sdk-1.0.2/monday_sdk/monday.py
+-rw-r--r--   0        0        0      739 2023-06-07 14:48:34.513570 monday_sdk-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-06-07 00:12:01.661191 monday_sdk-1.0.2/README.md
+-rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 monday_sdk-1.0.2/setup.py
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 monday_sdk-1.0.2/PKG-INFO
```

### Comparing `monday_sdk-1.0.1/LICENSE.txt` & `monday_sdk-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `monday_sdk-1.0.1/monday_sdk/authentication.py` & `monday_sdk-1.0.2/monday_sdk/authentication.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,73 +10,84 @@
 
 from starlette import status
 from jwt.exceptions import InvalidTokenError
 from pydantic import BaseModel
 
 
 WebToken = TypedDict(
-    'WebToken',
+    "WebToken",
     {
-        'accountId': int,
-        'userId': int,
-        'aud': str,
-        'exp': int,
-        'iat': int,
-        'shortLivedToken': str,
+        "accountId": int,
+        "userId": int,
+        "aud": str,
+        "exp": int,
+        "iat": int,
+        "shortLivedToken": str,
     }
 )
 
 
 class AuthResponse(BaseModel):
+    """
+    Response model for the authentication endpoint.
+
+    Returns a status code and a JSON web token if the request is valid.
+    If the request is invalid, returns a status code and an error message
+    accessible via the `data` attribute.
+    """
     status: int
     data: str | None = None
     webtoken: WebToken | None = None
 
 
-def decode(authorization: str, secret: str = '') -> WebToken:
+def _decode(authorization: str, secret: str = "") -> WebToken:
     decoded = jwt.decode(
         authorization,
-        os.environ.get('SIGNING_SECRET', secret),
-        algorithms=['HS256'],
+        os.environ.get("SIGNING_SECRET", secret),
+        algorithms=["HS256"],
         options={
-            'verify_aud': False,
+            "verify_aud": False,
         },
     )
+
     return cast(WebToken, decoded)
 
 
 def authenticate(req: Request) -> AuthResponse:
     """
     Process an inbound request and authenticate against the monday.com API.
 
+    Currently, the `req` parameter must be a `starlette.requests.Request`
+    instance. Support for request types from other libraries---or a more
+    generalized request type---will be added in the future.
+
     If the request contains a valid token, the token will be decoded and
     returned in the response with HTTP status 200. If the token is invalid,
     the response will contain an error message with HTTP status 401.
     """
     try:
-
         authorization = req.headers.get(
-            'Authorization',
-            req.query_params.get('token', '') if req.query_params else '',
+            "Authorization",
+            req.query_params.get("token", "") if req.query_params else "",
         )
 
-        decoded = decode(cast(str, authorization))
+        decoded = _decode(cast(str, authorization))
 
-        if pdl.now() >= pdl.from_timestamp(decoded['exp']):
+        if pdl.now() >= pdl.from_timestamp(decoded["exp"]):
             raise InvalidTokenError("Token has expired")
 
         return AuthResponse(
             status=status.HTTP_200_OK,
             webtoken={
-                'accountId': decoded['accountId'],
-                'userId': decoded['userId'],
-                'aud': decoded['aud'],
-                'exp': decoded['exp'],
-                'iat': decoded['iat'],
-                'shortLivedToken': decoded['shortLivedToken'],
+                "accountId": decoded["accountId"],
+                "userId": decoded["userId"],
+                "aud": decoded["aud"],
+                "exp": decoded["exp"],
+                "iat": decoded["iat"],
+                "shortLivedToken": decoded["shortLivedToken"],
             }
         )
 
     except InvalidTokenError as err:
         return AuthResponse(
             status=status.HTTP_401_UNAUTHORIZED,
             data=json.dumps(err.args),
```

### Comparing `monday_sdk-1.0.1/setup.py` & `monday_sdk-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 packages = \
 ['monday_sdk']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.88.0,<0.89.0', 'pendulum>=2.1.2,<3.0.0']
+['fastapi>=0.88.0,<0.89.0',
+ 'flask>=2.3.2,<3.0.0',
+ 'pendulum>=2.1.2,<3.0.0',
+ 'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'monday-sdk',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': '',
     'long_description': '# Python SDK for monday.com\n',
     'author': 'Jonathan Crum',
     'author_email': 'jcrum@theobogroup.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/krummja/MondaySDK.git',
```

### Comparing `monday_sdk-1.0.1/PKG-INFO` & `monday_sdk-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: monday-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Home-page: https://github.com/krummja/MondaySDK.git
 Author: Jonathan Crum
 Author-email: jcrum@theobogroup.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: fastapi (>=0.88.0,<0.89.0)
+Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
+Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Project-URL: Repository, https://github.com/krummja/MondaySDK.git
 Description-Content-Type: text/markdown
 
 # Python SDK for monday.com
```

