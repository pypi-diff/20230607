# Comparing `tmp/halfapi-0.6.8.tar.gz` & `tmp/halfapi-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halfapi-0.6.8.tar", last modified: Mon Feb 28 09:18:49 2022, max compression
+gzip compressed data, was "halfapi-0.6.9.tar", last modified: Wed Mar  2 15:53:34 2022, max compression
```

## Comparing `halfapi-0.6.8.tar` & `halfapi-0.6.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-02-28 09:18:49.485108 halfapi-0.6.8/
--rw-r--r--   0 emixam    (1000) emixam    (1000)      107 2020-08-31 08:44:06.000000 halfapi-0.6.8/MANIFEST.in
--rw-r--r--   0 emixam    (1000) emixam    (1000)     2393 2022-02-28 09:18:49.485108 halfapi-0.6.8/PKG-INFO
--rw-r--r--   0 emixam    (1000) emixam    (1000)     1618 2021-12-13 12:51:37.000000 halfapi-0.6.8/README.md
-drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-02-28 09:18:49.481775 halfapi-0.6.8/halfapi/
--rw-r--r--   0 emixam    (1000) emixam    (1000)      154 2022-02-28 09:10:19.000000 halfapi-0.6.8/halfapi/__init__.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)       62 2021-01-14 09:55:26.000000 halfapi-0.6.8/halfapi/__main__.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)      223 2021-12-13 12:51:37.000000 halfapi-0.6.8/halfapi/app.py
-drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-02-28 09:18:49.481775 halfapi-0.6.8/halfapi/cli/
--rw-r--r--   0 emixam    (1000) emixam    (1000)        0 2021-01-14 09:55:26.000000 halfapi-0.6.8/halfapi/cli/__init__.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)      592 2021-12-13 12:51:37.000000 halfapi-0.6.8/halfapi/cli/cli.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)      455 2021-12-13 12:52:19.000000 halfapi-0.6.8/halfapi/cli/config.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     4495 2021-12-13 12:52:19.000000 halfapi-0.6.8/halfapi/cli/domain.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     1299 2021-12-13 12:52:19.000000 halfapi-0.6.8/halfapi/cli/init.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     1665 2021-12-13 12:52:19.000000 halfapi-0.6.8/halfapi/cli/routes.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     2544 2022-02-10 10:55:24.000000 halfapi-0.6.8/halfapi/cli/run.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     4076 2022-02-10 10:55:24.000000 halfapi-0.6.8/halfapi/conf.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)    10940 2021-12-13 12:52:19.000000 halfapi-0.6.8/halfapi/half_domain.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     3253 2021-12-15 11:04:57.000000 halfapi-0.6.8/halfapi/half_route.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     7710 2022-02-10 10:55:24.000000 halfapi-0.6.8/halfapi/halfapi.py
-drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-02-28 09:18:49.485108 halfapi-0.6.8/halfapi/lib/
--rw-r--r--   0 emixam    (1000) emixam    (1000)        0 2020-07-08 09:53:33.000000 halfapi-0.6.8/halfapi/lib/__init__.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     3062 2021-12-13 12:51:37.000000 halfapi-0.6.8/halfapi/lib/acl.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     1616 2021-12-13 12:52:19.000000 halfapi-0.6.8/halfapi/lib/constants.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)    11720 2022-02-10 09:30:06.000000 halfapi-0.6.8/halfapi/lib/domain.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     1996 2021-12-13 12:52:19.000000 halfapi-0.6.8/halfapi/lib/domain_middleware.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     4703 2021-12-13 12:52:19.000000 halfapi-0.6.8/halfapi/lib/jwt_middleware.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     2450 2021-06-07 14:45:10.000000 halfapi-0.6.8/halfapi/lib/query.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     4139 2022-02-10 15:32:28.000000 halfapi-0.6.8/halfapi/lib/responses.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)      225 2021-12-13 12:52:19.000000 halfapi-0.6.8/halfapi/lib/router.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     4349 2021-12-13 12:52:19.000000 halfapi-0.6.8/halfapi/lib/routes.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     4887 2021-12-13 12:52:19.000000 halfapi-0.6.8/halfapi/lib/schemas.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)      556 2021-12-13 12:51:37.000000 halfapi-0.6.8/halfapi/lib/timing.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     1607 2021-12-13 12:51:37.000000 halfapi-0.6.8/halfapi/lib/user.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     1193 2021-12-13 12:51:37.000000 halfapi-0.6.8/halfapi/logging.py
-drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-02-28 09:18:49.485108 halfapi-0.6.8/halfapi/testing/
--rw-r--r--   0 emixam    (1000) emixam    (1000)        0 2021-12-13 13:45:22.000000 halfapi-0.6.8/halfapi/testing/__init__.py
--rw-r--r--   0 emixam    (1000) emixam    (1000)     3219 2022-02-28 09:10:19.000000 halfapi-0.6.8/halfapi/testing/test_domain.py
-drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-02-28 09:18:49.481775 halfapi-0.6.8/halfapi.egg-info/
--rw-r--r--   0 emixam    (1000) emixam    (1000)     2393 2022-02-28 09:18:49.000000 halfapi-0.6.8/halfapi.egg-info/PKG-INFO
--rw-r--r--   0 emixam    (1000) emixam    (1000)      912 2022-02-28 09:18:49.000000 halfapi-0.6.8/halfapi.egg-info/SOURCES.txt
--rw-r--r--   0 emixam    (1000) emixam    (1000)        1 2022-02-28 09:18:49.000000 halfapi-0.6.8/halfapi.egg-info/dependency_links.txt
--rw-r--r--   0 emixam    (1000) emixam    (1000)       48 2022-02-28 09:18:49.000000 halfapi-0.6.8/halfapi.egg-info/entry_points.txt
--rw-r--r--   0 emixam    (1000) emixam    (1000)      210 2022-02-28 09:18:49.000000 halfapi-0.6.8/halfapi.egg-info/requires.txt
--rw-r--r--   0 emixam    (1000) emixam    (1000)       48 2022-02-28 09:18:49.000000 halfapi-0.6.8/halfapi.egg-info/top_level.txt
--rw-r--r--   0 emixam    (1000) emixam    (1000)      230 2020-08-26 11:20:12.000000 halfapi-0.6.8/pyproject.toml
--rw-r--r--   0 emixam    (1000) emixam    (1000)       74 2022-02-28 09:18:49.485108 halfapi-0.6.8/setup.cfg
--rwxr-xr-x   0 emixam    (1000) emixam    (1000)     2243 2021-12-13 12:52:19.000000 halfapi-0.6.8/setup.py
+drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-03-02 15:53:34.201159 halfapi-0.6.9/
+-rw-r--r--   0 emixam    (1000) emixam    (1000)      107 2020-08-31 08:44:06.000000 halfapi-0.6.9/MANIFEST.in
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     2393 2022-03-02 15:53:34.201159 halfapi-0.6.9/PKG-INFO
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     1618 2021-12-13 12:51:37.000000 halfapi-0.6.9/README.md
+drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-03-02 15:53:34.201159 halfapi-0.6.9/halfapi/
+-rw-r--r--   0 emixam    (1000) emixam    (1000)      154 2022-03-02 15:47:47.000000 halfapi-0.6.9/halfapi/__init__.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)       62 2021-01-14 09:55:26.000000 halfapi-0.6.9/halfapi/__main__.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)      223 2021-12-13 12:51:37.000000 halfapi-0.6.9/halfapi/app.py
+drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-03-02 15:53:34.201159 halfapi-0.6.9/halfapi/cli/
+-rw-r--r--   0 emixam    (1000) emixam    (1000)        0 2021-01-14 09:55:26.000000 halfapi-0.6.9/halfapi/cli/__init__.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)      592 2021-12-13 12:51:37.000000 halfapi-0.6.9/halfapi/cli/cli.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)      455 2021-12-13 12:52:19.000000 halfapi-0.6.9/halfapi/cli/config.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     4495 2021-12-13 12:52:19.000000 halfapi-0.6.9/halfapi/cli/domain.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     1299 2021-12-13 12:52:19.000000 halfapi-0.6.9/halfapi/cli/init.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     1665 2021-12-13 12:52:19.000000 halfapi-0.6.9/halfapi/cli/routes.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     2544 2022-02-10 10:55:24.000000 halfapi-0.6.9/halfapi/cli/run.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     4076 2022-02-10 10:55:24.000000 halfapi-0.6.9/halfapi/conf.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)    10940 2022-03-02 15:45:45.000000 halfapi-0.6.9/halfapi/half_domain.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     3253 2021-12-15 11:04:57.000000 halfapi-0.6.9/halfapi/half_route.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     7710 2022-02-10 10:55:24.000000 halfapi-0.6.9/halfapi/halfapi.py
+drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-03-02 15:53:34.201159 halfapi-0.6.9/halfapi/lib/
+-rw-r--r--   0 emixam    (1000) emixam    (1000)        0 2020-07-08 09:53:33.000000 halfapi-0.6.9/halfapi/lib/__init__.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     2970 2022-03-02 15:47:47.000000 halfapi-0.6.9/halfapi/lib/acl.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     1616 2021-12-13 12:52:19.000000 halfapi-0.6.9/halfapi/lib/constants.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)    11720 2022-02-10 09:30:06.000000 halfapi-0.6.9/halfapi/lib/domain.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     1996 2021-12-13 12:52:19.000000 halfapi-0.6.9/halfapi/lib/domain_middleware.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     4703 2021-12-13 12:52:19.000000 halfapi-0.6.9/halfapi/lib/jwt_middleware.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     2450 2021-06-07 14:45:10.000000 halfapi-0.6.9/halfapi/lib/query.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     4139 2022-02-10 15:32:28.000000 halfapi-0.6.9/halfapi/lib/responses.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)      225 2021-12-13 12:52:19.000000 halfapi-0.6.9/halfapi/lib/router.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     4300 2022-03-02 15:47:47.000000 halfapi-0.6.9/halfapi/lib/routes.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     4887 2021-12-13 12:52:19.000000 halfapi-0.6.9/halfapi/lib/schemas.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)      556 2021-12-13 12:51:37.000000 halfapi-0.6.9/halfapi/lib/timing.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     1607 2021-12-13 12:51:37.000000 halfapi-0.6.9/halfapi/lib/user.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     1193 2021-12-13 12:51:37.000000 halfapi-0.6.9/halfapi/logging.py
+drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-03-02 15:53:34.201159 halfapi-0.6.9/halfapi/testing/
+-rw-r--r--   0 emixam    (1000) emixam    (1000)        0 2021-12-13 13:45:22.000000 halfapi-0.6.9/halfapi/testing/__init__.py
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     3219 2022-02-28 09:10:19.000000 halfapi-0.6.9/halfapi/testing/test_domain.py
+drwxr-xr-x   0 emixam    (1000) emixam    (1000)        0 2022-03-02 15:53:34.201159 halfapi-0.6.9/halfapi.egg-info/
+-rw-r--r--   0 emixam    (1000) emixam    (1000)     2393 2022-03-02 15:53:33.000000 halfapi-0.6.9/halfapi.egg-info/PKG-INFO
+-rw-r--r--   0 emixam    (1000) emixam    (1000)      912 2022-03-02 15:53:34.000000 halfapi-0.6.9/halfapi.egg-info/SOURCES.txt
+-rw-r--r--   0 emixam    (1000) emixam    (1000)        1 2022-03-02 15:53:34.000000 halfapi-0.6.9/halfapi.egg-info/dependency_links.txt
+-rw-r--r--   0 emixam    (1000) emixam    (1000)       48 2022-03-02 15:53:34.000000 halfapi-0.6.9/halfapi.egg-info/entry_points.txt
+-rw-r--r--   0 emixam    (1000) emixam    (1000)      210 2022-03-02 15:53:34.000000 halfapi-0.6.9/halfapi.egg-info/requires.txt
+-rw-r--r--   0 emixam    (1000) emixam    (1000)       48 2022-03-02 15:53:34.000000 halfapi-0.6.9/halfapi.egg-info/top_level.txt
+-rw-r--r--   0 emixam    (1000) emixam    (1000)      230 2020-08-26 11:20:12.000000 halfapi-0.6.9/pyproject.toml
+-rw-r--r--   0 emixam    (1000) emixam    (1000)       74 2022-03-02 15:53:34.204493 halfapi-0.6.9/setup.cfg
+-rwxr-xr-x   0 emixam    (1000) emixam    (1000)     2243 2021-12-13 12:52:19.000000 halfapi-0.6.9/setup.py
```

### Comparing `halfapi-0.6.8/PKG-INFO` & `halfapi-0.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halfapi
-Version: 0.6.8
+Version: 0.6.9
 Summary: Core to write deep APIs using a module's tree
 Home-page: https://github.com/halfAPI/halfapi
 Author: Maxime ALVES
 Author-email: maxime@freepoteries.fr
 License: GPLv3
 Project-URL: Source, https://github.com/halfAPI/halfapi
 Keywords: web-api development boilerplate
