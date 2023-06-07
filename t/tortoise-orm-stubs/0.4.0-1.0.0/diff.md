# Comparing `tmp/tortoise_orm_stubs-0.4.0.tar.gz` & `tmp/tortoise_orm_stubs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_orm_stubs-0.4.0.tar", max compression
+gzip compressed data, was "tortoise_orm_stubs-1.0.0.tar", max compression
```

## Comparing `tortoise_orm_stubs-0.4.0.tar` & `tortoise_orm_stubs-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2022-09-22 00:21:21.676040 tortoise_orm_stubs-0.4.0/LICENSE
--rw-r--r--   0        0        0      530 2023-06-07 05:41:26.929564 tortoise_orm_stubs-0.4.0/README.md
--rw-r--r--   0        0        0     1060 2023-06-07 05:41:39.556162 tortoise_orm_stubs-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    13348 2023-06-07 05:49:03.173727 tortoise_orm_stubs-0.4.0/tortoise-stubs/fields/__init__.pyi
--rw-r--r--   0        0        0        8 2022-09-22 19:51:35.803221 tortoise_orm_stubs-0.4.0/tortoise-stubs/py.typed
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 tortoise_orm_stubs-0.4.0/setup.py
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 tortoise_orm_stubs-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-09-22 00:21:21.676040 tortoise_orm_stubs-1.0.0/LICENSE
+-rw-r--r--   0        0        0      511 2023-04-25 17:47:14.750054 tortoise_orm_stubs-1.0.0/README.md
+-rw-r--r--   0        0        0     1060 2023-04-25 13:12:52.836668 tortoise_orm_stubs-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13458 2023-04-25 16:51:11.673362 tortoise_orm_stubs-1.0.0/tortoise-stubs/fields/__init__.pyi
+-rw-r--r--   0        0        0        8 2022-09-22 19:51:35.803221 tortoise_orm_stubs-1.0.0/tortoise-stubs/py.typed
+-rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 tortoise_orm_stubs-1.0.0/setup.py
+-rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 tortoise_orm_stubs-1.0.0/PKG-INFO
```

### Comparing `tortoise_orm_stubs-0.4.0/LICENSE` & `tortoise_orm_stubs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise_orm_stubs-0.4.0/pyproject.toml` & `tortoise_orm_stubs-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tortoise-orm-stubs"
-version = "0.4.0"
+version = "1.0.0"
 description = "Type stubs that make tortoise-orm a lot easier to work with when using type checkers."
 packages = [{ include = "tortoise-stubs" }]
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Ovsyanka83/tortoise-orm-stubs"
```

### Comparing `tortoise_orm_stubs-0.4.0/tortoise-stubs/fields/__init__.pyi` & `tortoise_orm_stubs-1.0.0/tortoise-stubs/fields/__init__.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import datetime
 import decimal
+import typing
 import uuid
-from typing import Any, Callable, Generic, List, Literal, Optional, Type, TypeVar, Union, overload
+from typing import Any, Callable, List, Literal, Optional, Type, Union, overload
 
+import tortoise.fields.base
 import tortoise.validators
-from tortoise.fields.base import NO_ACTION, SET_DEFAULT
-from tortoise.fields.base import Field as _Field
+from tortoise.fields.base import NO_ACTION, SET_DEFAULT, Field
 from tortoise.fields.data import CharEnumType, IntEnumType
 from tortoise.fields.relational import (
     CASCADE,
     RESTRICT,
     SET_NULL,
     BackwardFKRelation,
     BackwardOneToOneRelation,
+    ForeignKeyField,
     ForeignKeyNullableRelation,
     ForeignKeyRelation,
     ManyToManyField,
     ManyToManyRelation,
+    OneToOneField,
     OneToOneNullableRelation,
     OneToOneRelation,
     ReverseRelation,
 )
 from tortoise.models import Model
 
 __all__ = [
@@ -56,116 +59,108 @@
     "ManyToManyField",
     "ManyToManyRelation",
     "OneToOneField",
     "OneToOneNullableRelation",
     "OneToOneRelation",
     "ReverseRelation",
 ]
-VALUE = TypeVar("VALUE")
-
-class Field(Generic[VALUE], _Field):
-    def __new__(cls, *args: Any, **kwargs: Any) -> "Field[VALUE]": ...
-    @overload
-    def __get__(self, instance: None, owner: Type["Model"]) -> "Field[VALUE]": ...
-    @overload
-    def __get__(self, instance: "Model", owner: Type["Model"]) -> VALUE: ...
-    def __get__(self, instance: Optional["Model"], owner: Type["Model"]) -> "Field[VALUE] | VALUE": ...
-    def __set__(self, instance: "Model", value: VALUE) -> None: ...
 
 @overload
