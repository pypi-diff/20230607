# Comparing `tmp/alibabacloud-dkms-gcs-python2-0.0.5.tar.gz` & `tmp/alibabacloud-dkms-gcs-python2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud-dkms-gcs-python2-0.0.5.tar", last modified: Fri Aug  5 06:20:17 2022, max compression
+gzip compressed data, was "dist/alibabacloud-dkms-gcs-python2-0.0.6.tar", last modified: Wed Jun  7 13:46:58 2023, max compression
```

## Comparing `alibabacloud-dkms-gcs-python2-0.0.5.tar` & `alibabacloud-dkms-gcs-python2-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     1616 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      655 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/alibabacloud_dkms_gcs_python2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1616 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/alibabacloud_dkms_gcs_python2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      840 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/alibabacloud_dkms_gcs_python2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/alibabacloud_dkms_gcs_python2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/alibabacloud_dkms_gcs_python2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/alibabacloud_dkms_gcs_python2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi/
--rw-r--r--   0 root         (0) root         (0)       22 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8395 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi/client.py
--rw-r--r--   0 root         (0) root         (0)     5688 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/
--rw-r--r--   0 root         (0) root         (0)       22 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/auth/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      619 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/auth/credentials.py
--rw-r--r--   0 root         (0) root         (0)     2004 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/auth/signer.py
--rw-r--r--   0 root         (0) root         (0)     1964 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/client.py
--rw-r--r--   0 root         (0) root         (0)     2922 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      688 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/utils/credential_utils.py
--rw-r--r--   0 root         (0) root         (0)      197 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/utils/json_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_util/
--rw-r--r--   0 root         (0) root         (0)       22 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_util/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16571 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_util/client.py
--rw-r--r--   0 root         (0) root         (0)     5798 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_util/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_util/protobuf/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_util/protobuf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69032 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/openapi_util/protobuf/api_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/sdk/
--rw-r--r--   0 root         (0) root         (0)       22 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12588 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/sdk/client.py
--rw-r--r--   0 root         (0) root         (0)    27581 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/sdk/models.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1504 2022-08-05 06:20:17.000000 alibabacloud-dkms-gcs-python2-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      656 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/alibabacloud_dkms_gcs_python2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/alibabacloud_dkms_gcs_python2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      840 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/alibabacloud_dkms_gcs_python2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/alibabacloud_dkms_gcs_python2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/alibabacloud_dkms_gcs_python2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/alibabacloud_dkms_gcs_python2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8395 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi/client.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/auth/credentials.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/auth/signer.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/client.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      688 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/utils/credential_utils.py
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/utils/json_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_util/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21120 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_util/client.py
+-rw-r--r--   0 root         (0) root         (0)     5798 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_util/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_util/protobuf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_util/protobuf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91100 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/openapi_util/protobuf/api_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/sdk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16999 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/sdk/client.py
+-rw-r--r--   0 root         (0) root         (0)    38150 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/sdk/models.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-06-07 13:46:58.000000 alibabacloud-dkms-gcs-python2-0.0.6/setup.py
```

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/PKG-INFO` & `alibabacloud-dkms-gcs-python2-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: alibabacloud-dkms-gcs-python2
-Version: 0.0.5
+Version: 0.0.6
 Summary: AlibabaCloud DKMS-GCS SDK for Python2
 Home-page: https://github.com/aliyun/alibabacloud-dkms-gcs-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
-Description: English \| `简体中文 <README-CN.md>`__
+Description: English \| `简体中文 <README-CN.rst>`__
         
         |image0|
         
         AlibabaCloud DKMS-GCS SDK for Python
         ------------------------------------
         
         -  `Overview <https://www.alibabacloud.com/help/doc-detail/311016.htm>`__
```

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/README.rst` & `alibabacloud-dkms-gcs-python2-0.0.6/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-English \| `简体中文 <README-CN.md>`__
+English \| `简体中文 <README-CN.rst>`__
 
 |image0|
 
 AlibabaCloud DKMS-GCS SDK for Python
 ------------------------------------
 
 -  `Overview <https://www.alibabacloud.com/help/doc-detail/311016.htm>`__
```

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/alibabacloud_dkms_gcs_python2.egg-info/PKG-INFO` & `alibabacloud-dkms-gcs-python2-0.0.6/alibabacloud_dkms_gcs_python2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: alibabacloud-dkms-gcs-python2
-Version: 0.0.5
+Version: 0.0.6
 Summary: AlibabaCloud DKMS-GCS SDK for Python2
 Home-page: https://github.com/aliyun/alibabacloud-dkms-gcs-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
-Description: English \| `简体中文 <README-CN.md>`__
+Description: English \| `简体中文 <README-CN.rst>`__
         
         |image0|
         
         AlibabaCloud DKMS-GCS SDK for Python
         ------------------------------------
         
         -  `Overview <https://www.alibabacloud.com/help/doc-detail/311016.htm>`__
