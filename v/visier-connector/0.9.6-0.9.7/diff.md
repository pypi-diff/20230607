# Comparing `tmp/visier-connector-0.9.6.tar.gz` & `tmp/visier-connector-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visier-connector-0.9.6.tar", last modified: Wed May 31 01:12:22 2023, max compression
+gzip compressed data, was "visier-connector-0.9.7.tar", last modified: Tue Jun  6 23:32:22 2023, max compression
```

## Comparing `visier-connector-0.9.6.tar` & `visier-connector-0.9.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:12:22.963419 visier-connector-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 01:12:11.000000 visier-connector-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24749 2023-05-31 01:12:22.963419 visier-connector-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-31 01:12:11.000000 visier-connector-0.9.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-31 01:12:11.000000 visier-connector-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 01:12:22.963419 visier-connector-0.9.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:12:22.959419 visier-connector-0.9.6/visier/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:12:22.963419 visier-connector-0.9.6/visier/api/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/api/direct_intake.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/api/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:12:22.963419 visier-connector-0.9.6/visier/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/connector/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/connector/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-31 01:12:11.000000 visier-connector-0.9.6/visier/connector/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:12:22.963419 visier-connector-0.9.6/visier_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24749 2023-05-31 01:12:22.000000 visier-connector-0.9.6/visier_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-31 01:12:22.000000 visier-connector-0.9.6/visier_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:12:22.000000 visier-connector-0.9.6/visier_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 01:12:22.000000 visier-connector-0.9.6/visier_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 01:12:22.000000 visier-connector-0.9.6/visier_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:32:22.780756 visier-connector-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 23:32:11.000000 visier-connector-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26297 2023-06-06 23:32:22.780756 visier-connector-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-06-06 23:32:11.000000 visier-connector-0.9.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 23:32:11.000000 visier-connector-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 23:32:22.780756 visier-connector-0.9.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:32:22.776756 visier-connector-0.9.7/visier/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:32:22.780756 visier-connector-0.9.7/visier/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/api/direct_intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/api/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:32:22.780756 visier-connector-0.9.7/visier/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/connector/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/connector/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/connector/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:32:22.780756 visier-connector-0.9.7/visier_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26297 2023-06-06 23:32:22.000000 visier-connector-0.9.7/visier_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-06 23:32:22.000000 visier-connector-0.9.7/visier_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:32:22.000000 visier-connector-0.9.7/visier_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-06 23:32:22.000000 visier-connector-0.9.7/visier_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 23:32:22.000000 visier-connector-0.9.7/visier_connector.egg-info/top_level.txt
```

### Comparing `visier-connector-0.9.6/LICENSE` & `visier-connector-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.6/PKG-INFO` & `visier-connector-0.9.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.6
+Version: 0.9.7
 Summary: Visier People Data connector
 Author-email: Visier Research & Development <info@visier.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,14 +219,44 @@
 ## Prerequisites
 The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
 * The URL domain name prefix. For example: `https://{vanity-name}.api.visier.io`.
 * An API key issued by Visier.
 * A username identifying a user within your organization's Visier tenant who has been granted API access capabilities.
 * That user's password
 
+## Authentication Environment
+In order to avoid passing authentication credentials in via command line arguments, Visier recommends that basic authentication credentials such as username and password are provided via environment variables. 
+
+Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the various authentication parameters
+* `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant
+* `VISIER_USERNAME`: The user name with sufficient API capabilities
+* `VISIER_PASSWORD`: The password of that user
+* `VISIER_APIKEY`: The API key granted by Visier
+* `VISIER_VANITY`: The readable name of the customer organization
+* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations.
+
+To illustrate this process, consider the following example approach suitable in a non-production environment:
+
+On Linux-like systems, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
+```sh
+echo -n "Enter the password for the Visier API User: "
+read -s vpwd
+export VISIER_VANITY=example
+export VISIER_HOST=https://$VISIER_VANITY.api.visier.io
+export VISIER_USERNAME=apiuser@example.com
+export VISIER_PASSWORD=$vpwd
+export VISIER_TARGET_TENANT_ID=tenant-code
+export VISIER_APIKEY=the-api-key-issued-by-visier
+```
+
+Source this environment in and provide the password when prompted:
+```sh
+$ source .env
+```
+
 ## Connector Separation
 As of version `0.9.5`, the Python connector has separated the API calls from the `VisierSession` object. As a result of this change, the query execution methods on the `VisierSession` have been deprecated and will be subject to removal in a future release.
 
 The new way of invoking Visier public APIs through the Visier Python connector requires instantiating the appropriate API client and calling the methods defined on the client object. The following example, invokes the `analytic-objects` Model API to obtain the metadata for two analytic objects:
 ```python
     with VisierSession(auth) as session:
         model_client = ModelApiClient(session)
