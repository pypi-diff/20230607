# Comparing `tmp/RecordKeeper_Client-3.1.0.tar.gz` & `tmp/RecordKeeper_Client-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RecordKeeper_Client-3.1.0.tar", last modified: Wed May 17 12:57:40 2023, max compression
+gzip compressed data, was "RecordKeeper_Client-3.2.0.tar", last modified: Wed Jun  7 14:01:01 2023, max compression
```

## Comparing `RecordKeeper_Client-3.1.0.tar` & `RecordKeeper_Client-3.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-17 12:57:40.003083 RecordKeeper_Client-3.1.0/
--rw-r--r--   0 hubert    (1001) hubert    (1001)    35149 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.1.0/LICENSE
--rw-r--r--   0 hubert    (1001) hubert    (1001)       16 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.1.0/MANIFEST.in
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     6142 2023-05-17 12:57:40.003083 RecordKeeper_Client-3.1.0/PKG-INFO
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     4275 2023-05-17 12:49:18.000000 RecordKeeper_Client-3.1.0/README.md
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-17 12:57:39.999083 RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     6142 2023-05-17 12:57:39.000000 RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/PKG-INFO
--rw-rw-r--   0 hubert    (1001) hubert    (1001)      416 2023-05-17 12:57:39.000000 RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/SOURCES.txt
--rw-rw-r--   0 hubert    (1001) hubert    (1001)        1 2023-05-17 12:57:39.000000 RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/dependency_links.txt
--rw-rw-r--   0 hubert    (1001) hubert    (1001)        9 2023-05-17 12:57:39.000000 RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/top_level.txt
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-17 12:57:40.003083 RecordKeeper_Client-3.1.0/rkclient/
--rw-rw-r--   0 hubert    (1001) hubert    (1001)      820 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/rkclient/__init__.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)    14001 2023-05-12 12:37:06.000000 RecordKeeper_Client-3.1.0/rkclient/admin.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)       97 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.1.0/rkclient/auth.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     5540 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/rkclient/client.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     3264 2023-03-29 19:51:20.000000 RecordKeeper_Client-3.1.0/rkclient/entities.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     2294 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.1.0/rkclient/factory.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     3456 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/rkclient/request.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     4486 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/rkclient/serialization.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)       38 2023-05-17 12:57:40.003083 RecordKeeper_Client-3.1.0/setup.cfg
--rw-rw-r--   0 hubert    (1001) hubert    (1001)      894 2023-03-15 09:31:37.000000 RecordKeeper_Client-3.1.0/setup.py
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-17 12:57:40.003083 RecordKeeper_Client-3.1.0/test/
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     2880 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/test/test_api.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     6627 2023-05-09 09:27:33.000000 RecordKeeper_Client-3.1.0/test/test_serialization.py
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-07 14:01:01.379995 RecordKeeper_Client-3.2.0/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)    35149 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.2.0/LICENSE
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       16 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.2.0/MANIFEST.in
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     6500 2023-06-07 14:01:01.379995 RecordKeeper_Client-3.2.0/PKG-INFO
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     4545 2023-06-07 14:00:19.000000 RecordKeeper_Client-3.2.0/README.md
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-07 14:01:01.375995 RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     6500 2023-06-07 14:01:01.000000 RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/PKG-INFO
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)      434 2023-06-07 14:01:01.000000 RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/SOURCES.txt
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)        1 2023-06-07 14:01:01.000000 RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/dependency_links.txt
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)        9 2023-06-07 14:01:01.000000 RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/top_level.txt
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-07 14:01:01.379995 RecordKeeper_Client-3.2.0/rkclient/
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)      855 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/__init__.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     3806 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/admin.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)       97 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.2.0/rkclient/auth.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     4439 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/client.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     3264 2023-06-07 12:22:19.000000 RecordKeeper_Client-3.2.0/rkclient/entities.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     2294 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.2.0/rkclient/factory.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)    12049 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/query.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     4166 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/request.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     4770 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/serialization.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)       38 2023-06-07 14:01:01.379995 RecordKeeper_Client-3.2.0/setup.cfg
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)      894 2023-03-15 09:31:37.000000 RecordKeeper_Client-3.2.0/setup.py
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-07 14:01:01.379995 RecordKeeper_Client-3.2.0/test/
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     2665 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/test/test_api.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     6627 2023-06-07 12:22:19.000000 RecordKeeper_Client-3.2.0/test/test_serialization.py
```

### Comparing `RecordKeeper_Client-3.1.0/LICENSE` & `RecordKeeper_Client-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.1.0/PKG-INFO` & `RecordKeeper_Client-3.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecordKeeper_Client
-Version: 3.1.0
+Version: 3.2.0
 Summary: Client library for accessing Record Keepers Receiver
 Home-page: UNKNOWN
 Author: ERST
 Author-email: noreply@example.ecom
 License: GPLv3+
 Description: 
         # Context
