# Comparing `tmp/stripe_api_client-0.1.0.tar.gz` & `tmp/stripe_api_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stripe_api_client-0.1.0.tar", max compression
+gzip compressed data, was "stripe_api_client-0.1.1.tar", max compression
```

## Comparing `stripe_api_client-0.1.0.tar` & `stripe_api_client-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-06-07 10:16:48.295067 stripe_api_client-0.1.0/README.md
--rw-r--r--   0        0        0      344 2023-06-07 10:18:02.790220 stripe_api_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       26 2023-06-07 10:30:36.351871 stripe_api_client-0.1.0/stripe_api_client/__init__.py
--rw-r--r--   0        0        0     1345 2023-06-07 10:57:31.456854 stripe_api_client-0.1.0/stripe_api_client/client.py
--rw-r--r--   0        0        0      117 2023-06-07 10:55:06.849167 stripe_api_client-0.1.0/stripe_api_client/resources/__init__.py
--rw-r--r--   0        0        0     1412 2023-06-07 10:39:02.667985 stripe_api_client-0.1.0/stripe_api_client/resources/base.py
--rw-r--r--   0        0        0      538 2023-06-07 10:43:23.129565 stripe_api_client-0.1.0/stripe_api_client/resources/charges.py
--rw-r--r--   0        0        0     1093 2023-06-07 10:52:35.422836 stripe_api_client-0.1.0/stripe_api_client/resources/customers.py
--rw-r--r--   0        0        0      589 2023-06-07 10:50:26.654229 stripe_api_client-0.1.0/stripe_api_client/resources/payment_methods.py
--rw-r--r--   0        0        0      255 2023-06-07 10:20:06.632274 stripe_api_client-0.1.0/stripe_api_client/utils.py
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 stripe_api_client-0.1.0/setup.py
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 stripe_api_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-07 10:16:48.295067 stripe_api_client-0.1.1/README.md
+-rw-r--r--   0        0        0      343 2023-06-07 12:03:49.532384 stripe_api_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-06-07 10:30:36.351871 stripe_api_client-0.1.1/stripe_api_client/__init__.py
+-rw-r--r--   0        0        0     1345 2023-06-07 10:57:31.456854 stripe_api_client-0.1.1/stripe_api_client/client.py
+-rw-r--r--   0        0        0      117 2023-06-07 10:55:06.849167 stripe_api_client-0.1.1/stripe_api_client/resources/__init__.py
+-rw-r--r--   0        0        0     1412 2023-06-07 10:39:02.667985 stripe_api_client-0.1.1/stripe_api_client/resources/base.py
+-rw-r--r--   0        0        0      538 2023-06-07 10:43:23.129565 stripe_api_client-0.1.1/stripe_api_client/resources/charges.py
+-rw-r--r--   0        0        0     1093 2023-06-07 10:52:35.422836 stripe_api_client-0.1.1/stripe_api_client/resources/customers.py
+-rw-r--r--   0        0        0      589 2023-06-07 10:50:26.654229 stripe_api_client-0.1.1/stripe_api_client/resources/payment_methods.py
+-rw-r--r--   0        0        0      255 2023-06-07 10:20:06.632274 stripe_api_client-0.1.1/stripe_api_client/utils.py
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 stripe_api_client-0.1.1/setup.py
+-rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 stripe_api_client-0.1.1/PKG-INFO
```

### Comparing `stripe_api_client-0.1.0/stripe_api_client/client.py` & `stripe_api_client-0.1.1/stripe_api_client/client.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.0/stripe_api_client/resources/base.py` & `stripe_api_client-0.1.1/stripe_api_client/resources/base.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.0/stripe_api_client/resources/charges.py` & `stripe_api_client-0.1.1/stripe_api_client/resources/charges.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.0/stripe_api_client/resources/customers.py` & `stripe_api_client-0.1.1/stripe_api_client/resources/customers.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.0/stripe_api_client/resources/payment_methods.py` & `stripe_api_client-0.1.1/stripe_api_client/resources/payment_methods.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.0/setup.py` & `stripe_api_client-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'stripe-api-client',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '',
     'author': 'Steven Athouel',
     'author_email': 'sathouel@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

