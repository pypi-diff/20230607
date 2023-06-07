# Comparing `tmp/sui_brownie-1.0.4-py3-none-any.whl.zip` & `tmp/sui_brownie-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27902 bytes, number of entries: 16
+Zip file size: 27906 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
 -rw-r--r--  2.0 unx    12144 b- defN 23-Apr-21 09:58 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    94854 b- defN 23-May-11 09:08 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    94808 b- defN 23-Jun-07 02:58 sui_brownie/sui_brownie.py
 -rw-r--r--  2.0 unx    32439 b- defN 23-Apr-19 08:03 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-11 09:14 sui_brownie-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 09:14 sui_brownie-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-11 09:14 sui_brownie-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1296 b- defN 23-May-11 09:14 sui_brownie-1.0.4.dist-info/RECORD
-16 files, 160657 bytes uncompressed, 25768 bytes compressed:  84.0%
+-rw-r--r--  2.0 unx     1002 b- defN 23-Jun-07 02:58 sui_brownie-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 02:58 sui_brownie-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-07 02:58 sui_brownie-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1297 b- defN 23-Jun-07 02:58 sui_brownie-1.0.5.dist-info/RECORD
+16 files, 160632 bytes uncompressed, 25772 bytes compressed:  84.0%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-1.0.4.dist-info/METADATA
+Filename: sui_brownie-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-1.0.4.dist-info/WHEEL
+Filename: sui_brownie-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-1.0.4.dist-info/top_level.txt
+Filename: sui_brownie-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-1.0.4.dist-info/RECORD
+Filename: sui_brownie-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/sui_brownie.py

