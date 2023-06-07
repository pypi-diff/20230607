# Comparing `tmp/python-otbr-api-2.1.0.tar.gz` & `tmp/python-otbr-api-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-otbr-api-2.1.0.tar", last modified: Tue May 30 08:43:38 2023, max compression
+gzip compressed data, was "python-otbr-api-2.2.0.tar", last modified: Wed Jun  7 12:40:18 2023, max compression
```

## Comparing `python-otbr-api-2.1.0.tar` & `python-otbr-api-2.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:38.771971 python-otbr-api-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-30 08:43:38.771971 python-otbr-api-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:38.767971 python-otbr-api-2.1.0/python_otbr_api/
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/pskc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/tlv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:38.771971 python-otbr-api-2.1.0/python_otbr_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 08:43:38.771971 python-otbr-api-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:40:18.849282 python-otbr-api-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-07 12:40:18.849282 python-otbr-api-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:40:18.845282 python-otbr-api-2.2.0/python_otbr_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/pskc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/tlv_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:40:18.849282 python-otbr-api-2.2.0/python_otbr_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 12:40:18.849282 python-otbr-api-2.2.0/setup.cfg
```

### Comparing `python-otbr-api-2.1.0/LICENSE` & `python-otbr-api-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-otbr-api-2.1.0/pyproject.toml` & `python-otbr-api-2.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=65.6", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name         = "python-otbr-api"
-version      = "2.1.0"
+version      = "2.2.0"
 license      = {text = "MIT"}
 description  = "API to interact with an OTBR via its REST API"
 readme       = "README.md"
 authors      = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 requires-python = ">=3.9.0"
```

### Comparing `python-otbr-api-2.1.0/python_otbr_api/__init__.py` & `python-otbr-api-2.2.0/python_otbr_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,26 @@
         )
 
         if response.status == HTTPStatus.CONFLICT:
             raise ThreadNetworkActiveError
         if response.status not in (HTTPStatus.CREATED, HTTPStatus.OK):
             raise OTBRError(f"unexpected http status {response.status}")
 
+    async def delete_active_dataset(self) -> None:
+        """Delete active operational dataset."""
+        response = await self._session.delete(
+            f"{self._url}/node/dataset/active",
+            timeout=aiohttp.ClientTimeout(total=self._timeout),
+        )
+
+        if response.status == HTTPStatus.CONFLICT:
+            raise ThreadNetworkActiveError
+        if response.status != HTTPStatus.OK:
+            raise OTBRError(f"unexpected http status {response.status}")
+
     async def create_pending_dataset(self, dataset: PendingDataSet) -> None:
         """Create pending operational dataset.
 
         The passed in PendingDataSet does not need to be fully populated, any fields
         not set will be automatically set by the open thread border router.
         Raises if the http status is 400 or higher or if the response is invalid.
         """
@@ -144,14 +156,26 @@
         )
 
         if response.status == HTTPStatus.CONFLICT:
             raise ThreadNetworkActiveError
         if response.status not in (HTTPStatus.CREATED, HTTPStatus.OK):
             raise OTBRError(f"unexpected http status {response.status}")
 
+    async def delete_pending_dataset(self) -> None:
+        """Delete pending operational dataset."""
+        response = await self._session.delete(
+            f"{self._url}/node/dataset/pending",
+            timeout=aiohttp.ClientTimeout(total=self._timeout),
+        )
+
+        if response.status == HTTPStatus.CONFLICT:
+            raise ThreadNetworkActiveError
+        if response.status != HTTPStatus.OK:
+            raise OTBRError(f"unexpected http status {response.status}")
+
     async def set_active_dataset_tlvs(self, dataset: bytes) -> None:
         """Set current active operational dataset.
 
         Raises if the http status is 400 or higher or if the response is invalid.
         """
 
         response = await self._session.put(
```

### Comparing `python-otbr-api-2.1.0/python_otbr_api/mdns.py` & `python-otbr-api-2.2.0/python_otbr_api/mdns.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-2.1.0/python_otbr_api/models.py` & `python-otbr-api-2.2.0/python_otbr_api/models.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-2.1.0/python_otbr_api/pskc.py` & `python-otbr-api-2.2.0/python_otbr_api/pskc.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-2.1.0/python_otbr_api/tlv_parser.py` & `python-otbr-api-2.2.0/python_otbr_api/tlv_parser.py`

 * *Files identical despite different names*

