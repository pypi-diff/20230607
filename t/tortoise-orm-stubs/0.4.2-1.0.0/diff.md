# Comparing `tmp/tortoise_orm_stubs-0.4.2.tar.gz` & `tmp/tortoise_orm_stubs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_orm_stubs-0.4.2.tar", max compression
+gzip compressed data, was "tortoise_orm_stubs-1.0.0.tar", max compression
```

## Comparing `tortoise_orm_stubs-0.4.2.tar` & `tortoise_orm_stubs-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2022-09-22 00:21:21.676040 tortoise_orm_stubs-0.4.2/LICENSE
--rw-r--r--   0        0        0      511 2023-06-07 05:51:08.893037 tortoise_orm_stubs-0.4.2/README.md
--rw-r--r--   0        0        0     1060 2023-06-07 05:55:59.894774 tortoise_orm_stubs-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    13970 2023-06-07 05:55:45.824851 tortoise_orm_stubs-0.4.2/tortoise-stubs/fields/__init__.pyi
--rw-r--r--   0        0        0        8 2022-09-22 19:51:35.803221 tortoise_orm_stubs-0.4.2/tortoise-stubs/py.typed
--rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 tortoise_orm_stubs-0.4.2/setup.py
--rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 tortoise_orm_stubs-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-09-22 00:21:21.676040 tortoise_orm_stubs-1.0.0/LICENSE
+-rw-r--r--   0        0        0      511 2023-04-25 17:47:14.750054 tortoise_orm_stubs-1.0.0/README.md
+-rw-r--r--   0        0        0     1060 2023-04-25 13:12:52.836668 tortoise_orm_stubs-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13458 2023-04-25 16:51:11.673362 tortoise_orm_stubs-1.0.0/tortoise-stubs/fields/__init__.pyi
+-rw-r--r--   0        0        0        8 2022-09-22 19:51:35.803221 tortoise_orm_stubs-1.0.0/tortoise-stubs/py.typed
+-rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 tortoise_orm_stubs-1.0.0/setup.py
+-rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 tortoise_orm_stubs-1.0.0/PKG-INFO
```

### Comparing `tortoise_orm_stubs-0.4.2/LICENSE` & `tortoise_orm_stubs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise_orm_stubs-0.4.2/pyproject.toml` & `tortoise_orm_stubs-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tortoise-orm-stubs"
-version = "0.4.2"
+version = "1.0.0"
 description = "Type stubs that make tortoise-orm a lot easier to work with when using type checkers."
 packages = [{ include = "tortoise-stubs" }]
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Ovsyanka83/tortoise-orm-stubs"
```

### Comparing `tortoise_orm_stubs-0.4.2/tortoise-stubs/fields/__init__.pyi` & `tortoise_orm_stubs-1.0.0/tortoise-stubs/fields/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
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
@@ -58,24 +59,14 @@
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
 def BigIntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> tortoise.fields.base.Field[int]:
     """
     Big integer field. (64-bit signed)
 
     ``pk`` (bool):
```

### Comparing `tortoise_orm_stubs-0.4.2/setup.py` & `tortoise_orm_stubs-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'], 'tortoise-stubs': ['fields/*']}
 
 install_requires = \
 ['tortoise-orm']
 
 setup_kwargs = {
     'name': 'tortoise-orm-stubs',
-    'version': '0.4.2',
+    'version': '1.0.0',
     'description': 'Type stubs that make tortoise-orm a lot easier to work with when using type checkers.',
     'long_description': "# tortoise-orm-stubs\n\nType stubs that make **tortoise-orm** a bit easier to work with when using type checkers.\n\nSpecifically, data fields' types automatically reflect the value of null argument (i.e. become optional if you set null=True)\n\n## Installation\n\n`pip install tortoise-orm-stubs`\n\n## Disclaimer\n\nPreviously **tortoise-orm-stubs** provided a lot more value but now the majority of its functionality has become a part of **tortoise-orm**. Hopefully, it will become completely unnecessary in the future.\n",
     'author': 'Stanislav Zmiev',
     'author_email': 'szmiev2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Ovsyanka83/tortoise-orm-stubs',
```

### Comparing `tortoise_orm_stubs-0.4.2/PKG-INFO` & `tortoise_orm_stubs-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-orm-stubs
-Version: 0.4.2
+Version: 1.0.0
 Summary: Type stubs that make tortoise-orm a lot easier to work with when using type checkers.
 Home-page: https://github.com/Ovsyanka83/tortoise-orm-stubs
 License: MIT
 Author: Stanislav Zmiev
 Author-email: szmiev2000@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

