# Comparing `tmp/nlp_service-1.4.2.tar.gz` & `tmp/nlp_service-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp_service-1.4.2.tar", max compression
+gzip compressed data, was "nlp_service-1.4.3.tar", max compression
```

## Comparing `nlp_service-1.4.2.tar` & `nlp_service-1.4.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-06-07 09:11:27.174929 nlp_service-1.4.2/LICENSE
--rw-r--r--   0        0        0     8218 2023-06-07 09:11:27.174929 nlp_service-1.4.2/README.md
--rw-r--r--   0        0        0      226 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/__init__.py
--rw-r--r--   0        0        0       42 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/__main__.py
--rw-r--r--   0        0        0     2259 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/client.py
--rw-r--r--   0        0        0    10441 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/infersent.py
--rw-r--r--   0        0        0        0 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/py.typed
--rw-r--r--   0        0        0    15668 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/server.py
--rw-r--r--   0        0        0     9147 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/similarity.py
--rw-r--r--   0        0        0      344 2023-06-07 09:11:27.174929 nlp_service-1.4.2/nlp_service/typing.py
--rw-r--r--   0        0        0     1519 2023-06-07 09:11:51.930792 nlp_service-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     9983 1970-01-01 00:00:00.000000 nlp_service-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-07 09:28:54.184637 nlp_service-1.4.3/LICENSE
+-rw-r--r--   0        0        0     8218 2023-06-07 09:28:54.184637 nlp_service-1.4.3/README.md
+-rw-r--r--   0        0        0      226 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/__main__.py
+-rw-r--r--   0        0        0     2259 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/client.py
+-rw-r--r--   0        0        0    10441 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/infersent.py
+-rw-r--r--   0        0        0        0 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/py.typed
+-rw-r--r--   0        0        0    15668 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/server.py
+-rw-r--r--   0        0        0     9147 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/similarity.py
+-rw-r--r--   0        0        0      344 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/typing.py
+-rw-r--r--   0        0        0     1519 2023-06-07 09:29:21.228982 nlp_service-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     9983 1970-01-01 00:00:00.000000 nlp_service-1.4.3/PKG-INFO
```

### Comparing `nlp_service-1.4.2/LICENSE` & `nlp_service-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.2/README.md` & `nlp_service-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.2/nlp_service/client.py` & `nlp_service-1.4.3/nlp_service/client.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.2/nlp_service/infersent.py` & `nlp_service-1.4.3/nlp_service/infersent.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.2/nlp_service/server.py` & `nlp_service-1.4.3/nlp_service/server.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.2/nlp_service/similarity.py` & `nlp_service-1.4.3/nlp_service/similarity.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.2/pyproject.toml` & `nlp_service-1.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nlp-service"
-version = "1.4.2"
+version = "1.4.3"
 description = "Microservice for NLP tasks using gRPC"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/nlp-service"
 packages = [{ include = "nlp_service" }]
@@ -25,15 +25,15 @@
 gensim = { version = "^4.3.1", optional = true }
 python-Levenshtein = { version = "^0.21.0", optional = true }
 sentence-transformers = { version = "^2.2.2", optional = true }
 torch = { version = ">=1.13.1, <3.0", optional = true }
 transformers = { version = "^4.29.2", optional = true }
 tensorflow = { version = "^2.12.0", optional = true }
 tensorflow-hub = { version = "^0.13.0", optional = true }
-openai = { version = "^0.27.7", optional = true }
+openai = { version = "^0.27.8", optional = true }
 
 [tool.poetry.extras]
 wmd = ["gensim"]
 levenshtein = ["python-Levenshtein"]
 sentence-transformers = ["sentence-transformers", "torch"]
 transformers = ["transformers", "torch"]
 tensorflow = ["tensorflow", "tensorflow-hub"]
```

### Comparing `nlp_service-1.4.2/PKG-INFO` & `nlp_service-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-service
-Version: 1.4.2
+Version: 1.4.3
 Summary: Microservice for NLP tasks using gRPC
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 Provides-Extra: wmd
 Requires-Dist: arg-services (>=1.3.1,<2.0.0)
 Requires-Dist: gensim (>=4.3.1,<5.0.0) ; extra == "wmd" or extra == "all"
 Requires-Dist: mashumaro (>=3.7,<4.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: nptyping (>=2.5.0,<3.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: openai (>=0.27.7,<0.28.0) ; extra == "openai" or extra == "all"
+Requires-Dist: openai (>=0.27.8,<0.28.0) ; extra == "openai" or extra == "all"
 Requires-Dist: python-Levenshtein (>=0.21.0,<0.22.0) ; extra == "levenshtein" or extra == "all"
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "sentence-transformers" or extra == "all"
 Requires-Dist: spacy (>=3.5.3,<4.0.0)
 Requires-Dist: tensorflow (>=2.12.0,<3.0.0) ; extra == "tensorflow" or extra == "all"
 Requires-Dist: tensorflow-hub (>=0.13.0,<0.14.0) ; extra == "tensorflow"
 Requires-Dist: torch (>=1.13.1,<3.0) ; extra == "sentence-transformers" or extra == "transformers" or extra == "all"
```

