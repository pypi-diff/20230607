# Comparing `tmp/ckanext-oidc-pkce-0.2.3.tar.gz` & `tmp/ckanext-oidc-pkce-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-oidc-pkce-0.2.3.tar", last modified: Wed Apr  5 08:38:45 2023, max compression
+gzip compressed data, was "ckanext-oidc-pkce-0.3.0.tar", last modified: Wed Jun  7 13:32:34 2023, max compression
```

## Comparing `ckanext-oidc-pkce-0.2.3.tar` & `ckanext-oidc-pkce-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-05 08:38:45.727184 ckanext-oidc-pkce-0.2.3/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-11 15:10:49.000000 ckanext-oidc-pkce-0.2.3/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      210 2023-03-03 00:07:24.000000 ckanext-oidc-pkce-0.2.3/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3602 2023-04-05 08:38:45.727184 ckanext-oidc-pkce-0.2.3/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2877 2023-03-02 14:45:31.000000 ckanext-oidc-pkce-0.2.3/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-05 08:38:45.717184 ckanext-oidc-pkce-0.2.3/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-11 23:33:00.000000 ckanext-oidc-pkce-0.2.3/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-05 08:38:45.727184 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-11 15:10:49.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3369 2023-03-02 14:10:31.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2365 2023-03-02 14:34:51.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      764 2023-03-02 14:10:29.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2748 2023-04-05 08:08:22.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/interfaces.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1188 2023-04-05 08:29:39.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      560 2023-01-23 02:06:56.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/signals.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-05 08:38:45.727184 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-11 15:10:49.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      314 2023-03-02 14:57:25.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/tests/conftest.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      196 2022-10-11 15:30:08.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1021 2023-03-02 15:00:49.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/tests/test_utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1555 2023-03-02 14:10:31.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3835 2023-04-05 08:29:51.000000 ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-05 08:38:45.727184 ckanext-oidc-pkce-0.2.3/ckanext_oidc_pkce.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3602 2023-04-05 08:38:45.000000 ckanext-oidc-pkce-0.2.3/ckanext_oidc_pkce.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      819 2023-04-05 08:38:45.000000 ckanext-oidc-pkce-0.2.3/ckanext_oidc_pkce.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-04-05 08:38:45.000000 ckanext-oidc-pkce-0.2.3/ckanext_oidc_pkce.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      124 2023-04-05 08:38:45.000000 ckanext-oidc-pkce-0.2.3/ckanext_oidc_pkce.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-05 08:38:45.000000 ckanext-oidc-pkce-0.2.3/ckanext_oidc_pkce.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2023-04-05 08:38:45.000000 ckanext-oidc-pkce-0.2.3/ckanext_oidc_pkce.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-05 08:38:45.000000 ckanext-oidc-pkce-0.2.3/ckanext_oidc_pkce.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2936 2023-03-02 14:09:43.000000 ckanext-oidc-pkce-0.2.3/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-11 15:10:49.000000 ckanext-oidc-pkce-0.2.3/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1576 2023-04-05 08:38:45.727184 ckanext-oidc-pkce-0.2.3/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-11 23:33:00.000000 ckanext-oidc-pkce-0.2.3/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 13:32:34.920220 ckanext-oidc-pkce-0.3.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-11 15:10:49.000000 ckanext-oidc-pkce-0.3.0/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      210 2023-03-03 00:07:24.000000 ckanext-oidc-pkce-0.3.0/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3973 2023-06-07 13:32:34.920220 ckanext-oidc-pkce-0.3.0/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3248 2023-06-07 13:30:35.000000 ckanext-oidc-pkce-0.3.0/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 13:32:34.900221 ckanext-oidc-pkce-0.3.0/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-11 23:33:00.000000 ckanext-oidc-pkce-0.3.0/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 13:32:34.910221 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-11 15:10:49.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3849 2023-06-07 13:30:35.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2365 2023-03-02 14:34:51.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      764 2023-03-02 14:10:29.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2748 2023-04-05 08:08:22.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/interfaces.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1188 2023-04-05 08:29:39.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      560 2023-01-23 02:06:56.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/signals.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 13:32:34.920220 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-11 15:10:49.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      314 2023-03-02 14:57:25.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/tests/conftest.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      196 2022-10-11 15:30:08.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1021 2023-03-02 15:00:49.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/tests/test_utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1555 2023-03-02 14:10:31.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4071 2023-06-07 13:30:35.000000 ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-07 13:32:34.920220 ckanext-oidc-pkce-0.3.0/ckanext_oidc_pkce.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3973 2023-06-07 13:32:34.000000 ckanext-oidc-pkce-0.3.0/ckanext_oidc_pkce.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      819 2023-06-07 13:32:34.000000 ckanext-oidc-pkce-0.3.0/ckanext_oidc_pkce.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-07 13:32:34.000000 ckanext-oidc-pkce-0.3.0/ckanext_oidc_pkce.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      124 2023-06-07 13:32:34.000000 ckanext-oidc-pkce-0.3.0/ckanext_oidc_pkce.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-07 13:32:34.000000 ckanext-oidc-pkce-0.3.0/ckanext_oidc_pkce.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2023-06-07 13:32:34.000000 ckanext-oidc-pkce-0.3.0/ckanext_oidc_pkce.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-07 13:32:34.000000 ckanext-oidc-pkce-0.3.0/ckanext_oidc_pkce.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2936 2023-03-02 14:09:43.000000 ckanext-oidc-pkce-0.3.0/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-11 15:10:49.000000 ckanext-oidc-pkce-0.3.0/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1576 2023-06-07 13:32:34.920220 ckanext-oidc-pkce-0.3.0/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-11 23:33:00.000000 ckanext-oidc-pkce-0.3.0/setup.py
```

### Comparing `ckanext-oidc-pkce-0.2.3/LICENSE` & `ckanext-oidc-pkce-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-oidc-pkce-0.2.3/PKG-INFO` & `ckanext-oidc-pkce-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: ckanext-oidc-pkce
-Version: 0.2.3
-Summary: CKAN OIDC authenticator with PKCE flow
-Home-page: https://github.com/DataShades/ckanext-oidc-pkce
-Author: Sergey Motornyuk
-Author-email: sergey.motornyuk@linkdigital.com.au
-License: AGPL
-Keywords: CKAN,Okta,oidc,pkce,authentication
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 [![Tests](https://github.com/DataShades/ckanext-oidc-pkce/actions/workflows/test.yml/badge.svg)](https://github.com/DataShades/ckanext-oidc-pkce/actions/workflows/test.yml)
 
 # ckanext-oidc-pkce
 
 OpenID connect with PKCE flow authenticator for CKAN.
 
 > **Warning**
@@ -38,15 +19,14 @@
 Compatibility with core CKAN versions:
 
 | CKAN version | Compatible? |
 |--------------|-------------|
 | 2.9          | yes         |
 | 2.10         | yes         |
 
-
 ## Installation
 
 1. Install the package
    ```sh
    pip install ckanext-oidc-pkce
    ```
 
@@ -55,19 +35,26 @@
 
 1. Add SSO settings(refer [config settings](#config-settings) section for details)
 
 ## Config settings
 
 ```ini
 # URL of SSO application
+# Could be overriden at runtime with env var CKANEXT_OIDC_PKCE_BASE_URL
 ckanext.oidc_pkce.base_url = https://12345.example.okta.com
 
 # ClientID of SSO application
+# Could be overriden at runtime with env var CKANEXT_OIDC_PKCE_CLIENT_ID
 ckanext.oidc_pkce.client_id = clientid
 
+# ClientSecret of SSO application
+# (optional, only need id Client App defines a secret, default: "")
+# Could be overriden at runtime with env var CKANEXT_OIDC_PKCE_CLIENT_SECRET
+ckanext.oidc_pkce.client_secret = clientsecret
+
 # Path to the authorization endpont inside SSO application
 # (optional, default: /oauth2/default/v1/authorize)
 ckanext.oidc_pkce.auth_path = /auth
 
 # Path to the token endpont inside SSO application
 # (optional, default: /oauth2/default/v1/token)
 ckanext.oidc_pkce.token_path = /token
```

### Comparing `ckanext-oidc-pkce-0.2.3/README.md` & `ckanext-oidc-pkce-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: ckanext-oidc-pkce
+Version: 0.3.0
+Summary: CKAN OIDC authenticator with PKCE flow
+Home-page: https://github.com/DataShades/ckanext-oidc-pkce
+Author: Sergey Motornyuk
+Author-email: sergey.motornyuk@linkdigital.com.au
+License: AGPL
+Keywords: CKAN,Okta,oidc,pkce,authentication
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 [![Tests](https://github.com/DataShades/ckanext-oidc-pkce/actions/workflows/test.yml/badge.svg)](https://github.com/DataShades/ckanext-oidc-pkce/actions/workflows/test.yml)
 
 # ckanext-oidc-pkce
 
 OpenID connect with PKCE flow authenticator for CKAN.
 
 > **Warning**
@@ -19,15 +38,14 @@
 Compatibility with core CKAN versions:
 
 | CKAN version | Compatible? |
 |--------------|-------------|
 | 2.9          | yes         |
 | 2.10         | yes         |
 
-
 ## Installation
 
 1. Install the package
    ```sh
    pip install ckanext-oidc-pkce
    ```
 
@@ -36,19 +54,26 @@
 
 1. Add SSO settings(refer [config settings](#config-settings) section for details)
 
 ## Config settings
 
 ```ini
 # URL of SSO application
+# Could be overriden at runtime with env var CKANEXT_OIDC_PKCE_BASE_URL
 ckanext.oidc_pkce.base_url = https://12345.example.okta.com
 
 # ClientID of SSO application
+# Could be overriden at runtime with env var CKANEXT_OIDC_PKCE_CLIENT_ID
 ckanext.oidc_pkce.client_id = clientid
 
+# ClientSecret of SSO application
+# (optional, only need id Client App defines a secret, default: "")
+# Could be overriden at runtime with env var CKANEXT_OIDC_PKCE_CLIENT_SECRET
+ckanext.oidc_pkce.client_secret = clientsecret
+
 # Path to the authorization endpont inside SSO application
 # (optional, default: /oauth2/default/v1/authorize)
 ckanext.oidc_pkce.auth_path = /auth
 
 # Path to the token endpont inside SSO application
 # (optional, default: /oauth2/default/v1/token)
 ckanext.oidc_pkce.token_path = /token
```

### Comparing `ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/config.py` & `ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
+import os
 from typing import Optional
 
 import ckan.plugins.toolkit as tk
 from ckan.exceptions import CkanConfigurationException
 
 CONFIG_BASE_URL = "ckanext.oidc_pkce.base_url"
 CONFIG_CLIENT_ID = "ckanext.oidc_pkce.client_id"
+CONFIG_CLIENT_SECRET = "ckanext.oidc_pkce.client_secret"
 
 CONFIG_AUTH_PATH = "ckanext.oidc_pkce.auth_path"
 DEFAULT_AUTH_PATH = "/oauth2/default/v1/authorize"
 
 CONFIG_TOKEN_PATH = "ckanext.oidc_pkce.token_path"
 DEFAULT_TOKEN_PATH = "/oauth2/default/v1/token"
 
@@ -31,30 +33,42 @@
 
 CONFIG_MUNGE_PASSWORD = "ckanext.oidc_pkce.munge_password"
 DEFAULT_MUNGE_PASSWORD = False
 
 
 def client_id() -> str:
     """ClientID for SSO application"""
-    id_ = tk.config.get(CONFIG_CLIENT_ID)
+    id_ = os.environ.get('CKANEXT_OIDC_PKCE_CLIENT_ID')
     if not id_:
-        raise CkanConfigurationException(
-            f"{CONFIG_CLIENT_ID} must be configured"
-        )
+        id_ = tk.config.get(CONFIG_CLIENT_ID)
+        if not id_:
+            raise CkanConfigurationException(
+                f"{CONFIG_CLIENT_ID} must be configured"
+            )
 
     return id_
 
 
+def client_secret() -> str:
+    """ClientSecret for SSO application"""
+    secret_ = os.environ.get('CKANEXT_OIDC_PKCE_CLIENT_SECRET')
+    if not secret_:
+        secret_ = tk.config.get(CONFIG_CLIENT_SECRET)
+    return secret_
+
+
 def base_url() -> str:
     """Base URL of the SSO application."""
-    url = tk.config.get(CONFIG_BASE_URL, None)
+    url = os.environ.get('CKANEXT_OIDC_PKCE_BASE_URL')
     if not url:
-        raise CkanConfigurationException(
-            f"{CONFIG_BASE_URL} must be configured"
-        )
+        url = tk.config.get(CONFIG_BASE_URL, None)
+        if not url:
+            raise CkanConfigurationException(
+                f"{CONFIG_BASE_URL} must be configured"
+            )
 
     return url.rstrip("/")
 
 
 def auth_path() -> str:
     """Path(without base URL) where authentication happens."""
     return tk.config.get(CONFIG_AUTH_PATH, DEFAULT_AUTH_PATH)
```

### Comparing `ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/config_declaration.yaml` & `ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/config_declaration.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/helpers.py` & `ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/interfaces.py` & `ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/plugin.py` & `ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/signals.py` & `ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/signals.py`

 * *Files identical despite different names*

### Comparing `ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/tests/test_utils.py` & `ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/utils.py` & `ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-oidc-pkce-0.2.3/ckanext/oidc_pkce/views.py` & `ckanext-oidc-pkce-0.3.0/ckanext/oidc_pkce/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import base64
 import logging
 from urllib.parse import urlencode
 
 import requests
 from flask import Blueprint
 
 import ckan.plugins.toolkit as tk
@@ -87,14 +88,19 @@
         return tk.redirect_to(came_from)
 
     headers = {
         "accept": "application/json",
         "cache-control": "no-cache",
         "content-type": "application/x-www-form-urlencoded",
     }
+    
+    if config.client_secret():
+        auth_header: str = config.client_id() + ":" + config.client_secret()
+        headers["Authorization"] = "Basic " + base64.b64encode(auth_header.encode('ascii')).decode('ascii')
+
     data = {
         "grant_type": "authorization_code",
         "client_id": config.client_id(),
         "redirect_uri": config.redirect_url(),
         "code": code,
         "code_verifier": verifier,
     }
```

### Comparing `ckanext-oidc-pkce-0.2.3/ckanext_oidc_pkce.egg-info/PKG-INFO` & `ckanext-oidc-pkce-0.3.0/ckanext_oidc_pkce.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-oidc-pkce
-Version: 0.2.3
+Version: 0.3.0
 Summary: CKAN OIDC authenticator with PKCE flow
 Home-page: https://github.com/DataShades/ckanext-oidc-pkce
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN,Okta,oidc,pkce,authentication
 Classifier: Development Status :: 4 - Beta
@@ -38,15 +38,14 @@
 Compatibility with core CKAN versions:
 
 | CKAN version | Compatible? |
 |--------------|-------------|
 | 2.9          | yes         |
 | 2.10         | yes         |
 
-
 ## Installation
 
 1. Install the package
    ```sh
    pip install ckanext-oidc-pkce
    ```
 
@@ -55,19 +54,26 @@
 
 1. Add SSO settings(refer [config settings](#config-settings) section for details)
 
 ## Config settings
 
 ```ini
 # URL of SSO application
+# Could be overriden at runtime with env var CKANEXT_OIDC_PKCE_BASE_URL
 ckanext.oidc_pkce.base_url = https://12345.example.okta.com
 
 # ClientID of SSO application
+# Could be overriden at runtime with env var CKANEXT_OIDC_PKCE_CLIENT_ID
 ckanext.oidc_pkce.client_id = clientid
 
+# ClientSecret of SSO application
+# (optional, only need id Client App defines a secret, default: "")
+# Could be overriden at runtime with env var CKANEXT_OIDC_PKCE_CLIENT_SECRET
+ckanext.oidc_pkce.client_secret = clientsecret
+
 # Path to the authorization endpont inside SSO application
 # (optional, default: /oauth2/default/v1/authorize)
 ckanext.oidc_pkce.auth_path = /auth
 
 # Path to the token endpont inside SSO application
 # (optional, default: /oauth2/default/v1/token)
 ckanext.oidc_pkce.token_path = /token
```

### Comparing `ckanext-oidc-pkce-0.2.3/ckanext_oidc_pkce.egg-info/SOURCES.txt` & `ckanext-oidc-pkce-0.3.0/ckanext_oidc_pkce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-oidc-pkce-0.2.3/pyproject.toml` & `ckanext-oidc-pkce-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-oidc-pkce-0.2.3/setup.cfg` & `ckanext-oidc-pkce-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-oidc-pkce
-version = 0.2.3
+version = 0.3.0
 description = CKAN OIDC authenticator with PKCE flow
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-oidc-pkce
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

### Comparing `ckanext-oidc-pkce-0.2.3/setup.py` & `ckanext-oidc-pkce-0.3.0/setup.py`

 * *Files identical despite different names*

