# Comparing `tmp/cyberutils-0.0.4.tar.gz` & `tmp/cyberutils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberutils-0.0.4.tar", max compression
+gzip compressed data, was "cyberutils-0.0.5.tar", max compression
```

## Comparing `cyberutils-0.0.4.tar` & `cyberutils-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1075 2023-05-12 07:27:50.772962 cyberutils-0.0.4/LICENSE
--rw-r--r--   0        0        0     3603 2023-05-12 07:27:50.772962 cyberutils-0.0.4/README.md
--rw-r--r--   0        0        0      166 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/__init__.py
--rw-r--r--   0        0        0       77 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/bash/__init__.py
--rw-r--r--   0        0        0     2268 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/bash/execution.py
--rw-r--r--   0        0        0       40 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/contract/__init__.py
--rw-r--r--   0        0        0     2739 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/contract/execution.py
--rw-r--r--   0        0        0       93 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/graphql/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/graphql/execution.py
--rw-r--r--   0        0        0     2032 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/graphql/queries.py
--rw-r--r--   0        0        0     1818 2023-05-12 07:27:50.776963 cyberutils-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5038 1970-01-01 00:00:00.000000 cyberutils-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-07 03:24:28.597267 cyberutils-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3913 2023-06-07 03:24:28.597267 cyberutils-0.0.5/README.md
+-rw-r--r--   0        0        0      166 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/__init__.py
+-rw-r--r--   0        0        0       77 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/bash/__init__.py
+-rw-r--r--   0        0        0     2268 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/bash/execution.py
+-rw-r--r--   0        0        0       40 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/contract/__init__.py
+-rw-r--r--   0        0        0     3070 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/contract/execution.py
+-rw-r--r--   0        0        0       93 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/graphql/__init__.py
+-rw-r--r--   0        0        0     2238 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/graphql/execution.py
+-rw-r--r--   0        0        0     2032 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/graphql/queries.py
+-rw-r--r--   0        0        0     1841 2023-06-07 03:24:28.597267 cyberutils-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5392 1970-01-01 00:00:00.000000 cyberutils-0.0.5/PKG-INFO
```

### Comparing `cyberutils-0.0.4/LICENSE` & `cyberutils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.4/README.md` & `cyberutils-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 get_json_from_bash_query(
     bash_command='cyber status --node https://rpc.bostrom.cybernode.ai:443')
 ```
 
 ### execute a cosmwasm contract
 
 ```python
+import requests
+
 from cyber_sdk.client.lcd import LCDClient
 from cyber_sdk.key.mnemonic import MnemonicKey
 
 from cyberutils.contract import execute_contract
 
 WALLET_SEED = 'rack canyon puzzle grow afford faint heavy kick furnace economy change loop debate tip acquire render rib truth bachelor monster page range wine measure'
 CONTRACT_ADDRESS = 'bostrom1nwm9pjmfgmxgc4euyfps05p9pfde8vd4sm8pavy93eu9xquz27dsgyxtml'
@@ -45,31 +47,38 @@
 lcd_client = LCDClient(
     url='https://lcd.bostrom.cybernode.ai/',
     chain_id='bostrom',
     prefix='bostrom'
 )
 wallet = lcd_client.wallet(mk)
 
-# the execution message in a contract must match its schema
+# an execution message in a contract must match its schema
 execute_msg = {
     "transfer" :  {
         "recipient": "bostrom1xszmhkfjs3s00z2nvtn7evqxw3dtus6yr8e4pw",
         "amount": "1000000"
     }
 }
 
+# load a contract schema for an execute message validation
+contract_schema_json = \
+    requests.get(
+        url='https://raw.githubusercontent.com/Snedashkovsky/cw-plus/main/contracts/cw20-base/schema/cw20-base.json'
+    ).json()
+
 # execution of a contract
 execute_contract(
     execute_msgs=[execute_msg],
     wallet=wallet,
     contract_address=CONTRACT_ADDRESS,
     lcd_client=lcd_client,
     gas=500_000,
     fee_amount=0,
     fee_denom='boot',
+    contract_execute_schema=contract_schema_json['execute'],
     memo='the first transfer')
 ```
 
 ### execute a graphql query
 
 ```python
 import pandas as pd
