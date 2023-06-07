# Comparing `tmp/zebedee-0.0.6.tar.gz` & `tmp/zebedee-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zebedee-0.0.6.tar", last modified: Mon May 15 14:46:08 2023, max compression
+gzip compressed data, was "zebedee-0.0.7.tar", last modified: Wed Jun  7 15:31:12 2023, max compression
```

## Comparing `zebedee-0.0.6.tar` & `zebedee-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-15 14:46:08.962221 zebedee-0.0.6/
--rw-r--r--   0 santos     (501) staff       (20)     1065 2023-04-03 00:04:47.000000 zebedee-0.0.6/LICENSE
--rw-r--r--   0 santos     (501) staff       (20)     7012 2023-05-15 14:46:08.962103 zebedee-0.0.6/PKG-INFO
--rw-r--r--   0 santos     (501) staff       (20)     6424 2023-05-15 14:45:43.000000 zebedee-0.0.6/README.md
--rw-r--r--   0 santos     (501) staff       (20)       38 2023-05-15 14:46:08.962257 zebedee-0.0.6/setup.cfg
--rw-r--r--   0 santos     (501) staff       (20)     1167 2023-05-15 14:46:06.000000 zebedee-0.0.6/setup.py
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-15 14:46:08.961321 zebedee-0.0.6/zebedee/
--rw-r--r--   0 santos     (501) staff       (20)       19 2023-05-11 05:51:33.000000 zebedee-0.0.6/zebedee/__init__.py
--rw-r--r--   0 santos     (501) staff       (20)    11240 2023-05-15 04:00:08.000000 zebedee-0.0.6/zebedee/main.py
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-15 14:46:08.961930 zebedee-0.0.6/zebedee.egg-info/
--rw-r--r--   0 santos     (501) staff       (20)     7012 2023-05-15 14:46:08.000000 zebedee-0.0.6/zebedee.egg-info/PKG-INFO
--rw-r--r--   0 santos     (501) staff       (20)      216 2023-05-15 14:46:08.000000 zebedee-0.0.6/zebedee.egg-info/SOURCES.txt
--rw-r--r--   0 santos     (501) staff       (20)        1 2023-05-15 14:46:08.000000 zebedee-0.0.6/zebedee.egg-info/dependency_links.txt
--rw-r--r--   0 santos     (501) staff       (20)       49 2023-05-15 14:46:08.000000 zebedee-0.0.6/zebedee.egg-info/requires.txt
--rw-r--r--   0 santos     (501) staff       (20)        8 2023-05-15 14:46:08.000000 zebedee-0.0.6/zebedee.egg-info/top_level.txt
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-06-07 15:31:12.088352 zebedee-0.0.7/
+-rw-r--r--   0 santos     (501) staff       (20)     1065 2023-04-03 00:04:47.000000 zebedee-0.0.7/LICENSE
+-rw-r--r--   0 santos     (501) staff       (20)     7012 2023-06-07 15:31:12.088149 zebedee-0.0.7/PKG-INFO
+-rw-r--r--   0 santos     (501) staff       (20)     6424 2023-05-15 14:45:43.000000 zebedee-0.0.7/README.md
+-rw-r--r--   0 santos     (501) staff       (20)       38 2023-06-07 15:31:12.088404 zebedee-0.0.7/setup.cfg
+-rw-r--r--   0 santos     (501) staff       (20)     1167 2023-06-07 15:13:23.000000 zebedee-0.0.7/setup.py
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-06-07 15:31:12.086020 zebedee-0.0.7/zebedee/
+-rw-r--r--   0 santos     (501) staff       (20)       19 2023-05-11 05:51:33.000000 zebedee-0.0.7/zebedee/__init__.py
+-rw-r--r--   0 santos     (501) staff       (20)    13437 2023-06-07 15:22:57.000000 zebedee-0.0.7/zebedee/main.py
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-06-07 15:31:12.087264 zebedee-0.0.7/zebedee.egg-info/
+-rw-r--r--   0 santos     (501) staff       (20)     7012 2023-06-07 15:31:12.000000 zebedee-0.0.7/zebedee.egg-info/PKG-INFO
+-rw-r--r--   0 santos     (501) staff       (20)      216 2023-06-07 15:31:12.000000 zebedee-0.0.7/zebedee.egg-info/SOURCES.txt
+-rw-r--r--   0 santos     (501) staff       (20)        1 2023-06-07 15:31:12.000000 zebedee-0.0.7/zebedee.egg-info/dependency_links.txt
+-rw-r--r--   0 santos     (501) staff       (20)       49 2023-06-07 15:31:12.000000 zebedee-0.0.7/zebedee.egg-info/requires.txt
+-rw-r--r--   0 santos     (501) staff       (20)        8 2023-06-07 15:31:12.000000 zebedee-0.0.7/zebedee.egg-info/top_level.txt
```

### Comparing `zebedee-0.0.6/LICENSE` & `zebedee-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zebedee-0.0.6/PKG-INFO` & `zebedee-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebedee
-Version: 0.0.6
+Version: 0.0.7
 Summary: Move Money at the Speed of the Internet 
 Author: zantoshi (Santos Hernandez)
 Author-email: <santosdhernandez@gmail.com>
 Keywords: python,payments,bitcoin,lightning network,django,lightning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zebedee-0.0.6/README.md` & `zebedee-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `zebedee-0.0.6/setup.py` & `zebedee-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Move Money at the Speed of the Internet '
 LONG_DESCRIPTION = 'A package that allows for faster integration of the ZEBEDEE API.'
 
 # Setting up
 setup(
     name="zebedee",
     version=VERSION,
```

