# Comparing `tmp/dimplugins-0.1.3.tar.gz` & `tmp/dimplugins-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimplugins-0.1.3.tar", last modified: Sat Jan 21 10:24:39 2023, max compression
+gzip compressed data, was "dist/dimplugins-0.1.4.tar", last modified: Wed Jun  7 17:02:46 2023, max compression
```

## Comparing `dimplugins-0.1.3.tar` & `dimplugins-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-01-21 10:24:39.000000 dimplugins-0.1.3/
--rw-r--r--   0 moky       (501) staff       (20)     1068 2023-01-21 10:24:39.000000 dimplugins-0.1.3/PKG-INFO
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-01-21 10:24:39.000000 dimplugins-0.1.3/dimplugins/
--rw-r--r--   0 moky       (501) staff       (20)     4461 2022-12-11 11:11:29.000000 dimplugins-0.1.3/dimplugins/btc.py
--rw-r--r--   0 moky       (501) staff       (20)     2708 2023-01-20 14:12:57.000000 dimplugins-0.1.3/dimplugins/digest.py
--rw-r--r--   0 moky       (501) staff       (20)     4375 2022-12-11 11:11:47.000000 dimplugins-0.1.3/dimplugins/eth.py
--rw-r--r--   0 moky       (501) staff       (20)     4253 2023-01-21 09:41:52.000000 dimplugins-0.1.3/dimplugins/aes.py
--rw-r--r--   0 moky       (501) staff       (20)     6122 2023-01-21 09:44:04.000000 dimplugins-0.1.3/dimplugins/rsa.py
--rw-r--r--   0 moky       (501) staff       (20)     6017 2023-01-21 07:09:34.000000 dimplugins-0.1.3/dimplugins/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6154 2023-01-21 09:39:36.000000 dimplugins-0.1.3/dimplugins/ecc.py
--rw-r--r--   0 moky       (501) staff       (20)     4852 2023-01-20 08:48:03.000000 dimplugins-0.1.3/dimplugins/keys.py
--rw-r--r--   0 moky       (501) staff       (20)     6204 2023-01-21 09:58:06.000000 dimplugins-0.1.3/dimplugins/factories.py
--rw-r--r--   0 moky       (501) staff       (20)     3287 2023-01-20 14:11:05.000000 dimplugins-0.1.3/dimplugins/coder.py
--rw-r--r--   0 moky       (501) staff       (20)     6189 2022-10-26 10:22:26.000000 dimplugins-0.1.3/dimplugins/network.py
--rw-r--r--   0 moky       (501) staff       (20)     1939 2023-01-21 09:43:16.000000 dimplugins-0.1.3/dimplugins/plain.py
--rw-r--r--   0 moky       (501) staff       (20)     2542 2023-01-20 14:09:05.000000 dimplugins-0.1.3/dimplugins/entity.py
--rw-r--r--   0 moky       (501) staff       (20)     5350 2023-01-20 14:41:04.000000 dimplugins-0.1.3/dimplugins/meta.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-01-21 10:24:39.000000 dimplugins-0.1.3/dimplugins.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1068 2023-01-21 10:24:39.000000 dimplugins-0.1.3/dimplugins.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      466 2023-01-21 10:24:39.000000 dimplugins-0.1.3/dimplugins.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)       63 2023-01-21 10:24:39.000000 dimplugins-0.1.3/dimplugins.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)       11 2023-01-21 10:24:39.000000 dimplugins-0.1.3/dimplugins.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-01-21 10:24:39.000000 dimplugins-0.1.3/dimplugins.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      560 2022-11-08 13:07:00.000000 dimplugins-0.1.3/README.md
--rw-r--r--   0 moky       (501) staff       (20)     1182 2023-01-21 10:11:58.000000 dimplugins-0.1.3/setup.py
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-01-21 10:24:39.000000 dimplugins-0.1.3/setup.cfg
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:02:46.000000 dimplugins-0.1.4/
+-rw-r--r--   0 moky       (501) staff       (20)     1068 2023-06-07 17:02:46.000000 dimplugins-0.1.4/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      560 2022-12-11 05:05:26.000000 dimplugins-0.1.4/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:02:46.000000 dimplugins-0.1.4/dimplugins/
+-rw-r--r--   0 moky       (501) staff       (20)     6017 2023-01-31 05:24:56.000000 dimplugins-0.1.4/dimplugins/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4329 2023-06-01 17:55:02.000000 dimplugins-0.1.4/dimplugins/aes.py
+-rw-r--r--   0 moky       (501) staff       (20)     4379 2023-06-01 18:12:34.000000 dimplugins-0.1.4/dimplugins/btc.py
+-rw-r--r--   0 moky       (501) staff       (20)     3287 2023-01-31 05:24:56.000000 dimplugins-0.1.4/dimplugins/coder.py
+-rw-r--r--   0 moky       (501) staff       (20)     2708 2023-01-31 05:24:56.000000 dimplugins-0.1.4/dimplugins/digest.py
+-rw-r--r--   0 moky       (501) staff       (20)     6154 2023-01-31 05:24:56.000000 dimplugins-0.1.4/dimplugins/ecc.py
+-rw-r--r--   0 moky       (501) staff       (20)     2542 2023-01-31 05:24:56.000000 dimplugins-0.1.4/dimplugins/entity.py
+-rw-r--r--   0 moky       (501) staff       (20)     4375 2022-12-12 09:59:21.000000 dimplugins-0.1.4/dimplugins/eth.py
+-rw-r--r--   0 moky       (501) staff       (20)     6218 2023-06-01 18:17:27.000000 dimplugins-0.1.4/dimplugins/factories.py
+-rw-r--r--   0 moky       (501) staff       (20)     4972 2023-06-01 17:09:25.000000 dimplugins-0.1.4/dimplugins/keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     5350 2023-01-31 05:24:56.000000 dimplugins-0.1.4/dimplugins/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     6189 2022-12-11 05:05:26.000000 dimplugins-0.1.4/dimplugins/network.py
+-rw-r--r--   0 moky       (501) staff       (20)     1939 2023-01-31 05:24:56.000000 dimplugins-0.1.4/dimplugins/plain.py
+-rw-r--r--   0 moky       (501) staff       (20)     6232 2023-06-01 17:58:00.000000 dimplugins-0.1.4/dimplugins/rsa.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:02:46.000000 dimplugins-0.1.4/dimplugins.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1068 2023-06-07 17:02:46.000000 dimplugins-0.1.4/dimplugins.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      466 2023-06-07 17:02:46.000000 dimplugins-0.1.4/dimplugins.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-07 17:02:46.000000 dimplugins-0.1.4/dimplugins.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       63 2023-06-07 17:02:46.000000 dimplugins-0.1.4/dimplugins.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)       11 2023-06-07 17:02:46.000000 dimplugins-0.1.4/dimplugins.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-07 17:02:46.000000 dimplugins-0.1.4/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1182 2023-06-01 17:06:06.000000 dimplugins-0.1.4/setup.py
```

### Comparing `dimplugins-0.1.3/PKG-INFO` & `dimplugins-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimplugins
-Version: 0.1.3
+Version: 0.1.4
 Summary: Decentralized Instant Messaging (Python Plugins)
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python Plugins)
```

### Comparing `dimplugins-0.1.3/dimplugins/btc.py` & `dimplugins-0.1.4/dimplugins/btc.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 # SOFTWARE.
 # ==============================================================================
 
 from typing import Optional, Union
 
 from mkm.types import ConstantString
 from mkm.crypto import base58_encode, base58_decode, sha256, ripemd160
