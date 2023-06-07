# Comparing `tmp/autonity-1.0.0-py3-none-any.whl.zip` & `tmp/autonity-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 28044 bytes, number of entries: 31
+Zip file size: 28032 bytes, number of entries: 31
 -rw-r--r--  2.0 unx      530 b- defN 20-Feb-02 00:00 autonity/__init__.py
 -rw-r--r--  2.0 unx       69 b- defN 20-Feb-02 00:00 autonity/__version__.py
 -rw-r--r--  2.0 unx      929 b- defN 20-Feb-02 00:00 autonity/abi_manager.py
 -rw-r--r--  2.0 unx     5768 b- defN 20-Feb-02 00:00 autonity/abi_parser.py
 -rw-r--r--  2.0 unx    13618 b- defN 20-Feb-02 00:00 autonity/autonity.py
 -rw-r--r--  2.0 unx      699 b- defN 20-Feb-02 00:00 autonity/committee_member.py
 -rw-r--r--  2.0 unx     1582 b- defN 20-Feb-02 00:00 autonity/config.py
@@ -22,12 +22,12 @@
 -rw-r--r--  2.0 unx       40 b- defN 20-Feb-02 00:00 autonity/abi/autonity-commit.txt
 -rw-r--r--  2.0 unx       92 b- defN 20-Feb-02 00:00 autonity/abi/solc-version.txt
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 autonity/utils/__init__.py
 -rw-r--r--  2.0 unx     1173 b- defN 20-Feb-02 00:00 autonity/utils/denominations.py
 -rw-r--r--  2.0 unx     1814 b- defN 20-Feb-02 00:00 autonity/utils/keyfile.py
 -rw-r--r--  2.0 unx     5728 b- defN 20-Feb-02 00:00 autonity/utils/tx.py
 -rw-r--r--  2.0 unx     3061 b- defN 20-Feb-02 00:00 autonity/utils/web3.py
-?rw-r--r--  2.0 unx     6928 b- defN 20-Feb-02 00:00 autonity-1.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 autonity-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1065 b- defN 20-Feb-02 00:00 autonity-1.0.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     2461 b- defN 20-Feb-02 00:00 autonity-1.0.0.dist-info/RECORD
-31 files, 97445 bytes uncompressed, 24114 bytes compressed:  75.3%
+?rw-r--r--  2.0 unx     6892 b- defN 20-Feb-02 00:00 autonity-1.0.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 autonity-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1065 b- defN 20-Feb-02 00:00 autonity-1.0.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     2461 b- defN 20-Feb-02 00:00 autonity-1.0.1.dist-info/RECORD
+31 files, 97409 bytes uncompressed, 24102 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -75,20 +75,20 @@
 
 Filename: autonity/utils/tx.py
 Comment: 
 
 Filename: autonity/utils/web3.py
 Comment: 
 
-Filename: autonity-1.0.0.dist-info/METADATA
+Filename: autonity-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: autonity-1.0.0.dist-info/WHEEL
+Filename: autonity-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: autonity-1.0.0.dist-info/licenses/LICENSE
+Filename: autonity-1.0.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: autonity-1.0.0.dist-info/RECORD
+Filename: autonity-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## autonity/__version__.py

```diff
@@ -1,5 +1,5 @@
 """
 Release version of autonity package.
 """
 
-__version__ = "v1.0.0"
+__version__ = "v1.0.1"
```

