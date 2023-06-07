# Comparing `tmp/pytonapi-0.0.3.tar.gz` & `tmp/pytonapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytonapi-0.0.3.tar", last modified: Wed May 31 20:44:56 2023, max compression
+gzip compressed data, was "pytonapi-0.0.4.tar", last modified: Wed Jun  7 00:19:07 2023, max compression
```

## Comparing `pytonapi-0.0.3.tar` & `pytonapi-0.0.4.tar`

### file list

```diff
@@ -1,47 +1,52 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.896121 pytonapi-0.0.3/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2023-05-26 17:22:12.000000 pytonapi-0.0.3/LICENSE
--rw-rw-r--   0 ness      (1000) ness      (1000)     6262 2023-05-31 20:44:56.896121 pytonapi-0.0.3/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     5860 2023-05-31 20:44:28.000000 pytonapi-0.0.3/README.md
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)       65 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/__init__.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi/async_tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1376 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1646 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi/async_tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3410 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2236 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      890 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      501 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2660 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      587 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1030 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/exceptions.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi/schema/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1713 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      460 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1660 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      349 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      318 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/domains.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      969 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      983 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2968 2023-05-26 18:04:03.000000 pytonapi-0.0.3/pytonapi/schema/traces.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi/tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1357 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1618 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.896121 pytonapi-0.0.3/pytonapi/tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3316 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2166 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      850 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      473 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2578 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      559 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2220 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/utils.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi.egg-info/
--rw-rw-r--   0 ness      (1000) ness      (1000)     6262 2023-05-31 20:44:56.000000 pytonapi-0.0.3/pytonapi.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     1103 2023-05-31 20:44:56.000000 pytonapi-0.0.3/pytonapi.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2023-05-31 20:44:56.000000 pytonapi-0.0.3/pytonapi.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       64 2023-05-31 20:44:56.000000 pytonapi-0.0.3/pytonapi.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        9 2023-05-31 20:44:56.000000 pytonapi-0.0.3/pytonapi.egg-info/top_level.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-05-31 20:44:56.896121 pytonapi-0.0.3/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)      768 2023-05-31 20:44:51.000000 pytonapi-0.0.3/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-06-07 00:19:07.589607 pytonapi-0.0.4/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2023-05-26 17:22:12.000000 pytonapi-0.0.4/LICENSE
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6860 2023-06-07 00:19:07.589607 pytonapi-0.0.4/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6306 2023-06-07 00:06:40.000000 pytonapi-0.0.4/README.md
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-06-07 00:19:07.581607 pytonapi-0.0.4/pytonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      128 2023-06-04 16:22:48.000000 pytonapi-0.0.4/pytonapi/__init__.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-06-07 00:19:07.585607 pytonapi-0.0.4/pytonapi/async_tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1687 2023-06-05 04:16:14.000000 pytonapi-0.0.4/pytonapi/async_tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3475 2023-06-06 22:57:44.000000 pytonapi-0.0.4/pytonapi/async_tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-06-07 00:19:07.585607 pytonapi-0.0.4/pytonapi/async_tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-05-26 17:22:12.000000 pytonapi-0.0.4/pytonapi/async_tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3902 2023-06-06 22:57:44.000000 pytonapi-0.0.4/pytonapi/async_tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2269 2023-06-06 22:46:11.000000 pytonapi-0.0.4/pytonapi/async_tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      881 2023-06-06 22:46:11.000000 pytonapi-0.0.4/pytonapi/async_tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      496 2023-06-06 22:46:11.000000 pytonapi-0.0.4/pytonapi/async_tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2685 2023-06-06 22:46:11.000000 pytonapi-0.0.4/pytonapi/async_tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      872 2023-06-06 22:48:38.000000 pytonapi-0.0.4/pytonapi/async_tonapi/methods/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      543 2023-06-06 22:48:42.000000 pytonapi-0.0.4/pytonapi/async_tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1030 2023-05-26 17:22:12.000000 pytonapi-0.0.4/pytonapi/exceptions.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-06-07 00:19:07.585607 pytonapi-0.0.4/pytonapi/schema/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      409 2023-06-04 22:26:17.000000 pytonapi-0.0.4/pytonapi/schema/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      943 2023-06-04 22:23:56.000000 pytonapi-0.0.4/pytonapi/schema/_address.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      835 2023-06-04 22:23:56.000000 pytonapi-0.0.4/pytonapi/schema/_balance.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      618 2023-06-05 02:43:24.000000 pytonapi-0.0.4/pytonapi/schema/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1797 2023-06-05 02:43:24.000000 pytonapi-0.0.4/pytonapi/schema/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      402 2023-06-05 02:41:34.000000 pytonapi-0.0.4/pytonapi/schema/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      343 2023-06-04 15:56:37.000000 pytonapi-0.0.4/pytonapi/schema/domains.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1046 2023-06-04 22:25:05.000000 pytonapi-0.0.4/pytonapi/schema/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1077 2023-06-04 22:25:05.000000 pytonapi-0.0.4/pytonapi/schema/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      109 2023-06-05 04:09:30.000000 pytonapi-0.0.4/pytonapi/schema/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3036 2023-06-05 02:39:15.000000 pytonapi-0.0.4/pytonapi/schema/traces.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-06-07 00:19:07.585607 pytonapi-0.0.4/pytonapi/tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1624 2023-06-05 04:16:14.000000 pytonapi-0.0.4/pytonapi/tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3415 2023-06-06 22:57:44.000000 pytonapi-0.0.4/pytonapi/tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-06-07 00:19:07.589607 pytonapi-0.0.4/pytonapi/tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-05-26 17:22:12.000000 pytonapi-0.0.4/pytonapi/tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3773 2023-06-06 22:57:44.000000 pytonapi-0.0.4/pytonapi/tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2150 2023-06-06 22:46:40.000000 pytonapi-0.0.4/pytonapi/tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      842 2023-06-06 22:46:40.000000 pytonapi-0.0.4/pytonapi/tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      469 2023-06-06 22:46:40.000000 pytonapi-0.0.4/pytonapi/tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2562 2023-06-06 22:46:40.000000 pytonapi-0.0.4/pytonapi/tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      837 2023-06-06 22:48:38.000000 pytonapi-0.0.4/pytonapi/tonapi/methods/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      730 2023-06-06 22:46:40.000000 pytonapi-0.0.4/pytonapi/tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2368 2023-06-06 23:06:01.000000 pytonapi-0.0.4/pytonapi/utils.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-06-07 00:19:07.585607 pytonapi-0.0.4/pytonapi.egg-info/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6860 2023-06-07 00:19:07.000000 pytonapi-0.0.4/pytonapi.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1256 2023-06-07 00:19:07.000000 pytonapi-0.0.4/pytonapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2023-06-07 00:19:07.000000 pytonapi-0.0.4/pytonapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       64 2023-06-07 00:19:07.000000 pytonapi-0.0.4/pytonapi.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        9 2023-06-07 00:19:07.000000 pytonapi-0.0.4/pytonapi.egg-info/top_level.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-06-07 00:19:07.589607 pytonapi-0.0.4/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)      917 2023-06-06 23:59:38.000000 pytonapi-0.0.4/setup.py
```

### Comparing `pytonapi-0.0.3/LICENSE` & `pytonapi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.3/PKG-INFO` & `pytonapi-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-Metadata-Version: 2.1
-Name: pytonapi
-Version: 0.0.3
-Summary: Provide access to indexed TON blockchain.
-Home-page: https://github.com/nessshon/pytonapi/
-Author: nessshon
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# PyTONAPI
+[![PyPI](https://img.shields.io/pypi/v/pytonapi.svg)](https://pypi.python.org/pypi/pytonapi)
+![Python Versions](https://img.shields.io/pypi/pyversions/pytonapi.svg)
+![License](https://img.shields.io/github/license/nessshon/pytonapi)
 
-## PyTONAPI
-
-Python wrapper for [tonapi.io](https://tonapi.io/swagger-ui/v2) v2.
+Python wrapper for [tonapi.io](https://tonapi.io/swagger-ui/v2) v2
 \
-You need an api key to use it, get it here [tonconsole.com](https://tonconsole.com/).
+__You need an api key to use it, get it here [tonconsole.com](https://tonconsole.com/)__
+
+### Dependencies
+
+* [aiohttp](https://pypi.org/project/aiohttp/)
+* [requests](https://pypi.org/project/requests/)
+* [pydantic](https://pypi.org/project/pydantic/)
+* [libscrc](https://pypi.org/project/libscrc/)
+
 
 ### Installation
 
 ```bash
 pip install pytonapi
 ```
```

### Comparing `pytonapi-0.0.3/README.md` & `pytonapi-0.0.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,39 @@
-## PyTONAPI
+Metadata-Version: 2.1
+Name: pytonapi
+Version: 0.0.4
+Summary: Provide access to indexed TON blockchain.
+Home-page: https://github.com/nessshon/pytonapi/
+Author: nessshon
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-Python wrapper for [tonapi.io](https://tonapi.io/swagger-ui/v2) v2.
+# PyTONAPI
+[![PyPI](https://img.shields.io/pypi/v/pytonapi.svg)](https://pypi.python.org/pypi/pytonapi)
+![Python Versions](https://img.shields.io/pypi/pyversions/pytonapi.svg)
+![License](https://img.shields.io/github/license/nessshon/pytonapi)
+
+Python wrapper for [tonapi.io](https://tonapi.io/swagger-ui/v2) v2
 \
-You need an api key to use it, get it here [tonconsole.com](https://tonconsole.com/).
+__You need an api key to use it, get it here [tonconsole.com](https://tonconsole.com/)__
+
+### Dependencies
+
+* [aiohttp](https://pypi.org/project/aiohttp/)
+* [requests](https://pypi.org/project/requests/)
+* [pydantic](https://pypi.org/project/pydantic/)
+* [libscrc](https://pypi.org/project/libscrc/)
+
 
 ### Installation
 
 ```bash
 pip install pytonapi
 ```
```

### Comparing `pytonapi-0.0.3/pytonapi/async_tonapi/__init__.py` & `pytonapi-0.0.4/pytonapi/async_tonapi/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from .client import AsyncTonapiClient
-
-from .methods.accounts import AccountMethod
-from .methods.blockchain import BlockchainMethod
-from .methods.dns import DnsMethod
-from .methods.jettons import JettonMethod
-from .methods.nft import NftMethod
-from .methods.traces import TraceMethod
+from pytonapi.async_tonapi.client import AsyncTonapiClient
+from pytonapi.async_tonapi.methods.accounts import AccountMethod
+from pytonapi.async_tonapi.methods.blockchain import BlockchainMethod
+from pytonapi.async_tonapi.methods.dns import DnsMethod
+from pytonapi.async_tonapi.methods.jettons import JettonMethod
+from pytonapi.async_tonapi.methods.nft import NftMethod
+from pytonapi.async_tonapi.methods.rates import RateMethod
+from pytonapi.async_tonapi.methods.traces import TraceMethod
 
 
 class AsyncTonapi(AsyncTonapiClient):
+
     def __init__(self, api_key: str, testnet: bool = False):
         """
         :param api_key: You can get an access token here https://tonconsole.com/
         :param testnet: Use true, if you want to switch to testnet
         """
-        super(AsyncTonapi, self).__init__(api_key, testnet)
+        super().__init__(api_key, testnet)
 
     @property
     def blockchain(self) -> BlockchainMethod:
         return BlockchainMethod(api_key=self._api_key, testnet=self._testnet)
 
     @property
     def accounts(self) -> AccountMethod:
@@ -33,9 +34,13 @@
         return DnsMethod(api_key=self._api_key, testnet=self._testnet)
 
     @property
     def nft(self) -> NftMethod:
         return NftMethod(api_key=self._api_key, testnet=self._testnet)
 
     @property
+    def rates(self) -> RateMethod:
+        return RateMethod(api_key=self._api_key, testnet=self._testnet)
+
+    @property
     def traces(self) -> TraceMethod:
         return TraceMethod(api_key=self._api_key, testnet=self._testnet)
```

### Comparing `pytonapi-0.0.3/pytonapi/async_tonapi/methods/accounts.py` & `pytonapi-0.0.4/pytonapi/tonapi/methods/accounts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,71 @@
-from pytonapi.async_tonapi.client import AsyncTonapiClient
+from typing import List
 
-from pytonapi.schema.accounts import Account
+from pytonapi.tonapi.client import TonapiClient
+
+from pytonapi.schema.accounts import Account, Accounts
 from pytonapi.schema.domains import DomainNames
 from pytonapi.schema.jettons import JettonsBalances
 from pytonapi.schema.nft import NftItems
 from pytonapi.schema.traces import TraceIds
 
 
-class AccountMethod(AsyncTonapiClient):
+class AccountMethod(TonapiClient):
 
-    async def get_info(self, account_id: str) -> Account:
+    def get_info(self, account_id: str) -> Account:
         """
         Get human-friendly information about an account without low-level details.
 
         :param account_id: Account ID
         :return: :class:`Account`
         """
         method = f"v2/accounts/{account_id}"
-        response = await self._request(method=method)
+        response = self._get(method=method)
 
         return Account(**response)
 
-    async def get_domains(self, account_id: str) -> DomainNames:
+    def get_bulk_info(self, account_ids: List[str]) -> Accounts:
+        """
+        Get human-friendly information about multiple accounts without low-level details.
+
+        :param account_ids: List of account IDs
+        return: :class:`Accounts`
+        """
+        method = f"v2/accounts/_bulk"
+        params = {"account_ids": account_ids}
+        response = self._post(method=method, body=params)
+
+        return Accounts(**response)
+
+    def get_domains(self, account_id: str) -> DomainNames:
         """
         Get domains for wallet account.
 
         :param account_id: account ID
         :return: :class:`DomainNames`
         """
         method = f"v2/accounts/{account_id}/dns/backresolve"
-        response = await self._request(method=method)
+        response = self._get(method=method)
 
         return DomainNames(**response)
 
-    async def get_jettons_balances(self, account_id: str) -> JettonsBalances:
+    def get_jettons_balances(self, account_id: str) -> JettonsBalances:
         """
         Get all Jettons balances by owner address.
 
         :param account_id: account ID
         :return: :class:`JettonsBalances`
         """
         method = f"v2/accounts/{account_id}/jettons"
-        response = await self._request(method=method)
+        response = self._get(method=method)
 
         return JettonsBalances(**response)
 
-    async def get_nfts(self, account_id: str, limit: int = 1000, offset: int = 0,
-                       indirect_ownership: bool = False) -> NftItems:
+    def get_nfts(self, account_id: str, limit: int = 1000, offset: int = 0,
+                 indirect_ownership: bool = False) -> NftItems:
         """
         Get NFT items by owner address.
 
         :param account_id: account ID
         :param limit: Default value : 1000
         :param offset: Default value : 0
         :param indirect_ownership: Selling nft items in ton implemented usually via transfer items
@@ -58,47 +73,47 @@
         :return: :class:`NftItems`
         """
         method = f"v2/accounts/{account_id}/nfts"
         params = {
             "limit": limit, "offset": offset,
             'indirect_ownership': 'true' if indirect_ownership else 'false'
         }
-        response = await self._request(method=method, params=params)
+        response = self._get(method=method, params=params)
 
         return NftItems(**response)
 
-    async def get_all_nfts(self, account_id: str) -> NftItems:
+    def get_all_nfts(self, account_id: str) -> NftItems:
         """
         Get all NFT items by owner address.
 
         :param account_id: account ID
         :return: :class:`NftItems`
         """
         nft_items = []
         offset, limit = 0, 1000
 
         while True:
-            result = await self.get_nfts(
+            result = self.get_nfts(
                 account_id=account_id, limit=limit, offset=offset,
                 indirect_ownership=True,
             )
             nft_items += result.nft_items
             offset += limit
 
             if len(result.nft_items) != limit:
                 break
 
         return NftItems(nft_items=nft_items)
 
-    async def get_traces(self, account_id: str, limit: int = 100) -> TraceIds:
+    def get_traces(self, account_id: str, limit: int = 100) -> TraceIds:
         """
         Get traces for account.
 
         :param account_id: account ID
         :param limit: Default value : 100
         :return: :class:`TraceIds`
         """
         method = f"v2/accounts/{account_id}/traces"
         params = {"limit": limit}
-        response = await self._request(method=method, params=params)
+        response = self._get(method=method, params=params)
 
         return TraceIds(**response)
```

### Comparing `pytonapi-0.0.3/pytonapi/async_tonapi/methods/blockchain.py` & `pytonapi-0.0.4/pytonapi/tonapi/methods/blockchain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from pytonapi.async_tonapi.client import AsyncTonapiClient
+from pytonapi.tonapi.client import TonapiClient
 
 from pytonapi.schema.blockchain import Block, Transactions, Transaction
 
 
-class BlockchainMethod(AsyncTonapiClient):
+class BlockchainMethod(TonapiClient):
 
-    async def get_block_data(self, block_id: str) -> Block:
+    def get_block_data(self, block_id: str) -> Block:
         """
         Get block data.
 
         :param block_id: block ID (string), example: "(-1,8000000000000000,4234234)"
         :return: :class:`Block`
         """
         method = f"v2/blockchain/blocks/{block_id}"
-        response = await self._request(method=method)
+        response = self._get(method=method)
 
         return Block(**response)
 
-    async def get_transaction_from_block(self, block_id: str) -> Transactions:
+    def get_transaction_from_block(self, block_id: str) -> Transactions:
         """
         Get transactions from block.
 
         :param block_id: block ID (string), example: "(-1,8000000000000000,4234234)"
         :return: :class:`Block`
         """
         method = f"v2/blockchain/blocks/{block_id}/transactions"
-        response = await self._request(method=method)
+        response = self._get(method=method)
 
         return Transactions(**response)
 
-    async def get_transaction_data(self, transaction_id: str) -> Transaction:
+    def get_transaction_data(self, transaction_id: str) -> Transaction:
         """
         Get transaction data.
 
         :param transaction_id: Transaction_id ID (string),
          example: "97264395BD65A255A429B11326C84128B7D70FFED7949ABAE3036D506BA38621"
         :return: :class:`Transaction`
         """
         method = f"v2/blockchain/transactions/{transaction_id}"
-        response = await self._request(method=method)
+        response = self._get(method=method)
 
         return Transaction(**response)
 
-    async def get_account_transactions(self, account_id: str, after_lt: int = None,
-                                       before_lt: int = 0, limit: int = 100) -> Transactions:
+    def get_account_transactions(self, account_id: str, after_lt: int = None,
+                                 before_lt: int = 0, limit: int = 100) -> Transactions:
         """
         Get account transactions.
 
         :param account_id: account ID
         :param after_lt: omit this parameter to get last transactions
         :param before_lt: omit this parameter to get last transactions
         :param limit: Default value : 100
         :return: :class:`Transactions`
         """
         method = f"v2/blockchain/accounts/{account_id}/transactions"
         params = {'before_lt': before_lt, 'limit': limit}
         if after_lt: params['after_lt'] = after_lt  # noqa E701
-        response = await self._request(method=method, params=params)
+        response = self._get(method=method, params=params)
 
         return Transactions(**response)
```

### Comparing `pytonapi-0.0.3/pytonapi/async_tonapi/methods/dns.py` & `pytonapi-0.0.4/pytonapi/async_tonapi/methods/dns.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from pytonapi.async_tonapi.client import AsyncTonapiClient
-
 from pytonapi.schema.dns import DNSRecord
 from pytonapi.schema.domains import DomainBids
 
 
 class DnsMethod(AsyncTonapiClient):
 
     async def resolve(self, domain_name: str) -> DNSRecord:
         """
         DNS resolve for domain name.
 
         :param domain_name: domain name with .ton or .t.me
         :return: :class:`DNSRecord`
         """
         method = f"v2/dns/{domain_name}/resolve"
-        response = await self._request(method=method)
+        response = await self._get(method=method)
 
         return DNSRecord(**response)
 
     async def bids(self, domain_name: str) -> DomainBids:
         """
         Get domain bids.
 
         :param domain_name: domain name with .ton or .t.me
         :return: :class:`DomainBids`
         """
         method = f"v2/dns/{domain_name}/bids"
-        response = await self._request(method=method)
+        response = await self._get(method=method)
 
         return DomainBids(**response)
```

### Comparing `pytonapi-0.0.3/pytonapi/async_tonapi/methods/nft.py` & `pytonapi-0.0.4/pytonapi/async_tonapi/methods/nft.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from pytonapi.async_tonapi.client import AsyncTonapiClient
+from typing import List
 
+from pytonapi.async_tonapi.client import AsyncTonapiClient
 from pytonapi.schema.nft import NftCollections, NftCollection, NftItems, NftItem
 
 
 class NftMethod(AsyncTonapiClient):
 
     async def get_collections(self, limit: int = 15, offset: int = 0) -> NftCollections:
         """
@@ -11,27 +12,27 @@
 
         :param limit: Default value : 15
         :param offset: Default value : 0
         :return: :class:`NftCollections`
         """
         method = "v2/nfts/collections"
         params = {'limit': limit, 'offset': offset}
-        response = await self._request(method=method, params=params)
+        response = await self._get(method=method, params=params)
 
         return NftCollections(**response)
 
     async def get_collection_by_collection_address(self, account_id: str) -> NftCollection:
         """
         Get NFT collection by collection address.
 
         :param account_id: Account ID
         :return: :class:`NftCollection`
         """
         method = f"v2/nfts/collections/{account_id}"
-        response = await self._request(method=method)
+        response = await self._get(method=method)
 
         return NftCollection(**response)
 
     async def get_items_by_collection_address(self, account_id: str, limit: int = 1000,
                                               offset: int = 0) -> NftItems:
         """
         Get NFT items from collection by collection address.
@@ -39,26 +40,26 @@
         :param account_id: Account ID
         :param limit: Default value : 1000
         :param offset: Default value : 0
         :return: :class:`NftItems`
         """
         method = f"v2/nfts/collections/{account_id}/items"
         params = {'limit': limit, 'offset': offset}
-        response = await self._request(method=method, params=params)
+        response = await self._get(method=method, params=params)
 
         return NftItems(**response)
 
     async def get_all_items_by_collection_address(self, account_id: str) -> NftItems:
         """
         Get all NFT items from collection by collection address.
 
         :param account_id: Account ID
-        :return: :class:NftItems
+        :return: :class:`NftItems`
         """
-        nft_items = []
+        nft_items: List[NftItem] = []
         offset, limit = 0, 1000
 
         while True:
             result = await self.get_items_by_collection_address(
                 account_id=account_id, limit=limit, offset=offset,
             )
             nft_items += result.nft_items
@@ -73,10 +74,10 @@
         """
         Get NFT item by its address.
 
         :param account_id: account ID
         :return: :class:`NftItem`
         """
         method = f"v2/nfts/{account_id}"
-        response = await self._request(method=method)
+        response = await self._get(method=method)
 
         return NftItem(**response)
```

### Comparing `pytonapi-0.0.3/pytonapi/async_tonapi/methods/traces.py` & `pytonapi-0.0.4/pytonapi/tonapi/methods/traces.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import base64
+import binascii
 
-from pytonapi.async_tonapi.client import AsyncTonapiClient
+from pytonapi.tonapi.client import TonapiClient
 
 from pytonapi.schema.traces import Trace
 
 
-class TraceMethod(AsyncTonapiClient):
+class TraceMethod(TonapiClient):
 
-    async def get_trace(self, trace_id: str) -> Trace:
+    def get_trace(self, trace_id: str) -> Trace:
         """
         Get the trace by trace ID or hash of any transaction in trace.
 
         :param trace_id: trace ID or transaction hash in hex (without 0x) or base64url format
         :return: :class:`Trace`
         """
-        method = f"v2/traces/{base64.b64decode(trace_id).hex()}"
-        response = await self._request(method=method)
+        if len(trace_id) == 44:
+            decoded = base64.urlsafe_b64decode(trace_id + '=' * (-len(trace_id) % 4))
+            trace_id = binascii.hexlify(decoded).decode('utf-8')
+        method = f"v2/traces/{trace_id}"
+        response = self._get(method=method)
 
         return Trace(**response)
```

### Comparing `pytonapi-0.0.3/pytonapi/exceptions.py` & `pytonapi-0.0.4/pytonapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.3/pytonapi/schema/blockchain.py` & `pytonapi-0.0.4/pytonapi/schema/blockchain.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from typing import List, Optional
+
 from pydantic import BaseModel
 
 from pytonapi.schema.accounts import AccountAddress
-
-from pytonapi.schema.traces import (Message, AccountStatus, TransactionType,
-                                    ComputePhase, StoragePhase, CreditPhase, ActionPhase, BouncePhaseType)
+from pytonapi.schema.traces import (AccountStatus, TransactionType,
+                                    BouncePhaseType, ActionPhase,
+                                    CreditPhase, StoragePhase,
+                                    ComputePhase, Message)
 
 
 class Block(BaseModel):
     workchain_id: int
     shard: str
     seqno: int
     root_hash: str
@@ -23,18 +26,18 @@
     gen_utime: int
     start_lt: int
     end_lt: int
     vert_seqno: int
     gen_catchain_seqno: int
     min_ref_mc_seqno: int
     prev_key_block_seqno: int
-    gen_software_version: None | int
-    gen_software_capabilities: None | int
-    master_ref: None | str
-    prev_refs: list[str]
+    gen_software_version: Optional[int]
+    gen_software_capabilities: Optional[int]
+    master_ref: Optional[str]
+    prev_refs: List[str]
     in_msg_descr_length: int
     out_msg_descr_length: int
     rand_seed: str
     created_by: str
 
 
 class Transaction(BaseModel):
@@ -45,25 +48,23 @@
     utime: int
     orig_status: AccountStatus
     end_status: AccountStatus
     total_fees: int
     transaction_type: TransactionType
     state_update_old: str
     state_update_new: str
-    in_msg: None | Message
-    out_msgs: list[Message]
+    in_msg: Optional[Message]
+    out_msgs: List[Message]
     block: str
-    prev_trans_hash: None | str
-    prev_trans_lt: None | int
-    compute_phase: None | ComputePhase
-    storage_phase: None | StoragePhase
-    credit_phase: None | CreditPhase
-    action_phase: None | ActionPhase
-    bounce_phase: None | BouncePhaseType
+    prev_trans_hash: Optional[str]
+    prev_trans_lt: Optional[int]
+    compute_phase: Optional[ComputePhase]
+    storage_phase: Optional[StoragePhase]
+    credit_phase: Optional[CreditPhase]
+    action_phase: Optional[ActionPhase]
+    bounce_phase: Optional[BouncePhaseType]
     aborted: bool
     destroyed: bool
 
 
 class Transactions(BaseModel):
-    transactions: list[Transaction]
-
-
+    transactions: List[Transaction]
```

### Comparing `pytonapi-0.0.3/pytonapi/schema/jettons.py` & `pytonapi-0.0.4/pytonapi/schema/jettons.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from enum import Enum
+from typing import List, Optional
 
 from pydantic import BaseModel
 
-from . import Address
-from .accounts import AccountAddress
+from pytonapi.schema._address import Address
+from pytonapi.schema.accounts import AccountAddress
 
 
-class JettonVerificationType(Enum):
-    whitelist: str = "whitelist"
-    blacklist: str = "blacklist"
-    none: str = "none"
+class JettonVerificationType(str, Enum):
+    whitelist = "whitelist"
+    blacklist = "blacklist"
+    none = "none"
 
 
 class JettonMetadata(BaseModel):
     address: Address
     name: str
     symbol: str
     decimals: str
-    image: None | str
-    description: None | str
-    social: None | list[str]
-    websites: None | list[str]
-    catalogs: None | list[str]
+    image: Optional[str]
+    description: Optional[str]
+    social: Optional[List[str]]
+    websites: Optional[List[str]]
+    catalogs: Optional[List[str]]
 
 
 class JettonInfo(BaseModel):
     mintable: bool
     total_supply: str
     metadata: JettonMetadata
     verification: JettonVerificationType
@@ -43,8 +44,8 @@
 class JettonBalance(BaseModel):
     balance: str
     wallet_address: AccountAddress
     jetton: JettonPreview
 
 
 class JettonsBalances(BaseModel):
-    balances: list[JettonBalance]
+    balances: List[JettonBalance]
```

### Comparing `pytonapi-0.0.3/pytonapi/schema/nft.py` & `pytonapi-0.0.4/pytonapi/schema/nft.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from typing import List, Optional
+
 from pydantic import BaseModel
 
-from . import Address
-from .accounts import AccountAddress
+from pytonapi.schema._address import Address
+from pytonapi.schema.accounts import AccountAddress
 
 
 class Price(BaseModel):
     value: str
     token_name: str
 
 
 class Sale(BaseModel):
     address: Address
     market: AccountAddress
-    owner: None | AccountAddress
+    owner: Optional[AccountAddress]
     price: Price
 
 
 class ImagePreview(BaseModel):
     resolution: str
     url: str
 
@@ -27,29 +29,29 @@
 
 
 class NftCollection(BaseModel):
     address: Address
     next_item_index: int
     owner: AccountAddress
     raw_collection_content: str
-    metadata: None | dict
+    metadata: Optional[dict]
 
 
 class NftItem(BaseModel):
     address: Address
     index: int
-    owner: None | AccountAddress
-    collection: None | Collection
+    owner: Optional[AccountAddress]
+    collection: Optional[Collection]
     verified: bool
     metadata: dict
-    sale: None | Sale
-    previews: None | list[ImagePreview]
-    dns: None | str
-    approved_by: list[str]
+    sale: Optional[Sale]
+    previews: Optional[List[ImagePreview]]
+    dns: Optional[str]
+    approved_by: List[str]
 
 
 class NftItems(BaseModel):
-    nft_items: list[NftItem]
+    nft_items: List[NftItem]
 
 
 class NftCollections(BaseModel):
-    nft_collections: list[NftCollection]
+    nft_collections: List[NftCollection]
```

### Comparing `pytonapi-0.0.3/pytonapi/tonapi/methods/accounts.py` & `pytonapi-0.0.4/pytonapi/async_tonapi/methods/accounts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,70 @@
-from pytonapi.tonapi.client import TonapiClient
+from typing import List
 
-from pytonapi.schema.accounts import Account
+from pytonapi.async_tonapi.client import AsyncTonapiClient
+from pytonapi.schema.accounts import Account, Accounts
 from pytonapi.schema.domains import DomainNames
 from pytonapi.schema.jettons import JettonsBalances
-from pytonapi.schema.nft import NftItems
+from pytonapi.schema.nft import NftItems, NftItem
 from pytonapi.schema.traces import TraceIds
 
 
-class AccountMethod(TonapiClient):
+class AccountMethod(AsyncTonapiClient):
 
-    def get_info(self, account_id: str) -> Account:
+    async def get_info(self, account_id: str) -> Account:
         """
         Get human-friendly information about an account without low-level details.
 
         :param account_id: Account ID
         :return: :class:`Account`
         """
         method = f"v2/accounts/{account_id}"
-        response = self._request(method=method)
+        response = await self._get(method=method)
 
         return Account(**response)
 
-    def get_domains(self, account_id: str) -> DomainNames:
+    async def get_bulk_info(self, account_ids: List[str]) -> Accounts:
+        """
+        Get human-friendly information about multiple accounts without low-level details.
+
+        :param account_ids: List of account IDs
+        return: :class:`Accounts`
+        """
+        method = f"v2/accounts/_bulk"
+        params = {"account_ids": account_ids}
+        response = await self._post(method=method, body=params)
+
+        return Accounts(**response)
+
+    async def get_domains(self, account_id: str) -> DomainNames:
         """
         Get domains for wallet account.
 
         :param account_id: account ID
         :return: :class:`DomainNames`
         """
         method = f"v2/accounts/{account_id}/dns/backresolve"
-        response = self._request(method=method)
+        response = await self._get(method=method)
 
         return DomainNames(**response)
 
-    def get_jettons_balances(self, account_id: str) -> JettonsBalances:
+    async def get_jettons_balances(self, account_id: str) -> JettonsBalances:
         """
         Get all Jettons balances by owner address.
 
         :param account_id: account ID
         :return: :class:`JettonsBalances`
         """
         method = f"v2/accounts/{account_id}/jettons"
-        response = self._request(method=method)
+        response = await self._get(method=method)
 
         return JettonsBalances(**response)
 
-    def get_nfts(self, account_id: str, limit: int = 1000, offset: int = 0,
-                 indirect_ownership: bool = False) -> NftItems:
+    async def get_nfts(self, account_id: str, limit: int = 1000, offset: int = 0,
+                       indirect_ownership: bool = False) -> NftItems:
         """
         Get NFT items by owner address.
 
         :param account_id: account ID
         :param limit: Default value : 1000
         :param offset: Default value : 0
         :param indirect_ownership: Selling nft items in ton implemented usually via transfer items
@@ -58,47 +72,47 @@
         :return: :class:`NftItems`
         """
         method = f"v2/accounts/{account_id}/nfts"
         params = {
             "limit": limit, "offset": offset,
             'indirect_ownership': 'true' if indirect_ownership else 'false'
         }
-        response = self._request(method=method, params=params)
+        response = await self._get(method=method, params=params)
 
         return NftItems(**response)
 
-    def get_all_nfts(self, account_id: str) -> NftItems:
+    async def get_all_nfts(self, account_id: str) -> NftItems:
         """
         Get all NFT items by owner address.
 
         :param account_id: account ID
         :return: :class:`NftItems`
         """
-        nft_items = []
+        nft_items: List[NftItem] = []
         offset, limit = 0, 1000
 
         while True:
-            result = self.get_nfts(
+            result = await self.get_nfts(
                 account_id=account_id, limit=limit, offset=offset,
                 indirect_ownership=True,
             )
             nft_items += result.nft_items
             offset += limit
 
             if len(result.nft_items) != limit:
                 break
 
         return NftItems(nft_items=nft_items)
 
-    def get_traces(self, account_id: str, limit: int = 100) -> TraceIds:
+    async def get_traces(self, account_id: str, limit: int = 100) -> TraceIds:
         """
         Get traces for account.
 
         :param account_id: account ID
         :param limit: Default value : 100
         :return: :class:`TraceIds`
         """
         method = f"v2/accounts/{account_id}/traces"
         params = {"limit": limit}
-        response = self._request(method=method, params=params)
+        response = await self._get(method=method, params=params)
 
         return TraceIds(**response)
```

### Comparing `pytonapi-0.0.3/pytonapi/tonapi/methods/blockchain.py` & `pytonapi-0.0.4/pytonapi/async_tonapi/methods/blockchain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-from pytonapi.tonapi.client import TonapiClient
+from typing import Optional
 
+from pytonapi.async_tonapi.client import AsyncTonapiClient
 from pytonapi.schema.blockchain import Block, Transactions, Transaction
 
 
-class BlockchainMethod(TonapiClient):
+class BlockchainMethod(AsyncTonapiClient):
 
-    def get_block_data(self, block_id: str) -> Block:
+    async def get_block_data(self, block_id: str) -> Block:
         """
         Get block data.
 
         :param block_id: block ID (string), example: "(-1,8000000000000000,4234234)"
         :return: :class:`Block`
         """
         method = f"v2/blockchain/blocks/{block_id}"
-        response = self._request(method=method)
+        response = await self._get(method=method)
 
         return Block(**response)
 
-    def get_transaction_from_block(self, block_id: str) -> Transactions:
+    async def get_transaction_from_block(self, block_id: str) -> Transactions:
         """
         Get transactions from block.
 
         :param block_id: block ID (string), example: "(-1,8000000000000000,4234234)"
         :return: :class:`Block`
         """
         method = f"v2/blockchain/blocks/{block_id}/transactions"
-        response = self._request(method=method)
+        response = await self._get(method=method)
 
         return Transactions(**response)
 
-    def get_transaction_data(self, transaction_id: str) -> Transaction:
+    async def get_transaction_data(self, transaction_id: str) -> Transaction:
         """
         Get transaction data.
 
         :param transaction_id: Transaction_id ID (string),
          example: "97264395BD65A255A429B11326C84128B7D70FFED7949ABAE3036D506BA38621"
         :return: :class:`Transaction`
         """
         method = f"v2/blockchain/transactions/{transaction_id}"
-        response = self._request(method=method)
+        response = await self._get(method=method)
 
         return Transaction(**response)
 
-    def get_account_transactions(self, account_id: str, after_lt: int = None,
-                                 before_lt: int = 0, limit: int = 100) -> Transactions:
+    async def get_account_transactions(self, account_id: str, after_lt: Optional[int] = None,
+                                       before_lt: int = 0, limit: int = 100) -> Transactions:
         """
         Get account transactions.
 
         :param account_id: account ID
         :param after_lt: omit this parameter to get last transactions
         :param before_lt: omit this parameter to get last transactions
         :param limit: Default value : 100
         :return: :class:`Transactions`
         """
         method = f"v2/blockchain/accounts/{account_id}/transactions"
         params = {'before_lt': before_lt, 'limit': limit}
-        if after_lt: params['after_lt'] = after_lt  # noqa E701
-        response = self._request(method=method, params=params)
+        if after_lt is not None:
+            params['after_lt'] = after_lt
+        response = await self._get(method=method, params=params)
 
         return Transactions(**response)
```

### Comparing `pytonapi-0.0.3/pytonapi/tonapi/methods/dns.py` & `pytonapi-0.0.4/pytonapi/tonapi/methods/dns.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,22 @@
         """
         DNS resolve for domain name.
 
         :param domain_name: domain name with .ton or .t.me
         :return: :class:`DNSRecord`
         """
         method = f"v2/dns/{domain_name}/resolve"
-        response = self._request(method=method)
+        response = self._get(method=method)
 
         return DNSRecord(**response)
 
     def bids(self, domain_name: str) -> DomainBids:
         """
         Get domain bids.
 
         :param domain_name: domain name with .ton or .t.me
         :return: :class:`DomainBids`
         """
         method = f"v2/dns/{domain_name}/bids"
-        response = self._request(method=method)
+        response = self._get(method=method)
 
         return DomainBids(**response)
```

### Comparing `pytonapi-0.0.3/pytonapi/tonapi/methods/nft.py` & `pytonapi-0.0.4/pytonapi/tonapi/methods/nft.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 
         :param limit: Default value : 15
         :param offset: Default value : 0
         :return: :class:`NftCollections`
         """
         method = "v2/nfts/collections"
         params = {'limit': limit, 'offset': offset}
-        response = self._request(method=method, params=params)
+        response = self._get(method=method, params=params)
 
         return NftCollections(**response)
 
     def get_collection_by_collection_address(self, account_id: str) -> NftCollection:
         """
         Get NFT collection by collection address.
 
         :param account_id: Account ID
         :return: :class:`NftCollection`
         """
         method = f"v2/nfts/collections/{account_id}"
-        response = self._request(method=method)
+        response = self._get(method=method)
 
         return NftCollection(**response)
 
     def get_items_by_collection_address(self, account_id: str, limit: int = 1000,
                                         offset: int = 0) -> NftItems:
         """
         Get NFT items from collection by collection address.
@@ -39,15 +39,15 @@
         :param account_id: Account ID
         :param limit: Default value : 1000
         :param offset: Default value : 0
         :return: :class:`NftItems`
         """
         method = f"v2/nfts/collections/{account_id}/items"
         params = {'limit': limit, 'offset': offset}
-        response = self._request(method=method, params=params)
+        response = self._get(method=method, params=params)
 
         return NftItems(**response)
 
     def get_all_items_by_collection_address(self, account_id: str) -> NftItems:
         """
         Get all NFT items from collection by collection address.
 
@@ -73,10 +73,10 @@
         """
         Get NFT item by its address.
 
         :param account_id: account ID
         :return: :class:`NftItem`
         """
         method = f"v2/nfts/{account_id}"
-        response = self._request(method=method)
+        response = self._get(method=method)
 
         return NftItem(**response)
```

### Comparing `pytonapi-0.0.3/pytonapi/tonapi/methods/traces.py` & `pytonapi-0.0.4/pytonapi/async_tonapi/methods/traces.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import base64
-
-from pytonapi.tonapi.client import TonapiClient
-
+from pytonapi.async_tonapi.client import AsyncTonapiClient
 from pytonapi.schema.traces import Trace
 
 
-class TraceMethod(TonapiClient):
+class TraceMethod(AsyncTonapiClient):
 
-    def get_trace(self, trace_id: str) -> Trace:
+    async def get_trace(self, trace_id: str) -> Trace:
         """
         Get the trace by trace ID or hash of any transaction in trace.
 
         :param trace_id: trace ID or transaction hash in hex (without 0x) or base64url format
         :return: :class:`Trace`
         """
-        method = f"v2/traces/{base64.b64decode(trace_id).hex()}"
-        response = self._request(method=method)
+        method = f"v2/traces/{trace_id}"
+        response = await self._get(method=method)
 
         return Trace(**response)
```

### Comparing `pytonapi-0.0.3/pytonapi/utils.py` & `pytonapi-0.0.4/pytonapi/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import base64
 import struct
+from typing import Union
 
 import libscrc
 
+__all__ = [
+    'raw_to_userfriendly',
+    'userfriendly_to_raw',
+    'nano_to_amount',
+    'amount_to_nano'
+]
 
-def raw_to_userfriendly(address: str, tag=0x11) -> str:
+
+def raw_to_userfriendly(address: str, tag: int = 0x11) -> str:
     """
     Converts a raw address string to a user-friendly format.
 
     :param address: address (str): The raw address string in the format "workchain_id:key".
     :param tag: The tag value to include in the output. Defaults to 0x11.
     :return: The user-friendly address string, encoded in base64 and URL-safe.
     """
@@ -37,28 +45,28 @@
     k = base64.urlsafe_b64decode(address)[1:34]
     workchain_id = struct.unpack('b', k[:1])[0]
     key = k[1:].hex().upper()
 
     return f'{workchain_id}:{key}'
 
 
-def nano_to_amount(value: int | float, precision: int = 2) -> float:
+def nano_to_amount(value: Union[int, float], precision: int = 2) -> float:
     """
     Converts a value from nanoton to TON and rounds it to the specified precision.
 
     :param value: The value to convert, in nanoton. This should be a positive integer or float.
     :param precision: The number of decimal places to round the converted value to. Defaults to 2.
     :return: The converted value, in TON, rounded to the specified precision.
     """
     converted_value = round(value / 10 ** 9, 9)
 
-    return float(f'{converted_value:.{precision}f}')
+    return round(converted_value, precision)
 
 
-def amount_to_nano(value: int | float) -> int:
+def amount_to_nano(value: Union[int, float]) -> int:
     """
     Converts TON value to nanoton.
 
     :param value: TON value to be converted. Can be a float or an integer.
     :return: The value of the input in nanoton.
     """
     return int(value * (10 ** 9))
```

### Comparing `pytonapi-0.0.3/pytonapi.egg-info/PKG-INFO` & `pytonapi-0.0.4/pytonapi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 Metadata-Version: 2.1
 Name: pytonapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Provide access to indexed TON blockchain.
 Home-page: https://github.com/nessshon/pytonapi/
 Author: nessshon
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## PyTONAPI
+# PyTONAPI
+[![PyPI](https://img.shields.io/pypi/v/pytonapi.svg)](https://pypi.python.org/pypi/pytonapi)
+![Python Versions](https://img.shields.io/pypi/pyversions/pytonapi.svg)
+![License](https://img.shields.io/github/license/nessshon/pytonapi)
 
-Python wrapper for [tonapi.io](https://tonapi.io/swagger-ui/v2) v2.
+Python wrapper for [tonapi.io](https://tonapi.io/swagger-ui/v2) v2
 \
-You need an api key to use it, get it here [tonconsole.com](https://tonconsole.com/).
+__You need an api key to use it, get it here [tonconsole.com](https://tonconsole.com/)__
+
+### Dependencies
+
+* [aiohttp](https://pypi.org/project/aiohttp/)
+* [requests](https://pypi.org/project/requests/)
+* [pydantic](https://pypi.org/project/pydantic/)
+* [libscrc](https://pypi.org/project/libscrc/)
+
 
 ### Installation
 
 ```bash
 pip install pytonapi
 ```
```

### Comparing `pytonapi-0.0.3/pytonapi.egg-info/SOURCES.txt` & `pytonapi-0.0.4/pytonapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,30 @@
 pytonapi/async_tonapi/client.py
 pytonapi/async_tonapi/methods/__init__.py
 pytonapi/async_tonapi/methods/accounts.py
 pytonapi/async_tonapi/methods/blockchain.py
 pytonapi/async_tonapi/methods/dns.py
 pytonapi/async_tonapi/methods/jettons.py
 pytonapi/async_tonapi/methods/nft.py
+pytonapi/async_tonapi/methods/rates.py
 pytonapi/async_tonapi/methods/traces.py
 pytonapi/schema/__init__.py
+pytonapi/schema/_address.py
+pytonapi/schema/_balance.py
 pytonapi/schema/accounts.py
 pytonapi/schema/blockchain.py
 pytonapi/schema/dns.py
 pytonapi/schema/domains.py
 pytonapi/schema/jettons.py
 pytonapi/schema/nft.py
+pytonapi/schema/rates.py
 pytonapi/schema/traces.py
 pytonapi/tonapi/__init__.py
 pytonapi/tonapi/client.py
 pytonapi/tonapi/methods/__init__.py
 pytonapi/tonapi/methods/accounts.py
 pytonapi/tonapi/methods/blockchain.py
 pytonapi/tonapi/methods/dns.py
 pytonapi/tonapi/methods/jettons.py
 pytonapi/tonapi/methods/nft.py
+pytonapi/tonapi/methods/rates.py
 pytonapi/tonapi/methods/traces.py
```

### Comparing `pytonapi-0.0.3/setup.py` & `pytonapi-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytonapi",
-    version="0.0.3",
+    version="0.0.4",
     author="nessshon",
     description="Provide access to indexed TON blockchain.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nessshon/pytonapi/",
     packages=setuptools.find_packages(exclude="pytonapi"),
-    python_requires='>=3.10',
+    python_requires='>=3.7',
     install_requires=[
         "aiohttp>=3.8.3",
         "libscrc>=1.8.1",
         "pydantic>=1.10.4",
         "requests>=2.29.0",
     ],
     classifiers=[
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

