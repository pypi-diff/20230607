# Comparing `tmp/cubicweb-api-0.7.2.tar.gz` & `tmp/cubicweb-api-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-api-0.7.2.tar", last modified: Fri Mar 10 15:25:22 2023, max compression
+gzip compressed data, was "cubicweb-api-0.7.3.tar", last modified: Wed Jun  7 14:16:23 2023, max compression
```

## Comparing `cubicweb-api-0.7.2.tar` & `cubicweb-api-0.7.3.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:25:22.783048 cubicweb-api-0.7.2/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3206 2023-03-10 15:25:22.783048 cubicweb-api-0.7.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2755 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:25:22.775048 cubicweb-api-0.7.2/cubicweb_api/
--rw-rw-rw-   0 root         (0) root         (0)     1738 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     3309 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/api_transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:25:22.779048 cubicweb-api-0.7.2/cubicweb_api/auth/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3800 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/auth/jwt_auth.py
--rw-rw-rw-   0 root         (0) root         (0)    11557 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/auth/jwt_policy.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/httperrors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:25:22.779048 cubicweb-api-0.7.2/cubicweb_api/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:25:22.779048 cubicweb-api-0.7.2/cubicweb_api/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1060 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/migration/postcreate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:25:22.779048 cubicweb-api-0.7.2/cubicweb_api/openapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/openapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5383 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/openapi/openapi.py
--rw-rw-rw-   0 root         (0) root         (0)     6978 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/openapi/openapi_template.yaml
--rw-rw-rw-   0 root         (0) root         (0)    10193 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/routes.py
--rw-rw-rw-   0 root         (0) root         (0)     1195 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/cubicweb_api/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:25:22.775048 cubicweb-api-0.7.2/cubicweb_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3206 2023-03-10 15:25:22.000000 cubicweb-api-0.7.2/cubicweb_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      856 2023-03-10 15:25:22.000000 cubicweb-api-0.7.2/cubicweb_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 15:25:22.000000 cubicweb-api-0.7.2/cubicweb_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-10 15:25:22.000000 cubicweb-api-0.7.2/cubicweb_api.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 15:25:22.000000 cubicweb-api-0.7.2/cubicweb_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       82 2023-03-10 15:25:22.000000 cubicweb-api-0.7.2/cubicweb_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-10 15:25:22.000000 cubicweb-api-0.7.2/cubicweb_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-10 15:25:22.783048 cubicweb-api-0.7.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2594 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:25:22.779048 cubicweb-api-0.7.2/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:25:22.783048 cubicweb-api-0.7.2/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        4 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/test/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-03-10 15:25:01.000000 cubicweb-api-0.7.2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:16:23.299236 cubicweb-api-0.7.3/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3206 2023-06-07 14:16:23.299236 cubicweb-api-0.7.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2755 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:16:23.295236 cubicweb-api-0.7.3/cubicweb_api/
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3309 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/api_transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:16:23.299236 cubicweb-api-0.7.3/cubicweb_api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3800 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/auth/jwt_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    11557 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/auth/jwt_policy.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1810 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/httperrors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:16:23.299236 cubicweb-api-0.7.3/cubicweb_api/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:16:23.299236 cubicweb-api-0.7.3/cubicweb_api/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/migration/postcreate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:16:23.299236 cubicweb-api-0.7.3/cubicweb_api/openapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/openapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5383 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/openapi/openapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6978 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/openapi/openapi_template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     6968 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/routes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/cubicweb_api/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:16:23.299236 cubicweb-api-0.7.3/cubicweb_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3206 2023-06-07 14:16:23.000000 cubicweb-api-0.7.3/cubicweb_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      927 2023-06-07 14:16:23.000000 cubicweb-api-0.7.3/cubicweb_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 14:16:23.000000 cubicweb-api-0.7.3/cubicweb_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-07 14:16:23.000000 cubicweb-api-0.7.3/cubicweb_api.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 14:16:23.000000 cubicweb-api-0.7.3/cubicweb_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-07 14:16:23.000000 cubicweb-api-0.7.3/cubicweb_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 14:16:23.000000 cubicweb-api-0.7.3/cubicweb_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 14:16:23.299236 cubicweb-api-0.7.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2594 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:16:23.299236 cubicweb-api-0.7.3/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:16:23.299236 cubicweb-api-0.7.3/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     6247 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/test/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2023-06-07 14:16:15.000000 cubicweb-api-0.7.3/tox.ini
```

### Comparing `cubicweb-api-0.7.2/PKG-INFO` & `cubicweb-api-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-api
-Version: 0.7.2
+Version: 0.7.3
 Summary: This cube is the new api which will be integrated in CubicWeb 4.
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/api
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-api-0.7.2/README.rst` & `cubicweb-api-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-api-0.7.2/cubicweb_api/__init__.py` & `cubicweb-api-0.7.3/cubicweb_api/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,30 +17,52 @@
 
 This cube is the new api which will be integrated in CubicWeb 4.
 """
 from datetime import datetime, date, time
 from typing import Union
 
 from pyramid.config import Configurator
+from pyramid.interfaces import IViewDeriverInfo
 from pyramid.renderers import JSON
 
+from cubicweb_api.exceptions import ApiException
 from cubicweb_api.util import get_api_path_prefix
 
 
 def datetime_adapter(obj: Union[datetime, date, time], request):
     """
     Converts datetime, date and time object to an ISO string for JSON serialization
     :param obj: the object to convert
     :param request: the current request
     :return:
     """
     return obj.isoformat()
 
 
+def api_exception_view_deriver(view, info: IViewDeriverInfo):
+    if info.options.get("use_api_exceptions"):
+
+        def wrapper_view(context, request):
+            try:
+                response = view(context, request)
+            except Exception as e:
+                raise ApiException(e) from e
+            return response
+
+        return wrapper_view
+    return view
+
+
 def includeme(config: Configurator):
     json_renderer = JSON()
     json_renderer.add_adapter(datetime, datetime_adapter)
     json_renderer.add_adapter(date, datetime_adapter)
     json_renderer.add_adapter(time, datetime_adapter)
 
+    api_exception_view_deriver.options = ("use_api_exceptions",)
+    config.add_view_deriver(api_exception_view_deriver)
+
+    config.include(".exceptions")
+    config.include(".predicates")
+
     config.add_renderer("cubicweb_api_json", json_renderer)
     config.include(".routes", route_prefix=get_api_path_prefix(config))
```

### Comparing `cubicweb-api-0.7.2/cubicweb_api/__pkginfo__.py` & `cubicweb-api-0.7.3/cubicweb_api/__pkginfo__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 """cubicweb-api application packaging information"""
 
 
 modname = "cubicweb_api"
 distname = "cubicweb-api"
 
-numversion = (0, 7, 2)
+numversion = (0, 7, 3)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "This cube is the new api which will be integrated in CubicWeb 4."
 web = "https://forge.extranet.logilab.fr/cubicweb/cubes/api"
```

### Comparing `cubicweb-api-0.7.2/cubicweb_api/api_transaction.py` & `cubicweb-api-0.7.3/cubicweb_api/api_transaction.py`

 * *Files identical despite different names*

### Comparing `cubicweb-api-0.7.2/cubicweb_api/auth/jwt_auth.py` & `cubicweb-api-0.7.3/cubicweb_api/auth/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `cubicweb-api-0.7.2/cubicweb_api/auth/jwt_policy.py` & `cubicweb-api-0.7.3/cubicweb_api/auth/jwt_policy.py`

 * *Files identical despite different names*

### Comparing `cubicweb-api-0.7.2/cubicweb_api/constants.py` & `cubicweb-api-0.7.3/cubicweb_api/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,7 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 # The default prefix to use when no configuration has been set.
 API_PATH_DEFAULT_PREFIX = "/api"
 # The prefix to add to all pyramid route names created by the API.
 API_ROUTE_NAME_PREFIX = "cube_api_v1_"
-# Default parameters to use for API routes.
-DEFAULT_ROUTE_PARAMS = {
-    "request_method": "POST",
-    "renderer": "cubicweb_api_json",
-    "require_csrf": False,
-    "openapi": True,
-}
```

### Comparing `cubicweb-api-0.7.2/cubicweb_api/httperrors.py` & `cubicweb-api-0.7.3/cubicweb_api/httperrors.py`

 * *Files identical despite different names*

### Comparing `cubicweb-api-0.7.2/cubicweb_api/migration/postcreate.py` & `cubicweb-api-0.7.3/cubicweb_api/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-api-0.7.2/cubicweb_api/openapi/openapi.py` & `cubicweb-api-0.7.3/cubicweb_api/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-api-0.7.2/cubicweb_api/openapi/openapi_template.yaml` & `cubicweb-api-0.7.3/cubicweb_api/openapi/openapi_template.yaml`

 * *Files identical despite different names*

### Comparing `cubicweb-api-0.7.2/cubicweb_api/routes.py` & `cubicweb-api-0.7.3/cubicweb_api/routes.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,44 +9,37 @@
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
-from contextlib import contextmanager
+import logging
 from enum import Enum
-from typing import Callable
 
-from cubicweb import AuthenticationError, QueryError, Unauthorized, Forbidden
-from cubicweb.pyramid.core import Connection
+from cubicweb import AuthenticationError
 from cubicweb.schema_exporters import JSONSchemaExporter
-from rql import RQLException
-from yams import ValidationError, UnknownType
 from pyramid.config import Configurator
 from pyramid.request import Request
 from pyramid.response import Response
-from pyramid.view import view_config
-from pyramid.httpexceptions import HTTPError
-import logging
+from pyramid.security import remember
+from pyramid.view import view_config, view_defaults
 
 from cubicweb_api.api_transaction import ApiTransactionsRepository
+from cubicweb_api.auth.jwt_auth import setup_jwt
 from cubicweb_api.constants import (
-    DEFAULT_ROUTE_PARAMS,
     API_ROUTE_NAME_PREFIX,
 )
-from cubicweb_api.httperrors import get_http_error, get_http_500_error
-from cubicweb_api.auth.jwt_auth import setup_jwt
 from cubicweb_api.openapi.openapi import setup_openapi
 from cubicweb_api.util import get_cw_repo, get_transactions_repository
 
 log = logging.getLogger(__name__)
 
 
-class ApiRoutes(str, Enum):
+class ApiRoutes(Enum):
     """
     All the available routes as listed in the openapi/openapi_template.yml file.
     """
 
     schema = "schema"
     rql = "rql"
     login = "login"
@@ -54,253 +47,152 @@
     transaction_begin = "transaction/begin"
     transaction_execute = "transaction/execute"
     transaction_commit = "transaction/commit"
     transaction_rollback = "transaction/rollback"
     help = "help"
 
 
-def is_user_allowed(request: Request):
-    """
-    Checks if the user making the request is authenticated or if anonymous access is enabled
-
-    :param request: The request initiated by the user
-    :return: True if the user can access the resource, false otherwise
-    """
-    return (
-        request.authenticated_userid is not None
-        or get_cw_repo(request).config["anonymous-user"] is not None
-    )
-
-
-def get_route_name(route_name: str) -> str:
+def get_route_name(route_name: ApiRoutes) -> str:
     """
     Generates a unique route name using the api prefix to prevent clashes with routes
     from other cubes.
 
     :param route_name: The route name base
     :return: The generated route name
     """
-    return f"{API_ROUTE_NAME_PREFIX}{route_name}"
-
+    return f"{API_ROUTE_NAME_PREFIX}{route_name.value}"
 
-@contextmanager
-def _catch_rql_errors(cnx: Connection):
-    """
-    Calls and returns the result of the given function.
-    If an error related to RQL occurs, this will raise an HTTP 400 error
-
-    :param func: The function to check for errors
-    :return: The function's result if no error occurred
-    :raise HTTPError: with 400 code if a RQL related exception is caught
-    """
-    try:
-        try:
-            yield
-        except ValidationError as e:
-            e.translate(cnx._)
-            raise
-    except (RQLException, QueryError, ValidationError, UnknownType) as e:
-        log.info(e.__class__.__name__, exc_info=True)
-        raise get_http_error(400, e.__class__.__name__, str(e))
 
+@view_defaults(
+    request_method="POST",
+    renderer="cubicweb_api_json",
+    require_csrf=False,
+    openapi=True,
+    use_api_exceptions=True,
+)
+class ApiViews:
+    def __init__(self, request: Request):
+        self.request = request
+
+    @view_config(
+        route_name=get_route_name(ApiRoutes.schema),
+        request_method="GET",
+        anonymous_or_connected=True,
+    )
+    def schema_route(self):
+        """
+        See the openapi/openapi_template.yml file for more information on this route.
+        """
+        repo = get_cw_repo(self.request)
+        exporter = JSONSchemaExporter()
+        exported_schema = exporter.export_as_dict(repo.schema)
+        return exported_schema
+
+    @view_config(route_name=get_route_name(ApiRoutes.rql), anonymous_or_connected=True)
+    def rql_route(self):
+        """
+        See the openapi/openapi_template.yml file for more information on this route.
+        """
+        request_params = self.request.openapi_validated.body
+        query: str = request_params["query"]
+        params: dict = request_params["params"]
+        rset = self.request.cw_cnx.execute(query, params).rows
+        self.request.cw_cnx.commit()
+        return rset
 
-def view_exception_handler(func: Callable):
-    """
-    Use it as a decorator for any pyramid view to catch authentication errors
-    and raise HTTP 401 or 403 errors.
-    It also catches any other leftover exceptions and raises an HTTP 500 error.
-
-    :param func: The pyramid view function
-    :raise HTTPError: with different error codes depending on the exception caught
-    """
-
-    def request_wrapper(request: Request):
-        try:
-            return func(request)
-        except HTTPError as e:
-            # The decorated function raised its own HTTP error, simply forward it.
-            return e
-        except (AuthenticationError, Unauthorized) as e:
-            # User was not authenticated, return 401 HTTP error
-            log.info(e.__class__.__name__, exc_info=True)
-            return get_http_error(401, e.__class__.__name__, str(e))
-        except Forbidden as e:
-            # User was authenticated but had insufficient privileges, return 403 HTTP error
-            log.info(e.__class__.__name__, exc_info=True)
-            return get_http_error(403, e.__class__.__name__, str(e))
-        except Exception:
-            # An exception was raised but not caught, this is a server error (HTTP 5OO)
-            log.info("ServerError", exc_info=True)
-            raise get_http_500_error()
-
-    return request_wrapper
-
-
-def authorized_users_only(func: Callable):
-    """
-    Use it as a decorator to raise an AuthenticationError if no user is detected
-    and anonymous access is disabled.
-
-    :param func: The pyramid view function
-    """
-
-    def request_wrapper(request: Request):
-        if is_user_allowed(request):
-            return func(request)
-        raise AuthenticationError
-
-    return request_wrapper
-
-
-@view_config(
-    route_name=get_route_name(ApiRoutes.schema),
-    **dict(DEFAULT_ROUTE_PARAMS, request_method="GET"),
-)
-@view_exception_handler
-@authorized_users_only
-def schema_route(request: Request):
-    """
-    See the openapi/openapi_template.yml file for more information on this route.
-    """
-    repo = get_cw_repo(request)
-    exporter = JSONSchemaExporter()
-    exported_schema = exporter.export_as_dict(repo.schema)
-    return exported_schema
-
-
-@view_config(
-    route_name=get_route_name(ApiRoutes.rql),
-    **DEFAULT_ROUTE_PARAMS,
-)
-@view_exception_handler
-@authorized_users_only
-def rql_route(request: Request):
-    """
-    See the openapi/openapi_template.yml file for more information on this route.
-    """
-    request_params = request.openapi_validated.body
-    query: str = request_params["query"]
-    params: dict = request_params["params"]
-    with _catch_rql_errors(request.cw_cnx):
-        return request.cw_cnx.execute(query, params).rows
-
+    @view_config(
+        route_name=get_route_name(ApiRoutes.login),
+    )
+    def login_route(self):
+        """
+        See the openapi/openapi_template.yml file for more information on this route.
+        """
+        request_params = self.request.openapi_validated.body
+        login: str = request_params["login"]
+        pwd: str = request_params["password"]
+
+        repo = get_cw_repo(self.request)
+        with repo.internal_cnx() as cnx:
+            try:
+                cwuser = repo.authenticate_user(cnx, login, password=pwd)
+            except AuthenticationError:
+                raise AuthenticationError("Invalid credentials")
 
-@view_config(
-    route_name=get_route_name(ApiRoutes.login),
-    **DEFAULT_ROUTE_PARAMS,
-)
-@view_exception_handler
-def login_route(request: Request):
-    """
-    See the openapi/openapi_template.yml file for more information on this route.
-    """
-    request_params = request.openapi_validated.body
-    login: str = request_params["login"]
-    pwd: str = request_params["password"]
-
-    repo = get_cw_repo(request)
-    with repo.internal_cnx() as cnx:
-        try:
-            cwuser = repo.authenticate_user(cnx, login, password=pwd)
-        except AuthenticationError:
-            raise get_http_error(
-                401, "AuthenticationFailure", "Login and/or password invalid."
-            )
-        else:
-            headers = request.authentication_policy.remember(
-                request,
+            headers = remember(
+                self.request,
                 cwuser.eid,
-                login=cwuser.login,
-                firstname=cwuser.firstname,
-                lastname=cwuser.surname,
             )
             return Response(headers=headers, status=204)
 
-
-@view_config(
-    route_name=get_route_name(ApiRoutes.current_user),
-    **dict(DEFAULT_ROUTE_PARAMS, request_method="GET"),
-)
-@view_exception_handler
-@authorized_users_only
-def current_user(request: Request):
-    """
-    See the openapi/openapi_template.yml file for more information on this route.
-    """
-    user = request.cw_cnx.user
-    return {"eid": user.eid, "login": user.login, "dcTitle": user.dc_title()}
-
-
-@view_config(
-    route_name=get_route_name(ApiRoutes.transaction_begin),
-    **DEFAULT_ROUTE_PARAMS,
-)
-@view_exception_handler
-@authorized_users_only
-def transaction_begin_route(request: Request):
-    """
-    See the openapi/openapi_template.yml file for more information on this route.
-    """
-    transactions = get_transactions_repository(request)
-    user = request.cw_cnx.user
-    return transactions.begin_transaction(user)
-
-
-@view_config(
-    route_name=get_route_name(ApiRoutes.transaction_execute),
-    **DEFAULT_ROUTE_PARAMS,
-)
-@view_exception_handler
-@authorized_users_only
-def transaction_execute_route(request: Request):
-    """
-    See the openapi/openapi_template.yml file for more information on this route.
-    """
-    transactions = get_transactions_repository(request)
-    request_params = request.openapi_validated.body
-    uuid: str = request_params["uuid"]
-    query: str = request_params["query"]
-    params: dict = request_params["params"]
-    with _catch_rql_errors(request.cw_cnx):
+    @view_config(
+        route_name=get_route_name(ApiRoutes.current_user),
+        request_method="GET",
+        anonymous_or_connected=True,
+    )
+    def current_user(self):
+        """
+        See the openapi/openapi_template.yml file for more information on this route.
+        """
+        user = self.request.cw_cnx.user
+        return {"eid": user.eid, "login": user.login, "dcTitle": user.dc_title()}
+
+    @view_config(
+        route_name=get_route_name(ApiRoutes.transaction_begin),
+        anonymous_or_connected=True,
+    )
+    def transaction_begin_route(self):
+        """
+        See the openapi/openapi_template.yml file for more information on this route.
+        """
+        transactions = get_transactions_repository(self.request)
+        user = self.request.cw_cnx.user
+        return transactions.begin_transaction(user)
+
+    @view_config(
+        route_name=get_route_name(ApiRoutes.transaction_execute),
+        anonymous_or_connected=True,
+    )
+    def transaction_execute_route(self):
+        """
+        See the openapi/openapi_template.yml file for more information on this route.
+        """
+        transactions = get_transactions_repository(self.request)
+        request_params = self.request.openapi_validated.body
+        uuid: str = request_params["uuid"]
+        query: str = request_params["query"]
+        params: dict = request_params["params"]
         return transactions[uuid].execute(query, params).rows
 
-
-@view_config(
-    route_name=get_route_name(ApiRoutes.transaction_commit),
-    **DEFAULT_ROUTE_PARAMS,
-)
-@view_exception_handler
-@authorized_users_only
-def transaction_commit_route(request: Request):
-    """
-    See the openapi/openapi_template.yml file for more information on this route.
-    """
-    transactions = get_transactions_repository(request)
-    request_params = request.openapi_validated.body
-    uuid: str = request_params["uuid"]
-    with _catch_rql_errors(request.cw_cnx):
+    @view_config(
+        route_name=get_route_name(ApiRoutes.transaction_commit),
+        anonymous_or_connected=True,
+    )
+    def transaction_commit_route(self):
+        """
+        See the openapi/openapi_template.yml file for more information on this route.
+        """
+        transactions = get_transactions_repository(self.request)
+        request_params = self.request.openapi_validated.body
+        uuid: str = request_params["uuid"]
         return transactions[uuid].commit()
 
-
-@view_config(
-    route_name=get_route_name(ApiRoutes.transaction_rollback),
-    **DEFAULT_ROUTE_PARAMS,
-)
-@view_exception_handler
-@authorized_users_only
-def transaction_rollback_route(request: Request):
-    """
-    See the openapi/openapi_template.yml file for more information on this route.
-    """
-    transactions = get_transactions_repository(request)
-    request_params = request.openapi_validated.body
-    uuid: str = request_params["uuid"]
-    rollback_result = transactions[uuid].rollback()
-    transactions.end_transaction(uuid)
-    return rollback_result
+    @view_config(
+        route_name=get_route_name(ApiRoutes.transaction_rollback),
+        anonymous_or_connected=True,
+    )
+    def transaction_rollback_route(self):
+        """
+        See the openapi/openapi_template.yml file for more information on this route.
+        """
+        transactions = get_transactions_repository(self.request)
+        request_params = self.request.openapi_validated.body
+        uuid: str = request_params["uuid"]
+        rollback_result = transactions[uuid].rollback()
+        transactions.end_transaction(uuid)
+        return rollback_result
 
 
 def includeme(config: Configurator):
     setup_jwt(config)
     repo = get_cw_repo(config)
     repo.api_transactions = ApiTransactionsRepository(repo)
     setup_openapi(config)
```

### Comparing `cubicweb-api-0.7.2/cubicweb_api/site_cubicweb.py` & `cubicweb-api-0.7.3/cubicweb_api/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-api-0.7.2/cubicweb_api/util.py` & `cubicweb-api-0.7.3/cubicweb_api/util.py`

 * *Files identical despite different names*

### Comparing `cubicweb-api-0.7.2/cubicweb_api.egg-info/PKG-INFO` & `cubicweb-api-0.7.3/cubicweb_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-api
-Version: 0.7.2
+Version: 0.7.3
 Summary: This cube is the new api which will be integrated in CubicWeb 4.
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/api
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-api-0.7.2/cubicweb_api.egg-info/SOURCES.txt` & `cubicweb-api-0.7.3/cubicweb_api.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 README.rst
 setup.py
 tox.ini
 cubicweb_api/__init__.py
 cubicweb_api/__pkginfo__.py
 cubicweb_api/api_transaction.py
 cubicweb_api/constants.py
+cubicweb_api/exceptions.py
 cubicweb_api/httperrors.py
+cubicweb_api/predicates.py
 cubicweb_api/routes.py
 cubicweb_api/site_cubicweb.py
 cubicweb_api/util.py
 cubicweb_api.egg-info/PKG-INFO
 cubicweb_api.egg-info/SOURCES.txt
 cubicweb_api.egg-info/dependency_links.txt
 cubicweb_api.egg-info/entry_points.txt
@@ -23,9 +25,10 @@
 cubicweb_api/i18n/en.po
 cubicweb_api/i18n/es.po
 cubicweb_api/i18n/fr.po
 cubicweb_api/migration/postcreate.py
 cubicweb_api/openapi/__init__.py
 cubicweb_api/openapi/openapi.py
 cubicweb_api/openapi/openapi_template.yaml
+test/__init__.py
 test/test_api.py
 test/data/bootstrap_cubes
```

### Comparing `cubicweb-api-0.7.2/setup.py` & `cubicweb-api-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-api-0.7.2/tox.ini` & `cubicweb-api-0.7.3/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tox]
 envlist = py3,flake8,check-manifest,black
 
 [testenv]
 deps =
   pytest
+  webtest
 commands =
   {envpython} -m pytest {posargs:test}
 
 [testenv:flake8]
 basepython = python3
 skip_install = true
 deps =
```