```

#### html2text {}

```diff
@@ -3,35 +3,39 @@
 PyPI_Package Â· GitHub_Repository
 ## usage ### execute bash query get bash query result and error ```python from
 cyberutils.bash import execute_bash execute_bash( bash_command='cyber status --
 node https://rpc.bostrom.cybernode.ai:443') ``` get json from bash query result
 ```python from cyberutils.bash import get_json_from_bash_query
 get_json_from_bash_query( bash_command='cyber status --node https://
 rpc.bostrom.cybernode.ai:443') ``` ### execute a cosmwasm contract ```python
-from cyber_sdk.client.lcd import LCDClient from cyber_sdk.key.mnemonic import
-MnemonicKey from cyberutils.contract import execute_contract WALLET_SEED =
-'rack canyon puzzle grow afford faint heavy kick furnace economy change loop
-debate tip acquire render rib truth bachelor monster page range wine measure'
-CONTRACT_ADDRESS =
+import requests from cyber_sdk.client.lcd import LCDClient from
+cyber_sdk.key.mnemonic import MnemonicKey from cyberutils.contract import
+execute_contract WALLET_SEED = 'rack canyon puzzle grow afford faint heavy kick
+furnace economy change loop debate tip acquire render rib truth bachelor
+monster page range wine measure' CONTRACT_ADDRESS =
 'bostrom1nwm9pjmfgmxgc4euyfps05p9pfde8vd4sm8pavy93eu9xquz27dsgyxtml' # initiate
 lcd client and wallet mk = MnemonicKey(mnemonic=WALLET_SEED) lcd_client =
 LCDClient( url='https://lcd.bostrom.cybernode.ai/', chain_id='bostrom',
-prefix='bostrom' ) wallet = lcd_client.wallet(mk) # the execution message in a
+prefix='bostrom' ) wallet = lcd_client.wallet(mk) # an execution message in a
 contract must match its schema execute_msg = { "transfer" : { "recipient":
 "bostrom1xszmhkfjs3s00z2nvtn7evqxw3dtus6yr8e4pw", "amount": "1000000" } } #