```

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/alibabacloud_dkms_gcs_python2.egg-info/SOURCES.txt` & `alibabacloud-dkms-gcs-python2-0.0.6/alibabacloud_dkms_gcs_python2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/openapi/client.py` & `alibabacloud-dkms-gcs-python2-0.0.6/openapi/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/openapi/models.py` & `alibabacloud-dkms-gcs-python2-0.0.6/openapi/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/auth/credentials.py` & `alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/auth/signer.py` & `alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/auth/signer.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/client.py` & `alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/models.py` & `alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/openapi_credential/utils/credential_utils.py` & `alibabacloud-dkms-gcs-python2-0.0.6/openapi_credential/utils/credential_utils.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/openapi_util/client.py` & `alibabacloud-dkms-gcs-python2-0.0.6/openapi_util/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -478,7 +478,108 @@
         result["LastRotationDate"] = get_secret_value_response.LastRotationDate
         result["NextRotationDate"] = get_secret_value_response.NextRotationDate
         result["ExtendedConfig"] = get_secret_value_response.ExtendedConfig
         result["AutomaticRotation"] = get_secret_value_response.AutomaticRotation
         result["RotationInterval"] = get_secret_value_response.RotationInterval
         result["RequestId"] = get_secret_value_response.RequestId
         return result
+
+    @staticmethod
+    def get_serialized_advance_encrypt_request(req_body):
+        advance_encrypt_request = api_pb2.AdvanceEncryptRequest()
+        key_id = req_body.get("KeyId")
+        if key_id:
+            advance_encrypt_request.KeyId = key_id
+        plaintext = req_body.get("Plaintext")
+        if plaintext:
+            advance_encrypt_request.Plaintext = plaintext
+        algorithm = req_body.get("Algorithm")
+        if algorithm:
+            advance_encrypt_request.Algorithm = algorithm
+        iv = req_body.get("Iv")
+        if iv:
+            advance_encrypt_request.Iv = iv
+        aad = req_body.get("Aad")
+        if aad:
+            advance_encrypt_request.Aad = aad
+        padding_mode = req_body.get("PaddingMode")
+        if padding_mode:
+            advance_encrypt_request.PaddingMode = padding_mode
+        return advance_encrypt_request.SerializeToString()
+
+    @staticmethod
+    def parse_advance_encrypt_response(res_body):
+        result = {}
+        advance_encrypt_response = api_pb2.AdvanceEncryptResponse()
+        advance_encrypt_response.ParseFromString(res_body)
+        result["KeyId"] = advance_encrypt_response.KeyId
+        result["CiphertextBlob"] = advance_encrypt_response.CiphertextBlob
+        result["Iv"] = advance_encrypt_response.Iv
+        result["Algorithm"] = advance_encrypt_response.Algorithm
+        result["PaddingMode"] = advance_encrypt_response.PaddingMode
+        result["KeyVersionId"] = advance_encrypt_response.KeyVersionId
+        result["RequestId"] = advance_encrypt_response.RequestId
+        return result
+
+    @staticmethod
+    def get_serialized_advance_decrypt_request(req_body):
+        advance_decrypt_request = api_pb2.AdvanceDecryptRequest()
+        key_id = req_body.get("KeyId")
+        if key_id:
+            advance_decrypt_request.KeyId = key_id
+        ciphertext_blob = req_body.get("CiphertextBlob")
+        if ciphertext_blob:
+            advance_decrypt_request.CiphertextBlob = ciphertext_blob
+        algorithm = req_body.get("Algorithm")
+        if algorithm:
+            advance_decrypt_request.Algorithm = algorithm
+        iv = req_body.get("Iv")
+        if iv:
+            advance_decrypt_request.Iv = iv
+        aad = req_body.get("Aad")
+        if aad:
+            advance_decrypt_request.Aad = aad
+        padding_mode = req_body.get("PaddingMode")
+        if padding_mode:
+            advance_decrypt_request.PaddingMode = padding_mode
+        return advance_decrypt_request.SerializeToString()
+
+    @staticmethod
+    def parse_advance_decrypt_response(res_body):
+        result = {}
+        advance_decrypt_response = api_pb2.AdvanceDecryptResponse()
+        advance_decrypt_response.ParseFromString(res_body)
+        result["KeyId"] = advance_decrypt_response.KeyId
+        result["Plaintext"] = advance_decrypt_response.Plaintext
+        result["Algorithm"] = advance_decrypt_response.Algorithm
+        result["PaddingMode"] = advance_decrypt_response.PaddingMode
+        result["KeyVersionId"] = advance_decrypt_response.KeyVersionId
+        result["RequestId"] = advance_decrypt_response.RequestId
+        return result
+
+    @staticmethod
+    def get_serialized_advance_generate_data_key_request(req_body):
+        advance_generate_data_key_request = api_pb2.AdvanceGenerateDataKeyRequest()
+        key_id = req_body.get("KeyId")
+        if key_id:
+            advance_generate_data_key_request.KeyId = key_id
+        number_of_bytes = req_body.get("NumberOfBytes")
+        if number_of_bytes:
+            advance_generate_data_key_request.NumberOfBytes = number_of_bytes
+        aad = req_body.get("Aad")
+        if aad:
+            advance_generate_data_key_request.Aad = aad
+        return advance_generate_data_key_request.SerializeToString()
+
+    @staticmethod
+    def parse_advance_generate_data_key_response(res_body):
+        result = {}
+        advance_generate_data_key_response = api_pb2.AdvanceGenerateDataKeyResponse()
+        advance_generate_data_key_response.ParseFromString(res_body)
+        result["KeyId"] = advance_generate_data_key_response.KeyId
+        result["Iv"] = advance_generate_data_key_response.Iv
+        result["Plaintext"] = advance_generate_data_key_response.Plaintext
+        result["CiphertextBlob"] = advance_generate_data_key_response.CiphertextBlob
+        result["Algorithm"] = advance_generate_data_key_response.Algorithm
+        result["KeyVersionId"] = advance_generate_data_key_response.KeyVersionId
+        result["RequestId"] = advance_generate_data_key_response.RequestId
+        return result
```

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/openapi_util/models.py` & `alibabacloud-dkms-gcs-python2-0.0.6/openapi_util/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/openapi_util/protobuf/api_pb2.py` & `alibabacloud-dkms-gcs-python2-0.0.6/openapi_util/protobuf/api_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='api.proto',
   package='protobuf',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\tapi.proto\x12\x08protobuf\"B\n\x11KmsEncryptRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPlaintext\x18\x02 \x01(\x0c\x12\x0b\n\x03\x41\x61\x64\x18\x03 \x01(\x0c\"N\n\x12KmsEncryptResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x16\n\x0e\x43iphertextBlob\x18\x02 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\"s\n\x0e\x45ncryptRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPlaintext\x18\x02 \x01(\x0c\x12\x11\n\tAlgorithm\x18\x03 \x01(\t\x12\x0b\n\x03\x41\x61\x64\x18\x04 \x01(\x0c\x12\n\n\x02Iv\x18\x05 \x01(\x0c\x12\x13\n\x0bPaddingMode\x18\x06 \x01(\t\"\x7f\n\x0f\x45ncryptResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x16\n\x0e\x43iphertextBlob\x18\x02 \x01(\x0c\x12\n\n\x02Iv\x18\x03 \x01(\x0c\x12\x11\n\tRequestId\x18\x04 \x01(\t\x12\x11\n\tAlgorithm\x18\x05 \x01(\t\x12\x13\n\x0bPaddingMode\x18\x06 \x01(\t\"8\n\x11KmsDecryptRequest\x12\x16\n\x0e\x43iphertextBlob\x18\x01 \x01(\x0c\x12\x0b\n\x03\x41\x61\x64\x18\x02 \x01(\x0c\"I\n\x12KmsDecryptResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPlaintext\x18\x02 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\"x\n\x0e\x44\x65\x63ryptRequest\x12\x16\n\x0e\x43iphertextBlob\x18\x01 \x01(\x0c\x12\r\n\x05KeyId\x18\x02 \x01(\t\x12\x11\n\tAlgorithm\x18\x03 \x01(\t\x12\x0b\n\x03\x41\x61\x64\x18\x04 \x01(\x0c\x12\n\n\x02Iv\x18\x05 \x01(\x0c\x12\x13\n\x0bPaddingMode\x18\x06 \x01(\t\"n\n\x0f\x44\x65\x63ryptResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPlaintext\x18\x02 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\x12\x11\n\tAlgorithm\x18\x04 \x01(\t\x12\x13\n\x0bPaddingMode\x18\x05 \x01(\t\"e\n\x0bSignRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x0e\n\x06\x44igest\x18\x02 \x01(\x0c\x12\x11\n\tAlgorithm\x18\x03 \x01(\t\x12\x0f\n\x07Message\x18\x04 \x01(\x0c\x12\x13\n\x0bMessageType\x18\x05 \x01(\t\"k\n\x0cSignResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tSignature\x18\x02 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\x12\x11\n\tAlgorithm\x18\x04 \x01(\t\x12\x13\n\x0bMessageType\x18\x05 \x01(\t\"z\n\rVerifyRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x0e\n\x06\x44igest\x18\x02 \x01(\x0c\x12\x11\n\tSignature\x18\x03 \x01(\x0c\x12\x11\n\tAlgorithm\x18\x04 \x01(\t\x12\x0f\n\x07Message\x18\x05 \x01(\x0c\x12\x13\n\x0bMessageType\x18\x06 \x01(\t\"i\n\x0eVerifyResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\r\n\x05Value\x18\x02 \x01(\x08\x12\x11\n\tRequestId\x18\x03 \x01(\t\x12\x11\n\tAlgorithm\x18\x04 \x01(\t\x12\x13\n\x0bMessageType\x18\x05 \x01(\t\"-\n\x0bHmacRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x0f\n\x07Message\x18\x02 \x01(\x0c\"C\n\x0cHmacResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tSignature\x18\x02 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\"\'\n\x15GenerateRandomRequest\x12\x0e\n\x06Length\x18\x01 \x01(\x05\";\n\x16GenerateRandomResponse\x12\x0e\n\x06Random\x18\x01 \x01(\x0c\x12\x11\n\tRequestId\x18\x02 \x01(\t\"1\n\x0bHashRequest\x12\x0f\n\x07Message\x18\x01 \x01(\x0c\x12\x11\n\tAlgorithm\x18\x02 \x01(\t\"1\n\x0cHashResponse\x12\x0e\n\x06\x44igest\x18\x01 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\"^\n\x16GenerateDataKeyRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tAlgorithm\x18\x02 \x01(\t\x12\x15\n\rNumberOfBytes\x18\x03 \x01(\x05\x12\x0b\n\x03\x41\x61\x64\x18\x04 \x01(\x0c\"\x85\x01\n\x17GenerateDataKeyResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\n\n\x02Iv\x18\x02 \x01(\x0c\x12\x11\n\tPlaintext\x18\x03 \x01(\x0c\x12\x16\n\x0e\x43iphertextBlob\x18\x04 \x01(\x0c\x12\x11\n\tRequestId\x18\x05 \x01(\t\x12\x11\n\tAlgorithm\x18\x06 \x01(\t\"$\n\x13GetPublicKeyRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\"K\n\x14GetPublicKeyResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPublicKey\x18\x02 \x01(\t\x12\x11\n\tRequestId\x18\x03 \x01(\t\"W\n\x05\x45rror\x12\x12\n\nStatusCode\x18\x01 \x01(\x05\x12\x11\n\tErrorCode\x18\x02 \x01(\t\x12\x14\n\x0c\x45rrorMessage\x18\x03 \x01(\t\x12\x11\n\tRequestId\x18\x04 \x01(\t\"q\n\x15GetSecretValueRequest\x12\x12\n\nSecretName\x18\x01 \x01(\t\x12\x14\n\x0cVersionStage\x18\x02 \x01(\t\x12\x11\n\tVersionId\x18\x03 \x01(\t\x12\x1b\n\x13\x46\x65tchExtendedConfig\x18\x04 \x01(\x08\"\xbe\x02\n\x16GetSecretValueResponse\x12\x12\n\nSecretName\x18\x01 \x01(\t\x12\x12\n\nSecretType\x18\x02 \x01(\t\x12\x12\n\nSecretData\x18\x03 \x01(\t\x12\x16\n\x0eSecretDataType\x18\x04 \x01(\t\x12\x15\n\rVersionStages\x18\x05 \x03(\t\x12\x11\n\tVersionId\x18\x06 \x01(\t\x12\x12\n\nCreateTime\x18\x07 \x01(\t\x12\x11\n\tRequestId\x18\x08 \x01(\t\x12\x18\n\x10LastRotationDate\x18\t \x01(\t\x12\x18\n\x10NextRotationDate\x18\n \x01(\t\x12\x16\n\x0e\x45xtendedConfig\x18\x0b \x01(\t\x12\x19\n\x11\x41utomaticRotation\x18\x0c \x01(\t\x12\x18\n\x10RotationInterval\x18\r \x01(\tb\x06proto3'
