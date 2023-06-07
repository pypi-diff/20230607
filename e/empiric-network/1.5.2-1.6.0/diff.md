# Comparing `tmp/empiric_network-1.5.2.tar.gz` & `tmp/empiric_network-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empiric_network-1.5.2.tar", max compression
+gzip compressed data, was "empiric_network-1.6.0.tar", max compression
```

## Comparing `empiric_network-1.5.2.tar` & `empiric_network-1.6.0.tar`

### file list

```diff
@@ -1,64 +1,42 @@
--rw-r--r--   0        0        0      284 2023-04-23 18:47:52.389966 empiric_network-1.5.2/README.md
--rw-r--r--   0        0        0        0 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/__init__.py
--rw-r--r--   0        0        0      204 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/cli/.example.config copy.ini
--rw-r--r--   0        0        0      697 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/cli/README.md
--rw-r--r--   0        0        0      342 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/cli/__init__.py
--rw-r--r--   0        0        0      148 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/cli/__main__.py
--rw-r--r--   0        0        0     1628 2023-04-23 18:47:52.389966 empiric_network-1.5.2/empiric/cli/account.py
--rw-r--r--   0        0        0   544336 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/compiled_account_contract.py
--rw-r--r--   0        0        0     2050 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/config.py
--rw-r--r--   0        0        0     1118 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/contracts/__init__.py
--rw-r--r--   0        0        0     8098 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/contracts/oracle.py
--rw-r--r--   0        0        0     5217 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/contracts/publisher_registry.py
--rw-r--r--   0        0        0     2638 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/contracts/summary_stats.py
--rw-r--r--   0        0        0     3318 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/contracts/utils.py
--rw-r--r--   0        0        0     4080 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/empiric_cli.py
--rw-r--r--   0        0        0     2682 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/net.py
--rw-r--r--   0        0        0     1420 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/publisher/__init__.py
--rw-r--r--   0        0        0    12230 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/randomness/__init__.py
--rw-r--r--   0        0        0    16306 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/randomness/randomness_utils.py
--rw-r--r--   0        0        0     3682 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/randomness/utils.py
--rw-r--r--   0        0        0      547 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/sample_config/oracle_constructor_data.json
--rw-r--r--   0        0        0        0 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/tests/__init__.py
--rw-r--r--   0        0        0      262 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/tests/test_empiric_cli.py
--rw-r--r--   0        0        0      236 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/cli/utils.py
--rw-r--r--   0        0        0      193 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/__init__.py
--rw-r--r--   0        0        0      284 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/__init__.py
--rw-r--r--   0        0        0    14135 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/oracle.py
--rw-r--r--   0        0        0     1436 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/proxy.py
--rw-r--r--   0        0        0     3896 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/publisher_registry.py
--rw-r--r--   0        0        0     5912 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/randomness.py
--rw-r--r--   0        0        0      868 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/abis/summary_stats.py
--rw-r--r--   0        0        0     4557 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/client.py
--rw-r--r--   0        0        0     2150 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/config.py
--rw-r--r--   0        0        0     3801 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/contract.py
--rw-r--r--   0        0        0     9972 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/entry.py
--rw-r--r--   0        0        0      387 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/logger.py
--rw-r--r--   0        0        0      295 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/__init__.py
--rw-r--r--   0        0        0    25441 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/evm.py
--rw-r--r--   0        0        0     3074 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/nonce.py
--rw-r--r--   0        0        0     8808 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/oracle.py
--rw-r--r--   0        0        0     2287 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0     3065 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/mixins/transactions.py
--rw-r--r--   0        0        0     3306 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/types.py
--rw-r--r--   0        0        0      880 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/core/utils.py
--rw-r--r--   0        0        0       82 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/__init__.py
--rw-r--r--   0        0        0     2716 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/assets.py
--rw-r--r--   0        0        0     2261 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/client.py
--rw-r--r--   0        0        0      354 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     3755 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     3017 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     3380 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2953 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3980 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     3826 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/defillama.py
--rw-r--r--   0        0        0     3814 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     3754 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/kaiko.py
--rw-r--r--   0        0        0     3631 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     3762 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0      668 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/publisher/types.py
--rw-r--r--   0        0        0        0 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/test/__init__.py
--rw-r--r--   0        0        0     5965 2023-04-23 18:47:52.393966 empiric_network-1.5.2/empiric/test/interface_consistency.py
--rw-r--r--   0        0        0     1088 2023-04-23 18:47:52.393966 empiric_network-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 empiric_network-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-06-07 10:39:12.630562 empiric_network-1.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/__init__.py
+-rw-r--r--   0        0        0      193 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/__init__.py
+-rw-r--r--   0        0        0      284 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/__init__.py
+-rw-r--r--   0        0        0    14135 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/oracle.py
+-rw-r--r--   0        0        0     1436 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/proxy.py
+-rw-r--r--   0        0        0     3896 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/publisher_registry.py
+-rw-r--r--   0        0        0     5912 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/randomness.py
+-rw-r--r--   0        0        0      868 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/summary_stats.py
+-rw-r--r--   0        0        0     4232 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/client.py
+-rw-r--r--   0        0        0     1461 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/config.py
+-rw-r--r--   0        0        0     3801 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/contract.py
+-rw-r--r--   0        0        0     9972 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/entry.py
+-rw-r--r--   0        0        0      387 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/logger.py
+-rw-r--r--   0        0        0      295 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/__init__.py
+-rw-r--r--   0        0        0    25441 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/evm.py
+-rw-r--r--   0        0        0     3074 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/nonce.py
+-rw-r--r--   0        0        0     8808 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2287 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0     3065 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/transactions.py
+-rw-r--r--   0        0        0     3886 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/types.py
+-rw-r--r--   0        0        0      880 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/utils.py
+-rw-r--r--   0        0        0       82 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/__init__.py
+-rw-r--r--   0        0        0     2716 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/assets.py
+-rw-r--r--   0        0        0     2261 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/client.py
+-rw-r--r--   0        0        0      354 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3755 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     3017 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     3380 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2953 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3980 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     3826 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/defillama.py
+-rw-r--r--   0        0        0     3814 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     3754 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/kaiko.py
+-rw-r--r--   0        0        0     3631 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     3762 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0      668 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/types.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/test/__init__.py
+-rw-r--r--   0        0        0     5965 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/test/interface_consistency.py
+-rw-r--r--   0        0        0     1016 2023-06-07 10:39:12.630562 empiric_network-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 empiric_network-1.6.0/PKG-INFO
```

### Comparing `empiric_network-1.5.2/empiric/core/abis/oracle.py` & `empiric_network-1.6.0/empiric/core/abis/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/abis/proxy.py` & `empiric_network-1.6.0/empiric/core/abis/proxy.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/abis/publisher_registry.py` & `empiric_network-1.6.0/empiric/core/abis/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/abis/randomness.py` & `empiric_network-1.6.0/empiric/core/abis/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/abis/summary_stats.py` & `empiric_network-1.6.0/empiric/core/abis/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/client.py` & `empiric_network-1.6.0/empiric/core/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     NonceMixin,
     OracleMixin,
     PublisherRegistryMixin,
     RandomnessMixin,
     TransactionMixin,
 )
 from starknet_py.net.account.account import Account