```diff
@@ -6,29 +6,27 @@
 import hashlib
 import json
 import multiprocessing
 import os
 import time
 import traceback
 from pathlib import Path
-from typing import Union, Dict
 from pprint import pprint
-from retrying import retry
-
-from dotenv import dotenv_values
-
-from atomicwrites import atomic_write
+from typing import Union, Dict
 
-import yaml
 import toml
+import yaml
+from atomicwrites import atomic_write
+from dotenv import dotenv_values
+from retrying import retry
 
-from .account import Account
-from .parallelism import ThreadExecutor
 from . import bcs
+from .account import Account
 from .bcs import *
+from .parallelism import ThreadExecutor
 from .sui_client import SuiClient
 
 _load_project = []
 
 _cache_file_lock = multiprocessing.Lock()
 
 
@@ -473,15 +471,15 @@
     def generate_call_arg(cls, param_type, data, object_infos):
         if isinstance(param_type, dict) and \
                 ("MutableReference" in param_type or
                  "Reference" in param_type or
                  "Struct" in param_type):
             if "Vector" in param_type.get("MutableReference", {}) or "Vector" in param_type.get("Reference",
                                                                                                 {}) or "Vector" in param_type.get(
-                    "Struct", {}):
+                "Struct", {}):
                 assert isinstance(data, list)
                 call_args = []
                 for object_id in data:
                     call_args.append(CallArg("Object", cls.generate_object_arg(object_id, object_infos, param_type)))
                 return call_args
             else:
                 return CallArg("Object", cls.generate_object_arg(data, object_infos, param_type))
@@ -948,41 +946,41 @@
     @classmethod
     def dola_upgrade(
             cls,
             package_id,
             proposal_package_id,
             sender,
             governance_info: str,
-            governance_contracts: str,
+            governance_genesis: str,
             proposal: str,
             compiled_modules: list,
             dep_ids,
             gas_price,
             gas_budget
     ):
-        object_infos = cls.get_objects([governance_info, governance_contracts, proposal])
+        object_infos = cls.get_objects([governance_info, governance_genesis, proposal])
         inputs = [
             CallArg("Object", ObjectArg("SharedObject",
                                         SharedObject(
                                             ObjectID(governance_info),
                                             SequenceNumber(int(object_infos[governance_info]["owner"]["Shared"]
                                                                ["initial_shared_version"])),
                                             Bool(False)
                                         ))),
             CallArg("Object", ObjectArg("SharedObject",
                                         SharedObject(
-                                            ObjectID(governance_contracts),
-                                            SequenceNumber(int(object_infos[governance_contracts]["owner"]["Shared"]
+                                            ObjectID(proposal),
+                                            SequenceNumber(int(object_infos[proposal]["owner"]["Shared"]
                                                                ["initial_shared_version"])),
                                             Bool(True)
                                         ))),
             CallArg("Object", ObjectArg("SharedObject",
                                         SharedObject(
-                                            ObjectID(proposal),
-                                            SequenceNumber(int(object_infos[proposal]["owner"]["Shared"]
+                                            ObjectID(governance_genesis),
+                                            SequenceNumber(int(object_infos[governance_genesis]["owner"]["Shared"]
                                                                ["initial_shared_version"])),
                                             Bool(True)
                                         ))),
         ]
         arguments = [Argument("Input", U16(i)) for i in range(len(inputs))]
         commands = [
             Command("MoveCall", ProgrammableMoveCall(
@@ -999,15 +997,15 @@
                 Argument("Result", U16(0))
             )),
             Command("MoveCall", ProgrammableMoveCall(
                 ObjectID(proposal_package_id),
                 Identifier("upgrade_proposal"),
                 Identifier("commit_upgrade"),
                 [],
-                [Argument("Input", U16(1)), Argument("Result", U16(1))]
+                [Argument("Input", U16(2)), Argument("Result", U16(1))]
             )),
         ]
 
         return cls.build_intent_message(sender, inputs, commands, gas_price, gas_budget)
 
     @classmethod
     def pay_all_sui(
@@ -1429,15 +1427,15 @@
             gas_budget = self.project.gas_budget
         if gas_price is None:
             gas_price = self.project.estimate_gas_price()
         replace_tomls = self.replace_addresses(replace_address=replace_address,
                                                replace_publish_at=replace_publish_at,
                                                output=dict())
         try:
-            cmd = f"sui move build --dump-bytecode-as-base64 --legacy-digest " \
+            cmd = f"sui move build --dump-bytecode-as-base64 " \
                   f"--path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             try:
                 first_part_start = result.find("{")
                 first_part_end = result.find("}") + 1
                 result = json.loads(result[first_part_start:first_part_end])
@@ -1488,45 +1486,45 @@
             replace_address: dict = None,
             replace_publish_at: dict = None,
     ):
         replace_tomls = self.replace_addresses(replace_address=replace_address,
                                                replace_publish_at=replace_publish_at,
                                                output=dict())
         try:
-            cmd = f"sui move build --legacy-digest " \
+            cmd = f"sui move build --dump-bytecode-as-base64 " \
                   f"--path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             return result
         except:
             traceback.print_exc()
 
         for k in replace_tomls:
             replace_tomls[k].restore()
 
     def program_dola_upgrade_package(
             self,
             proposal_package_id,
             governance_info: str,
-            governance_contracts: str,
+            governance_genesis: str,
             proposal: str,
             replace_address: dict = None,
             replace_publish_at: dict = None,
             gas_price=None,
             gas_budget=None,
     ):
         if gas_budget is None:
             gas_budget = self.project.gas_budget
         if gas_price is None:
             gas_price = self.project.estimate_gas_price()
         replace_tomls = self.replace_addresses(replace_address=replace_address,
                                                replace_publish_at=replace_publish_at,
                                                output=dict())
         try:
-            cmd = f"sui move build --dump-bytecode-as-base64 --legacy-digest " \
+            cmd = f"sui move build --dump-bytecode-as-base64 " \
                   f"--path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             try:
                 first_part_start = result.find("{")
                 first_part_end = result.find("}") + 1
                 result = json.loads(result[first_part_start:first_part_end])
@@ -1544,15 +1542,15 @@
             print("\n" + "-" * 50 + view + "-" * 50)
             result = self.project.dola_upgrade(
                 self.package_id,
                 proposal_package_id,
                 move_modules,
                 dep_ids,
                 governance_info,
-                governance_contracts,
+                governance_genesis,
                 proposal,
                 gas_price,
                 gas_budget,
             )
             self.update_abi()
             result = self.format_result(result)
             pprint(result)
@@ -2287,15 +2285,15 @@
     def dola_upgrade(
             self,
             package_id,
             proposal_package_id,
             compiled_modules,
             dep_ids,
             governance_info: str,
-            governance_contracts: str,
+            governance_genesis: str,
             proposal: str,
             gas_price=None,
             gas_budget=None
     ):
         if gas_budget is None:
             gas_budget = self.gas_budget
         if gas_price is None:
@@ -2303,15 +2301,15 @@
         msg = TransactionBuild.dola_upgrade(
             package_id=package_id,
             proposal_package_id=proposal_package_id,
             sender=self.account.account_address,
             compiled_modules=compiled_modules,
             dep_ids=dep_ids,
             governance_info=governance_info,
-            governance_contracts=governance_contracts,
+            governance_genesis=governance_genesis,
             proposal=proposal,
             gas_price=gas_price,
             gas_budget=gas_budget)
 
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
         self.simulate_fail_abort(tx_bytes)
```