```

### Comparing `visier-connector-0.9.6/README.md` & `visier-connector-0.9.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,44 @@
 ## Prerequisites
 The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
 * The URL domain name prefix. For example: `https://{vanity-name}.api.visier.io`.
 * An API key issued by Visier.
 * A username identifying a user within your organization's Visier tenant who has been granted API access capabilities.
 * That user's password
 
+## Authentication Environment
+In order to avoid passing authentication credentials in via command line arguments, Visier recommends that basic authentication credentials such as username and password are provided via environment variables. 
+
+Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the various authentication parameters
+* `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant
+* `VISIER_USERNAME`: The user name with sufficient API capabilities
+* `VISIER_PASSWORD`: The password of that user
+* `VISIER_APIKEY`: The API key granted by Visier
+* `VISIER_VANITY`: The readable name of the customer organization
+* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations.
+
+To illustrate this process, consider the following example approach suitable in a non-production environment:
+
+On Linux-like systems, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
+```sh
+echo -n "Enter the password for the Visier API User: "
+read -s vpwd
+export VISIER_VANITY=example
+export VISIER_HOST=https://$VISIER_VANITY.api.visier.io
+export VISIER_USERNAME=apiuser@example.com
+export VISIER_PASSWORD=$vpwd
+export VISIER_TARGET_TENANT_ID=tenant-code
+export VISIER_APIKEY=the-api-key-issued-by-visier
+```
+
+Source this environment in and provide the password when prompted:
+```sh
+$ source .env
+```
+
 ## Connector Separation
 As of version `0.9.5`, the Python connector has separated the API calls from the `VisierSession` object. As a result of this change, the query execution methods on the `VisierSession` have been deprecated and will be subject to removal in a future release.
 
 The new way of invoking Visier public APIs through the Visier Python connector requires instantiating the appropriate API client and calling the methods defined on the client object. The following example, invokes the `analytic-objects` Model API to obtain the metadata for two analytic objects:
 ```python
     with VisierSession(auth) as session:
         model_client = ModelApiClient(session)