-def BigIntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> int:
+def BigIntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> tortoise.fields.base.Field[int]:
     """
     Big integer field. (64-bit signed)
 
     ``pk`` (bool):
         True if field is Primary Key.
     """
 
 @overload
-def BigIntField(pk: bool = False, *, null: Literal[True], **kwargs: Any) -> Union[int, None]: ...
+def BigIntField(
+    pk: bool = False, *, null: Literal[True], **kwargs: Any
+) -> tortoise.fields.base.Field[typing.Optional[int]]: ...
 @overload
 def BinaryField(
-    source_field: Union[str, None] = None,
+    source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[False] = False,
     default: Any = None,
     unique: bool = False,
     index: bool = False,
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     model: "Optional[Model]" = None,
-    validators: Union[List[Union[tortoise.validators.Validator, Callable]], None] = None,
+    validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> bytes:
+) -> tortoise.fields.base.Field[bytes]:
     """
     Binary field.
 
     This is for storing ``bytes`` objects.
     Note that filter or queryset-update operations are not supported.
     """
 
 @overload
 def BinaryField(
-    source_field: Union[str, None] = None,
+    source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[True],
     default: Any = None,
     unique: bool = False,
     index: bool = False,
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     model: "Optional[Model]" = None,
-    validators: Union[List[Union[tortoise.validators.Validator, Callable]], None] = None,
+    validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Union[bytes, None]: ...
+) -> tortoise.fields.base.Field[typing.Optional[bytes]]: ...
 @overload
 def BooleanField(
-    source_field: Union[str, None] = None,
+    source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[False] = False,
     default: Any = None,
     unique: bool = False,
     index: bool = False,
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     model: "Optional[Model]" = None,
-    validators: Union[List[Union[tortoise.validators.Validator, Callable]], None] = None,
+    validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> bool:
+) -> tortoise.fields.base.Field[bool]:
     """
     Boolean field.
     """
 
 @overload
 def BooleanField(
-    source_field: Union[str, None] = None,
+    source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[True],
     default: Any = None,
     unique: bool = False,
     index: bool = False,
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     model: "Optional[Model]" = None,
-    validators: Union[List[Union[tortoise.validators.Validator, Callable]], None] = None,
+    validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Union[bool, None]: ...
+) -> tortoise.fields.base.Field[typing.Optional[bool]]: ...
 @overload
 def CharEnumField(
     enum_type: Type[CharEnumType],
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     max_length: int = 0,
     *,
     null: Literal[False] = False,
     **kwargs: Any,
-) -> CharEnumType:
+) -> tortoise.fields.base.Field[CharEnumType]:
     """
     Char Enum Field
 
     A field representing a character enumeration.
 
     **Warning**: If ``max_length`` is not specified or equals to zero, the size of represented
     char fields is automatically detected. So if later you update the enum, you need to update your
@@ -183,71 +178,73 @@
         enum_type.
 
     """
 
 @overload
 def CharEnumField(
     enum_type: Type[CharEnumType],
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     max_length: int = 0,
     *,
     null: Literal[True],
     **kwargs: Any,
-) -> Union[CharEnumType, None]: ...
+) -> tortoise.fields.base.Field[typing.Optional[CharEnumType]]: ...
 @overload
-def CharField(max_length: int, *, null: Literal[False] = False, **kwargs: Any) -> str:
+def CharField(max_length: int, *, null: Literal[False] = False, **kwargs: Any) -> tortoise.fields.base.Field[str]:
     """
     Character field.
 
     You must provide the following:
 
     ``max_length`` (int):
         Maximum length of the field in characters.
     """
 
 @overload