+  serialized_pb=b'\n\tapi.proto\x12\x08protobuf\"B\n\x11KmsEncryptRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPlaintext\x18\x02 \x01(\x0c\x12\x0b\n\x03\x41\x61\x64\x18\x03 \x01(\x0c\"N\n\x12KmsEncryptResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x16\n\x0e\x43iphertextBlob\x18\x02 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\"s\n\x0e\x45ncryptRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPlaintext\x18\x02 \x01(\x0c\x12\x11\n\tAlgorithm\x18\x03 \x01(\t\x12\x0b\n\x03\x41\x61\x64\x18\x04 \x01(\x0c\x12\n\n\x02Iv\x18\x05 \x01(\x0c\x12\x13\n\x0bPaddingMode\x18\x06 \x01(\t\"\x7f\n\x0f\x45ncryptResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x16\n\x0e\x43iphertextBlob\x18\x02 \x01(\x0c\x12\n\n\x02Iv\x18\x03 \x01(\x0c\x12\x11\n\tRequestId\x18\x04 \x01(\t\x12\x11\n\tAlgorithm\x18\x05 \x01(\t\x12\x13\n\x0bPaddingMode\x18\x06 \x01(\t\"8\n\x11KmsDecryptRequest\x12\x16\n\x0e\x43iphertextBlob\x18\x01 \x01(\x0c\x12\x0b\n\x03\x41\x61\x64\x18\x02 \x01(\x0c\"I\n\x12KmsDecryptResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPlaintext\x18\x02 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\"x\n\x0e\x44\x65\x63ryptRequest\x12\x16\n\x0e\x43iphertextBlob\x18\x01 \x01(\x0c\x12\r\n\x05KeyId\x18\x02 \x01(\t\x12\x11\n\tAlgorithm\x18\x03 \x01(\t\x12\x0b\n\x03\x41\x61\x64\x18\x04 \x01(\x0c\x12\n\n\x02Iv\x18\x05 \x01(\x0c\x12\x13\n\x0bPaddingMode\x18\x06 \x01(\t\"n\n\x0f\x44\x65\x63ryptResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPlaintext\x18\x02 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\x12\x11\n\tAlgorithm\x18\x04 \x01(\t\x12\x13\n\x0bPaddingMode\x18\x05 \x01(\t\"e\n\x0bSignRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x0e\n\x06\x44igest\x18\x02 \x01(\x0c\x12\x11\n\tAlgorithm\x18\x03 \x01(\t\x12\x0f\n\x07Message\x18\x04 \x01(\x0c\x12\x13\n\x0bMessageType\x18\x05 \x01(\t\"k\n\x0cSignResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tSignature\x18\x02 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\x12\x11\n\tAlgorithm\x18\x04 \x01(\t\x12\x13\n\x0bMessageType\x18\x05 \x01(\t\"z\n\rVerifyRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x0e\n\x06\x44igest\x18\x02 \x01(\x0c\x12\x11\n\tSignature\x18\x03 \x01(\x0c\x12\x11\n\tAlgorithm\x18\x04 \x01(\t\x12\x0f\n\x07Message\x18\x05 \x01(\x0c\x12\x13\n\x0bMessageType\x18\x06 \x01(\t\"i\n\x0eVerifyResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\r\n\x05Value\x18\x02 \x01(\x08\x12\x11\n\tRequestId\x18\x03 \x01(\t\x12\x11\n\tAlgorithm\x18\x04 \x01(\t\x12\x13\n\x0bMessageType\x18\x05 \x01(\t\"-\n\x0bHmacRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x0f\n\x07Message\x18\x02 \x01(\x0c\"C\n\x0cHmacResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tSignature\x18\x02 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\"\'\n\x15GenerateRandomRequest\x12\x0e\n\x06Length\x18\x01 \x01(\x05\";\n\x16GenerateRandomResponse\x12\x0e\n\x06Random\x18\x01 \x01(\x0c\x12\x11\n\tRequestId\x18\x02 \x01(\t\"1\n\x0bHashRequest\x12\x0f\n\x07Message\x18\x01 \x01(\x0c\x12\x11\n\tAlgorithm\x18\x02 \x01(\t\"1\n\x0cHashResponse\x12\x0e\n\x06\x44igest\x18\x01 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\"^\n\x16GenerateDataKeyRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tAlgorithm\x18\x02 \x01(\t\x12\x15\n\rNumberOfBytes\x18\x03 \x01(\x05\x12\x0b\n\x03\x41\x61\x64\x18\x04 \x01(\x0c\"\x85\x01\n\x17GenerateDataKeyResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\n\n\x02Iv\x18\x02 \x01(\x0c\x12\x11\n\tPlaintext\x18\x03 \x01(\x0c\x12\x16\n\x0e\x43iphertextBlob\x18\x04 \x01(\x0c\x12\x11\n\tRequestId\x18\x05 \x01(\t\x12\x11\n\tAlgorithm\x18\x06 \x01(\t\"$\n\x13GetPublicKeyRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\"K\n\x14GetPublicKeyResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPublicKey\x18\x02 \x01(\t\x12\x11\n\tRequestId\x18\x03 \x01(\t\"W\n\x05\x45rror\x12\x12\n\nStatusCode\x18\x01 \x01(\x05\x12\x11\n\tErrorCode\x18\x02 \x01(\t\x12\x14\n\x0c\x45rrorMessage\x18\x03 \x01(\t\x12\x11\n\tRequestId\x18\x04 \x01(\t\"q\n\x15GetSecretValueRequest\x12\x12\n\nSecretName\x18\x01 \x01(\t\x12\x14\n\x0cVersionStage\x18\x02 \x01(\t\x12\x11\n\tVersionId\x18\x03 \x01(\t\x12\x1b\n\x13\x46\x65tchExtendedConfig\x18\x04 \x01(\x08\"\xbe\x02\n\x16GetSecretValueResponse\x12\x12\n\nSecretName\x18\x01 \x01(\t\x12\x12\n\nSecretType\x18\x02 \x01(\t\x12\x12\n\nSecretData\x18\x03 \x01(\t\x12\x16\n\x0eSecretDataType\x18\x04 \x01(\t\x12\x15\n\rVersionStages\x18\x05 \x03(\t\x12\x11\n\tVersionId\x18\x06 \x01(\t\x12\x12\n\nCreateTime\x18\x07 \x01(\t\x12\x11\n\tRequestId\x18\x08 \x01(\t\x12\x18\n\x10LastRotationDate\x18\t \x01(\t\x12\x18\n\x10NextRotationDate\x18\n \x01(\t\x12\x16\n\x0e\x45xtendedConfig\x18\x0b \x01(\t\x12\x19\n\x11\x41utomaticRotation\x18\x0c \x01(\t\x12\x18\n\x10RotationInterval\x18\r \x01(\t\"z\n\x15\x41\x64vanceEncryptRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPlaintext\x18\x02 \x01(\x0c\x12\x11\n\tAlgorithm\x18\x03 \x01(\t\x12\x0b\n\x03\x41\x61\x64\x18\x04 \x01(\x0c\x12\n\n\x02Iv\x18\x05 \x01(\x0c\x12\x13\n\x0bPaddingMode\x18\x06 \x01(\t\"\x9c\x01\n\x16\x41\x64vanceEncryptResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x16\n\x0e\x43iphertextBlob\x18\x02 \x01(\x0c\x12\n\n\x02Iv\x18\x03 \x01(\x0c\x12\x11\n\tRequestId\x18\x04 \x01(\t\x12\x11\n\tAlgorithm\x18\x05 \x01(\t\x12\x13\n\x0bPaddingMode\x18\x06 \x01(\t\x12\x14\n\x0cKeyVersionId\x18\x07 \x01(\t\"\x7f\n\x15\x41\x64vanceDecryptRequest\x12\x16\n\x0e\x43iphertextBlob\x18\x01 \x01(\x0c\x12\r\n\x05KeyId\x18\x02 \x01(\t\x12\x11\n\tAlgorithm\x18\x03 \x01(\t\x12\x0b\n\x03\x41\x61\x64\x18\x04 \x01(\x0c\x12\n\n\x02Iv\x18\x05 \x01(\x0c\x12\x13\n\x0bPaddingMode\x18\x06 \x01(\t\"\x8b\x01\n\x16\x41\x64vanceDecryptResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x11\n\tPlaintext\x18\x02 \x01(\x0c\x12\x11\n\tRequestId\x18\x03 \x01(\t\x12\x11\n\tAlgorithm\x18\x04 \x01(\t\x12\x13\n\x0bPaddingMode\x18\x05 \x01(\t\x12\x14\n\x0cKeyVersionId\x18\x06 \x01(\t\"R\n\x1d\x41\x64vanceGenerateDataKeyRequest\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\x15\n\rNumberOfBytes\x18\x02 \x01(\x05\x12\x0b\n\x03\x41\x61\x64\x18\x03 \x01(\x0c\"\xa2\x01\n\x1e\x41\x64vanceGenerateDataKeyResponse\x12\r\n\x05KeyId\x18\x01 \x01(\t\x12\n\n\x02Iv\x18\x02 \x01(\x0c\x12\x11\n\tPlaintext\x18\x03 \x01(\x0c\x12\x16\n\x0e\x43iphertextBlob\x18\x04 \x01(\x0c\x12\x11\n\tRequestId\x18\x05 \x01(\t\x12\x11\n\tAlgorithm\x18\x06 \x01(\t\x12\x14\n\x0cKeyVersionId\x18\x07 \x01(\tb\x06proto3'
 )
 
 
 
 
 _KMSENCRYPTREQUEST = _descriptor.Descriptor(
   name='KmsEncryptRequest',
@@ -1359,14 +1359,409 @@
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=2099,
   serialized_end=2417,
 )
 