-from mkm.protocol import entity_is_user, entity_is_group
 
 from mkm import Address, EntityType
 
 from .network import NetworkType, network_to_type
 
 
 class BTCAddress(ConstantString, Address):
@@ -67,20 +66,20 @@
     @property  # Override
     def is_broadcast(self) -> bool:
         return False
 
     @property  # Override
     def is_user(self) -> bool:
         network = network_to_type(network=self.type)
-        return entity_is_user(network=network)
+        return EntityType.is_user(network=network)
 
     @property  # Override
     def is_group(self) -> bool:
         network = network_to_type(network=self.type)
-        return entity_is_group(network=network)
+        return EntityType.is_group(network=network)
 
     #
     #   Factory methods
     #
     @classmethod
     def from_data(cls, fingerprint: bytes, network: Union[EntityType, NetworkType, int]) -> Address:
         """
@@ -90,36 +89,38 @@
         :param network:     address type
         :return: Address object
         """
         if isinstance(network, EntityType):
             network = network.value
         elif isinstance(network, NetworkType):
             network = network.value
-        prefix = chr(network).encode('latin1')
-        digest = ripemd160(sha256(fingerprint))
-        code = check_code(prefix + digest)
-        address = base58_encode(prefix + digest + code)
+        head = chr(network).encode('latin1')
+        body = ripemd160(sha256(fingerprint))
+        tail = check_code(head + body)
+        address = base58_encode(head + body + tail)
         return cls(address=address, network=network)
 
     @classmethod
     def from_str(cls, address: str) -> Optional[Address]:
         """
         Parse a string for BTC address
 
         :param address: address string
         :return: Address object
         """