### Comparing `zebedee-0.0.6/zebedee/main.py` & `zebedee-0.0.7/zebedee/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,34 +22,45 @@
     '''
         Charge Actions
     '''
 
     def get_wallet_details(self):
         URL = 'https://api.zebedee.io/v0/wallet'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]
+        except:
+            return requests.get(URL, headers=heads).json()
+
         
     def create_charge(self, amount_of_seconds_to_expire_after, amount_msats, description, internal_id = None):
         URL = 'https://api.zebedee.io/v0/charges'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
 
         payload = json.dumps({
             "expiresIn": amount_of_seconds_to_expire_after,
             "amount": str(amount_msats),
             "description": description,
             "internalId": internal_id,
             "callbackUrl": self.callback_url
         })
+        try:
+            return requests.post(URL, headers=heads, data=payload).json()["data"]
+        except:
+            return requests.post(URL, headers=heads, data=payload).json()
 
-        return requests.post(URL, headers=heads, data=payload).json()["data"]
         
     def get_charge_details(self, zbd_id):
         URL = f'https://api.zebedee.io/v0/charges/{zbd_id}'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]
+        except:
+            return requests.get(URL, headers=heads).json()
+
 
     '''
         Static Charge Actions
     '''
 
     def create_static_charge(self,  min_amount_msats, max_amount_msats, description, internal_id, success_message, allowed_slots=None):
         URL = 'https://api.zebedee.io/v0/static-charges'
@@ -60,36 +71,47 @@
             "minAmount": str(min_amount_msats),
             "maxAmount": str(max_amount_msats),
             "description": description,
             "internalId": internal_id,
             "callbackUrl": self.callback_url,
             "successMessage": success_message
         })
+        try:
+            return requests.post(URL, headers=heads, data=payload).json()["data"]
+        except:
+            return requests.post(URL, headers=heads, data=payload).json()
 
-        return requests.post(URL, headers=heads, data=payload).json()["data"]
         
 
     def update_static_charge_details(self, id, min_amount_msats, max_amount_msats, description, success_message, allowed_slots = None):
         url = f"https://api.zebedee.io/v0/static-charges/{id}"
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
         payload = {
             "allowedSlots": allowed_slots,
             "minAmount": str(min_amount_msats),
             "maxAmount": str(max_amount_msats),
             "description": description,
             "callbackUrl": self.callback_url,
             "successMessage": success_message
         }
