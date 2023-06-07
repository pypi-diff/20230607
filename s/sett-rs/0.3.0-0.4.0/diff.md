# Comparing `tmp/sett_rs-0.3.0-cp39-none-win_amd64.whl.zip` & `tmp/sett_rs-0.4.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 3593553 bytes, number of entries: 8
--rw-r--r--  4.6 unx     1706 b- defN 23-Apr-18 14:26 sett_rs-0.3.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-18 14:26 sett_rs-0.3.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     2950 b- defN 23-Apr-18 14:26 sett_rs/pgp.py
--rw-r--r--  4.6 unx        0 b- defN 23-Apr-18 14:26 sett_rs/py.typed
--rw-r--r--  4.6 unx     3097 b- defN 23-Apr-18 14:26 sett_rs/_sett_rs.pyi
--rw-r--r--  4.6 unx      236 b- defN 23-Apr-18 14:26 sett_rs/__init__.py
--rwxr-xr-x  4.6 unx  8604160 b- defN 23-Apr-18 14:26 sett_rs/_sett_rs.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      594 b- defN 23-Apr-18 14:26 sett_rs-0.3.0.dist-info/RECORD
-8 files, 8612839 bytes uncompressed, 3592533 bytes compressed:  58.3%
+Zip file size: 5137054 bytes, number of entries: 9
+-rw-r--r--  4.6 unx     1791 b- defN 23-Jun-07 14:49 sett_rs-0.4.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jun-07 14:49 sett_rs-0.4.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx      629 b- defN 23-Jun-07 14:49 sett_rs/cert.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-07 14:49 sett_rs/py.typed
+-rw-r--r--  4.6 unx      487 b- defN 23-Jun-07 14:49 sett_rs/workflow.py
+-rw-r--r--  4.6 unx     5127 b- defN 23-Jun-07 14:49 sett_rs/_sett_rs.pyi
+-rw-r--r--  4.6 unx       84 b- defN 23-Jun-07 14:49 sett_rs/__init__.py
+-rwxr-xr-x  4.6 unx 12137472 b- defN 23-Jun-07 14:49 sett_rs/_sett_rs.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      669 b- defN 23-Jun-07 14:49 sett_rs-0.4.0.dist-info/RECORD
+9 files, 12146353 bytes uncompressed, 5135918 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
-Filename: sett_rs-0.3.0.dist-info/METADATA
+Filename: sett_rs-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: sett_rs-0.3.0.dist-info/WHEEL
+Filename: sett_rs-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: sett_rs/pgp.py
+Filename: sett_rs/cert.py
 Comment: 
 
 Filename: sett_rs/py.typed
 Comment: 
 
+Filename: sett_rs/workflow.py
+Comment: 
+
 Filename: sett_rs/_sett_rs.pyi
 Comment: 
 
 Filename: sett_rs/__init__.py
 Comment: 
 
 Filename: sett_rs/_sett_rs.cp39-win_amd64.pyd
 Comment: 
 
-Filename: sett_rs-0.3.0.dist-info/RECORD
+Filename: sett_rs-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sett_rs/_sett_rs.pyi

