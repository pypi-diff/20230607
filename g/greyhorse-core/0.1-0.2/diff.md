# Comparing `tmp/greyhorse_core-0.1.tar.gz` & `tmp/greyhorse_core-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse_core-0.1.tar", max compression
+gzip compressed data, was "greyhorse_core-0.2.tar", max compression
```

## Comparing `greyhorse_core-0.1.tar` & `greyhorse_core-0.2.tar`

### file list

```diff
@@ -1,68 +1,42 @@
--rw-r--r--   0        0        0        0 2023-04-24 18:05:03.042538 greyhorse_core-0.1/greyhorse_core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 18:45:18.959739 greyhorse_core-0.1/greyhorse_core/app/__init__.py
--rw-r--r--   0        0        0      179 2023-04-26 16:01:41.328606 greyhorse_core-0.1/greyhorse_core/app/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6557 2023-05-06 14:50:51.286361 greyhorse_core-0.1/greyhorse_core/app/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     6377 2023-04-24 20:21:29.479688 greyhorse_core-0.1/greyhorse_core/app/application.py
--rw-r--r--   0        0        0     2576 2023-04-26 18:21:39.345299 greyhorse_core-0.1/greyhorse_core/app/base.py
--rw-r--r--   0        0        0     7745 2023-04-24 20:21:29.311692 greyhorse_core-0.1/greyhorse_core/app/module.py
--rw-r--r--   0        0        0     4195 2023-04-24 20:21:28.631707 greyhorse_core-0.1/greyhorse_core/app/service.py
--rw-r--r--   0        0        0       57 2023-04-24 20:21:28.679706 greyhorse_core-0.1/greyhorse_core/context/__init__.py
--rw-r--r--   0        0        0      294 2023-04-24 20:37:09.254223 greyhorse_core-0.1/greyhorse_core/context/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4529 2023-04-24 20:39:34.799071 greyhorse_core-0.1/greyhorse_core/context/__pycache__/data.cpython-311.pyc
--rw-r--r--   0        0        0     1683 2023-04-24 20:39:33.731147 greyhorse_core-0.1/greyhorse_core/context/data.py
--rw-r--r--   0        0        0        0 2023-04-24 19:30:35.532333 greyhorse_core-0.1/greyhorse_core/data/__init__.py
--rw-r--r--   0        0        0      180 2023-04-24 20:42:20.412021 greyhorse_core-0.1/greyhorse_core/data/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-04-24 19:32:47.064406 greyhorse_core-0.1/greyhorse_core/data/cache/__init__.py
--rw-r--r--   0        0        0      186 2023-04-24 20:42:20.416021 greyhorse_core-0.1/greyhorse_core/data/cache/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5140 2023-04-24 20:42:20.416021 greyhorse_core-0.1/greyhorse_core/data/cache/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     5486 2023-04-24 20:42:20.416021 greyhorse_core-0.1/greyhorse_core/data/cache/__pycache__/method.cpython-311.pyc
--rw-r--r--   0        0        0     1909 2023-04-24 20:21:29.083697 greyhorse_core-0.1/greyhorse_core/data/cache/base.py
--rw-r--r--   0        0        0     2467 2023-04-24 20:21:28.907701 greyhorse_core-0.1/greyhorse_core/data/cache/method.py
--rw-r--r--   0        0        0        0 2023-04-26 18:11:49.403523 greyhorse_core-0.1/greyhorse_core/data/models/__init__.py
--rw-r--r--   0        0        0      187 2023-05-06 14:52:53.455081 greyhorse_core-0.1/greyhorse_core/data/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4283 2023-05-06 20:27:17.984410 greyhorse_core-0.1/greyhorse_core/data/models/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     7237 2023-05-06 14:52:53.535079 greyhorse_core-0.1/greyhorse_core/data/models/__pycache__/fields.cpython-311.pyc
--rw-r--r--   0        0        0     6997 2023-05-06 20:27:17.984410 greyhorse_core-0.1/greyhorse_core/data/models/__pycache__/filterable.cpython-311.pyc
--rw-r--r--   0        0        0     8950 2023-05-06 20:27:17.988410 greyhorse_core-0.1/greyhorse_core/data/models/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     1878 2023-05-06 20:27:15.000505 greyhorse_core-0.1/greyhorse_core/data/models/base.py
--rw-r--r--   0        0        0     3621 2023-04-26 18:45:50.368589 greyhorse_core-0.1/greyhorse_core/data/models/fields.py
--rw-r--r--   0        0        0     3550 2023-05-06 20:27:15.116501 greyhorse_core-0.1/greyhorse_core/data/models/filterable.py
--rw-r--r--   0        0        0     4606 2023-05-06 20:27:14.836510 greyhorse_core-0.1/greyhorse_core/data/models/model.py
--rw-r--r--   0        0        0     1620 2023-04-26 18:40:56.383656 greyhorse_core-0.1/greyhorse_core/data/models/serializable.py
--rw-r--r--   0        0        0        0 2023-04-24 19:45:59.112951 greyhorse_core-0.1/greyhorse_core/data/repositories/__init__.py
--rw-r--r--   0        0        0      193 2023-05-06 14:52:53.535079 greyhorse_core-0.1/greyhorse_core/data/repositories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4877 2023-05-06 20:27:17.992410 greyhorse_core-0.1/greyhorse_core/data/repositories/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     2344 2023-05-06 20:27:17.992410 greyhorse_core-0.1/greyhorse_core/data/repositories/__pycache__/filterable.cpython-311.pyc
--rw-r--r--   0        0        0     2203 2023-05-06 20:27:15.184499 greyhorse_core-0.1/greyhorse_core/data/repositories/base.py
--rw-r--r--   0        0        0     1042 2023-05-06 20:27:15.380493 greyhorse_core-0.1/greyhorse_core/data/repositories/filterable.py
--rw-r--r--   0        0        0      117 2023-04-24 20:21:28.447712 greyhorse_core-0.1/greyhorse_core/data/serializers/__init__.py
--rw-r--r--   0        0        0      580 2023-04-24 20:21:28.335714 greyhorse_core-0.1/greyhorse_core/data/serializers/base.py
--rw-r--r--   0        0        0      523 2023-04-26 18:21:39.277304 greyhorse_core-0.1/greyhorse_core/data/serializers/pickle.py
--rw-r--r--   0        0        0        0 2023-04-25 12:15:10.040554 greyhorse_core-0.1/greyhorse_core/engines/__init__.py
--rw-r--r--   0        0        0      183 2023-04-26 11:47:46.345694 greyhorse_core-0.1/greyhorse_core/engines/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3597 2023-05-06 14:50:51.034368 greyhorse_core-0.1/greyhorse_core/engines/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     3095 2023-04-26 11:47:46.345694 greyhorse_core-0.1/greyhorse_core/engines/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     1451 2023-04-26 17:59:27.740179 greyhorse_core-0.1/greyhorse_core/engines/base.py
--rw-r--r--   0        0        0     1102 2023-04-25 12:36:12.576326 greyhorse_core-0.1/greyhorse_core/engines/factory.py
--rw-r--r--   0        0        0       67 2023-04-24 20:21:28.403712 greyhorse_core-0.1/greyhorse_core/i18n/__init__.py
--rw-r--r--   0        0        0      283 2023-04-24 20:37:09.234225 greyhorse_core-0.1/greyhorse_core/i18n/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6053 2023-05-06 23:36:15.712381 greyhorse_core-0.1/greyhorse_core/i18n/__pycache__/translator.cpython-311.pyc
--rw-r--r--   0        0        0     2798 2023-05-06 23:36:14.668431 greyhorse_core-0.1/greyhorse_core/i18n/translator.py
--rw-r--r--   0        0        0     1584 2023-04-24 20:21:28.723705 greyhorse_core-0.1/greyhorse_core/logging.py
--rw-r--r--   0        0        0     2340 2023-04-26 19:36:39.848852 greyhorse_core-0.1/greyhorse_core/result.py
--rw-r--r--   0        0        0        0 2023-04-24 18:46:51.552811 greyhorse_core-0.1/greyhorse_core/utils/__init__.py
--rw-r--r--   0        0        0      181 2023-04-24 20:37:09.254223 greyhorse_core-0.1/greyhorse_core/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1422 2023-04-26 16:01:40.864655 greyhorse_core-0.1/greyhorse_core/utils/__pycache__/confs.cpython-311.pyc
--rw-r--r--   0        0        0     4383 2023-04-24 20:37:09.258223 greyhorse_core-0.1/greyhorse_core/utils/__pycache__/dicts.cpython-311.pyc
--rw-r--r--   0        0        0     1419 2023-04-24 20:42:20.420021 greyhorse_core-0.1/greyhorse_core/utils/__pycache__/hashes.cpython-311.pyc
--rw-r--r--   0        0        0     1826 2023-05-06 14:59:29.548240 greyhorse_core-0.1/greyhorse_core/utils/__pycache__/invoke.cpython-311.pyc
--rw-r--r--   0        0        0      397 2023-04-24 20:21:29.039698 greyhorse_core-0.1/greyhorse_core/utils/confs.py
--rw-r--r--   0        0        0     2154 2023-04-24 20:21:29.255693 greyhorse_core-0.1/greyhorse_core/utils/dicts.py
--rw-r--r--   0        0        0      573 2023-04-24 20:21:28.247716 greyhorse_core-0.1/greyhorse_core/utils/hashes.py
--rw-r--r--   0        0        0      922 2023-04-26 18:21:39.397295 greyhorse_core-0.1/greyhorse_core/utils/imports.py
--rw-r--r--   0        0        0      865 2023-04-24 20:21:28.567709 greyhorse_core-0.1/greyhorse_core/utils/invoke.py
--rw-r--r--   0        0        0      452 2023-04-24 20:27:59.930714 greyhorse_core-0.1/greyhorse_core/utils/json.py
--rw-r--r--   0        0        0      568 2023-04-24 20:21:29.135696 greyhorse_core-0.1/greyhorse_core/utils/strings.py
--rw-r--r--   0        0        0     1101 2023-04-24 20:34:00.643458 greyhorse_core-0.1/greyhorse_core/utils/time.py
--rw-r--r--   0        0        0     1060 2023-05-06 23:39:44.926750 greyhorse_core-0.1/pyproject.toml
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 greyhorse_core-0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 18:05:03.042538 greyhorse_core-0.2/greyhorse_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 18:45:18.959739 greyhorse_core-0.2/greyhorse_core/app/__init__.py
+-rw-r--r--   0        0        0     6377 2023-04-24 20:21:29.479688 greyhorse_core-0.2/greyhorse_core/app/application.py
+-rw-r--r--   0        0        0     2576 2023-04-26 18:21:39.345299 greyhorse_core-0.2/greyhorse_core/app/base.py
+-rw-r--r--   0        0        0     7745 2023-04-24 20:21:29.311692 greyhorse_core-0.2/greyhorse_core/app/module.py
+-rw-r--r--   0        0        0     4195 2023-04-24 20:21:28.631707 greyhorse_core-0.2/greyhorse_core/app/service.py
+-rw-r--r--   0        0        0       57 2023-04-24 20:21:28.679706 greyhorse_core-0.2/greyhorse_core/context/__init__.py
+-rw-r--r--   0        0        0     1683 2023-04-24 20:39:33.731147 greyhorse_core-0.2/greyhorse_core/context/data.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:30:35.532333 greyhorse_core-0.2/greyhorse_core/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:32:47.064406 greyhorse_core-0.2/greyhorse_core/data/cache/__init__.py
+-rw-r--r--   0        0        0     1909 2023-04-24 20:21:29.083697 greyhorse_core-0.2/greyhorse_core/data/cache/base.py
+-rw-r--r--   0        0        0     2467 2023-04-24 20:21:28.907701 greyhorse_core-0.2/greyhorse_core/data/cache/method.py
+-rw-r--r--   0        0        0        0 2023-04-26 18:11:49.403523 greyhorse_core-0.2/greyhorse_core/data/models/__init__.py
+-rw-r--r--   0        0        0     1878 2023-05-06 20:27:15.000505 greyhorse_core-0.2/greyhorse_core/data/models/base.py
+-rw-r--r--   0        0        0     3621 2023-04-26 18:45:50.368589 greyhorse_core-0.2/greyhorse_core/data/models/fields.py
+-rw-r--r--   0        0        0     2088 2023-06-05 00:54:27.830750 greyhorse_core-0.2/greyhorse_core/data/models/filterable.py
+-rw-r--r--   0        0        0     4491 2023-06-07 18:56:58.759508 greyhorse_core-0.2/greyhorse_core/data/models/model.py
+-rw-r--r--   0        0        0     1620 2023-04-26 18:40:56.383656 greyhorse_core-0.2/greyhorse_core/data/models/serializable.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:45:59.112951 greyhorse_core-0.2/greyhorse_core/data/repositories/__init__.py
+-rw-r--r--   0        0        0     2752 2023-06-07 18:56:58.847505 greyhorse_core-0.2/greyhorse_core/data/repositories/base.py
+-rw-r--r--   0        0        0     2387 2023-06-07 18:56:58.927503 greyhorse_core-0.2/greyhorse_core/data/repositories/filterable.py
+-rw-r--r--   0        0        0      117 2023-04-24 20:21:28.447712 greyhorse_core-0.2/greyhorse_core/data/serializers/__init__.py
+-rw-r--r--   0        0        0      580 2023-04-24 20:21:28.335714 greyhorse_core-0.2/greyhorse_core/data/serializers/base.py
+-rw-r--r--   0        0        0      523 2023-04-26 18:21:39.277304 greyhorse_core-0.2/greyhorse_core/data/serializers/pickle.py
+-rw-r--r--   0        0        0        0 2023-04-25 12:15:10.040554 greyhorse_core-0.2/greyhorse_core/engines/__init__.py
+-rw-r--r--   0        0        0     1451 2023-04-26 17:59:27.740179 greyhorse_core-0.2/greyhorse_core/engines/base.py
+-rw-r--r--   0        0        0     1102 2023-04-25 12:36:12.576326 greyhorse_core-0.2/greyhorse_core/engines/factory.py
+-rw-r--r--   0        0        0       67 2023-04-24 20:21:28.403712 greyhorse_core-0.2/greyhorse_core/i18n/__init__.py
+-rw-r--r--   0        0        0     2798 2023-05-06 23:36:14.668431 greyhorse_core-0.2/greyhorse_core/i18n/translator.py
+-rw-r--r--   0        0        0     1584 2023-04-24 20:21:28.723705 greyhorse_core-0.2/greyhorse_core/logging.py
+-rw-r--r--   0        0        0     2340 2023-04-26 19:36:39.848852 greyhorse_core-0.2/greyhorse_core/result.py
+-rw-r--r--   0        0        0        0 2023-04-24 18:46:51.552811 greyhorse_core-0.2/greyhorse_core/utils/__init__.py
+-rw-r--r--   0        0        0      397 2023-04-24 20:21:29.039698 greyhorse_core-0.2/greyhorse_core/utils/confs.py
+-rw-r--r--   0        0        0     2154 2023-04-24 20:21:29.255693 greyhorse_core-0.2/greyhorse_core/utils/dicts.py
+-rw-r--r--   0        0        0      573 2023-04-24 20:21:28.247716 greyhorse_core-0.2/greyhorse_core/utils/hashes.py
+-rw-r--r--   0        0        0      922 2023-04-26 18:21:39.397295 greyhorse_core-0.2/greyhorse_core/utils/imports.py
+-rw-r--r--   0        0        0      865 2023-04-24 20:21:28.567709 greyhorse_core-0.2/greyhorse_core/utils/invoke.py
+-rw-r--r--   0        0        0      452 2023-04-24 20:27:59.930714 greyhorse_core-0.2/greyhorse_core/utils/json.py
+-rw-r--r--   0        0        0      823 2023-05-07 00:18:41.443382 greyhorse_core-0.2/greyhorse_core/utils/strings.py
+-rw-r--r--   0        0        0     1101 2023-04-24 20:34:00.643458 greyhorse_core-0.2/greyhorse_core/utils/time.py
+-rw-r--r--   0        0        0     1060 2023-06-07 18:55:02.811162 greyhorse_core-0.2/pyproject.toml
+-rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 greyhorse_core-0.2/PKG-INFO
```

### Comparing `greyhorse_core-0.1/greyhorse_core/app/application.py` & `greyhorse_core-0.2/greyhorse_core/app/application.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/app/base.py` & `greyhorse_core-0.2/greyhorse_core/app/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/app/module.py` & `greyhorse_core-0.2/greyhorse_core/app/module.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/app/service.py` & `greyhorse_core-0.2/greyhorse_core/app/service.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/context/data.py` & `greyhorse_core-0.2/greyhorse_core/context/data.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/data/cache/base.py` & `greyhorse_core-0.2/greyhorse_core/data/cache/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/data/cache/method.py` & `greyhorse_core-0.2/greyhorse_core/data/cache/method.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/data/models/base.py` & `greyhorse_core-0.2/greyhorse_core/data/models/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/data/models/fields.py` & `greyhorse_core-0.2/greyhorse_core/data/models/fields.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/data/models/model.py` & `greyhorse_core-0.2/greyhorse_core/data/models/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import asyncio
-from abc import ABC, abstractmethod
-from typing import Any, Mapping, Optional, Sequence, Set, TYPE_CHECKING, Tuple, TypeVar, Union, Self
+from abc import ABC
+from typing import Any, Mapping, Sequence, TYPE_CHECKING, Tuple, TypeVar, Self
 
 from pydantic.main import BaseModel as PydanticModel
 
 from .base import AbstractModel, IdType
 from .fields import ModelFieldsMixin
