# Comparing `tmp/gopay-1.3.1.tar.gz` & `tmp/gopay-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gopay-1.3.1.tar", last modified: Thu Jun  1 10:15:51 2023, max compression
+gzip compressed data, was "gopay-2.0.0.tar", max compression
```

## Comparing `gopay-1.3.1.tar` & `gopay-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,11 @@
-drwxrwxr-x   0 sfoldesi  (1000) sfoldesi  (1000)        0 2023-06-01 10:15:51.355308 gopay-1.3.1/
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)      113 2023-06-01 09:31:18.000000 gopay-1.3.1/CHANGELOG.md
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     1075 2023-06-01 09:31:18.000000 gopay-1.3.1/LICENSE
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)       50 2023-06-01 09:31:18.000000 gopay-1.3.1/MANIFEST.in
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     9011 2023-06-01 10:15:51.355308 gopay-1.3.1/PKG-INFO
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     8194 2023-06-01 10:05:29.000000 gopay-1.3.1/README.md
-drwxrwxr-x   0 sfoldesi  (1000) sfoldesi  (1000)        0 2023-06-01 10:15:51.347308 gopay-1.3.1/gopay/
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)      709 2023-06-01 09:31:18.000000 gopay-1.3.1/gopay/__init__.py
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     1741 2023-06-01 09:31:18.000000 gopay-1.3.1/gopay/api.py
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     5762 2023-06-01 10:05:29.000000 gopay-1.3.1/gopay/enums.py
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     1256 2023-06-01 09:31:18.000000 gopay-1.3.1/gopay/http.py
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     2220 2023-06-01 09:31:18.000000 gopay-1.3.1/gopay/oauth2.py
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     4674 2023-06-01 10:05:29.000000 gopay-1.3.1/gopay/payments.py
-drwxrwxr-x   0 sfoldesi  (1000) sfoldesi  (1000)        0 2023-06-01 10:15:51.355308 gopay-1.3.1/gopay.egg-info/
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     9011 2023-06-01 10:15:51.000000 gopay-1.3.1/gopay.egg-info/PKG-INFO
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)      299 2023-06-01 10:15:51.000000 gopay-1.3.1/gopay.egg-info/SOURCES.txt
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)        1 2023-06-01 10:15:51.000000 gopay-1.3.1/gopay.egg-info/dependency_links.txt
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)       27 2023-06-01 10:15:51.000000 gopay-1.3.1/gopay.egg-info/requires.txt
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)        6 2023-06-01 10:15:51.000000 gopay-1.3.1/gopay.egg-info/top_level.txt
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)      108 2023-06-01 10:15:51.355308 gopay-1.3.1/setup.cfg
--rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     1173 2023-06-01 10:08:44.000000 gopay-1.3.1/setup.py
+-rw-r--r--   0        0        0     1075 2023-06-05 14:15:56.541156 gopay-2.0.0/LICENSE
+-rw-r--r--   0        0        0     9214 2023-06-07 17:46:47.082495 gopay-2.0.0/README.md
+-rw-r--r--   0        0        0     1074 2023-06-07 19:27:48.972875 gopay-2.0.0/gopay/__init__.py
+-rw-r--r--   0        0        0     2078 2023-06-07 19:43:18.722194 gopay-2.0.0/gopay/api.py
+-rw-r--r--   0        0        0     6017 2023-06-07 15:59:32.469096 gopay-2.0.0/gopay/enums.py
+-rw-r--r--   0        0        0     4707 2023-06-07 19:48:11.894502 gopay-2.0.0/gopay/http.py
+-rw-r--r--   0        0        0      421 2023-06-07 19:18:42.537102 gopay-2.0.0/gopay/models.py
+-rw-r--r--   0        0        0     4797 2023-06-07 19:37:46.464213 gopay-2.0.0/gopay/payments.py
+-rw-r--r--   0        0        0     1612 2023-06-07 19:50:57.714267 gopay-2.0.0/gopay/services.py
+-rw-r--r--   0        0        0     1145 2023-06-07 19:18:36.705128 gopay-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10225 1970-01-01 00:00:00.000000 gopay-2.0.0/PKG-INFO
```

### Comparing `gopay-1.3.1/LICENSE` & `gopay-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gopay-1.3.1/PKG-INFO` & `gopay-2.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,15 @@
-Metadata-Version: 2.1
-Name: gopay
-Version: 1.3.1
-Home-page: https://github.com/gopaycommunity/gopay-python-sdk
-Author: GoPay
-Author-email: integrace@gopay.cz
-License: MIT
-Keywords: gopay payments sdk rest api
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # GoPay's Python SDK for Payments REST API
 
 [![Build Status](https://travis-ci.org/gopaycommunity/gopay-python-api.svg?branch=master)](https://travis-ci.org/gopaycommunity/gopay-python-api)
 
 ## Requirements
 
-- Python >= 3.7
+- Python >= 3.8.1
 - dependencies:
   - [`requests`](https://github.com/kennethreitz/requests)
   - [`deprecated`](https://github.com/tantale/deprecated)
 
 ## Installation
 
 The simplest way to install SDK is to use [PIP](https://docs.python.org/3/installing/):
@@ -39,205 +18,217 @@
 pip install gopay
 ```
 
 ## Basic usage
 
 ```python
 import gopay
+from gopay.enums import TokenScope, Language
 
 # minimal configuration
 payments = gopay.payments({
-    'goid': 'my goid',
-    'clientId': 'my id',
-    'clientSecret': 'my secret',
-  'gatewayUrl': 'url'
+    "goid": "{{YOUR-GOID}}",
+    "client_id": "{{YOUR-CLIENT-ID}}",
+    "client_secret": "{{YOUR-CLIENT-SECRET}}",
+    "gateway_url": 'https://gw.sandbox.gopay.com/api'
 })
 
 # full configuration
 payments = gopay.payments({
-    'goid': 'my goid',
-    'clientId': 'my id',
-    'clientSecret': 'my secret',
-    'gatewayUrl': 'url/',
-    'scope': gopay.TokenScope.ALL,
-    'language': gopay.Language.CZECH,
-    'timeout': 30
+    "goid": "{{YOUR-GOID}}",
+    "client_id": "{{YOUR-CLIENT-ID}}",
+    "client_secret": "{{YOUR-CLIENT-SECRET}}",
+    "gateway_url": 'https://gw.sandbox.gopay.com/api'
+    "scope": TokenScope.ALL,
+    "language": Language.CZECH
 })
+
+# Sandbox URL: https://gw.sandbox.gopay.com/api
+# Production URL: https://gate.gopay.cz/api
 ```
 
 ### Configuration
 
 #### Required fields
 
 Required field | Data type | Documentation |
 -------------- | --------- | ----------- |
-`goid` | string | default GoPay account used in `createPayment` if `target` is not specified
-`clientId` | string | <https://doc.gopay.com/#access-token> |
-`clientSecret` | string | <https://doc.gopay.com/#access-token> |
-`gatewayUrl` | string | [test or production environment?](https://help.gopay.com/en/s/uY) |
+`goid` | string | GoID assigned by GoPay (production or sandbox) |
+`client_id` | string | Client ID assigned by GoPay (production or sandbox) |
+`client_secret` | string | Client Secret assigned by GoPay (production or sandbox) |
+`gateway_url` | string | URL of the environment - production or sandbox (see [Docs](https://doc.gopay.com)) |
 
 #### Optional fields
 
 Optional field | Data type | Default value | Documentation |
 -------------- | --------- | ------------- | ------------- |
-`scope` | string | [`GoPay\Definition\TokenScope::ALL`](src/Definition/TokenScope.php) | <https://doc.gopay.com/#access-token> |
-`language` | string | [`GoPay\Definition\Language::ENGLISH`](src/Definition/Language.php) | language used in `createPayment` if `lang` is not specified + used for [localization of errors](https://doc.gopay.com/#errors)
-`timeout` | int | 30 | Browser timeout in seconds |
+`scope` | string | [`gopay.enums.TokenScope.ALL`](gopay/enums.py) | <https://doc.gopay.com/#access-token> |
+`language` | string | [`gopay.enums.Language.ENGLISH`](gopay/enums.py) | default language to use + [localization of errors](https://doc.gopay.com/#error)
 
 ### Available methods
 
 API | SDK method |
 --- | ---------- |
-[Create standard payment](https://doc.gopay.com/#payment-creation) | `$gopay->createPayment(array $payment)` |
-[Status of the payment](https://doc.gopay.com/#payment-status) | `$gopay->getStatus($id)` |
-[Refund of the payment](https://doc.gopay.com/#payment-refund) | `$gopay->refundPayment($id, $amount)` |
-[Create recurring payment](https://doc.gopay.com/#recurring-payments) | `$gopay->createPayment(array $payment)` |
-[Recurring payment on demand](https://doc.gopay.com/#recurring-on-demand) | `$gopay->createRecurrence($id, array $payment)` |
-[Cancellation of the recurring payment](https://doc.gopay.com/#recurring-payment-cancellation) | `$gopay->voidRecurrence($id)` |
-[Create pre-authorized payment](https://doc.gopay.com/#preauthorized-payments) | `$gopay->createPayment(array $payment)` |
-[Charge of pre-authorized payment](https://doc.gopay.com/#capturing-a-preauthorized-payment) | `$gopay->captureAuthorization($id)` |
-[Cancellation of the pre-authorized payment](https://doc.gopay.com/#cancelling-a-preauthorized-payment) | `$gopay->voidAuthorization($id)` |
+[Create a payment](https://doc.gopay.com#payment-creation) | `payments.create_payment(payment: dict)` |
+[Get status of a payment](https://doc.gopay.com#payment-inquiry) | `payments.get_status(payment_id: str \| int)` |
+[Refund a payment](https://doc.gopay.com#payment-refund) | `payments.refund_payment(payment_id: int \| str, amount: int)` |
+[Create a recurring payment](https://doc.gopay.com#creating-a-recurrence) | `payments.create_recurrence(payment_id: int \| str, payment: dict)` |
+[Cancel a recurring payment](https://doc.gopay.com#void-a-recurring-payment) | `payments.void_recurrence(payment_id: int \| str)` |
+[Capture a preauthorized payment](https://doc.gopay.com#capturing-a-preauthorized-payment) | `payments.capture_authorization(payment_id: int \| str)` |
+[Capture a preauthorized payment partially](https://doc.gopay.com#partially-capturing-a-preauthorized-payment) | `payments.capture_authorization_partial(payment_id: int \| str, payment: dict)` |
+[Void a preauthorized payment](https://doc.gopay.com#voiding-a-preauthorized-payment) | `payments.void_authorization(payment_id: int \| str)` |
+[Get payment card details](https://doc.gopay.com#payment-card-inquiry) | `payments.get_card_details(card_id: int \| str)` |
+[Delete a saved card](https://doc.gopay.com#payment-card-deletion) | `payments.delete_card(card_id: int \| str)` |
+[Get allowed payment methods for a currency](https://doc.gopay.com#available-payment-methods-for-a-currency) | `payments.get_payment_instruments(goid: int \| str, currency: gopay.enums.Currency)` |
+[Get all allowed payment methods](https://doc.gopay.com#all-available-payment-methods) | `payments.get_payment_instruments_all(goid: int \| str)` |
+[Generate an account statement](https://doc.gopay.com#account-statement) | `payments.get_account_statement(statement_request: dict)`
 
 ### SDK response? Has my call succeed?
 
 SDK returns wrapped API response. Every method returns
-[`GoPay\Http\Response` object](src/Http/Response.php). Structure of `json/__toString`
-should be same as in [documentation](https://doc.gopay.com/en).
+[`gopay.http.Response` object](gopay/http.py). Structure of the `json`
+should be same as in [documentation](https://doc.gopay.com).
 SDK throws no exception. Please create an issue if you catch one.
 
 ```python
-response = payments.create_payment({...})
-if response.has_succeed():
-    print("hooray, API returned " + str(response))
-    return response.json['gw_url'] # url for initiation of gateway
+response = payments.create_payment(...)
+if response.success:
+    print(f"Hooray, API returned {response}")
+    return response.json["gw_url"] # url for initiation of gateway
 else:
-    # errors format: https://doc.gopay.com/en/?shell#http-result-codes
-    print("oops, API returned " + str(response.status_code) + ": " + str(response))
+    # errors format: https://doc.gopay.com#HTTP-result-codes
+    print(f"Oops, API returned  {response.status_code}: {response}")
 ```
 
-Method | Description |
+Property/Method | Description |
 ------ | ---------- |
-`response.has_succeed()` | checks if API returns status code _200_ |
-`response.json` | decoded response, returned objects are converted into associative arrays |
+`response.success` | Checks if API call was successful |
+`response.json` | decoded response, returned objects are converted into a dictionary if possiblem |
 `response.status_code` | HTTP status code |
-`response.__str__()` | raw body from HTTP response |
+`response.raw_body` | raw bytes of the reponse content
 
 ### Are required fields and allowed values validated?
 
-**No.** API [validates fields](https://doc.gopay.com/#error) pretty extensively
-so there is no need to duplicate validation in SDK. It would only introduce new type of error.
-Or we would have to perfectly simulate API error messages. That's why SDK just calls API which
+**Not yet.** API [validates fields](https://doc.gopay.com/#error) pretty extensively
+so there is no need to duplicate validation in SDK. That's why SDK just calls API which
 behavior is well documented in [doc.gopay.com](https://doc.gopay.com).
+In the future, we might use Pydantic for parsing and validation.
 
 *****
 
 ## Advanced usage
 
 ### Initiation of the payment gateway
 
 ```python
-# create payment and pass url to template
-response = payments.create_payment({})
+# create payment and pass url to template (e.g. Flask, Django)
+response = payments.create_payment(...)
 if response.has_succeed():
-    templateParameters = {
-        'gatewayUrl': response.json['gw_url'],
-        'embedJs': gopay.url_to_embedjs()
+    context = {
+        'gateway_url': response.json['gw_url'],
+        'embedjs_url': payments.get_embedjs_url
     }
     # render template
 ```
 
-#### [Inline gateway](https://doc.gopay.com/#inline)
+#### [Inline gateway](https://doc.gopay.com#inline)
 
 ```jinja
-<form action="<%= $gatewayUrl %>" method="post" id="gopay-payment-button">
+<form action="{{ gateway_url }}" method="post" id="gopay-payment-button">
   <button name="pay" type="submit">Pay</button>
-  <script type="text/javascript" src="<%= $embedJs %>"></script>
+  <script type="text/javascript" src="{{ embedjs_url }}"></script>
 </form>
 ```
 
-#### [Redirect gateway](https://doc.gopay.com/#redirect)
+#### [Redirect gateway](https://doc.gopay.com#redirect)
 
 ```jinja
-<form action="<%= $gatewayUrl %>" method="post">
+<form action="{{ gateway_url }}" method="post">
   <button name="pay" type="submit">Pay</button>
 </form>
 ```
 
-#### [Asynchronous initialization using JavaScript](/examples/js-initialization.md)
+#### [Asynchronous initialization using JavaScript](https://doc.gopay.com#inline)
 
-### Enums ([Code lists](https://doc.gopay.com/#ciselniky)
+### [Enums](https://doc.gopay.com#enums)
 
 Instead of hardcoding bank codes string you can use predefined enums.
 Check using enums in  [create-payment example](/examples/create_payment.py)
 
 Type | Description |
 ---- | ----------- |
 [Language](/gopay/enums.py) | Payment language, localization of error messages |
 [Token scope](/gopay/enums.py) | Authorization scope for [OAuth2](https://doc.gopay.com/en/#oauth) |
 [Payment enums](/gopay/enums.py) | Enums for creating payment |
 [Response enums](/gopay/enums.py) | Result of creating payment, executing payment operations |
 
 ### Cache access token
 
 Access token expires after 30 minutes it's expensive to use new token for every request.
-Unfortunately it's default behavior of [`gopay.oauth2.InMemoryTokenCache`](/gopay/oauth2.py).
+By default, tokens are stored in memory [`gopay.services.DefaultCache`](/gopay/services.py) so they are reused as long as the object exists.
 But you can implement your cache and store tokens in Memcache, Redis, files, ... It's up to you.
 
-Your cache must implement template methods `get_token` and `set_token`.
+Your cache should inherit from [`gopay.services.AbstractCache`](/gopay/services.py) and implement its methods `get_token` and `set_token`.
 Be aware that there are two [scopes](https://doc.gopay.com/#access-token) (`TokenScope`) and
-SDK can be used for different clients (`clientId`, `gatewayUrl`). So `client` passed to
-methods is unique identifier (`string`) that is built for current environment.
+SDK can be used for different clients (`client_id`, `gateway_url`). So `key` passed to methods is unique identifier (`str`) that is built for current environment.
 Below you can see example implementation of caching tokens in memory:
 
 ```python
-# register cache in optional service configuration
-payments = gopay.payments(
-    {}, # your config
-    {'cache': MyCache()}
-)
-```
+from gopay.services import AbstractCache
+from gopay.http import AccessToken
 
-```python
-class MyCache:
+class MyCache(AbstractCache):
     def __init__(self):
-        self.tokens = {}
+        self.tokens: dict[str, AccessToken] = {}
+
+    def get_token(self, key: str) -> AccessToken | None:
+        return self.tokens.get(key) # return None if token doesn't exist
 
-    def get_token(self, client):
-        return self.tokens.get(client) # return None if token not exists
+    def set_token(self, key: str, token: AccessToken) -> None:
+        self.tokens[key] = token
 
-    def set_token(self, client, token):
-        self.tokens[client] = token
+# register cache in optional service configuration
+payments = gopay.payments(
+    {...}, # your config
+    {"cache": MyCache()}
+)
 ```
 
 ### Log HTTP communication
 
 You can log every request and response from communication with API. Check available loggers below.
-Or you can implement your own logger, just implement function that takes two arguments:
-[`gopay.http.request`](/gopay/http.py) and [`gopay.http.response`](/gopay/http.py).
+Or you can implement your own logger, just implement function that matches the following signature:
 
 ```python
-# register logger in optional service configuration
-payments = gopay.payments(
-    {}, # your config
-    {'logger': my_logger}
-)
+def logger(gopay.http.Request, gopay.http.Response) -> Any: ...
+# or
+Callable[[gopay.http.Response, gopay.http.Request], Any]
+```
+
+For example:
 
-def my_logger(request, response):
+```python
+from gopay.http import Request, Response
+
+def my_logger(request: Request, response: Response) -> None:
     print(vars(request))
     print(vars(response))
+
+# register logger in optional service configuration
+payments = gopay.payments(
+    {...}, # your config
+    {"logger": my_logger}
+)
 ```
 
-Available logger | Description |
----------------- | ----------- |
-[gopay.http.null_logger](/gopay/http.py) | Default logger which does nothing |
-[tests.remote.debug_logger](/tests/remote/__init__.py) | Prints request and response in [remote tests](tests/remote/) |
+The default logger uses `logging.debug` to log the responses and requests.
 
 ## Contributing
 
 Contributions from others would be very much appreciated! Send
 [pull request](https://github.com/gopaycommunity/gopay-python-api/pulls)/
 [issue](https://github.com/gopaycommunity/gopay-python-api/issues). Thanks!
 
 ## License
 
-Copyright (c) 2021 GoPay.com. MIT Licensed,
+Copyright (c) 2023 GoPay.com. MIT Licensed,
 see [LICENSE](https://github.com/gopaycommunity/gopay-python-api/blob/master/LICENSE) for details.
```

### Comparing `gopay-1.3.1/README.md` & `gopay-2.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,40 @@
+Metadata-Version: 2.1
+Name: gopay
+Version: 2.0.0
+Summary: GoPay's Python SDK for Payments REST API
+Home-page: https://github.com/gopaycommunity/gopay-python-api
+License: MIT
+Keywords: gopay,payments,sdk,rest,api
+Author: GoPay
+Author-email: integrace@gopay.cz
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: deprecated (>=1.2.14,<2.0.0)
+Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Documentation, https://doc.gopay.com
+Project-URL: Repository, https://github.com/gopaycommunity/gopay-python-api
+Description-Content-Type: text/markdown
+
 
 # GoPay's Python SDK for Payments REST API
 
 [![Build Status](https://travis-ci.org/gopaycommunity/gopay-python-api.svg?branch=master)](https://travis-ci.org/gopaycommunity/gopay-python-api)
 
 ## Requirements
 
-- Python >= 3.7
+- Python >= 3.8.1
 - dependencies:
   - [`requests`](https://github.com/kennethreitz/requests)
   - [`deprecated`](https://github.com/tantale/deprecated)
 
 ## Installation
 
 The simplest way to install SDK is to use [PIP](https://docs.python.org/3/installing/):
@@ -18,205 +43,218 @@
 pip install gopay
 ```
 
 ## Basic usage
 
 ```python
 import gopay
+from gopay.enums import TokenScope, Language
 
 # minimal configuration
 payments = gopay.payments({
-    'goid': 'my goid',
-    'clientId': 'my id',
-    'clientSecret': 'my secret',
-  'gatewayUrl': 'url'
+    "goid": "{{YOUR-GOID}}",
+    "client_id": "{{YOUR-CLIENT-ID}}",
+    "client_secret": "{{YOUR-CLIENT-SECRET}}",
+    "gateway_url": 'https://gw.sandbox.gopay.com/api'
 })
 
 # full configuration
 payments = gopay.payments({
-    'goid': 'my goid',
-    'clientId': 'my id',
-    'clientSecret': 'my secret',
-    'gatewayUrl': 'url/',
-    'scope': gopay.TokenScope.ALL,
-    'language': gopay.Language.CZECH,
-    'timeout': 30
+    "goid": "{{YOUR-GOID}}",
+    "client_id": "{{YOUR-CLIENT-ID}}",
+    "client_secret": "{{YOUR-CLIENT-SECRET}}",
+    "gateway_url": 'https://gw.sandbox.gopay.com/api'
+    "scope": TokenScope.ALL,
+    "language": Language.CZECH
 })
+
+# Sandbox URL: https://gw.sandbox.gopay.com/api
+# Production URL: https://gate.gopay.cz/api
 ```
 
 ### Configuration
 
 #### Required fields
 
 Required field | Data type | Documentation |
 -------------- | --------- | ----------- |
-`goid` | string | default GoPay account used in `createPayment` if `target` is not specified
-`clientId` | string | <https://doc.gopay.com/#access-token> |
-`clientSecret` | string | <https://doc.gopay.com/#access-token> |
-`gatewayUrl` | string | [test or production environment?](https://help.gopay.com/en/s/uY) |
+`goid` | string | GoID assigned by GoPay (production or sandbox) |
+`client_id` | string | Client ID assigned by GoPay (production or sandbox) |
+`client_secret` | string | Client Secret assigned by GoPay (production or sandbox) |
+`gateway_url` | string | URL of the environment - production or sandbox (see [Docs](https://doc.gopay.com)) |
 
 #### Optional fields
 
 Optional field | Data type | Default value | Documentation |
 -------------- | --------- | ------------- | ------------- |
-`scope` | string | [`GoPay\Definition\TokenScope::ALL`](src/Definition/TokenScope.php) | <https://doc.gopay.com/#access-token> |
-`language` | string | [`GoPay\Definition\Language::ENGLISH`](src/Definition/Language.php) | language used in `createPayment` if `lang` is not specified + used for [localization of errors](https://doc.gopay.com/#errors)
-`timeout` | int | 30 | Browser timeout in seconds |
+`scope` | string | [`gopay.enums.TokenScope.ALL`](gopay/enums.py) | <https://doc.gopay.com/#access-token> |
+`language` | string | [`gopay.enums.Language.ENGLISH`](gopay/enums.py) | default language to use + [localization of errors](https://doc.gopay.com/#error)
 
 ### Available methods
 
 API | SDK method |
 --- | ---------- |
-[Create standard payment](https://doc.gopay.com/#payment-creation) | `$gopay->createPayment(array $payment)` |
-[Status of the payment](https://doc.gopay.com/#payment-status) | `$gopay->getStatus($id)` |
-[Refund of the payment](https://doc.gopay.com/#payment-refund) | `$gopay->refundPayment($id, $amount)` |
-[Create recurring payment](https://doc.gopay.com/#recurring-payments) | `$gopay->createPayment(array $payment)` |
-[Recurring payment on demand](https://doc.gopay.com/#recurring-on-demand) | `$gopay->createRecurrence($id, array $payment)` |
-[Cancellation of the recurring payment](https://doc.gopay.com/#recurring-payment-cancellation) | `$gopay->voidRecurrence($id)` |
-[Create pre-authorized payment](https://doc.gopay.com/#preauthorized-payments) | `$gopay->createPayment(array $payment)` |
-[Charge of pre-authorized payment](https://doc.gopay.com/#capturing-a-preauthorized-payment) | `$gopay->captureAuthorization($id)` |
-[Cancellation of the pre-authorized payment](https://doc.gopay.com/#cancelling-a-preauthorized-payment) | `$gopay->voidAuthorization($id)` |
+[Create a payment](https://doc.gopay.com#payment-creation) | `payments.create_payment(payment: dict)` |
+[Get status of a payment](https://doc.gopay.com#payment-inquiry) | `payments.get_status(payment_id: str \| int)` |
+[Refund a payment](https://doc.gopay.com#payment-refund) | `payments.refund_payment(payment_id: int \| str, amount: int)` |
+[Create a recurring payment](https://doc.gopay.com#creating-a-recurrence) | `payments.create_recurrence(payment_id: int \| str, payment: dict)` |
+[Cancel a recurring payment](https://doc.gopay.com#void-a-recurring-payment) | `payments.void_recurrence(payment_id: int \| str)` |
+[Capture a preauthorized payment](https://doc.gopay.com#capturing-a-preauthorized-payment) | `payments.capture_authorization(payment_id: int \| str)` |
+[Capture a preauthorized payment partially](https://doc.gopay.com#partially-capturing-a-preauthorized-payment) | `payments.capture_authorization_partial(payment_id: int \| str, payment: dict)` |
+[Void a preauthorized payment](https://doc.gopay.com#voiding-a-preauthorized-payment) | `payments.void_authorization(payment_id: int \| str)` |
+[Get payment card details](https://doc.gopay.com#payment-card-inquiry) | `payments.get_card_details(card_id: int \| str)` |
+[Delete a saved card](https://doc.gopay.com#payment-card-deletion) | `payments.delete_card(card_id: int \| str)` |
+[Get allowed payment methods for a currency](https://doc.gopay.com#available-payment-methods-for-a-currency) | `payments.get_payment_instruments(goid: int \| str, currency: gopay.enums.Currency)` |
+[Get all allowed payment methods](https://doc.gopay.com#all-available-payment-methods) | `payments.get_payment_instruments_all(goid: int \| str)` |
+[Generate an account statement](https://doc.gopay.com#account-statement) | `payments.get_account_statement(statement_request: dict)`
 
 ### SDK response? Has my call succeed?
 
 SDK returns wrapped API response. Every method returns
-[`GoPay\Http\Response` object](src/Http/Response.php). Structure of `json/__toString`
-should be same as in [documentation](https://doc.gopay.com/en).
+[`gopay.http.Response` object](gopay/http.py). Structure of the `json`
+should be same as in [documentation](https://doc.gopay.com).
 SDK throws no exception. Please create an issue if you catch one.
 
 ```python
-response = payments.create_payment({...})
-if response.has_succeed():
-    print("hooray, API returned " + str(response))
-    return response.json['gw_url'] # url for initiation of gateway
+response = payments.create_payment(...)
+if response.success:
+    print(f"Hooray, API returned {response}")
+    return response.json["gw_url"] # url for initiation of gateway
 else:
-    # errors format: https://doc.gopay.com/en/?shell#http-result-codes
-    print("oops, API returned " + str(response.status_code) + ": " + str(response))
+    # errors format: https://doc.gopay.com#HTTP-result-codes
+    print(f"Oops, API returned  {response.status_code}: {response}")
 ```
 
-Method | Description |
+Property/Method | Description |
 ------ | ---------- |
-`response.has_succeed()` | checks if API returns status code _200_ |
-`response.json` | decoded response, returned objects are converted into associative arrays |
+`response.success` | Checks if API call was successful |
+`response.json` | decoded response, returned objects are converted into a dictionary if possiblem |
 `response.status_code` | HTTP status code |
-`response.__str__()` | raw body from HTTP response |
+`response.raw_body` | raw bytes of the reponse content
 
 ### Are required fields and allowed values validated?
 
-**No.** API [validates fields](https://doc.gopay.com/#error) pretty extensively
-so there is no need to duplicate validation in SDK. It would only introduce new type of error.
-Or we would have to perfectly simulate API error messages. That's why SDK just calls API which
+**Not yet.** API [validates fields](https://doc.gopay.com/#error) pretty extensively
+so there is no need to duplicate validation in SDK. That's why SDK just calls API which
 behavior is well documented in [doc.gopay.com](https://doc.gopay.com).
+In the future, we might use Pydantic for parsing and validation.
 
 *****
 
 ## Advanced usage
 
 ### Initiation of the payment gateway
 
 ```python
-# create payment and pass url to template
-response = payments.create_payment({})
+# create payment and pass url to template (e.g. Flask, Django)
+response = payments.create_payment(...)
 if response.has_succeed():
-    templateParameters = {
-        'gatewayUrl': response.json['gw_url'],
-        'embedJs': gopay.url_to_embedjs()
+    context = {
+        'gateway_url': response.json['gw_url'],
+        'embedjs_url': payments.get_embedjs_url
     }
     # render template
 ```
 
-#### [Inline gateway](https://doc.gopay.com/#inline)
+#### [Inline gateway](https://doc.gopay.com#inline)
 
 ```jinja
-<form action="<%= $gatewayUrl %>" method="post" id="gopay-payment-button">
+<form action="{{ gateway_url }}" method="post" id="gopay-payment-button">
   <button name="pay" type="submit">Pay</button>
-  <script type="text/javascript" src="<%= $embedJs %>"></script>
+  <script type="text/javascript" src="{{ embedjs_url }}"></script>
 </form>
 ```
 
-#### [Redirect gateway](https://doc.gopay.com/#redirect)
+#### [Redirect gateway](https://doc.gopay.com#redirect)
 
 ```jinja
-<form action="<%= $gatewayUrl %>" method="post">
+<form action="{{ gateway_url }}" method="post">
   <button name="pay" type="submit">Pay</button>
 </form>
 ```
 
-#### [Asynchronous initialization using JavaScript](/examples/js-initialization.md)
+#### [Asynchronous initialization using JavaScript](https://doc.gopay.com#inline)
 
-### Enums ([Code lists](https://doc.gopay.com/#ciselniky)
+### [Enums](https://doc.gopay.com#enums)
 
 Instead of hardcoding bank codes string you can use predefined enums.
 Check using enums in  [create-payment example](/examples/create_payment.py)
 
 Type | Description |
 ---- | ----------- |
 [Language](/gopay/enums.py) | Payment language, localization of error messages |
 [Token scope](/gopay/enums.py) | Authorization scope for [OAuth2](https://doc.gopay.com/en/#oauth) |
 [Payment enums](/gopay/enums.py) | Enums for creating payment |
 [Response enums](/gopay/enums.py) | Result of creating payment, executing payment operations |
 
 ### Cache access token
 
 Access token expires after 30 minutes it's expensive to use new token for every request.
-Unfortunately it's default behavior of [`gopay.oauth2.InMemoryTokenCache`](/gopay/oauth2.py).
+By default, tokens are stored in memory [`gopay.services.DefaultCache`](/gopay/services.py) so they are reused as long as the object exists.
 But you can implement your cache and store tokens in Memcache, Redis, files, ... It's up to you.
 
-Your cache must implement template methods `get_token` and `set_token`.
+Your cache should inherit from [`gopay.services.AbstractCache`](/gopay/services.py) and implement its methods `get_token` and `set_token`.
 Be aware that there are two [scopes](https://doc.gopay.com/#access-token) (`TokenScope`) and
-SDK can be used for different clients (`clientId`, `gatewayUrl`). So `client` passed to
-methods is unique identifier (`string`) that is built for current environment.
+SDK can be used for different clients (`client_id`, `gateway_url`). So `key` passed to methods is unique identifier (`str`) that is built for current environment.
 Below you can see example implementation of caching tokens in memory:
 
 ```python
-# register cache in optional service configuration
-payments = gopay.payments(
-    {}, # your config
-    {'cache': MyCache()}
-)
-```
+from gopay.services import AbstractCache
+from gopay.http import AccessToken
 
-```python
-class MyCache:
+class MyCache(AbstractCache):
     def __init__(self):
-        self.tokens = {}
+        self.tokens: dict[str, AccessToken] = {}
+
+    def get_token(self, key: str) -> AccessToken | None:
+        return self.tokens.get(key) # return None if token doesn't exist
 
-    def get_token(self, client):
-        return self.tokens.get(client) # return None if token not exists
+    def set_token(self, key: str, token: AccessToken) -> None:
+        self.tokens[key] = token
 
-    def set_token(self, client, token):
-        self.tokens[client] = token
+# register cache in optional service configuration
+payments = gopay.payments(
+    {...}, # your config
+    {"cache": MyCache()}
+)
 ```
 
 ### Log HTTP communication
 
 You can log every request and response from communication with API. Check available loggers below.
-Or you can implement your own logger, just implement function that takes two arguments:
-[`gopay.http.request`](/gopay/http.py) and [`gopay.http.response`](/gopay/http.py).
+Or you can implement your own logger, just implement function that matches the following signature:
 
 ```python
-# register logger in optional service configuration
-payments = gopay.payments(
-    {}, # your config
-    {'logger': my_logger}
-)
+def logger(gopay.http.Request, gopay.http.Response) -> Any: ...
+# or
+Callable[[gopay.http.Response, gopay.http.Request], Any]
+```
+
+For example:
+
+```python
+from gopay.http import Request, Response
 
-def my_logger(request, response):
+def my_logger(request: Request, response: Response) -> None:
     print(vars(request))
     print(vars(response))
+
+# register logger in optional service configuration
+payments = gopay.payments(
+    {...}, # your config
+    {"logger": my_logger}
+)
 ```
 
-Available logger | Description |
----------------- | ----------- |
-[gopay.http.null_logger](/gopay/http.py) | Default logger which does nothing |
-[tests.remote.debug_logger](/tests/remote/__init__.py) | Prints request and response in [remote tests](tests/remote/) |
+The default logger uses `logging.debug` to log the responses and requests.
 
 ## Contributing
 
 Contributions from others would be very much appreciated! Send
 [pull request](https://github.com/gopaycommunity/gopay-python-api/pulls)/
 [issue](https://github.com/gopaycommunity/gopay-python-api/issues). Thanks!
 
 ## License
 
-Copyright (c) 2021 GoPay.com. MIT Licensed,
+Copyright (c) 2023 GoPay.com. MIT Licensed,
 see [LICENSE](https://github.com/gopaycommunity/gopay-python-api/blob/master/LICENSE) for details.
+
```

### Comparing `gopay-1.3.1/gopay/enums.py` & `gopay-2.0.0/gopay/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,56 @@
-class Recurrence:
+from enum import Enum
+
+
+class StrEnum(str, Enum):
+    def __str__(self) -> str:
+        return self.value
+
+
+class Recurrence(StrEnum):
     DAILY = "DAY"
     WEEKLY = "WEEK"
     MONTHLY = "MONTH"
     ON_DEMAND = "ON_DEMAND"
 
 
-class Currency:
+class Currency(StrEnum):
     CZECH_CROWNS = "CZK"
     EUROS = "EUR"
     POLISH_ZLOTY = "PLN"
     HUNGARIAN_FORINT = "HUF"
     BRITISH_POUND = "GBP"
     US_DOLLAR = "USD"
     ROMANIAN_LEU = "RON"
     BULGARIAN_LEV = "BGN"
 
 
-class TokenScope:
+class TokenScope(StrEnum):
     CREATE_PAYMENT = "payment-create"
     ALL = "payment-all"
 
 
-class Result:
+class Result(StrEnum):
     ACCEPTED = "ACCEPTED"
     FINISHED = "FINISHED"
     FAILED = "FAILED"
 
 
-class PaymentStatus:
+class PaymentStatus(StrEnum):
     CREATED = "CREATED"
     PAYMENT_METHOD_CHOSEN = "PAYMENT_METHOD_CHOSEN"
     PAID = "PAID"
     AUTHORIZED = "AUTHORIZED"
     CANCELED = "CANCELED"
     TIMEOUTED = "TIMEOUTED"
     REFUNDED = "REFUNDED"
     PARTIALLY_REFUNDED = "PARTIALLY_REFUNDED"
 
 
-class Language:
+class Language(StrEnum):
     CZECH = "CS"
     ENGLISH = "EN"
     SLOVAK = "SK"
     GERMAN = "DE"
     RUSSIAN = "RU"
     POLISH = "PL"
     HUNGARIAN = "HU"
@@ -56,15 +64,15 @@
     ESTONIAN = "EE"
     LITHUANIAN = "LT"
     LATVIAN = "LV"
     SLOVENIAN = "SI"
     PORTUGUESE = "PT"
 
 
-class PaymentInstrument:
+class PaymentInstrument(StrEnum):
     PAYMENT_CARD = "PAYMENT_CARD"
     BANK_ACCOUNT = "BANK_ACCOUNT"
     PREMIUM_SMS = "PRSMS"
     MPAYMENT = "MPAYMENT"
     PAYSAFECARD = "PAYSAFECARD"
     SUPERCASH = "SUPERCASH"
     GOPAY = "GOPAY"
@@ -72,46 +80,45 @@
     BITCOIN = "BITCOIN"
     GPAY = "GPAY"
     ACCOUNT = "ACCOUNT"
     APPLE_PAY = "APPLE_PAY"
     CLICK_TO_PAY = "CLICK_TO_PAY"
 
 
-class StatementGeneratingFormat:
+class StatementGeneratingFormat(StrEnum):
     XLS_A = "XLS_A"
     XLS_B = "XLS_B"
     XLS_C = "XLS_C"
     CSV_A = "CSV_A"
     CSV_B = "CSV_B"
     CSV_C = "CSV_C"
     CSV_D = "CSV_D"
     CSV_E = "CSV_E"
     ABO_A = "ABO_A"
 
 
-class ItemType:
+class ItemType(StrEnum):
     ITEM = "ITEM"
     DISCOUNT = "DISCOUNT"
     DELIVERY = "DELIVERY"
     POSTAGE = "POSTAGE"
 
 
-
-class EETReceiptState:
+class EETReceiptState(StrEnum):
     CREATED = "CREATED"
     DELIVERY_FAILED = "DELIVERY_FAILED"
     DELIVERED = "DELIVERED"
 
 
-class EETMode:
+class EETMode(StrEnum):
     AUTO = "AUTO"
     EET = "EET"
 
 
-class BankSwiftCode:
+class BankSwiftCode(StrEnum):
     # CZ
     CESKA_SPORITELNA = "GIBACZPX"
     KOMERCNI_BANKA = "KOMBCZPP"
     CSOB = "CEKOCZPP"
     RAIFFEISENBANK = "RZBCCZPP"
     UNICREDIT_BANK_CZ = "BACXCZPP"
     MONETA_MONEY_BANK = "AGBACZPP"
@@ -178,28 +185,28 @@
     E_SKOK = "NBPLPLPW"
     EUROBANK = "SOGEPLPW"
     POLSKI_BANK_PRZEDSIEBIORCZOSCI_SPOLKA_AKCYJNA = "PBPBPLPW"
     # Others
     SPECIAL = "OTHERS"
 
 
-class RecurrenceState:
+class RecurrenceState(StrEnum):
     REQUESTED = "REQUESTED"
     STARTED = "STARTED"
     STOPPED = "STOPPED"
 
 
-class PreAuthState:
+class PreAuthState(StrEnum):
     REQUESTED = "REQUESTED"
     AUTHORIZED = "AUTHORIZED"
     CAPTURED = "CAPTURED"
     CANCELED = "CANCELED"
 
 
-class PaymentSubStatus:
+class PaymentSubStatus(StrEnum):
     _101 = "_101"
     _102 = "_102"
     _3001 = "_3001"
     _3002 = "_3002"
     _3003 = "_3003"
     _5001 = "_5001"
     _5002 = "_5002"
@@ -255,10 +262,10 @@
     _6004 = "_6004"
     _6005 = "_6005"
     _6501 = "_6501"
     _6502 = "_6502"
     _6504 = "_6504"
 
 
-class SupercashSubType:
-    SUB_TYPE_PREPAID = "PREPAID"
-    SUB_TYPE_POSTPAID = "POSTPAID"
+class ContentType(StrEnum):
+    FORM = "application/x-www-form-urlencoded"
+    JSON = "application/json"
```

