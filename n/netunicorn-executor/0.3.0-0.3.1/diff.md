# Comparing `tmp/netunicorn-executor-0.3.0.tar.gz` & `tmp/netunicorn-executor-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/netunicorn/netunicorn/netunicorn-executor/dist/.tmp-zldw1r7u/netunicorn-executor-0.3.0.tar", last modified: Wed May 10 07:50:15 2023, max compression
+gzip compressed data, was "/home/runner/work/netunicorn/netunicorn/netunicorn-executor/dist/.tmp-t38ovkql/netunicorn-executor-0.3.1.tar", last modified: Wed Jun  7 00:22:55 2023, max compression
```

## Comparing `netunicorn-executor-0.3.0.tar` & `netunicorn-executor-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-10 07:50:00.000000 netunicorn-executor-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn/executor/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 07:50:00.000000 netunicorn-executor-0.3.0/src/netunicorn/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 07:50:00.000000 netunicorn-executor-0.3.0/src/netunicorn/executor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-05-10 07:50:00.000000 netunicorn-executor-0.3.0/src/netunicorn/executor/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-07 00:22:40.000000 netunicorn-executor-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/src/netunicorn/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 00:22:40.000000 netunicorn-executor-0.3.1/src/netunicorn/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 00:22:40.000000 netunicorn-executor-0.3.1/src/netunicorn/executor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-06-07 00:22:40.000000 netunicorn-executor-0.3.1/src/netunicorn/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-07 00:22:40.000000 netunicorn-executor-0.3.1/src/netunicorn/executor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/src/netunicorn_executor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/src/netunicorn_executor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/src/netunicorn_executor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/src/netunicorn_executor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/src/netunicorn_executor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 00:22:55.000000 netunicorn-executor-0.3.1/src/netunicorn_executor.egg-info/top_level.txt
```

### Comparing `netunicorn-executor-0.3.0/pyproject.toml` & `netunicorn-executor-0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-executor"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn executor module"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["netunicorn"]
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "returns",
     "cloudpickle",
     "requests",
-    "netunicorn-base >= 0.3.0",
+    "netunicorn-base >= 0.3.3",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.mypy]
 python_version = "3.8"
```

### Comparing `netunicorn-executor-0.3.0/src/netunicorn/executor/executor.py` & `netunicorn-executor-0.3.1/src/netunicorn/executor/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import os
 import sys
 import time
 from asyncio import CancelledError
 from base64 import b64decode, b64encode
 from collections import defaultdict
 from copy import deepcopy
-from typing import Any, Optional, Tuple, Type
+from typing import Any, List, Optional, Tuple, Type, cast
 
 import cloudpickle
 import requests as req
 import requests.exceptions
 from netunicorn.base.pipeline import Pipeline
-from netunicorn.base.task import Task
+from netunicorn.base.task import Task, TaskDispatcher
 from netunicorn.base.types import PipelineExecutorState, PipelineResult
-from netunicorn.base.utils import NonStablePool as Pool
-from netunicorn.base.utils import safe
 from returns.pipeline import is_successful
 from returns.result import Failure, Result, Success
 
+from .utils import NonStablePool as Pool
+from .utils import safe
+
 
 class PipelineExecutor:
     def __init__(
         self,
         executor_id: Optional[str] = None,
         gateway_endpoint: Optional[str] = None,
         experiment_id: Optional[str] = None,
@@ -146,15 +147,15 @@
             self.logger.info(
                 f"Failed to receive pipeline. Status code: {result.status_code}, content: {result.content.decode('utf-8')}"
             )
 
     @staticmethod
     def execute_task(serialized_task: bytes) -> Tuple[str, bytes]:
         task = cloudpickle.loads(serialized_task)
-        result = safe(task.run)()
+        result: Result[Any, Any] = safe(task.run)()
         return task.name, cloudpickle.dumps(result)
 
     def std_redirection(self, *args: Any) -> None:
         _ = args
         sys.stdout = self.print_file
         sys.stderr = self.print_file
 
@@ -168,37 +169,45 @@
 
         if not self.pipeline:
             self.logger.error("No pipeline to execute.")
             self.pipeline_results = Failure(self.step_results)
             return
 
         resulting_type: Type[Result[PipelineResult, PipelineResult]] = Success
-        for element in self.pipeline.tasks:
-            if isinstance(element, Task):
-                element = [element]
+        for elements in self.pipeline.tasks:
+            if isinstance(elements, Task):
+                elements = [elements]
+            for task in elements:
+                if isinstance(task, TaskDispatcher):
+                    self.step_results[task.name].append(
+                        Failure("Element is unexpectedly TaskDispatcher")
+                    )
+                    continue
+
+            element: List[Task] = cast(List[Task], elements)
 
             # create processes and execute tasks
             with Pool(len(element), initializer=self.std_redirection) as p:
                 # attach previous task results to the next step
                 for task in element:
                     task.previous_steps = deepcopy(self.step_results)
 
-                element = [cloudpickle.dumps(task) for task in element]
-                results = p.map_async(
-                    PipelineExecutor.execute_task, element, chunksize=1
+                serialized_element = [cloudpickle.dumps(task) for task in element]
+                execution_results_awaiter = p.map_async(
+                    PipelineExecutor.execute_task, serialized_element, chunksize=1
                 )
 
-                while not results.ready():
+                while not execution_results_awaiter.ready():
                     await asyncio.sleep(1.0)
 
-                results = results.get()
+                execution_results = execution_results_awaiter.get()
 
             results = tuple(
                 (task_name, cloudpickle.loads(result))
-                for (task_name, result) in results
+                for (task_name, result) in execution_results
             )
 
             for task_name, result in results:
                 self.step_results[task_name].append(result)
 
             if any(not is_successful(result) for _, result in results):
                 resulting_type = Failure
@@ -249,11 +258,7 @@
             self.logger.warning(
                 f"Failed to report results. Status code: {result.status_code}, content: {result.content.decode('utf-8')}"
             )
 
 
 if __name__ == "__main__":
     PipelineExecutor().__call__()
-
-# TODO: add event system
-#  short idea: task should somehow be able to send and receive events,
-#  probably pass to run() some object that would allow to do it
```