-def CharField(max_length: int, *, null: Literal[True], **kwargs: Any) -> Union[str, None]: ...
+def CharField(
+    max_length: int, *, null: Literal[True], **kwargs: Any
+) -> tortoise.fields.base.Field[typing.Optional[str]]: ...
 @overload
 def DateField(
-    source_field: Union[str, None] = None,
+    source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[False] = False,
     default: Any = None,
     unique: bool = False,
     index: bool = False,
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     model: "Optional[Model]" = None,
-    validators: Union[List[Union[tortoise.validators.Validator, Callable]], None] = None,
+    validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> datetime.date:
+) -> tortoise.fields.base.Field[datetime.date]:
     """
     Date field.
     """
 
 @overload
 def DateField(
-    source_field: Union[str, None] = None,
+    source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[True],
     default: Any = None,
     unique: bool = False,
     index: bool = False,
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     model: "Optional[Model]" = None,
-    validators: Union[List[Union[tortoise.validators.Validator, Callable]], None] = None,
+    validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Union[datetime.date, None]: ...
+) -> tortoise.fields.base.Field[typing.Optional[datetime.date]]: ...
 @overload
 def DatetimeField(
     auto_now: bool = False, auto_now_add: bool = False, *, null: Literal[False] = False, **kwargs: Any
-) -> datetime.datetime:
+) -> tortoise.fields.base.Field[datetime.datetime]:
     """
     Datetime field.
 
     ``auto_now`` and ``auto_now_add`` is exclusive.
     You can opt to set neither or only ONE of them.
 
     ``auto_now`` (bool):
@@ -255,72 +252,72 @@
     ``auto_now_add`` (bool):
         Set to ``datetime.utcnow()`` on first save only.
     """
 
 @overload
 def DatetimeField(
     auto_now: bool = False, auto_now_add: bool = False, *, null: Literal[True], **kwargs: Any
-) -> Union[datetime.datetime, None]: ...
+) -> tortoise.fields.base.Field[typing.Optional[datetime.datetime]]: ...
 @overload
 def DecimalField(
     max_digits: int, decimal_places: int, *, null: Literal[False] = False, **kwargs: Any
-) -> decimal.Decimal:
+) -> tortoise.fields.base.Field[decimal.Decimal]:
     """
     Accurate decimal field.
 
     You must provide the following:
 
     ``max_digits`` (int):
         Max digits of significance of the decimal field.
     ``decimal_places`` (int):
         How many of those significant digits is after the decimal point.
     """
 
 @overload
 def DecimalField(
     max_digits: int, decimal_places: int, *, null: Literal[True], **kwargs: Any
-) -> Union[decimal.Decimal, None]: ...
+) -> tortoise.fields.base.Field[typing.Optional[decimal.Decimal]]: ...
 @overload
 def FloatField(
-    source_field: Union[str, None] = None,
+    source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[False] = False,
     default: Any = None,
     unique: bool = False,
     index: bool = False,
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     model: "Optional[Model]" = None,
-    validators: Union[List[Union[tortoise.validators.Validator, Callable]], None] = None,
+    validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> float:
+) -> tortoise.fields.base.Field[float]:
     """
     Float (double) field.
     """
 
 @overload
 def FloatField(
-    source_field: Union[str, None] = None,
+    source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[True],
     default: Any = None,
     unique: bool = False,
     index: bool = False,
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     model: "Optional[Model]" = None,
-    validators: Union[List[Union[tortoise.validators.Validator, Callable]], None] = None,
+    validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Union[float, None]: ...
+) -> tortoise.fields.base.Field[typing.Optional[float]]: ...
 @overload
 def IntEnumField(
-    enum_type: Type[IntEnumType], description: Union[str, None] = None, *, null: Literal[False] = False, **kwargs: Any
-) -> IntEnumType:
+    enum_type: Type[IntEnumType], description: Optional[str] = None, *, null: Literal[False] = False, **kwargs: Any
+) -> tortoise.fields.base.Field[IntEnumType]:
     """
     Enum Field
 
     A field representing an integer enumeration.
 
     The description of the field is set automatically if not specified to a multiline list of
     "name: value" pairs.
@@ -333,35 +330,37 @@
         The description of the field. It is set automatically if not specified to a multiline list
         of "name: value" pairs.
 
     """
 
 @overload
 def IntEnumField(
-    enum_type: Type[IntEnumType], description: Union[str, None] = None, *, null: Literal[True], **kwargs: Any
-) -> Union[IntEnumType, None]: ...
+    enum_type: Type[IntEnumType], description: Optional[str] = None, *, null: Literal[True], **kwargs: Any
+) -> tortoise.fields.base.Field[typing.Optional[IntEnumType]]: ...
 @overload
-def IntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> int:
+def IntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> tortoise.fields.base.Field[int]:
     """
     Integer field. (32-bit signed)
 
     ``pk`` (bool):
         True if field is Primary Key.
     """
 
 @overload