-        return requests.patch(url, headers=heads, data=json.dumps(payload)).json()["data"]
+        try:
+            return requests.patch(url, headers=heads, data=json.dumps(payload)).json()["data"]
+        except:
+            return requests.patch(url, headers=heads, data=json.dumps(payload)).json()
+
 
 
     def get_static_charge_details(self, zbd_id):
         URL = f'https://api.zebedee.io/v0/static-charges/{zbd_id}'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]
+        except:
+            return requests.get(URL, headers=heads).json()
+
 
     '''
         Withdrawal Request Actions
     '''
 
     def create_withdrawal_request(self, amount_of_seconds_to_expire_after, amount_msats, description, internal_id):
         URL = 'https://api.zebedee.io/v0/withdrawal-requests'
@@ -98,21 +120,28 @@
         payload = json.dumps({
             "expiresIn": amount_of_seconds_to_expire_after,
             "amount": str(amount_msats),
             "description": description,
             "internalId": internal_id,
             "callbackUrl": self.callback_url
         })
+        try:
+            return requests.post(URL, headers=heads, data=payload).json()["data"]
+        except:
+            return requests.post(URL, headers=heads, data=payload).json()
 
-        return requests.post(URL, headers=heads, data=payload).json()["data"]
         
     def get_withdrawal_request_details(self, zbd_id):
         URL = f'https://api.zebedee.io/v0/withdrawal-requests/{zbd_id}'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]
+        except:
+            return requests.get(URL, headers=heads).json()
+
 
     '''
         Keysend Payment Action
     '''
     def send_keysend_payment(self, public_key, amount_msats, metadata = None, tlv_records = None):
         URL = 'https://api.zebedee.io/v0/keysend-payment'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
@@ -120,16 +149,19 @@
         payload = json.dumps({
             "amount": str(amount_msats),
             "pubkey": str(public_key),
             "tlvRecords": tlv_records,
             "metadata": metadata,
             "callbackUrl": f"{self.callback_url}"
         })
+        try:
+            return requests.post(URL, headers=heads, data=payload).json()["data"]
+        except:
+            return requests.post(URL, headers=heads, data=payload).json()
 
-        return requests.post(URL, headers=heads, data=payload).json()["data"]
 
     '''
         Invoice Payment Actions
     '''
 
     def pay_invoice(self, invoice, description, internal_id, amount = None):
         URL = 'https://api.zebedee.io/v0/payments'
@@ -146,30 +178,40 @@
         else:
             payload = json.dumps({
                 "description": description,
                 "internalId": internal_id,
                 "invoice": invoice,
                 "callbackUrl": self.callback_url
             })
+        try:
+            return requests.post(URL, headers=heads, data=payload).json()["data"]
+        except:
+            return requests.post(URL, headers=heads, data=payload).json()
 
-        return requests.post(URL, headers=heads, data=payload).json()["data"]
 
     def get_payment_details(self, zbd_id):
         URL = f'https://api.zebedee.io/v0/payments/{zbd_id}'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]
+        except:
+            return requests.get(URL, headers=heads).json()
 
     '''
         Lightning Address Actions
     '''
 
     def validate_lightning_address(self, lightning_address):
         URL = f'https://api.zebedee.io/v0/ln-address/validate/{lightning_address}'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]
