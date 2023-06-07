# Comparing `tmp/snekmate-0.0.1.tar.gz` & `tmp/snekmate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snekmate-0.0.1.tar", last modified: Mon Mar  6 10:29:29 2023, max compression
+gzip compressed data, was "snekmate-0.0.2.tar", last modified: Wed Jun  7 08:55:22 2023, max compression
```

## Comparing `snekmate-0.0.1.tar` & `snekmate-0.0.2.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:29:29.869383 snekmate-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-06 10:29:20.000000 snekmate-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-06 10:29:20.000000 snekmate-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-06 10:29:20.000000 snekmate-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-03-06 10:29:29.869383 snekmate-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-03-06 10:29:20.000000 snekmate-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-06 10:29:20.000000 snekmate-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 10:29:29.869383 snekmate-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:29:29.857383 snekmate-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:29:29.861383 snekmate-0.0.1/src/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/auth/AccessControl.vy
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/auth/Ownable.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/auth/Ownable2Step.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:29:29.861383 snekmate-0.0.1/src/auth/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/auth/interfaces/IAccessControl.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:29:29.861383 snekmate-0.0.1/src/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)    45128 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/extensions/ERC4626.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:29:29.861383 snekmate-0.0.1/src/snekmate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-03-06 10:29:29.000000 snekmate-0.0.1/src/snekmate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-06 10:29:29.000000 snekmate-0.0.1/src/snekmate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 10:29:29.000000 snekmate-0.0.1/src/snekmate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-06 10:29:29.000000 snekmate-0.0.1/src/snekmate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:29:29.865383 snekmate-0.0.1/src/tokens/
--rw-r--r--   0 runner    (1001) docker     (123)    39045 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/ERC1155.vy
--rw-r--r--   0 runner    (1001) docker     (123)    28430 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/ERC20.vy
--rw-r--r--   0 runner    (1001) docker     (123)    44256 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/ERC721.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:29:29.865383 snekmate-0.0.1/src/tokens/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/interfaces/IERC1155.vy
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/interfaces/IERC1155MetadataURI.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/interfaces/IERC1155Receiver.vy
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/interfaces/IERC20Permit.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/interfaces/IERC4906.vy
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/interfaces/IERC721Enumerable.vy
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/interfaces/IERC721Metadata.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/interfaces/IERC721Permit.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/tokens/interfaces/IERC721Receiver.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 10:29:29.869383 snekmate-0.0.1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/utils/Base64.vy
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/utils/BatchDistributor.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/utils/Create2Address.vy
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/utils/CreateAddress.vy
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/utils/ECDSA.vy
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/utils/EIP712DomainSeparator.vy
--rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/utils/Math.vy
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/utils/MerkleProofVerification.vy
--rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/utils/Multicall.vy
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-03-06 10:29:20.000000 snekmate-0.0.1/src/utils/SignatureChecker.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:55:22.885503 snekmate-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-06-07 08:55:08.000000 snekmate-0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-07 08:55:08.000000 snekmate-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-07 08:55:08.000000 snekmate-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-07 08:55:22.885503 snekmate-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-07 08:55:08.000000 snekmate-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-07 08:55:08.000000 snekmate-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 08:55:22.885503 snekmate-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:55:22.881503 snekmate-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:55:22.881503 snekmate-0.0.2/src/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/auth/AccessControl.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/auth/Ownable.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/auth/Ownable2Step.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:55:22.881503 snekmate-0.0.2/src/auth/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/auth/interfaces/IAccessControl.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:55:22.881503 snekmate-0.0.2/src/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)    46212 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/extensions/ERC4626.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:55:22.881503 snekmate-0.0.2/src/snekmate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-07 08:55:22.000000 snekmate-0.0.2/src/snekmate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-07 08:55:22.000000 snekmate-0.0.2/src/snekmate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:55:22.000000 snekmate-0.0.2/src/snekmate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 08:55:22.000000 snekmate-0.0.2/src/snekmate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:55:22.881503 snekmate-0.0.2/src/tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)    39364 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/ERC1155.vy
+-rw-r--r--   0 runner    (1001) docker     (123)    30098 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/ERC20.vy
+-rw-r--r--   0 runner    (1001) docker     (123)    46131 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/ERC721.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:55:22.885503 snekmate-0.0.2/src/tokens/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/interfaces/IERC1155.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/interfaces/IERC1155MetadataURI.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/interfaces/IERC1155Receiver.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/interfaces/IERC20Permit.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/interfaces/IERC4906.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/interfaces/IERC721Enumerable.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/interfaces/IERC721Metadata.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/interfaces/IERC721Permit.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/tokens/interfaces/IERC721Receiver.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:55:22.885503 snekmate-0.0.2/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/utils/Base64.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/utils/BatchDistributor.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/utils/Create2Address.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/utils/CreateAddress.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/utils/ECDSA.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/utils/EIP712DomainSeparator.vy
+-rw-r--r--   0 runner    (1001) docker     (123)    29213 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/utils/Math.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/utils/MerkleProofVerification.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/utils/Multicall.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/utils/SignatureChecker.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:55:22.885503 snekmate-0.0.2/src/utils/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-07 08:55:08.000000 snekmate-0.0.2/src/utils/interfaces/IERC5267.vy
```

### Comparing `snekmate-0.0.1/LICENSE` & `snekmate-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snekmate-0.0.1/PKG-INFO` & `snekmate-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: snekmate
-Version: 0.0.1
+Version: 0.0.2
 Summary: State-of-the-art, highly opinionated, hyper-optimised, and secure Vyper smart contract building blocks.
 Author-email: Pascal Marco Caversaccio <pascal.caversaccio@hotmail.ch>
 Maintainer-email: Pascal Marco Caversaccio <pascal.caversaccio@hotmail.ch>
 License: AGPL-3.0 License
 Project-URL: Homepage, https://github.com/pcaversaccio/snekmate#readme
 Project-URL: GitHub, https://github.com/pcaversaccio/snekmate
 Project-URL: Changelog, https://github.com/pcaversaccio/snekmate/blob/main/CHANGELOG.md
 Keywords: security,library,ethereum,smart-contracts,evm,vyper,vyper-contracts
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🐍 snekmate
 
 [![Test smart contracts](https://github.com/pcaversaccio/snekmate/actions/workflows/test-contracts.yml/badge.svg)](https://github.com/pcaversaccio/snekmate/actions/workflows/test-contracts.yml)
-[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
-[![npm package](https://img.shields.io/npm/v/snekmate.svg)](https://www.npmjs.com/package/snekmate)
+[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
+[![npm package](https://img.shields.io/npm/v/snekmate.svg?color=blue)](https://www.npmjs.com/package/snekmate)
 [![PyPI package](https://img.shields.io/pypi/v/snekmate?color=blue)](https://pypi.org/project/snekmate)
 
 **State-of-the-art**, **highly opinionated**, **hyper-optimised**, and **secure** 🐍Vyper smart contract building blocks.
 
 > This is **experimental software** and is provided on an "as is" and "as available" basis. We **do not give any warranties** and **will not be liable for any losses** incurred through any use of this code base.
 
 ## 📜 Contracts
```

### Comparing `snekmate-0.0.1/README.md` & `snekmate-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 🐍 snekmate
 
 [![Test smart contracts](https://github.com/pcaversaccio/snekmate/actions/workflows/test-contracts.yml/badge.svg)](https://github.com/pcaversaccio/snekmate/actions/workflows/test-contracts.yml)
-[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
-[![npm package](https://img.shields.io/npm/v/snekmate.svg)](https://www.npmjs.com/package/snekmate)
+[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
+[![npm package](https://img.shields.io/npm/v/snekmate.svg?color=blue)](https://www.npmjs.com/package/snekmate)
 [![PyPI package](https://img.shields.io/pypi/v/snekmate?color=blue)](https://pypi.org/project/snekmate)
 
 **State-of-the-art**, **highly opinionated**, **hyper-optimised**, and **secure** 🐍Vyper smart contract building blocks.
 
 > This is **experimental software** and is provided on an "as is" and "as available" basis. We **do not give any warranties** and **will not be liable for any losses** incurred through any use of this code base.
 
 ## 📜 Contracts
```

### Comparing `snekmate-0.0.1/pyproject.toml` & `snekmate-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "snekmate"
-version = "0.0.1"
+version = "0.0.2"
 description = "State-of-the-art, highly opinionated, hyper-optimised, and secure Vyper smart contract building blocks."
 readme = {file = "README.md", content-type = "text/markdown"}
-requires-python = ">=3.6"
+requires-python = ">=3.10"
 license = {text = "AGPL-3.0 License"}
 keywords = ["security", "library", "ethereum", "smart-contracts", "evm", "vyper", "vyper-contracts"]
 authors = [
   {name = "Pascal Marco Caversaccio", email = "pascal.caversaccio@hotmail.ch"},
 ]
 maintainers = [
   {name = "Pascal Marco Caversaccio", email = "pascal.caversaccio@hotmail.ch"},
```

### Comparing `snekmate-0.0.1/src/auth/AccessControl.vy` & `snekmate-0.0.2/src/auth/AccessControl.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Multi-Role-Based Access Control Functions
+@custom:contract-name AccessControl
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions can be used to implement role-based access
         control mechanisms. Roles are referred to by their `bytes32`
         identifier. These should be exposed in the external API and
         be unique. The best way to achieve this is by using `public
         constant` hash digests:
         ```vy
         MY_ROLE: public(constant(bytes32)) = keccak256("MY_ROLE");
         ```
 
         Roles can be used to represent a set of permissions. To restrict
         access to a function call, use the `external` function `hasRole`
-        or the `internal` function `_check_role`:
+        or the `internal` function `_check_role` (to avoid any NatSpec
+        parsing error, no `@` character is added to the visibility decorator
+        `@external` in the following examples; please add them accordingly):
         ```vy
-        @external
+        external
         def foo():
             assert self.hasRole[MY_ROLE][msg.sender], "AccessControl: account is missing role"
             ...
 
         OR
 
-        @external
+        external
         def foo():
             self._check_role(MY_ROLE, msg.sender)
             ...
         ```
 
         Roles can be granted and revoked dynamically via the `grantRole`
         and `revokeRole` functions. Each role has an associated admin role,
```

### Comparing `snekmate-0.0.1/src/auth/Ownable.vy` & `snekmate-0.0.2/src/auth/Ownable.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Owner-Based Access Control Functions
+@custom:contract-name Ownable
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions can be used to implement a basic access
         control mechanism, where there is an account (an owner)
         that can be granted exclusive access to specific functions.
         By default, the owner account will be the one that deploys
         the contract. This can later be changed with `transfer_ownership`.
```

### Comparing `snekmate-0.0.1/src/auth/Ownable2Step.vy` & `snekmate-0.0.2/src/auth/Ownable2Step.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title 2-Step Ownership Transfer Functions
+@custom:contract-name Ownable2Step
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions can be used to implement a basic access
         control mechanism, where there is an account (an owner)
         that can be granted exclusive access to specific functions.
         By default, the owner account will be the one that deploys
         the contract. This can later be changed with `transfer_ownership`
```

### Comparing `snekmate-0.0.1/src/auth/interfaces/IAccessControl.vy` & `snekmate-0.0.2/src/auth/interfaces/IAccessControl.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title AccessControl Interface Definition
+@custom:contract-name IAccessControl
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice The interface definition of `AccessControl`
         to support the ERC-165 detection. In order
         to ensure consistency and interoperability,
         we follow OpenZeppelin's definition here:
         https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/access/IAccessControl.sol.
```

### Comparing `snekmate-0.0.1/src/extensions/ERC4626.vy` & `snekmate-0.0.2/src/extensions/ERC4626.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Modern and Gas-Efficient ERC-4626 Tokenised Vault Implementation
+@custom:contract-name ERC4626
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions implement the ERC-4626
         standard interface:
         - https://eips.ethereum.org/EIPS/eip-4626.
         In addition, the following functions have
         been added for convenience:
         - `permit` (`external` function),
         - `nonces` (`external` `view` function),
-        - `DOMAIN_SEPARATOR` (`external` `view` function).
+        - `DOMAIN_SEPARATOR` (`external` `view` function),
+        - `eip712Domain` (`external` `view` function).
         The `permit` function implements approvals via
         EIP-712 secp256k1 signatures:
         https://eips.ethereum.org/EIPS/eip-2612.
+        In addition, this contract also implements the EIP-5267
+        function `eip712Domain`:
+        https://eips.ethereum.org/EIPS/eip-5267.
         The implementation is inspired by OpenZeppelin's
         implementation here:
         https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/extensions/ERC4626.sol,
         as well as by fubuloubu's implementation here:
         https://github.com/fubuloubu/ERC4626/blob/main/contracts/VyperVault.vy.
 @custom:security Most of the following security analysis was sourced from OpenZeppelin's
                  implementation: This implementation uses virtual assets and shares to
@@ -46,47 +51,51 @@
                  shares and assets will cause the first user to exit to experience reduced losses
                  in detriment to the last users that will experience bigger losses.
 """
 
 
 # @dev We import and implement the `ERC20` interface,
 # which is a built-in interface of the Vyper compiler.
-# @notice We do not import and implement the interface
-# `ERC20Detailed` (https://github.com/vyperlang/vyper/blob/master/vyper/builtins/interfaces/ERC20Detailed.py)
-# to be able to declare `name`, `symbol`, and `decimals`
-# as `immutable` variables. This is a known compiler bug
-# (https://github.com/vyperlang/vyper/issues/3130) and
-# we will import and implement the interface `ERC20Detailed`
-# once it is fixed.
 from vyper.interfaces import ERC20
 implements: ERC20
 
 
+# @dev We import and implement the `ERC20Detailed` interface,
+# which is a built-in interface of the Vyper compiler.
+from vyper.interfaces import ERC20Detailed
+implements: ERC20Detailed
+
+
 # @dev We import and implement the `IERC20Permit`
 # interface, which is written using standard Vyper
 # syntax.
-import src.tokens.interfaces.IERC20Permit as IERC20Permit
+from ..tokens.interfaces.IERC20Permit import IERC20Permit
 implements: IERC20Permit
 
 
-# @dev We import the `ERC4626` interface, which is a
-# built-in interface of the Vyper compiler.
-# @notice We do not implement the interface `ERC4626`
-# (https://github.com/vyperlang/vyper/blob/master/vyper/builtins/interfaces/ERC4626.py)
-# to be able to declare `asset` as an `immutable` variable.
-# This is a known compiler bug (https://github.com/vyperlang/vyper/issues/3130)
-# and we will implement the interface `ERC4626` once it
-# is fixed.
+# @dev We import and implement the `ERC4626` interface,
+# which is a built-in interface of the Vyper compiler.
 from vyper.interfaces import ERC4626
+implements: ERC4626
+
+
+# @dev We import and implement the `IERC5267` interface,
+# which is written using standard Vyper syntax.
+from ..utils.interfaces.IERC5267 import IERC5267
+implements: IERC5267
 
 
 # @dev Constant used as part of the ECDSA recovery function.
 _MALLEABILITY_THRESHOLD: constant(bytes32) = 0x7FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF5D576E7357A4501DDFE92F46681B20A0
 
 
+# @dev The 32-byte type hash for the EIP-712 domain separator.
+_TYPE_HASH: constant(bytes32) = keccak256("EIP712Domain(string name,string version,uint256 chainId,address verifyingContract)")
+
+
 # @dev The 32-byte type hash of the `permit` function.
 _PERMIT_TYPE_HASH: constant(bytes32) = keccak256("Permit(address owner,address spender,uint256 value,uint256 nonce,uint256 deadline)")
 
 
 # @dev Returns the name of the token.
 # @notice If you declare a variable as `public`,
 # Vyper automatically generates an `external`
@@ -118,27 +127,33 @@
 # the `immutable` variable `name`.
 # @notice Vyper returns the `address` type for interface
 # types by default.
 asset: public(immutable(ERC20))
 
 
 # @dev Caches the domain separator as an `immutable`
-# value, but also stores the corresponding chain id
+# value, but also stores the corresponding chain ID
 # to invalidate the cached domain separator if the
-# chain id changes.
+# chain ID changes.
+_CACHED_DOMAIN_SEPARATOR: immutable(bytes32)
 _CACHED_CHAIN_ID: immutable(uint256)
+
+
+# @dev Caches `self` to `immutable` storage to avoid
+# potential issues if a vanilla contract is used in
+# a `delegatecall` context.
 _CACHED_SELF: immutable(address)
-_CACHED_DOMAIN_SEPARATOR: immutable(bytes32)
 
 
-# @dev `immutable` variables to store the name,
-# version, and type hash during contract creation.
+# @dev `immutable` variables to store the (hashed)
+# name and (hashed) version during contract creation.
+_NAME: immutable(String[50])
 _HASHED_NAME: immutable(bytes32)
+_VERSION: immutable(String[20])
 _HASHED_VERSION: immutable(bytes32)
-_TYPE_HASH: immutable(bytes32)
 
 
 # @dev An offset in the decimal representation between
 # the underlying asset's decimals and the vault decimals.
 # @notice While not fully preventing the attack, analysis
 # (https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/docs/modules/ROOT/pages/erc4626.adoc#security-concern-inflation-attack)
 # shows that a standard offset of `0` makes an inflation
@@ -207,14 +222,20 @@
     sender: indexed(address)
     receiver: indexed(address)
     owner: indexed(address)
     assets: uint256
     shares: uint256
 
 
+# @dev May be emitted to signal that the domain could
+# have changed.
+event EIP712DomainChanged:
+    pass
+
+
 @external
 @payable
 def __init__(name_: String[25], symbol_: String[5], asset_: ERC20, decimals_offset_: uint8, name_eip712_: String[50], version_eip712_: String[20]):
     """
     @dev To omit the opcodes for checking the `msg.value`
          in the creation-time EVM bytecode, the constructor
          is declared as `payable`.
@@ -242,37 +263,27 @@
     success: bool = empty(bool)
     decoded_decimals: uint8 = empty(uint8)
     # Attempt to fetch the underlying's decimals. A return
     # value of `False` indicates that the attempt failed in
     # some way.
     success, decoded_decimals = self._try_get_underlying_decimals(asset_)
 
-    underlying_decimals: uint8 = empty(uint8)
-    # Due to a known compiler bug (https://github.com/vyperlang/vyper/issues/3278),
-    # we use a local variable for the first value assignment.
-    if (success):
-        underlying_decimals = decoded_decimals
-    else:
-        underlying_decimals = 18
-
-    _UNDERLYING_DECIMALS = underlying_decimals
+    _UNDERLYING_DECIMALS = decoded_decimals if success else 18
     _DECIMALS_OFFSET = decimals_offset_
     # The following line uses intentionally checked arithmetic
     # to prevent a theoretically possible overflow.
     decimals = _UNDERLYING_DECIMALS + _DECIMALS_OFFSET
 
-    hashed_name: bytes32 = keccak256(convert(name_eip712_, Bytes[50]))
-    hashed_version: bytes32 = keccak256(convert(version_eip712_, Bytes[20]))
-    type_hash: bytes32 = keccak256(convert("EIP712Domain(string name,string version,uint256 chainId,address verifyingContract)", Bytes[82]))
-    _HASHED_NAME = hashed_name
-    _HASHED_VERSION = hashed_version
-    _TYPE_HASH = type_hash
+    _NAME = name_eip712_
+    _VERSION = version_eip712_
+    _HASHED_NAME = keccak256(name_eip712_)
+    _HASHED_VERSION = keccak256(version_eip712_)
+    _CACHED_DOMAIN_SEPARATOR = self._build_domain_separator()
     _CACHED_CHAIN_ID = chain.id
     _CACHED_SELF = self
-    _CACHED_DOMAIN_SEPARATOR = self._build_domain_separator(type_hash, hashed_name, hashed_version)
 
 
 @external
 def transfer(to: address, amount: uint256) -> bool:
     """
     @dev Sourced from {ERC20-transfer}.
     @notice See {ERC20-transfer} for the function
@@ -359,14 +370,40 @@
             function docstring.
     """
     return self._domain_separator_v4()
 
 
 @external
 @view
+def eip712Domain() -> (bytes1, String[50], String[20], uint256, address, bytes32, DynArray[uint256, 128]):
+    """
+    @dev Returns the fields and values that describe the domain
+         separator used by this contract for EIP-712 signatures.
+    @notice The bits in the 1-byte bit map are read from the least
+            significant to the most significant, and fields are indexed
+            in the order that is specified by EIP-712, identical to the
+            order in which they are listed in the function type.
+    @return bytes1 The 1-byte bit map where bit `i` is set to 1
+            if and only if domain field `i` is present (`0 ≤ i ≤ 4`).
+    @return String The maximum 50-character user-readable string name
+            of the signing domain, i.e. the name of the dApp or protocol.
+    @return String The maximum 20-character current main version of
+            the signing domain. Signatures from different versions are
+            not compatible.
+    @return uint256 The 32-byte EIP-155 chain ID.
+    @return address The 20-byte address of the verifying contract.
+    @return bytes32 The 32-byte disambiguation salt for the protocol.
+    @return DynArray The 32-byte array of EIP-712 extensions.
+    """
+    # Note that `\x0f` equals `01111`.
+    return (convert(b"\x0f", bytes1), _NAME, _VERSION, chain.id, self, empty(bytes32), empty(DynArray[uint256, 128]))
+
+
+@external
+@view
 def totalAssets() -> uint256:
     """
     @dev Returns the total amount of the underlying asset
          that is managed by the vault.
     @notice For the to be fulfilled conditions, please refer to:
             https://eips.ethereum.org/EIPS/eip-4626#totalassets.
     @return uint256 The 32-byte total managed assets.
@@ -713,26 +750,26 @@
     @dev Sourced from {EIP712DomainSeparator-domain_separator_v4}.
     @notice See {EIP712DomainSeparator-domain_separator_v4}
             for the function docstring.
     """
     if (self == _CACHED_SELF and chain.id == _CACHED_CHAIN_ID):
         return _CACHED_DOMAIN_SEPARATOR
     else:
-        return self._build_domain_separator(_TYPE_HASH, _HASHED_NAME, _HASHED_VERSION)
+        return self._build_domain_separator()
 
 
 @internal
 @view
-def _build_domain_separator(type_hash: bytes32, name_hash: bytes32, version_hash: bytes32) -> bytes32:
+def _build_domain_separator() -> bytes32:
     """
     @dev Sourced from {EIP712DomainSeparator-_build_domain_separator}.
     @notice See {EIP712DomainSeparator-_build_domain_separator}
             for the function docstring.
     """
-    return keccak256(_abi_encode(type_hash, name_hash, version_hash, chain.id, self))
+    return keccak256(_abi_encode(_TYPE_HASH, _HASHED_NAME, _HASHED_VERSION, chain.id, self))
 
 
 @internal
 @view
 def _hash_typed_data_v4(struct_hash: bytes32) -> bytes32:
     """
     @dev Sourced from {EIP712DomainSeparator-hash_typed_data_v4}.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snekmate-0.0.1/src/snekmate.egg-info/PKG-INFO` & `snekmate-0.0.2/src/snekmate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: snekmate
-Version: 0.0.1
+Version: 0.0.2
 Summary: State-of-the-art, highly opinionated, hyper-optimised, and secure Vyper smart contract building blocks.
 Author-email: Pascal Marco Caversaccio <pascal.caversaccio@hotmail.ch>
 Maintainer-email: Pascal Marco Caversaccio <pascal.caversaccio@hotmail.ch>
 License: AGPL-3.0 License
 Project-URL: Homepage, https://github.com/pcaversaccio/snekmate#readme
 Project-URL: GitHub, https://github.com/pcaversaccio/snekmate
 Project-URL: Changelog, https://github.com/pcaversaccio/snekmate/blob/main/CHANGELOG.md
 Keywords: security,library,ethereum,smart-contracts,evm,vyper,vyper-contracts
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🐍 snekmate
 
 [![Test smart contracts](https://github.com/pcaversaccio/snekmate/actions/workflows/test-contracts.yml/badge.svg)](https://github.com/pcaversaccio/snekmate/actions/workflows/test-contracts.yml)
-[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
-[![npm package](https://img.shields.io/npm/v/snekmate.svg)](https://www.npmjs.com/package/snekmate)
+[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
+[![npm package](https://img.shields.io/npm/v/snekmate.svg?color=blue)](https://www.npmjs.com/package/snekmate)
 [![PyPI package](https://img.shields.io/pypi/v/snekmate?color=blue)](https://pypi.org/project/snekmate)
 
 **State-of-the-art**, **highly opinionated**, **hyper-optimised**, and **secure** 🐍Vyper smart contract building blocks.
 
 > This is **experimental software** and is provided on an "as is" and "as available" basis. We **do not give any warranties** and **will not be liable for any losses** incurred through any use of this code base.
 
 ## 📜 Contracts
```

### Comparing `snekmate-0.0.1/src/snekmate.egg-info/SOURCES.txt` & `snekmate-0.0.2/src/snekmate.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 src/utils/Create2Address.vy
 src/utils/CreateAddress.vy
 src/utils/ECDSA.vy
 src/utils/EIP712DomainSeparator.vy
 src/utils/Math.vy
 src/utils/MerkleProofVerification.vy
 src/utils/Multicall.vy
-src/utils/SignatureChecker.vy
+src/utils/SignatureChecker.vy
+src/utils/interfaces/IERC5267.vy
```

### Comparing `snekmate-0.0.1/src/tokens/ERC1155.vy` & `snekmate-0.0.2/src/tokens/ERC1155.vy`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Modern and Gas-Efficient ERC-1155 Implementation
+@custom:contract-name ERC1155
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @custom:coauthor jtriley.eth
 @notice These functions implement the ERC-1155
         standard interface:
         - https://eips.ethereum.org/EIPS/eip-1155.
         In addition, the following functions have
@@ -63,15 +64,15 @@
     0x01FFC9A7, # The ERC-165 identifier for ERC-165.
     0xD9B67A26, # The ERC-165 identifier for ERC-1155.
     0x0E89341C, # The ERC-165 identifier for the ERC-1155 metadata extension.
 ]
 
 
 # @dev Stores the upper bound for batch calls.
-_BATCH_SIZE: constant(uint16) = max_value(uint8)
+_BATCH_SIZE: constant(uint16) = 255
 
 
 # @dev Stores the base URI for computing `uri`.
 _BASE_URI: immutable(String[80])
 
 
 # @dev Mapping from owner to operator approvals.
@@ -298,15 +299,15 @@
 
 @external
 @view
 def uri(id: uint256) -> String[512]:
     """
     @dev Returns the Uniform Resource Identifier (URI)
          for token type `id`.
-    @notice If the `id` substring is present in the URI,
+    @notice If the `{id}` substring is present in the URI,
             it must be replaced by clients with the actual
             token type ID. Note that the `uri` function must
             not be used to check for the existence of a token
             as it is possible for the implementation to return
             a valid string even if the token does not exist.
     @param id The 32-byte identifier of the token type `id`.
     @return String The maximum 512-character user-readable
@@ -682,15 +683,15 @@
 
 @internal
 @view
 def _uri(id: uint256) -> String[512]:
     """
     @dev An `internal` helper function that returns the Uniform
          Resource Identifier (URI) for token type `id`.
-    @notice If the `id` substring is present in the URI,
+    @notice If the `{id}` substring is present in the URI,
             it must be replaced by clients with the actual
             token type ID. Note that the `uri` function must
             not be used to check for the existence of a token
             as it is possible for the implementation to return
             a valid string even if the token does not exist.
     @param id The 32-byte identifier of the token type `id`.
     @return String The maximum 512-character user-readable
@@ -707,14 +708,20 @@
     # and token URI.
     if (len(token_uri) != empty(uint256)):
         return concat(_BASE_URI, token_uri)
 
     # If there is no token URI but a base URI,
     # concatenate the base URI and token ID.
     if (base_uri_length != empty(uint256)):
+        # Please note that for projects where the
+        # substring `{id}` is present in the URI
+        # and this URI is to be set as `_BASE_URI`,
+        # it is recommended to remove the following
+        # concatenation and simply return `_BASE_URI`
+        # for easier off-chain handling.
         return concat(_BASE_URI, uint2str(id))
     else:
         return ""
 
 
 @internal
 def _set_uri(id: uint256, token_uri: String[432]):
```

### Comparing `snekmate-0.0.1/src/tokens/ERC20.vy` & `snekmate-0.0.2/src/tokens/ERC20.vy`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Modern and Gas-Efficient ERC-20 + EIP-2612 Implementation
+@custom:contract-name ERC20
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions implement the ERC-20
         standard interface:
         - https://eips.ethereum.org/EIPS/eip-20.
         In addition, the following functions have
         been added for convenience:
@@ -17,22 +18,26 @@
         - `burn_from` (`external` function),
         - `is_minter` (`external` `view` function),
         - `mint` (`external` function),
         - `set_minter` (`external` function),
         - `permit` (`external` function),
         - `nonces` (`external` `view` function),
         - `DOMAIN_SEPARATOR` (`external` `view` function),
+        - `eip712Domain` (`external` `view` function),
         - `owner` (`external` `view` function),
         - `transfer_ownership` (`external` function),
         - `renounce_ownership` (`external` function),
         - `_before_token_transfer` (`internal` function),
         - `_after_token_transfer` (`internal` function).
         The `permit` function implements approvals via
         EIP-712 secp256k1 signatures:
         https://eips.ethereum.org/EIPS/eip-2612.
+        In addition, this contract also implements the EIP-5267
+        function `eip712Domain`:
+        https://eips.ethereum.org/EIPS/eip-5267.
         The implementation is inspired by OpenZeppelin's
         implementation here:
         https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol,
         as well as by ApeAcademy's implementation here:
         https://github.com/ApeAcademy/ERC20/blob/main/%7B%7Bcookiecutter.project_name%7D%7D/contracts/Token.vy.
 @custom:security This ERC-20 implementation allows the commonly known
                  address poisoning attack, where `transferFrom` instructions
@@ -46,32 +51,37 @@
                  as well as in the OpenZeppelin repository:
                  https://github.com/OpenZeppelin/openzeppelin-contracts/issues/3931.
 """
 
 
 # @dev We import and implement the `ERC20` interface,
 # which is a built-in interface of the Vyper compiler.
-# @notice We do not import and implement the interface
-# `ERC20Detailed` (https://github.com/vyperlang/vyper/blob/master/vyper/builtins/interfaces/ERC20Detailed.py)
-# to be able to declare `name`, `symbol`, and `decimals`
-# as `immutable` and `constant` variables. This is a
-# known compiler bug (https://github.com/vyperlang/vyper/issues/3130)
-# and we will import and implement the interface `ERC20Detailed`
-# once it is fixed.
 from vyper.interfaces import ERC20
 implements: ERC20
 
 
+# @dev We import and implement the `ERC20Detailed` interface,
+# which is a built-in interface of the Vyper compiler.
+from vyper.interfaces import ERC20Detailed
+implements: ERC20Detailed
+
+
 # @dev We import and implement the `IERC20Permit`
 # interface, which is written using standard Vyper
 # syntax.
 import interfaces.IERC20Permit as IERC20Permit
 implements: IERC20Permit
 
 
+# @dev We import and implement the `IERC5267` interface,
+# which is written using standard Vyper syntax.
+from ..utils.interfaces.IERC5267 import IERC5267
+implements: IERC5267
+
+
 # @dev Returns the decimals places of the token.
 # The default value is 18.
 # @notice If you declare a variable as `public`,
 # Vyper automatically generates an `external`
 # getter function for the variable. Furthermore,
 # to preserve consistency with the interface for
 # the optional metadata functions of the ERC-20
@@ -81,14 +91,18 @@
 decimals: public(constant(uint8)) = 18
 
 
 # @dev Constant used as part of the ECDSA recovery function.
 _MALLEABILITY_THRESHOLD: constant(bytes32) = 0x7FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF5D576E7357A4501DDFE92F46681B20A0
 
 
+# @dev The 32-byte type hash for the EIP-712 domain separator.
+_TYPE_HASH: constant(bytes32) = keccak256("EIP712Domain(string name,string version,uint256 chainId,address verifyingContract)")
+
+
 # @dev The 32-byte type hash of the `permit` function.
 _PERMIT_TYPE_HASH: constant(bytes32) = keccak256("Permit(address owner,address spender,uint256 value,uint256 nonce,uint256 deadline)")
 
 
 # @dev Returns the name of the token.
 # @notice See comment on lower case letters
 # above at `decimals`.
@@ -98,27 +112,33 @@
 # @dev Returns the symbol of the token.
 # @notice See comment on lower case letters
 # above at `decimals`.
 symbol: public(immutable(String[5]))
 
 
 # @dev Caches the domain separator as an `immutable`
-# value, but also stores the corresponding chain id
+# value, but also stores the corresponding chain ID
 # to invalidate the cached domain separator if the
-# chain id changes.
+# chain ID changes.
+_CACHED_DOMAIN_SEPARATOR: immutable(bytes32)
 _CACHED_CHAIN_ID: immutable(uint256)
+
+
+# @dev Caches `self` to `immutable` storage to avoid
+# potential issues if a vanilla contract is used in
+# a `delegatecall` context.
 _CACHED_SELF: immutable(address)
-_CACHED_DOMAIN_SEPARATOR: immutable(bytes32)
 
 
-# @dev `immutable` variables to store the name,
-# version, and type hash during contract creation.
+# @dev `immutable` variables to store the (hashed)
+# name and (hashed) version during contract creation.
+_NAME: immutable(String[50])
 _HASHED_NAME: immutable(bytes32)
+_VERSION: immutable(String[20])
 _HASHED_VERSION: immutable(bytes32)
-_TYPE_HASH: immutable(bytes32)
 
 
 # @dev Returns the amount of tokens owned by an `address`.
 balanceOf: public(HashMap[address, uint256])
 
 
 # @dev Returns the remaining number of tokens that a
@@ -162,14 +182,20 @@
 # The parameter `amount` is the new allowance.
 event Approval:
     owner: indexed(address)
     spender: indexed(address)
     amount: uint256
 
 
+# @dev May be emitted to signal that the domain could
+# have changed.
+event EIP712DomainChanged:
+    pass
+
+
 # @dev Emitted when the ownership is transferred
 # from `previous_owner` to `new_owner`.
 event OwnershipTransferred:
     previous_owner: indexed(address)
     new_owner: indexed(address)
 
 
@@ -213,23 +239,21 @@
     if (initial_supply != empty(uint256)):
         self._before_token_transfer(empty(address), msg.sender, initial_supply)
         self.totalSupply = initial_supply
         self.balanceOf[msg.sender] = initial_supply
         log Transfer(empty(address), msg.sender, initial_supply)
         self._after_token_transfer(empty(address), msg.sender, initial_supply)
 
-    hashed_name: bytes32 = keccak256(convert(name_eip712_, Bytes[50]))
-    hashed_version: bytes32 = keccak256(convert(version_eip712_, Bytes[20]))
-    type_hash: bytes32 = keccak256(convert("EIP712Domain(string name,string version,uint256 chainId,address verifyingContract)", Bytes[82]))
-    _HASHED_NAME = hashed_name
-    _HASHED_VERSION = hashed_version
-    _TYPE_HASH = type_hash
+    _NAME = name_eip712_
+    _VERSION = version_eip712_
+    _HASHED_NAME = keccak256(name_eip712_)
+    _HASHED_VERSION = keccak256(version_eip712_)
+    _CACHED_DOMAIN_SEPARATOR = self._build_domain_separator()
     _CACHED_CHAIN_ID = chain.id
     _CACHED_SELF = self
-    _CACHED_DOMAIN_SEPARATOR = self._build_domain_separator(type_hash, hashed_name, hashed_version)
 
 
 @external
 def transfer(to: address, amount: uint256) -> bool:
     """
     @dev Moves `amount` tokens from the caller's
          account to `to`.
@@ -447,14 +471,40 @@
     @dev Returns the domain separator for the current chain.
     @return bytes32 The 32-byte domain separator.
     """
     return self._domain_separator_v4()
 
 
 @external
+@view
+def eip712Domain() -> (bytes1, String[50], String[20], uint256, address, bytes32, DynArray[uint256, 128]):
+    """
+    @dev Returns the fields and values that describe the domain
+         separator used by this contract for EIP-712 signatures.
+    @notice The bits in the 1-byte bit map are read from the least
+            significant to the most significant, and fields are indexed
+            in the order that is specified by EIP-712, identical to the
+            order in which they are listed in the function type.
+    @return bytes1 The 1-byte bit map where bit `i` is set to 1
+            if and only if domain field `i` is present (`0 ≤ i ≤ 4`).
+    @return String The maximum 50-character user-readable string name
+            of the signing domain, i.e. the name of the dApp or protocol.
+    @return String The maximum 20-character current main version of
+            the signing domain. Signatures from different versions are
+            not compatible.
+    @return uint256 The 32-byte EIP-155 chain ID.
+    @return address The 20-byte address of the verifying contract.
+    @return bytes32 The 32-byte disambiguation salt for the protocol.
+    @return DynArray The 32-byte array of EIP-712 extensions.
+    """
+    # Note that `\x0f` equals `01111`.
+    return (convert(b"\x0f", bytes1), _NAME, _VERSION, chain.id, self, empty(bytes32), empty(DynArray[uint256, 128]))
+
+
+@external
 def transfer_ownership(new_owner: address):
     """
     @dev Transfers the ownership of the contract
          to a new account `new_owner`.
     @notice Note that this function can only be
             called by the current `owner`. Also,
             the `new_owner` cannot be the zero address.
@@ -688,26 +738,26 @@
     @dev Sourced from {EIP712DomainSeparator-domain_separator_v4}.
     @notice See {EIP712DomainSeparator-domain_separator_v4}
             for the function docstring.
     """
     if (self == _CACHED_SELF and chain.id == _CACHED_CHAIN_ID):
         return _CACHED_DOMAIN_SEPARATOR
     else:
-        return self._build_domain_separator(_TYPE_HASH, _HASHED_NAME, _HASHED_VERSION)
+        return self._build_domain_separator()
 
 
 @internal
 @view
-def _build_domain_separator(type_hash: bytes32, name_hash: bytes32, version_hash: bytes32) -> bytes32:
+def _build_domain_separator() -> bytes32:
     """
     @dev Sourced from {EIP712DomainSeparator-_build_domain_separator}.
     @notice See {EIP712DomainSeparator-_build_domain_separator}
             for the function docstring.
     """
-    return keccak256(_abi_encode(type_hash, name_hash, version_hash, chain.id, self))
+    return keccak256(_abi_encode(_TYPE_HASH, _HASHED_NAME, _HASHED_VERSION, chain.id, self))
 
 
 @internal
 @view
 def _hash_typed_data_v4(struct_hash: bytes32) -> bytes32:
     """
     @dev Sourced from {EIP712DomainSeparator-hash_typed_data_v4}.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snekmate-0.0.1/src/tokens/ERC721.vy` & `snekmate-0.0.2/src/tokens/ERC721.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Modern and Gas-Efficient ERC-721 + EIP-4494 Implementation
+@custom:contract-name ERC721
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions implement the ERC-721
         standard interface:
         - https://eips.ethereum.org/EIPS/eip-721.
         In addition, the following functions have
         been added for convenience:
@@ -17,23 +18,30 @@
         - `burn` (`external` function),
         - `is_minter` (`external` `view` function),
         - `safe_mint` (`external` function),
         - `set_minter` (`external` function),
         - `permit` (`external` function),
         - `nonces` (`external` `view` function),
         - `DOMAIN_SEPARATOR` (`external` `view` function),
+        - `eip712Domain` (`external` `view` function),
         - `owner` (`external` `view` function),
         - `transfer_ownership` (`external` function),
         - `renounce_ownership` (`external` function),
         - `_check_on_erc721_received` (`internal` function),
         - `_before_token_transfer` (`internal` function),
         - `_after_token_transfer` (`internal` function).
         The `permit` function implements approvals via
         EIP-712 secp256k1 signatures for ERC-721 tokens:
         https://eips.ethereum.org/EIPS/eip-4494.
+        In addition, this contract also implements the EIP-5267
+        function `eip712Domain`:
+        https://eips.ethereum.org/EIPS/eip-5267.
+        Eventually, this contract also implements the EIP-4906
+        metadata update extension:
+        https://eips.ethereum.org/EIPS/eip-4906.
         The implementation is inspired by OpenZeppelin's
         implementation here:
         https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC721/ERC721.sol,
         as well as by ApeAcademy's implementation here:
         https://github.com/ApeAcademy/ERC721/blob/main/%7B%7Bcookiecutter.project_name%7D%7D/contracts/NFT.vy.
 """
 
@@ -42,25 +50,25 @@
 # which is a built-in interface of the Vyper compiler.
 from vyper.interfaces import ERC165
 implements: ERC165
 
 
 # @dev We import and implement the `ERC721` interface,
 # which is a built-in interface of the Vyper compiler.
-# @notice We do not import the interface `IERC721Metadata`
-# (https://github.com/pcaversaccio/snekmate/blob/main/src/tokens/interfaces/IERC721Metadata.vy)
-# to be able to declare `name` and `symbol` as
-# `immutable` variables. This is a known compiler
-# bug (https://github.com/vyperlang/vyper/issues/3130)
-# and we will import the interface `IERC721Metadata`
-# once it is fixed.
 from vyper.interfaces import ERC721
 implements: ERC721
 
 
+# @dev We import and implement the `IERC721Metadata`
+# interface, which is written using standard Vyper
+# syntax.
+import interfaces.IERC721Metadata as IERC721Metadata
+implements: IERC721Metadata
+
+
 # @dev We import and implement the `IERC721Enumerable`
 # interface, which is written using standard Vyper
 # syntax.
 import interfaces.IERC721Enumerable as IERC721Enumerable
 implements: IERC721Enumerable
 
 
@@ -73,14 +81,20 @@
 
 # @dev We import and implement the `IERC4906` interface,
 # which is written using standard Vyper syntax.
 import interfaces.IERC4906 as IERC4906
 implements: IERC4906
 
 
+# @dev We import and implement the `IERC5267` interface,
+# which is written using standard Vyper syntax.
+from ..utils.interfaces.IERC5267 import IERC5267
+implements: IERC5267
+
+
 # @dev We import the `IERC721Receiver` interface, which
 # is written using standard Vyper syntax.
 import interfaces.IERC721Receiver as IERC721Receiver
 
 
 # @dev Stores the ERC-165 interface identifier for each
 # imported interface. The ERC-165 interface identifier
@@ -96,14 +110,18 @@
 ]
 
 
 # @dev Constant used as part of the ECDSA recovery function.
 _MALLEABILITY_THRESHOLD: constant(bytes32) = 0x7FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF5D576E7357A4501DDFE92F46681B20A0
 
 
+# @dev The 32-byte type hash for the EIP-712 domain separator.
+_TYPE_HASH: constant(bytes32) = keccak256("EIP712Domain(string name,string version,uint256 chainId,address verifyingContract)")
+
+
 # @dev The 32-byte type hash of the `permit` function.
 _PERMIT_TYPE_HASH: constant(bytes32) = keccak256("Permit(address spender,uint256 tokenId,uint256 nonce,uint256 deadline)")
 
 
 # @dev Returns the token collection name.
 # @notice If you declare a variable as `public`,
 # Vyper automatically generates an `external`
@@ -122,27 +140,33 @@
 
 
 # @dev Stores the base URI for computing `tokenURI`.
 _BASE_URI: immutable(String[80])
 
 
 # @dev Caches the domain separator as an `immutable`
-# value, but also stores the corresponding chain id
+# value, but also stores the corresponding chain ID
 # to invalidate the cached domain separator if the
-# chain id changes.
+# chain ID changes.
+_CACHED_DOMAIN_SEPARATOR: immutable(bytes32)
 _CACHED_CHAIN_ID: immutable(uint256)
+
+
+# @dev Caches `self` to `immutable` storage to avoid
+# potential issues if a vanilla contract is used in
+# a `delegatecall` context.
 _CACHED_SELF: immutable(address)
-_CACHED_DOMAIN_SEPARATOR: immutable(bytes32)
 
 
-# @dev `immutable` variables to store the name,
-# version, and type hash during contract creation.
+# @dev `immutable` variables to store the (hashed)
+# name and (hashed) version during contract creation.
+_NAME: immutable(String[50])
 _HASHED_NAME: immutable(bytes32)
+_VERSION: immutable(String[20])
 _HASHED_VERSION: immutable(bytes32)
-_TYPE_HASH: immutable(bytes32)
 
 
 # @dev Mapping from owner to operator approvals.
 isApprovedForAll: public(HashMap[address, HashMap[address, bool]])
 
 
 # @dev Returns the address of the current owner.
@@ -240,14 +264,20 @@
 # @dev Emitted when the metadata of a range of
 # tokens is changed.
 event BatchMetadataUpdate:
     from_token_id: uint256
     token_id: uint256
 
 
+# @dev May be emitted to signal that the domain could
+# have changed.
+event EIP712DomainChanged:
+    pass
+
+
 # @dev Emitted when the ownership is transferred
 # from `previous_owner` to `new_owner`.
 event OwnershipTransferred:
     previous_owner: indexed(address)
     new_owner: indexed(address)
 
 
@@ -286,23 +316,21 @@
     symbol = symbol_
     _BASE_URI = base_uri_
 
     self._transfer_ownership(msg.sender)
     self.is_minter[msg.sender] = True
     log RoleMinterChanged(msg.sender, True)
 
-    hashed_name: bytes32 = keccak256(convert(name_eip712_, Bytes[50]))
-    hashed_version: bytes32 = keccak256(convert(version_eip712_, Bytes[20]))
-    type_hash: bytes32 = keccak256(convert("EIP712Domain(string name,string version,uint256 chainId,address verifyingContract)", Bytes[82]))
-    _HASHED_NAME = hashed_name
-    _HASHED_VERSION = hashed_version
-    _TYPE_HASH = type_hash
+    _NAME = name_eip712_
+    _VERSION = version_eip712_
+    _HASHED_NAME = keccak256(name_eip712_)
+    _HASHED_VERSION = keccak256(version_eip712_)
+    _CACHED_DOMAIN_SEPARATOR = self._build_domain_separator()
     _CACHED_CHAIN_ID = chain.id
     _CACHED_SELF = self
-    _CACHED_DOMAIN_SEPARATOR = self._build_domain_separator(type_hash, hashed_name, hashed_version)
 
 
 @external
 @view
 def supportsInterface(interface_id: bytes4) -> bool:
     """
     @dev Returns `True` if this contract implements the
@@ -643,14 +671,40 @@
     @dev Returns the domain separator for the current chain.
     @return bytes32 The 32-byte domain separator.
     """
     return self._domain_separator_v4()
 
 
 @external
+@view
+def eip712Domain() -> (bytes1, String[50], String[20], uint256, address, bytes32, DynArray[uint256, 128]):
+    """
+    @dev Returns the fields and values that describe the domain
+         separator used by this contract for EIP-712 signatures.
+    @notice The bits in the 1-byte bit map are read from the least
+            significant to the most significant, and fields are indexed
+            in the order that is specified by EIP-712, identical to the
+            order in which they are listed in the function type.
+    @return bytes1 The 1-byte bit map where bit `i` is set to 1
+            if and only if domain field `i` is present (`0 ≤ i ≤ 4`).
+    @return String The maximum 50-character user-readable string name
+            of the signing domain, i.e. the name of the dApp or protocol.
+    @return String The maximum 20-character current main version of
+            the signing domain. Signatures from different versions are
+            not compatible.
+    @return uint256 The 32-byte EIP-155 chain ID.
+    @return address The 20-byte address of the verifying contract.
+    @return bytes32 The 32-byte disambiguation salt for the protocol.
+    @return DynArray The 32-byte array of EIP-712 extensions.
+    """
+    # Note that `\x0f` equals `01111`.
+    return (convert(b"\x0f", bytes1), _NAME, _VERSION, chain.id, self, empty(bytes32), empty(DynArray[uint256, 128]))
+
+
+@external
 def transfer_ownership(new_owner: address):
     """
     @dev Transfers the ownership of the contract
          to a new account `new_owner`.
     @notice Note that this function can only be
             called by the current `owner`. Also,
             the `new_owner` cannot be the zero address.
@@ -1168,26 +1222,26 @@
     @dev Sourced from {EIP712DomainSeparator-domain_separator_v4}.
     @notice See {EIP712DomainSeparator-domain_separator_v4}
             for the function docstring.
     """
     if (self == _CACHED_SELF and chain.id == _CACHED_CHAIN_ID):
         return _CACHED_DOMAIN_SEPARATOR
     else:
-        return self._build_domain_separator(_TYPE_HASH, _HASHED_NAME, _HASHED_VERSION)
+        return self._build_domain_separator()
 
 
 @internal
 @view
-def _build_domain_separator(type_hash: bytes32, name_hash: bytes32, version_hash: bytes32) -> bytes32:
+def _build_domain_separator() -> bytes32:
     """
     @dev Sourced from {EIP712DomainSeparator-_build_domain_separator}.
     @notice See {EIP712DomainSeparator-_build_domain_separator}
             for the function docstring.
     """
-    return keccak256(_abi_encode(type_hash, name_hash, version_hash, chain.id, self))
+    return keccak256(_abi_encode(_TYPE_HASH, _HASHED_NAME, _HASHED_VERSION, chain.id, self))
 
 
 @internal
 @view
 def _hash_typed_data_v4(struct_hash: bytes32) -> bytes32:
     """
     @dev Sourced from {EIP712DomainSeparator-hash_typed_data_v4}.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snekmate-0.0.1/src/tokens/interfaces/IERC1155.vy` & `snekmate-0.0.2/src/tokens/interfaces/IERC1155.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title EIP-1155 Interface Definition
+@custom:contract-name IERC1155
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice The required interface definition of an ERC-1155
         compliant smart contract as defined in:
         https://eips.ethereum.org/EIPS/eip-1155. Note that
         smart contracts implementing the ERC-1155 standard
         must implement all of the functions in the ERC-1155
```

### Comparing `snekmate-0.0.1/src/tokens/interfaces/IERC1155MetadataURI.vy` & `snekmate-0.0.2/src/tokens/interfaces/IERC1155MetadataURI.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title EIP-1155 Optional Metadata Interface Definition
+@custom:contract-name IERC1155MetadataURI
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice The metadata extension is optional for an ERC-1155
         smart contract. This allows a smart contract to
         be interrogated for the Uniform Resource Identifier
         (URI) details of a specific token type. For more
         details, please refer to:
@@ -46,15 +47,15 @@
 
 @external
 @view
 def uri(_id: uint256) -> String[512]:
     """
     @dev Returns the Uniform Resource Identifier (URI)
          for token type `_id`.
-    @notice If the `_id` substring is present in the URI,
+    @notice If the `{id}` substring is present in the URI,
             it must be replaced by clients with the actual
             token type ID. Note that the `uri` function must
             not be used to check for the existence of a token
             as it is possible for an implementation to return
             a valid string even if the token does not exist.
     @param _id The 32-byte identifier of the token type `_id`.
     @return String The maximum 512-character user-readable
```

### Comparing `snekmate-0.0.1/src/tokens/interfaces/IERC1155Receiver.vy` & `snekmate-0.0.2/src/tokens/interfaces/IERC1155Receiver.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title EIP-1155 Token Receiver Interface Definition
+@custom:contract-name IERC1155Receiver
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice The interface definition for any contract
         that wants to support safe transfers from
         ERC-1155 asset contracts. For more details,
         please refer to:
         https://eips.ethereum.org/EIPS/eip-1155#erc-1155-token-receiver.
```

### Comparing `snekmate-0.0.1/src/tokens/interfaces/IERC20Permit.vy` & `snekmate-0.0.2/src/tokens/interfaces/IERC20Permit.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title EIP-2612 Interface Definition
+@custom:contract-name IERC20Permit
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice The `permit` function implements approvals via
         EIP-712 secp256k1 signatures:
         https://eips.ethereum.org/EIPS/eip-2612.
         The `permit` function allows users to modify
         the allowance mapping using a signed message
```

### Comparing `snekmate-0.0.1/src/tokens/interfaces/IERC4906.vy` & `snekmate-0.0.2/src/tokens/interfaces/IERC4906.vy`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title EIP-4906 Interface Definition
+@custom:contract-name IERC4906
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice The ERC-4906 standard is an extension of EIP-721.
         It adds a `MetadataUpdate` event to EIP-721 tokens.
-        The ERC-165 identifier for this interface is 0x49064906.
+        The ERC-165 identifier for this interface is `0x49064906`.
         For more details, please refer to:
         https://eips.ethereum.org/EIPS/eip-4906.
 
         On how to use interfaces in Vyper, please visit:
         https://vyper.readthedocs.io/en/latest/interfaces.html#interfaces.
 """
```

### Comparing `snekmate-0.0.1/src/tokens/interfaces/IERC721Enumerable.vy` & `snekmate-0.0.2/src/tokens/interfaces/IERC721Enumerable.vy`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title EIP-721 Optional Enumeration Interface Definition
+@custom:contract-name IERC721Enumerable
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice The enumeration extension is optional for an ERC-721
         smart contract. This allows a contract to publish its
         full list of ERC-721 tokens and make them discoverable.
         For more details, please refer to:
         https://eips.ethereum.org/EIPS/eip-721#specification.
```

### Comparing `snekmate-0.0.1/src/tokens/interfaces/IERC721Metadata.vy` & `snekmate-0.0.2/src/tokens/interfaces/IERC721Metadata.vy`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title EIP-721 Optional Metadata Interface Definition
+@custom:contract-name IERC721Metadata
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice The metadata extension is optional for an ERC-721
         smart contract. This allows a smart contract to
         be interrogated for its name and for details about
         the asset(s) which a non-fungible token (NFT)
         represents. For more details, please refer to:
```

### Comparing `snekmate-0.0.1/src/tokens/interfaces/IERC721Permit.vy` & `snekmate-0.0.2/src/tokens/interfaces/IERC721Permit.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title EIP-4494 Interface Definition
+@custom:contract-name IERC721Permit
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice The `permit` function implements approvals via
         EIP-712 secp256k1 signatures for ERC-721 tokens:
         https://eips.ethereum.org/EIPS/eip-4494. The
         `permit` function allows users to modify the
         permission of who can manage a `tokenId` using
@@ -16,15 +17,15 @@
         such as meta-transactions.
 
         IMPORTANT: Due to sake of consistency, we follow EIP-2612's
         pattern (see https://eips.ethereum.org/EIPS/eip-2612) and
         implement the `permit` function via the secp256k1 signature
         parameters `v`, `r`, and `s` and do not support EIP-2098
         signatures (64-byte length, see https://eips.ethereum.org/EIPS/eip-2098).
-        The ERC-165 identifier for this interface is 0x589C5CE2.
+        The ERC-165 identifier for this interface is `0x589C5CE2`.
 
         On how to use interfaces in Vyper, please visit:
         https://vyper.readthedocs.io/en/latest/interfaces.html#interfaces.
 """
 
 
 # @dev We import and implement the `ERC165` interface,
```

### Comparing `snekmate-0.0.1/src/tokens/interfaces/IERC721Receiver.vy` & `snekmate-0.0.2/src/tokens/interfaces/IERC721Receiver.vy`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title EIP-721 Token Receiver Interface Definition
+@custom:contract-name IERC721Receiver
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice The interface definition for any contract
         that wants to support safe transfers from
         ERC-721 asset contracts. For more details,
         please refer to:
         https://eips.ethereum.org/EIPS/eip-721#specification.
```

### Comparing `snekmate-0.0.1/src/utils/Base64.vy` & `snekmate-0.0.2/src/utils/Base64.vy`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Base64 Encoding and Decoding Functions
+@custom:contract-name Base64
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions can be used to encode bytes or to decode strings
         using the Base64 binary-to-text encoding scheme. For more details,
         please refer to: https://www.rfc-editor.org/rfc/rfc4648#section-4.
         The implementation is inspired by Brecht Devos' implementation here:
         https://github.com/Brechtpd/base64/blob/main/base64.sol,
@@ -59,15 +60,15 @@
            or not.
     @return DynArray The maximum 4-character user-readable
             string array that combined results in the Base64
             encoding of `data`.
     """
     data_length: uint256 = len(data)
     if (data_length == empty(uint256)):
-        return empty(DynArray[String[4], 1])
+        return empty(DynArray[String[4], _DATA_OUTPUT_BOUND])
 
     # If the length of the unencoded input is not
     # a multiple of three, the encoded output must
     # have padding added so that its length is a
     # multiple of four.
     padding: uint256 = data_length % 3
     data_padded: Bytes[_DATA_INPUT_BOUND + 2] = b""
@@ -101,17 +102,17 @@
         # `>> 18` (right shift `c1` by 18 bits)
         #   6bit   6bit   6bit   6bit
         # │------│------│------│------│
         #  000000 000000 000000 011100
         #
         # 63 (or `0x3F`) is `000000000000000000111111` in binary.
         # Thus, the bitwise `AND` operation is redundant.
-        c1: uint256 = shift(chunk, -18)
-        c2: uint256 = shift(chunk, -12) & 63
-        c3: uint256 = shift(chunk, -6) & 63
+        c1: uint256 = chunk >> 18
+        c2: uint256 = (chunk >> 12) & 63
+        c3: uint256 = (chunk >> 6) & 63
         c4: uint256 = chunk & 63
 
         # Base64 encoding with an URL and filename-safe
         # alphabet.
         if (base64_url):
             char_chunks.append(concat(slice(_TABLE_URL_CHARS, c1, 1), slice(_TABLE_URL_CHARS, c2, 1), slice(_TABLE_URL_CHARS, c3, 1),\
                                       slice(_TABLE_URL_CHARS, c4, 1)))
@@ -189,20 +190,20 @@
             c2: uint256 = self._index_of(slice(chunk, 1, 1), True)
             c3: uint256 = self._index_of(slice(chunk, 2, 1), True)
             c4: uint256 = self._index_of(slice(chunk, 3, 1), True)
 
             # We concatenate the 6-bit index in the Base64
             # character list, which gives the 24-bit number
             # for the original three characters.
-            chunk_bytes: uint256 = shift(c1, 18) | shift(c2, 12) | shift(c3, 6) | c4
+            chunk_bytes: uint256 = (c1 << 18) | (c2 << 12) | (c3 << 6) | c4
 
             # We split the 24-bit number into the original
             # three 8-bit characters.
-            b1: bytes1 = convert(convert(shift(chunk_bytes, -16) & 255, uint8), bytes1)
-            b2: bytes1 = convert(convert(shift(chunk_bytes, -8) & 255, uint8), bytes1)
+            b1: bytes1 = convert(convert((chunk_bytes >> 16) & 255, uint8), bytes1)
+            b2: bytes1 = convert(convert((chunk_bytes >> 8) & 255, uint8), bytes1)
             b3: bytes1 = convert(convert(chunk_bytes & 255, uint8), bytes1)
 
             # Case 1: padding of "=" as part of the
             # encoded input.
             if (c4 == 64):
                 result.append(concat(b1, b2, b"\x00"))
             # Case 2: padding of "==" as part of the
@@ -226,20 +227,20 @@
         # Base64 encoding using the standard characters.
         else:
             c1: uint256 = self._index_of(slice(chunk, 0, 1), False)
             c2: uint256 = self._index_of(slice(chunk, 1, 1), False)
             c3: uint256 = self._index_of(slice(chunk, 2, 1), False)
             c4: uint256 = self._index_of(slice(chunk, 3, 1), False)
 
-            chunk_bytes: uint256 = shift(c1, 18) | shift(c2, 12) | shift(c3, 6) | c4
+            chunk_bytes: uint256 = (c1 << 18) | (c2 << 12) | (c3 << 6) | c4
 
             # We split the 24-bit number into the original
             # three 8-bit characters.
-            b1: bytes1 = convert(convert(shift(chunk_bytes, -16) & 255, uint8), bytes1)
-            b2: bytes1 = convert(convert(shift(chunk_bytes, -8) & 255, uint8), bytes1)
+            b1: bytes1 = convert(convert((chunk_bytes >> 16) & 255, uint8), bytes1)
+            b2: bytes1 = convert(convert((chunk_bytes >> 8) & 255, uint8), bytes1)
             b3: bytes1 = convert(convert(chunk_bytes & 255, uint8), bytes1)
 
             # Case 1: padding of "=" as part of the
             # encoded input.
             if (c4 == 64):
                 result.append(concat(b1, b2, b"\x00"))
             # Case 2: padding of "==" as part of the
```

### Comparing `snekmate-0.0.1/src/utils/BatchDistributor.vy` & `snekmate-0.0.2/src/utils/BatchDistributor.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Batch Sending Both Native and ERC-20 Tokens
+@custom:contract-name BatchDistributor
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions can be used for batch sending
         both native and ERC-20 tokens. The implementation
         is inspired by my implementation here:
         https://github.com/pcaversaccio/batch-distributor/blob/main/contracts/BatchDistributor.sol,
         as well as by the original implementation of banteg:
```

### Comparing `snekmate-0.0.1/src/utils/Create2Address.vy` & `snekmate-0.0.2/src/utils/Create2Address.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title `CREATE2` EVM Opcode Utility Functions for Address Calculations
+@custom:contract-name Create2Address
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions can be used to compute in advance the address
         where a smart contract will be deployed if deployed via the
         `CREATE2` opcode. The implementation is inspired by OpenZeppelin's
         implementation here:
         https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/utils/Create2.sol.
@@ -83,8 +84,8 @@
 @pure
 def _convert_keccak256_2_address(digest: bytes32) -> address:
     """
     @dev Converts a 32-byte keccak256 digest to an address.
     @param digest The 32-byte keccak256 digest.
     @return address The converted 20-byte address.
     """
-    return convert(convert(digest, uint256) & max_value(uint160), address)
+    return convert(convert(digest, uint256) & convert(max_value(uint160), uint256), address)
```

### Comparing `snekmate-0.0.1/src/utils/CreateAddress.vy` & `snekmate-0.0.2/src/utils/CreateAddress.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title `CREATE` EVM Opcode Utility Functions for Address Calculations
+@custom:contract-name CreateAddress
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions can be used to compute in advance the address
         where a smart contract will be deployed if deployed via the
         `CREATE` opcode. The implementation is inspired by my
         implementation here:
         https://github.com/pcaversaccio/create-util/blob/main/contracts/Create.sol.
@@ -124,8 +125,8 @@
 @pure
 def _convert_keccak256_2_address(digest: bytes32) -> address:
     """
     @dev Converts a 32-byte keccak256 digest to an address.
     @param digest The 32-byte keccak256 digest.
     @return address The converted 20-byte address.
     """
-    return convert(convert(digest, uint256) & max_value(uint160), address)
+    return convert(convert(digest, uint256) & convert(max_value(uint160), uint256), address)
```

### Comparing `snekmate-0.0.1/src/utils/ECDSA.vy` & `snekmate-0.0.2/src/utils/ECDSA.vy`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Elliptic Curve Digital Signature Algorithm (ECDSA) Functions
+@custom:contract-name ECDSA
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions can be used to verify that a message was signed
         by the holder of the private key of a given address. Additionally,
         we provide helper functions to handle signed data in Ethereum
         contracts based on EIP-191: https://eips.ethereum.org/EIPS/eip-191.
         The implementation is inspired by OpenZeppelin's implementation here:
@@ -164,17 +165,17 @@
     @param hash The 32-byte message digest that was signed.
     @param r The secp256k1 32-byte signature parameter `r`.
     @param vs The secp256k1 32-byte short signature field of `v` and `s`.
     @return address The recovered 20-byte signer address.
     """
     s: uint256 = vs & convert(_SIGNATURE_INCREMENT, uint256)
     # We do not check for an overflow here since the shift operation
-    # `shift(vs, -255)` results essentially in a uint8 type (0 or 1)
-    # and we use uint256 as result type.
-    v: uint256 = unsafe_add(shift(vs, -255), 27)
+    # `vs >> 255` results essentially in a `uint8` type (0 or 1) and
+    # we use `uint256` as result type.
+    v: uint256 = unsafe_add(vs >> 255, 27)
     return self._try_recover_vrs(hash, v, r, s)
 
 
 @internal
 @pure
 def _try_recover_vrs(hash: bytes32, v: uint256, r: uint256, s: uint256) -> address:
     """
```

### Comparing `snekmate-0.0.1/src/utils/Math.vy` & `snekmate-0.0.2/src/utils/Math.vy`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,33 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Standard Mathematical Utility Functions
+@custom:contract-name Math
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @custom:coauthor bout3fiddy
 @notice These functions implement standard mathematical utility
         functions that are missing in the Vyper language. If a
         function is inspired by an existing implementation, it
-        is properly referenced in the function docstring.
+        is properly referenced in the function docstring. The
+        following functions have been added for convenience:
+        - `uint256_average` (`external` `pure` function),
+        - `int256_average` (`external` `pure` function),
+        - `ceil_div` (`external` `pure` function),
+        - `is_negative` (`external` `pure` function),
+        - `mul_div` (`external` `pure` function),
+        - `log_2` (`external` `pure` function),
+        - `log_10` (`external` `pure` function),
+        - `log_256` (`external` `pure` function),
+        - `wad_ln` (`external` `pure` function),
+        - `wad_exp` (`external` `pure` function),
+        - `cbrt` (`external` `pure` function),
+        - `wad_cbrt` (`external` `pure` function),
+        - `_log_2` (`internal` `pure` function),
+        - `_wad_cbrt` (`internal` `pure` function).
 """
 
 
 @external
 @payable
 def __init__():
     """
@@ -20,14 +36,78 @@
          is declared as `payable`.
     """
     pass
 
 
 @external
 @pure
+def uint256_average(x: uint256, y: uint256) -> uint256:
+    """
+    @dev Returns the average of two 32-byte unsigned integers.
+    @notice Note that the result is rounded towards zero. For
+            more details on finding the average of two unsigned
+            integers without an overflow, please refer to:
+            https://devblogs.microsoft.com/oldnewthing/20220207-00/?p=106223.
+    @param x The first 32-byte unsigned integer of the data set.
+    @param y The second 32-byte unsigned integer of the data set.
+    @return uint256 The 32-byte average (rounded towards zero) of
+            `x` and `y`.
+    """
+    return unsafe_add(x & y, (x ^ y) >> 1)
+
+
+@external
+@pure
+def int256_average(x: int256, y: int256) -> int256:
+    """
+    @dev Returns the average of two 32-byte signed integers.
+    @notice Note that the result is rounded towards infinity.
+            For more details on finding the average of two signed
+            integers without an overflow, please refer to:
+            https://patents.google.com/patent/US6007232A/en.
+    @param x The first 32-byte signed integer of the data set.
+    @param y The second 32-byte signed integer of the data set.
+    @return int256 The 32-byte average (rounded towards infinity)
+            of `x` and `y`.
+    """
+    return unsafe_add(unsafe_add(x >> 1, y >> 1), x & y & 1)
+
+
+@external
+@pure
+def ceil_div(x: uint256, y: uint256) -> uint256:
+    """
+    @dev Calculates "ceil(x / y)" for any strictly positive `y`.
+    @notice The implementation is inspired by OpenZeppelin's
+            implementation here:
+            https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/utils/math/Math.sol.
+    @param x The 32-byte numerator.
+    @param y The 32-byte denominator.
+    @return uint256 The 32-byte rounded up result of "x/y".
+    """
+    assert y != empty(uint256), "Math: ceil_div division by zero"
+    # Due to a known compiler bug (https://github.com/vyperlang/vyper/issues/3480),
+    # we use `0` instead of `empty(uint256)` as return value.
+    return 0 if (x == empty(uint256)) else unsafe_add(unsafe_div(x - 1, y), 1)
+
+
+@external
+@pure
+def is_negative(x: int256) -> bool:
+    """
+    @dev Returns `True` if a 32-byte signed integer is negative.
+    @notice Note that this function returns `False` for 0.
+    @param x The 32-byte signed integer variable.
+    @return bool The verification whether `x` is negative or not.
+    """
+    return (x ^ 1 < empty(int256))
+
+
+@external
+@pure
 def mul_div(x: uint256, y: uint256, denominator: uint256, roundup: bool) -> uint256:
     """
     @dev Calculates "(x * y) / denominator" in 512-bit precision,
          following the selected rounding direction.
     @notice The implementation is inspired by Remco Bloemen's
             implementation under the MIT license here:
             https://xn--2-umb.com/21/muldiv.
@@ -142,117 +222,32 @@
         result += 1
 
     return result
 
 
 @external
 @pure
-def uint256_average(x: uint256, y: uint256) -> uint256:
-    """
-    @dev Returns the average of two 32-byte unsigned integers.
-    @notice Note that the result is rounded towards zero. For
-            more details on finding the average of two unsigned
-            integers without an overflow, please refer to:
-            https://devblogs.microsoft.com/oldnewthing/20220207-00/?p=106223.
-    @param x The first 32-byte unsigned integer of the data set.
-    @param y The second 32-byte unsigned integer of the data set.
-    @return uint256 The 32-byte average (rounded towards zero) of
-            `x` and `y`.
-    """
-    return unsafe_add(x & y, shift(x ^ y, -1))
-
-
-@external
-@pure
-def int256_average(x: int256, y: int256) -> int256:
-    """
-    @dev Returns the average of two 32-byte signed integers.
-    @notice Note that the result is rounded towards infinity.
-            For more details on finding the average of two signed
-            integers without an overflow, please refer to:
-            https://patents.google.com/patent/US6007232A/en.
-    @param x The first 32-byte signed integer of the data set.
-    @param y The second 32-byte signed integer of the data set.
-    @return uint256 The 32-byte average (rounded towards infinity)
-            of `x` and `y`.
-    """
-    return unsafe_add(unsafe_add(shift(x, -1), shift(y, -1)), x & y & 1)
-
-
-@external
-@pure
-def ceil_div(x: uint256, y: uint256) -> uint256:
-    """
-    @dev Calculates "ceil(x / y)" for any strictly positive `y`.
-    @notice The implementation is inspired by OpenZeppelin's
-            implementation here:
-            https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/utils/math/Math.sol.
-    @param x The 32-byte numerator.
-    @param y The 32-byte denominator.
-    @return uint256 The 32-byte rounded up result of "x/y".
-    """
-    assert y != empty(uint256), "Math: ceil_div division by zero"
-    if (x == empty(uint256)):
-        return empty(uint256)
-    else:
-        return unsafe_add(unsafe_div(x - 1, y), 1)
-
-
-@external
-@pure
 def log_2(x: uint256, roundup: bool) -> uint256:
     """
     @dev Returns the log in base 2 of `x`, following the selected
          rounding direction.
     @notice Note that it returns 0 if given 0. The implementation is
             inspired by OpenZeppelin's implementation here:
             https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/utils/math/Math.sol.
     @param x The 32-byte variable.
     @param roundup The Boolean variable that specifies whether
            to round up or not. The default `False` is round down.
     @return uint256 The 32-byte calculation result.
     """
-    value: uint256 = x
-    result: uint256 = empty(uint256)
-
+    # For the special case `x == 0` we already return 0 here in order
+    # not to iterate through the remaining code.
     if (x == empty(uint256)):
-        # For the special case `x == 0` we already return 0 here in order
-        # not to iterate through the remaining code.
         return empty(uint256)
 
-    # The following lines cannot overflow because we have the well-known
-    # decay behaviour of `log_2(max_value(uint256)) < max_value(uint256)`.
-    if (shift(x, -128) != empty(uint256)):
-        value = shift(x, -128)
-        result = 128
-    if (shift(value, -64) != empty(uint256)):
-        value = shift(value, -64)
-        result = unsafe_add(result, 64)
-    if (shift(value, -32) != empty(uint256)):
-        value = shift(value, -32)
-        result = unsafe_add(result, 32)
-    if (shift(value, -16) != empty(uint256)):
-        value = shift(value, -16)
-        result = unsafe_add(result, 16)
-    if (shift(value, -8) != empty(uint256)):
-        value = shift(value, -8)
-        result = unsafe_add(result, 8)
-    if (shift(value, -4) != empty(uint256)):
-        value = shift(value, -4)
-        result = unsafe_add(result, 4)
-    if (shift(value, -2) != empty(uint256)):
-        value = shift(value, -2)
-        result = unsafe_add(result, 2)
-    if (shift(value, -1) != empty(uint256)):
-        result = unsafe_add(result, 1)
-
-    if (roundup and (shift(1, convert(result, int256)) < x)):
-        result = unsafe_add(result, 1)
-
-    return result
+    return self._log_2(x, roundup)
 
 
 @external
 @pure
 def log_10(x: uint256, roundup: bool) -> uint256:
     """
     @dev Returns the log in base 10 of `x`, following the selected
@@ -264,17 +259,17 @@
     @param roundup The Boolean variable that specifies whether
            to round up or not. The default `False` is round down.
     @return uint256 The 32-byte calculation result.
     """
     value: uint256 = x
     result: uint256 = empty(uint256)
 
+    # For the special case `x == 0` we already return 0 here in order
+    # not to iterate through the remaining code.
     if (x == empty(uint256)):
-        # For the special case `x == 0` we already return 0 here in order
-        # not to iterate through the remaining code.
         return empty(uint256)
 
     # The following lines cannot overflow because we have the well-known
     # decay behaviour of `log_10(max_value(uint256)) < max_value(uint256)`.
     if (x >= 10 ** 64):
         value = unsafe_div(x, 10 ** 64)
         result = 64
@@ -317,59 +312,200 @@
     @param roundup The Boolean variable that specifies whether
            to round up or not. The default `False` is round down.
     @return uint256 The 32-byte calculation result.
     """
     value: uint256 = x
     result: uint256 = empty(uint256)
 
+    # For the special case `x == 0` we already return 0 here in order
+    # not to iterate through the remaining code.
     if (x == empty(uint256)):
-        # For the special case `x == 0` we already return 0 here in order
-        # not to iterate through the remaining code.
         return empty(uint256)
 
     # The following lines cannot overflow because we have the well-known
     # decay behaviour of `log_256(max_value(uint256)) < max_value(uint256)`.
-    if (shift(x, -128) != empty(uint256)):
-        value = shift(x, -128)
+    if (x >> 128 != empty(uint256)):
+        value = x >> 128
         result = 16
-    if (shift(value, -64) != empty(uint256)):
-        value = shift(value, -64)
+    if (value >> 64 != empty(uint256)):
+        value = value >> 64
         result = unsafe_add(result, 8)
-    if (shift(value, -32) != empty(uint256)):
-        value = shift(value, -32)
+    if (value >> 32 != empty(uint256)):
+        value = value >> 32
         result = unsafe_add(result, 4)
-    if (shift(value, -16) != empty(uint256)):
-        value = shift(value, -16)
+    if (value >> 16 != empty(uint256)):
+        value = value >> 16
         result = unsafe_add(result, 2)
-    if (shift(value, -8) != empty(uint256)):
+    if (value >> 8 != empty(uint256)):
         result = unsafe_add(result, 1)
 
-    if (roundup and (shift(1, convert(shift(result, 3), int256)) < x)):
+    if (roundup and ((1 << (result << 3)) < x)):
         result = unsafe_add(result, 1)
 
     return result
 
 
 @external
-@view
+@pure
+def wad_ln(x: int256) -> int256:
+    """
+    @dev Calculates the natural logarithm of a signed integer with a
+         precision of 1e18.
+    @notice Note that it returns 0 if given 0. Furthermore, this function
+            consumes about 1,400 to 1,650 gas units depending on the value
+            of `x`. The implementation is inspired by Remco Bloemen's
+            implementation under the MIT license here:
+            https://xn--2-umb.com/22/exp-ln.
+    @param x The 32-byte variable.
+    @return int256 The 32-byte calculation result.
+    """
+    value: int256 = x
+
+    assert x >= empty(int256), "Math: wad_ln undefined"
+
+    # For the special case `x == 0` we already return 0 here in order
+    # not to iterate through the remaining code.
+    if (x == empty(int256)):
+        return empty(int256)
+
+    # We want to convert `x` from "10 ** 18" fixed point to "2 ** 96"
+    # fixed point. We do this by multiplying by "2 ** 96 / 10 ** 18".
+    # But since "ln(x * C) = ln(x) + ln(C)" holds, we can just do nothing
+    # here and add "ln(2 ** 96 / 10 ** 18)" at the end.
+
+    # Reduce the range of `x` to "(1, 2) * 2 ** 96".
+    # Also remember that "ln(2 ** k * x) = k * ln(2) + ln(x)" holds.
+    k: int256 = unsafe_sub(convert(self._log_2(convert(x, uint256), False), int256), 96)
+    # Note that to circumvent Vyper's safecast feature for the potentially
+    # negative expression `value <<= uint256(159 - k)`, we first convert the
+    # expression `value <<= uint256(159 - k)` to `bytes32` and subsequently
+    # to `uint256`. Remember that the EVM default behaviour is to use two's
+    # complement representation to handle signed integers.
+    value = convert(convert(convert(value << convert(unsafe_sub(159, k), uint256), bytes32), uint256) >> 159, int256)
+
+    # Evaluate using a "(8, 8)"-term rational approximation. Since `p` is monic,
+    # we will multiply by a scaling factor later.
+    p: int256 = unsafe_add(unsafe_mul(unsafe_add(value, 3273285459638523848632254066296), value) >> 96, 24828157081833163892658089445524)
+    p = unsafe_add(unsafe_mul(p, value) >> 96, 43456485725739037958740375743393)
+    p = unsafe_sub(unsafe_mul(p, value) >> 96, 11111509109440967052023855526967)
+    p = unsafe_sub(unsafe_mul(p, value) >> 96, 45023709667254063763336534515857)
+    p = unsafe_sub(unsafe_mul(p, value) >> 96, 14706773417378608786704636184526)
+    p = unsafe_sub(unsafe_mul(p, value), 795164235651350426258249787498 << 96)
+
+    # We leave `p` in the "2 ** 192" base so that we do not have to scale it up
+    # again for the division. Note that `q` is monic by convention.
+    q: int256 = unsafe_add(unsafe_mul(unsafe_add(value, 5573035233440673466300451813936), value) >> 96, 71694874799317883764090561454958)
+    q = unsafe_add(unsafe_mul(q, value) >> 96, 283447036172924575727196451306956)
+    q = unsafe_add(unsafe_mul(q, value) >> 96, 401686690394027663651624208769553)
+    q = unsafe_add(unsafe_mul(q, value) >> 96, 204048457590392012362485061816622)
+    q = unsafe_add(unsafe_mul(q, value) >> 96, 31853899698501571402653359427138)
+    q = unsafe_add(unsafe_mul(q, value) >> 96, 909429971244387300277376558375)
+
+    # It is known that the polynomial `q` has no zeros in the domain.
+    # No scaling is required, as `p` is already "2 ** 96" too large. Also,
+    # `r` is in the range "(0, 0.125) * 2 ** 96" after the division.
+    r: int256 = unsafe_div(p, q)
+
+    # To finalise the calculation, we have to proceed with the following steps:
+    #   - multiply by the scaling factor "s = 5.549...",
+    #   - add "ln(2 ** 96 / 10 ** 18)",
+    #   - add "k * ln(2)", and
+    #   - multiply by "10 ** 18 / 2 ** 96 = 5 ** 18 >> 78".
+    # In order to perform the most gas-efficient calculation, we carry out all
+    # these steps in one expression.
+    return unsafe_add(unsafe_add(unsafe_mul(r, 1677202110996718588342820967067443963516166),\
+           unsafe_mul(k, 16597577552685614221487285958193947469193820559219878177908093499208371)),\
+           600920179829731861736702779321621459595472258049074101567377883020018308) >> 174
+
+
+@external
+@pure
+def wad_exp(x: int256) -> int256:
+    """
+    @dev Calculates the natural exponential function of a signed integer with
+         a precision of 1e18.
+    @notice Note that this function consumes about 810 gas units. The implementation
+            is inspired by Remco Bloemen's implementation under the MIT license here:
+            https://xn--2-umb.com/22/exp-ln.
+    @param x The 32-byte variable.
+    @return int256 The 32-byte calculation result.
+    """
+    value: int256 = x
+
+    # If the result is `< 0.5`, we return zero. This happens when we have the following:
+    # "x <= floor(log(0.5e18) * 1e18) ~ -42e18".
+    if (x <= -42139678854452767551):
+        return empty(int256)
+
+    # When the result is "> (2 ** 255 - 1) / 1e18" we cannot represent it as a signed integer.
+    # This happens when "x >= floor(log((2 ** 255 - 1) / 1e18) * 1e18) ~ 135".
+    assert x < 135305999368893231589, "Math: wad_exp overflow"
+
+    # `x` is now in the range "(-42, 136) * 1e18". Convert to "(-42, 136) * 2 ** 96" for higher
+    # intermediate precision and a binary base. This base conversion is a multiplication with
+    # "1e18 / 2 ** 96 = 5 ** 18 / 2 ** 78".
+    value = unsafe_div(x << 78, 5 ** 18)
+
+    # Reduce the range of `x` to "(-½ ln 2, ½ ln 2) * 2 ** 96" by factoring out powers of two
+    # so that "exp(x) = exp(x') * 2 ** k", where `k` is a signer integer. Solving this gives
+    # "k = round(x / log(2))" and "x' = x - k * log(2)". Thus, `k` is in the range "[-61, 195]".
+    k: int256 = unsafe_add(unsafe_div(value << 96, 54916777467707473351141471128), 2 ** 95) >> 96
+    value = unsafe_sub(value, unsafe_mul(k, 54916777467707473351141471128))
+
+    # Evaluate using a "(6, 7)"-term rational approximation. Since `p` is monic,
+    # we will multiply by a scaling factor later.
+    y: int256 = unsafe_add(unsafe_mul(unsafe_add(value, 1346386616545796478920950773328), value) >> 96, 57155421227552351082224309758442)
+    p: int256 = unsafe_add(unsafe_mul(unsafe_add(unsafe_mul(unsafe_sub(unsafe_add(y, value), 94201549194550492254356042504812), y) >> 96,\
+                           28719021644029726153956944680412240), value), 4385272521454847904659076985693276 << 96)
+
+    # We leave `p` in the "2 ** 192" base so that we do not have to scale it up
+    # again for the division.
+    q: int256 = unsafe_add(unsafe_mul(unsafe_sub(value, 2855989394907223263936484059900), value) >> 96, 50020603652535783019961831881945)
+    q = unsafe_sub(unsafe_mul(q, value) >> 96, 533845033583426703283633433725380)
+    q = unsafe_add(unsafe_mul(q, value) >> 96, 3604857256930695427073651918091429)
+    q = unsafe_sub(unsafe_mul(q, value) >> 96, 14423608567350463180887372962807573)
+    q = unsafe_add(unsafe_mul(q, value) >> 96, 26449188498355588339934803723976023)
+
+    # The polynomial `q` has no zeros in the range because all its roots are complex.
+    # No scaling is required, as `p` is already "2 ** 96" too large. Also,
+    # `r` is in the range "(0.09, 0.25) * 2**96" after the division.
+    r: int256 = unsafe_div(p, q)
+
+    # To finalise the calculation, we have to multiply `r` by:
+    #   - the scale factor "s = ~6.031367120",
+    #   - the factor "2 ** k" from the range reduction, and
+    #   - the factor "1e18 / 2 ** 96" for the base conversion.
+    # We do this all at once, with an intermediate result in "2**213" base,
+    # so that the final right shift always gives a positive value.
+
+    # Note that to circumvent Vyper's safecast feature for the potentially
+    # negative parameter value `r`, we first convert `r` to `bytes32` and
+    # subsequently to `uint256`. Remember that the EVM default behaviour is
+    # to use two's complement representation to handle signed integers.
+    return convert(unsafe_mul(convert(convert(r, bytes32), uint256), 3822833074963236453042738258902158003155416615667) >>\
+           convert(unsafe_sub(195, k), uint256), int256)
+
+
+@external
+@pure
 def cbrt(x: uint256, roundup: bool) -> uint256:
     """
     @dev Calculates the cube root of an unsigned integer.
-    @notice Note that this function consumes about 1,950 to 2,050 gas units
+    @notice Note that this function consumes about 1,600 to 1,800 gas units
             depending on the value of `x` and `roundup`. The implementation is
             inspired by Curve Finance's implementation under the MIT license here:
             https://github.com/curvefi/tricrypto-ng/blob/main/contracts/CurveCryptoMathOptimized3.vy.
     @param x The 32-byte variable from which the cube root is calculated.
     @param roundup The Boolean variable that specifies whether
            to round up or not. The default `False` is round down.
     @return The 32-byte cube root of `x`.
     """
+    # For the special case `x == 0` we already return 0 here in order
+    # not to iterate through the remaining code.
     if (x == empty(uint256)):
-        # For the special case `x == 0` we already return 0 here in order
-        # not to iterate through the remaining code.
         return empty(uint256)
 
     y: uint256 = unsafe_div(self._wad_cbrt(x), 10 ** 12)
 
     if (roundup and (unsafe_mul(unsafe_mul(y, y), y) != x)):
         y = unsafe_add(y, 1)
 
@@ -378,89 +514,104 @@
 
 @external
 @pure
 def wad_cbrt(x: uint256) -> uint256:
     """
     @dev Calculates the cube root of an unsigned integer with a precision
          of 1e18.
-    @notice Note that this function consumes about 1,850 to 1,950 gas units
+    @notice Note that this function consumes about 1,500 to 1,700 gas units
             depending on the value of `x`. The implementation is inspired
             by Curve Finance's implementation under the MIT license here:
             https://github.com/curvefi/tricrypto-ng/blob/main/contracts/CurveCryptoMathOptimized3.vy.
     @param x The 32-byte variable from which the cube root is calculated.
     @return The 32-byte cubic root of `x` with a precision of 1e18.
     """
+    # For the special case `x == 0` we already return 0 here in order
+    # not to iterate through the remaining code.
     if (x == empty(uint256)):
-        # For the special case `x == 0` we already return 0 here in order
-        # not to iterate through the remaining code.
         return empty(uint256)
 
     return self._wad_cbrt(x)
 
 
-@external
+@internal
 @pure
-def is_negative(x: int256) -> bool:
+def _log_2(x: uint256, roundup: bool) -> uint256:
     """
-    @dev Returns `True` if a 32-byte signed integer is negative.
-    @notice Note that this function returns `False` for 0.
-    @param x The 32-byte signed integer variable.
-    @return bool The verification whether `x` is negative or not.
+    @dev An `internal` helper function that returns the log in base 2
+         of `x`, following the selected rounding direction.
+    @notice Note that it returns 0 if given 0. The implementation is
+            inspired by OpenZeppelin's implementation here:
+            https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/utils/math/Math.sol.
+    @param x The 32-byte variable.
+    @param roundup The Boolean variable that specifies whether
+           to round up or not. The default `False` is round down.
+    @return uint256 The 32-byte calculation result.
     """
-    return (x ^ 1 < empty(int256))
+    value: uint256 = x
+    result: uint256 = empty(uint256)
+
+    # The following lines cannot overflow because we have the well-known
+    # decay behaviour of `log_2(max_value(uint256)) < max_value(uint256)`.
+    if (x >> 128 != empty(uint256)):
+        value = x >> 128
+        result = 128
+    if (value >> 64 != empty(uint256)):
+        value = value >> 64
+        result = unsafe_add(result, 64)
+    if (value >> 32 != empty(uint256)):
+        value = value >> 32
+        result = unsafe_add(result, 32)
+    if (value >> 16 != empty(uint256)):
+        value = value >> 16
+        result = unsafe_add(result, 16)
+    if (value >> 8 != empty(uint256)):
+        value = value >> 8
+        result = unsafe_add(result, 8)
+    if (value >> 4 != empty(uint256)):
+        value = value >> 4
+        result = unsafe_add(result, 4)
+    if (value >> 2 != empty(uint256)):
+        value = value >> 2
+        result = unsafe_add(result, 2)
+    if (value >> 1 != empty(uint256)):
+        result = unsafe_add(result, 1)
+
+    if (roundup and ((1 << result) < x)):
+        result = unsafe_add(result, 1)
+
+    return result
 
 
 @internal
 @pure
 def _wad_cbrt(x: uint256) -> uint256:
     """
     @dev An `internal` helper function that calculates the cube root of an
          unsigned integer with a precision of 1e18.
-    @notice Note that this function consumes about 1,800 to 1,850 gas units
+    @notice Note that this function consumes about 1,450 to 1,650 gas units
             depending on the value of `x`. The implementation is inspired
             by Curve Finance's implementation under the MIT license here:
             https://github.com/curvefi/tricrypto-ng/blob/main/contracts/CurveCryptoMathOptimized3.vy.
     @param x The 32-byte variable from which the cube root is calculated.
     @return The 32-byte cubic root of `x` with a precision of 1e18.
     """
     # Since this cube root is for numbers with base 1e18, we have to scale
     # the input by 1e36 to increase the precision. This leads to an overflow
     # for very large numbers. So we conditionally sacrifice precision.
-    xx: uint256 = empty(uint256)
+    value: uint256 = empty(uint256)
     if (x >= unsafe_mul(unsafe_div(max_value(uint256), 10 ** 36), 10 ** 18)):
-        xx = x
+        value = x
     elif (x >= unsafe_div(max_value(uint256), 10 ** 36)):
-        xx = unsafe_mul(x, 10 ** 18)
+        value = unsafe_mul(x, 10 ** 18)
     else:
-        xx = unsafe_mul(x, 10 ** 36)
+        value = unsafe_mul(x, 10 ** 36)
 
-    # Compute the binary logarithm of `xx`. This approach was inspired by Sean
-    # Eron Anderson's "Bit Twiddling Hacks" from Stanford:
-    # https://graphics.stanford.edu/~seander/bithacks.html#IntegerLog.
-    # Further inspiration stems from solmate:
-    # https://github.com/transmissions11/solmate/blob/main/src/utils/SignedWadMath.sol.
-    # A detailed mathematical explanation by Remco Bloemen can be found here:
-    # https://xn--2-umb.com/22/exp-ln.
-    log2x: uint256 = empty(uint256)
-    if (xx > max_value(uint128)):
-        log2x = 128
-    if (unsafe_div(xx, shift(2, convert(log2x, int256))) > max_value(uint64)):
-        log2x = log2x | 64
-    if (unsafe_div(xx, shift(2, convert(log2x, int256))) > max_value(uint32)):
-        log2x = log2x | 32
-    if (unsafe_div(xx, shift(2, convert(log2x, int256))) > max_value(uint16)):
-        log2x = log2x | 16
-    if (unsafe_div(xx, shift(2, convert(log2x, int256))) > max_value(uint8)):
-        log2x = log2x | 8
-    if (unsafe_div(xx, shift(2, convert(log2x, int256))) > 15):
-        log2x = log2x | 4
-    if (unsafe_div(xx, shift(2, convert(log2x, int256))) > 3):
-        log2x = log2x | 2
-    if (unsafe_div(xx, shift(2, convert(log2x, int256))) > 1):
-        log2x = log2x | 1
+    # Compute the binary logarithm of `value`.
+    log2x: uint256 = self._log_2(value, False)
 
     # If we divide log2x by 3, the remainder is "log2x % 3". So if we simply
     # multiply "2 ** (log2x/3)" and discard the remainder to calculate our guess,
     # the Newton-Raphson method takes more iterations to converge to a solution
     # because it lacks this precision. A few more calculations now in order to
     # do fewer calculations later:
     #   - "pow = log2(x) // 3" (the operator `//` means integer division),
@@ -472,22 +623,22 @@
     y: uint256 = unsafe_div(unsafe_mul(pow_mod256(2, unsafe_div(log2x, 3)), pow_mod256(1260, remainder)), pow_mod256(1000, remainder))
 
     # Since we have chosen good initial values for the cube roots, 7 Newton-Raphson
     # iterations are just sufficient. 6 iterations would lead to non-convergences,
     # and 8 would be one iteration too many. Without initial values, the iteration
     # number can be up to 20 or more. The iterations are unrolled. This reduces the
     # gas cost, but requires more bytecode.
-    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(xx, unsafe_mul(y, y))), 3)
-    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(xx, unsafe_mul(y, y))), 3)
-    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(xx, unsafe_mul(y, y))), 3)
-    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(xx, unsafe_mul(y, y))), 3)
-    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(xx, unsafe_mul(y, y))), 3)
-    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(xx, unsafe_mul(y, y))), 3)
-    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(xx, unsafe_mul(y, y))), 3)
+    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(value, unsafe_mul(y, y))), 3)
+    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(value, unsafe_mul(y, y))), 3)
+    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(value, unsafe_mul(y, y))), 3)
+    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(value, unsafe_mul(y, y))), 3)
+    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(value, unsafe_mul(y, y))), 3)
+    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(value, unsafe_mul(y, y))), 3)
+    y = unsafe_div(unsafe_add(unsafe_mul(2, y), unsafe_div(value, unsafe_mul(y, y))), 3)
 
     # Since we scaled up, we have to scale down accordingly.
     if (x >= unsafe_mul(unsafe_div(max_value(uint256), 10 ** 36), 10 ** 18)):
         return unsafe_mul(y, 10 ** 12)
-    elif x >= unsafe_div(max_value(uint256), 10 ** 36):
+    elif (x >= unsafe_div(max_value(uint256), 10 ** 36)):
         return unsafe_mul(y, 10 ** 6)
     else:
         return y
```

### Comparing `snekmate-0.0.1/src/utils/MerkleProofVerification.vy` & `snekmate-0.0.2/src/utils/MerkleProofVerification.vy`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Merkle Tree Proof Verification Functions
+@custom:contract-name MerkleProofVerification
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice The Merkle tree and the corresponding proofs can be generated
         using the following JavaScript libraries:
         - https://github.com/OpenZeppelin/merkle-tree (recommended),
         - https://github.com/miguelmota/merkletreejs (deprecated).
         If you are using the (deprecated) JavaScript library `merkletreej`
```

### Comparing `snekmate-0.0.1/src/utils/Multicall.vy` & `snekmate-0.0.2/src/utils/Multicall.vy`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title Multicall Functions
+@custom:contract-name Multicall
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice These functions can be used to batch together multiple external
-        function calls into one single external function call.
+        function calls into one single external function call. Please note
+        that this contract is written in the most agnostic way possible and
+        users should adjust statically allocatable memory to their specific
+        needs before deploying it:
+        https://github.com/pcaversaccio/snekmate/discussions/82.
         The implementation is inspired by Matt Solomon's implementation here:
         https://github.com/mds1/multicall/blob/master/src/Multicall3.sol.
 @custom:security Make sure you understand how `msg.sender` works in `CALL` vs
                  `DELEGATECALL` to the multicall contract, as well as the risks
                  of using `msg.value` in a multicall. To learn more about the latter, see:
                  - https://github.com/runtimeverification/verified-smart-contracts/wiki/List-of-Security-Vulnerabilities#payable-multicall,
                  - https://samczsun.com/two-rights-might-make-a-wrong.
@@ -76,20 +81,20 @@
     @return DynArray The array of `Result` structs.
     """
     results: DynArray[Result, max_value(uint8)] = []
     return_data: Bytes[max_value(uint8)] = b""
     success: bool = empty(bool)
     for batch in data:
         if (batch.allow_failure == False):
-            return_data = raw_call(batch.target, batch.call_data, max_outsize=max_value(uint8))
+            return_data = raw_call(batch.target, batch.call_data, max_outsize=255)
             success = True
             results.append(Result({success: success, return_data: return_data}))
         else:
             success, return_data = \
-                raw_call(batch.target, batch.call_data, max_outsize=max_value(uint8), revert_on_failure=False)
+                raw_call(batch.target, batch.call_data, max_outsize=255, revert_on_failure=False)
             results.append(Result({success: success, return_data: return_data}))
     return results
 
 
 @external
 @payable
 def multicall_value(data: DynArray[BatchValue, max_value(uint8)]) -> DynArray[Result, max_value(uint8)]:
@@ -109,20 +114,20 @@
     results: DynArray[Result, max_value(uint8)] = []
     return_data: Bytes[max_value(uint8)] = b""
     success: bool = empty(bool)
     for batch in data:
         msg_value: uint256 = batch.value
         value_accumulator = unsafe_add(value_accumulator, msg_value)
         if (batch.allow_failure == False):
-            return_data = raw_call(batch.target, batch.call_data, max_outsize=max_value(uint8), value=msg_value)
+            return_data = raw_call(batch.target, batch.call_data, max_outsize=255, value=msg_value)
             success = True
             results.append(Result({success: success, return_data: return_data}))
         else:
             success, return_data = \
-                raw_call(batch.target, batch.call_data, max_outsize=max_value(uint8), value=msg_value, revert_on_failure=False)
+                raw_call(batch.target, batch.call_data, max_outsize=255, value=msg_value, revert_on_failure=False)
             results.append(Result({success: success, return_data: return_data}))
     assert msg.value == value_accumulator, "Multicall: value mismatch"
     return results
 
 
 @external
 def multicall_self(data: DynArray[BatchSelf, max_value(uint8)]) -> DynArray[Result, max_value(uint8)]:
@@ -145,20 +150,20 @@
     @return DynArray The array of `Result` structs.
     """
     results: DynArray[Result, max_value(uint8)] = []
     return_data: Bytes[max_value(uint8)] = b""
     success: bool = empty(bool)
     for batch in data:
         if (batch.allow_failure == False):
-            return_data = raw_call(self, batch.call_data, max_outsize=max_value(uint8), is_delegate_call=True)
+            return_data = raw_call(self, batch.call_data, max_outsize=255, is_delegate_call=True)
             success = True
             results.append(Result({success: success, return_data: return_data}))
         else:
             success, return_data = \
-                raw_call(self, batch.call_data, max_outsize=max_value(uint8), is_delegate_call=True, revert_on_failure=False)
+                raw_call(self, batch.call_data, max_outsize=255, is_delegate_call=True, revert_on_failure=False)
             results.append(Result({success: success, return_data: return_data}))
     return results
 
 
 @external
 @payable
 def multicall_value_self(data: DynArray[BatchValueSelf, max_value(uint8)]) -> DynArray[Result, max_value(uint8)]:
@@ -185,20 +190,20 @@
     results: DynArray[Result, max_value(uint8)] = []
     return_data: Bytes[max_value(uint8)] = b""
     success: bool = empty(bool)
     for batch in data:
         msg_value: uint256 = batch.value
         value_accumulator = unsafe_add(value_accumulator, msg_value)
         if (batch.allow_failure == False):
-            return_data = raw_call(self, batch.call_data, max_outsize=max_value(uint8), value=msg_value, is_delegate_call=True)
+            return_data = raw_call(self, batch.call_data, max_outsize=255, value=msg_value, is_delegate_call=True)
             success = True
             results.append(Result({success: success, return_data: return_data}))
         else:
             success, return_data = \
-                raw_call(self, batch.call_data, max_outsize=max_value(uint8), value=msg_value, is_delegate_call=True, revert_on_failure=False)
+                raw_call(self, batch.call_data, max_outsize=255, value=msg_value, is_delegate_call=True, revert_on_failure=False)
             results.append(Result({success: success, return_data: return_data}))
     assert msg.value == value_accumulator, "Multicall: value mismatch"
     return results
 
 
 @external
 @view
@@ -213,15 +218,15 @@
     @return DynArray The array of `Result` structs.
     """
     results: DynArray[Result, max_value(uint8)] = []
     return_data: Bytes[max_value(uint8)] = b""
     success: bool = empty(bool)
     for batch in data:
         if (batch.allow_failure == False):
-            return_data = raw_call(batch.target, batch.call_data, max_outsize=max_value(uint8), is_static_call=True)
+            return_data = raw_call(batch.target, batch.call_data, max_outsize=255, is_static_call=True)
             success = True
             results.append(Result({success: success, return_data: return_data}))
         else:
             success, return_data = \
-                raw_call(batch.target, batch.call_data, max_outsize=max_value(uint8), is_static_call=True, revert_on_failure=False)
+                raw_call(batch.target, batch.call_data, max_outsize=255, is_static_call=True, revert_on_failure=False)
             results.append(Result({success: success, return_data: return_data}))
     return results
```

### Comparing `snekmate-0.0.1/src/utils/SignatureChecker.vy` & `snekmate-0.0.2/src/utils/SignatureChecker.vy`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# @version ^0.3.7
+# @version ^0.3.9
 """
 @title ECDSA and EIP-1271 Signature Verification Functions
+@custom:contract-name SignatureChecker
 @license GNU Affero General Public License v3.0
 @author pcaversaccio
 @notice Signature verification helper functions that can be used
         instead of `ECDSA.recover_sig` to seamlessly support both
         ECDSA signatures from externally-owned accounts (EOAs) as
         well as EIP-1271 (https://eips.ethereum.org/EIPS/eip-1271)
         signatures from smart contract wallets like Argent and Gnosis
@@ -154,17 +155,17 @@
     """
     @dev Sourced from {ECDSA-_try_recover_r_vs}.
     @notice See {ECDSA-_try_recover_r_vs} for the
             function docstring.
     """
     s: uint256 = vs & convert(_SIGNATURE_INCREMENT, uint256)
     # We do not check for an overflow here since the shift operation
-    # `shift(vs, -255)` results essentially in a uint8 type (0 or 1)
-    # and we use uint256 as result type.
-    v: uint256 = unsafe_add(shift(vs, -255), 27)
+    # `vs >> 255` results essentially in a `uint8` type (0 or 1) and
+    # we use `uint256` as result type.
+    v: uint256 = unsafe_add(vs >> 255, 27)
     return self._try_recover_vrs(hash, v, r, s)
 
 
 @internal
 @pure
 def _try_recover_vrs(hash: bytes32, v: uint256, r: uint256, s: uint256) -> address:
     """
```

