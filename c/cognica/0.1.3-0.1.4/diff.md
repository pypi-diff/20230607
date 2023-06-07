# Comparing `tmp/cognica-0.1.3.tar.gz` & `tmp/cognica-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognica-0.1.3.tar", last modified: Sat Jun  3 01:44:36 2023, max compression
+gzip compressed data, was "cognica-0.1.4.tar", last modified: Wed Jun  7 03:53:32 2023, max compression
```

## Comparing `cognica-0.1.3.tar` & `cognica-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-03 01:44:36.687629 cognica-0.1.3/
--rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-29 03:56:50.000000 cognica-0.1.3/LICENSE
--rw-r--r--   0 jaepil     (501) staff       (20)    15701 2023-06-03 01:44:36.687434 cognica-0.1.3/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 05:58:03.000000 cognica-0.1.3/README.md
--rw-r--r--   0 jaepil     (501) staff       (20)     1337 2023-06-03 01:44:30.000000 cognica-0.1.3/pyproject.toml
--rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-06-03 01:44:36.687686 cognica-0.1.3/setup.cfg
--rw-r--r--   0 jaepil     (501) staff       (20)     2034 2023-06-03 01:44:25.000000 cognica-0.1.3/setup.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-03 01:44:36.683419 cognica-0.1.3/src/
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-03 01:44:36.684773 cognica-0.1.3/src/cognica/
--rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-15 08:05:25.000000 cognica-0.1.3/src/cognica/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-15 08:05:26.000000 cognica-0.1.3/src/cognica/channel.py
--rw-r--r--   0 jaepil     (501) staff       (20)    15678 2023-06-03 01:26:57.000000 cognica-0.1.3/src/cognica/document_db.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 03:46:32.000000 cognica-0.1.3/src/cognica/fts_analysis_pipeline.py
--rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 03:46:59.000000 cognica-0.1.3/src/cognica/key_value_db.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-03 01:44:36.687192 cognica-0.1.3/src/cognica/protobuf/
--rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-15 08:05:26.000000 cognica-0.1.3/src/cognica/protobuf/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)    12703 2023-06-03 01:42:35.000000 cognica-0.1.3/src/cognica/protobuf/document_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-06-03 01:34:57.000000 cognica-0.1.3/src/cognica/protobuf/document_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-06-03 01:33:38.000000 cognica-0.1.3/src/cognica/protobuf/document_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2669 2023-06-03 01:33:38.000000 cognica-0.1.3/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-06-03 01:35:26.000000 cognica-0.1.3/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     7337 2023-06-03 01:33:38.000000 cognica-0.1.3/src/cognica/protobuf/key_value_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-06-03 01:35:45.000000 cognica-0.1.3/src/cognica/protobuf/key_value_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     6085 2023-06-03 01:33:38.000000 cognica-0.1.3/src/cognica/protobuf/sentence_transformer_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-06-03 01:36:10.000000 cognica-0.1.3/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 03:47:19.000000 cognica-0.1.3/src/cognica/sentence_transformer.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-03 01:44:36.685796 cognica-0.1.3/src/cognica.egg-info/
--rw-r--r--   0 jaepil     (501) staff       (20)    15701 2023-06-03 01:44:36.000000 cognica-0.1.3/src/cognica.egg-info/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)      840 2023-06-03 01:44:36.000000 cognica-0.1.3/src/cognica.egg-info/SOURCES.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-06-03 01:44:36.000000 cognica-0.1.3/src/cognica.egg-info/dependency_links.txt
--rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-06-03 01:44:36.000000 cognica-0.1.3/src/cognica.egg-info/requires.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-06-03 01:44:36.000000 cognica-0.1.3/src/cognica.egg-info/top_level.txt
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 03:53:32.509926 cognica-0.1.4/
+-rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-29 03:56:50.000000 cognica-0.1.4/LICENSE
+-rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-07 03:53:32.509735 cognica-0.1.4/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 05:58:03.000000 cognica-0.1.4/README.md
+-rw-r--r--   0 jaepil     (501) staff       (20)     1282 2023-06-07 03:53:24.000000 cognica-0.1.4/pyproject.toml
+-rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-06-07 03:53:32.509968 cognica-0.1.4/setup.cfg
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 03:53:32.503395 cognica-0.1.4/src/
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 03:53:32.505759 cognica-0.1.4/src/cognica/
+-rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-15 08:05:25.000000 cognica-0.1.4/src/cognica/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-15 08:05:26.000000 cognica-0.1.4/src/cognica/channel.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    17045 2023-06-07 03:42:37.000000 cognica-0.1.4/src/cognica/document_db.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 03:46:32.000000 cognica-0.1.4/src/cognica/fts_analysis_pipeline.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 03:46:59.000000 cognica-0.1.4/src/cognica/key_value_db.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 03:53:32.509345 cognica-0.1.4/src/cognica/protobuf/
+-rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-15 08:05:26.000000 cognica-0.1.4/src/cognica/protobuf/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    13536 2023-06-07 03:42:37.000000 cognica-0.1.4/src/cognica/protobuf/document_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-06-03 01:34:57.000000 cognica-0.1.4/src/cognica/protobuf/document_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-06-03 01:33:38.000000 cognica-0.1.4/src/cognica/protobuf/document_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2669 2023-06-03 01:33:38.000000 cognica-0.1.4/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-06-03 01:35:26.000000 cognica-0.1.4/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     7337 2023-06-03 01:33:38.000000 cognica-0.1.4/src/cognica/protobuf/key_value_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-06-03 01:35:45.000000 cognica-0.1.4/src/cognica/protobuf/key_value_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     6085 2023-06-03 01:33:38.000000 cognica-0.1.4/src/cognica/protobuf/sentence_transformer_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-06-03 01:36:10.000000 cognica-0.1.4/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 03:47:19.000000 cognica-0.1.4/src/cognica/sentence_transformer.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 03:53:32.506587 cognica-0.1.4/src/cognica.egg-info/
+-rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-07 03:53:32.000000 cognica-0.1.4/src/cognica.egg-info/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)      831 2023-06-07 03:53:32.000000 cognica-0.1.4/src/cognica.egg-info/SOURCES.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-06-07 03:53:32.000000 cognica-0.1.4/src/cognica.egg-info/dependency_links.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-06-07 03:53:32.000000 cognica-0.1.4/src/cognica.egg-info/requires.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-06-07 03:53:32.000000 cognica-0.1.4/src/cognica.egg-info/top_level.txt
```

### Comparing `cognica-0.1.3/LICENSE` & `cognica-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/PKG-INFO` & `cognica-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python client for Cognica database
-Home-page: https://github.com/cognicadb/cognica-python
-Author: Cognica, Inc.
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -213,21 +211,19 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: protobuf
 License-File: LICENSE
 
 # Cognica Python Client
 
 A Python client for Cognica database server.