-execution of a contract execute_contract( execute_msgs=[execute_msg],
-wallet=wallet, contract_address=CONTRACT_ADDRESS, lcd_client=lcd_client,
-gas=500_000, fee_amount=0, fee_denom='boot', memo='the first transfer') ``` ###
-execute a graphql query ```python import pandas as pd from cyberutils.graphql
-import execute_graphql res = await execute_graphql( request=""" query
-AllContracts { contracts(order_by: {tx: desc_nulls_last}) { address admin
-code_id creation_time creator fees gas height label tx } } """,
-graphql_url='https://index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res
-['contracts']) ``` a query with variable values ```python import pandas as pd
-from cyberutils.graphql import execute_graphql res = await execute_graphql
+load a contract schema for an execute message validation contract_schema_json =
+\ requests.get( url='https://raw.githubusercontent.com/Snedashkovsky/cw-plus/
+main/contracts/cw20-base/schema/cw20-base.json' ).json() # execution of a
+contract execute_contract( execute_msgs=[execute_msg], wallet=wallet,
+contract_address=CONTRACT_ADDRESS, lcd_client=lcd_client, gas=500_000,
+fee_amount=0, fee_denom='boot', contract_execute_schema=contract_schema_json
+['execute'], memo='the first transfer') ``` ### execute a graphql query
+```python import pandas as pd from cyberutils.graphql import execute_graphql
+res = await execute_graphql( request=""" query AllContracts { contracts
+(order_by: {tx: desc_nulls_last}) { address admin code_id creation_time creator
+fees gas height label tx } } """, graphql_url='https://
+index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res['contracts']) ``` a
+query with variable values ```python import pandas as pd from
+cyberutils.graphql import execute_graphql res = await execute_graphql
 ( request=""" query ContractsCodeID($code_id: bigint) { contracts(order_by:
 {tx: desc_nulls_last}, where: {code_id: {_eq: $code_id}}) { address admin
 creation_time creator fees gas height label tx code_id } } """,
 variable_values={"code_id": "3"}, graphql_url='https://
 index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res['contracts']) ``` get
 messages with a given address and type ```python import pandas as pd from
 cyberutils.graphql import get_messages_by_address_and_type res = await
```

### Comparing `cyberutils-0.0.4/cyberutils/bash/execution.py` & `cyberutils-0.0.5/cyberutils/bash/execution.py`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.4/cyberutils/contract/execution.py` & `cyberutils-0.0.5/cyberutils/contract/execution.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from jsonschema import validate
 from typing import Optional, Union
 
 from cyber_sdk.client.lcd import LCDClient
 from cyber_sdk.client.lcd.api.tx import CreateTxOptions, BlockTxBroadcastResult, SignerOptions
 from cyber_sdk.client.lcd.wallet import Wallet
 from cyber_sdk.core import Coin, Coins, AccAddress
 from cyber_sdk.core.fee import Fee
@@ -15,30 +16,36 @@
                      lcd_client: LCDClient,
                      fee_denom: str,
                      fee_amount: int = 0,
                      gas: int = 300_000,
                      wallet: Optional[Wallet] = None,
                      sender: Optional[Union[str, AccAddress]] = None,
                      sign_and_broadcast_tx: bool = True,
+                     contract_execute_schema: Optional[dict] = None,
                      memo: Optional[str] = None) -> Optional[Union[BlockTxBroadcastResult, Tx]]:
     """
     Execute contract list of messages for a contract in a transaction or get an unsigned transaction
     :param execute_msgs: list of execute messages
     :param contract_address: contract address
     :param lcd_client: network LCD client
     :param gas: amount of gas
     :param fee_amount: fee amount
     :param fee_denom: fee denom
     :param wallet: executable wallet
     :param sender: transaction sender address
     :param sign_and_broadcast_tx: sign and broadcast a transaction if true, otherwise return an unsigned transaction
+    :param contract_execute_schema: schema of contract execute messages for message validation
     :param memo: note(memo) of a transaction
     :return: a transaction result or an unsigned transaction
     """
     assert ((wallet or sender) and not sign_and_broadcast_tx) or (wallet and sign_and_broadcast_tx)
+    if contract_execute_schema:
+        for _execute_msg in execute_msgs:
+            validate(_execute_msg, contract_execute_schema)
+
     _sender = wallet.key.acc_address if sender is None else AccAddress(sender)
     _msgs = \
         [MsgExecuteContract(
             sender=_sender,
             contract=AccAddress(contract_address),
             execute_msg=execute_msg) for execute_msg in execute_msgs]
```

### Comparing `cyberutils-0.0.4/cyberutils/graphql/execution.py` & `cyberutils-0.0.5/cyberutils/graphql/execution.py`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.4/cyberutils/graphql/queries.py` & `cyberutils-0.0.5/cyberutils/graphql/queries.py`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.4/pyproject.toml` & `cyberutils-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 documentation = "https://github.com/Snedashkovsky/cyberutils"
 homepage = "https://github.com/Snedashkovsky/cyberutils"
 keywords = ["bostrom", "cyber", "knowledge-graph", "dex", "swap", "defi", "crypto", "blockchain", ]
 license = "MIT"
 packages = [{ include = "cyberutils" }]
 readme = "README.md"
 repository = "https://github.com/Snedashkovsky/cyberutils.git"
-version = "0.0.4"
+version = "0.0.5"
 
 [tool.poetry.dependencies]
 pandas = "^1.0.0"
 numpy = "^1.0.0"
 python-dotenv = "^0.20.0"
 tqdm = "^4.0.0"
 ipython = "^8.0.0"
 pandarallel = "^1.6.0"
 multiprocess = "^0.70.14"
 python = "^3.9"
 cyber_sdk = "^1.1.2"
+jsonschema = "^4.17.1"
 gql = { version = "^3.0.0", extras = ["all"] }
 
 [tool.poetry.dev-dependencies]
 aioresponses = "^0.7.2"
 asynctest = "^0.13.0"
 pytest-cov = "^3.0.0"
 pytest = "^7.0.1"
```

### Comparing `cyberutils-0.0.4/PKG-INFO` & `cyberutils-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberutils
-Version: 0.0.4
+Version: 0.0.5
 Summary: the toolset for cyber protocol and cosmos ecosystem
 Home-page: https://github.com/Snedashkovsky/cyberutils
 License: MIT
 Keywords: bostrom,cyber,knowledge-graph,dex,swap,defi,crypto,blockchain
 Author: Snedashkovsky,
 Author-email: sn@cyberdrop.ai
 Requires-Python: >=3.9,<4.0
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: cyber_sdk (>=1.1.2,<2.0.0)
 Requires-Dist: gql[all] (>=3.0.0,<4.0.0)
 Requires-Dist: ipython (>=8.0.0,<9.0.0)
+Requires-Dist: jsonschema (>=4.17.1,<5.0.0)
 Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
 Requires-Dist: numpy (>=1.0.0,<2.0.0)
 Requires-Dist: pandarallel (>=1.6.0,<2.0.0)
 Requires-Dist: pandas (>=1.0.0,<2.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: tqdm (>=4.0.0,<5.0.0)
 Project-URL: Documentation, https://github.com/Snedashkovsky/cyberutils
@@ -62,14 +63,16 @@
 get_json_from_bash_query(
     bash_command='cyber status --node https://rpc.bostrom.cybernode.ai:443')
 ```
 
 ### execute a cosmwasm contract
 
 ```python
+import requests
+
 from cyber_sdk.client.lcd import LCDClient
 from cyber_sdk.key.mnemonic import MnemonicKey
 
 from cyberutils.contract import execute_contract
 
 WALLET_SEED = 'rack canyon puzzle grow afford faint heavy kick furnace economy change loop debate tip acquire render rib truth bachelor monster page range wine measure'
 CONTRACT_ADDRESS = 'bostrom1nwm9pjmfgmxgc4euyfps05p9pfde8vd4sm8pavy93eu9xquz27dsgyxtml'
@@ -79,31 +82,38 @@
 lcd_client = LCDClient(
     url='https://lcd.bostrom.cybernode.ai/',
     chain_id='bostrom',
     prefix='bostrom'
 )
 wallet = lcd_client.wallet(mk)
 
-# the execution message in a contract must match its schema
+# an execution message in a contract must match its schema
 execute_msg = {
     "transfer" :  {
         "recipient": "bostrom1xszmhkfjs3s00z2nvtn7evqxw3dtus6yr8e4pw",
         "amount": "1000000"
     }
 }
 
+# load a contract schema for an execute message validation
+contract_schema_json = \
+    requests.get(
+        url='https://raw.githubusercontent.com/Snedashkovsky/cw-plus/main/contracts/cw20-base/schema/cw20-base.json'
+    ).json()
+
 # execution of a contract
 execute_contract(
     execute_msgs=[execute_msg],
     wallet=wallet,
     contract_address=CONTRACT_ADDRESS,
     lcd_client=lcd_client,
     gas=500_000,
     fee_amount=0,
     fee_denom='boot',
+    contract_execute_schema=contract_schema_json['execute'],
     memo='the first transfer')
 ```
 
 ### execute a graphql query
 
 ```python
 import pandas as pd
```

#### html2text {}

```diff
@@ -1,56 +1,61 @@
-Metadata-Version: 2.1 Name: cyberutils Version: 0.0.4 Summary: the toolset for
+Metadata-Version: 2.1 Name: cyberutils Version: 0.0.5 Summary: the toolset for
 cyber protocol and cosmos ecosystem Home-page: https://github.com/
 Snedashkovsky/cyberutils License: MIT Keywords: bostrom,cyber,knowledge-
 graph,dex,swap,defi,crypto,blockchain Author: Snedashkovsky, Author-email:
 sn@cyberdrop.ai Requires-Python: >=3.9,<4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9 Requires-Dist: cyber_sdk
 (>=1.1.2,<2.0.0) Requires-Dist: gql[all] (>=3.0.0,<4.0.0) Requires-Dist:
-ipython (>=8.0.0,<9.0.0) Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
-Requires-Dist: numpy (>=1.0.0,<2.0.0) Requires-Dist: pandarallel
-(>=1.6.0,<2.0.0) Requires-Dist: pandas (>=1.0.0,<2.0.0) Requires-Dist: python-
-dotenv (>=0.20.0,<0.21.0) Requires-Dist: tqdm (>=4.0.0,<5.0.0) Project-URL:
-Documentation, https://github.com/Snedashkovsky/cyberutils Project-URL:
-Repository, https://github.com/Snedashkovsky/cyberutils.git Description-
-Content-Type: text/markdown # cyberutils
+ipython (>=8.0.0,<9.0.0) Requires-Dist: jsonschema (>=4.17.1,<5.0.0) Requires-
+Dist: multiprocess (>=0.70.14,<0.71.0) Requires-Dist: numpy (>=1.0.0,<2.0.0)
+Requires-Dist: pandarallel (>=1.6.0,<2.0.0) Requires-Dist: pandas
+(>=1.0.0,<2.0.0) Requires-Dist: python-dotenv (>=0.20.0,<0.21.0) Requires-Dist:
+tqdm (>=4.0.0,<5.0.0) Project-URL: Documentation, https://github.com/
+Snedashkovsky/cyberutils Project-URL: Repository, https://github.com/
+Snedashkovsky/cyberutils.git Description-Content-Type: text/markdown #
+cyberutils
 [GitHub] [Python] [pip]
 PyPI_Package Â· GitHub_Repository
 ## usage ### execute bash query get bash query result and error ```python from
 cyberutils.bash import execute_bash execute_bash( bash_command='cyber status --
 node https://rpc.bostrom.cybernode.ai:443') ``` get json from bash query result
 ```python from cyberutils.bash import get_json_from_bash_query
 get_json_from_bash_query( bash_command='cyber status --node https://
 rpc.bostrom.cybernode.ai:443') ``` ### execute a cosmwasm contract ```python
-from cyber_sdk.client.lcd import LCDClient from cyber_sdk.key.mnemonic import
-MnemonicKey from cyberutils.contract import execute_contract WALLET_SEED =
-'rack canyon puzzle grow afford faint heavy kick furnace economy change loop
-debate tip acquire render rib truth bachelor monster page range wine measure'
-CONTRACT_ADDRESS =
+import requests from cyber_sdk.client.lcd import LCDClient from
+cyber_sdk.key.mnemonic import MnemonicKey from cyberutils.contract import
+execute_contract WALLET_SEED = 'rack canyon puzzle grow afford faint heavy kick
+furnace economy change loop debate tip acquire render rib truth bachelor
+monster page range wine measure' CONTRACT_ADDRESS =
 'bostrom1nwm9pjmfgmxgc4euyfps05p9pfde8vd4sm8pavy93eu9xquz27dsgyxtml' # initiate
 lcd client and wallet mk = MnemonicKey(mnemonic=WALLET_SEED) lcd_client =
 LCDClient( url='https://lcd.bostrom.cybernode.ai/', chain_id='bostrom',
-prefix='bostrom' ) wallet = lcd_client.wallet(mk) # the execution message in a
+prefix='bostrom' ) wallet = lcd_client.wallet(mk) # an execution message in a
 contract must match its schema execute_msg = { "transfer" : { "recipient":
 "bostrom1xszmhkfjs3s00z2nvtn7evqxw3dtus6yr8e4pw", "amount": "1000000" } } #
-execution of a contract execute_contract( execute_msgs=[execute_msg],
-wallet=wallet, contract_address=CONTRACT_ADDRESS, lcd_client=lcd_client,
-gas=500_000, fee_amount=0, fee_denom='boot', memo='the first transfer') ``` ###
-execute a graphql query ```python import pandas as pd from cyberutils.graphql
-import execute_graphql res = await execute_graphql( request=""" query
-AllContracts { contracts(order_by: {tx: desc_nulls_last}) { address admin
-code_id creation_time creator fees gas height label tx } } """,
-graphql_url='https://index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res
-['contracts']) ``` a query with variable values ```python import pandas as pd
-from cyberutils.graphql import execute_graphql res = await execute_graphql
+load a contract schema for an execute message validation contract_schema_json =
+\ requests.get( url='https://raw.githubusercontent.com/Snedashkovsky/cw-plus/
+main/contracts/cw20-base/schema/cw20-base.json' ).json() # execution of a
+contract execute_contract( execute_msgs=[execute_msg], wallet=wallet,
+contract_address=CONTRACT_ADDRESS, lcd_client=lcd_client, gas=500_000,
+fee_amount=0, fee_denom='boot', contract_execute_schema=contract_schema_json
+['execute'], memo='the first transfer') ``` ### execute a graphql query
+```python import pandas as pd from cyberutils.graphql import execute_graphql
+res = await execute_graphql( request=""" query AllContracts { contracts
+(order_by: {tx: desc_nulls_last}) { address admin code_id creation_time creator
+fees gas height label tx } } """, graphql_url='https://
+index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res['contracts']) ``` a
+query with variable values ```python import pandas as pd from
+cyberutils.graphql import execute_graphql res = await execute_graphql
 ( request=""" query ContractsCodeID($code_id: bigint) { contracts(order_by:
 {tx: desc_nulls_last}, where: {code_id: {_eq: $code_id}}) { address admin
 creation_time creator fees gas height label tx code_id } } """,
 variable_values={"code_id": "3"}, graphql_url='https://
 index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res['contracts']) ``` get
 messages with a given address and type ```python import pandas as pd from
 cyberutils.graphql import get_messages_by_address_and_type res = await
```