-def IntField(pk: bool = False, *, null: Literal[True], **kwargs: Any) -> Union[int, None]: ...
+def IntField(
+    pk: bool = False, *, null: Literal[True], **kwargs: Any
+) -> tortoise.fields.base.Field[typing.Optional[int]]: ...
 @overload
 def JSONField(
     encoder: Callable[[Any], str] = ...,
     decoder: Callable[[Union[str, bytes]], Any] = ...,
     *,
     null: Literal[False] = False,
     **kwargs: Any,
-) -> Any:
+) -> tortoise.fields.base.Field[typing.Union[dict, list]]:
     """
     JSON field.
 
     This field can store dictionaries or lists of any JSON-compliant structure.
 
     You can specify your own custom JSON encoder/decoder, leaving at the default should work well.
     If you have ``python-rapidjson`` installed, we default to using that,
@@ -377,103 +376,91 @@
 @overload
 def JSONField(
     encoder: Callable[[Any], str] = ...,
     decoder: Callable[[Union[str, bytes]], Any] = ...,
     *,
     null: Literal[True],
     **kwargs: Any,
-) -> Optional[Any]: ...
+) -> tortoise.fields.base.Field[typing.Union[dict, list, None]]: ...
 @overload
-def SmallIntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> int:
+def SmallIntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> tortoise.fields.base.Field[int]:
     """
     Small integer field. (16-bit signed)
 
     ``pk`` (bool):
         True if field is Primary Key.
     """
 
 @overload
-def SmallIntField(pk: bool = False, *, null: Literal[True], **kwargs: Any) -> Union[int, None]: ...
+def SmallIntField(
+    pk: bool = False, *, null: Literal[True], **kwargs: Any
+) -> tortoise.fields.base.Field[typing.Optional[int]]: ...
 @overload
 def TextField(
     pk: bool = False, unique: bool = False, index: bool = False, *, null: Literal[False] = False, **kwargs: Any
-) -> str:
+) -> tortoise.fields.base.Field[str]:
     """
     Large Text field.
     """
 
 @overload
 def TextField(
     pk: bool = False, unique: bool = False, index: bool = False, *, null: Literal[True], **kwargs: Any
-) -> Union[str, None]: ...
+) -> tortoise.fields.base.Field[typing.Optional[str]]: ...
 @overload
 def TimeDeltaField(
-    source_field: Union[str, None] = None,
+    source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[False] = False,
     default: Any = None,
     unique: bool = False,
     index: bool = False,
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     model: "Optional[Model]" = None,
-    validators: Union[List[Union[tortoise.validators.Validator, Callable]], None] = None,
+    validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> datetime.timedelta:
+) -> tortoise.fields.base.Field[datetime.timedelta]:
     """
     A field for storing time differences.
     """
 
 @overload
 def TimeDeltaField(
-    source_field: Union[str, None] = None,
+    source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[True],
     default: Any = None,
     unique: bool = False,
     index: bool = False,
-    description: Union[str, None] = None,
+    description: Optional[str] = None,
     model: "Optional[Model]" = None,
-    validators: Union[List[Union[tortoise.validators.Validator, Callable]], None] = None,
+    validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Union[datetime.timedelta, None]: ...
+) -> tortoise.fields.base.Field[typing.Optional[datetime.timedelta]]: ...
 @overload
 def TimeField(
     auto_now: bool = False, auto_now_add: bool = False, *, null: Literal[False] = False, **kwargs: Any
-) -> datetime.time:
+) -> tortoise.fields.base.Field[datetime.time]:
     """
     Time field.
     """
 
 @overload
 def TimeField(
     auto_now: bool = False, auto_now_add: bool = False, *, null: Literal[True], **kwargs: Any
-) -> Union[datetime.time, None]: ...
+) -> tortoise.fields.base.Field[typing.Optional[datetime.time]]: ...
 @overload
-def UUIDField(*, null: Literal[False] = False, **kwargs: Any) -> uuid.UUID:
+def UUIDField(*, null: Literal[False] = False, **kwargs: Any) -> tortoise.fields.base.Field[uuid.UUID]:
     """
     UUID Field
 
     This field can store uuid value.
 
     If used as a primary key, it will auto-generate a UUID4 by default.
     """
 
 @overload
-def UUIDField(*, null: Literal[True], **kwargs: Any) -> Union[uuid.UUID, None]: ...
-def ForeignKeyField(
-    model_name: str,
-    related_name: Union[str, None, Literal[False]] = None,
-    on_delete: str = "CASCADE",
-    db_constraint: bool = True,
-    **kwargs: Any,
-) -> Any: ...
-def OneToOneField(
-    model_name: str,
-    related_name: Union[str, None, Literal[False]] = None,
-    on_delete: str = "CASCADE",
-    db_constraint: bool = True,
-    **kwargs: Any,
-) -> Any: ...
+def UUIDField(*, null: Literal[True], **kwargs: Any) -> tortoise.fields.base.Field[typing.Optional[uuid.UUID]]: ...
```

