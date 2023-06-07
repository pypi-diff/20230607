# Comparing `tmp/ez_cqrs-1.0.1.tar.gz` & `tmp/ez_cqrs-1.0.2.tar.gz`

## Comparing `ez_cqrs-1.0.1.tar` & `ez_cqrs-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/components.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/error.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/framework.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/py.typed
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/shared_state.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/testing.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/requirements/core.txt
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/tests/integration/conftest.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/README.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/error.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/framework.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/py.typed
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/shared_state.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/ez_cqrs/testing.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/requirements/core.txt
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/tests/integration/conftest.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/README.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ez_cqrs-1.0.2/PKG-INFO
```

### Comparing `ez_cqrs-1.0.1/.github/workflows/release.yml` & `ez_cqrs-1.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/.github/workflows/test.yml` & `ez_cqrs-1.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/.vscode/settings.json` & `ez_cqrs-1.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/ez_cqrs/acid_exec.py` & `ez_cqrs-1.0.2/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/ez_cqrs/components.py` & `ez_cqrs-1.0.2/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/ez_cqrs/error.py` & `ez_cqrs-1.0.2/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/ez_cqrs/framework.py` & `ez_cqrs-1.0.2/ez_cqrs/framework.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,16 +35,20 @@
 
     @final
     async def run(
         self,
         cmd: C,
         max_transactions: int,
         config: Config,
-    ) -> Result[None, ExecutionError | pydantic.ValidationError]:
-        """Validate and execute command, then dispatch command events."""
+    ) -> Result[list[E], ExecutionError | pydantic.ValidationError]:
+        """
+        Validate and execute command, then dispatch command events.
+
+        Dispatched events are returned to the caller for client specific usage.
+        """
         validated = self.cmd_handler.validate(command=cmd)
         if not isinstance(validated, Ok):
             return Err(validated.err())
 
         resultant_events = await asyncio.create_task(
             coro=self.cmd_handler.handle(
                 command=cmd,
@@ -52,14 +56,18 @@
                 config=config,
             ),
         )
         if not isinstance(resultant_events, Ok):
             return Err(resultant_events.err())
 
         event_dispatch_tasks: list[Coroutine[Any, Any, None]] = []
-        for event in resultant_events.unwrap():
+
+        list_of_events = resultant_events.unwrap()
+
+        for event in list_of_events:
             event_dispatch_tasks.append(
                 self.event_dispatcher.dispatch(event=event, config=config),
             )
 
-        asyncio.gather(*event_dispatch_tasks)
-        return Ok()
+        asyncio.gather(*event_dispatch_tasks, return_exceptions=False)
+
+        return Ok(list_of_events)
```

### Comparing `ez_cqrs-1.0.1/ez_cqrs/handler.py` & `ez_cqrs-1.0.2/ez_cqrs/handler.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/ez_cqrs/shared_state.py` & `ez_cqrs-1.0.2/ez_cqrs/shared_state.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/ez_cqrs/testing.py` & `ez_cqrs-1.0.2/ez_cqrs/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     from ez_cqrs.shared_state import Config
 
 NO_RESULT_MSG = "No result to evaluate."
 
 
 @final
 @dataclass(frozen=False, repr=False, eq=False)
-class Framework(Generic[C, E]):
-    """Testing framework."""
+class CommandHandlerFramework(Generic[C, E]):
+    """Testing framework for command hanlder."""
 
     cmd_handler: CommandHandler[C, E]
     cmd: C
 
     _result: Result[list[E], ExecutionError] | None = field(init=False, default=None)
     _is_valid: bool | None = field(init=False, default=None)
```

### Comparing `ez_cqrs-1.0.1/requirements/core.txt` & `ez_cqrs-1.0.2/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/requirements/dev.txt` & `ez_cqrs-1.0.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/scripts/new_release.py` & `ez_cqrs-1.0.2/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/tests/integration/conftest.py` & `ez_cqrs-1.0.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/tests/integration/test_execution.py` & `ez_cqrs-1.0.2/tests/integration/test_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from result import Err, Ok, Result
 from typing_extensions import assert_never
 
 from ez_cqrs.acid_exec import OpsRegistry
 from ez_cqrs.components import Command, DomainEvent
 from ez_cqrs.handler import CommandHandler
 from ez_cqrs.shared_state import Config
-from ez_cqrs.testing import Framework
+from ez_cqrs.testing import CommandHandlerFramework
 
 if TYPE_CHECKING:
     import sys
 
     if sys.version_info >= (3, 10):
         from typing import TypeAlias
     else:
@@ -163,15 +163,15 @@
     async def test_with_framework(
         self,
         cmd_handler: BankAccountCommandHandler,
         cmd: BankAccountCommand,
         expected_events: list[BankAccountEvent],
     ) -> None:
         """Test validate command with testing framework."""
-        framework = Framework[
+        framework = CommandHandlerFramework[
             BankAccountCommand,
             BankAccountEvent,
         ](
             cmd_handler=cmd_handler,
             cmd=cmd,
         )
```

### Comparing `ez_cqrs-1.0.1/tests/unit/test_acid_exec.py` & `ez_cqrs-1.0.2/tests/unit/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/.gitignore` & `ez_cqrs-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/LICENSE` & `ez_cqrs-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.1/pyproject.toml` & `ez_cqrs-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-1.0.1/PKG-INFO` & `ez_cqrs-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 1.0.1
+Version: 1.0.2
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

