# Comparing `tmp/langchainplus_sdk-0.0.5.tar.gz` & `tmp/langchainplus_sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchainplus_sdk-0.0.5.tar", max compression
+gzip compressed data, was "langchainplus_sdk-0.0.6.tar", max compression
```

## Comparing `langchainplus_sdk-0.0.5.tar` & `langchainplus_sdk-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     8124 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/README.md
--rw-r--r--   0        0        0      529 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/cli/conf/nginx.conf
--rw-r--r--   0        0        0      315 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1198 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/cli/docker-compose.yaml
--rw-r--r--   0        0        0    12934 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/cli/main.py
--rw-r--r--   0        0        0    20044 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/client.py
--rw-r--r--   0        0        0      250 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/evaluation/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/evaluation/evaluator.py
--rw-r--r--   0        0        0     1545 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     7178 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/run_trees.py
--rw-r--r--   0        0        0     7001 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/schemas.py
--rw-r--r--   0        0        0     3235 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/utils.py
--rw-r--r--   0        0        0      879 2023-06-07 02:20:09.730435 langchainplus_sdk-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     8124 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/README.md
+-rw-r--r--   0        0        0      529 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      315 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1198 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    12934 2023-06-07 04:44:48.014877 langchainplus_sdk-0.0.6/langchainplus_sdk/cli/main.py
+-rw-r--r--   0        0        0    20044 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/client.py
+-rw-r--r--   0        0        0      250 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/evaluation/__init__.py
+-rw-r--r--   0        0        0     1419 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1545 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     7178 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/run_trees.py
+-rw-r--r--   0        0        0     7001 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/schemas.py
+-rw-r--r--   0        0        0     3235 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/langchainplus_sdk/utils.py
+-rw-r--r--   0        0        0      879 2023-06-07 04:44:48.018877 langchainplus_sdk-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.6/PKG-INFO
```

### Comparing `langchainplus_sdk-0.0.5/README.md` & `langchainplus_sdk-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.5/langchainplus_sdk/__init__.py` & `langchainplus_sdk-0.0.6/langchainplus_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.5/langchainplus_sdk/cli/docker-compose.yaml` & `langchainplus_sdk-0.0.6/langchainplus_sdk/cli/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.5/langchainplus_sdk/cli/main.py` & `langchainplus_sdk-0.0.6/langchainplus_sdk/cli/main.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.5/langchainplus_sdk/client.py` & `langchainplus_sdk-0.0.6/langchainplus_sdk/client.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.5/langchainplus_sdk/evaluation/evaluator.py` & `langchainplus_sdk-0.0.6/langchainplus_sdk/evaluation/evaluator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from abc import abstractmethod
 from typing import Dict, Optional, Union
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from langchainplus_sdk.schemas import SCORE_TYPE, VALUE_TYPE, Example, Run
 
 
 class EvaluationResult(BaseModel):
     """Evaluation result."""
 
     key: str
+    """The aspect, metric name, or label for this evaluation."""
     score: SCORE_TYPE = None
+    """The numeric score for this evaluation."""
     value: VALUE_TYPE = None
+    """The value for this evaluation, if not numeric."""
     comment: Optional[str] = None
+    """An explanation regarding the evaluation."""
     correction: Optional[Union[Dict, str]] = None
-    evaluator_info: Optional[Dict] = None
+    """What the correct value should be, if applicable."""
+    evaluator_info: Dict = Field(default_factory=dict)
+    """Additional information about the evaluator."""
 
     class Config:
         """Pydantic model configuration."""
 
         frozen = True
         allow_extra = False
```

### Comparing `langchainplus_sdk-0.0.5/langchainplus_sdk/evaluation/string_evaluator.py` & `langchainplus_sdk-0.0.6/langchainplus_sdk/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.5/langchainplus_sdk/run_trees.py` & `langchainplus_sdk-0.0.6/langchainplus_sdk/run_trees.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.5/langchainplus_sdk/schemas.py` & `langchainplus_sdk-0.0.6/langchainplus_sdk/schemas.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.5/langchainplus_sdk/utils.py` & `langchainplus_sdk-0.0.6/langchainplus_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.5/pyproject.toml` & `langchainplus_sdk-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchainplus-sdk"
-version = "0.0.5"
+version = "0.0.6"
 description = "Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langchainplus_sdk"}]
 
 [tool.poetry.scripts]
```

### Comparing `langchainplus_sdk-0.0.5/PKG-INFO` & `langchainplus_sdk-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchainplus-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

