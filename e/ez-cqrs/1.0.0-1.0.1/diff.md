# Comparing `tmp/ez_cqrs-1.0.0.tar.gz` & `tmp/ez_cqrs-1.0.1.tar.gz`

## Comparing `ez_cqrs-1.0.0.tar` & `ez_cqrs-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/ez_cqrs/components.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/ez_cqrs/error.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/ez_cqrs/framework.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/ez_cqrs/handler.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/ez_cqrs/ops.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/ez_cqrs/py.typed
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/ez_cqrs/shared_state.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/ez_cqrs/testing.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/requirements/core.txt
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/README.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ez_cqrs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/framework.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/py.typed
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/shared_state.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/ez_cqrs/testing.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/requirements/core.txt
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/README.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ez_cqrs-1.0.1/PKG-INFO
```

### Comparing `ez_cqrs-1.0.0/.github/workflows/release.yml` & `ez_cqrs-1.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/.github/workflows/test.yml` & `ez_cqrs-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/.vscode/settings.json` & `ez_cqrs-1.0.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/ez_cqrs/acid_exec.py` & `ez_cqrs-1.0.1/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/ez_cqrs/components.py` & `ez_cqrs-1.0.1/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/ez_cqrs/error.py` & `ez_cqrs-1.0.1/ez_cqrs/error.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Error base class."""
 from __future__ import annotations
 
 import abc
+import sys
 from typing import TYPE_CHECKING, Union
 
+if sys.version_info >= (3, 8):
+    from typing import final
+else:
+    from typing_extensions import final
 if TYPE_CHECKING:
-    import sys
-
     if sys.version_info >= (3, 10):
         from typing import TypeAlias
     else:
         from typing_extensions import TypeAlias
 
 
 class DomainError(abc.ABC, Exception):
@@ -20,21 +23,23 @@
     This is the error returned when a user violates a business rule. The payload passed
     should be used to inform the user of the nature of a problem.
 
     This translates into a `Bad Request` status.
     """
 
 
+@final
 class DatabaseError(Exception):
     """Raised whwne that's an error interacting with system's database."""
 
     def __init__(self, database_error: Exception) -> None:  # noqa: D107
         super().__init__(f"An error ocurred with database {database_error}")
 
 
+@final
 class UnexpectedError(Exception):
     """
     Raised when an unexpected error was encountered.
 
     A technical error was encountered teht prevented the command from being applied to
     the aggregate. In general the accompanying message should be logged for
     investigation rather than returned to the user.
```

### Comparing `ez_cqrs-1.0.0/ez_cqrs/framework.py` & `ez_cqrs-1.0.1/ez_cqrs/framework.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 """Ez-Cqrs Framwork."""
 from __future__ import annotations
 
 import asyncio
+import sys
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Generic
 
 from result import Err, Ok, Result
 
 from ez_cqrs.acid_exec import OpsRegistry
 from ez_cqrs.components import C, E
 
+if sys.version_info >= (3, 8):
+    from typing import final
+else:
+    from typing_extensions import final
+
 if TYPE_CHECKING:
     from collections.abc import Coroutine
 
     import pydantic
 
     from ez_cqrs.error import ExecutionError
     from ez_cqrs.handler import CommandHandler, EventDispatcher
@@ -23,14 +29,15 @@
 @dataclass(repr=True, frozen=True, eq=False)
 class EzCqrs(Generic[C, E]):
     """EzCqrs framework."""
 
     cmd_handler: CommandHandler[C, E]
     event_dispatcher: EventDispatcher[E]
 
+    @final
     async def run(
         self,
         cmd: C,
         max_transactions: int,
         config: Config,
     ) -> Result[None, ExecutionError | pydantic.ValidationError]:
         """Validate and execute command, then dispatch command events."""
```

### Comparing `ez_cqrs-1.0.0/ez_cqrs/handler.py` & `ez_cqrs-1.0.1/ez_cqrs/handler.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/ez_cqrs/shared_state.py` & `ez_cqrs-1.0.1/ez_cqrs/shared_state.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/ez_cqrs/testing.py` & `ez_cqrs-1.0.1/ez_cqrs/testing.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     from ez_cqrs.handler import CommandHandler
     from ez_cqrs.shared_state import Config
 
 NO_RESULT_MSG = "No result to evaluate."
 
 
 @final
-@dataclass()
+@dataclass(frozen=False, repr=False, eq=False)
 class Framework(Generic[C, E]):
     """Testing framework."""
 
     cmd_handler: CommandHandler[C, E]
     cmd: C
 
     _result: Result[list[E], ExecutionError] | None = field(init=False, default=None)
```

### Comparing `ez_cqrs-1.0.0/requirements/core.txt` & `ez_cqrs-1.0.1/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/requirements/dev.txt` & `ez_cqrs-1.0.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/scripts/new_release.py` & `ez_cqrs-1.0.1/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/tests/integration/conftest.py` & `ez_cqrs-1.0.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/tests/integration/test_execution.py` & `ez_cqrs-1.0.1/tests/integration/test_execution.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import pydantic
 import pytest
 from pydantic import BaseModel, ValidationError
 from result import Err, Ok, Result
 from typing_extensions import assert_never
 
-from ez_cqrs import ops
 from ez_cqrs.acid_exec import OpsRegistry
 from ez_cqrs.components import Command, DomainEvent
 from ez_cqrs.handler import CommandHandler
 from ez_cqrs.shared_state import Config
 from ez_cqrs.testing import Framework
 
 if TYPE_CHECKING:
@@ -151,39 +150,14 @@
         )
         assert resultant_events.unwrap() == expected_events
 
     @pytest.mark.parametrize(
         argnames=["cmd_handler", "cmd", "expected_events"],
         argvalues=[
             (
-                BankAccountCommandHandler(),
-                OpenAccount(account_id="123", amount=1),
-                [AccountOpened(account_id="123", amount=1)],
-            ),
-        ],
-    )
-    async def test_validate_and_execute_cmd(
-        self,
-        cmd_handler: BankAccountCommandHandler,
-        cmd: BankAccountCommand,
-        expected_events: list[BankAccountEvent],
-    ) -> None:
-        """Test validate and execution cmd operation."""
-        resultant_events = await ops.validate_and_execute_cmd(
-            cmd_handler=cmd_handler,
-            command=cmd,
-            max_transactions=0,
-            config=Config(),
-        )
-        assert resultant_events.unwrap() == expected_events
-
-    @pytest.mark.parametrize(
-        argnames=["cmd_handler", "cmd", "expected_events"],
-        argvalues=[
-            (
                 BankAccountCommandHandler(),
                 OpenAccount(account_id="123", amount=1),
                 [AccountOpened(account_id="123", amount=1)],
             ),
         ],
     )
     async def test_with_framework(
```

### Comparing `ez_cqrs-1.0.0/tests/unit/test_acid_exec.py` & `ez_cqrs-1.0.1/tests/unit/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/.gitignore` & `ez_cqrs-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/LICENSE` & `ez_cqrs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.0.0/pyproject.toml` & `ez_cqrs-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "1.0.0"
+version = "1.0.1"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-1.0.0/PKG-INFO` & `ez_cqrs-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 1.0.0
+Version: 1.0.1
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