@@ -45,29 +45,36 @@
         
         # API
         
         RKClient:
         - prepare_pem
         - prepare_artifact
         - send_pem
-        - get_info
-        - get_tag
         - set_tag
         
-        RKAdmin:
+        RKQuery:
         - get_pems
         - get_pems_count
         - get_artifact
         - get_artifacts
         - get_artifacts_count
         - get_taxonomy_file
+        - get_tag
         - get_tags
         - get_tags_count
+        - get_info
+        
+        RKAdmin:
+        - check_connections
         - query_graph
         - clean_dbs
+        - graph_rebuild
+        - graph_flush
+        - graph_verify
+        - get_graph_info
         
         
         # Authenticating
         
         If you want to do anything more than sending a PEM, you will need to pass a
         RK authentication credential when creating RKClient or RKAdmin.
         
@@ -82,25 +89,29 @@
         However, you will need to ask RK admin to create the PUC and send you its auth code.
         
         ## RKClient from Python console
         
         ```
         cd rkclient/
         python3
-        >>> from rkclient import RKAdmin
-        >>> rk = RKAdmin('http://127.0.0.1:8082/receiver/')
+        >>> from rkclient import RKQuery
+        >>> rk = RKQuery('http://127.0.0.1:8082/receiver/')
         >>> pems, msg, ok = rk.get_pems()
         >>> assert ok, msg
         >>> for pem in pems:
         >>>   print(pem)
         ```
         ## Changelog
         
         ### Unreleased
         
+        ### [3.2.0] - 2023-06-07
+        - Moved "getter" functions to new class RKQuery. RKAdmin is left with truly low-level functions.
+        - Added helper function RKQuery.get_artifact_latest().
+        
         ## [3.1.0] - 2023-04-06 and 2023-05-17
         - Improved error logging, by creating less irrelevant logs. 
         - Add default User-Agent to requests to be equal to `recordkeeper-client-{version}`.
         - RKAdmin supports /info and /verify endpoints of GraphBuilder.
         
         ## [3.0.0] - 2023-02-06
         - Changed Artifact id field from uuid to string. This forces changes in many functions API.
```

### Comparing `RecordKeeper_Client-3.1.0/README.md` & `RecordKeeper_Client-3.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,29 +37,36 @@
 
 # API
 
 RKClient:
 - prepare_pem
 - prepare_artifact
 - send_pem
-- get_info
-- get_tag
 - set_tag
 
-RKAdmin:
+RKQuery:
 - get_pems
 - get_pems_count
 - get_artifact
 - get_artifacts
 - get_artifacts_count
 - get_taxonomy_file
+- get_tag
 - get_tags
 - get_tags_count
+- get_info
+
+RKAdmin:
+- check_connections
 - query_graph
 - clean_dbs
+- graph_rebuild
+- graph_flush
+- graph_verify
+- get_graph_info
 
 
 # Authenticating
 
 If you want to do anything more than sending a PEM, you will need to pass a
 RK authentication credential when creating RKClient or RKAdmin.
 
@@ -74,25 +81,29 @@
 However, you will need to ask RK admin to create the PUC and send you its auth code.
 
 ## RKClient from Python console
 
 ```
 cd rkclient/
 python3
->>> from rkclient import RKAdmin
->>> rk = RKAdmin('http://127.0.0.1:8082/receiver/')
+>>> from rkclient import RKQuery
+>>> rk = RKQuery('http://127.0.0.1:8082/receiver/')
 >>> pems, msg, ok = rk.get_pems()
 >>> assert ok, msg
 >>> for pem in pems:
 >>>   print(pem)
 ```
 ## Changelog
 
 ### Unreleased
 
