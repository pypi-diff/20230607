# Comparing `tmp/nlp_service-1.4.1.tar.gz` & `tmp/nlp_service-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp_service-1.4.1.tar", max compression
+gzip compressed data, was "nlp_service-1.4.2.tar", max compression
```

## Comparing `nlp_service-1.4.1.tar` & `nlp_service-1.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-05-23 20:47:25.026725 nlp_service-1.4.1/LICENSE
--rw-r--r--   0        0        0     8218 2023-05-23 20:47:25.030725 nlp_service-1.4.1/README.md
--rw-r--r--   0        0        0      226 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/__init__.py
--rw-r--r--   0        0        0       42 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/__main__.py
--rw-r--r--   0        0        0     2259 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/client.py
--rw-r--r--   0        0        0    10441 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/infersent.py
--rw-r--r--   0        0        0        0 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/py.typed
--rw-r--r--   0        0        0    15629 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/server.py
--rw-r--r--   0        0        0     9147 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/similarity.py
--rw-r--r--   0        0        0      344 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/typing.py
--rw-r--r--   0        0        0     1519 2023-05-23 20:47:56.247040 nlp_service-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     9983 1970-01-01 00:00:00.000000 nlp_service-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-07 09:11:27.174929 nlp_service-1.4.2/LICENSE
+-rw-r--r--   0        0        0     8218 2023-06-07 09:11:27.174929 nlp_service-1.4.2/README.md
+-rw-r--r--   0        0        0      226 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/__main__.py
+-rw-r--r--   0        0        0     2259 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/client.py
+-rw-r--r--   0        0        0    10441 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/infersent.py
+-rw-r--r--   0        0        0        0 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/py.typed
+-rw-r--r--   0        0        0    15668 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/server.py
+-rw-r--r--   0        0        0     9147 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/similarity.py
+-rw-r--r--   0        0        0      344 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/typing.py
+-rw-r--r--   0        0        0     1519 2023-06-07 09:11:51.930792 nlp_service-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     9983 1970-01-01 00:00:00.000000 nlp_service-1.4.2/PKG-INFO
```

### Comparing `nlp_service-1.4.1/LICENSE` & `nlp_service-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.1/README.md` & `nlp_service-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.1/nlp_service/client.py` & `nlp_service-1.4.2/nlp_service/client.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.1/nlp_service/infersent.py` & `nlp_service-1.4.2/nlp_service/infersent.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.1/nlp_service/server.py` & `nlp_service-1.4.2/nlp_service/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,17 +172,17 @@
         def vector(self, text: str) -> SpacyVector:
             embeddings = t.cast(
                 NumpyVector, self.model.encode([text], convert_to_numpy=True)
             )
 
             return embeddings[0]
 
-    embedding_map[
-        nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SENTENCE_TRANSFORMERS
-    ] = SentenceTransformersModel
+    embedding_map[nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SENTENCE_TRANSFORMERS] = (
+        SentenceTransformersModel
+    )
 
 except ModuleNotFoundError:
     log.info("'sentence-transformers' not installed.")
 
 
 try:
     import tensorflow_hub as hub
@@ -192,17 +192,17 @@
             self.model: t.Any = hub.load(model.model_name)
 
         def vector(self, text: str) -> SpacyVector:
             embeddings: t.Sequence[t.Any] = self.model([text])
 
             return embeddings[0].numpy()
 
-    embedding_map[
-        nlp_pb2.EmbeddingType.EMBEDDING_TYPE_TENSORFLOW_HUB
-    ] = TensorflowHubModel
+    embedding_map[nlp_pb2.EmbeddingType.EMBEDDING_TYPE_TENSORFLOW_HUB] = (
+        TensorflowHubModel
+    )
 
 except ModuleNotFoundError:
     log.info("'tensorflow-hub' not installed.")
 
 
 try:
     import openai
@@ -467,19 +467,20 @@
     nlp_pb2_grpc.add_NlpServiceServicer_to_server(NlpService(), server)
     # topic_modeling_pb2_grpc.add_TopicModelingServiceServicer_to_server(
     #     TopicModelingService(), server
     # )
 
 
 @app.command()
-def main(address: str = typer.Argument("127.0.0.1:50100")):
+def main(address: str = typer.Argument("127.0.0.1:50100"), threads: int = 1):
     """Main entry point for the server."""
 
     arg_services.serve(
         address,
         add_services,
         [arg_services.full_service_name(nlp_pb2, "NlpService")],
+        threads,
     )
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `nlp_service-1.4.1/nlp_service/similarity.py` & `nlp_service-1.4.2/nlp_service/similarity.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.1/pyproject.toml` & `nlp_service-1.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nlp-service"
-version = "1.4.1"
+version = "1.4.2"
 description = "Microservice for NLP tasks using gRPC"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/nlp-service"
 packages = [{ include = "nlp_service" }]
```

### Comparing `nlp_service-1.4.1/PKG-INFO` & `nlp_service-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-service
-Version: 1.4.1
+Version: 1.4.2
 Summary: Microservice for NLP tasks using gRPC
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