+
+_ADVANCEENCRYPTREQUEST = _descriptor.Descriptor(
+  name='AdvanceEncryptRequest',
+  full_name='protobuf.AdvanceEncryptRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='KeyId', full_name='protobuf.AdvanceEncryptRequest.KeyId', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Plaintext', full_name='protobuf.AdvanceEncryptRequest.Plaintext', index=1,
+      number=2, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Algorithm', full_name='protobuf.AdvanceEncryptRequest.Algorithm', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Aad', full_name='protobuf.AdvanceEncryptRequest.Aad', index=3,
+      number=4, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Iv', full_name='protobuf.AdvanceEncryptRequest.Iv', index=4,
+      number=5, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='PaddingMode', full_name='protobuf.AdvanceEncryptRequest.PaddingMode', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2419,
+  serialized_end=2541,
+)
+
+
+_ADVANCEENCRYPTRESPONSE = _descriptor.Descriptor(
+  name='AdvanceEncryptResponse',
+  full_name='protobuf.AdvanceEncryptResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='KeyId', full_name='protobuf.AdvanceEncryptResponse.KeyId', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='CiphertextBlob', full_name='protobuf.AdvanceEncryptResponse.CiphertextBlob', index=1,
+      number=2, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Iv', full_name='protobuf.AdvanceEncryptResponse.Iv', index=2,
+      number=3, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='RequestId', full_name='protobuf.AdvanceEncryptResponse.RequestId', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Algorithm', full_name='protobuf.AdvanceEncryptResponse.Algorithm', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='PaddingMode', full_name='protobuf.AdvanceEncryptResponse.PaddingMode', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='KeyVersionId', full_name='protobuf.AdvanceEncryptResponse.KeyVersionId', index=6,
+      number=7, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2544,
+  serialized_end=2700,
+)
+
+
+_ADVANCEDECRYPTREQUEST = _descriptor.Descriptor(
+  name='AdvanceDecryptRequest',
+  full_name='protobuf.AdvanceDecryptRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='CiphertextBlob', full_name='protobuf.AdvanceDecryptRequest.CiphertextBlob', index=0,
+      number=1, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='KeyId', full_name='protobuf.AdvanceDecryptRequest.KeyId', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Algorithm', full_name='protobuf.AdvanceDecryptRequest.Algorithm', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Aad', full_name='protobuf.AdvanceDecryptRequest.Aad', index=3,
+      number=4, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Iv', full_name='protobuf.AdvanceDecryptRequest.Iv', index=4,
+      number=5, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='PaddingMode', full_name='protobuf.AdvanceDecryptRequest.PaddingMode', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2702,
+  serialized_end=2829,
+)
+
+
+_ADVANCEDECRYPTRESPONSE = _descriptor.Descriptor(
+  name='AdvanceDecryptResponse',
+  full_name='protobuf.AdvanceDecryptResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='KeyId', full_name='protobuf.AdvanceDecryptResponse.KeyId', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Plaintext', full_name='protobuf.AdvanceDecryptResponse.Plaintext', index=1,
+      number=2, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='RequestId', full_name='protobuf.AdvanceDecryptResponse.RequestId', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Algorithm', full_name='protobuf.AdvanceDecryptResponse.Algorithm', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='PaddingMode', full_name='protobuf.AdvanceDecryptResponse.PaddingMode', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='KeyVersionId', full_name='protobuf.AdvanceDecryptResponse.KeyVersionId', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2832,
+  serialized_end=2971,
+)
+
+
+_ADVANCEGENERATEDATAKEYREQUEST = _descriptor.Descriptor(
+  name='AdvanceGenerateDataKeyRequest',
+  full_name='protobuf.AdvanceGenerateDataKeyRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='KeyId', full_name='protobuf.AdvanceGenerateDataKeyRequest.KeyId', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='NumberOfBytes', full_name='protobuf.AdvanceGenerateDataKeyRequest.NumberOfBytes', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Aad', full_name='protobuf.AdvanceGenerateDataKeyRequest.Aad', index=2,
+      number=3, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2973,
+  serialized_end=3055,
+)
+
+
+_ADVANCEGENERATEDATAKEYRESPONSE = _descriptor.Descriptor(
+  name='AdvanceGenerateDataKeyResponse',
+  full_name='protobuf.AdvanceGenerateDataKeyResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='KeyId', full_name='protobuf.AdvanceGenerateDataKeyResponse.KeyId', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Iv', full_name='protobuf.AdvanceGenerateDataKeyResponse.Iv', index=1,
+      number=2, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Plaintext', full_name='protobuf.AdvanceGenerateDataKeyResponse.Plaintext', index=2,
+      number=3, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='CiphertextBlob', full_name='protobuf.AdvanceGenerateDataKeyResponse.CiphertextBlob', index=3,
+      number=4, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='RequestId', full_name='protobuf.AdvanceGenerateDataKeyResponse.RequestId', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='Algorithm', full_name='protobuf.AdvanceGenerateDataKeyResponse.Algorithm', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='KeyVersionId', full_name='protobuf.AdvanceGenerateDataKeyResponse.KeyVersionId', index=6,
+      number=7, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3058,
+  serialized_end=3220,
+)
+
 DESCRIPTOR.message_types_by_name['KmsEncryptRequest'] = _KMSENCRYPTREQUEST
 DESCRIPTOR.message_types_by_name['KmsEncryptResponse'] = _KMSENCRYPTRESPONSE
 DESCRIPTOR.message_types_by_name['EncryptRequest'] = _ENCRYPTREQUEST
 DESCRIPTOR.message_types_by_name['EncryptResponse'] = _ENCRYPTRESPONSE
 DESCRIPTOR.message_types_by_name['KmsDecryptRequest'] = _KMSDECRYPTREQUEST
 DESCRIPTOR.message_types_by_name['KmsDecryptResponse'] = _KMSDECRYPTRESPONSE
 DESCRIPTOR.message_types_by_name['DecryptRequest'] = _DECRYPTREQUEST
