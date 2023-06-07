# Comparing `tmp/substrate-interface-polkascan-0.1.tar.gz` & `tmp/substrate-interface-polkascan-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-interface-polkascan-0.1.tar", last modified: Fri Jun  2 13:42:42 2023, max compression
+gzip compressed data, was "substrate-interface-polkascan-0.2.tar", last modified: Wed Jun  7 13:07:44 2023, max compression
```

## Comparing `substrate-interface-polkascan-0.1.tar` & `substrate-interface-polkascan-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:42:42.067634 substrate-interface-polkascan-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 13:42:17.000000 substrate-interface-polkascan-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-02 13:42:42.067634 substrate-interface-polkascan-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-02 13:42:17.000000 substrate-interface-polkascan-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 13:42:42.067634 substrate-interface-polkascan-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-02 13:42:17.000000 substrate-interface-polkascan-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:42:42.063634 substrate-interface-polkascan-0.1/substrate_interface_polkascan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-02 13:42:41.000000 substrate-interface-polkascan-0.1/substrate_interface_polkascan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-02 13:42:42.000000 substrate-interface-polkascan-0.1/substrate_interface_polkascan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:42:41.000000 substrate-interface-polkascan-0.1/substrate_interface_polkascan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-02 13:42:41.000000 substrate-interface-polkascan-0.1/substrate_interface_polkascan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 13:42:41.000000 substrate-interface-polkascan-0.1/substrate_interface_polkascan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:42:42.067634 substrate-interface-polkascan-0.1/substrateinterface_polkascan/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-02 13:42:17.000000 substrate-interface-polkascan-0.1/substrateinterface_polkascan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-02 13:42:17.000000 substrate-interface-polkascan-0.1/substrateinterface_polkascan/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:42:42.067634 substrate-interface-polkascan-0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-02 13:42:17.000000 substrate-interface-polkascan-0.1/test/test_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:07:44.953773 substrate-interface-polkascan-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 13:07:16.000000 substrate-interface-polkascan-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-07 13:07:44.953773 substrate-interface-polkascan-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-07 13:07:16.000000 substrate-interface-polkascan-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:07:44.953773 substrate-interface-polkascan-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-07 13:07:16.000000 substrate-interface-polkascan-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:07:44.949773 substrate-interface-polkascan-0.2/substrate_interface_polkascan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-07 13:07:44.000000 substrate-interface-polkascan-0.2/substrate_interface_polkascan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-07 13:07:44.000000 substrate-interface-polkascan-0.2/substrate_interface_polkascan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:07:44.000000 substrate-interface-polkascan-0.2/substrate_interface_polkascan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 13:07:44.000000 substrate-interface-polkascan-0.2/substrate_interface_polkascan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 13:07:44.000000 substrate-interface-polkascan-0.2/substrate_interface_polkascan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:07:44.953773 substrate-interface-polkascan-0.2/substrateinterface_polkascan/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-07 13:07:16.000000 substrate-interface-polkascan-0.2/substrateinterface_polkascan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-07 13:07:16.000000 substrate-interface-polkascan-0.2/substrateinterface_polkascan/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:07:44.953773 substrate-interface-polkascan-0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-07 13:07:16.000000 substrate-interface-polkascan-0.2/test/test_extension.py
```

### Comparing `substrate-interface-polkascan-0.1/LICENSE` & `substrate-interface-polkascan-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-interface-polkascan-0.1/PKG-INFO` & `substrate-interface-polkascan-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: substrate-interface-polkascan
-Version: 0.1
+Version: 0.2
 Summary: py-substrate-interface extension to utilize Polkascan API indexes
 Home-page: https://github.com/polkascan/py-substrate-interface-extension-polkascan
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
-Description: # Python Substrate Polkascan Extension
+Description: # Python Substrate Interface: Polkascan Extension
         
         [![Latest Version](https://img.shields.io/pypi/v/substrate-interface-polkascan.svg)](https://pypi.org/project/substrate-interface-polkascan/)
         [![Supported Python versions](https://img.shields.io/pypi/pyversions/substrate-interface-polkascan.svg)](https://pypi.org/project/substrate-interface/)
         [![License](https://img.shields.io/pypi/l/substrate-interface-polkascan.svg)](https://github.com/polkascan/py-substrate-interface-extension-polkascan/blob/master/LICENSE)
         
         
         ## Description
-        This extension enables [Substrate Interface](https://github.com/polkascan/py-substrate-interface) to use indexes provided by [Polkascan Explorer API](https://github.com/polkascan/explorer#explorer-api-component)   
+        This extension enables [Substrate Interface](https://github.com/polkascan/py-substrate-interface) to use indexes provided by the [Polkascan Explorer API](https://github.com/polkascan/explorer#explorer-api-component)   
         
         ## Installation
         ```bash
         pip install substrate-interface-polkascan
         ```
         
         ## Initialization
         
         ```python
-        from substrateinterface import SubstrateInterface 
-        from substrateinterface_polkascan.extensions import PolkascanSearchExtension
+        from substrateinterface import SubstrateInterface
+        from substrateinterface_polkascan.extensions import PolkascanExtension
         
         substrate = SubstrateInterface(url="ws://127.0.0.1:9944")
         
-        substrate.register_extension(PolkascanSearchExtension(url='http://127.0.0.1:8000/graphql/'))
+        substrate.register_extension(PolkascanExtension(url='http://127.0.0.1:8000/graphql/'))
         ```
         
         ## Usage
         
         ### Filter events
         
         ```python
```

### Comparing `substrate-interface-polkascan-0.1/README.md` & `substrate-interface-polkascan-0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Python Substrate Polkascan Extension
+# Python Substrate Interface: Polkascan Extension
 
 [![Latest Version](https://img.shields.io/pypi/v/substrate-interface-polkascan.svg)](https://pypi.org/project/substrate-interface-polkascan/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/substrate-interface-polkascan.svg)](https://pypi.org/project/substrate-interface/)
 [![License](https://img.shields.io/pypi/l/substrate-interface-polkascan.svg)](https://github.com/polkascan/py-substrate-interface-extension-polkascan/blob/master/LICENSE)
 
 
 ## Description
-This extension enables [Substrate Interface](https://github.com/polkascan/py-substrate-interface) to use indexes provided by [Polkascan Explorer API](https://github.com/polkascan/explorer#explorer-api-component)   
+This extension enables [Substrate Interface](https://github.com/polkascan/py-substrate-interface) to use indexes provided by the [Polkascan Explorer API](https://github.com/polkascan/explorer#explorer-api-component)   
 
 ## Installation
 ```bash
 pip install substrate-interface-polkascan
 ```
 
 ## Initialization
 
 ```python
-from substrateinterface import SubstrateInterface 
-from substrateinterface_polkascan.extensions import PolkascanSearchExtension
+from substrateinterface import SubstrateInterface
+from substrateinterface_polkascan.extensions import PolkascanExtension
 
 substrate = SubstrateInterface(url="ws://127.0.0.1:9944")
 
-substrate.register_extension(PolkascanSearchExtension(url='http://127.0.0.1:8000/graphql/'))
+substrate.register_extension(PolkascanExtension(url='http://127.0.0.1:8000/graphql/'))
 ```
 
 ## Usage
 
 ### Filter events
 
 ```python
```

### Comparing `substrate-interface-polkascan-0.1/setup.py` & `substrate-interface-polkascan-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-polkascan-0.1/substrate_interface_polkascan.egg-info/PKG-INFO` & `substrate-interface-polkascan-0.2/substrate_interface_polkascan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: substrate-interface-polkascan
-Version: 0.1
+Version: 0.2
 Summary: py-substrate-interface extension to utilize Polkascan API indexes
 Home-page: https://github.com/polkascan/py-substrate-interface-extension-polkascan
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
-Description: # Python Substrate Polkascan Extension
+Description: # Python Substrate Interface: Polkascan Extension
         
         [![Latest Version](https://img.shields.io/pypi/v/substrate-interface-polkascan.svg)](https://pypi.org/project/substrate-interface-polkascan/)
         [![Supported Python versions](https://img.shields.io/pypi/pyversions/substrate-interface-polkascan.svg)](https://pypi.org/project/substrate-interface/)
         [![License](https://img.shields.io/pypi/l/substrate-interface-polkascan.svg)](https://github.com/polkascan/py-substrate-interface-extension-polkascan/blob/master/LICENSE)
         
         
         ## Description
-        This extension enables [Substrate Interface](https://github.com/polkascan/py-substrate-interface) to use indexes provided by [Polkascan Explorer API](https://github.com/polkascan/explorer#explorer-api-component)   
+        This extension enables [Substrate Interface](https://github.com/polkascan/py-substrate-interface) to use indexes provided by the [Polkascan Explorer API](https://github.com/polkascan/explorer#explorer-api-component)   
         
         ## Installation
         ```bash
         pip install substrate-interface-polkascan
         ```
         
         ## Initialization
         
         ```python
-        from substrateinterface import SubstrateInterface 
-        from substrateinterface_polkascan.extensions import PolkascanSearchExtension
+        from substrateinterface import SubstrateInterface
+        from substrateinterface_polkascan.extensions import PolkascanExtension
         
         substrate = SubstrateInterface(url="ws://127.0.0.1:9944")
         
-        substrate.register_extension(PolkascanSearchExtension(url='http://127.0.0.1:8000/graphql/'))
+        substrate.register_extension(PolkascanExtension(url='http://127.0.0.1:8000/graphql/'))
         ```
         
         ## Usage
         
         ### Filter events
         
         ```python
```

### Comparing `substrate-interface-polkascan-0.1/substrateinterface_polkascan/__init__.py` & `substrate-interface-polkascan-0.2/substrateinterface_polkascan/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-polkascan-0.1/substrateinterface_polkascan/extensions.py` & `substrate-interface-polkascan-0.2/substrateinterface_polkascan/extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 
 from substrateinterface.extensions import SearchExtension
 from gql import gql, Client
 from gql.transport.aiohttp import AIOHTTPTransport
 
 
-class PolkascanSearchExtension(SearchExtension):
+class PolkascanExtension(SearchExtension):
 
     def __init__(self, url: str):
         self.url = url
         # Select your transport with a defined url endpoint
         transport = AIOHTTPTransport(url=url)
 
         # Create a GraphQL client using the defined transport
```

### Comparing `substrate-interface-polkascan-0.1/test/test_extension.py` & `substrate-interface-polkascan-0.2/test/test_extension.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 #  limitations under the License.
 #
 
 import unittest
 from os import environ
 
 from substrateinterface import SubstrateInterface
-from substrateinterface_polkascan.extensions import PolkascanSearchExtension
+from substrateinterface_polkascan.extensions import PolkascanExtension
 
 POLKADOT_NODE_URL = environ.get('SUBSTRATE_NODE_URL_POLKADOT') or 'ws://127.0.0.1:9944'
 POLKASCAN_API_URL = environ.get('POLKASCAN_API_URL') or 'http://127.0.0.1:8000/graphql/'
 
 
 class TestExtension(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.substrate = SubstrateInterface(url=POLKADOT_NODE_URL)
-        cls.substrate.register_extension(PolkascanSearchExtension(url=POLKASCAN_API_URL))
+        cls.substrate.register_extension(PolkascanExtension(url=POLKASCAN_API_URL))
 
     def test_filter_events(self):
 
         events = self.substrate.extensions.filter_events(pallet_name="Balances", event_name="Transfer", page_size=5)
 
         self.assertEqual(len(events), 5)
```