```

### Comparing `halfapi-0.6.8/README.md` & `halfapi-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/cli/cli.py` & `halfapi-0.6.9/halfapi/cli/cli.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/cli/domain.py` & `halfapi-0.6.9/halfapi/cli/domain.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/cli/init.py` & `halfapi-0.6.9/halfapi/cli/init.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/cli/routes.py` & `halfapi-0.6.9/halfapi/cli/routes.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/cli/run.py` & `halfapi-0.6.9/halfapi/cli/run.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/conf.py` & `halfapi-0.6.9/halfapi/conf.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/half_domain.py` & `halfapi-0.6.9/halfapi/half_domain.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/half_route.py` & `halfapi-0.6.9/halfapi/half_route.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/halfapi.py` & `halfapi-0.6.9/halfapi/halfapi.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/lib/acl.py` & `halfapi-0.6.9/halfapi/lib/acl.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,16 +90,14 @@
         else:
             """ Unsafe mode, without specified arguments
             """
             data = data_
 
         kwargs['data'] = data
 
-        logger.debug('args_check %s:%s %s %s', fct.__module__, fct.__name__, args, kwargs)
-
         return await fct(req, *args, **kwargs)
 
     return caller
 
 # ACLS list for doc and priorities
 # Write your own constant in your domain or import this one
 ACLS = (
```

### Comparing `halfapi-0.6.8/halfapi/lib/constants.py` & `halfapi-0.6.9/halfapi/lib/constants.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/lib/domain.py` & `halfapi-0.6.9/halfapi/lib/domain.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/lib/domain_middleware.py` & `halfapi-0.6.9/halfapi/lib/domain_middleware.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/lib/jwt_middleware.py` & `halfapi-0.6.9/halfapi/lib/jwt_middleware.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/lib/query.py` & `halfapi-0.6.9/halfapi/lib/query.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/lib/responses.py` & `halfapi-0.6.9/halfapi/lib/responses.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/lib/routes.py` & `halfapi-0.6.9/halfapi/lib/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         data (Any):
             The data to return
 
     Returns:
         async function
     """
     async def wrapped(request, *args, **kwargs):
-        logger.debug('JSONRoute data: %s', data)
         return ORJSONResponse(data)
 
     return wrapped
 
 
 def gen_domain_routes(m_domain: ModuleType):
     """
```

### Comparing `halfapi-0.6.8/halfapi/lib/schemas.py` & `halfapi-0.6.9/halfapi/lib/schemas.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/lib/timing.py` & `halfapi-0.6.9/halfapi/lib/timing.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/lib/user.py` & `halfapi-0.6.9/halfapi/lib/user.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/logging.py` & `halfapi-0.6.9/halfapi/logging.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi/testing/test_domain.py` & `halfapi-0.6.9/halfapi/testing/test_domain.py`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/halfapi.egg-info/PKG-INFO` & `halfapi-0.6.9/halfapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halfapi
-Version: 0.6.8
+Version: 0.6.9
 Summary: Core to write deep APIs using a module's tree
 Home-page: https://github.com/halfAPI/halfapi
 Author: Maxime ALVES
 Author-email: maxime@freepoteries.fr
 License: GPLv3
 Project-URL: Source, https://github.com/halfAPI/halfapi
 Keywords: web-api development boilerplate
```

### Comparing `halfapi-0.6.8/halfapi.egg-info/SOURCES.txt` & `halfapi-0.6.9/halfapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halfapi-0.6.8/setup.py` & `halfapi-0.6.9/setup.py`

 * *Files identical despite different names*

