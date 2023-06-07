# Comparing `tmp/poetry_grpc_plugin-0.1.6.tar.gz` & `tmp/poetry_grpc_plugin-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_grpc_plugin-0.1.6.tar", max compression
+gzip compressed data, was "poetry_grpc_plugin-0.1.7.tar", max compression
```

## Comparing `poetry_grpc_plugin-0.1.6.tar` & `poetry_grpc_plugin-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1062 2023-05-07 16:11:00.073133 poetry_grpc_plugin-0.1.6/LICENSE
--rw-r--r--   0        0        0     1293 2023-05-07 16:11:00.073133 poetry_grpc_plugin-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-05-07 16:11:00.073133 poetry_grpc_plugin-0.1.6/poetry_grpc_plugin/__init__.py
--rw-r--r--   0        0        0     7092 2023-05-07 16:11:00.073133 poetry_grpc_plugin-0.1.6/poetry_grpc_plugin/plugins.py
--rw-r--r--   0        0        0     1743 2023-05-07 16:11:00.073133 poetry_grpc_plugin-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 poetry_grpc_plugin-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-07 19:25:11.464928 poetry_grpc_plugin-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1293 2023-06-07 19:25:11.464928 poetry_grpc_plugin-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 19:25:11.464928 poetry_grpc_plugin-0.1.7/poetry_grpc_plugin/__init__.py
+-rw-r--r--   0        0        0     7092 2023-06-07 19:25:11.464928 poetry_grpc_plugin-0.1.7/poetry_grpc_plugin/plugins.py
+-rw-r--r--   0        0        0     1743 2023-06-07 19:25:11.464928 poetry_grpc_plugin-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2379 1970-01-01 00:00:00.000000 poetry_grpc_plugin-0.1.7/PKG-INFO
```

### Comparing `poetry_grpc_plugin-0.1.6/LICENSE` & `poetry_grpc_plugin-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_grpc_plugin-0.1.6/README.md` & `poetry_grpc_plugin-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `poetry_grpc_plugin-0.1.6/poetry_grpc_plugin/plugins.py` & `poetry_grpc_plugin-0.1.7/poetry_grpc_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_grpc_plugin-0.1.6/pyproject.toml` & `poetry_grpc_plugin-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-grpc-plugin"
-version = "0.1.6"
+version = "0.1.7"
 description = "gRPC Poetry plugin"
 authors = ["Federico Jaite <fede_654_87@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "poetry_grpc_plugin"}]
 repository = "https://github.com/fedej/poetry-grpc-plugin"
 classifiers = [
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Code Generators",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 grpcio-tools = "^1.39.0"
-poetry = ">=1.2.0,<1.5"
+poetry = ">=1.2.0,<1.6"
 mypy-protobuf = ">=2.9,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.11.5"
 flake8 = "^3.9.2"
 mypy = "^1.2.0"
```

### Comparing `poetry_grpc_plugin-0.1.6/PKG-INFO` & `poetry_grpc_plugin-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-grpc-plugin
-Version: 0.1.6
+Version: 0.1.7
 Summary: gRPC Poetry plugin
 Home-page: https://github.com/fedej/poetry-grpc-plugin
 License: MIT
 Author: Federico Jaite
 Author-email: fede_654_87@hotmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,21 +14,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Dist: grpcio-tools (>=1.39.0,<2.0.0)
 Requires-Dist: mypy-protobuf (>=2.9,<4.0)
-Requires-Dist: poetry (>=1.2.0,<1.5)
+Requires-Dist: poetry (>=1.2.0,<1.6)
 Project-URL: Repository, https://github.com/fedej/poetry-grpc-plugin
 Description-Content-Type: text/markdown
 
 # Poetry gRPC plugin
 
 A [**Poetry**](https://python-poetry.org/) plugin to run the Protocol Buffers compiler with gRPC support.
```

