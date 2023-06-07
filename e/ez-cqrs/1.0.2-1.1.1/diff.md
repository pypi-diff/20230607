# Comparing `tmp/ez_cqrs-1.0.2.tar.gz` & `tmp/ez_cqrs-1.1.1.tar.gz`

## Comparing `ez_cqrs-1.0.2.tar` & `ez_cqrs-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/components.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/error.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/framework.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/py.typed
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/shared_state.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/testing.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/requirements/core.txt
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/tests/integration/conftest.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/README.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/error.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/framework.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/py.typed
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/shared_state.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/testing.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/requirements/core.txt
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/README.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/PKG-INFO
```

### Comparing `ez_cqrs-1.0.2/.github/workflows/release.yml` & `ez_cqrs-1.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/.github/workflows/test.yml` & `ez_cqrs-1.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/.vscode/settings.json` & `ez_cqrs-1.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/ez_cqrs/acid_exec.py` & `ez_cqrs-1.1.1/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/ez_cqrs/components.py` & `ez_cqrs-1.1.1/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/ez_cqrs/error.py` & `ez_cqrs-1.1.1/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/ez_cqrs/framework.py` & `ez_cqrs-1.1.1/ez_cqrs/framework.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Ez-Cqrs Framwork."""
 from __future__ import annotations
 
 import asyncio
 import sys
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Generic
+from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
 from result import Err, Ok, Result
 
 from ez_cqrs.acid_exec import OpsRegistry
 from ez_cqrs.components import C, E
 
 if sys.version_info >= (3, 8):
@@ -21,53 +21,60 @@
 
     import pydantic
 
     from ez_cqrs.error import ExecutionError
     from ez_cqrs.handler import CommandHandler, EventDispatcher
     from ez_cqrs.shared_state import Config
 
+T = TypeVar("T")
+
 
 @dataclass(repr=True, frozen=True, eq=False)
 class EzCqrs(Generic[C, E]):
     """EzCqrs framework."""
 
     cmd_handler: CommandHandler[C, E]
     event_dispatcher: EventDispatcher[E]
 
     @final
     async def run(
         self,
         cmd: C,
         max_transactions: int,
         config: Config,
-    ) -> Result[list[E], ExecutionError | pydantic.ValidationError]:
+        expected_val: type[T],
+    ) -> Result[T, ExecutionError | pydantic.ValidationError]:
         """
         Validate and execute command, then dispatch command events.
 
         Dispatched events are returned to the caller for client specific usage.
         """
         validated = self.cmd_handler.validate(command=cmd)
         if not isinstance(validated, Ok):
             return Err(validated.err())
 
-        resultant_events = await asyncio.create_task(
+        execution_result = await asyncio.create_task(
             coro=self.cmd_handler.handle(
                 command=cmd,
                 ops_registry=OpsRegistry[Any](max_lenght=max_transactions),
                 config=config,
             ),
         )
-        if not isinstance(resultant_events, Ok):
-            return Err(resultant_events.err())
+        if not isinstance(execution_result, Ok):
+            return Err(execution_result.err())
 
         event_dispatch_tasks: list[Coroutine[Any, Any, None]] = []
 
-        list_of_events = resultant_events.unwrap()
+        execution_value, list_of_events = execution_result.unwrap()
 
         for event in list_of_events:
             event_dispatch_tasks.append(
                 self.event_dispatcher.dispatch(event=event, config=config),
             )
 
         asyncio.gather(*event_dispatch_tasks, return_exceptions=False)
 
-        return Ok(list_of_events)
+        if not isinstance(execution_value, expected_val):
+            msg = "Returned value from command does not match expected type."
+            raise TypeError(msg)
+
+        return Ok(execution_value)
```

### Comparing `ez_cqrs-1.0.2/ez_cqrs/handler.py` & `ez_cqrs-1.1.1/ez_cqrs/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     @abc.abstractmethod
     async def handle(
         self,
         command: C,
         ops_registry: OpsRegistry[Any],
         config: Config,
-    ) -> Result[list[E], ExecutionError]:
+    ) -> Result[tuple[Any, list[E]], ExecutionError]:
         """
         Consume and process commands.
 
         The result should be either a vector of events if the command is successful,
         or an error is the command is rejected.
 
         _All business logic belongs in this method_.
