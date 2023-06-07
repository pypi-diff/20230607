# Comparing `tmp/pdpyras-5.0.3.tar.gz` & `tmp/pdpyras-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpyras-5.0.3.tar", last modified: Wed May 17 21:04:26 2023, max compression
+gzip compressed data, was "pdpyras-5.0.4.tar", last modified: Wed Jun  7 20:41:28 2023, max compression
```

## Comparing `pdpyras-5.0.3.tar` & `pdpyras-5.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-17 21:04:26.476956 pdpyras-5.0.3/
--rw-r--r--   0 demitri    (503) staff       (20)     1053 2023-05-01 18:31:04.000000 pdpyras-5.0.3/LICENSE
--rw-r--r--   0 demitri    (503) staff       (20)      374 2023-05-17 21:04:26.476821 pdpyras-5.0.3/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)     4792 2023-05-01 18:31:04.000000 pdpyras-5.0.3/README.rst
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-17 21:04:26.476641 pdpyras-5.0.3/pdpyras.egg-info/
--rw-r--r--   0 demitri    (503) staff       (20)      374 2023-05-17 21:04:26.000000 pdpyras-5.0.3/pdpyras.egg-info/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)      192 2023-05-17 21:04:26.000000 pdpyras-5.0.3/pdpyras.egg-info/SOURCES.txt
--rw-r--r--   0 demitri    (503) staff       (20)        1 2023-05-17 21:04:26.000000 pdpyras-5.0.3/pdpyras.egg-info/dependency_links.txt
--rw-r--r--   0 demitri    (503) staff       (20)       29 2023-05-17 21:04:26.000000 pdpyras-5.0.3/pdpyras.egg-info/requires.txt
--rw-r--r--   0 demitri    (503) staff       (20)        8 2023-05-17 21:04:26.000000 pdpyras-5.0.3/pdpyras.egg-info/top_level.txt
--rw-r--r--   0 demitri    (503) staff       (20)    86839 2023-05-17 21:04:23.000000 pdpyras-5.0.3/pdpyras.py
--rw-r--r--   0 demitri    (503) staff       (20)       38 2023-05-17 21:04:26.477009 pdpyras-5.0.3/setup.cfg
--rw-r--r--   0 demitri    (503) staff       (20)      657 2023-05-17 21:04:23.000000 pdpyras-5.0.3/setup.py
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-06-07 20:41:28.642223 pdpyras-5.0.4/
+-rw-r--r--   0 demitri    (503) staff       (20)     1053 2023-05-01 18:31:04.000000 pdpyras-5.0.4/LICENSE
+-rw-r--r--   0 demitri    (503) staff       (20)      374 2023-06-07 20:41:28.642088 pdpyras-5.0.4/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)     4792 2023-05-17 22:04:20.000000 pdpyras-5.0.4/README.rst
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-06-07 20:41:28.641909 pdpyras-5.0.4/pdpyras.egg-info/
+-rw-r--r--   0 demitri    (503) staff       (20)      374 2023-06-07 20:41:28.000000 pdpyras-5.0.4/pdpyras.egg-info/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)      192 2023-06-07 20:41:28.000000 pdpyras-5.0.4/pdpyras.egg-info/SOURCES.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        1 2023-06-07 20:41:28.000000 pdpyras-5.0.4/pdpyras.egg-info/dependency_links.txt
+-rw-r--r--   0 demitri    (503) staff       (20)       29 2023-06-07 20:41:28.000000 pdpyras-5.0.4/pdpyras.egg-info/requires.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        8 2023-06-07 20:41:28.000000 pdpyras-5.0.4/pdpyras.egg-info/top_level.txt
+-rw-r--r--   0 demitri    (503) staff       (20)    87112 2023-06-07 20:38:03.000000 pdpyras-5.0.4/pdpyras.py
+-rw-r--r--   0 demitri    (503) staff       (20)       38 2023-06-07 20:41:28.642270 pdpyras-5.0.4/setup.cfg
+-rw-r--r--   0 demitri    (503) staff       (20)      657 2023-06-07 20:38:03.000000 pdpyras-5.0.4/setup.py
```

### Comparing `pdpyras-5.0.3/LICENSE` & `pdpyras-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdpyras-5.0.3/README.rst` & `pdpyras-5.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `pdpyras-5.0.3/pdpyras.py` & `pdpyras-5.0.4/pdpyras.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Libraries from PyPI
 import requests
 from deprecation import deprecated, DeprecatedWarning
 from urllib3.exceptions import HTTPError, PoolError
 from requests.exceptions import RequestException
 
-__version__ = '5.0.3'
+__version__ = '5.0.4'
 
 #######################
 ### CLIENT DEFAULTS ###
 #######################
 ITERATION_LIMIT = 1e4
 """
 The maximum position of a result in classic pagination.
@@ -37,15 +37,15 @@
 
 TIMEOUT = 60
 """
 The default timeout in seconds for any given HTTP request.
 
 Modifying this value will not affect any preexisting API session instances.
 Rather, it will only affect new instances. It is recommended to use
-:attr:`pdpyras.PDSession.timeout` to configure the timeout for a given session.
+:attr:`PDSession.timeout` to configure the timeout for a given session.
 """
 
 TEXT_LEN_LIMIT = 100
 """
 The longest permissible length of API content to include in error messages.
 """
 
@@ -417,36 +417,45 @@
     for i, node in enumerate(url_path.split('/')[1:]):
         j = i+1
         patterns = list(filter(
             lambda p: p.split('/')[j] == node or is_path_param(p.split('/')[j]),
             patterns
         ))
         # Don't break early if len(patterns) == 1, but require an exact match...
+
     if len(patterns) == 0:
         raise URLError(f"URL {url} does not match any canonical API path " \
             'supported by this client.')
     elif len(patterns) > 1:
+        # If there's multiple matches but one matches exactly, return that.
+        if url_path in patterns:
+            return url_path
+
+        # ...otherwise this is ambiguous.
         raise Exception(f"Ambiguous URL {url} matches more than one " \
             "canonical path pattern: "+', '.join(patterns)+'; this is likely ' \
             'a bug.')
     else:
         return patterns[0]
 
 def endpoint_matches(endpoint_pattern: str, method: str, path: str):
     """
     Returns true if a method and path match an endpoint pattern.
 
     This is the filtering logic  used for finding the appropriate entry in
     :attr:`ENTITY_WRAPPER_CONFIG` to use for a given method and API path.
 
-    :param e: The endpoint pattern in the form ``METHOD PATH`` where ``METHOD``
-        is the HTTP method in uppercase or ``*`` to match all methods, and
-        ``PATH`` is a canonical API path.
-    :param m: The HTTP method
-    :param p: The canonical API path (i.e. as returned by ``canonical_path``)
+    :param endpoint_pattern:
+        The endpoint pattern in the form ``METHOD PATH`` where ``METHOD`` is the
+        HTTP method in uppercase or ``*`` to match all methods, and ``PATH`` is
+        a canonical API path.
+    :param method:
+        The HTTP method.
+    :param path:
+        The canonical API path (i.e. as returned by :func:`canonical_path`)
     :rtype: boolean
     """
     return (
         endpoint_pattern.startswith(method.upper()) \
             or endpoint_pattern.startswith('*')
     ) and endpoint_pattern.endswith(f" {path}")
 
@@ -983,15 +992,16 @@
 
     sleep_timer = 1.5
     """
     Default initial cooldown time factor for rate limiting and network errors.
 
     Each time that the request makes a followup request, there will be a delay
     in seconds equal to this number times :attr:`sleep_timer_base` to the power
-    of how many attempts have already been made so far.
+    of how many attempts have already been made so far, unless
+    :attr:`stagger_cooldown` is nonzero.
     """
 
     sleep_timer_base = 2
     """
     After each retry, the time to sleep before reattempting the API connection
     and request will increase by a factor of this amount.
     """
```

### Comparing `pdpyras-5.0.3/setup.py` & `pdpyras-5.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '5.0.3'
+__version__ = '5.0.4'
 
 if __name__ == '__main__':
     setup(
         name='pdpyras',
         description="PagerDuty Python REST API Sessions",
         long_description="A basic REST API client for PagerDuty based on Requests' Session class",
         py_modules=['pdpyras'],
```