```

### Comparing `cognica-0.1.3/README.md` & `cognica-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/pyproject.toml` & `cognica-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cognica"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{ name = "Cognica, Inc.", email = "jaepil@cognica.io" }]
 description = "Python client for Cognica database"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
   "pandas>=1.5.3",
@@ -32,17 +32,18 @@
   "Environment :: Console",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 
 [project.urls]
 "Homepage" = "https://www.cognica.io"
+
+[tool.black]
+line-length = 80
```

### Comparing `cognica-0.1.3/src/cognica/__init__.py` & `cognica-0.1.4/src/cognica/__init__.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/channel.py` & `cognica-0.1.4/src/cognica/channel.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/document_db.py` & `cognica-0.1.4/src/cognica/document_db.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,32 +51,24 @@
 
 InsertRequest: t.TypeAlias = messages.InsertRequest  # type: ignore
 InsertResponse: t.TypeAlias = messages.InsertResponse  # type: ignore
 UpdateRequest: t.TypeAlias = messages.UpdateRequest  # type: ignore
 UpdateResponse: t.TypeAlias = messages.UpdateResponse  # type: ignore
 RemoveRequest: t.TypeAlias = messages.RemoveRequest  # type: ignore
 RemoveResponse: t.TypeAlias = messages.RemoveResponse  # type: ignore
-GetCollectionRequest: t.TypeAlias = (
-    messages.GetCollectionRequest  # type: ignore
-)
-GetCollectionResponse: t.TypeAlias = (
-    messages.GetCollectionResponse  # type: ignore
-)
+GetCollectionRequest: t.TypeAlias = messages.GetCollectionRequest  # type: ignore
+GetCollectionResponse: t.TypeAlias = messages.GetCollectionResponse  # type: ignore
 TruncateCollectionRequest: t.TypeAlias = (
     messages.TruncateCollectionRequest  # type: ignore
 )
 TruncateCollectionResponse: t.TypeAlias = (
     messages.TruncateCollectionResponse  # type: ignore
 )