+        except:
+            return requests.get(URL, headers=heads).json()
+
     
     def send_payment_to_lightning_address(self, lightning_address, amount_msats, comment, internal_id):
         URL = 'https://api.zebedee.io/v0/ln-address/send-payment'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
 
         payload = json.dumps({
             "lnAddress": "santos@zbd.gg",
@@ -194,78 +236,109 @@
 
         payload = json.dumps({
             "lnaddress": lightning_address,
             "amount": str(amount_msats),
             "description": description
         })
 
-        return requests.post(URL, headers=heads, data=payload).json()["data"]
-
+        try:
+            return requests.post(URL, headers=heads, data=payload).json()["data"]
+        except:
+            return requests.post(URL, headers=heads, data=payload).json()
     '''
         Gamertag Actions
     '''
 
     def send_payment_to_gamertag(self, gamertag, amount_msats, description):
         URL = 'https://api.zebedee.io/v0/gamertag/send-payment'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
 
         payload = json.dumps({
             "gamertag": gamertag,
             "amount": str(amount_msats),
             "description": description
         })
+        try:
+            return requests.post(URL, headers=heads, data=payload).json()["data"]
+        except:
+            return requests.post(URL, headers=heads, data=payload).json()
 
-        return requests.post(URL, headers=heads, data=payload).json()["data"]
 
     def get_gamertag_transaction_details(self, zbd_id):
         URL = f'https://api.zebedee.io/v0/gamertag/transaction/{zbd_id}'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]
+        except:
+            return requests.get(URL, headers=heads).json()
+
 
     def get_user_id_from_gamertag(self, gamertag):
         URL = f'https://api.zebedee.io/v0/user-id/gamertag/{gamertag}'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]["id"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]["id"]
+        except:
+            return requests.get(URL, headers=heads).json()
+
 
     def get_gamertag_from_user_id(self, user_id):
         URL = f'https://api.zebedee.io/v0/gamertag/user-id/{user_id}'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]["gamertag"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]["gamertag"]
+        except:
+            return requests.get(URL, headers=heads).json()
+
 
     def fetch_charge_from_gamertag(self, gamertag, amount_msats, description, internal_id):
         URL = 'https://api.zebedee.io/v0/gamertag/charges'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
 
         payload = json.dumps({
             "amount": str(amount_msats),
             "gamertag": gamertag,
             "description": description,
             "callbackUrl": self.callback_url,
             "internalId": internal_id
         })
+        try:
+            return requests.post(URL, headers=heads, data=payload).json()["data"]
+        except:
+            return requests.post(URL, headers=heads, data=payload).json()
 
-        return requests.post(URL, headers=heads, data=payload).json()["data"]
 
     '''
         Util Actions
     '''
     def is_supported_region(self, ip):
         URL = f'https://api.zebedee.io/v0/is-supported-region/{ip}'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]
+        except:
+            return requests.get(URL, headers=heads).json()
 
     def get_zbd_prod_server_ip(self):
         URL = f'https://api.zebedee.io/v0/prod-ips'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]
+        except:
+            return requests.get(URL, headers=heads).json()
+
 
     def get_btc_usd_quote_price(self):
         URL = 'https://api.zebedee.io/v0/btcusd'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
-        return requests.get(URL, headers=heads).json()["data"]["btcUsdPrice"]
+        try:
+            return requests.get(URL, headers=heads).json()["data"]["btcUsdPrice"]
+        except:
+            return requests.get(URL, headers=heads).json()
+
     
     def convert_usd_to_sats(self, usd_amount):
         btc_price = self.get_btc_usd_quote_price()
         sats_amount = math.floor(round(int(usd_amount) / int(btc_price), 8) * 100000000)
         return sats_amount
 
     def convert_msats_to_sats(self, amount_sats):
@@ -278,16 +351,19 @@
         URL = 'https://api.zebedee.io/v0/internal-transfer'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
 
         payload = json.dumps({
             "amount": str(amount_msats),
             "receiverWalletId": recevier_wallet_id
         })
+        try:
+            return requests.post(URL, headers=heads, data=payload).json()["data"]
+        except:
+            return requests.post(URL, headers=heads, data=payload).json()
 
-        return requests.post(URL, headers=heads, data=payload).json()["data"]
     
     def get_static_charge_metadata(self, id):
         url = f"https://api.zebedee.io/v0/request-static-charges/{id}"
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
         res = requests.get(url, headers=heads).json()
         return res
```

### Comparing `zebedee-0.0.6/zebedee.egg-info/PKG-INFO` & `zebedee-0.0.7/zebedee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebedee
-Version: 0.0.6
+Version: 0.0.7
 Summary: Move Money at the Speed of the Internet 
 Author: zantoshi (Santos Hernandez)
 Author-email: <santosdhernandez@gmail.com>
 Keywords: python,payments,bitcoin,lightning network,django,lightning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