+### [3.2.0] - 2023-06-07
+- Moved "getter" functions to new class RKQuery. RKAdmin is left with truly low-level functions.
+- Added helper function RKQuery.get_artifact_latest().
+
 ## [3.1.0] - 2023-04-06 and 2023-05-17
 - Improved error logging, by creating less irrelevant logs. 
 - Add default User-Agent to requests to be equal to `recordkeeper-client-{version}`.
 - RKAdmin supports /info and /verify endpoints of GraphBuilder.
 
 ## [3.0.0] - 2023-02-06
 - Changed Artifact id field from uuid to string. This forces changes in many functions API.
```

### Comparing `RecordKeeper_Client-3.1.0/RecordKeeper_Client.egg-info/PKG-INFO` & `RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecordKeeper-Client
-Version: 3.1.0
+Version: 3.2.0
 Summary: Client library for accessing Record Keepers Receiver
 Home-page: UNKNOWN
 Author: ERST
 Author-email: noreply@example.ecom
 License: GPLv3+
 Description: 
         # Context
@@ -45,29 +45,36 @@
         
         # API
         
         RKClient:
         - prepare_pem
         - prepare_artifact
         - send_pem
-        - get_info
-        - get_tag
         - set_tag
         
-        RKAdmin:
+        RKQuery:
         - get_pems
         - get_pems_count
         - get_artifact
         - get_artifacts
         - get_artifacts_count
         - get_taxonomy_file
+        - get_tag
         - get_tags
         - get_tags_count
+        - get_info
+        
+        RKAdmin:
+        - check_connections
         - query_graph
         - clean_dbs
+        - graph_rebuild
+        - graph_flush
+        - graph_verify
+        - get_graph_info
         
         
         # Authenticating
         
         If you want to do anything more than sending a PEM, you will need to pass a
         RK authentication credential when creating RKClient or RKAdmin.
         
@@ -82,25 +89,29 @@
         However, you will need to ask RK admin to create the PUC and send you its auth code.
         
         ## RKClient from Python console
         
         ```
         cd rkclient/
         python3
-        >>> from rkclient import RKAdmin
-        >>> rk = RKAdmin('http://127.0.0.1:8082/receiver/')
+        >>> from rkclient import RKQuery
+        >>> rk = RKQuery('http://127.0.0.1:8082/receiver/')
         >>> pems, msg, ok = rk.get_pems()
         >>> assert ok, msg
         >>> for pem in pems:
         >>>   print(pem)
         ```
         ## Changelog
         
         ### Unreleased
         
+        ### [3.2.0] - 2023-06-07
+        - Moved "getter" functions to new class RKQuery. RKAdmin is left with truly low-level functions.
+        - Added helper function RKQuery.get_artifact_latest().
+        
         ## [3.1.0] - 2023-04-06 and 2023-05-17
         - Improved error logging, by creating less irrelevant logs. 
         - Add default User-Agent to requests to be equal to `recordkeeper-client-{version}`.
         - RKAdmin supports /info and /verify endpoints of GraphBuilder.
         
         ## [3.0.0] - 2023-02-06
         - Changed Artifact id field from uuid to string. This forces changes in many functions API.
```

### Comparing `RecordKeeper_Client-3.1.0/rkclient/__init__.py` & `RecordKeeper_Client-3.2.0/rkclient/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from rkclient.client import RKClient, PEM, Artifact
 from rkclient.serialization import ArtifactSerialization, PEMSerialization, Info, GraphBuilderInfo, deserialize_info, deserialize_graph_builder_info
 from rkclient.admin import RKAdmin
+from rkclient.query import RKQuery
 from rkclient.factory import RKClientFactory
 
 import os
 import logging
 
 LOG_FORMAT = '[%(asctime)s] - %(levelname)s - RKClient: %(message)s'
 LOG_DATE_FORMAT = '%Y-%m-%d %H:%M:%S'
```

### Comparing `RecordKeeper_Client-3.1.0/rkclient/admin.py` & `RecordKeeper_Client-3.2.0/rkclient/query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,57 @@
 import ast
 import json
-import logging
-import time
-from typing import Tuple, List, Optional, Any, Callable, Dict
+from typing import Tuple, List, Optional, Any, Dict
 from uuid import UUID
+import logging
+from importlib.metadata import version
 
-from rkclient.client import RKClient
 from rkclient.entities import Artifact, PEM