@@ -1384,14 +1779,20 @@
 DESCRIPTOR.message_types_by_name['GenerateDataKeyRequest'] = _GENERATEDATAKEYREQUEST
 DESCRIPTOR.message_types_by_name['GenerateDataKeyResponse'] = _GENERATEDATAKEYRESPONSE
 DESCRIPTOR.message_types_by_name['GetPublicKeyRequest'] = _GETPUBLICKEYREQUEST
 DESCRIPTOR.message_types_by_name['GetPublicKeyResponse'] = _GETPUBLICKEYRESPONSE
 DESCRIPTOR.message_types_by_name['Error'] = _ERROR
 DESCRIPTOR.message_types_by_name['GetSecretValueRequest'] = _GETSECRETVALUEREQUEST
 DESCRIPTOR.message_types_by_name['GetSecretValueResponse'] = _GETSECRETVALUERESPONSE
+DESCRIPTOR.message_types_by_name['AdvanceEncryptRequest'] = _ADVANCEENCRYPTREQUEST
+DESCRIPTOR.message_types_by_name['AdvanceEncryptResponse'] = _ADVANCEENCRYPTRESPONSE
+DESCRIPTOR.message_types_by_name['AdvanceDecryptRequest'] = _ADVANCEDECRYPTREQUEST
+DESCRIPTOR.message_types_by_name['AdvanceDecryptResponse'] = _ADVANCEDECRYPTRESPONSE
+DESCRIPTOR.message_types_by_name['AdvanceGenerateDataKeyRequest'] = _ADVANCEGENERATEDATAKEYREQUEST
+DESCRIPTOR.message_types_by_name['AdvanceGenerateDataKeyResponse'] = _ADVANCEGENERATEDATAKEYRESPONSE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 KmsEncryptRequest = _reflection.GeneratedProtocolMessageType('KmsEncryptRequest', (_message.Message,), {
   'DESCRIPTOR' : _KMSENCRYPTREQUEST,
   '__module__' : 'api_pb2'
   # @@protoc_insertion_point(class_scope:protobuf.KmsEncryptRequest)
   })
