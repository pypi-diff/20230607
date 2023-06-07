# Comparing `tmp/langchainplus_sdk-0.0.4.tar.gz` & `tmp/langchainplus_sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchainplus_sdk-0.0.4.tar", max compression
+gzip compressed data, was "langchainplus_sdk-0.0.5.tar", max compression
```

## Comparing `langchainplus_sdk-0.0.4.tar` & `langchainplus_sdk-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     8124 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/README.md
--rw-r--r--   0        0        0      529 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/cli/conf/nginx.conf
--rw-r--r--   0        0        0      315 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1198 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/cli/docker-compose.yaml
--rw-r--r--   0        0        0    12934 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/cli/main.py
--rw-r--r--   0        0        0    18507 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/client.py
--rw-r--r--   0        0        0      250 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/evaluation/__init__.py
--rw-r--r--   0        0        0      738 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/evaluation/evaluator.py
--rw-r--r--   0        0        0     1545 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     7178 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/run_trees.py
--rw-r--r--   0        0        0     7001 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/schemas.py
--rw-r--r--   0        0        0     3235 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/utils.py
--rw-r--r--   0        0        0      879 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     8124 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/README.md
+-rw-r--r--   0        0        0      529 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      315 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1198 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    12934 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/cli/main.py
+-rw-r--r--   0        0        0    20044 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/client.py
+-rw-r--r--   0        0        0      250 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/evaluation/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1545 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     7178 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/run_trees.py
+-rw-r--r--   0        0        0     7001 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/schemas.py
+-rw-r--r--   0        0        0     3235 2023-06-07 02:20:09.726435 langchainplus_sdk-0.0.5/langchainplus_sdk/utils.py
+-rw-r--r--   0        0        0      879 2023-06-07 02:20:09.730435 langchainplus_sdk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.5/PKG-INFO
```

### Comparing `langchainplus_sdk-0.0.4/README.md` & `langchainplus_sdk-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.4/langchainplus_sdk/__init__.py` & `langchainplus_sdk-0.0.5/langchainplus_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.4/langchainplus_sdk/cli/docker-compose.yaml` & `langchainplus_sdk-0.0.5/langchainplus_sdk/cli/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.4/langchainplus_sdk/cli/main.py` & `langchainplus_sdk-0.0.5/langchainplus_sdk/cli/main.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.4/langchainplus_sdk/client.py` & `langchainplus_sdk-0.0.5/langchainplus_sdk/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -420,14 +420,16 @@
         raise_for_status_with_text(response)
         return Example(**response.json())
 
     def evaluate_run(
         self,
         run: Union[Run, str, UUID],
         evaluator: RunEvaluator,
+        *,
+        source_info: Optional[Dict[str, Any]] = None,
     ) -> Feedback:
         """Evaluate a run."""
         if isinstance(run, (str, UUID)):
             run_ = self.read_run(run)
         elif isinstance(run, Run):
             run_ = run
         else:
@@ -436,21 +438,61 @@
             reference_example = self.read_example(run_.reference_example_id)
         else:
             reference_example = None
         feedback_result = evaluator.evaluate_run(
             run_,
             example=reference_example,
         )
+        source_info = source_info or {}
+        if feedback_result.evaluator_info:
+            source_info = {**feedback_result.evaluator_info, **source_info}
         return self.create_feedback(
             run_.id,
             feedback_result.key,
             score=feedback_result.score,
             value=feedback_result.value,
             comment=feedback_result.comment,
             correction=feedback_result.correction,
+            source_info=source_info,
+            feedback_source_type=FeedbackSourceType.MODEL,
+        )
+
+    async def aevaluate_run(
+        self,
+        run: Union[Run, str, UUID],
+        evaluator: RunEvaluator,
+        *,
+        source_info: Optional[Dict[str, Any]] = None,
+    ) -> Feedback:
+        """Evaluate a run."""
+        if isinstance(run, (str, UUID)):
+            run_ = self.read_run(run)
+        elif isinstance(run, Run):
+            run_ = run
+        else:
+            raise TypeError(f"Invalid run type: {type(run)}")
+        if run_.reference_example_id is not None:
+            reference_example = self.read_example(run_.reference_example_id)
+        else:
+            reference_example = None
+        feedback_result = await evaluator.aevaluate_run(
+            run_,
+            example=reference_example,
+        )
+        source_info = source_info or {}
+        if feedback_result.evaluator_info:
+            source_info = {**feedback_result.evaluator_info, **source_info}
+        return self.create_feedback(
+            run_.id,
+            feedback_result.key,
+            score=feedback_result.score,
+            value=feedback_result.value,
+            comment=feedback_result.comment,
+            correction=feedback_result.correction,
+            source_info=source_info,
             feedback_source_type=FeedbackSourceType.MODEL,
         )
 
     def create_feedback(
         self,
         run_id: ID_TYPE,
         key: str,
```

### Comparing `langchainplus_sdk-0.0.4/langchainplus_sdk/evaluation/string_evaluator.py` & `langchainplus_sdk-0.0.5/langchainplus_sdk/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.4/langchainplus_sdk/run_trees.py` & `langchainplus_sdk-0.0.5/langchainplus_sdk/run_trees.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.4/langchainplus_sdk/schemas.py` & `langchainplus_sdk-0.0.5/langchainplus_sdk/schemas.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.4/langchainplus_sdk/utils.py` & `langchainplus_sdk-0.0.5/langchainplus_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.4/pyproject.toml` & `langchainplus_sdk-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchainplus-sdk"
-version = "0.0.4"
+version = "0.0.5"
 description = "Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langchainplus_sdk"}]
 
 [tool.poetry.scripts]
```

### Comparing `langchainplus_sdk-0.0.4/PKG-INFO` & `langchainplus_sdk-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchainplus-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