## Comparing `autonity-1.0.0.dist-info/METADATA` & `autonity-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonity
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library for interacting with Autonity
 License-Expression: MIT
 License-File: LICENSE
 Keywords: autonity,client,library,rpc,web3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 [Autonity](https://autonity.org) is a protocol that provides smart contract and settlement infrastructure specialized for developing new risk markets.  It is a fork of the [Ethereum protocol](https://ethereum.org/).  See the [Autonity documentation](https://docs.autonity.org) for further information.
 
 This package provides typed wrappers around the Autonity-specific extensions of Ethereum, using the [Web3.py](https://github.com/ethereum/web3.py) framework, for convenient and statically checked interactions with the Autonity network.
 
 # Installation
 
 ```console
-pip install git+https://github.com/autonity/autonity.py
+pip install autonity
 ```
 
 # Usage
 
 The primary utility of this library is the typed wrappers around the Autonity protocol contract, which provides access to Autonity-specific functionality.
 
 ```python
@@ -63,15 +63,15 @@
 
 The project uses [hatch](https://hatch.pypa.io/latest/install/#pipx) as build tool.
 
 ## Test and linting
 
 For linting use the command:
 
-```console 
+```console
 make lint
 ```
 
 To run the test with coverage report use the command:
 ```
 make coverage
 ```
```

## Comparing `autonity-1.0.0.dist-info/licenses/LICENSE` & `autonity-1.0.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `autonity-1.0.0.dist-info/RECORD` & `autonity-1.0.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 autonity/__init__.py,sha256=_arYrxLVsIaga7y3TzRM-I44xWF1xo7ZJyTBwaQuYJY,530
-autonity/__version__.py,sha256=umKXolbityZNFFkEP5Eg2YNp8RSsUWB4mT7cmT_pYxU,69
+autonity/__version__.py,sha256=52EN7h0FR_kYN4zUXpljkA7EPVK2fssx64bjNKQnRz8,69
 autonity/abi_manager.py,sha256=ogPaRBb0MaAJ-arsGZZk9C4Zih1EkcGdAAPZOz5ShDI,929
 autonity/abi_parser.py,sha256=0katCkS2t8DOfoOZzPBgwmMfzqtUtsdPXzH_umqnZJM,5768
 autonity/autonity.py,sha256=scq8IrsF7ZGfYUlwcMg7YgnXBY_kkJlrWbqE7HFj64Y,13618
 autonity/committee_member.py,sha256=IyIMqp9yxXOniZlkLsAZnp-y23WobaurFdns_4Xzpx0,699
 autonity/config.py,sha256=HSWUEZHXkk6-rrftFA6HdZ-IfzNevUAk2Pz6L3CJ2JU,1582
 autonity/erc20.py,sha256=DGbmozuM2QDwlcv9V-whHhiq4dH82ErQ8KA8PUBj5wQ,5620
 autonity/liquid_newton.py,sha256=JLI2MamvntQpj6eoVOzk1WlJsovR5iuI72favMUPIfU,1500
@@ -21,11 +21,11 @@
 autonity/abi/autonity-commit.txt,sha256=xWQPY94otC7QPdRYNOHTNJy7-gOpeOuw9GU5RnIholY,40
 autonity/abi/solc-version.txt,sha256=BEwPRa_nyw3CFP5VlCGIazmZefItYDUBddR2lwpeJoM,92
 autonity/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autonity/utils/denominations.py,sha256=gsJme6ZNlCKA073NfBWJ6u0Ka5KZR2M2bxbyoR0wrWk,1173
 autonity/utils/keyfile.py,sha256=HCT8hTlJdF9-j6h5YmYupJjGYiVrpPx4aVNtYaCKzsM,1814
 autonity/utils/tx.py,sha256=fkrYp-GvYZ2AB-bIoqsFBujh30lmMQWUwI1RRyU3s1s,5728
 autonity/utils/web3.py,sha256=U0diDJvK1zX3JrBWCYRJkxwRCDIwLk-O5J50Gydyrhw,3061
-autonity-1.0.0.dist-info/METADATA,sha256=QOe01fMjOxg8vCZ3Leh4q1P4Igmn1mieSscx7yeHkYQ,6928
-autonity-1.0.0.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-autonity-1.0.0.dist-info/licenses/LICENSE,sha256=g9cJ2Md1MlI9a2915dqvKbwFwLAjTCb8gbu00TkEzVc,1065
-autonity-1.0.0.dist-info/RECORD,,
+autonity-1.0.1.dist-info/METADATA,sha256=SULtkhSccmR9PeIaggBQqezhaPLDjYeYKvT-tgyC7YY,6892
+autonity-1.0.1.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+autonity-1.0.1.dist-info/licenses/LICENSE,sha256=g9cJ2Md1MlI9a2915dqvKbwFwLAjTCb8gbu00TkEzVc,1065
+autonity-1.0.1.dist-info/RECORD,,
```