@@ -1561,9 +1962,51 @@
 GetSecretValueResponse = _reflection.GeneratedProtocolMessageType('GetSecretValueResponse', (_message.Message,), {
   'DESCRIPTOR' : _GETSECRETVALUERESPONSE,
   '__module__' : 'api_pb2'
   # @@protoc_insertion_point(class_scope:protobuf.GetSecretValueResponse)
   })
 _sym_db.RegisterMessage(GetSecretValueResponse)
 
+AdvanceEncryptRequest = _reflection.GeneratedProtocolMessageType('AdvanceEncryptRequest', (_message.Message,), {
+  'DESCRIPTOR' : _ADVANCEENCRYPTREQUEST,
+  '__module__' : 'api_pb2'
+  # @@protoc_insertion_point(class_scope:protobuf.AdvanceEncryptRequest)
+  })
+_sym_db.RegisterMessage(AdvanceEncryptRequest)
+
+AdvanceEncryptResponse = _reflection.GeneratedProtocolMessageType('AdvanceEncryptResponse', (_message.Message,), {
+  'DESCRIPTOR' : _ADVANCEENCRYPTRESPONSE,
+  '__module__' : 'api_pb2'
+  # @@protoc_insertion_point(class_scope:protobuf.AdvanceEncryptResponse)
+  })
+_sym_db.RegisterMessage(AdvanceEncryptResponse)
+
+AdvanceDecryptRequest = _reflection.GeneratedProtocolMessageType('AdvanceDecryptRequest', (_message.Message,), {
+  'DESCRIPTOR' : _ADVANCEDECRYPTREQUEST,
+  '__module__' : 'api_pb2'
+  # @@protoc_insertion_point(class_scope:protobuf.AdvanceDecryptRequest)
+  })
+_sym_db.RegisterMessage(AdvanceDecryptRequest)
+
+AdvanceDecryptResponse = _reflection.GeneratedProtocolMessageType('AdvanceDecryptResponse', (_message.Message,), {
+  'DESCRIPTOR' : _ADVANCEDECRYPTRESPONSE,
+  '__module__' : 'api_pb2'
+  # @@protoc_insertion_point(class_scope:protobuf.AdvanceDecryptResponse)
+  })
+_sym_db.RegisterMessage(AdvanceDecryptResponse)
+
+AdvanceGenerateDataKeyRequest = _reflection.GeneratedProtocolMessageType('AdvanceGenerateDataKeyRequest', (_message.Message,), {
+  'DESCRIPTOR' : _ADVANCEGENERATEDATAKEYREQUEST,
+  '__module__' : 'api_pb2'
+  # @@protoc_insertion_point(class_scope:protobuf.AdvanceGenerateDataKeyRequest)
+  })
+_sym_db.RegisterMessage(AdvanceGenerateDataKeyRequest)
+
+AdvanceGenerateDataKeyResponse = _reflection.GeneratedProtocolMessageType('AdvanceGenerateDataKeyResponse', (_message.Message,), {
+  'DESCRIPTOR' : _ADVANCEGENERATEDATAKEYRESPONSE,
+  '__module__' : 'api_pb2'
+  # @@protoc_insertion_point(class_scope:protobuf.AdvanceGenerateDataKeyResponse)
+  })
+_sym_db.RegisterMessage(AdvanceGenerateDataKeyResponse)
+
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/sdk/client.py` & `alibabacloud-dkms-gcs-python2-0.0.6/sdk/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding=utf-8
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.core import TeaCore
+from alibabacloud_tea_util.client import Client as UtilClient
 
 from openapi.client import Client as DedicatedKmsOpenapiClient
-from sdk import models as dedicated_kms_sdk_models
 from openapi_util import models as dedicated_kms_openapi_util_models
-from alibabacloud_tea_util.client import Client as UtilClient
 from openapi_util.client import Client as DedicatedKmsOpenapiUtilClient
+from sdk import models as dedicated_kms_sdk_models
 
 
 class Client(DedicatedKmsOpenapiClient):
     def __init__(
             self,
             config,
     ):
@@ -293,7 +293,87 @@
 
     def get_secret_value(
             self,
             request,
     ):
         runtime = dedicated_kms_openapi_util_models.RuntimeOptions()
         return self.get_secret_value_with_options(request, runtime)
