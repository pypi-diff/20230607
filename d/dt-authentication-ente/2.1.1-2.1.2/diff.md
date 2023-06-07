# Comparing `tmp/dt-authentication-ente-2.1.1.tar.gz` & `tmp/dt-authentication-ente-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt-authentication-ente-2.1.1.tar", last modified: Tue May 30 05:45:56 2023, max compression
+gzip compressed data, was "dt-authentication-ente-2.1.2.tar", last modified: Wed Jun  7 13:37:21 2023, max compression
```

## Comparing `dt-authentication-ente-2.1.1.tar` & `dt-authentication-ente-2.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-30 05:45:56.003044 dt-authentication-ente-2.1.1/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       34 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.1/MANIFEST.in
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-30 05:45:56.003044 dt-authentication-ente-2.1.1/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      400 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.1/README.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-05-30 05:45:56.003044 dt-authentication-ente-2.1.1/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2374 2023-05-23 13:18:48.000000 dt-authentication-ente-2.1.1/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-30 05:45:55.999044 dt-authentication-ente-2.1.1/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-30 05:45:55.999044 dt-authentication-ente-2.1.1/src/dt_authentication/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2023-05-30 05:45:54.000000 dt-authentication-ente-2.1.1/src/dt_authentication/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3659 2023-05-30 05:44:24.000000 dt-authentication-ente-2.1.1/src/dt_authentication/cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      482 2023-05-22 20:16:11.000000 dt-authentication-ente-2.1.1/src/dt_authentication/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2194 2023-05-07 07:05:57.000000 dt-authentication-ente-2.1.1/src/dt_authentication/scope.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    13360 2023-05-30 05:44:24.000000 dt-authentication-ente-2.1.1/src/dt_authentication/token.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1415 2023-05-22 20:52:39.000000 dt-authentication-ente-2.1.1/src/dt_authentication/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-30 05:45:56.003044 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      524 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      179 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-07 13:37:21.208474 dt-authentication-ente-2.1.2/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       34 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.2/MANIFEST.in
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-06-07 13:37:21.208474 dt-authentication-ente-2.1.2/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      400 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.2/README.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-06-07 13:37:21.208474 dt-authentication-ente-2.1.2/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2374 2023-05-23 13:18:48.000000 dt-authentication-ente-2.1.2/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-07 13:37:21.204474 dt-authentication-ente-2.1.2/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-07 13:37:21.208474 dt-authentication-ente-2.1.2/src/dt_authentication/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2023-06-07 13:37:19.000000 dt-authentication-ente-2.1.2/src/dt_authentication/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3659 2023-05-30 05:44:24.000000 dt-authentication-ente-2.1.2/src/dt_authentication/cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      741 2023-06-07 13:33:39.000000 dt-authentication-ente-2.1.2/src/dt_authentication/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2194 2023-05-07 07:05:57.000000 dt-authentication-ente-2.1.2/src/dt_authentication/scope.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    13453 2023-06-07 13:35:36.000000 dt-authentication-ente-2.1.2/src/dt_authentication/token.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1415 2023-05-22 20:52:39.000000 dt-authentication-ente-2.1.2/src/dt_authentication/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-07 13:37:21.208474 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      524 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      179 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-06-07 13:37:21.000000 dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/top_level.txt
```

### Comparing `dt-authentication-ente-2.1.1/setup.py` & `dt-authentication-ente-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.1.1/src/dt_authentication/cli.py` & `dt-authentication-ente-2.1.2/src/dt_authentication/cli.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.1.1/src/dt_authentication/scope.py` & `dt-authentication-ente-2.1.2/src/dt_authentication/scope.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.1.1/src/dt_authentication/token.py` & `dt-authentication-ente-2.1.2/src/dt_authentication/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,18 @@
         # parse scope
         if "scope" in payload:
             payload["scope"] = [Scope.parse(s) for s in payload["scope"]]
         # create token object
         token = DuckietownToken(version, payload, signature)
         # make sure the token is not expired
         if not allow_expired and token.expired:
-            raise ExpiredToken("This token is expired. Obtain a new one.")
+            raise ExpiredToken(
+                token.expiration,
+                f"This token is expired on '{str(token.expiration)}'. Obtain a new one"
+            )
         # ---
         return token
 
     @classmethod
     def generate(cls, key: SigningKey, user_id: int, *,
                  # duration
                  days: int = 0, hours: int = 0, minutes: int = 0,
```

### Comparing `dt-authentication-ente-2.1.1/src/dt_authentication/utils.py` & `dt-authentication-ente-2.1.2/src/dt_authentication/utils.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/SOURCES.txt` & `dt-authentication-ente-2.1.2/src/dt_authentication_ente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

