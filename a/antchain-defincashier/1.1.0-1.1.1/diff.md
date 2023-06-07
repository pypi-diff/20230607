# Comparing `tmp/antchain_defincashier-1.1.0.tar.gz` & `tmp/antchain_defincashier-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_defincashier-1.1.0.tar", last modified: Fri May 12 08:23:50 2023, max compression
+gzip compressed data, was "dist/antchain_defincashier-1.1.1.tar", last modified: Wed Jun  7 09:23:19 2023, max compression
```

## Comparing `antchain_defincashier-1.1.0.tar` & `antchain_defincashier-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2216 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2216 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_sdk_defincashier/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_sdk_defincashier/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39521 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_sdk_defincashier/client.py
--rw-r--r--   0 root         (0) root         (0)    76117 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_sdk_defincashier/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2533 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_sdk_defincashier/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_sdk_defincashier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39521 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_sdk_defincashier/client.py
+-rw-r--r--   0 root         (0) root         (0)    76711 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_sdk_defincashier/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/setup.py
```

### Comparing `antchain_defincashier-1.1.0/LICENSE` & `antchain_defincashier-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_defincashier-1.1.0/PKG-INFO` & `antchain_defincashier-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_defincashier
-Version: 1.1.0
+Version: 1.1.1
 Summary: Ant Chain DEFINCASHIER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_defincashier-1.1.0/README-CN.md` & `antchain_defincashier-1.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_defincashier-1.1.0/README.md` & `antchain_defincashier-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_defincashier-1.1.0/antchain_defincashier.egg-info/PKG-INFO` & `antchain_defincashier-1.1.1/antchain_defincashier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-defincashier
-Version: 1.1.0
+Version: 1.1.1
 Summary: Ant Chain DEFINCASHIER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_defincashier-1.1.0/antchain_sdk_defincashier/client.py` & `antchain_defincashier-1.1.1/antchain_sdk_defincashier/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.0',
+                    'sdk_version': '1.1.1',
                     '_prod_code': 'DEFINCASHIER',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.0',
+                    'sdk_version': '1.1.1',
                     '_prod_code': 'DEFINCASHIER',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_defincashier-1.1.0/antchain_sdk_defincashier/models.py` & `antchain_defincashier-1.1.1/antchain_sdk_defincashier/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         self.status = status
         # 分类 BUYER付款账户； SELLER收款账户
         self.category = category
         # 上次支付是否失败
         self.last_pay_fail = last_pay_fail
         # 支付方式 BALANCE余额账户；BILL票据账户
         self.pay_method = pay_method
-        # 账户类型 MAIN 银行账户；ECOLLECTION e收宝
+        # 账户类型 MAIN 银行账户；ECOLLECTION e收宝；Q_PAYEE 通用静默户；
         self.type = type
         # 主体：I-个人；E-企业
         self.principal = principal
         # 金额明细
         self.amount_item = amount_item
 
     def validate(self):
@@ -863,22 +863,28 @@
 
 class PaymentShareAcceptanceResult(TeaModel):
     def __init__(
         self,
         out_order_id: str = None,
         out_request_id: str = None,
         state: str = None,
+        sub_code: str = None,
+        sub_msg: str = None,
     ):
         # 外部业务平台原始交易号
         self.out_order_id = out_order_id
         # 外部请求ID，幂等字段
         # 
         self.out_request_id = out_request_id
         # 分账单状态
         self.state = state
+        # 业务错误码(为空表示成功，否则为业务错误码)
+        self.sub_code = sub_code
+        # 业务错误描述
+        self.sub_msg = sub_msg
 
     def validate(self):
         self.validate_required(self.out_order_id, 'out_order_id')
         self.validate_required(self.out_request_id, 'out_request_id')
         self.validate_required(self.state, 'state')
 
     def to_map(self):
@@ -889,24 +895,32 @@
         result = dict()
         if self.out_order_id is not None:
             result['out_order_id'] = self.out_order_id
         if self.out_request_id is not None:
             result['out_request_id'] = self.out_request_id
         if self.state is not None:
             result['state'] = self.state
+        if self.sub_code is not None:
+            result['sub_code'] = self.sub_code
+        if self.sub_msg is not None:
+            result['sub_msg'] = self.sub_msg
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('out_order_id') is not None:
             self.out_order_id = m.get('out_order_id')
         if m.get('out_request_id') is not None:
             self.out_request_id = m.get('out_request_id')
         if m.get('state') is not None:
             self.state = m.get('state')
+        if m.get('sub_code') is not None:
+            self.sub_code = m.get('sub_code')
+        if m.get('sub_msg') is not None:
+            self.sub_msg = m.get('sub_msg')
         return self
 
 
 class AgreementQueryResult(TeaModel):
     def __init__(
         self,
         platform_member_id: str = None,
```

### Comparing `antchain_defincashier-1.1.0/setup.py` & `antchain_defincashier-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_defincashier.
 
-Created on 12/05/2023
+Created on 07/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_defincashier"
 NAME = "antchain_defincashier" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain DEFINCASHIER SDK Library for Python"
```