-        prefix_digest_code = base58_decode(address)
-        if len(prefix_digest_code) == 25:
-            # split them
-            prefix = prefix_digest_code[:1]
-            digest = prefix_digest_code[1:-4]
-            code = prefix_digest_code[-4:]
-            # check them
-            if check_code(prefix + digest) == code:
-                network = ord(prefix)
-                return cls(address=address, network=network)
+        if len(address) < 26 or len(address) > 35:
+            return None
+        # decode
+        data = base58_decode(address)
+        if data is None or len(data) != 25:
+            return None
+        # check code
+        prefix = data[:21]
+        suffix = data[21:]
+        if check_code(prefix) == suffix:
+            network = ord(data[:1])
+            return cls(address=address, network=network)
 
 
 def check_code(data: bytes) -> bytes:
     # check code in BTC address
     return sha256(sha256(data))[:4]
```

### Comparing `dimplugins-0.1.3/dimplugins/digest.py` & `dimplugins-0.1.4/dimplugins/digest.py`

 * *Files identical despite different names*

### Comparing `dimplugins-0.1.3/dimplugins/eth.py` & `dimplugins-0.1.4/dimplugins/eth.py`

 * *Files identical despite different names*

### Comparing `dimplugins-0.1.3/dimplugins/aes.py` & `dimplugins-0.1.4/dimplugins/aes.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,17 +94,20 @@
     def encrypt(self, data: bytes) -> bytes:
         data = pkcs7_pad(data=data, block_size=AES.block_size)
         key = AES.new(self.data, AES.MODE_CBC, self.iv)
         return key.encrypt(data)
 
     # Override
     def decrypt(self, data: bytes) -> Optional[bytes]:
-        key = AES.new(self.data, AES.MODE_CBC, self.iv)
-        plaintext = key.decrypt(data)
-        return pkcs7_unpad(data=plaintext)
+        try:
+            key = AES.new(self.data, AES.MODE_CBC, self.iv)
+            plaintext = key.decrypt(data)
+            return pkcs7_unpad(data=plaintext)
+        except ValueError:
+            return None
 
 
 def generate(key_size: int, block_size: int) -> (bytes, bytes):
     data = random_bytes(key_size)
     iv = random_bytes(block_size)
     return data, iv
```

### Comparing `dimplugins-0.1.3/dimplugins/rsa.py` & `dimplugins-0.1.4/dimplugins/rsa.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from Crypto.Hash import SHA256
 from Crypto.PublicKey import RSA
 from Crypto.Cipher import PKCS1_v1_5 as Cipher_PKCS1_v1_5
 from Crypto.Signature import PKCS1_v1_5 as Signature_PKCS1_v1_5
 
 from mkm.crypto import EncryptKey, DecryptKey
 from mkm.crypto import PublicKey
-from mkm.crypto.factory import FactoryManager
+from mkm.crypto.factory import CryptographyKeyFactoryManager
 
 from .keys import BasePublicKey, BasePrivateKey
 
 
 class RSAPublicKey(BasePublicKey, EncryptKey):
     """ RSA Public Key """
 
@@ -77,17 +77,17 @@
     # Override
     def encrypt(self, data: bytes) -> bytes:
         cipher = Cipher_PKCS1_v1_5.new(self.rsa_key)
         return cipher.encrypt(data)
 
     # Override
     def verify(self, data: bytes, signature: bytes) -> bool:
-        hash_obj = SHA256.SHA256Hash(data)
-        verifier = Signature_PKCS1_v1_5.new(self.rsa_key)
         try:
+            hash_obj = SHA256.SHA256Hash(data)
+            verifier = Signature_PKCS1_v1_5.new(self.rsa_key)
             verifier.verify(hash_obj, signature)
             return True
         except ValueError:
             # raise ValueError("Invalid signature")
             return False
 
 
@@ -160,25 +160,28 @@
             'digest': 'SHA256'
         }
         return RSAPublicKey(key=info)
 
     # Override
     # noinspection PyTypeChecker
     def decrypt(self, data: bytes) -> Optional[bytes]:
-        cipher = Cipher_PKCS1_v1_5.new(self.rsa_key)
-        return cipher.decrypt(data, None)
+        try:
+            cipher = Cipher_PKCS1_v1_5.new(self.rsa_key)
+            return cipher.decrypt(data, None)
+        except ValueError:
+            return None
 
     # Override
     def sign(self, data: bytes) -> bytes:
         hash_obj = SHA256.SHA256Hash(data)
         signer = Signature_PKCS1_v1_5.new(self.rsa_key)
         return signer.sign(hash_obj)
 
     # Override
     def match(self, key: EncryptKey) -> bool:
-        gf = FactoryManager.general_factory
+        gf = CryptographyKeyFactoryManager.general_factory
         return gf.keys_match(encrypt_key=key, decrypt_key=self)
 
 
 def generate(bits: int) -> (RSA.RsaKey, bytes):
     key = RSA.generate(bits=bits)
     return key, key.exportKey()
```

### Comparing `dimplugins-0.1.3/dimplugins/__init__.py` & `dimplugins-0.1.4/dimplugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dimplugins-0.1.3/dimplugins/ecc.py` & `dimplugins-0.1.4/dimplugins/ecc.py`

 * *Files identical despite different names*

### Comparing `dimplugins-0.1.3/dimplugins/keys.py` & `dimplugins-0.1.4/dimplugins/keys.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 from abc import ABC
 from typing import Dict, Any
 
 from mkm.types import Dictionary
 from mkm.crypto import CryptographyKey, EncryptKey, SignKey
 from mkm.crypto import SymmetricKey, AsymmetricKey
 from mkm.crypto import PublicKey, PrivateKey
-from mkm.crypto.factory import FactoryManager
+from mkm.crypto.factory import CryptographyKeyFactoryManager
 
 
 class BaseKey(Dictionary, CryptographyKey, ABC):
 
     def __init__(self, key: Dict[str, Any]):
         super().__init__(dictionary=key)
 
     @property  # Override
     def algorithm(self) -> str:
-        gf = FactoryManager.general_factory
+        gf = CryptographyKeyFactoryManager.general_factory
         return gf.get_key_algorithm(key=self.dictionary)
 
 
 class BaseSymmetricKey(Dictionary, SymmetricKey, ABC):
 
     def __init__(self, key: Dict[str, Any]):
         super().__init__(dictionary=key)
@@ -67,47 +67,47 @@
             # check by encryption
             return not self.match(key=other)
         else:
             return True
 
     @property  # Override
     def algorithm(self) -> str:
-        gf = FactoryManager.general_factory
+        gf = CryptographyKeyFactoryManager.general_factory
         return gf.get_key_algorithm(key=self.dictionary)
 
     # Override
     def match(self, key: EncryptKey) -> bool:
-        gf = FactoryManager.general_factory
+        gf = CryptographyKeyFactoryManager.general_factory
         return gf.keys_match(encrypt_key=key, decrypt_key=self)
 
 
 class BaseAsymmetricKey(Dictionary, AsymmetricKey, ABC):
 
     def __init__(self, key: Dict[str, Any]):
         super().__init__(dictionary=key)
 
     @property  # Override
     def algorithm(self) -> str:
-        gf = FactoryManager.general_factory
+        gf = CryptographyKeyFactoryManager.general_factory
         return gf.get_key_algorithm(key=self.dictionary)
 
 
 class BasePublicKey(Dictionary, PublicKey, ABC):
 
     def __init__(self, key: Dict[str, Any]):
         super().__init__(dictionary=key)
 
     @property  # Override
     def algorithm(self) -> str:
-        gf = FactoryManager.general_factory
+        gf = CryptographyKeyFactoryManager.general_factory
         return gf.get_key_algorithm(key=self.dictionary)
 
     # Override
     def match(self, key: SignKey) -> bool:
-        gf = FactoryManager.general_factory
+        gf = CryptographyKeyFactoryManager.general_factory
         return gf.asymmetric_keys_match(sign_key=key, verify_key=self)
 
 
 class BasePrivateKey(Dictionary, PrivateKey, ABC):
 
     def __init__(self, key: Dict[str, Any]):
         super().__init__(dictionary=key)
@@ -134,9 +134,9 @@
             assert verify_key is not None, 'failed to get public key: %s' % self
             return not verify_key.match(key=other)
         else:
             return True
 
     @property  # Override
     def algorithm(self) -> str:
-        gf = FactoryManager.general_factory
+        gf = CryptographyKeyFactoryManager.general_factory
         return gf.get_key_algorithm(key=self.dictionary)
```

### Comparing `dimplugins-0.1.3/dimplugins/factories.py` & `dimplugins-0.1.4/dimplugins/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from typing import Optional, Union
 
 from mkm.crypto import utf8_encode
 from mkm.crypto import SymmetricKey, AsymmetricKey
 from mkm.crypto import SignKey, VerifyKey
 from mkm.crypto import PublicKey, PrivateKey
 from mkm.crypto import SymmetricKeyFactory, PublicKeyFactory, PrivateKeyFactory
-from mkm.factory import FactoryManager
+from mkm.factory import AccountFactoryManager
 
 from mkm import ANYWHERE, EVERYWHERE, Address
 from mkm import MetaType, Meta, MetaFactory
 
 from dimp import BaseAddressFactory
 
 from .rsa import RSAPublicKey, RSAPrivateKey
@@ -157,15 +157,15 @@
             return ETHMeta(version=self.__type, key=key)
         elif self.__type == MetaType.ExETH:
             # ExETH
             return ETHMeta(version=self.__type, key=key, seed=seed, fingerprint=fingerprint)
 
     # Override
     def parse_meta(self, meta: dict) -> Optional[Meta]:
-        gf = FactoryManager.general_factory
+        gf = AccountFactoryManager.general_factory
         version = gf.get_meta_type(meta=meta)
         if version == MetaType.MKM:
             # MKM
             out = DefaultMeta(meta=meta)
         elif version == MetaType.BTC or version == MetaType.ExBTC:
             # BTC, ExBTC
             out = BTCMeta(meta=meta)
```

### Comparing `dimplugins-0.1.3/dimplugins/coder.py` & `dimplugins-0.1.4/dimplugins/coder.py`

 * *Files identical despite different names*

### Comparing `dimplugins-0.1.3/dimplugins/network.py` & `dimplugins-0.1.4/dimplugins/network.py`

 * *Files identical despite different names*

### Comparing `dimplugins-0.1.3/dimplugins/plain.py` & `dimplugins-0.1.4/dimplugins/plain.py`

 * *Files identical despite different names*

### Comparing `dimplugins-0.1.3/dimplugins/entity.py` & `dimplugins-0.1.4/dimplugins/entity.py`

 * *Files identical despite different names*

### Comparing `dimplugins-0.1.3/dimplugins/meta.py` & `dimplugins-0.1.4/dimplugins/meta.py`

 * *Files identical despite different names*

### Comparing `dimplugins-0.1.3/dimplugins.egg-info/PKG-INFO` & `dimplugins-0.1.4/dimplugins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimplugins
-Version: 0.1.3
+Version: 0.1.4
 Summary: Decentralized Instant Messaging (Python Plugins)
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python Plugins)
```

### Comparing `dimplugins-0.1.3/README.md` & `dimplugins-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dimplugins-0.1.3/setup.py` & `dimplugins-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Plugins for MingKeMing module
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -35,16 +35,16 @@
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'dimp>=0.12.6',
-        'dkd>=0.12.6',
-        'mkm>=0.12.6',
+        'dimp>=0.12.8',
+        'dkd>=0.12.7',
+        'mkm>=0.12.7',
 
         'pycryptodome',  # 3.14.1
         'base58',  # 1.0.3
         'ecdsa',   # 0.16.1
     ]
 )
```