-from starknet_py.net.gateway_client import GatewayClient
 from starknet_py.net.signer.stark_curve_signer import KeyPair, StarkCurveSigner
 
 logger = logging.getLogger(__name__)
 
 class EmpiricClient(
     NonceMixin, OracleMixin, PublisherRegistryMixin, RandomnessMixin, TransactionMixin
 ):
@@ -37,21 +36,15 @@
         :param account_private_key: Optional private key for requests.  Not necessary if not making network updates
         :param account_contract_address: Optional account contract address.  Not necessary if not making network updates
         :param contract_addresses_config: Optional Contract Addresses for Empiric.  Will default to the provided network but must be set if using non standard contracts.
         """
         self.network_config = NETWORKS[network]
         self.network = network
 
-        if network not in ["mainnet", "testnet"]:
-            if network in NETWORKS:
-                self.client = GatewayClient(self.network_config.gateway_url)
-            else:
-                raise NotImplementedError(f"Network {network} not recognized")
-        else:
-            self.client = GatewayClient(network)
+        self.client = get_client_from_network(network)
 
         if account_contract_address and account_private_key:
             self._setup_account_client(
                 self.network_config.chain_id,
                 account_private_key,
                 account_contract_address,
             )
```

### Comparing `empiric_network-1.5.2/empiric/core/contract.py` & `empiric_network-1.6.0/empiric/core/contract.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/entry.py` & `empiric_network-1.6.0/empiric/core/entry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/mixins/evm.py` & `empiric_network-1.6.0/empiric/core/mixins/evm.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/mixins/nonce.py` & `empiric_network-1.6.0/empiric/core/mixins/nonce.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/mixins/oracle.py` & `empiric_network-1.6.0/empiric/core/mixins/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/mixins/publisher_registry.py` & `empiric_network-1.6.0/empiric/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/mixins/randomness.py` & `empiric_network-1.6.0/empiric/core/mixins/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/mixins/transactions.py` & `empiric_network-1.6.0/empiric/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/core/types.py` & `empiric_network-1.6.0/empiric/core/types.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 from enum import IntEnum, unique
 from typing import List, Literal
 
 from empiric.core.utils import str_to_felt
+from starknet_py.net.full_node_client import FullNodeClient
 
 ADDRESS = int
 HEX_STR = str
 
 # Network Types
 STAGING = "staging"
 TESTNET = "testnet"
 INTEGRATION = "integration"
 MAINNET = "mainnet"
 SCROLL_TESTNET = "scroll_testnet"
 LINEA_TESTNET = "linea_testnet"
 ERA_TESTNET = "era_testnet"
+SHARINGAN = "sharingan"
 
-Network = Literal["staging", "testnet", "integration", "mainnet"]
+Network = Literal["staging", "testnet", "integration", "mainnet", "sharingan"]
 
 CHAIN_IDS = {
     INTEGRATION: 1536727068981429685321,
+    SHARINGAN: 1536727068981429685321,
     TESTNET: 1536727068981429685321,
     MAINNET: 23448594291968334,
     SCROLL_TESTNET: 534353,
     LINEA_TESTNET: 59140,
     ERA_TESTNET: 280
 }
 
-GATEWAY_URLS = {
-    TESTNET: "https://alpha4.starknet.io",
-    INTEGRATION: "https://external.integration.starknet.io",
-    MAINNET: "https://alpha-mainnet.starknet.io",
-    SCROLL_TESTNET: "https://scroll-alphanet.public.blastapi.io",
-    LINEA_TESTNET: "https://consensys-zkevm-goerli-prealpha.infura.io/v3/ef9b71db32e242f39c6cf0691c8b521a",
-    ERA_TESTNET: "https://testnet.era.zksync.dev"
+STARKSCAN_URLS = {
+    "mainnet": "https://starkscan.co",
+    "testnet": "https://testnet.starkscan.co",
+    "testnet2": "https://testnet-2.starkscan.co",
+    "devnet": "https://devnet.starkscan.co",
+    "sharingan": "https://starknet-madara.netlify.app/#/explorer/query",
 }
 
+if not os.getenv("RPC_KEY") and NETWORK in ["mainnet", "testnet", "testnet2"]:
+    raise ValueError(f"RPC_KEY env variable is required when targeting {NETWORK}")
+RPC_URLS = {
+    "mainnet": f"https://starknet-mainnet.infura.io/v3/{os.getenv('RPC_KEY')}",
+    "testnet": f"https://starknet-goerli.infura.io/v3/{os.getenv('RPC_KEY')}",
+    "testnet2": f"https://starknet-goerli2.infura.io/v3/{os.getenv('RPC_KEY')}",
+    "devnet": "http://127.0.0.1:5050/rpc",
+    "sharingan": os.getenv("SHARINGAN_RPC_URL"),
+}
+RPC_CLIENT = FullNodeClient(node_url=RPC_URLS[NETWORK])
+
 
 # aggregation mode enum
 @unique
 class AggregationMode(IntEnum):
     MEDIAN = 84959893733710  # str_to_felt("MEDIAN")
```

### Comparing `empiric_network-1.5.2/empiric/core/utils.py` & `empiric_network-1.6.0/empiric/core/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/assets.py` & `empiric_network-1.6.0/empiric/publisher/assets.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/client.py` & `empiric_network-1.6.0/empiric/publisher/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/fetchers/ascendex.py` & `empiric_network-1.6.0/empiric/publisher/fetchers/ascendex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/fetchers/bitstamp.py` & `empiric_network-1.6.0/empiric/publisher/fetchers/bitstamp.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/fetchers/cex.py` & `empiric_network-1.6.0/empiric/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/fetchers/coinbase.py` & `empiric_network-1.6.0/empiric/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/fetchers/coingecko.py` & `empiric_network-1.6.0/empiric/publisher/fetchers/coingecko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/fetchers/defillama.py` & `empiric_network-1.6.0/empiric/publisher/fetchers/defillama.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/fetchers/gemini.py` & `empiric_network-1.6.0/empiric/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/fetchers/kaiko.py` & `empiric_network-1.6.0/empiric/publisher/fetchers/kaiko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/fetchers/okx.py` & `empiric_network-1.6.0/empiric/publisher/fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/fetchers/thegraph.py` & `empiric_network-1.6.0/empiric/publisher/fetchers/thegraph.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/publisher/types.py` & `empiric_network-1.6.0/empiric/publisher/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/empiric/test/interface_consistency.py` & `empiric_network-1.6.0/empiric/test/interface_consistency.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.5.2/PKG-INFO` & `empiric_network-1.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: empiric-network
-Version: 1.5.2
+Version: 1.6.0
 Summary: Core package for rollup-native Pragma Oracle
 Home-page: https://pragmaoracle.com
 Author: Pragma
 Author-email: contact@pragmaoracle.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: cairo-lang (==0.10.3)
-Requires-Dist: starknet.py (==0.14.0a0)
+Requires-Dist: cairo-lang (>=0.11,<0.12)
+Requires-Dist: starknet.py (>=0.16,<0.17)
 Requires-Dist: typer (==0.6.1)
 Project-URL: Documentation, https://docs.pragmaoracle.com
 Project-URL: Repository, https://github.com/Astraly-Labs/Pragma
 Description-Content-Type: text/markdown
 
 # Empiric Network
```

