# Comparing `tmp/substrate-interface-1.7.1.tar.gz` & `tmp/substrate-interface-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-interface-1.7.1.tar", last modified: Fri May 12 10:59:50 2023, max compression
+gzip compressed data, was "substrate-interface-1.7.2.tar", last modified: Wed Jun  7 13:46:41 2023, max compression
```

## Comparing `substrate-interface-1.7.1.tar` & `substrate-interface-1.7.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:59:50.569325 substrate-interface-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-12 10:59:50.569325 substrate-interface-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:59:50.569325 substrate-interface-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:59:50.565325 substrate-interface-1.7.1/substrate_interface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-12 10:59:50.000000 substrate-interface-1.7.1/substrate_interface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-12 10:59:50.000000 substrate-interface-1.7.1/substrate_interface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:59:50.000000 substrate-interface-1.7.1/substrate_interface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-12 10:59:50.000000 substrate-interface-1.7.1/substrate_interface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 10:59:50.000000 substrate-interface-1.7.1/substrate_interface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:59:50.565325 substrate-interface-1.7.1/substrateinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   126315 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    31151 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:59:50.565325 substrate-interface-1.7.1/substrateinterface/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/ecdsa_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/encrypted_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/ss58.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:59:50.569325 substrate-interface-1.7.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16587 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_create_extrinsics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_extension_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_rpc_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_runtime_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_ss58.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_type_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:46:41.012362 substrate-interface-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-07 13:46:41.012362 substrate-interface-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:46:41.012362 substrate-interface-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:46:41.008362 substrate-interface-1.7.2/substrate_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-07 13:46:40.000000 substrate-interface-1.7.2/substrate_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-07 13:46:40.000000 substrate-interface-1.7.2/substrate_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:46:40.000000 substrate-interface-1.7.2/substrate_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-07 13:46:40.000000 substrate-interface-1.7.2/substrate_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 13:46:40.000000 substrate-interface-1.7.2/substrate_interface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:46:41.008362 substrate-interface-1.7.2/substrateinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126315 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31530 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:46:41.012362 substrate-interface-1.7.2/substrateinterface/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/ecdsa_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/encrypted_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/ss58.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:46:41.012362 substrate-interface-1.7.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16587 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_create_extrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_extension_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_rpc_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_runtime_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_ss58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_type_registry.py
```

### Comparing `substrate-interface-1.7.1/LICENSE` & `substrate-interface-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/PKG-INFO` & `substrate-interface-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate-interface
-Version: 1.7.1
+Version: 1.7.2
 Summary: Library for interfacing with a Substrate node
 Home-page: https://github.com/polkascan/py-substrate-interface
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
 Description: # Python Substrate Interface
```

### Comparing `substrate-interface-1.7.1/README.md` & `substrate-interface-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/setup.py` & `substrate-interface-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrate_interface.egg-info/PKG-INFO` & `substrate-interface-1.7.2/substrate_interface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate-interface
-Version: 1.7.1
+Version: 1.7.2
 Summary: Library for interfacing with a Substrate node
 Home-page: https://github.com/polkascan/py-substrate-interface
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
 Description: # Python Substrate Interface
```

### Comparing `substrate-interface-1.7.1/substrate_interface.egg-info/SOURCES.txt` & `substrate-interface-1.7.2/substrate_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/__init__.py` & `substrate-interface-1.7.2/substrateinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/base.py` & `substrate-interface-1.7.2/substrateinterface/base.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/constants.py` & `substrate-interface-1.7.2/substrateinterface/constants.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/contracts.py` & `substrate-interface-1.7.2/substrateinterface/contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -785,28 +785,31 @@
 
             except NotImplementedError:
                 pass
 
         return call_result
 
     def exec(self, keypair: Keypair, method: str, args: dict = None,
-             value: int = 0, gas_limit: Optional[dict] = None, storage_deposit_limit: int = None
+             value: int = 0, gas_limit: Optional[dict] = None, storage_deposit_limit: int = None,
+             wait_for_inclusion: bool = True, wait_for_finalization: bool = False
              ) -> ContractExecutionReceipt:
         """
         Executes provided message by creating and submitting an extrinsic. To get a gas prediction or perform a
         'dry-run' of executing this message, see `ContractInstance.read`.
 
         Parameters
         ----------
         keypair
         method: name of message to execute
         args: arguments of message in {'name': value} format
         value: value to send when executing the message
         gas_limit: dict repesentation of `WeightV2` type. When omited the gas limit will be calculated with a `read()`
         storage_deposit_limit: The maximum amount of balance that can be charged to pay for the storage consumed
+        wait_for_inclusion: wait until extrinsic is included in a block (only works for websocket connections)
+        wait_for_finalization: wait until extrinsic is finalized (only works for websocket connections)
 
         Returns
         -------
         ContractExecutionReceipt
         """
 
         if gas_limit is None:
@@ -825,10 +828,12 @@
                 'storage_deposit_limit': storage_deposit_limit,
                 'data': input_data.to_hex()
             }
         )
 
         extrinsic = self.substrate.create_signed_extrinsic(call=call, keypair=keypair)
 
-        receipt = self.substrate.submit_extrinsic(extrinsic, wait_for_inclusion=True)
+        receipt = self.substrate.submit_extrinsic(
+            extrinsic, wait_for_inclusion=wait_for_inclusion, wait_for_finalization=wait_for_finalization
+        )
 
         return ContractExecutionReceipt.create_from_extrinsic_receipt(receipt, self.metadata)
```

### Comparing `substrate-interface-1.7.1/substrateinterface/exceptions.py` & `substrate-interface-1.7.2/substrateinterface/exceptions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/extensions.py` & `substrate-interface-1.7.2/substrateinterface/extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import TYPE_CHECKING
 
 import math
 from datetime import datetime, timedelta
 