-from rkclient.request import _parse_sorting_filtering_params, RequestHelper
-from rkclient.serialization import ArtifactSerialization, PEMSerialization, _decode_from_base64
+from rkclient.request import _parse_sorting_filtering_params, RequestHelper, _handle_request, \
+    _handle_request_with_response
+from rkclient.serialization import ArtifactSerialization, PEMSerialization, _decode_from_base64, _encode_as_base64, \
+    create_artifact_from_neo4j
 
 log = logging.getLogger("rkclient")
+RK_VERSION = version('RecordKeeper_Client')
 
 
-class RKAdmin:
+class RKQuery:
     """
-    This class is not supposed to be used by normal RK user, but by RK administrator or in tests.
+    Calls RK Query service to obtain data about RK from SQL db and from graph view.
     """
 
     def __init__(self,
                  receiver_url: str,
-                 graph_builder_url: str,
                  timeout_sec: int = 5,
                  insecure: bool = True,
                  user_auth: str = '',
                  puc_auth: str = ''):
-        self.receiver_client = RKClient(receiver_url, emitter_id='admin', timeout_sec=timeout_sec, insecure=insecure,
-                                        user_auth=user_auth, puc_auth=puc_auth)
-        graph_builder_url = graph_builder_url.rstrip('/')
-        log.info(f"Connecting to Graph Builder: {graph_builder_url}")
-        self.graph_builder_client = RequestHelper(graph_builder_url, timeout_sec=timeout_sec, insecure=insecure,
-                                                  user_auth=user_auth, puc_auth=puc_auth,
-                                                  user_agent=f'recordkeeper-client-{self.receiver_client.get_version()}')
-
-    def check_connections(self) -> Tuple[str, bool]:
-        msg, ok = self.graph_builder_client.get("/info")
-        if not ok:
-            return f"Graph Builder connection error: {msg}", False
-        msg, ok = self.receiver_client.get_info()
-        if not ok:
-            return f"Receiver connection error: {msg}", False
-        return 'OK', True
-
-    def graph_rebuild(self) -> Tuple[str, bool]:
-        """
-        :return: first element: error message or 'OK'
-                 second element: True for success, False for error
-        """
-        text, ok = self.graph_builder_client.post("/rebuild", "{}")
-        if not ok:
-            return f"Starting rebuilding process failed: {text}", False
-        return 'OK', True
-
-    def graph_flush(self) -> Tuple[str, bool]:
-        """
-        Waits till all PEMs from queue have been added to graph.
-        :return: first element: error message or 'OK'
-                 second element: True for success, False for error
-        """
-        start_time = time.time()
-        text, ok = self.graph_builder_client.post("/flush", "{}")
-        total_flush_time = time.time() - start_time
-        if not ok:
-            return f"flushing queue failed: {text}", False
-        return f"flushing queue finished, in {total_flush_time:.2f}s", True
-
-    def graph_verify(self) -> Tuple[str, bool]:
-        """
-        Starts sql vs graph comparison, and returns result as string with newlines.
-        :return: first element: error message or 'OK'
-                 second element: True for success, False for error
-        """
-        text, ok = self.graph_builder_client.post("/verify", "{}")
-        if not ok:
-            return f"Verifying integrity failed: {text}", False
-        return text, True
+        receiver_url = receiver_url.rstrip('/')
+        self.receiver_request = RequestHelper(receiver_url, timeout_sec, insecure, user_auth, puc_auth, f'recordkeeper-client-{RK_VERSION}')
+        log.info(f"ver {RK_VERSION}, connecting to: {receiver_url}")
 
-    def get_graph_info(self) -> Tuple[str, bool]:
+    def get_info(self) -> Tuple[str, bool]:
         """
-        Returns json with fields as in GraphBuilderInfo class - the GB state. Use `deserialize_graph_builder_info` for easy parsing.
+        Returns json with fields as in Info class - the Receiver state. Use `deserialize_info` for easy parsing.
         :return: check class description
         """
-        text, ok = self.graph_builder_client.get("/info")
-        return text, ok
+        def _get_info():
+            return self.receiver_request.get("/info")
 
-    def clean_dbs(self) -> Tuple[str, bool]:
-        """
-        :return: first element: error message or 'OK'
-                 second element: True for success, False for error
-        """
-        text, ok = self.receiver_client.receiver_request.post("/clean", "{}")
-        if not ok:
-            return f"Cleaning db failed: {text}", False
-        return 'OK', True
+        return _handle_request_with_response(_get_info, "Getting info", True)
 
     def get_pem(self, pem_id: str) -> Tuple[Optional[PEM], str, bool]:
         """
-        Returns pem from sql db.
+        Returns pem from sql db. Warning: the artifacts will contain just names, without properties.
         :param pem_id: UUID, should be in hex format.
         :return: PEM or None
         """
         def _get_pem() -> Tuple[Optional[PEM], str, bool]:
-            text, ok = self.receiver_client.receiver_request.get(f"/pem/{pem_id}")
+            text, ok = self.receiver_request.get(f"/pem/{pem_id}")
             if not ok:
                 return None, text, False
             pem_json = json.loads(text)
             pem = PEMSerialization.from_dict(pem_json, True)
             return pem, 'OK', True
 
         return _handle_request(_get_pem, "Getting pem")
@@ -128,15 +74,15 @@
                  The artifacts lists in PEM will contain only artifact ID
                  second element: True for success, False for error
         """
 
         def _get_pems() -> Tuple[List[Any], str, bool]:
             query_params: Dict[str, Any] = _parse_sorting_filtering_params(page_index, page_size,
                                                                            sort_field, sort_order, filters)
-            text, ok = self.receiver_client.receiver_request.get("/pems", query_params)
+            text, ok = self.receiver_request.get("/pems", query_params)
             if not ok:
                 return [], text, False
             pems = []
             pems_json = json.loads(text)
             for p in pems_json:
                 pems.append(PEMSerialization.from_dict(p, True))
             return pems, 'OK', True
@@ -152,15 +98,15 @@
         """
         Returns amount of PEMs which match the filters. See `get_pems` for more info.
         """
 
         def _get_pems() -> Tuple[int, str, bool]:
             query_params: Dict[str, Any] = _parse_sorting_filtering_params(page_index, page_size,
                                                                            sort_field, sort_order, filters)
-            text, ok = self.receiver_client.receiver_request.get("/pems_count", query_params)
+            text, ok = self.receiver_request.get("/pems_count", query_params)
             if not ok:
                 return -1, text, False
             obj = json.loads(text)
             return int(obj['pems_count']), 'OK', True
 
         return _handle_request(_get_pems, "Getting pems count")
 
@@ -174,14 +120,31 @@
         artifacts: List[Artifact] = res
         for a in artifacts:
             if a.Name == artifact_name:
                 return a, True
 
         return None, True
 
+    def get_artifact_latest(self, artifact_name: str) -> Tuple[Optional[Artifact], str, bool]:
+        """
+        Returns the newest Artifact whose name includes the string provided by the artifact_name argument.
+        """
+        artifacts, msg, ok = self.get_artifacts(
+            sort_field='CreatedAt',
+            sort_order='desc',
+            page_size=1,
+            filters={'Name': artifact_name}
+        )
+        if ok:
+            if len(artifacts) > 0:
+                return artifacts[0], "", True
+            else:
+                return None, "", True
+        return None, msg, False
+
     def get_artifacts(self,
                       source: str = 'sqldb',
                       page_index: int = -1,
                       page_size: int = -1,
                       sort_field: str = '',
                       sort_order: str = '',
                       filters: Optional[Dict] = None) -> Tuple[List[Artifact], str, bool]:
@@ -214,15 +177,15 @@
         :return: first element: count of artifact objs
                  second element: optional str error message
                  third element: True for success, False for error
         """
 
         def _get_artifacts_count_from_sql() -> Tuple[int, str, bool]:
             query_params: Dict[str, Any] = _parse_sorting_filtering_params(-1, -1, "", "", filters)
-            text, ok = self.receiver_client.receiver_request.get("/artifacts_count", query_params)
+            text, ok = self.receiver_request.get("/artifacts_count", query_params)
             if not ok:
                 return -1, text, False
             objs = json.loads(text)
             return int(objs['artifacts_count']), "", True
 
         def _get_artifacts_count_from_graph() -> Tuple[int, str, bool]:
             text, ok = self.query_graph('MATCH (a:Artifact) RETURN count(a);', 'r')
@@ -235,60 +198,72 @@
             return _handle_request(_get_artifacts_count_from_sql, 'Getting artifacts count')
         elif source == 'graphdb':
             return _handle_request(_get_artifacts_count_from_graph, 'Getting artifacts count')
         else:
             return -1, f"Getting artifacts count: didn't recognize source: {source}", False
 
     def get_taxonomy_file(self, taxonomy_id: UUID) -> Tuple[str, bool]:
-        text, ok = self.receiver_client.receiver_request.get(f"/taxonomy/{taxonomy_id.hex}")
+        text, ok = self.receiver_request.get(f"/taxonomy/{taxonomy_id.hex}")
         if not ok:
             return f"Getting taxonomy file failed: {text}", False
         return _decode_from_base64(text), True
 
+    def get_tag(self, namespace: str, tag_name: str) -> Tuple[str, bool]:
+        """
+        Returned tag is UUID in hex (do: UUID(hex=result))
+        :return: check class description
+        """
+        def _get_tag():
+            tag_base64 = _encode_as_base64(tag_name)
+            namespace_base64 = _encode_as_base64(namespace)
+            return self.receiver_request.get(f"/tag/{namespace_base64}/{tag_base64}")
+
+        return _handle_request_with_response(_get_tag, "Getting tag", True)
+
     def get_tags(self) -> Tuple[List[Dict], str, bool]:
         """
         :return: first element: list of metadata (as Dict), with fields: NamespaceID, Tag, EventID, UpdatedAt
                  second element: error message
                  third element: True for success, False for error
         """
 
         def _get_tags() -> Tuple[List[Any], str, bool]:
-            text, ok = self.receiver_client.receiver_request.get("/tags")
+            text, ok = self.receiver_request.get("/tags")
             if not ok:
                 return [], text, False
             tags = json.loads(text)
             return tags, 'OK', True
 
         return _handle_request(_get_tags, "Getting tags")
 
     def get_tags_count(self) -> Tuple[int, str, bool]:
         """
         Returns amount of tags.
         """
 
         def _get_tags() -> Tuple[int, str, bool]:
-            text, ok = self.receiver_client.receiver_request.get("/tags_count")
+            text, ok = self.receiver_request.get("/tags_count")
             if not ok:
                 return -1, text, False
             obj = json.loads(text)
             return int(obj['tags_count']), 'OK', True
 
         return _handle_request(_get_tags, "Getting tags count")
 
     def query_graph(self, query: str, query_type='rw') -> Tuple[str, bool]:
         """
         :return: first element: returned result (as str with format corresponding to what query requests) or error message
                  second element: True for success, False for error
         """
         query_fmt = f'"query": "{query}", "type": "{query_type}"'
         payload = '{' + query_fmt + '}'
-        return self.receiver_client.receiver_request.post("/query", payload)
+        return self.receiver_request.post("/query", payload)
 
     def _get_artifacts_from_sql(self, query_params: Dict[str, Any]) -> Tuple[List[Artifact], str, bool]:
-        text, ok = self.receiver_client.receiver_request.get("/artifacts", query_params)
+        text, ok = self.receiver_request.get("/artifacts", query_params)
         if not ok:
             return [], f"Querying SQL failed: {text}", False
 
         objs = json.loads(text)
         artifacts: List[Artifact] = [ArtifactSerialization.from_dict(o) for o in objs]
         return artifacts, "", True
 
@@ -300,29 +275,7 @@
         # the text contains python like list [['<name>','<properties-as-json>'], ['<name>', ... ] ]
         objs = ast.literal_eval(text)
         artifacts: List[Artifact] = [
             create_artifact_from_neo4j(o)
             for o in objs
         ]
         return artifacts, "", True
-
-
-def create_artifact_from_neo4j(result: tuple) -> Artifact:
-    art = ArtifactSerialization.from_dict(
-        {'Name': result[0],
-         'Properties': json.loads(result[1]) if result[1] else {},
-         'CreatedAt': result[2],
-         'TaxonomyFiles': None}
-    )
-    return art
-
-
-def _handle_request(func: Callable, name: str) -> Tuple[Any, str, bool]:
-    """
-    Wraps the error, logging and exception handling.
-    """
-    obj, text, ok = func()
-    if not ok:
-        text = f"{name} failed: {text}"
-        log.error(text)
-        return "", text, False
-    return obj, 'OK', True
```

### Comparing `RecordKeeper_Client-3.1.0/rkclient/entities.py` & `RecordKeeper_Client-3.2.0/rkclient/entities.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.1.0/rkclient/factory.py` & `RecordKeeper_Client-3.2.0/rkclient/factory.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.1.0/rkclient/request.py` & `RecordKeeper_Client-3.2.0/rkclient/request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ssl
 import logging
 import urllib.parse
 import urllib.request
 from _socket import timeout
