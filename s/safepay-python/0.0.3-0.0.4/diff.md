# Comparing `tmp/safepay_python-0.0.3.tar.gz` & `tmp/safepay_python-0.0.4.tar.gz`

## Comparing `safepay_python-0.0.3.tar` & `safepay_python-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 safepay_python-0.0.3/readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 safepay_python-0.0.3/safepay_python/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 safepay_python-0.0.3/safepay_python/safepay.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 safepay_python-0.0.3/safepay_python/resources/checkout.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 safepay_python-0.0.3/safepay_python/resources/payments.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 safepay_python-0.0.3/safepay_python/resources/verify.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 safepay_python-0.0.3/safepay_python/utils/builder.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 safepay_python-0.0.3/safepay_python/utils/constants.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 safepay_python-0.0.3/safepay_python/utils/secure_compare.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 safepay_python-0.0.3/safepay_python/utils/validation.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 safepay_python-0.0.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 safepay_python-0.0.3/LICENSE
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 safepay_python-0.0.3/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 safepay_python-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 safepay_python-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 safepay_python-0.0.4/readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 safepay_python-0.0.4/safepay_python/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 safepay_python-0.0.4/safepay_python/safepay.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 safepay_python-0.0.4/safepay_python/resources/checkout.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 safepay_python-0.0.4/safepay_python/resources/payments.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 safepay_python-0.0.4/safepay_python/resources/verify.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 safepay_python-0.0.4/safepay_python/utils/builder.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 safepay_python-0.0.4/safepay_python/utils/constants.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 safepay_python-0.0.4/safepay_python/utils/secure_compare.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 safepay_python-0.0.4/safepay_python/utils/validation.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 safepay_python-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 safepay_python-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 safepay_python-0.0.4/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 safepay_python-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 safepay_python-0.0.4/PKG-INFO
```

### Comparing `safepay_python-0.0.3/readme.md` & `safepay_python-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: safepay_python
+Version: 0.0.4
+Summary: Safepay's python SDK for checkout integration
+Project-URL: Homepage, https://github.com/getsafepay/safepay-python
+Project-URL: Bug Tracker, https://github.com/getsafepay/safepay-python/issues
+Author-email: Fatima Aurangzeb <faurangzeb@getsafepay.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Requires-Dist: requests==2.28.2
+Requires-Dist: six==1.16.0
+Requires-Dist: urllib3==1.26.14
+Description-Content-Type: text/markdown
+
 # Safepay Python SDK
 
 Official python library for [Safepay API](https://getsafepay.com).
 
 ## Installation
 
 ### With Pip
@@ -11,17 +28,17 @@
 ```
 
 ## Usage
 
 Import and create a Safepay client by passing your config;
 
 ```python
-from "python_sdk" import safepay;
+from safepay_python.safepay import *
 
-env = safepay.Safepay(
+env = Safepay(
     {
         "environment": "sandbox",
         "apiKey": "sec_asd12-2342s-1231s",
         "v1Secret": "bar",
         "webhookSecret": "foo",
     }
 )
@@ -38,15 +55,15 @@
 | ---------- | ------------ | -------- |
 | `amount`   | `number`     | Yes      |
 | `currency` | `PKR`, `USD` | Yes      |
 
 ```python
 payment_response = env.set_payment_details({"amount": 10000, "currency": "PKR"})
 
-token = payment_response["data"]["token"]
+token = (payment_response['data'])['token']
 
 
 
 # Pass `token` to create checkout link
 ```
 
 ### Checkout
@@ -79,31 +96,33 @@
 # redirect user to `url`
 ```
 
 ### Verification
 
 #### Signature
 
-| Parameter | Type     | Description                       | Required |
-| --------- | -------- | --------------------------------- | -------- |
-| `request` | `object` | The `req` object from your server | Yes      |
+| Parameter | Type     | Description                             | Required |
+| --------- | -------- | --------------------------------------- | -------- |
+| `sig`     | `string` | The `signature` string from your server | Yes      |
+| `tracker` | `string` | The `tracker` string from your server   | Yes      |
 
 ```python
 signature_verification = env.is_signature_valid({"sig": "abcd", "tracker": token})
 
 
 # mark the invoice as paid if valid
 # show an error if invalid
 ```
 
 #### Webhook
 
-| Parameter | Type     | Description                       | Required |
-| --------- | -------- | --------------------------------- | -------- |
-| `request` | `object` | The `req` object from your server | Yes      |
+| Parameter          | Type     | Description                             | Required |
+| ------------------ | -------- | --------------------------------------- | -------- |
+| `x-sfpy-signature` | `string` | The `signature` string from your server | Yes      |
+| `data`             | `object` | The `data` object from your server      | Yes      |
 
 ```python
 webhook_verification = env.is_webhook_valid(
     {"x-sfpy-signature": "abcd"}, {"data": data}
 )
```

### Comparing `safepay_python-0.0.3/safepay_python/safepay.py` & `safepay_python-0.0.4/safepay_python/safepay.py`

 * *Files identical despite different names*

### Comparing `safepay_python-0.0.3/safepay_python/resources/checkout.py` & `safepay_python-0.0.4/safepay_python/resources/checkout.py`

 * *Files identical despite different names*

### Comparing `safepay_python-0.0.3/safepay_python/resources/payments.py` & `safepay_python-0.0.4/safepay_python/resources/payments.py`

 * *Files identical despite different names*

### Comparing `safepay_python-0.0.3/safepay_python/resources/verify.py` & `safepay_python-0.0.4/safepay_python/resources/verify.py`

 * *Files identical despite different names*

### Comparing `safepay_python-0.0.3/safepay_python/utils/validation.py` & `safepay_python-0.0.4/safepay_python/utils/validation.py`

 * *Files identical despite different names*

### Comparing `safepay_python-0.0.3/LICENSE` & `safepay_python-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `safepay_python-0.0.3/README.md` & `safepay_python-0.0.4/readme.md`

 * *Files 26% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ```
 
 ## Usage
 
 Import and create a Safepay client by passing your config;
 
 ```python
-from "python_sdk" import safepay;
+from safepay_python.safepay import *
 
-env = safepay.Safepay(
+env = Safepay(
     {
         "environment": "sandbox",
         "apiKey": "sec_asd12-2342s-1231s",
         "v1Secret": "bar",
         "webhookSecret": "foo",
     }
 )
@@ -38,15 +38,15 @@
 | ---------- | ------------ | -------- |
 | `amount`   | `number`     | Yes      |
 | `currency` | `PKR`, `USD` | Yes      |
 
 ```python
 payment_response = env.set_payment_details({"amount": 10000, "currency": "PKR"})
 
-token = payment_response["data"]["token"]
+token = (payment_response['data'])['token']
 
 
 
 # Pass `token` to create checkout link
 ```
 
 ### Checkout
@@ -79,31 +79,33 @@
 # redirect user to `url`
 ```
 
 ### Verification
 
 #### Signature
 
-| Parameter | Type     | Description                       | Required |
-| --------- | -------- | --------------------------------- | -------- |
-| `request` | `object` | The `req` object from your server | Yes      |
+| Parameter | Type     | Description                             | Required |
+| --------- | -------- | --------------------------------------- | -------- |
+| `sig`     | `string` | The `signature` string from your server | Yes      |
+| `tracker` | `string` | The `tracker` string from your server   | Yes      |
 
 ```python
 signature_verification = env.is_signature_valid({"sig": "abcd", "tracker": token})
 
 
 # mark the invoice as paid if valid
 # show an error if invalid
 ```
 
 #### Webhook
 
-| Parameter | Type     | Description                       | Required |
-| --------- | -------- | --------------------------------- | -------- |
-| `request` | `object` | The `req` object from your server | Yes      |
+| Parameter          | Type     | Description                             | Required |
+| ------------------ | -------- | --------------------------------------- | -------- |
+| `x-sfpy-signature` | `string` | The `signature` string from your server | Yes      |
+| `data`             | `object` | The `data` object from your server      | Yes      |
 
 ```python
 webhook_verification = env.is_webhook_valid(
     {"x-sfpy-signature": "abcd"}, {"data": data}
 )
```

### Comparing `safepay_python-0.0.3/pyproject.toml` & `safepay_python-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "safepay_python"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Fatima Aurangzeb", email="faurangzeb@getsafepay.com" },
 ]
 description = "Safepay's python SDK for checkout integration"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "requests==2.28.2",
     "urllib3==1.26.14",
+    "six==1.16.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/getsafepay/safepay-python"
 "Bug Tracker" = "https://github.com/getsafepay/safepay-python/issues"
```

