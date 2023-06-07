# Comparing `tmp/cryoet_data_portal-0.0.1.tar.gz` & `tmp/cryoet_data_portal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryoet_data_portal-0.0.1.tar", last modified: Tue Jun  6 04:43:45 2023, max compression
+gzip compressed data, was "cryoet_data_portal-0.0.2.tar", last modified: Wed Jun  7 19:38:09 2023, max compression
```

## Comparing `cryoet_data_portal-0.0.1.tar` & `cryoet_data_portal-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:43:45.283725 cryoet_data_portal-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-06 04:43:45.283725 cryoet_data_portal-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:43:45.279725 cryoet_data_portal-0.0.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 04:43:45.283725 cryoet_data_portal-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:43:45.275725 cryoet_data_portal-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:43:45.279725 cryoet_data_portal-0.0.1/src/cryoet_data_portal/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/src/cryoet_data_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/src/cryoet_data_portal/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/src/cryoet_data_portal/_file_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/src/cryoet_data_portal/_gql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/src/cryoet_data_portal/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:43:45.279725 cryoet_data_portal-0.0.1/src/cryoet_data_portal/data/
--rw-r--r--   0 runner    (1001) docker     (123)   174865 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/src/cryoet_data_portal/data/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:43:45.279725 cryoet_data_portal-0.0.1/src/cryoet_data_portal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-06 04:43:45.000000 cryoet_data_portal-0.0.1/src/cryoet_data_portal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-06 04:43:45.000000 cryoet_data_portal-0.0.1/src/cryoet_data_portal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:43:45.000000 cryoet_data_portal-0.0.1/src/cryoet_data_portal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-06 04:43:45.000000 cryoet_data_portal-0.0.1/src/cryoet_data_portal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 04:43:45.000000 cryoet_data_portal-0.0.1/src/cryoet_data_portal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:43:45.279725 cryoet_data_portal-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-06 04:43:25.000000 cryoet_data_portal-0.0.1/tests/test_get_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.616719 cryoet_data_portal-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 19:38:09.616719 cryoet_data_portal-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.612719 cryoet_data_portal-0.0.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:38:09.616719 cryoet_data_portal-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.612719 cryoet_data_portal-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.612719 cryoet_data_portal-0.0.2/src/cryoet_data_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/_file_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/_gql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26971 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.612719 cryoet_data_portal-0.0.2/src/cryoet_data_portal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   174865 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/data/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.612719 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 19:38:09.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-07 19:38:09.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:38:09.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 19:38:09.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 19:38:09.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.616719 cryoet_data_portal-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/tests/test_get_client.py
```

### Comparing `cryoet_data_portal-0.0.1/LICENSE` & `cryoet_data_portal-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.1/PKG-INFO` & `cryoet_data_portal-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoet_data_portal
-Version: 0.0.1
+Version: 0.0.2
 Summary: API Client to facilitate the use of the CryoET Portal. For more information about the API and the project visit https://github.com/chanzuckerberg/cryoet-data-portal/
 Author-email: Chan Zuckerberg Initiative <cryoetdataportal@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cryoet-data-portal
 Project-URL: repository, https://github.com/chanzuckerberg/cryoet-data-portal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cryoet_data_portal-0.0.1/README.md` & `cryoet_data_portal-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.1/pyproject.toml` & `cryoet_data_portal-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.1/src/cryoet_data_portal/__init__.py` & `cryoet_data_portal-0.0.2/src/cryoet_data_portal/__init__.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.1/src/cryoet_data_portal/_client.py` & `cryoet_data_portal-0.0.2/src/cryoet_data_portal/_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,28 @@
 
 from gql import Client as GQLClient
 from gql.dsl import DSLQuery, DSLSchema, dsl_gql
 from gql.transport.requests import RequestsHTTPTransport
 
 
 class Client:
+    """A GraphQL Client library that can traverse all of the metadata in the CryoET Data Portal
+
+    Args:
+        url (Optional[str]): The API URL to connect to, defaults to "https://graphql.cryoetdataportal.cziscience.com/v1/graphql"
+
+    Returns:
+        A GraphQL API Client library
+
+    Examples:
+        Generate a client that connects to the default GraphQL API:
+
+        >>> client = cryoet_data_portal.Client()
+    """
+
     def __init__(self, url: Optional[str] = None):
         # Use our default API URL
         if not url:
             url = "https://graphql.cryoetdataportal.cziscience.com/v1/graphql"
         transport = RequestsHTTPTransport(
             url=url,
             retries=3,
@@ -30,18 +44,14 @@
         else:
             query_filters = {"where": query_filters}
         gql_type = getattr(ds, gql_class_name)
         scalar_fields = [getattr(gql_type, fieldname) for fieldname in cls._get_scalar_fields()]
         query = dsl_gql(DSLQuery(getattr(ds.query_root, gql_class_name)(**query_filters).select(*scalar_fields)))
         return query
 
-    def generate_filters(self, cls, field, value):
-        filter = {"where": {field: {"_eq": value}}}
-        return filter
-
     def find(self, cls, query_filters=None):
         gql_type = cls._get_gql_type()
         response = self.client.execute(self.build_query(cls, gql_type, query_filters))
         for item in response[gql_type]:
             yield cls(self, **item)
 
     def find_one(self, *args, **kwargs):
```

### Comparing `cryoet_data_portal-0.0.1/src/cryoet_data_portal/_file_tools.py` & `cryoet_data_portal-0.0.2/src/cryoet_data_portal/_file_tools.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.1/src/cryoet_data_portal/data/schema.graphql` & `cryoet_data_portal-0.0.2/src/cryoet_data_portal/data/schema.graphql`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.1/src/cryoet_data_portal.egg-info/PKG-INFO` & `cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoet-data-portal
-Version: 0.0.1
+Version: 0.0.2
 Summary: API Client to facilitate the use of the CryoET Portal. For more information about the API and the project visit https://github.com/chanzuckerberg/cryoet-data-portal/
 Author-email: Chan Zuckerberg Initiative <cryoetdataportal@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cryoet-data-portal
 Project-URL: repository, https://github.com/chanzuckerberg/cryoet-data-portal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cryoet_data_portal-0.0.1/src/cryoet_data_portal.egg-info/SOURCES.txt` & `cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.1/tests/README.md` & `cryoet_data_portal-0.0.2/tests/README.md`

 * *Files identical despite different names*