```

### Comparing `ez_cqrs-1.0.2/ez_cqrs/shared_state.py` & `ez_cqrs-1.1.1/ez_cqrs/shared_state.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/ez_cqrs/testing.py` & `ez_cqrs-1.1.1/ez_cqrs/testing.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 @dataclass(frozen=False, repr=False, eq=False)
 class CommandHandlerFramework(Generic[C, E]):
     """Testing framework for command hanlder."""
 
     cmd_handler: CommandHandler[C, E]
     cmd: C
 
-    _result: Result[list[E], ExecutionError] | None = field(init=False, default=None)
+    _result: Result[tuple[Any, list[E]], ExecutionError] | None = field(
+        init=False,
+        default=None,
+    )
     _is_valid: bool | None = field(init=False, default=None)
 
     def then_expect_is_valid(self) -> bool:
         """Verify command is valid."""
         if not self._is_valid:
             raise RuntimeError(NO_RESULT_MSG)
         return self._is_valid
@@ -51,25 +54,47 @@
     def then_expect_events(self, expected_events: list[E]) -> bool:
         """Verify expected events have been produced by the command."""
         if not self._result:
             raise RuntimeError(NO_RESULT_MSG)
         if not isinstance(self._result, Ok):
             msg = f"expected success, received execution error: {self._result.err()}"
             raise TypeError(msg)
-        return self._result.unwrap() == expected_events
+        _, resultant_events = self._result.unwrap()
+        return resultant_events == expected_events
+
+    def then_expect_value(self, expected_value: Any) -> bool:  # noqa: ANN401
+        """Verify expected value has been produced by the command."""
+        if not self._result:
+            raise RuntimeError(NO_RESULT_MSG)
+        if not isinstance(self._result, Ok):
+            msg = f"expected success, received execution error: {self._result.err()}"
+            raise TypeError(msg)
+        resultant_value, _ = self._result.unwrap()
+        return resultant_value == expected_value
 
     def then_expect_error_message(self, err_msg: str) -> bool:
         """Verify expected error msg have been produced by the command."""
         if not self._result:
             raise RuntimeError(NO_RESULT_MSG)
         if isinstance(self._result, Ok):
             msg = f"expected error, received events: {self._result.unwrap()}"
             raise TypeError(msg)
         return str(self._result.err()) == err_msg
 
+    def inspect_result(self) -> tuple[Any, list[E]]:
+        """Inspect execution result."""
+        if not self._result:
+            raise RuntimeError(NO_RESULT_MSG)
+
+        if not isinstance(self._result, Ok):
+            msg = f"expected success, received execution error: {self._result.err()}"
+            raise TypeError(msg)
+
+        return self._result.unwrap()
+
     def validate(
         self,
     ) -> Self:
         """Validate command."""
         validated = self.cmd_handler.validate(
             command=self.cmd,
         )
@@ -81,17 +106,18 @@
     async def execute(
         self,
         max_transactions: int,
         config: Config,
     ) -> Self:
         """Execute command while asserting and validating framework's rules."""
         ops_registry = OpsRegistry[Any](max_lenght=max_transactions)
-        resultant_events = await self.cmd_handler.handle(
+        execution_result = await self.cmd_handler.handle(
             command=self.cmd,
             ops_registry=ops_registry,
             config=config,
         )
         if not ops_registry.is_empty():
             msg = "OpsRegistry is not empty after cmd execution."
             raise RuntimeError(msg)
-        self._result = resultant_events
+
+        self._result = execution_result
         return self
```

### Comparing `ez_cqrs-1.0.2/requirements/core.txt` & `ez_cqrs-1.1.1/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/requirements/dev.txt` & `ez_cqrs-1.1.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/scripts/new_release.py` & `ez_cqrs-1.1.1/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/tests/integration/conftest.py` & `ez_cqrs-1.1.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/tests/unit/test_acid_exec.py` & `ez_cqrs-1.1.1/tests/unit/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/.gitignore` & `ez_cqrs-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/LICENSE` & `ez_cqrs-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.2/pyproject.toml` & `ez_cqrs-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "1.0.2"
+version = "1.1.1"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-1.0.2/PKG-INFO` & `ez_cqrs-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 1.0.2
+Version: 1.1.1
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