-ListCollectionsRequest: t.TypeAlias = (
-    messages.ListCollectionsRequest  # type: ignore
-)
-ListCollectionsResponse: t.TypeAlias = (
-    messages.ListCollectionsResponse  # type: ignore
-)
+ListCollectionsRequest: t.TypeAlias = messages.ListCollectionsRequest  # type: ignore
+ListCollectionsResponse: t.TypeAlias = messages.ListCollectionsResponse  # type: ignore
 
 
 def _to_json(doc):
     if isinstance(doc, document_pb2.Document):  # type: ignore
         return doc
     elif isinstance(doc, (dict, list)):
         return document_pb2.Document(  # type: ignore
@@ -302,44 +294,46 @@
 
         return {
             "success": resp.status == 0,
             "message": resp.message,
             "data": [
                 {
                     "collection_name": resp.collection.collection_name,
-                    "primary_key": {
-                        "index_id": resp.collection.primary_key.index_id,
-                        "index_name": resp.collection.primary_key.index_name,
-                        "fields": list(resp.collection.primary_key.fields),
-                        "unique": resp.collection.primary_key.unique,
-                        "index_type": IndexType.Name(
-                            resp.collection.primary_key.index_type
-                        ),
-                        "status": IndexStatus.Name(
-                            resp.collection.primary_key.status
-                        ),
-                        "options": json.loads(
-                            resp.collection.primary_key.options.json or "{}"
-                        ),
-                    },
-                    "secondary_keys": [
+                    "index_descriptors": [
                         {
-                            "index_id": secondary_key.index_id,
-                            "index_name": secondary_key.index_name,
-                            "fields": list(secondary_key.fields),
-                            "unique": secondary_key.unique,
-                            "index_type": IndexType.Name(
-                                secondary_key.index_type
-                            ),
-                            "status": IndexStatus.Name(secondary_key.status),
+                            "index_id": index_desc.index_id,
+                            "index_name": index_desc.index_name,
+                            "fields": list(index_desc.fields),
+                            "unique": index_desc.unique,
+                            "index_type": IndexType.Name(index_desc.index_type),
+                            "status": IndexStatus.Name(index_desc.status),
                             "options": json.loads(
-                                secondary_key.options.json or "{}"
+                                index_desc.options.json or "{}"
                             ),
                         }
-                        for secondary_key in resp.collection.secondary_keys
+                        for index_desc in resp.collection.index_descriptors
+                    ],
+                    "index_stats": [
+                        {
+                            "index_id": index_stats.index_id,
+                            "index_name": index_stats.index_name,
+                            "approximated_size": index_stats.approximated_size,
+                            "num_docs": index_stats.num_docs,
+                            "accessed": index_stats.accessed,
+                            "added": index_stats.added,
+                            "updated": index_stats.updated,
+                            "deleted": index_stats.deleted,
+                            "merged": index_stats.merged,
+                            "accessed_at": index_stats.accessed_at,
+                            "added_at": index_stats.added_at,
+                            "updated_at": index_stats.updated_at,
+                            "deleted_at": index_stats.deleted_at,
+                            "merged_at": index_stats.merged_at,
+                        }
+                        for index_stats in resp.collection.index_stats
                     ],
                 }
             ],
         }
 
     def list_collections(self) -> t.List[str]:
         req = ListCollectionsRequest()
@@ -379,37 +373,56 @@
 
     def drop_index(self, collection, index_name) -> None:
         req = DropIndexRequest(
             collection_name=collection, index_name=index_name
         )
         self._invoke(self._stub.drop_index, req, wait_for_ready=True)
 
-    def get_index(
-        self, collection, index_name
-    ) -> t.List[t.Dict[str, t.Union[int, str]]]:
+    def get_index(self, collection, index_name) -> t.Dict[str, t.Any]:
         req = GetIndexRequest(collection_name=collection, index_name=index_name)
-
-        index_infos = []
-        resp: IndexDesc = self._invoke(
+        resp: GetIndexResponse = self._invoke(
             self._stub.get_index, req, wait_for_ready=True
         )
         index_desc = resp.index_desc
-        index_infos.append(
-            {
-                "index_id": index_desc.index_id,
-                "index_name": index_desc.index_name,
-                "fields": list(index_desc.fields),
-                "unique": index_desc.unique,
-                "index_type": index_desc.index_type,
-                "status": index_desc.status,
-                "options": str(index_desc.options),
-            }
-        )
+        index_stats = resp.index_stats
 
-        return index_infos
+        return {
+            "success": resp.status == 0,
+            "message": resp.message,
+            "data": [
+                {
+                    "collection_name": resp.collection_name,
+                    "index_descriptor": {
+                        "index_id": index_desc.index_id,
+                        "index_name": index_desc.index_name,
+                        "fields": list(index_desc.fields),
+                        "unique": index_desc.unique,
+                        "index_type": IndexType.Name(index_desc.index_type),
+                        "status": IndexStatus.Name(index_desc.status),
+                        "options": json.loads(index_desc.options.json or "{}"),
+                    },
+                    "index_stats": {
+                        "index_id": index_stats.index_id,
+                        "index_name": index_stats.index_name,
+                        "approximated_size": index_stats.approximated_size,
+                        "num_docs": index_stats.num_docs,
+                        "accessed": index_stats.accessed,
+                        "added": index_stats.added,
+                        "updated": index_stats.updated,
+                        "deleted": index_stats.deleted,
+                        "merged": index_stats.merged,
+                        "accessed_at": index_stats.accessed_at,
+                        "added_at": index_stats.added_at,
+                        "updated_at": index_stats.updated_at,
+                        "deleted_at": index_stats.deleted_at,
+                        "merged_at": index_stats.merged_at,
+                    },
+                }
+            ],
+        }
 
     def empty(self, collection, query, dtypes=None) -> bool:
         df = self.find(collection, query, dtypes=dtypes, limit=1)
 
         return len(df) == 0
 
     def _invoke(self, func, *args, **kwargs):
```

### Comparing `cognica-0.1.3/src/cognica/fts_analysis_pipeline.py` & `cognica-0.1.4/src/cognica/fts_analysis_pipeline.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/key_value_db.py` & `cognica-0.1.4/src/cognica/key_value_db.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/protobuf/document_db_pb2.py` & `cognica-0.1.4/src/cognica/protobuf/document_db_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,94 +10,96 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import cognica.protobuf.document_pb2 as document__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x64ocument_db.proto\x12\x17\x63ognica.rpc.db.document\x1a\x0e\x64ocument.proto\"\xf3\x01\n\tIndexDesc\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x03(\t\x12\x0e\n\x06unique\x18\x04 \x01(\x08\x12\x36\n\nindex_type\x18\x05 \x01(\x0e\x32\".cognica.rpc.db.document.IndexType\x12\x34\n\x06status\x18\x07 \x01(\x0e\x32$.cognica.rpc.db.document.IndexStatus\x12\x32\n\x07options\x18\x08 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\x9e\x01\n\x0e\x43ollectionInfo\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x37\n\x0bprimary_key\x18\x02 \x01(\x0b\x32\".cognica.rpc.db.document.IndexDesc\x12:\n\x0esecondary_keys\x18\x03 \x03(\x0b\x32\".cognica.rpc.db.document.IndexDesc\"\x7f\n\x0bProfileInfo\x12\x0f\n\x07matched\x18\x01 \x01(\x04\x12\x0f\n\x07scanned\x18\x02 \x01(\x04\x12\x10\n\x08\x66iltered\x18\x03 \x01(\x04\x12\x19\n\x11query_duration_us\x18\x04 \x01(\x04\x12!\n\x19serialization_duration_us\x18\x05 \x01(\x04\"V\n\x17\x43reateCollectionRequest\x12;\n\ncollection\x18\x01 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\"r\n\x18\x43reateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"0\n\x15\x44ropCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"p\n\x16\x44ropCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"/\n\x14GetCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"\xac\x01\n\x15GetCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12;\n\ncollection\x18\x03 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"e\n\x12\x43reateIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x36\n\nindex_desc\x18\x02 \x01(\x0b\x32\".cognica.rpc.db.document.IndexDesc\"m\n\x13\x43reateIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"?\n\x10\x44ropIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"k\n\x11\x44ropIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\">\n\x0fGetIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\xbb\x01\n\x10GetIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x36\n\nindex_desc\x18\x04 \x01(\x0b\x32\".cognica.rpc.db.document.IndexDesc\x12\x35\n\x07profile\x18\x05 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"R\n\x05Query\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x30\n\x05query\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\xe4\x01\n\x0b\x46indRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\x15\n\rindex_columns\x18\x03 \x03(\t\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12@\n\x06\x64types\x18\x05 \x03(\x0b\x32\x30.cognica.rpc.db.document.FindRequest.DtypesEntry\x1a-\n\x0b\x44typesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"|\n\x0c\x46indResponse\x12\x13\n\x0bnum_columns\x18\x01 \x01(\x05\x12\x10\n\x08num_rows\x18\x02 \x01(\x05\x12\x0e\n\x06\x62uffer\x18\x03 \x01(\x0c\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"J\n\x10\x46indBatchRequest\x12\x36\n\x08requests\x18\x01 \x03(\x0b\x32$.cognica.rpc.db.document.FindRequest\"M\n\x11\x46indBatchResponse\x12\x38\n\tresponses\x18\x01 \x03(\x0b\x32%.cognica.rpc.db.document.FindResponse\"=\n\x0c\x43ountRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"v\n\rCountResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x03\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"@\n\x0f\x43ontainsRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"y\n\x10\x43ontainsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x66ound\x18\x03 \x01(\x08\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rInsertRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eInsertResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x8f\x01\n\rUpdateRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x06\x66ilter\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\x12\x32\n\x07updates\x18\x03 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"h\n\x0eUpdateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rRemoveRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eRemoveResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"4\n\x19TruncateCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"t\n\x1aTruncateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x18\n\x16ListCollectionsRequest\"\x8b\x01\n\x17ListCollectionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo*e\n\tIndexType\x12\x0f\n\x0bkPrimaryKey\x10\x00\x12\x11\n\rkSecondaryKey\x10\x01\x12\x1a\n\x16kClusteredSecondaryKey\x10\x02\x12\x18\n\x14kFullTextSearchIndex\x10\x03*\x8d\x01\n\x0bIndexStatus\x12\x0c\n\x08kEnabled\x10\x00\x12\r\n\tkDisabled\x10\x01\x12\x0f\n\x0bkReadyToUse\x10\x02\x12\x14\n\x10kBuildInProgress\x10\x03\x12\x12\n\x0ekBuildFinished\x10\x04\x12\x13\n\x0fkDropInProgress\x10\x05\x12\x11\n\rkDropFinished\x10\x06\x32\xbe\x0c\n\x11\x44ocumentDBService\x12U\n\x04\x66ind\x12$.cognica.rpc.db.document.FindRequest\x1a%.cognica.rpc.db.document.FindResponse\"\x00\x12\x65\n\nfind_batch\x12).cognica.rpc.db.document.FindBatchRequest\x1a*.cognica.rpc.db.document.FindBatchResponse\"\x00\x12X\n\x05\x63ount\x12%.cognica.rpc.db.document.CountRequest\x1a&.cognica.rpc.db.document.CountResponse\"\x00\x12\x61\n\x08\x63ontains\x12(.cognica.rpc.db.document.ContainsRequest\x1a).cognica.rpc.db.document.ContainsResponse\"\x00\x12[\n\x06insert\x12&.cognica.rpc.db.document.InsertRequest\x1a\'.cognica.rpc.db.document.InsertResponse\"\x00\x12[\n\x06update\x12&.cognica.rpc.db.document.UpdateRequest\x1a\'.cognica.rpc.db.document.UpdateResponse\"\x00\x12[\n\x06remove\x12&.cognica.rpc.db.document.RemoveRequest\x1a\'.cognica.rpc.db.document.RemoveResponse\"\x00\x12z\n\x11\x63reate_collection\x12\x30.cognica.rpc.db.document.CreateCollectionRequest\x1a\x31.cognica.rpc.db.document.CreateCollectionResponse\"\x00\x12t\n\x0f\x64rop_collection\x12..cognica.rpc.db.document.DropCollectionRequest\x1a/.cognica.rpc.db.document.DropCollectionResponse\"\x00\x12q\n\x0eget_collection\x12-.cognica.rpc.db.document.GetCollectionRequest\x1a..cognica.rpc.db.document.GetCollectionResponse\"\x00\x12w\n\x10list_collections\x12/.cognica.rpc.db.document.ListCollectionsRequest\x1a\x30.cognica.rpc.db.document.ListCollectionsResponse\"\x00\x12\x80\x01\n\x13truncate_collection\x12\x32.cognica.rpc.db.document.TruncateCollectionRequest\x1a\x33.cognica.rpc.db.document.TruncateCollectionResponse\"\x00\x12k\n\x0c\x63reate_index\x12+.cognica.rpc.db.document.CreateIndexRequest\x1a,.cognica.rpc.db.document.CreateIndexResponse\"\x00\x12\x65\n\ndrop_index\x12).cognica.rpc.db.document.DropIndexRequest\x1a*.cognica.rpc.db.document.DropIndexResponse\"\x00\x12\x62\n\tget_index\x12(.cognica.rpc.db.document.GetIndexRequest\x1a).cognica.rpc.db.document.GetIndexResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x64ocument_db.proto\x12\x17\x63ognica.rpc.db.document\x1a\x0e\x64ocument.proto\"\xf9\x01\n\x0fIndexDescriptor\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x03(\t\x12\x0e\n\x06unique\x18\x04 \x01(\x08\x12\x36\n\nindex_type\x18\x05 \x01(\x0e\x32\".cognica.rpc.db.document.IndexType\x12\x34\n\x06status\x18\x06 \x01(\x0e\x32$.cognica.rpc.db.document.IndexStatus\x12\x32\n\x07options\x18\x07 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\x94\x02\n\nIndexStats\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x19\n\x11\x61pproximated_size\x18\x03 \x01(\x04\x12\x10\n\x08num_docs\x18\x04 \x01(\x04\x12\x10\n\x08\x61\x63\x63\x65ssed\x18\x05 \x01(\x04\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x06 \x01(\x04\x12\x0f\n\x07updated\x18\x07 \x01(\x04\x12\x0f\n\x07\x64\x65leted\x18\x08 \x01(\x04\x12\x0e\n\x06merged\x18\t \x01(\x04\x12\x13\n\x0b\x61\x63\x63\x65ssed_at\x18\n \x01(\x03\x12\x10\n\x08\x61\x64\x64\x65\x64_at\x18\x0b \x01(\x03\x12\x12\n\nupdated_at\x18\x0c \x01(\x03\x12\x12\n\ndeleted_at\x18\r \x01(\x03\x12\x11\n\tmerged_at\x18\x0e \x01(\x03\"\xa8\x01\n\x0e\x43ollectionInfo\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x43\n\x11index_descriptors\x18\x02 \x03(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\x12\x38\n\x0bindex_stats\x18\x03 \x03(\x0b\x32#.cognica.rpc.db.document.IndexStats\"\x7f\n\x0bProfileInfo\x12\x0f\n\x07matched\x18\x01 \x01(\x04\x12\x0f\n\x07scanned\x18\x02 \x01(\x04\x12\x10\n\x08\x66iltered\x18\x03 \x01(\x04\x12\x19\n\x11query_duration_us\x18\x04 \x01(\x04\x12!\n\x19serialization_duration_us\x18\x05 \x01(\x04\"V\n\x17\x43reateCollectionRequest\x12;\n\ncollection\x18\x01 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\"r\n\x18\x43reateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"0\n\x15\x44ropCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"p\n\x16\x44ropCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"/\n\x14GetCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"\xac\x01\n\x15GetCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12;\n\ncollection\x18\x03 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"k\n\x12\x43reateIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12<\n\nindex_desc\x18\x02 \x01(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\"m\n\x13\x43reateIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"?\n\x10\x44ropIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"k\n\x11\x44ropIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\">\n\x0fGetIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\xfb\x01\n\x10GetIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12<\n\nindex_desc\x18\x04 \x01(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\x12\x38\n\x0bindex_stats\x18\x05 \x01(\x0b\x32#.cognica.rpc.db.document.IndexStats\x12\x35\n\x07profile\x18\x06 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"R\n\x05Query\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x30\n\x05query\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\xe4\x01\n\x0b\x46indRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\x15\n\rindex_columns\x18\x03 \x03(\t\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12@\n\x06\x64types\x18\x05 \x03(\x0b\x32\x30.cognica.rpc.db.document.FindRequest.DtypesEntry\x1a-\n\x0b\x44typesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"|\n\x0c\x46indResponse\x12\x13\n\x0bnum_columns\x18\x01 \x01(\x05\x12\x10\n\x08num_rows\x18\x02 \x01(\x05\x12\x0e\n\x06\x62uffer\x18\x03 \x01(\x0c\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"J\n\x10\x46indBatchRequest\x12\x36\n\x08requests\x18\x01 \x03(\x0b\x32$.cognica.rpc.db.document.FindRequest\"M\n\x11\x46indBatchResponse\x12\x38\n\tresponses\x18\x01 \x03(\x0b\x32%.cognica.rpc.db.document.FindResponse\"=\n\x0c\x43ountRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"v\n\rCountResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x03\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"@\n\x0f\x43ontainsRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"y\n\x10\x43ontainsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x66ound\x18\x03 \x01(\x08\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rInsertRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eInsertResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x8f\x01\n\rUpdateRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x06\x66ilter\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\x12\x32\n\x07updates\x18\x03 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"h\n\x0eUpdateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rRemoveRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eRemoveResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"4\n\x19TruncateCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"t\n\x1aTruncateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x18\n\x16ListCollectionsRequest\"\x8b\x01\n\x17ListCollectionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo*e\n\tIndexType\x12\x0f\n\x0bkPrimaryKey\x10\x00\x12\x11\n\rkSecondaryKey\x10\x01\x12\x1a\n\x16kClusteredSecondaryKey\x10\x02\x12\x18\n\x14kFullTextSearchIndex\x10\x03*\x8d\x01\n\x0bIndexStatus\x12\x0c\n\x08kEnabled\x10\x00\x12\r\n\tkDisabled\x10\x01\x12\x0f\n\x0bkReadyToUse\x10\x02\x12\x14\n\x10kBuildInProgress\x10\x03\x12\x12\n\x0ekBuildFinished\x10\x04\x12\x13\n\x0fkDropInProgress\x10\x05\x12\x11\n\rkDropFinished\x10\x06\x32\xbe\x0c\n\x11\x44ocumentDBService\x12U\n\x04\x66ind\x12$.cognica.rpc.db.document.FindRequest\x1a%.cognica.rpc.db.document.FindResponse\"\x00\x12\x65\n\nfind_batch\x12).cognica.rpc.db.document.FindBatchRequest\x1a*.cognica.rpc.db.document.FindBatchResponse\"\x00\x12X\n\x05\x63ount\x12%.cognica.rpc.db.document.CountRequest\x1a&.cognica.rpc.db.document.CountResponse\"\x00\x12\x61\n\x08\x63ontains\x12(.cognica.rpc.db.document.ContainsRequest\x1a).cognica.rpc.db.document.ContainsResponse\"\x00\x12[\n\x06insert\x12&.cognica.rpc.db.document.InsertRequest\x1a\'.cognica.rpc.db.document.InsertResponse\"\x00\x12[\n\x06update\x12&.cognica.rpc.db.document.UpdateRequest\x1a\'.cognica.rpc.db.document.UpdateResponse\"\x00\x12[\n\x06remove\x12&.cognica.rpc.db.document.RemoveRequest\x1a\'.cognica.rpc.db.document.RemoveResponse\"\x00\x12z\n\x11\x63reate_collection\x12\x30.cognica.rpc.db.document.CreateCollectionRequest\x1a\x31.cognica.rpc.db.document.CreateCollectionResponse\"\x00\x12t\n\x0f\x64rop_collection\x12..cognica.rpc.db.document.DropCollectionRequest\x1a/.cognica.rpc.db.document.DropCollectionResponse\"\x00\x12q\n\x0eget_collection\x12-.cognica.rpc.db.document.GetCollectionRequest\x1a..cognica.rpc.db.document.GetCollectionResponse\"\x00\x12w\n\x10list_collections\x12/.cognica.rpc.db.document.ListCollectionsRequest\x1a\x30.cognica.rpc.db.document.ListCollectionsResponse\"\x00\x12\x80\x01\n\x13truncate_collection\x12\x32.cognica.rpc.db.document.TruncateCollectionRequest\x1a\x33.cognica.rpc.db.document.TruncateCollectionResponse\"\x00\x12k\n\x0c\x63reate_index\x12+.cognica.rpc.db.document.CreateIndexRequest\x1a,.cognica.rpc.db.document.CreateIndexResponse\"\x00\x12\x65\n\ndrop_index\x12).cognica.rpc.db.document.DropIndexRequest\x1a*.cognica.rpc.db.document.DropIndexResponse\"\x00\x12\x62\n\tget_index\x12(.cognica.rpc.db.document.GetIndexRequest\x1a).cognica.rpc.db.document.GetIndexResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'document_db_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\370\001\001'
   _FINDREQUEST_DTYPESENTRY._options = None
   _FINDREQUEST_DTYPESENTRY._serialized_options = b'8\001'
-  _INDEXTYPE._serialized_start=3738
-  _INDEXTYPE._serialized_end=3839
-  _INDEXSTATUS._serialized_start=3842
-  _INDEXSTATUS._serialized_end=3983
-  _INDEXDESC._serialized_start=63
-  _INDEXDESC._serialized_end=306
-  _COLLECTIONINFO._serialized_start=309
-  _COLLECTIONINFO._serialized_end=467
-  _PROFILEINFO._serialized_start=469
-  _PROFILEINFO._serialized_end=596
-  _CREATECOLLECTIONREQUEST._serialized_start=598
-  _CREATECOLLECTIONREQUEST._serialized_end=684
-  _CREATECOLLECTIONRESPONSE._serialized_start=686
-  _CREATECOLLECTIONRESPONSE._serialized_end=800
-  _DROPCOLLECTIONREQUEST._serialized_start=802
-  _DROPCOLLECTIONREQUEST._serialized_end=850
-  _DROPCOLLECTIONRESPONSE._serialized_start=852
-  _DROPCOLLECTIONRESPONSE._serialized_end=964
-  _GETCOLLECTIONREQUEST._serialized_start=966
-  _GETCOLLECTIONREQUEST._serialized_end=1013
-  _GETCOLLECTIONRESPONSE._serialized_start=1016
-  _GETCOLLECTIONRESPONSE._serialized_end=1188
-  _CREATEINDEXREQUEST._serialized_start=1190
-  _CREATEINDEXREQUEST._serialized_end=1291
-  _CREATEINDEXRESPONSE._serialized_start=1293
-  _CREATEINDEXRESPONSE._serialized_end=1402
-  _DROPINDEXREQUEST._serialized_start=1404
-  _DROPINDEXREQUEST._serialized_end=1467
-  _DROPINDEXRESPONSE._serialized_start=1469
-  _DROPINDEXRESPONSE._serialized_end=1576
-  _GETINDEXREQUEST._serialized_start=1578
-  _GETINDEXREQUEST._serialized_end=1640
-  _GETINDEXRESPONSE._serialized_start=1643
-  _GETINDEXRESPONSE._serialized_end=1830
-  _QUERY._serialized_start=1832
-  _QUERY._serialized_end=1914
-  _FINDREQUEST._serialized_start=1917
-  _FINDREQUEST._serialized_end=2145
-  _FINDREQUEST_DTYPESENTRY._serialized_start=2100
-  _FINDREQUEST_DTYPESENTRY._serialized_end=2145
-  _FINDRESPONSE._serialized_start=2147
-  _FINDRESPONSE._serialized_end=2271
-  _FINDBATCHREQUEST._serialized_start=2273
-  _FINDBATCHREQUEST._serialized_end=2347
-  _FINDBATCHRESPONSE._serialized_start=2349
-  _FINDBATCHRESPONSE._serialized_end=2426
-  _COUNTREQUEST._serialized_start=2428
-  _COUNTREQUEST._serialized_end=2489
-  _COUNTRESPONSE._serialized_start=2491
-  _COUNTRESPONSE._serialized_end=2609
-  _CONTAINSREQUEST._serialized_start=2611
-  _CONTAINSREQUEST._serialized_end=2675
-  _CONTAINSRESPONSE._serialized_start=2677
-  _CONTAINSRESPONSE._serialized_end=2798
-  _INSERTREQUEST._serialized_start=2800
-  _INSERTREQUEST._serialized_end=2865
-  _INSERTRESPONSE._serialized_start=2867
-  _INSERTRESPONSE._serialized_end=2971
-  _UPDATEREQUEST._serialized_start=2974
-  _UPDATEREQUEST._serialized_end=3117
-  _UPDATERESPONSE._serialized_start=3119
-  _UPDATERESPONSE._serialized_end=3223
-  _REMOVEREQUEST._serialized_start=3225
-  _REMOVEREQUEST._serialized_end=3290
-  _REMOVERESPONSE._serialized_start=3292
-  _REMOVERESPONSE._serialized_end=3396
-  _TRUNCATECOLLECTIONREQUEST._serialized_start=3398
-  _TRUNCATECOLLECTIONREQUEST._serialized_end=3450
-  _TRUNCATECOLLECTIONRESPONSE._serialized_start=3452
-  _TRUNCATECOLLECTIONRESPONSE._serialized_end=3568
-  _LISTCOLLECTIONSREQUEST._serialized_start=3570
-  _LISTCOLLECTIONSREQUEST._serialized_end=3594
-  _LISTCOLLECTIONSRESPONSE._serialized_start=3597
-  _LISTCOLLECTIONSRESPONSE._serialized_end=3736
-  _DOCUMENTDBSERVICE._serialized_start=3986
-  _DOCUMENTDBSERVICE._serialized_end=5584
+  _INDEXTYPE._serialized_start=4103
+  _INDEXTYPE._serialized_end=4204
+  _INDEXSTATUS._serialized_start=4207
+  _INDEXSTATUS._serialized_end=4348
+  _INDEXDESCRIPTOR._serialized_start=63
+  _INDEXDESCRIPTOR._serialized_end=312
+  _INDEXSTATS._serialized_start=315
+  _INDEXSTATS._serialized_end=591
+  _COLLECTIONINFO._serialized_start=594
+  _COLLECTIONINFO._serialized_end=762
+  _PROFILEINFO._serialized_start=764
+  _PROFILEINFO._serialized_end=891
+  _CREATECOLLECTIONREQUEST._serialized_start=893
+  _CREATECOLLECTIONREQUEST._serialized_end=979
+  _CREATECOLLECTIONRESPONSE._serialized_start=981
+  _CREATECOLLECTIONRESPONSE._serialized_end=1095
+  _DROPCOLLECTIONREQUEST._serialized_start=1097
+  _DROPCOLLECTIONREQUEST._serialized_end=1145
+  _DROPCOLLECTIONRESPONSE._serialized_start=1147
+  _DROPCOLLECTIONRESPONSE._serialized_end=1259
+  _GETCOLLECTIONREQUEST._serialized_start=1261
+  _GETCOLLECTIONREQUEST._serialized_end=1308
+  _GETCOLLECTIONRESPONSE._serialized_start=1311
+  _GETCOLLECTIONRESPONSE._serialized_end=1483
+  _CREATEINDEXREQUEST._serialized_start=1485
+  _CREATEINDEXREQUEST._serialized_end=1592
+  _CREATEINDEXRESPONSE._serialized_start=1594
+  _CREATEINDEXRESPONSE._serialized_end=1703
+  _DROPINDEXREQUEST._serialized_start=1705
+  _DROPINDEXREQUEST._serialized_end=1768
+  _DROPINDEXRESPONSE._serialized_start=1770
+  _DROPINDEXRESPONSE._serialized_end=1877
+  _GETINDEXREQUEST._serialized_start=1879
+  _GETINDEXREQUEST._serialized_end=1941
+  _GETINDEXRESPONSE._serialized_start=1944
+  _GETINDEXRESPONSE._serialized_end=2195
+  _QUERY._serialized_start=2197
+  _QUERY._serialized_end=2279
+  _FINDREQUEST._serialized_start=2282
+  _FINDREQUEST._serialized_end=2510
+  _FINDREQUEST_DTYPESENTRY._serialized_start=2465
+  _FINDREQUEST_DTYPESENTRY._serialized_end=2510
+  _FINDRESPONSE._serialized_start=2512
+  _FINDRESPONSE._serialized_end=2636
+  _FINDBATCHREQUEST._serialized_start=2638
+  _FINDBATCHREQUEST._serialized_end=2712
+  _FINDBATCHRESPONSE._serialized_start=2714
+  _FINDBATCHRESPONSE._serialized_end=2791
+  _COUNTREQUEST._serialized_start=2793
+  _COUNTREQUEST._serialized_end=2854
+  _COUNTRESPONSE._serialized_start=2856
+  _COUNTRESPONSE._serialized_end=2974
+  _CONTAINSREQUEST._serialized_start=2976
+  _CONTAINSREQUEST._serialized_end=3040
+  _CONTAINSRESPONSE._serialized_start=3042
+  _CONTAINSRESPONSE._serialized_end=3163
+  _INSERTREQUEST._serialized_start=3165
+  _INSERTREQUEST._serialized_end=3230
+  _INSERTRESPONSE._serialized_start=3232
+  _INSERTRESPONSE._serialized_end=3336
+  _UPDATEREQUEST._serialized_start=3339
+  _UPDATEREQUEST._serialized_end=3482
+  _UPDATERESPONSE._serialized_start=3484
+  _UPDATERESPONSE._serialized_end=3588
+  _REMOVEREQUEST._serialized_start=3590
+  _REMOVEREQUEST._serialized_end=3655
+  _REMOVERESPONSE._serialized_start=3657
+  _REMOVERESPONSE._serialized_end=3761
+  _TRUNCATECOLLECTIONREQUEST._serialized_start=3763
+  _TRUNCATECOLLECTIONREQUEST._serialized_end=3815
+  _TRUNCATECOLLECTIONRESPONSE._serialized_start=3817
+  _TRUNCATECOLLECTIONRESPONSE._serialized_end=3933
+  _LISTCOLLECTIONSREQUEST._serialized_start=3935
+  _LISTCOLLECTIONSREQUEST._serialized_end=3959
+  _LISTCOLLECTIONSRESPONSE._serialized_start=3962
+  _LISTCOLLECTIONSRESPONSE._serialized_end=4101
+  _DOCUMENTDBSERVICE._serialized_start=4351
+  _DOCUMENTDBSERVICE._serialized_end=5949
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cognica-0.1.3/src/cognica/protobuf/document_db_pb2_grpc.py` & `cognica-0.1.4/src/cognica/protobuf/document_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/protobuf/document_pb2.py` & `cognica-0.1.4/src/cognica/protobuf/document_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/protobuf/fts_analysis_pipeline_pb2.py` & `cognica-0.1.4/src/cognica/protobuf/fts_analysis_pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py` & `cognica-0.1.4/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/protobuf/key_value_db_pb2.py` & `cognica-0.1.4/src/cognica/protobuf/key_value_db_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/protobuf/key_value_db_pb2_grpc.py` & `cognica-0.1.4/src/cognica/protobuf/key_value_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/protobuf/sentence_transformer_pb2.py` & `cognica-0.1.4/src/cognica/protobuf/sentence_transformer_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/protobuf/sentence_transformer_pb2_grpc.py` & `cognica-0.1.4/src/cognica/protobuf/sentence_transformer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica/sentence_transformer.py` & `cognica-0.1.4/src/cognica/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.3/src/cognica.egg-info/PKG-INFO` & `cognica-0.1.4/src/cognica.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python client for Cognica database
-Home-page: https://github.com/cognicadb/cognica-python
-Author: Cognica, Inc.
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -213,21 +211,19 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: protobuf
 License-File: LICENSE
 
 # Cognica Python Client
 
 A Python client for Cognica database server.
```

### Comparing `cognica-0.1.3/src/cognica.egg-info/SOURCES.txt` & `cognica-0.1.4/src/cognica.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 src/cognica/__init__.py
 src/cognica/channel.py
 src/cognica/document_db.py
 src/cognica/fts_analysis_pipeline.py
 src/cognica/key_value_db.py
 src/cognica/sentence_transformer.py
 src/cognica.egg-info/PKG-INFO
```

