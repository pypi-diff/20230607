# Comparing `tmp/cognica-0.1.4.tar.gz` & `tmp/cognica-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognica-0.1.4.tar", last modified: Wed Jun  7 03:53:32 2023, max compression
+gzip compressed data, was "cognica-0.1.5.tar", last modified: Wed Jun  7 10:52:30 2023, max compression
```

## Comparing `cognica-0.1.4.tar` & `cognica-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 03:53:32.509926 cognica-0.1.4/
--rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-29 03:56:50.000000 cognica-0.1.4/LICENSE
--rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-07 03:53:32.509735 cognica-0.1.4/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 05:58:03.000000 cognica-0.1.4/README.md
--rw-r--r--   0 jaepil     (501) staff       (20)     1282 2023-06-07 03:53:24.000000 cognica-0.1.4/pyproject.toml
--rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-06-07 03:53:32.509968 cognica-0.1.4/setup.cfg
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 03:53:32.503395 cognica-0.1.4/src/
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 03:53:32.505759 cognica-0.1.4/src/cognica/
--rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-15 08:05:25.000000 cognica-0.1.4/src/cognica/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-15 08:05:26.000000 cognica-0.1.4/src/cognica/channel.py
--rw-r--r--   0 jaepil     (501) staff       (20)    17045 2023-06-07 03:42:37.000000 cognica-0.1.4/src/cognica/document_db.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 03:46:32.000000 cognica-0.1.4/src/cognica/fts_analysis_pipeline.py
--rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 03:46:59.000000 cognica-0.1.4/src/cognica/key_value_db.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 03:53:32.509345 cognica-0.1.4/src/cognica/protobuf/
--rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-15 08:05:26.000000 cognica-0.1.4/src/cognica/protobuf/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)    13536 2023-06-07 03:42:37.000000 cognica-0.1.4/src/cognica/protobuf/document_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-06-03 01:34:57.000000 cognica-0.1.4/src/cognica/protobuf/document_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-06-03 01:33:38.000000 cognica-0.1.4/src/cognica/protobuf/document_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2669 2023-06-03 01:33:38.000000 cognica-0.1.4/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-06-03 01:35:26.000000 cognica-0.1.4/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     7337 2023-06-03 01:33:38.000000 cognica-0.1.4/src/cognica/protobuf/key_value_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-06-03 01:35:45.000000 cognica-0.1.4/src/cognica/protobuf/key_value_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     6085 2023-06-03 01:33:38.000000 cognica-0.1.4/src/cognica/protobuf/sentence_transformer_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-06-03 01:36:10.000000 cognica-0.1.4/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 03:47:19.000000 cognica-0.1.4/src/cognica/sentence_transformer.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 03:53:32.506587 cognica-0.1.4/src/cognica.egg-info/
--rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-07 03:53:32.000000 cognica-0.1.4/src/cognica.egg-info/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)      831 2023-06-07 03:53:32.000000 cognica-0.1.4/src/cognica.egg-info/SOURCES.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-06-07 03:53:32.000000 cognica-0.1.4/src/cognica.egg-info/dependency_links.txt
--rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-06-07 03:53:32.000000 cognica-0.1.4/src/cognica.egg-info/requires.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-06-07 03:53:32.000000 cognica-0.1.4/src/cognica.egg-info/top_level.txt
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 10:52:30.312876 cognica-0.1.5/
+-rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-29 03:56:50.000000 cognica-0.1.5/LICENSE
+-rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-07 10:52:30.312696 cognica-0.1.5/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 05:58:03.000000 cognica-0.1.5/README.md
+-rw-r--r--   0 jaepil     (501) staff       (20)     1282 2023-06-07 10:52:14.000000 cognica-0.1.5/pyproject.toml
+-rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-06-07 10:52:30.312929 cognica-0.1.5/setup.cfg
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 10:52:30.309246 cognica-0.1.5/src/
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 10:52:30.310431 cognica-0.1.5/src/cognica/
+-rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-15 08:05:25.000000 cognica-0.1.5/src/cognica/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-15 08:05:26.000000 cognica-0.1.5/src/cognica/channel.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    17063 2023-06-07 10:50:53.000000 cognica-0.1.5/src/cognica/document_db.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 03:46:32.000000 cognica-0.1.5/src/cognica/fts_analysis_pipeline.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 03:46:59.000000 cognica-0.1.5/src/cognica/key_value_db.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 10:52:30.312494 cognica-0.1.5/src/cognica/protobuf/
+-rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-15 08:05:26.000000 cognica-0.1.5/src/cognica/protobuf/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    13536 2023-06-07 03:42:37.000000 cognica-0.1.5/src/cognica/protobuf/document_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-06-03 01:34:57.000000 cognica-0.1.5/src/cognica/protobuf/document_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-06-03 01:33:38.000000 cognica-0.1.5/src/cognica/protobuf/document_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2669 2023-06-03 01:33:38.000000 cognica-0.1.5/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-06-03 01:35:26.000000 cognica-0.1.5/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     7337 2023-06-03 01:33:38.000000 cognica-0.1.5/src/cognica/protobuf/key_value_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-06-03 01:35:45.000000 cognica-0.1.5/src/cognica/protobuf/key_value_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     6085 2023-06-03 01:33:38.000000 cognica-0.1.5/src/cognica/protobuf/sentence_transformer_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-06-03 01:36:10.000000 cognica-0.1.5/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 03:47:19.000000 cognica-0.1.5/src/cognica/sentence_transformer.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 10:52:30.311070 cognica-0.1.5/src/cognica.egg-info/
+-rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-07 10:52:30.000000 cognica-0.1.5/src/cognica.egg-info/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)      831 2023-06-07 10:52:30.000000 cognica-0.1.5/src/cognica.egg-info/SOURCES.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-06-07 10:52:30.000000 cognica-0.1.5/src/cognica.egg-info/dependency_links.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-06-07 10:52:30.000000 cognica-0.1.5/src/cognica.egg-info/requires.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-06-07 10:52:30.000000 cognica-0.1.5/src/cognica.egg-info/top_level.txt
```

### Comparing `cognica-0.1.4/LICENSE` & `cognica-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/PKG-INFO` & `cognica-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python client for Cognica database
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cognica-0.1.4/README.md` & `cognica-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/pyproject.toml` & `cognica-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cognica"
-version = "0.1.4"
+version = "0.1.5"
 authors = [{ name = "Cognica, Inc.", email = "jaepil@cognica.io" }]
 description = "Python client for Cognica database"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
   "pandas>=1.5.3",
