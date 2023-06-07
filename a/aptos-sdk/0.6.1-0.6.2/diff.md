# Comparing `tmp/aptos_sdk-0.6.1.tar.gz` & `tmp/aptos_sdk-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aptos_sdk-0.6.1.tar", max compression
+gzip compressed data, was "aptos_sdk-0.6.2.tar", max compression
```

## Comparing `aptos_sdk-0.6.1.tar` & `aptos_sdk-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     2743 2023-03-31 16:40:44.468455 aptos_sdk-0.6.1/README.md
--rw-r--r--   0        0        0       70 2023-03-25 17:54:29.320812 aptos_sdk-0.6.1/aptos_sdk/__init__.py
--rw-r--r--   0        0        0     5651 2023-03-31 16:40:44.468580 aptos_sdk-0.6.1/aptos_sdk/account.py
--rw-r--r--   0        0        0     5873 2023-05-10 13:54:28.475480 aptos_sdk-0.6.1/aptos_sdk/account_address.py
--rw-r--r--   0        0        0    18891 2023-05-10 13:54:28.476911 aptos_sdk-0.6.1/aptos_sdk/aptos_token_client.py
--rw-r--r--   0        0        0    26404 2023-05-10 13:54:28.477184 aptos_sdk-0.6.1/aptos_sdk/async_client.py
--rw-r--r--   0        0        0     5811 2023-03-31 16:40:44.469044 aptos_sdk-0.6.1/aptos_sdk/authenticator.py
--rw-r--r--   0        0        0    10447 2023-03-25 17:54:29.321178 aptos_sdk-0.6.1/aptos_sdk/bcs.py
--rw-r--r--   0        0        0    24234 2023-05-10 13:54:28.477387 aptos_sdk-0.6.1/aptos_sdk/client.py
--rw-r--r--   0        0        0    12056 2023-03-31 16:40:44.469357 aptos_sdk-0.6.1/aptos_sdk/ed25519.py
--rw-r--r--   0        0        0    26552 2023-05-10 13:54:28.477553 aptos_sdk-0.6.1/aptos_sdk/transactions.py
--rw-r--r--   0        0        0     8991 2023-03-25 17:54:29.321627 aptos_sdk-0.6.1/aptos_sdk/type_tag.py
--rw-r--r--   0        0        0      742 2023-05-11 08:18:57.258580 aptos_sdk-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3625 1970-01-01 00:00:00.000000 aptos_sdk-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     2746 2023-06-06 10:45:46.911352 aptos_sdk-0.6.2/README.md
+-rw-r--r--   0        0        0       70 2023-03-20 22:18:46.787532 aptos_sdk-0.6.2/aptos_sdk/__init__.py
+-rw-r--r--   0        0        0     5651 2023-03-22 16:06:08.428473 aptos_sdk-0.6.2/aptos_sdk/account.py
+-rw-r--r--   0        0        0     5873 2023-05-12 23:36:33.034261 aptos_sdk-0.6.2/aptos_sdk/account_address.py
+-rw-r--r--   0        0        0    18891 2023-06-01 17:39:30.476859 aptos_sdk-0.6.2/aptos_sdk/aptos_token_client.py
+-rw-r--r--   0        0        0    26553 2023-06-06 10:45:46.911540 aptos_sdk-0.6.2/aptos_sdk/async_client.py
+-rw-r--r--   0        0        0     5811 2023-03-27 16:58:44.414814 aptos_sdk-0.6.2/aptos_sdk/authenticator.py
+-rw-r--r--   0        0        0    10447 2023-03-20 22:18:46.787856 aptos_sdk-0.6.2/aptos_sdk/bcs.py
+-rw-r--r--   0        0        0    24350 2023-06-06 10:45:46.911858 aptos_sdk-0.6.2/aptos_sdk/client.py
+-rw-r--r--   0        0        0    12056 2023-03-27 16:58:44.414953 aptos_sdk-0.6.2/aptos_sdk/ed25519.py
+-rw-r--r--   0        0        0      277 2023-06-06 10:45:46.912067 aptos_sdk-0.6.2/aptos_sdk/metadata.py
+-rw-r--r--   0        0        0    26552 2023-06-01 17:39:30.543085 aptos_sdk-0.6.2/aptos_sdk/transactions.py
+-rw-r--r--   0        0        0     8991 2023-03-20 22:18:46.788343 aptos_sdk-0.6.2/aptos_sdk/type_tag.py
+-rw-r--r--   0        0        0      763 2023-06-06 10:45:46.912325 aptos_sdk-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3670 1970-01-01 00:00:00.000000 aptos_sdk-0.6.2/PKG-INFO
```

### Comparing `aptos_sdk-0.6.1/README.md` & `aptos_sdk-0.6.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -69,8 +69,8 @@
 This project follows [semver](https://semver.org/) as closely as possible
 
 [repo]: https://github.com/aptos-labs/aptos-core
 [pypi-image-version]: https://img.shields.io/pypi/v/aptos-sdk.svg
 [pypi-image-downloads]: https://img.shields.io/pypi/dm/aptos-sdk.svg
 [pypi-url]: https://pypi.org/project/aptos-sdk
 [discord-image]: https://img.shields.io/discord/945856774056083548?label=Discord&logo=discord&style=flat~~~~
-[discord-url]: https://discord.gg/aptoslabs
+[discord-url]: https://discord.gg/aptosnetwork
```

### Comparing `aptos_sdk-0.6.1/aptos_sdk/account.py` & `aptos_sdk-0.6.2/aptos_sdk/account.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.1/aptos_sdk/account_address.py` & `aptos_sdk-0.6.2/aptos_sdk/account_address.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.1/aptos_sdk/aptos_token_client.py` & `aptos_sdk-0.6.2/aptos_sdk/aptos_token_client.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.1/aptos_sdk/async_client.py` & `aptos_sdk-0.6.2/aptos_sdk/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import httpx
 
 from . import ed25519
 from .account import Account
 from .account_address import AccountAddress
 from .authenticator import Authenticator, Ed25519Authenticator, MultiAgentAuthenticator
 from .bcs import Serializer
+from .metadata import Metadata
 from .transactions import (
     EntryFunction,
     MultiAgentRawTransaction,
     RawTransaction,
     SignedTransaction,
     TransactionArgument,
     TransactionPayload,
@@ -45,16 +46,18 @@
     def __init__(self, base_url: str, client_config: ClientConfig = ClientConfig()):
         self.base_url = base_url
         # Default limits
         limits = httpx.Limits()
         # Default timeouts but do not set a pool timeout, since the idea is that jobs will wait as
         # long as progress is being made.
         timeout = httpx.Timeout(60.0, pool=None)
+        # Default headers
+        headers = {Metadata.APTOS_HEADER: Metadata.get_aptos_header_val()}
         self.client = httpx.AsyncClient(
-            http2=client_config.http2, limits=limits, timeout=timeout
+            http2=client_config.http2, limits=limits, timeout=timeout, headers=headers
         )
         self.client_config = client_config
         self._chain_id = None
 
     async def close(self):
         await self.client.aclose()
```

### Comparing `aptos_sdk-0.6.1/aptos_sdk/authenticator.py` & `aptos_sdk-0.6.2/aptos_sdk/authenticator.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.1/aptos_sdk/bcs.py` & `aptos_sdk-0.6.2/aptos_sdk/bcs.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.1/aptos_sdk/client.py` & `aptos_sdk-0.6.2/aptos_sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import httpx
 
 from . import ed25519
 from .account import Account
 from .account_address import AccountAddress
 from .authenticator import Authenticator, Ed25519Authenticator, MultiAgentAuthenticator
 from .bcs import Serializer
+from .metadata import Metadata
 from .transactions import (
     EntryFunction,
     MultiAgentRawTransaction,
     RawTransaction,
     SignedTransaction,
     TransactionArgument,
     TransactionPayload,
@@ -40,14 +41,15 @@
     client: httpx.Client
     client_config: ClientConfig
     base_url: str
 
     def __init__(self, base_url: str, client_config: ClientConfig = ClientConfig()):
         self.base_url = base_url
         self.client = httpx.Client()
+        self.client.headers[Metadata.APTOS_HEADER] = Metadata.get_aptos_header_val()
         self.client_config = client_config
         self.chain_id = int(self.info()["chain_id"])
 
     def close(self):
         self.client.close()
 
     #
```

### Comparing `aptos_sdk-0.6.1/aptos_sdk/ed25519.py` & `aptos_sdk-0.6.2/aptos_sdk/ed25519.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.1/aptos_sdk/transactions.py` & `aptos_sdk-0.6.2/aptos_sdk/transactions.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.1/aptos_sdk/type_tag.py` & `aptos_sdk-0.6.2/aptos_sdk/type_tag.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.1/pyproject.toml` & `aptos_sdk-0.6.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "aptos-sdk"
-version = "0.6.1"
+version = "0.6.2"
 description = "Aptos SDK"
 authors = ["Aptos Labs <opensource@aptoslabs.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/aptos-labs/aptos-core"
 homepage = "https://github.com/aptos-labs/aptos-core/tree/main/ecosystem/python/sdk"
 keywords = ["web3", "sdk", "aptos", "blockchain"]
 
 [tool.poetry.dependencies]
 h2 = "^4.1.0"
 httpx = "^0.23.0"
 PyNaCl = "^1.5.0"
 python = ">=3.7,<4.0"
+importlib = "^1.0.4"
 
 [tool.poetry.dev-dependencies]
 autoflake = "1.4.0"
 black = "^22.6.0"
 flake8 = ">=3.8.3,<6.0.0"
 isort = "^5.10.1"
 mypy = "^0.982"
```

### Comparing `aptos_sdk-0.6.1/PKG-INFO` & `aptos_sdk-0.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aptos-sdk
-Version: 0.6.1
+Version: 0.6.2
 Summary: Aptos SDK
 Home-page: https://github.com/aptos-labs/aptos-core/tree/main/ecosystem/python/sdk
 License: Apache-2.0
 Keywords: web3,sdk,aptos,blockchain
 Author: Aptos Labs
 Author-email: opensource@aptoslabs.com
 Requires-Python: >=3.7,<4.0
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyNaCl (>=1.5.0,<2.0.0)
 Requires-Dist: h2 (>=4.1.0,<5.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: importlib (>=1.0.4,<2.0.0)
 Project-URL: Repository, https://github.com/aptos-labs/aptos-core
 Description-Content-Type: text/markdown
 
 # Aptos Python SDK
 [![Discord][discord-image]][discord-url]
 [![PyPI Package Version][pypi-image-version]][pypi-url]
 [![PyPI Package Downloads][pypi-image-downloads]][pypi-url]
@@ -92,9 +93,9 @@
 This project follows [semver](https://semver.org/) as closely as possible
 
 [repo]: https://github.com/aptos-labs/aptos-core
 [pypi-image-version]: https://img.shields.io/pypi/v/aptos-sdk.svg
 [pypi-image-downloads]: https://img.shields.io/pypi/dm/aptos-sdk.svg
 [pypi-url]: https://pypi.org/project/aptos-sdk
 [discord-image]: https://img.shields.io/discord/945856774056083548?label=Discord&logo=discord&style=flat~~~~
-[discord-url]: https://discord.gg/aptoslabs
+[discord-url]: https://discord.gg/aptosnetwork
```