-__all__ = ['Extension', 'SearchExtension', 'SubstrateNodeSearchExtension']
+__all__ = ['Extension', 'SearchExtension', 'SubstrateNodeExtension']
 
 if TYPE_CHECKING:
     from .base import SubstrateInterface
 
 
 class Extension:
     """
@@ -131,15 +131,15 @@
         Returns
         -------
         int
         """
         raise NotImplementedError()
 
 
-class SubstrateNodeSearchExtension(SearchExtension):
+class SubstrateNodeExtension(SearchExtension):
     """
     Implementation of `SearchExtension` using only Substrate RPC methods. Could be significant inefficient.
     """
 
     def filter_extrinsics(self, block_start: int = None, block_end: int = None, ss58_address: str = None,
                           pallet_name: str = None, call_name: str = None) -> list:
 
@@ -264,7 +264,12 @@
             current_delta = current_timestamp - target_block_timestamp
 
             self.debug_message(f"Current delta {current_delta} sec; predicted #{predicted_block_number}")
 
         self.debug_message(f"Accepted prediction #{predicted_block_number}")
 
         return predicted_block_number
+
+
+# Backwards compatibility
+class SubstrateNodeSearchExtension(SubstrateNodeExtension):
+    pass
```

### Comparing `substrate-interface-1.7.1/substrateinterface/interfaces.py` & `substrate-interface-1.7.2/substrateinterface/interfaces.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/key.py` & `substrate-interface-1.7.2/substrateinterface/key.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/keypair.py` & `substrate-interface-1.7.2/substrateinterface/keypair.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/storage.py` & `substrate-interface-1.7.2/substrateinterface/storage.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/utils/__init__.py` & `substrate-interface-1.7.2/substrateinterface/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/utils/caching.py` & `substrate-interface-1.7.2/substrateinterface/utils/caching.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/utils/ecdsa_helpers.py` & `substrate-interface-1.7.2/substrateinterface/utils/ecdsa_helpers.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/utils/encrypted_json.py` & `substrate-interface-1.7.2/substrateinterface/utils/encrypted_json.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/utils/hasher.py` & `substrate-interface-1.7.2/substrateinterface/utils/hasher.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/substrateinterface/utils/ss58.py` & `substrate-interface-1.7.2/substrateinterface/utils/ss58.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_block.py` & `substrate-interface-1.7.2/test/test_block.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_contracts.py` & `substrate-interface-1.7.2/test/test_contracts.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_create_extrinsics.py` & `substrate-interface-1.7.2/test/test_create_extrinsics.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_extension_interface.py` & `substrate-interface-1.7.2/test/test_extension_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,35 +16,39 @@
 
 from datetime import datetime, timezone
 
 import unittest
 
 from substrateinterface import SubstrateInterface
 from substrateinterface.exceptions import ExtensionCallNotFound
-from substrateinterface.extensions import SubstrateNodeSearchExtension
+from substrateinterface.extensions import SubstrateNodeExtension
 from test import settings
 
 
 class ExtensionsTestCase(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.substrate = SubstrateInterface(
             url=settings.POLKADOT_NODE_URL
         )
-        cls.substrate.register_extension(SubstrateNodeSearchExtension(max_block_range=100))
+        cls.substrate.register_extension(SubstrateNodeExtension(max_block_range=100))
 
     def test_search_block_number(self):
         block_datetime = datetime(2020, 7, 12, 0, 0, 0, tzinfo=timezone.utc)
 
         block_number = self.substrate.extensions.search_block_number(block_datetime=block_datetime)
 
         self.assertGreaterEqual(block_number, 665270)
         self.assertLessEqual(block_number, 665280)
 
+    def test_search_block_timestamp(self):
+        block_timestamp = self.substrate.extensions.get_block_timestamp(1000)
+        self.assertEqual(1590513426, block_timestamp)
+
     def test_unsupported_extension_call(self):
         with self.assertRaises(ExtensionCallNotFound):
             self.substrate.extensions.unknown()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `substrate-interface-1.7.1/test/test_helper_functions.py` & `substrate-interface-1.7.2/test/test_helper_functions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_init.py` & `substrate-interface-1.7.2/test/test_init.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_keypair.py` & `substrate-interface-1.7.2/test/test_keypair.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_query.py` & `substrate-interface-1.7.2/test/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             params=['GSEX8kR4Kz5UZGhvRUCJG93D5hhTAoVZ5tAe6Zne7V42DSi']
         )
 
         self.assertEqual(
             {
                 'nonce': 0, 'consumers': 0, 'providers': 0, 'sufficients': 0,
                 'data': {
-                    'free': 0, 'reserved': 0, 'misc_frozen': 0, 'fee_frozen': 0
+                    'free': 0, 'reserved': 0, 'frozen': 0, 'flags': 170141183460469231731687303715884105728
                 }
             }, result.value)
 
     def test_non_existing_query(self):
         with self.assertRaises(StorageFunctionNotFound) as cm:
             self.kusama_substrate.query("Unknown", "StorageFunction")
```

### Comparing `substrate-interface-1.7.1/test/test_query_map.py` & `substrate-interface-1.7.2/test/test_query_map.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_rpc_compatibility.py` & `substrate-interface-1.7.2/test/test_rpc_compatibility.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_runtime_call.py` & `substrate-interface-1.7.2/test/test_runtime_call.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_ss58.py` & `substrate-interface-1.7.2/test/test_ss58.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_subscriptions.py` & `substrate-interface-1.7.2/test/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.1/test/test_type_registry.py` & `substrate-interface-1.7.2/test/test_type_registry.py`

 * *Files identical despite different names*