```

### Comparing `visier-connector-0.9.6/pyproject.toml` & `visier-connector-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.6/visier/__init__.py` & `visier-connector-0.9.7/visier/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Public Python Connector
 """
 
-__version__ = "0.9.6"
+__version__ = "0.9.7"
```

### Comparing `visier-connector-0.9.6/visier/api/__init__.py` & `visier-connector-0.9.7/visier/api/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.6/visier/api/base.py` & `visier-connector-0.9.7/visier/api/base.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.6/visier/api/direct_intake.py` & `visier-connector-0.9.7/visier/api/direct_intake.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,70 +44,70 @@
     def set_configuration(self, configuration: Configuration) -> Response:
         """Set the configuration for the the direct intake environment.
         
         Arguments:
         - configuration: The direct intake environment configuration."""
         def call_impl(context: SessionContext) -> Response:
             url = context.mk_url(f"{BASE_PATH}/configs")
-            return context.session().put(url, json=configuration.config)
+            return context.session().put(url, json=configuration.config, headers=context.mk_headers())
         return self.run(call_impl)
 
     def get_object_schema(self, object_id: str) -> Response:
         """Get the staging schema for the given object. This is the schema that the data file must conform to.
         
         Arguments:
         - object_id: The id of the object to get the schema for"""
         def call_impl(context: SessionContext) -> Response:
             url = context.mk_url(f"{BASE_PATH}/schemas/{object_id}")
-            return context.session().get(url)
+            return context.session().get(url, headers=context.mk_headers())
         return self.run(call_impl)
 
     def start_transaction(self) -> Response:
         """Start an upload transaction"""
         def call_impl(context: SessionContext) -> Response:
             url = context.mk_url(f"{BASE_PATH}/transactions")
-            return context.session().post(url)
+            return context.session().post(url, headers=context.mk_headers())
         return self.run(call_impl)
 
     def upload_file(self, transaction_id: str, object_name: str, payload_file_path: str) -> Response:
         """Upload a data file to the given object.
         
         Arguments:
         - transaction_id: The transaction id returned by start_transaction
         - obejct_name: The name of the object to upload to
         - payload_file: The path to the file to upload"""
         def call_impl(context: SessionContext) -> Response:
             url = context.mk_url(f"{BASE_PATH}/transactions/{transaction_id}/{object_name}")
             with open(payload_file_path, "rb") as payload_file:
                 files = {"file": payload_file}
-                return context.session().put(url, files=files)
+                return context.session().put(url, files=files, headers=context.mk_headers())
         return self.run(call_impl)
 
     def rollback_transaction(self, transaction_id: str) -> Response:
         """Roll-back a pending transaction and discard all uploaded data.
         
         Arguments:
         - transaction_id: The transaction id returned by start_transaction"""
         def call_impl(context: SessionContext) -> Response:
             url = context.mk_url(f"{BASE_PATH}/transactions/{transaction_id}")
-            return context.session().delete(url)
+            return context.session().delete(url, headers=context.mk_headers())
         return self.run(call_impl)
 
     def commit_transaction(self, transaction_id: str) -> Response:
         """Commit the transaction and make the uploaded data available for use.
         
         Arguments:
         - transaction_id: The transaction id returned by start_transaction"""
         def call_impl(context: SessionContext) -> Response:
             url = context.mk_url(f"{BASE_PATH}/transactions/{transaction_id}")
-            return context.session().post(url)
+            return context.session().post(url, headers=context.mk_headers())
         return self.run(call_impl)
 
     def get_transaction_status(self, transaction_id: str) -> Response:
         """Get the status of the committed transaction.
 
         Arguments:
         - transaction_id: The transaction id returned by start_transaction"""
         def call_impl(context: SessionContext) -> Response:
             url = context.mk_url(f"{BASE_PATH}/transactions/{transaction_id}")
-            return context.session().get(url)
+            return context.session().get(url, headers=context.mk_headers())
         return self.run(call_impl)
```

### Comparing `visier-connector-0.9.6/visier/api/model.py` & `visier-connector-0.9.7/visier/api/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,63 +25,67 @@
 class ModelApiClient(ApiClientBase):
     """API client for the Visier Model API."""
     def get_analytic_objects(self, ids: List[str] = None) -> Response:
         """Get analytic objects by id"""
         def call_impl(context: SessionContext) -> Response:
             args = _ids_as_url_args(ids)
             url = context.mk_url(f"/v1/data/model/analytic-objects{args}")
-            return context.session().get(url)
+            return _get_with_header(context, url)
         return self.run(call_impl)
 
     def get_dimensions(self, object_id: str, ids: List[str] = None) -> Response:
         """Get dimensions by id"""
         def call_impl(context: SessionContext) -> Response:
             args = _ids_as_url_args(ids)
             url = context.mk_url(f"/v1/data/model/analytic-objects/{object_id}/dimensions{args}")
-            return context.session().get(url)
+            return _get_with_header(context, url)
         return self.run(call_impl)
 
     def get_selection_concepts(self, object_id: str, ids: List[str] = None) -> Response:
         """Get concepts by id"""
         def call_impl(context: SessionContext) -> Response:
             args = _ids_as_url_args(ids)
             url = context.mk_url(f"/v1/data/model/analytic-objects/{object_id}/selection-concepts{args}")
-            return context.session().get(url)
+            return _get_with_header(context, url)
         return self.run(call_impl)
 
     def get_properties(self, object_id: str, ids: List[str] = None) -> Response:
         """Get properties by id"""
         def call_impl(context: SessionContext) -> Response:
             args = _ids_as_url_args(ids)
             url = context.mk_url(f"/v1/data/model/analytic-objects/{object_id}/properties{args}")
-            return context.session().get(url)
+            return _get_with_header(context, url)
         return self.run(call_impl)
 
     def get_metrics(self, ids: List[str] = None) -> Response:
         """Get metrics by id"""
         def call_impl(context: SessionContext) -> Response:
             args = _ids_as_url_args(ids)
             url = context.mk_url(f"/v1/data/model/metrics{args}")
-            return context.session().get(url)
+            return _get_with_header(context, url)
         return self.run(call_impl)
 
     def get_metric_dimensions(self, metric_id: str) -> Response:
         """Get dimensions by id"""
         def call_impl(context: SessionContext) -> Response:
             url = context.mk_url(f"/v1/data/model/metrics/{metric_id}/dimensions")
-            return context.session().get(url)
+            return _get_with_header(context, url)
         return self.run(call_impl)
 
     def get_metric_selection_concepts(self, metric_id: str) -> Response:
         """Get concepts by id"""
         def call_impl(context: SessionContext) -> Response:
             url = context.mk_url(f"/v1/data/model/metrics/{metric_id}/selection-concepts")
-            return context.session().get(url)
+            return _get_with_header(context, url)
         return self.run(call_impl)
 
 
+def _get_with_header(context: SessionContext, url: str) -> Response:
+    """Invokes the Model GET request on the provided url with the provided headers."""
+    return context.session().get(url, headers=context.mk_headers())
+
 def _ids_as_url_args(ids: List[str]) -> str:
     """Constructs a URL argument string from a list of ids."""
     if (ids and len(ids) > 0):
         args = "&id=".join([urlparse.quote_plus(id) for id in ids])
         return f"?id={args}"
     return ""
```

### Comparing `visier-connector-0.9.6/visier/api/query.py` & `visier-connector-0.9.7/visier/api/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,9 +38,11 @@
             body["options"] = options
         return self._execute_query_api("/v1/data/query/sql", body)
 
     def _execute_query_api(self, path: str, body: object):
         """Helper method for executing a query API with flattened result."""
         result = self.run(lambda s: s.session().post(url=s.mk_url(path),
                                                          json=body,
-                                                         headers=self.HEADER))
-        return ResultTable(result.iter_lines())
+                                                         headers=s.mk_headers(self.HEADER)))
+        if result is not None:
+            return ResultTable(result.iter_lines())
+        return None
```

### Comparing `visier-connector-0.9.6/visier/connector/__init__.py` & `visier-connector-0.9.7/visier/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.6/visier/connector/authentication.py` & `visier-connector-0.9.7/visier/connector/authentication.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,25 +25,28 @@
     
     Keyword arguments:
     username -- The name of the user to authenticate as
     password -- The password of the user
     api_key -- The tenant's API Key
     host -- The host and protocol portion of the url. E.g. https://customer-name.visierinc.io
     vanity -- Optional vanity name for the customer
+    target_tenant_id -- Optional tenant id to target in a partner authentication setting
     """
 
     def __init__(
             self,
             username: str,
             password: str,
             api_key: str,
             host: str,
-            vanity: str = None) -> None:
+            vanity: str = None,
+            target_tenant_id: str = None) -> None:
         if not username or not password or not api_key or not host:
             raise ValueError("""ERROR: Missing required credentials.
             Please provide username, password, api_key, and host.""")
 
         self.vanity = vanity
         self.host = host
         self.api_key = api_key
         self.username = username
         self.password = password