## Comparing `sui_brownie-1.0.4.dist-info/METADATA` & `sui_brownie-1.0.5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 1.0.4
+Version: 1.0.5
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
@@ -23,7 +24,9 @@
 Requires-Dist: retrying
 Requires-Dist: mnemonic
 Requires-Dist: httpx
 Requires-Dist: python-dotenv
 Requires-Dist: pynacl
 
 This is an sui python tool to quickly implement sui calls
+
+
```

## Comparing `sui_brownie-1.0.4.dist-info/RECORD` & `sui_brownie-1.0.5.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 sui_brownie/MANIFEST.in,sha256=BzExY9sw9x0Pqk6SYHuMRRvYS-cm75AxBOBjsYGFfU4,10
 sui_brownie/README.md,sha256=-7DxT6cGHbWLr_VufOEwIzl4Vtojp5dZc_r89lwnK3o,878
 sui_brownie/__init__.py,sha256=ROrbn7qi0haZjB8FG5JqXpD5mQ6qQPDNOwe0-rPnKeM,38
 sui_brownie/account.py,sha256=suZRI__kDNhyuoCZ9_q4mIV673lJDz0jgj0HyEj_hsQ,2514
 sui_brownie/bcs.py,sha256=8LwJihqmjLGwtzq87XKAQhE7ZgxiRDUsUYRbK6yRy7s,12144
 sui_brownie/ed25519.py,sha256=8hLHtC21og60B3MzXi4JmdQoOCbUutExyQIJhypJ9dg,4326
 sui_brownie/parallelism.py,sha256=Thh7TUrRU1fn47lNTF30RrcL5lBPBeMT2DX9A_swXDg,10047
-sui_brownie/sui_brownie.py,sha256=-BcQJj13TIXHqf8TfWwGQWfa0OwkHR-FNQUJ8BleVqQ,94854
+sui_brownie/sui_brownie.py,sha256=IzdkmRLqCtcvPbnTy_V0QlE_c667iouBtQlqOAOMy-A,94808
 sui_brownie/sui_client.py,sha256=Epyu5pXAI6jl_L-lzBg4gnNLYQVjdQTZ8kR4YrJfnqk,32439
 sui_brownie/sui_config.template.yaml,sha256=Qa6n48nf4qeLDhZnpVNjZJIYDm8jYFs7dVLCyLjxMTs,140
 sui_brownie/sui_keystore.template.keystore,sha256=dIQsJL_H6FdnGlET9u5NYXSmjTc1-8dk8wZWKrzcLOM,19
 sui_brownie/utils.py,sha256=bttovGstKoozRoMvzYFOFs_z73aled7UFbNBDPxX9Uo,866
-sui_brownie-1.0.4.dist-info/METADATA,sha256=InbTzbxWdOelznyTittfwPQD6UkMUVtOlDM0W3J_mB4,982
-sui_brownie-1.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sui_brownie-1.0.4.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
-sui_brownie-1.0.4.dist-info/RECORD,,
+sui_brownie-1.0.5.dist-info/METADATA,sha256=TVk2AymYjM6k9uUSJ-vgwRTNpkz_LtV5KNBkPYNCnj8,1002
+sui_brownie-1.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sui_brownie-1.0.5.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
+sui_brownie-1.0.5.dist-info/RECORD,,
```

