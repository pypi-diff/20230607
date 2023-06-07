# Comparing `tmp/ez_cqrs-0.2.3.tar.gz` & `tmp/ez_cqrs-0.2.4.tar.gz`

## Comparing `ez_cqrs-0.2.3.tar` & `ez_cqrs-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/ez_cqrs/components.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/ez_cqrs/error.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/ez_cqrs/handler.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/ez_cqrs/ops.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/ez_cqrs/py.typed
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/ez_cqrs/shared_state.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/ez_cqrs/testing.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/requirements/core.txt
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/tests/integration/conftest.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/README.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ez_cqrs-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/ez_cqrs/handler.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/ez_cqrs/ops.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/ez_cqrs/py.typed
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/ez_cqrs/shared_state.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/ez_cqrs/testing.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/requirements/core.txt
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/tests/integration/conftest.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/README.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ez_cqrs-0.2.4/PKG-INFO
```

### Comparing `ez_cqrs-0.2.3/.github/workflows/release.yml` & `ez_cqrs-0.2.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/.github/workflows/test.yml` & `ez_cqrs-0.2.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/.vscode/settings.json` & `ez_cqrs-0.2.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/ez_cqrs/acid_exec.py` & `ez_cqrs-0.2.4/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/ez_cqrs/components.py` & `ez_cqrs-0.2.4/ez_cqrs/components.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,37 +3,27 @@
 
 import abc
 from dataclasses import dataclass
 from typing import TypeVar
 
 from mashumaro import DataClassDictMixin
 from mashumaro.mixins.orjson import DataClassORJSONMixin
-from pydantic import BaseModel
 
 
 @dataclass(frozen=True)
 class Command(abc.ABC, DataClassDictMixin):
     """
     Command baseclass.
 
     In order to make changes to our system we'll need commands. These
     are the simplest components of any CQRS system and consist of little more than
     packaged data.
     """
 
 
-class CommandValidator(abc.ABC, BaseModel):
-    """Command input validator."""
-
-    class Config:
-        """Custom configuration."""
-
-        allow_mutation = False
-
-
 @dataclass(frozen=True)
 class DomainEvent(abc.ABC, DataClassORJSONMixin):
     """
     Domain Event base class.
 
     A `DomainEvent` represents any business change in the state of an `Aggregate`.
     `DomainEvents` are inmutable, and when [event sourcing](https://martinfowler.com/eaaDev/EventSourcing.html)
@@ -47,8 +37,7 @@
     To simplify serialization, an event should be an enum, and each variant should carry
     any important information.
     """
 
 
 C = TypeVar("C", bound=Command)
 E = TypeVar("E", bound=DomainEvent)
-V = TypeVar("V", bound=CommandValidator)
```

### Comparing `ez_cqrs-0.2.3/ez_cqrs/error.py` & `ez_cqrs-0.2.4/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/ez_cqrs/handler.py` & `ez_cqrs-0.2.4/ez_cqrs/handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """Command handler definition."""
 from __future__ import annotations
 
 import abc
 from typing import TYPE_CHECKING, Any, Generic
 
-from ez_cqrs.components import C, E, V
+from ez_cqrs.components import C, E
 
 if TYPE_CHECKING:
-    from pydantic import ValidationError
+    import pydantic
     from result import Result
 
     from ez_cqrs.acid_exec import OpsRegistry
     from ez_cqrs.error import ExecutionError
     from ez_cqrs.shared_state import Config
 
 