+
+    def advance_encrypt(self, request):
+        runtime = dedicated_kms_openapi_util_models.RuntimeOptions()
+        return self.advance_encrypt_with_options(request, runtime)
+
+    def advance_encrypt_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        req_body = UtilClient.to_map(request)
+        req_body_bytes = DedicatedKmsOpenapiUtilClient.get_serialized_advance_encrypt_request(req_body)
+        response_entity = self.do_request('AdvanceEncrypt', 'dkms-gcs-0.2', 'https', 'POST', 'RSA_PKCS1_SHA_256',
+                                          req_body_bytes, runtime, request.request_headers)
+        resp_map = DedicatedKmsOpenapiUtilClient.parse_advance_encrypt_response(
+            UtilClient.assert_as_bytes(response_entity.body_bytes))
+        advance_encrypt_response = TeaCore.from_map(
+            dedicated_kms_sdk_models.AdvanceEncryptResponse(),
+            {
+                'KeyId': resp_map.get('KeyId'),
+                'CiphertextBlob': resp_map.get('CiphertextBlob'),
+                'Iv': resp_map.get('Iv'),
+                'RequestId': resp_map.get('RequestId'),
+                'Algorithm': resp_map.get('Algorithm'),
+                'PaddingMode': resp_map.get('PaddingMode'),
+                'KeyVersionId': resp_map.get('KeyVersionId'),
+            }
+        )
+        advance_encrypt_response.response_headers = response_entity.response_headers
+        return advance_encrypt_response
+
+    def advance_decrypt(self, request):
+        runtime = dedicated_kms_openapi_util_models.RuntimeOptions()
+        return self.advance_decrypt_with_options(request, runtime)
+
+    def advance_decrypt_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        req_body = UtilClient.to_map(request)
+        req_body_bytes = DedicatedKmsOpenapiUtilClient.get_serialized_advance_decrypt_request(req_body)
+        response_entity = self.do_request('AdvanceDecrypt', 'dkms-gcs-0.2', 'https', 'POST', 'RSA_PKCS1_SHA_256',
+                                          req_body_bytes, runtime, request.request_headers)
+        resp_map = DedicatedKmsOpenapiUtilClient.parse_advance_decrypt_response(
+            UtilClient.assert_as_bytes(response_entity.body_bytes))
+        advance_decrypt_response = TeaCore.from_map(
+            dedicated_kms_sdk_models.AdvanceDecryptResponse(),
+            {
+                'KeyId': resp_map.get('KeyId'),
+                'Plaintext': resp_map.get('Plaintext'),
+                'RequestId': resp_map.get('RequestId'),
+                'Algorithm': resp_map.get('Algorithm'),
+                'PaddingMode': resp_map.get('PaddingMode'),
+                'KeyVersionId': resp_map.get('KeyVersionId'),
+            }
+        )
+        advance_decrypt_response.response_headers = response_entity.response_headers
+        return advance_decrypt_response
+
+    def advance_generate_data_key(self, request):
+        runtime = dedicated_kms_openapi_util_models.RuntimeOptions()
+        return self.advance_generate_data_key_with_options(request, runtime)
+
+    def advance_generate_data_key_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        req_body = UtilClient.to_map(request)
+        req_body_bytes = DedicatedKmsOpenapiUtilClient.get_serialized_advance_generate_data_key_request(req_body)
+        response_entity = self.do_request('AdvanceGenerateDataKey', 'dkms-gcs-0.2', 'https', 'POST',
+                                          'RSA_PKCS1_SHA_256', req_body_bytes, runtime, request.request_headers)
+        resp_map = DedicatedKmsOpenapiUtilClient.parse_advance_generate_data_key_response(
+            UtilClient.assert_as_bytes(response_entity.body_bytes))
+        advance_generate_data_key_response = TeaCore.from_map(
+            dedicated_kms_sdk_models.AdvanceGenerateDataKeyResponse(),
+            {
+                'KeyId': resp_map.get('KeyId'),
+                'Iv': resp_map.get('Iv'),
+                'Plaintext': resp_map.get('Plaintext'),
+                'CiphertextBlob': resp_map.get('CiphertextBlob'),
+                'RequestId': resp_map.get('RequestId'),
+                'Algorithm': resp_map.get('Algorithm'),
+                'KeyVersionId': resp_map.get('KeyVersionId'),
+            }
+        )
+        advance_generate_data_key_response.response_headers = response_entity.response_headers
+        return advance_generate_data_key_response
```

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/sdk/models.py` & `alibabacloud-dkms-gcs-python2-0.0.6/sdk/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -792,28 +792,28 @@
         if m.get('FetchExtendedConfig') is not None:
             self.fetch_extended_config = m.get('FetchExtendedConfig')
         return self
 
 
 class GetSecretValueResponse(DKMSResponse):
     def __init__(
-        self,
-        secret_name=None,
-        secret_type=None,
-        secret_data=None,
-        secret_data_type=None,
-        version_stages=None,
-        version_id=None,
-        create_time=None,
-        request_id=None,
-        last_rotation_date=None,
-        next_rotation_date=None,
-        extended_config=None,
-        automatic_rotation=None,
-        rotation_interval=None,
+            self,
+            secret_name=None,
+            secret_type=None,
+            secret_data=None,
+            secret_data_type=None,
+            version_stages=None,
+            version_id=None,
+            create_time=None,
+            request_id=None,
+            last_rotation_date=None,
+            next_rotation_date=None,
+            extended_config=None,
+            automatic_rotation=None,
+            rotation_interval=None,
     ):
         super(GetSecretValueResponse, self).__init__()
         self.secret_name = secret_name
         self.secret_type = secret_type
         self.secret_data = secret_data
         self.secret_data_type = secret_data_type
         self.version_stages = version_stages
@@ -888,7 +888,305 @@
         if m.get('ExtendedConfig') is not None:
             self.extended_config = m.get('ExtendedConfig')
         if m.get('AutomaticRotation') is not None:
             self.automatic_rotation = m.get('AutomaticRotation')
         if m.get('RotationInterval') is not None:
             self.rotation_interval = m.get('RotationInterval')
         return self
+
+
+class AdvanceEncryptRequest(DKMSRequest):
+    def __init__(self, key_id=None, plaintext=None, algorithm=None, aad=None, iv=None, padding_mode=None):
+        super(AdvanceEncryptRequest, self).__init__()
+        self.key_id = key_id
+        self.plaintext = plaintext
+        self.algorithm = algorithm
+        self.aad = aad
+        self.iv = iv
+        self.padding_mode = padding_mode
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AdvanceEncryptRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key_id is not None:
+            result['KeyId'] = self.key_id
+        if self.plaintext is not None:
+            result['Plaintext'] = self.plaintext
+        if self.algorithm is not None:
+            result['Algorithm'] = self.algorithm
+        if self.aad is not None:
+            result['Aad'] = self.aad
+        if self.iv is not None:
+            result['Iv'] = self.iv
+        if self.padding_mode is not None:
+            result['PaddingMode'] = self.padding_mode
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('KeyId') is not None:
+            self.key_id = m.get('KeyId')
+        if m.get('Plaintext') is not None:
+            self.plaintext = m.get('Plaintext')
+        if m.get('Algorithm') is not None:
+            self.algorithm = m.get('Algorithm')
+        if m.get('Aad') is not None:
+            self.aad = m.get('Aad')
+        if m.get('Iv') is not None:
+            self.iv = m.get('Iv')
+        if m.get('PaddingMode') is not None:
+            self.padding_mode = m.get('PaddingMode')
+        return self
+
+
+class AdvanceEncryptResponse(DKMSResponse):
+    def __init__(self, key_id=None, ciphertext_blob=None, iv=None, request_id=None, algorithm=None,
+                 padding_mode=None, key_version_id=None):
+        super(AdvanceEncryptResponse, self).__init__()
+        self.key_id = key_id
+        self.ciphertext_blob = ciphertext_blob
+        self.iv = iv
+        self.request_id = request_id
+        self.algorithm = algorithm
+        self.padding_mode = padding_mode
+        self.key_version_id = key_version_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AdvanceEncryptResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key_id is not None:
+            result['KeyId'] = self.key_id
+        if self.ciphertext_blob is not None:
+            result['CiphertextBlob'] = self.ciphertext_blob
+        if self.iv is not None:
+            result['Iv'] = self.iv
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.algorithm is not None:
+            result['Algorithm'] = self.algorithm
+        if self.padding_mode is not None:
+            result['PaddingMode'] = self.padding_mode
+        if self.key_version_id is not None:
+            result['KeyVersionId'] = self.key_version_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('KeyId') is not None:
+            self.key_id = m.get('KeyId')
+        if m.get('CiphertextBlob') is not None:
+            self.ciphertext_blob = m.get('CiphertextBlob')
+        if m.get('Iv') is not None:
+            self.iv = m.get('Iv')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Algorithm') is not None:
+            self.algorithm = m.get('Algorithm')
+        if m.get('PaddingMode') is not None:
+            self.padding_mode = m.get('PaddingMode')
+        if m.get('KeyVersionId') is not None:
+            self.key_version_id = m.get('KeyVersionId')
+        return self
+
+
+class AdvanceDecryptRequest(DKMSRequest):
+    def __init__(self, ciphertext_blob=None, key_id=None, algorithm=None, aad=None, iv=None, padding_mode=None):
+        super(AdvanceDecryptRequest, self).__init__()
+        self.ciphertext_blob = ciphertext_blob
+        self.key_id = key_id
+        self.algorithm = algorithm
+        self.aad = aad
+        self.iv = iv
+        self.padding_mode = padding_mode
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AdvanceDecryptRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ciphertext_blob is not None:
+            result['CiphertextBlob'] = self.ciphertext_blob
+        if self.key_id is not None:
+            result['KeyId'] = self.key_id
+        if self.algorithm is not None:
+            result['Algorithm'] = self.algorithm
+        if self.aad is not None:
+            result['Aad'] = self.aad
+        if self.iv is not None:
+            result['Iv'] = self.iv
+        if self.padding_mode is not None:
+            result['PaddingMode'] = self.padding_mode
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CiphertextBlob') is not None:
+            self.ciphertext_blob = m.get('CiphertextBlob')
+        if m.get('KeyId') is not None:
+            self.key_id = m.get('KeyId')
+        if m.get('Algorithm') is not None:
+            self.algorithm = m.get('Algorithm')
+        if m.get('Aad') is not None:
+            self.aad = m.get('Aad')
+        if m.get('Iv') is not None:
+            self.iv = m.get('Iv')
+        if m.get('PaddingMode') is not None:
+            self.padding_mode = m.get('PaddingMode')
+        return self
+
+
+class AdvanceDecryptResponse(DKMSResponse):
+    def __init__(self, key_id=None, plaintext=None, request_id=None, algorithm=None, padding_mode=None,
+                 key_version_id=None):
+        super(AdvanceDecryptResponse, self).__init__()
+        self.key_id = key_id
+        self.plaintext = plaintext
+        self.request_id = request_id
+        self.algorithm = algorithm
+        self.padding_mode = padding_mode
+        self.key_version_id = key_version_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AdvanceDecryptResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key_id is not None:
+            result['KeyId'] = self.key_id
+        if self.plaintext is not None:
+            result['Plaintext'] = self.plaintext
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.algorithm is not None:
+            result['Algorithm'] = self.algorithm
+        if self.padding_mode is not None:
+            result['PaddingMode'] = self.padding_mode
+        if self.key_version_id is not None:
+            result['KeyVersionId'] = self.key_version_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('KeyId') is not None:
+            self.key_id = m.get('KeyId')
+        if m.get('Plaintext') is not None:
+            self.plaintext = m.get('Plaintext')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Algorithm') is not None:
+            self.algorithm = m.get('Algorithm')
+        if m.get('PaddingMode') is not None:
+            self.padding_mode = m.get('PaddingMode')
+        if m.get('KeyVersionId') is not None:
+            self.key_version_id = m.get('KeyVersionId')
+        return self
+
+
+class AdvanceGenerateDataKeyRequest(DKMSRequest):
+    def __init__(self, key_id=None, number_of_bytes=None, aad=None):
+        super(AdvanceGenerateDataKeyRequest, self).__init__()
+        self.key_id = key_id
+        self.number_of_bytes = number_of_bytes
+        self.aad = aad
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AdvanceGenerateDataKeyRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key_id is not None:
+            result['KeyId'] = self.key_id
+        if self.number_of_bytes is not None:
+            result['NumberOfBytes'] = self.number_of_bytes
+        if self.aad is not None:
+            result['Aad'] = self.aad
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('KeyId') is not None:
+            self.key_id = m.get('KeyId')
+        if m.get('NumberOfBytes') is not None:
+            self.number_of_bytes = m.get('NumberOfBytes')
+        if m.get('Aad') is not None:
+            self.aad = m.get('Aad')
+        return self
+
+
+class AdvanceGenerateDataKeyResponse(DKMSResponse):
+    def __init__(self, key_id=None, iv=None, plaintext=None, ciphertext_blob=None, request_id=None, algorithm=None,
+                 key_version_id=None):
+        super(AdvanceGenerateDataKeyResponse, self).__init__()
+        self.key_id = key_id
+        self.iv = iv
+        self.plaintext = plaintext
+        self.ciphertext_blob = ciphertext_blob
+        self.request_id = request_id
+        self.algorithm = algorithm
+        self.key_version_id = key_version_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AdvanceGenerateDataKeyResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key_id is not None:
+            result['KeyId'] = self.key_id
+        if self.iv is not None:
+            result['Iv'] = self.iv
+        if self.plaintext is not None:
+            result['Plaintext'] = self.plaintext
+        if self.ciphertext_blob is not None:
+            result['CiphertextBlob'] = self.ciphertext_blob
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.algorithm is not None:
+            result['Algorithm'] = self.algorithm
+        if self.key_version_id is not None:
+            result['KeyVersionId'] = self.key_version_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('KeyId') is not None:
+            self.key_id = m.get('KeyId')
+        if m.get('Iv') is not None:
+            self.iv = m.get('Iv')
+        if m.get('Plaintext') is not None:
+            self.plaintext = m.get('Plaintext')
+        if m.get('CiphertextBlob') is not None:
+            self.ciphertext_blob = m.get('CiphertextBlob')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Algorithm') is not None:
+            self.algorithm = m.get('Algorithm')
+        if m.get('KeyVersionId') is not None:
+            self.key_version_id = m.get('KeyVersionId')
+        return self
```

### Comparing `alibabacloud-dkms-gcs-python2-0.0.5/setup.py` & `alibabacloud-dkms-gcs-python2-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 packages = find_packages()
 NAME = "alibabacloud-dkms-gcs-python2"
 DESCRIPTION = "AlibabaCloud DKMS-GCS SDK for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-dkms-gcs-python2-sdk"
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 REQUIRES = [
     "protobuf>=3.12.0,<=3.17.0",
     "alibabacloud_tea_util_py2>=0.0.1",
     'pyopenssl>=16.2.0,<=21.0.0',
     'cryptography<=3.3.2'
 ]
```