-from ..repositories.base import Repository
-from ...utils.invoke import is_awaitable
+
+if TYPE_CHECKING:
+    from ..repositories.base import ModelRepository
+
 
 CreateSchemaType = TypeVar('CreateSchemaType', bound=PydanticModel)
 UpdateSchemaType = TypeVar('UpdateSchemaType', bound=PydanticModel)
 
 
 class Model(AbstractModel[IdType], ModelFieldsMixin, ABC):
-    _repo: Repository[IdType, Self]
+    _repo: 'ModelRepository[IdType, Self]'
 
     @classmethod
-    def bind(cls, repository: Repository[IdType, Self]):
+    def bind(cls, repository: 'ModelRepository[IdType, Self]'):
         cls._repo = repository
 
     @classmethod
     async def construct(cls, data: Mapping[str, Any], **kwargs) -> Self:
-        result = cls._repo.model_factory(**data)
-        if is_awaitable(result):
-            return await result
-        return result
+        return await cls._repo.construct(data, **kwargs)
 
     @classmethod
     async def construct_all(cls, objects: Sequence[Mapping[str, Any] | None], **kwargs) -> Sequence[Self | None]:
         loop = asyncio.get_event_loop()
         awaitables = list()
 
         for data in objects:
```

### Comparing `greyhorse_core-0.1/greyhorse_core/data/models/serializable.py` & `greyhorse_core-0.2/greyhorse_core/data/models/serializable.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/data/serializers/base.py` & `greyhorse_core-0.2/greyhorse_core/data/serializers/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/data/serializers/pickle.py` & `greyhorse_core-0.2/greyhorse_core/data/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/engines/base.py` & `greyhorse_core-0.2/greyhorse_core/engines/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/engines/factory.py` & `greyhorse_core-0.2/greyhorse_core/engines/factory.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/i18n/translator.py` & `greyhorse_core-0.2/greyhorse_core/i18n/translator.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/logging.py` & `greyhorse_core-0.2/greyhorse_core/logging.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/result.py` & `greyhorse_core-0.2/greyhorse_core/result.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/utils/dicts.py` & `greyhorse_core-0.2/greyhorse_core/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/utils/hashes.py` & `greyhorse_core-0.2/greyhorse_core/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/utils/imports.py` & `greyhorse_core-0.2/greyhorse_core/utils/imports.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/utils/invoke.py` & `greyhorse_core-0.2/greyhorse_core/utils/invoke.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/greyhorse_core/utils/time.py` & `greyhorse_core-0.2/greyhorse_core/utils/time.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.1/pyproject.toml` & `greyhorse_core-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "greyhorse-core"
-version = "0.1"
+version = "0.2"
 description = "Greyhorse Core library"
 license = "MIT"
 repository = "https://gitlab.com/max-plutonium/greyhorse"
 authors = ["Max Plutonium <plutonium.max@gmail.com>"]
 maintainers = ["Max Plutonium <plutonium.max@gmail.com>"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `greyhorse_core-0.1/PKG-INFO` & `greyhorse_core-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greyhorse-core
-Version: 0.1
+Version: 0.2
 Summary: Greyhorse Core library
 Home-page: https://gitlab.com/max-plutonium/greyhorse
 License: MIT
 Author: Max Plutonium
 Author-email: plutonium.max@gmail.com
 Maintainer: Max Plutonium
 Maintainer-email: plutonium.max@gmail.com
```

