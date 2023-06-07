# Comparing `tmp/cert-issuer-3.4.0.tar.gz` & `tmp/cert-issuer-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cert-issuer-3.4.0.tar", last modified: Fri May 26 13:35:07 2023, max compression
+gzip compressed data, was "cert-issuer-3.5.0.tar", last modified: Wed Jun  7 14:32:42 2023, max compression
```

## Comparing `cert-issuer-3.4.0.tar` & `cert-issuer-3.5.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      934 2023-05-26 13:35:05.000000 cert-issuer-3.4.0/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1096 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    19777 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    19438 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/bitcoin_requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.935884 cert-issuer-3.4.0/cert_issuer/
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-05-26 13:35:05.000000 cert-issuer-3.4.0/cert_issuer/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      544 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/__main__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.935884 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.935884 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3595 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10248 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/connectors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3031 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/signer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4611 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/transaction_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4805 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/tx_utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3624 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13037 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/connectors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/signer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4233 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/transaction_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1210 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/tx_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5688 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/certificate_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/chained_proof_2021.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9143 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1079 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4841 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1590 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/issue_certificates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1352 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/issuer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2968 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/merkle_tree_generator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/cert_issuer/models/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3421 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2646 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/models/metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5857 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/models/verifiable_credential.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      793 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/normalization_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1961 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/proof_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2689 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/signer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/cert_issuer/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.935884 cert-issuer-3.4.0/cert_issuer.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19777 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1629 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      266 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2023-05-26 13:35:07.000000 cert-issuer-3.4.0/cert_issuer.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      309 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/conf_regtest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/ethereum_requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      134 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2138 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-26 13:35:07.939885 cert-issuer-3.4.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8798 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_certificate_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5773 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_connectors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3756 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_merkle_tree_generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11817 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_proof_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      363 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_signer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6054 2023-05-26 13:33:59.000000 cert-issuer-3.4.0/tests/test_tx_utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-07 14:32:41.999331 cert-issuer-3.5.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      645 2023-06-07 14:32:39.000000 cert-issuer-3.5.0/CHANGELOG.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1096 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19749 2023-06-07 14:32:41.999331 cert-issuer-3.5.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19410 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       25 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/bitcoin_requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-07 14:32:41.991330 cert-issuer-3.5.0/cert_issuer/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-06-07 14:32:39.000000 cert-issuer-3.5.0/cert_issuer/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      544 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/__main__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-07 14:32:41.991330 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-07 14:32:41.995331 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/bitcoin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3615 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/bitcoin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10248 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/bitcoin/connectors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3031 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/bitcoin/signer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4611 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/bitcoin/transaction_handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4805 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/bitcoin/tx_utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-07 14:32:41.995331 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/ethereum/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3624 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/ethereum/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13037 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/ethereum/connectors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/ethereum/signer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4233 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/ethereum/transaction_handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1210 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/blockchain_handlers/ethereum/tx_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5870 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/certificate_handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/chained_proof_2021.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10030 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1079 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4841 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1590 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/issue_certificates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1352 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/issuer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2968 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/merkle_tree_generator.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-07 14:32:41.995331 cert-issuer-3.5.0/cert_issuer/models/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3421 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/models/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2646 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/models/metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5857 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/models/verifiable_credential.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      793 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/normalization_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2421 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/proof_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2689 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/signer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/cert_issuer/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-07 14:32:41.991330 cert-issuer-3.5.0/cert_issuer.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19749 2023-06-07 14:32:41.000000 cert-issuer-3.5.0/cert_issuer.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1629 2023-06-07 14:32:41.000000 cert-issuer-3.5.0/cert_issuer.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-07 14:32:41.000000 cert-issuer-3.5.0/cert_issuer.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2023-06-07 14:32:41.000000 cert-issuer-3.5.0/cert_issuer.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      266 2023-06-07 14:32:41.000000 cert-issuer-3.5.0/cert_issuer.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       18 2023-06-07 14:32:41.000000 cert-issuer-3.5.0/cert_issuer.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      309 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/conf_regtest.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)       25 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/ethereum_requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      134 2023-06-07 14:32:41.999331 cert-issuer-3.5.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2138 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-07 14:32:41.999331 cert-issuer-3.5.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8802 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/tests/test_certificate_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5773 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/tests/test_connectors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3756 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/tests/test_merkle_tree_generator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13459 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/tests/test_proof_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      363 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/tests/test_signer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6054 2023-06-07 14:31:33.000000 cert-issuer-3.5.0/tests/test_tx_utils.py
```

### Comparing `cert-issuer-3.4.0/LICENSE` & `cert-issuer-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/PKG-INFO` & `cert-issuer-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cert-issuer
-Version: 3.4.0
+Version: 3.5.0
 Summary: Issues blockchain certificates using the Bitcoin blockchain
 Home-page: https://github.com/blockchain-certificates/cert-issuer
 Author: Blockcerts
 Author-email: info@blockcerts.org
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Verifiable Credential Compliance result](https://badgen.net/badge/Verifiable%20Credentials%20v1/compliant/green?icon=https://www.w3.org/Icons/WWW/w3c_home_nb-v.svg)](https://github.com/blockchain-certificates/cert-issuer/vc-compliance-report.html)
+[![Verifiable Credential Compliance result](https://badgen.net/badge/Verifiable%20Credentials%20v1/compliant/green?icon=https://www.w3.org/Icons/WWW/w3c_home_nb-v.svg)](https://www.blockcerts.org/vc-compliance-report.html)
 [![Build Status](https://travis-ci.org/blockchain-certificates/cert-issuer.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-issuer)
 [![PyPI version](https://badge.fury.io/py/cert-issuer.svg)](https://badge.fury.io/py/cert-issuer)
 
 # cert-issuer
 
 The cert-issuer project issues blockchain certificates by creating a transaction from the issuing institution to the
 recipient on the Bitcoin or Ethereum blockchains. That transaction includes the hash of the certificate itself.
```

### Comparing `cert-issuer-3.4.0/README.md` & `cert-issuer-3.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Verifiable Credential Compliance result](https://badgen.net/badge/Verifiable%20Credentials%20v1/compliant/green?icon=https://www.w3.org/Icons/WWW/w3c_home_nb-v.svg)](https://github.com/blockchain-certificates/cert-issuer/vc-compliance-report.html)
+[![Verifiable Credential Compliance result](https://badgen.net/badge/Verifiable%20Credentials%20v1/compliant/green?icon=https://www.w3.org/Icons/WWW/w3c_home_nb-v.svg)](https://www.blockcerts.org/vc-compliance-report.html)
 [![Build Status](https://travis-ci.org/blockchain-certificates/cert-issuer.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-issuer)
 [![PyPI version](https://badge.fury.io/py/cert-issuer.svg)](https://badge.fury.io/py/cert-issuer)
 
 # cert-issuer
 
 The cert-issuer project issues blockchain certificates by creating a transaction from the issuing institution to the
 recipient on the Bitcoin or Ethereum blockchains. That transaction includes the hash of the certificate itself.
```

### Comparing `cert-issuer-3.4.0/cert_issuer/__main__.py` & `cert-issuer-3.5.0/cert_issuer/__main__.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/__init__.py` & `cert-issuer-3.5.0/cert_issuer/blockchain_handlers/bitcoin/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,20 +45,20 @@
 def instantiate_blockchain_handlers(app_config, file_mode=True):
     issuing_address = app_config.issuing_address
     chain = app_config.chain
     secret_manager = initialize_signer(app_config)
 
     if file_mode:
         certificate_batch_handler = CertificateBatchHandler(secret_manager=secret_manager,
-                                                            certificate_handler=CertificateV3Handler(),
+                                                            certificate_handler=CertificateV3Handler(app_config),
                                                             merkle_tree=MerkleTreeGenerator(),
                                                             config=app_config)
     else:
         certificate_batch_handler = CertificateBatchWebHandler(secret_manager=secret_manager,
-                                                               certificate_handler=CertificateWebV3Handler(),
+                                                               certificate_handler=CertificateWebV3Handler(app_config),
                                                                merkle_tree=MerkleTreeGenerator(),
                                                                config=app_config)
     if chain.is_mock_type():
         transaction_handler = MockTransactionHandler()
         connector = MockServiceProviderConnector()
     else:
         cost_constants = BitcoinTransactionCostConstants(app_config.tx_fee, app_config.dust_threshold,
```

### Comparing `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/connectors.py` & `cert-issuer-3.5.0/cert_issuer/blockchain_handlers/bitcoin/connectors.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/signer.py` & `cert-issuer-3.5.0/cert_issuer/blockchain_handlers/bitcoin/signer.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/transaction_handlers.py` & `cert-issuer-3.5.0/cert_issuer/blockchain_handlers/bitcoin/transaction_handlers.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/bitcoin/tx_utils.py` & `cert-issuer-3.5.0/cert_issuer/blockchain_handlers/bitcoin/tx_utils.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/__init__.py` & `cert-issuer-3.5.0/cert_issuer/blockchain_handlers/ethereum/__init__.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/connectors.py` & `cert-issuer-3.5.0/cert_issuer/blockchain_handlers/ethereum/connectors.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/signer.py` & `cert-issuer-3.5.0/cert_issuer/blockchain_handlers/ethereum/signer.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/transaction_handlers.py` & `cert-issuer-3.5.0/cert_issuer/blockchain_handlers/ethereum/transaction_handlers.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/blockchain_handlers/ethereum/tx_utils.py` & `cert-issuer-3.5.0/cert_issuer/blockchain_handlers/ethereum/tx_utils.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/certificate_handlers.py` & `cert-issuer-3.5.0/cert_issuer/certificate_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,41 +7,47 @@
 from cert_issuer.normalization_handler import JSONLDHandler
 from cert_issuer.models import CertificateHandler, BatchHandler
 
 from cert_issuer.signer import FinalizableSigner
 
 
 class CertificateV3Handler(CertificateHandler):
+    def __init__(self, app_config):
+        self.app_config = app_config
+
     def get_byte_array_to_issue(self, certificate_metadata):
         certificate_json = self._get_certificate_to_issue(certificate_metadata)
         return JSONLDHandler.normalize_to_utf8(certificate_json)
 
     def add_proof(self, certificate_metadata, merkle_proof):
         """
         :param certificate_metadata:
         :param merkle_proof:
         :return:
         """
         certificate_json = self._get_certificate_to_issue(certificate_metadata)
-        certificate_json = ProofHandler().add_proof(certificate_json, merkle_proof)
+        certificate_json = ProofHandler().add_proof(certificate_json, merkle_proof, self.app_config)
 
         with open(certificate_metadata.blockchain_cert_file_name, 'w') as out_file:
             out_file.write(json.dumps(certificate_json))
 
     def _get_certificate_to_issue(self, certificate_metadata):
         with open(certificate_metadata.unsigned_cert_file_name, 'r') as unsigned_cert_file:
             certificate_json = json.load(unsigned_cert_file)
         return certificate_json
 
 class CertificateWebV3Handler(CertificateHandler):
+    def __init__(self, app_config):
+        self.app_config = app_config
+
     def get_byte_array_to_issue(self, certificate_json):
         return JSONLDHandler.normalize_to_utf8(certificate_json)
 
     def add_proof(self, certificate_json, merkle_proof):
-        certificate_json = ProofHandler().add_proof(certificate_json, merkle_proof)
+        certificate_json = ProofHandler().add_proof(certificate_json, merkle_proof, self.app_config)
         return certificate_json
 
 class CertificateBatchWebHandler(BatchHandler):
     def finish_batch(self, tx_id, chain):
         self.proof = []
         proof_generator = self.merkle_tree.get_proof_generator(tx_id, self.config.verification_method, chain)
         for metadata in self.certificates_to_issue:
```

### Comparing `cert-issuer-3.4.0/cert_issuer/chained_proof_2021.py` & `cert-issuer-3.5.0/cert_issuer/chained_proof_2021.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/config.py` & `cert-issuer-3.5.0/cert_issuer/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,26 @@
                    help='When trying to sign a document with an unsupported context, ' +
                         'provide the url and the path to the local context file. ' +
                         'Space separated list, must be used in conjunction with the `--context_urls` property. ' +
                         'Path should be relative to CWD, order should match `--context_urls` order.',
                    env_var='CONTEXT_FILE_PATHS',
                    nargs='+'
                    )
+    p.add_argument('--multiple_proofs',
+                   default='chained',
+                   type=str,
+                   choices=['chained', 'concurrent'],
+                   help='How to handle a document that was previously signed by another party. \n' +
+                        'If the document has not been signed yet, a single proof will be added. \n' +
+                        '"chained": Chained proof also sign the previous proof(s) of the document, making them ' +
+                        'untemperable with in the final document, ie: a notary signs over the signatures of the buyer ' +
+                        'and the seller in a real estate transaction. \n' +
+                        '"concurrent": Concurrent proofs mean the parties independently sign the document without ' +
+                        'the other parties\' signatures. Defaults to chained proofs.'
+    )
 
 
 def get_config():
     configure_logger()
     p = configargparse.getArgumentParser(default_config_files=[os.path.join(PATH, 'conf.ini'),
                                                                '/etc/cert-issuer/conf.ini'])
     add_arguments(p)
```

### Comparing `cert-issuer-3.4.0/cert_issuer/errors.py` & `cert-issuer-3.5.0/cert_issuer/errors.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/helpers.py` & `cert-issuer-3.5.0/cert_issuer/helpers.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/issue_certificates.py` & `cert-issuer-3.5.0/cert_issuer/issue_certificates.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/issuer.py` & `cert-issuer-3.5.0/cert_issuer/issuer.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/merkle_tree_generator.py` & `cert-issuer-3.5.0/cert_issuer/merkle_tree_generator.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/models/__init__.py` & `cert-issuer-3.5.0/cert_issuer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/models/metadata.py` & `cert-issuer-3.5.0/cert_issuer/models/metadata.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/models/verifiable_credential.py` & `cert-issuer-3.5.0/cert_issuer/models/verifiable_credential.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/normalization_handler.py` & `cert-issuer-3.5.0/cert_issuer/normalization_handler.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer/proof_handler.py` & `cert-issuer-3.5.0/cert_issuer/proof_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,28 +2,39 @@
 from cert_schema import ContextUrls
 from cert_issuer.utils import array_intersect
 
 class ProofHandler:
     def __init__(self):
         self.contextUrls = ContextUrls()
 
-    def add_proof(self, certificate_json, merkle_proof):
+    def add_proof(self, certificate_json, merkle_proof, app_config=None):
         if 'proof' in certificate_json:
             if not isinstance(certificate_json['proof'], list):
                 # convert proof to list
                 initial_proof = certificate_json['proof']
                 certificate_json['proof'] = [initial_proof]
-            previous_proof = certificate_json['proof'][-1]
-            certificate_json['proof'].append(ChainedProof2021(previous_proof, merkle_proof).to_json_object())
-            self.update_context_for_chained_proof(certificate_json)
+            if self.is_multiple_proof_config_chained(app_config):
+                self.add_chained_proof(certificate_json, merkle_proof)
+            else:
+                certificate_json['proof'].append(merkle_proof)
         else:
             certificate_json['proof'] = merkle_proof
             self.update_context_for_single_proof(certificate_json)
         return certificate_json
 
+    def is_multiple_proof_config_chained(self, app_config):
+        if app_config is None:
+            return True
+        return app_config.multiple_proofs == 'chained'
+
+    def add_chained_proof(self, certificate_json, merkle_proof):
+        previous_proof = certificate_json['proof'][-1]
+        certificate_json['proof'].append(ChainedProof2021(previous_proof, merkle_proof).to_json_object())
+        self.update_context_for_chained_proof(certificate_json)
+
     def update_context_for_chained_proof(self, certificate_json):
         context = certificate_json['@context']
         if self.contextUrls.merkle_proof_2019() not in context:
             context.append(self.contextUrls.merkle_proof_2019())
 
         if self.contextUrls.chained_proof_2021() not in context:
             context.append(self.contextUrls.chained_proof_2021())
```

### Comparing `cert-issuer-3.4.0/cert_issuer/signer.py` & `cert-issuer-3.5.0/cert_issuer/signer.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/cert_issuer.egg-info/PKG-INFO` & `cert-issuer-3.5.0/cert_issuer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cert-issuer
-Version: 3.4.0
+Version: 3.5.0
 Summary: Issues blockchain certificates using the Bitcoin blockchain
 Home-page: https://github.com/blockchain-certificates/cert-issuer
 Author: Blockcerts
 Author-email: info@blockcerts.org
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Verifiable Credential Compliance result](https://badgen.net/badge/Verifiable%20Credentials%20v1/compliant/green?icon=https://www.w3.org/Icons/WWW/w3c_home_nb-v.svg)](https://github.com/blockchain-certificates/cert-issuer/vc-compliance-report.html)
+[![Verifiable Credential Compliance result](https://badgen.net/badge/Verifiable%20Credentials%20v1/compliant/green?icon=https://www.w3.org/Icons/WWW/w3c_home_nb-v.svg)](https://www.blockcerts.org/vc-compliance-report.html)
 [![Build Status](https://travis-ci.org/blockchain-certificates/cert-issuer.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-issuer)
 [![PyPI version](https://badge.fury.io/py/cert-issuer.svg)](https://badge.fury.io/py/cert-issuer)
 
 # cert-issuer
 
 The cert-issuer project issues blockchain certificates by creating a transaction from the issuing institution to the
 recipient on the Bitcoin or Ethereum blockchains. That transaction includes the hash of the certificate itself.
```

### Comparing `cert-issuer-3.4.0/cert_issuer.egg-info/SOURCES.txt` & `cert-issuer-3.5.0/cert_issuer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/setup.py` & `cert-issuer-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/tests/test_certificate_handler.py` & `cert-issuer-3.5.0/tests/test_certificate_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         calls = mock_open.mock_calls
         print(calls)
         call_strings = map(str, calls)
         print(mock_open.return_value.__enter__().write.mock_calls)
         assert file_call in call_strings
 
     def test_web_add_proof(self):
-        handler = CertificateWebV3Handler()
+        handler = CertificateWebV3Handler(None)
         proof = {'a': 'merkel'}
         chain = mock.Mock()
         certificate_json = {
             '@context': [
                 'https://www.w3.org/2018/credentials/v1'
             ],
             'kek': 'kek'
```

### Comparing `cert-issuer-3.4.0/tests/test_connectors.py` & `cert-issuer-3.5.0/tests/test_connectors.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/tests/test_merkle_tree_generator.py` & `cert-issuer-3.5.0/tests/test_merkle_tree_generator.py`

 * *Files identical despite different names*

### Comparing `cert-issuer-3.4.0/tests/test_proof_handler.py` & `cert-issuer-3.5.0/tests/test_proof_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,46 @@
             'proofValue': 'zMcm4LfQFUZkWZyLJp1bqtXF8vkZZwp79x7Nvt5BmN2XV4usLLtDoeqiq3et923mcWfXde4a3m4f57yUZcATCbBXV1byb5AXbV8EzT6E8B9JKf3scvxxZCBVePtV4SrhYysAiLNJ9N2R8LgnpJ47wnQHkaTB1AMxrcLEHUTxm4zJTtQqf9orDLf3L4VoLzmST7ZzsDjuX9cw2hZ3Aazhhjy7swG44xfF1PC73SyCv77pDnJ6BSHm3azmbVG6BXv1EPtwF4J1YRqwojBEWk9nDgduACR7b9qNhQ46ND4B5vL8p3LkqTh',
             'proofPurpose': 'assertionMethod',
             'verificationMethod': 'did:ion:EiA_Z6LQILbB2zj_eVrqfQ2xDm4HNqeJUw5Kj2Z7bFOOeQ#key-1'
         }
         output = self.handler.add_proof(fixture_certificate_json, fixture_proof)
         self.assertIn(self.contextUrls.merkle_proof_2019(), output['@context'])
 
+    def test_multiple_non_chained_signature(self):
+        fixture_initial_proof = {
+          'type': 'Ed25519Signature2020',
+          'created': '2022-05-02T16:36:22.933Z',
+          'verificationMethod': 'did:key:z6MkjHnntGvtLjwfAMHWTAXXGJHhVL3DPtaT9BHmyTjWpjqs#z6MkjHnntGvtLjwfAMHWTAXXGJHhVL3DPtaT9BHmyTjWpjqs',
+          'proofPurpose': 'assertionMethod',
+          'proofValue': 'zAvFt59599JweBZ4zPP6Ge8LhKgECtBvDRmjG5VQbgEkPCiyMcM9QAPanJgSCs6RRGcKu96qNpfmpe9eTygpFZP6'
+        }
+        fixture_certificate_json = {
+            '@context': [
+                'https://www.w3.org/2018/credentials/v1',
+                'https://w3id.org/blockcerts/v3'
+            ],
+            'kek': 'kek',
+            'proof': fixture_initial_proof
+        }
+        fixture_proof = {
+            'type': 'MerkleProof2019',
+            'created': '2022-05-05T08:05:14.912828',
+            'proofValue': 'zMcm4LfQFUZkWZyLJp1bqtXF8vkZZwp79x7Nvt5BmN2XV4usLLtDoeqiq3et923mcWfXde4a3m4f57yUZcATCbBXV1byb5AXbV8EzT6E8B9JKf3scvxxZCBVePtV4SrhYysAiLNJ9N2R8LgnpJ47wnQHkaTB1AMxrcLEHUTxm4zJTtQqf9orDLf3L4VoLzmST7ZzsDjuX9cw2hZ3Aazhhjy7swG44xfF1PC73SyCv77pDnJ6BSHm3azmbVG6BXv1EPtwF4J1YRqwojBEWk9nDgduACR7b9qNhQ46ND4B5vL8p3LkqTh',
+            'proofPurpose': 'assertionMethod',
+            'verificationMethod': 'did:ion:EiA_Z6LQILbB2zj_eVrqfQ2xDm4HNqeJUw5Kj2Z7bFOOeQ#key-1'
+        }
+        class MockConfig:
+            multiple_proofs = 'concurrent'
+
+        output = self.handler.add_proof(fixture_certificate_json, fixture_proof, MockConfig())
+        self.assertEqual(output['proof'], [
+            fixture_initial_proof,
+            fixture_proof
+        ])
+
     def test_multiple_two_chained_signature(self):
         fixture_initial_proof = {
           'type': 'Ed25519Signature2020',
           'created': '2022-05-02T16:36:22.933Z',
           'verificationMethod': 'did:key:z6MkjHnntGvtLjwfAMHWTAXXGJHhVL3DPtaT9BHmyTjWpjqs#z6MkjHnntGvtLjwfAMHWTAXXGJHhVL3DPtaT9BHmyTjWpjqs',
           'proofPurpose': 'assertionMethod',
           'proofValue': 'zAvFt59599JweBZ4zPP6Ge8LhKgECtBvDRmjG5VQbgEkPCiyMcM9QAPanJgSCs6RRGcKu96qNpfmpe9eTygpFZP6'
```

### Comparing `cert-issuer-3.4.0/tests/test_tx_utils.py` & `cert-issuer-3.5.0/tests/test_tx_utils.py`

 * *Files identical despite different names*