+        self.target_tenant_id = target_tenant_id
```

### Comparing `visier-connector-0.9.6/visier/connector/sessions.py` & `visier-connector-0.9.7/visier/connector/sessions.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 from typing import Callable
 import requests
 from requests import Session, Response
 from deprecated import deprecated
 from .table import ResultTable
 from .authentication import Authentication
+from .constants import TARGET_TENANT_ID
+
 
 class QueryExecutionError(Exception):
     """Description of error from executing a query"""
     def __init__(self, status_code, message) -> None:
         self.args = (f"""The query execution failed with the following
         HTTP status code: {status_code}
         The server returned the following description of the error:
@@ -36,30 +38,41 @@
         """Returns the HTTP status code"""
         return self._status_code
 
     def message(self) -> str:
         """Returns the error message"""
         return self._message
 
+
 class SessionContext:
     """
     Context object passed to the user-defined function in the execute() method.
     """
-    def __init__(self, session: Session, host: str) -> None:
+    def __init__(self, session: Session, host: str, target_tenant_id: str = None) -> None:
         self._session = session
         self._host = host
+        self._target_tenant_id = target_tenant_id
 
     def session(self) -> Session:
         """Returns the current session object"""
         return self._session
 
     def mk_url(self, path: str) -> str:
         """Returns a URL for the given path"""
         return self._host + path
 
+    def mk_headers(self, headers: dict = None) -> dict:
+        """Returns the headers for the current request"""
+        if headers is None:
+            headers = {}
+        if self._target_tenant_id is not None:
+            headers[TARGET_TENANT_ID] = self._target_tenant_id
+        return headers
+
+
 class VisierSession:
     """Visier Session object through which SQL-like queries are executed.
     
     Keyword arguments:
     auth -- Authentication configuration
     """
     HEADER = {"Accept": "application/jsonlines, application/json"}
@@ -92,15 +105,15 @@
         Keyword arguments:
         call_function -- Function that takes a SessionContext object as input and
                          returns a Response object.
         """
         num_attempts_left = 2
         is_ok = False
         while not is_ok and num_attempts_left > 0:
-            context = SessionContext(self._session, self._auth.host)
+            context = SessionContext(self._session, self._auth.host, self._auth.target_tenant_id)
             result = call_function(context)
             num_attempts_left -= 1
             is_ok = result.ok
             if not is_ok:
                 if result.status_code == 401 and num_attempts_left > 0:
                     self._connect()
                 else:
@@ -111,15 +124,17 @@
         self._connect()
         return self
 
     def __exit__(self, ex_type, ex_value, trace_back):
         self.close()
 
     def _execute_query_api(self, path: str, body: object):
-        """Helper method for executing a query API with flattened result."""
+        """Helper method for executing a query API with flattened result.
+        This is a legacy and deprecated method that doesn't support partner administrative
+        principals to execute queries in the customer tenants."""
         result = self.execute(lambda s: s.session().post(url=s.mk_url(path),
                                                          json=body,
                                                          headers=self.HEADER))
         return ResultTable(result.iter_lines())
 
     def _connect(self):
         url = self._auth.host + "/v1/admin/visierSecureToken"
```

### Comparing `visier-connector-0.9.6/visier/connector/table.py` & `visier-connector-0.9.7/visier/connector/table.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.6/visier_connector.egg-info/PKG-INFO` & `visier-connector-0.9.7/visier_connector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.6
+Version: 0.9.7
 Summary: Visier People Data connector
 Author-email: Visier Research & Development <info@visier.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,14 +219,44 @@
 ## Prerequisites
 The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
 * The URL domain name prefix. For example: `https://{vanity-name}.api.visier.io`.
 * An API key issued by Visier.
 * A username identifying a user within your organization's Visier tenant who has been granted API access capabilities.
 * That user's password
 
+## Authentication Environment
+In order to avoid passing authentication credentials in via command line arguments, Visier recommends that basic authentication credentials such as username and password are provided via environment variables. 
+
+Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the various authentication parameters
+* `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant
+* `VISIER_USERNAME`: The user name with sufficient API capabilities
+* `VISIER_PASSWORD`: The password of that user
+* `VISIER_APIKEY`: The API key granted by Visier
+* `VISIER_VANITY`: The readable name of the customer organization
+* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations.
+
+To illustrate this process, consider the following example approach suitable in a non-production environment:
+
+On Linux-like systems, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
+```sh
+echo -n "Enter the password for the Visier API User: "
+read -s vpwd
+export VISIER_VANITY=example
+export VISIER_HOST=https://$VISIER_VANITY.api.visier.io
+export VISIER_USERNAME=apiuser@example.com
+export VISIER_PASSWORD=$vpwd
+export VISIER_TARGET_TENANT_ID=tenant-code
+export VISIER_APIKEY=the-api-key-issued-by-visier
+```
+
+Source this environment in and provide the password when prompted:
+```sh
+$ source .env
+```
+
 ## Connector Separation
 As of version `0.9.5`, the Python connector has separated the API calls from the `VisierSession` object. As a result of this change, the query execution methods on the `VisierSession` have been deprecated and will be subject to removal in a future release.
 
 The new way of invoking Visier public APIs through the Visier Python connector requires instantiating the appropriate API client and calling the methods defined on the client object. The following example, invokes the `analytic-objects` Model API to obtain the metadata for two analytic objects:
 ```python
     with VisierSession(auth) as session:
         model_client = ModelApiClient(session)
```