-class CommandHandler(abc.ABC, Generic[C, E, V]):
+class CommandHandler(abc.ABC, Generic[C, E]):
     """Command handler handles every command to complete one user intent."""
 
     @abc.abstractmethod
     def validate(
         self,
         command: C,
-        schema: type[V],
-    ) -> Result[None, ValidationError]:
+    ) -> Result[None, pydantic.ValidationError]:
         """Validate command data."""
 
     @abc.abstractmethod
     async def handle(
         self,
         command: C,
         ops_registry: OpsRegistry[Any],
```

### Comparing `ez_cqrs-0.2.3/ez_cqrs/shared_state.py` & `ez_cqrs-0.2.4/ez_cqrs/shared_state.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/ez_cqrs/testing.py` & `ez_cqrs-0.2.4/ez_cqrs/testing.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,35 +9,34 @@
 
 if sys.version_info >= (3, 8):
     from typing import final
 else:
     from typing_extensions import final
 
 from ez_cqrs.acid_exec import OpsRegistry
-from ez_cqrs.components import C, E, V
+from ez_cqrs.components import C, E
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from ez_cqrs.error import ExecutionError
     from ez_cqrs.handler import CommandHandler
     from ez_cqrs.shared_state import Config
 
 NO_RESULT_MSG = "No result to evaluate."
 
 
 @final
 @dataclass()
-class Framework(Generic[C, E, V]):
+class Framework(Generic[C, E]):
     """Testing framework."""
 
-    cmd_handler: CommandHandler[C, E, V]
+    cmd_handler: CommandHandler[C, E]
     cmd: C
 
-    schema_validator: type[V]
     _result: Result[list[E], ExecutionError] | None = field(init=False, default=None)
     _is_valid: bool | None = field(init=False, default=None)
 
     def then_expect_is_valid(self) -> bool:
         """Verify command is valid."""
         if not self._is_valid:
             raise RuntimeError(NO_RESULT_MSG)
@@ -69,15 +68,14 @@
 
     def validate(
         self,
     ) -> Self:
         """Validate command."""
         validated = self.cmd_handler.validate(
             command=self.cmd,
-            schema=self.schema_validator,
         )
         if not isinstance(validated, Ok):
             self._is_valid = False
         self._is_valid = True
         return self
 
     async def execute(
```

### Comparing `ez_cqrs-0.2.3/requirements/core.txt` & `ez_cqrs-0.2.4/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/requirements/dev.txt` & `ez_cqrs-0.2.4/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/scripts/new_release.py` & `ez_cqrs-0.2.4/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/tests/integration/conftest.py` & `ez_cqrs-0.2.4/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/tests/integration/test_execution.py` & `ez_cqrs-0.2.4/tests/integration/test_execution.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Union
 
 import pydantic
 import pytest
-from pydantic import ValidationError
+from pydantic import BaseModel, ValidationError
 from result import Err, Ok, Result
+from typing_extensions import assert_never
 
 from ez_cqrs import ops
 from ez_cqrs.acid_exec import OpsRegistry
-from ez_cqrs.components import Command, CommandValidator, DomainEvent
+from ez_cqrs.components import Command, DomainEvent
 from ez_cqrs.handler import CommandHandler
 from ez_cqrs.shared_state import Config
 from ez_cqrs.testing import Framework
 
 if TYPE_CHECKING:
     import sys
 
@@ -38,21 +39,14 @@
     account_id: str
     amount: int
 
 
 BankAccountCommand: TypeAlias = Union[OpenAccount, DepositMoney]
 
 
-class OpenAccountValidator(CommandValidator):  # noqa: D101
-    amount: int = pydantic.Field(gt=0)
-
-
-BankAccountValidator: TypeAlias = OpenAccountValidator
-
-
 @dataclass(frozen=True)
 class AccountOpened(DomainEvent):  # noqa: D101
     account_id: str
     amount: int
 
 
 @dataclass(frozen=True)
@@ -61,27 +55,42 @@
     amount: int
 
 
 BankAccountEvent: TypeAlias = Union[AccountOpened, MoneyDeposited]
 
 
 class BankAccountCommandHandler(  # noqa: D101
-    CommandHandler[BankAccountCommand, BankAccountEvent, BankAccountValidator],
+    CommandHandler[BankAccountCommand, BankAccountEvent],
 ):
     def validate(  # noqa: D102
         self,
         command: BankAccountCommand,
-        schema: type[BankAccountValidator],
     ) -> Result[None, ValidationError]:
-        try:
-            schema(**command.to_dict())
-        except ValidationError as e:
-            return Err(e)
+        if isinstance(command, OpenAccount):
+
+            class OpenAccountValidator(BaseModel):
+                amount: int = pydantic.Field(gt=0)
+
+            try:
+                OpenAccountValidator(amount=command.amount)
+            except ValidationError as e:
+                return Err(e)
+            return Ok()
+        if isinstance(command, DepositMoney):
+
+            class DepositMoneyValidator(BaseModel):
+                amount: int = pydantic.Field(gt=0)
+
+            try:
+                DepositMoneyValidator(amount=command.amount)
+            except ValidationError as e:
+                return Err(e)
+            return Ok()
 
-        return Ok()
+        assert_never(command)
 
     async def handle(  # noqa: D102
         self,
         command: BankAccountCommand,
         ops_registry: OpsRegistry[Any],
         config: Config,
     ) -> Result[list[BankAccountEvent], ExecutionError]:
@@ -91,36 +100,34 @@
             return Ok(
                 [AccountOpened(account_id=command.account_id, amount=command.amount)],
             )
         if isinstance(command, DepositMoney):
             return Ok(
                 [MoneyDeposited(account_id=command.account_id, amount=command.amount)],
             )
-        return None
+        assert_never(command)
 
 
 @pytest.mark.integration()
 class TestCommandHanlder:  # noqa: D101
     @pytest.mark.parametrize(
-        argnames=["command", "validator"],
+        argnames="command",
         argvalues=[
-            (OpenAccount(account_id="123", amount=1_000_000), OpenAccountValidator),
+            OpenAccount(account_id="123", amount=1_000_000),
         ],
     )
     async def test_validate(
         self,
         command: BankAccountCommand,
-        validator: type[BankAccountValidator],
     ) -> None:
         """Test validate method."""
         cmd_handler = BankAccountCommandHandler()
 
         validated = cmd_handler.validate(
             command=command,
-            schema=validator,
         )
         assert validated.unwrap()
 
     @pytest.mark.parametrize(
         argnames=["command", "expected_events"],
         argvalues=[
             (
@@ -141,68 +148,61 @@
             command=command,
             ops_registry=OpsRegistry[Any](max_lenght=0),
             config=app_config,
         )
         assert resultant_events.unwrap() == expected_events
 
     @pytest.mark.parametrize(
-        argnames=["cmd_handler", "cmd", "validator", "expected_events"],
+        argnames=["cmd_handler", "cmd", "expected_events"],
         argvalues=[
             (
                 BankAccountCommandHandler(),
                 OpenAccount(account_id="123", amount=1),
-                OpenAccountValidator,
                 [AccountOpened(account_id="123", amount=1)],
             ),
         ],
     )
     async def test_validate_and_execute_cmd(
         self,
         cmd_handler: BankAccountCommandHandler,
         cmd: BankAccountCommand,
-        validator: type[BankAccountValidator],
         expected_events: list[BankAccountEvent],
     ) -> None:
         """Test validate and execution cmd operation."""
         resultant_events = await ops.validate_and_execute_cmd(
             cmd_handler=cmd_handler,
             command=cmd,
-            schema=validator,
             max_transactions=0,
             config=Config(),
         )
         assert resultant_events.unwrap() == expected_events
 
     @pytest.mark.parametrize(
-        argnames=["cmd_handler", "cmd", "validator", "expected_events"],
+        argnames=["cmd_handler", "cmd", "expected_events"],
         argvalues=[
             (
                 BankAccountCommandHandler(),
                 OpenAccount(account_id="123", amount=1),
-                OpenAccountValidator,
                 [AccountOpened(account_id="123", amount=1)],
             ),
         ],
     )
     async def test_with_framework(
         self,
         cmd_handler: BankAccountCommandHandler,
         cmd: BankAccountCommand,
-        validator: type[BankAccountValidator],
         expected_events: list[BankAccountEvent],
     ) -> None:
         """Test validate command with testing framework."""
         framework = Framework[
             BankAccountCommand,
             BankAccountEvent,
-            BankAccountValidator,
         ](
             cmd_handler=cmd_handler,
             cmd=cmd,
-            schema_validator=validator,
         )
 
         assert framework.validate().then_expect_is_valid()
         await framework.execute(
             max_transactions=0,
             config=Config(),
         )
```

### Comparing `ez_cqrs-0.2.3/tests/unit/test_acid_exec.py` & `ez_cqrs-0.2.4/tests/unit/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/.gitignore` & `ez_cqrs-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/LICENSE` & `ez_cqrs-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.3/pyproject.toml` & `ez_cqrs-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "0.2.3"
+version = "0.2.4"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-0.2.3/PKG-INFO` & `ez_cqrs-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 0.2.3
+Version: 0.2.4
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