```diff
@@ -1,30 +1,32 @@
 """Type hints (stub file) for the classes and functions exported from rust."""
 
 from datetime import datetime
 from enum import Enum
-from typing import Sequence, List, Optional, Callable, Any, Union
+from typing import Any, Callable, List, Optional, Sequence, Union, Tuple
 
 class SftpOpts:
+    base_path: str
     host: str
     port: int
     username: str
-    destination_dir: str
     envelope_dir: Optional[str]
+    filename: Optional[str]
     pkey: Optional[str]
     pkey_password: Optional[str]
     buf_size: Optional[int]
 
     def __init__(
         self,
+        base_path: str,
         host: str,
         port: int,
         username: str,
-        destination_dir: Optional[str] = None,
         envelope_dir: Optional[str] = None,
+        filename: Optional[str] = None,
         pkey: Optional[str] = None,
         pkey_password: Optional[str] = None,
         buf_size: Optional[int] = None,
     ) -> None: ...
 
 class S3Opts:
     endpoint: str
@@ -42,60 +44,115 @@
         region: str = "",
         profile: Optional[str] = None,
         access_key: Optional[str] = None,
         secret_key: Optional[str] = None,
         session_token: Optional[str] = None,
     ) -> None: ...
 
+class CompressionAlgorithm(Enum):
+    Stored: None
+    Gzip: None
+    Zstandard: None
+
+class LocalOpts:
+    output: Optional[str]
+
+    def __init__(self, output: Optional[str] = None) -> None: ...
+
+class EncryptOpts:
+    dry_run: bool
+    files: Sequence[str]
+    force: bool
+    recipients: Sequence[bytes]
+    compression_algorithm: Optional[CompressionAlgorithm]
+    compression_level: Optional[int]
+    max_cpu: Optional[int]
+    password: Optional[str]
+    purpose: Optional[str]
+    signer: Optional[bytes]
+    transfer_id: Optional[int]
+
+    def __init__(
+        self,
+        dry_run: bool,
+        files: Sequence[str],
+        force: bool,
+        recipients: Sequence[bytes],
+        compression_algorithm: Optional[
+            CompressionAlgorithm
+        ] = CompressionAlgorithm.Zstandard,
+        compression_level: Optional[int] = None,
+        max_cpu: Optional[int] = None,
+        password: Optional[str] = None,
+        purpose: Optional[str] = None,
+        signer: Optional[bytes] = None,
+        transfer_id: Optional[int] = None,
+    ) -> None: ...
+
+class DecryptOpts:
+    decrypt_only: bool
+    dry_run: bool
+    file: str
+    recipients: Sequence[bytes]
+    signer: bytes
+    max_cpu: Optional[int]
+    output: Optional[str]
+    password: Optional[str]
+
+    def __init__(
+        self,
+        decrypt_only: bool,
+        dry_run: bool,
+        file: str,
+        recipients: Sequence[bytes],
+        signer: bytes,
+        max_cpu: Optional[int] = None,
+        output: Optional[str] = None,
+        password: Optional[str] = None,
+    ) -> None: ...
+
 def transfer(
     files: Sequence[str],
     destination: Union[S3Opts, SftpOpts],
     progress: Optional[Callable[[float], Any]] = None,
     two_factor_callback: Optional[Callable[[], str]] = None,
 ) -> None: ...
 def encrypt(
-    files: Sequence[str],
-    recipients: Sequence[str],
-    sender: Optional[str],
-    password: Optional[str],
-    dry_run: bool = False,
-    force: bool = False,
-    output: Optional[str] = None,
-    purpose: Optional[str] = None,
-    transfer_id: Optional[int] = None,
-    compression_level: Optional[int] = None,
-    max_cpu: Optional[int] = None,
+    opts: EncryptOpts,
+    destination: Union[SftpOpts, LocalOpts],
     progress: Optional[Callable[[float], Any]] = None,
-    remote: Union[S3Opts, SftpOpts, None] = None,
     two_factor_callback: Optional[Callable[[], str]] = None,
 ) -> Optional[str]: ...
 def decrypt(
-    file: str,
-    recipients: Sequence[str],
-    signer: Optional[str],
-    password: Optional[str],
-    dry_run: bool = False,
-    decrypt_only: bool = False,
-    output: Optional[str] = None,
-    max_cpu: Optional[int] = None,
+    opts: DecryptOpts,
     progress: Optional[Callable[[float], Any]] = None,
 ) -> Optional[str]: ...
 
 class KeyType(Enum):
     Public: Any
     Secret: Any
 
+class CertType(Enum):
+    Public: Any
+    Secret: Any
+
 class Validity(Enum):
     Condemned: Any
     Expired: Any
     Invalid: Any
     Revoked: Any
     Unknown: Any
     Valid: Any
 
+class RevocationReason(Enum):
+    Compromised: Any
+    Superseded: Any
+    Retired: Any
+    Unspecified: Any
+
 class UserID:
     value: bytes
     name: Optional[str]
     email: Optional[str]
     comment: Optional[str]
 
 class Key:
@@ -103,16 +160,35 @@
     key_type: KeyType
     fingerprint: str
     length: Optional[int]
     creation_date: datetime
     expiration_date: Optional[datetime]
     pub_key_algorithm: int
     validity: Validity
+    revocation_reason: Optional[List[str]]
 
-class Cert:
-    key_id: str
+class CertInfo:
+    email: str
     fingerprint: str
+    key_id: str
+    keys: List[Key]
+    primary_key: Key
+    subkeys: List[Key]
+    uid: Optional[UserID]
     uids: List[UserID]
     validity: Validity
-    keys: List[Key]
 
-def read_cert(src: bytes, end_relax: Optional[int]) -> Cert: ...
+    @classmethod
+    def from_bytes(cls, data: bytes, end_relax: Optional[int] = None) -> "CertInfo": ...
+
+def create_revocation_signature(
+    cert: bytes, reason: RevocationReason, message: bytes, password: bytes
+) -> bytes: ...
+def generate_cert(uid: str, password: bytes) -> Tuple[bytes, bytes]: ...
+
+class CertStore:
+    def import_cert(self, cert: bytes, cert_type: CertType) -> CertInfo: ...
+    def export_cert(self, fingerprint: str, cert_type: CertType) -> bytes: ...
+    def list_certs(self, cert_type: CertType) -> List[CertInfo]: ...
+    def revoke(self, rev_sig: bytes) -> None: ...
+
+class CertParsingError(Exception): ...
```