```

### Comparing `cognica-0.1.4/src/cognica/__init__.py` & `cognica-0.1.5/src/cognica/__init__.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/channel.py` & `cognica-0.1.5/src/cognica/channel.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/document_db.py` & `cognica-0.1.5/src/cognica/document_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 messages: t.TypeAlias = document_db_pb2  # type: ignore
 
 DocumentDBServiceStub = document_db_pb2_grpc.DocumentDBServiceStub
 
 IndexType: t.TypeAlias = messages.IndexType  # type: ignore
 IndexStatus: t.TypeAlias = messages.IndexStatus  # type: ignore
-IndexDesc: t.TypeAlias = messages.IndexDesc  # type: ignore
+IndexDescriptor: t.TypeAlias = messages.IndexDescriptor  # type: ignore
 CreateIndexRequest: t.TypeAlias = messages.CreateIndexRequest  # type: ignore
 CreateIndexResponse: t.TypeAlias = messages.CreateIndexResponse  # type: ignore
 DropIndexRequest: t.TypeAlias = messages.DropIndexRequest  # type: ignore
 DropIndexResponse: t.TypeAlias = messages.DropIndexResponse  # type: ignore
 GetIndexRequest: t.TypeAlias = messages.GetIndexRequest  # type: ignore
 GetIndexResponse: t.TypeAlias = messages.GetIndexResponse  # type: ignore
 
@@ -353,15 +353,15 @@
 
     def create_index(
         self, collection, index_name, fields, unique, index_type, options
     ) -> None:
         if options is not None:
             options = _to_json(options)
 
-        index_desc = IndexDesc(
+        index_desc = IndexDescriptor(
             index_id=0,
             index_name=index_name,
             fields=fields,
             unique=unique,
             index_type=index_type,
             status=IndexStatus.kEnabled,
             options=options,
```

### Comparing `cognica-0.1.4/src/cognica/fts_analysis_pipeline.py` & `cognica-0.1.5/src/cognica/fts_analysis_pipeline.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/key_value_db.py` & `cognica-0.1.5/src/cognica/key_value_db.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/protobuf/document_db_pb2.py` & `cognica-0.1.5/src/cognica/protobuf/document_db_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/protobuf/document_db_pb2_grpc.py` & `cognica-0.1.5/src/cognica/protobuf/document_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/protobuf/document_pb2.py` & `cognica-0.1.5/src/cognica/protobuf/document_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/protobuf/fts_analysis_pipeline_pb2.py` & `cognica-0.1.5/src/cognica/protobuf/fts_analysis_pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py` & `cognica-0.1.5/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/protobuf/key_value_db_pb2.py` & `cognica-0.1.5/src/cognica/protobuf/key_value_db_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/protobuf/key_value_db_pb2_grpc.py` & `cognica-0.1.5/src/cognica/protobuf/key_value_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/protobuf/sentence_transformer_pb2.py` & `cognica-0.1.5/src/cognica/protobuf/sentence_transformer_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/protobuf/sentence_transformer_pb2_grpc.py` & `cognica-0.1.5/src/cognica/protobuf/sentence_transformer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica/sentence_transformer.py` & `cognica-0.1.5/src/cognica/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.4/src/cognica.egg-info/PKG-INFO` & `cognica-0.1.5/src/cognica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python client for Cognica database
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cognica-0.1.4/src/cognica.egg-info/SOURCES.txt` & `cognica-0.1.5/src/cognica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