-from typing import Optional, Dict, Any, Tuple
+from typing import Optional, Dict, Any, Tuple, Callable
 from urllib.error import HTTPError, URLError
 
 from rkclient.auth import RK_USER_AUTH_HEADER, RK_PUC_AUTH_HEADER
 
 log = logging.getLogger("rkclient")
 
 
@@ -88,7 +88,33 @@
     if sort_order != '':
         params['sortOrder'] = sort_order
 
     for key, value in filters.items():
         params[key] = value
     return params
 
+
+def _handle_request(func: Callable, name: str) -> Tuple[Any, str, bool]:
+    """
+    Wraps the error, logging and exception handling.
+    """
+    obj, text, ok = func()
+    if not ok:
+        text = f"{name} failed: {text}"
+        log.error(text)
+        return "", text, False
+    return obj, 'OK', True
+
+
+def _handle_request_with_response(func: Callable, name: str, ret_text_on_ok: bool = False) -> Tuple[str, bool]:
+    """
+    Wraps the error, logging and exception handling.
+    """
+    text, ok = func()
+    if not ok:
+        msg = f"{name} failed: {text}"
+        log.error(msg)
+        return msg, False
+    if ret_text_on_ok:
+        return text, True
+    else:
+        return 'OK', True
```

### Comparing `RecordKeeper_Client-3.1.0/rkclient/serialization.py` & `RecordKeeper_Client-3.2.0/rkclient/serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,7 +141,16 @@
 def deserialize_graph_builder_info(s: str) -> Optional[GraphBuilderInfo]:
     try:
         json_obj = json.loads(s)
         return GraphBuilderInfo(**json_obj)
     except JSONDecodeError:
         return None
 
+
+def create_artifact_from_neo4j(result: tuple) -> Artifact:
+    art = ArtifactSerialization.from_dict(
+        {'Name': result[0],
+         'Properties': json.loads(result[1]) if result[1] else {},
+         'CreatedAt': result[2],
+         'TaxonomyFiles': None}
+    )
+    return art
```

### Comparing `RecordKeeper_Client-3.1.0/setup.py` & `RecordKeeper_Client-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.1.0/test/test_api.py` & `RecordKeeper_Client-3.2.0/test/test_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,44 +12,35 @@
         os.environ['RK_MOCK'] = 'true'
         rk = RKClientFactory.get('', 'emitter-name')
         del os.environ['RK_MOCK']
 
         pred = rk.prepare_pem('', None)
         self.assertIsNotNone(pred)
 
-        pem = rk.prepare_pem('some_type_name', pred.ID, { "value_int": -123 })
+        pem = rk.prepare_pem('some_type_name', pred.ID, {"value_int": -123})
         self.assertIsNotNone(pem)
 
         _, ok = rk.send_pem(pred)
         self.assertTrue(ok)
 
-        _, ok = rk.get_info()
-        self.assertTrue(ok)
-
-        _, ok = rk.get_tag('test-namespace-unique-name', 'foo')
-        self.assertTrue(ok)
-
         _, ok = rk.set_tag('test-namespace-unique-name', 'bar', pem)
         self.assertTrue(ok)
 
-        _, ok = rk.get_info()
-        self.assertTrue(ok)
-
     def test_rk_factory_default(self):
         rk = RKClientFactory.get('http://localhost', 'emitter-name')
         pem = rk.prepare_pem('', None)
         self.assertIsNotNone(pem)
 
         _, ok = rk.send_pem(pem)
         self.assertFalse(ok)
 
     def test_prepare_pem(self):
         rk = RKClient('', 'emitter-name')
         pred = rk.prepare_pem('', None)
-        pem = rk.prepare_pem('some_type_name', pred.ID, { "value_int": -123 })
+        pem = rk.prepare_pem('some_type_name', pred.ID, {"value_int": -123})
 
         self.assertIs(type(pem.ID), UUID)
         self.assertEqual(pem.Predecessor, pred.ID)
         self.assertEqual(pem.Type, 'some_type_name')
         self.assertEqual(pem.Emitter, 'emitter-name')
         self.assertEqual(pem.Properties["value_int"], -123)
```

### Comparing `RecordKeeper_Client-3.1.0/test/test_serialization.py` & `RecordKeeper_Client-3.2.0/test/test_serialization.py`

 * *Files identical despite different names*