## sett_rs/__init__.py

```diff
@@ -1,10 +1,3 @@
-from ._sett_rs import (
-    decrypt as decrypt,
-    encrypt as encrypt,
-    transfer as transfer,
-    S3Opts as S3Opts,
-    SftpOpts as SftpOpts,
-)
-from . import pgp as pgp
+from . import cert as cert, workflow as workflow
 
-__all__ = ["decrypt", "encrypt", "transfer", "pgp"]
+__all__ = ["cert", "workflow"]
```

## Comparing `sett_rs-0.3.0.dist-info/METADATA` & `sett_rs-0.4.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sett_rs
-Version: 0.3.0
-Requires-Dist: pylint==2.17.2; extra == 'dev'
-Requires-Dist: mypy==1.2.0; extra == 'dev'
-Requires-Dist: black==23.3.0; extra == 'dev'
-Requires-Dist: pytest==7.3.0; extra == 'dev'
+Version: 0.4.0
+Requires-Dist: ruff ==0.0.270 ; extra == 'dev'
+Requires-Dist: mypy ==1.3.0 ; extra == 'dev'
+Requires-Dist: black ==23.3.0 ; extra == 'dev'
+Requires-Dist: pytest ==7.3.1 ; extra == 'dev'
 Provides-Extra: dev
 Summary: sett-rs Python bindings.
-Author: Gerhard Bräunlich <gerhard.braeunlich@id.ethz.ch>, Christian Ribeaud <christian.ribeaud@karakun.com>, Jarosław Surkont <jaroslaw.surkont@unibas.ch>
-Author-email: Gerhard Bräunlich <gerhard.braeunlich@id.ethz.ch>, Christian Ribeaud <christian.ribeaud@karakun.com>, Jarosław Surkont <jaroslaw.surkont@unibas.ch>
+Author: Gerhard Bräunlich <gerhard.braeunlich@id.ethz.ch>, Christian Ribeaud <christian.ribeaud@karakun.com>, Jarosław Surkont <jaroslaw.surkont@unibas.ch>, Simone Guzzi <simone.guzzi@sib.swiss>
+Author-email: Gerhard Bräunlich <gerhard.braeunlich@id.ethz.ch>, Christian Ribeaud <christian.ribeaud@karakun.com>, Jarosław Surkont <jaroslaw.surkont@unibas.ch>, Simone Guzzi <simone.guzzi@sib.swiss>
 License: LGPL-3.0-or-later
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://gitlab.com/biomedit/sett-rs
 
 # sett-rs Python bindings
 
 Building sett-rs Python bindings requires the
```

