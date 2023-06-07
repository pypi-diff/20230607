# Comparing `tmp/FastApi-RESTful-0.4.3.tar.gz` & `tmp/fastapi_restful-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastApi-RESTful-0.4.3.tar", max compression
+gzip compressed data, was "fastapi_restful-0.4.4.tar", max compression
```

## Comparing `FastApi-RESTful-0.4.3.tar` & `fastapi_restful-0.4.4.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1081 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/LICENSE
--rw-r--r--   0        0        0     3597 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/README.md
--rw-r--r--   0        0        0      196 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/__init__.py
--rw-r--r--   0        0        0      845 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/api_model.py
--rw-r--r--   0        0        0     2488 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/api_settings.py
--rw-r--r--   0        0        0      846 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/camelcase.py
--rw-r--r--   0        0        0     6910 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/cbv.py
--rw-r--r--   0        0        0     1029 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/cbv_base.py
--rw-r--r--   0        0        0     1186 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/enums.py
--rw-r--r--   0        0        0     2246 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/guid_type.py
--rw-r--r--   0        0        0      726 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/inferring_router.py
--rw-r--r--   0        0        0      331 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/openapi.py
--rw-r--r--   0        0        0        0 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/py.typed
--rw-r--r--   0        0        0     5179 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/session.py
--rw-r--r--   0        0        0     3578 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/tasks.py
--rw-r--r--   0        0        0     6994 2022-02-12 20:17:27.176406 FastApi-RESTful-0.4.3/fastapi_restful/timing.py
--rw-r--r--   0        0        0     3118 2022-02-12 20:17:27.180406 FastApi-RESTful-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     4571 2022-02-12 20:18:34.788574 FastApi-RESTful-0.4.3/setup.py
--rw-r--r--   0        0        0     5494 2022-02-12 20:18:34.789099 FastApi-RESTful-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/LICENSE
+-rw-r--r--   0        0        0     3597 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/README.md
+-rw-r--r--   0        0        0      196 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/__init__.py
+-rw-r--r--   0        0        0      881 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/api_model.py
+-rw-r--r--   0        0        0     2518 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/api_settings.py
+-rw-r--r--   0        0        0      882 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/camelcase.py
+-rw-r--r--   0        0        0     6990 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/cbv.py
+-rw-r--r--   0        0        0     1045 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/cbv_base.py
+-rw-r--r--   0        0        0     1226 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/enums.py
+-rw-r--r--   0        0        0     2251 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/guid_type.py
+-rw-r--r--   0        0        0      245 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/inferring_router.py
+-rw-r--r--   0        0        0      367 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/openapi.py
+-rw-r--r--   0        0        0        0 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/py.typed
+-rw-r--r--   0        0        0     5205 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/session.py
+-rw-r--r--   0        0        0     3519 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/tasks.py
+-rw-r--r--   0        0        0     7113 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/timing.py
+-rw-r--r--   0        0        0     3272 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 fastapi_restful-0.4.4/PKG-INFO
```

### Comparing `FastApi-RESTful-0.4.3/LICENSE` & `fastapi_restful-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FastApi-RESTful-0.4.3/README.md` & `fastapi_restful-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 **Source Code**: <a href="https://github.com/yuval9313/fastapi-restful" target="_blank">https://github.com/yuval9313/fastapi-restful</a>
 
 Base on: <a href="https://github.com/dmontagu/fastapi-utils" target="_blank">https://github.com/dmontagu/fastapi-utils</a>
 
 ---
 
-<a href="https://fastapi.tiangolo.com">FastAPI</a> is a modern, fast web framework for building APIs with Python 3.6+.
+<a href="https://fastapi.tiangolo.com">FastAPI</a> is a modern, fast web framework for building APIs with Python 3.7+.
 
 But if you're here, you probably already knew that!
 
 ---
 
 ## Features
 
@@ -57,15 +57,15 @@
 * **CamelCase Conversions**: Convenience functions for converting strings from `snake_case` to `camelCase` or `PascalCase` and back
 * **GUID Type**: The provided GUID type makes it easy to use UUIDs as the primary keys for your database tables
 
 See the [docs](https://fastapi-restful.netlify.app/) for more details and examples. 
 
 ## Requirements
 
-This package is intended for use with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python 3.6+.
+This package is intended for use with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python 3.7+.
 
 ## Installation
 
 ```bash
 pip install fastapi-restful  # For basic slim package :)
 
 pip install fastapi-restful[session]  # To add sqlalchemy session maker
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
                        Quicker FastApi developing tools
   [https://img.shields.io/github/last-commit/yuval9313/fastapi-restful.svg]_
                          [Build_CI] [Netlify_status]
                  [Package_version] [Python_versions]_[License]
 --- **Documentation**: https://fastapi-restful.netlify.app **Source Code**:
 https://github.com/yuval9313/fastapi-restful Base on: https://github.com/
 dmontagu/fastapi-utils --- FastAPI is a modern, fast web framework for building
-APIs with Python 3.6+. But if you're here, you probably already knew that! --
+APIs with Python 3.7+. But if you're here, you probably already knew that! --
 - ## Features This package includes a number of utilities to help reduce
 boilerplate and reuse common functionality across projects: * **Resource
 Class**: Create CRUD with ease the OOP way with `Resource` base class that lets
 you implement methods quick. * **Class Based Views**: Stop repeating the same
 dependencies over and over in the signature of related endpoints. * **Response-
 Model Inferring Router**: Let FastAPI infer the `response_model` to use based
 on your return type annotation. * **Repeated Tasks**: Easily trigger periodic
@@ -25,11 +25,11 @@
 `StrEnum` and `CamelStrEnum` classes make string-valued enums easier to
 maintain * **CamelCase Conversions**: Convenience functions for converting
 strings from `snake_case` to `camelCase` or `PascalCase` and back * **GUID
 Type**: The provided GUID type makes it easy to use UUIDs as the primary keys
 for your database tables See the [docs](https://fastapi-restful.netlify.app/
 ) for more details and examples. ## Requirements This package is intended for
 use with any recent version of FastAPI (depending on `pydantic>=1.0`), and
-Python 3.6+. ## Installation ```bash pip install fastapi-restful # For basic
+Python 3.7+. ## Installation ```bash pip install fastapi-restful # For basic
 slim package :) pip install fastapi-restful[session] # To add sqlalchemy
 session maker pip install fastapi-restful[all] # For all the packages ``` ##
 License This project is licensed under the terms of the MIT license.
```

### Comparing `FastApi-RESTful-0.4.3/fastapi_restful/api_model.py` & `fastapi_restful-0.4.4/fastapi_restful/api_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import partial
 
 from pydantic import BaseConfig, BaseModel
 
 from .camelcase import snake2camel
```

### Comparing `FastApi-RESTful-0.4.3/fastapi_restful/api_settings.py` & `fastapi_restful-0.4.4/fastapi_restful/api_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 from functools import lru_cache
-from typing import Any, Dict
+from typing import Any
 
 from pydantic import BaseSettings
 
 
 class APISettings(BaseSettings):
     """
     This class enables the configuration of your FastAPI instance through the use of environment variables.
@@ -27,22 +29,22 @@
     title: str = "FastAPI"
     version: str = "0.1.0"
 
     # Custom settings
     disable_docs: bool = False
 
     @property
-    def fastapi_kwargs(self) -> Dict[str, Any]:
+    def fastapi_kwargs(self) -> dict[str, Any]:
         """
         This returns a dictionary of the most commonly used keyword arguments when initializing a FastAPI instance
 
         If `self.disable_docs` is True, the various docs-related arguments are disabled, preventing your spec from being
         published.
         """
-        fastapi_kwargs: Dict[str, Any] = {
+        fastapi_kwargs: dict[str, Any] = {
             "debug": self.debug,
             "docs_url": self.docs_url,
             "openapi_prefix": self.openapi_prefix,
             "openapi_url": self.openapi_url,
             "redoc_url": self.redoc_url,
             "title": self.title,
             "version": self.version,
```

### Comparing `FastApi-RESTful-0.4.3/fastapi_restful/camelcase.py` & `fastapi_restful-0.4.4/fastapi_restful/camelcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 
 
 def snake2camel(snake: str, start_lower: bool = False) -> str:
     """
     Converts a snake_case string to camelCase.
```

### Comparing `FastApi-RESTful-0.4.3/fastapi_restful/cbv.py` & `fastapi_restful-0.4.4/fastapi_restful/cbv.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,23 +88,25 @@
 def _register_endpoints(router: APIRouter, cls: Type[Any], *urls: str) -> None:
     cbv_router = APIRouter()
     function_members = inspect.getmembers(cls, inspect.isfunction)
     for url in urls:
         _allocate_routes_by_method_name(router, url, function_members)
     router_roles = []
     for route in router.routes:
-        assert isinstance(route, APIRoute)
+        if not isinstance(route, APIRoute):
+            raise ValueError("The provided routes should be of type APIRoute")
+
         route_methods: Any = route.methods
         cast(Tuple[Any], route_methods)
         router_roles.append((route.path, tuple(route_methods)))
 
     if len(set(router_roles)) != len(router_roles):
         raise Exception("An identical route role has been implemented more then once")
 
-    functions_set = set(func for _, func in function_members)
+    functions_set = {func for _, func in function_members}
     cbv_routes = [
         route
         for route in router.routes
         if isinstance(route, (Route, WebSocketRoute)) and route.endpoint in functions_set
     ]
     prefix_length = len(router.prefix)  # Until 'black' would fix an issue which causes PEP8: E203
     for route in cbv_routes:
```

### Comparing `FastApi-RESTful-0.4.3/fastapi_restful/cbv_base.py` & `fastapi_restful-0.4.4/fastapi_restful/cbv_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 
 
 def take_init_parameters(cls: Any) -> Any:
     setattr(cls, INCLUDE_INIT_PARAMS_KEY, True)
     return cls
 
 
-def set_responses(response: Any, status_code: int = 200, responses: Dict[str, Any] = None, **kwargs: Any) -> Any:
+def set_responses(
+    response: Any, status_code: int = 200, responses: Optional[Dict[str, Any]] = None, **kwargs: Any
+) -> Any:
     def decorator(func: Any) -> Any:
         def get_responses() -> Tuple[Any, int, Optional[Dict[str, Any]], Optional[Any]]:
             return response, status_code, responses, kwargs
 
         setattr(func, RETURN_TYPES_FUNC_KEY, get_responses)
         return func
```

### Comparing `FastApi-RESTful-0.4.3/fastapi_restful/enums.py` & `fastapi_restful-0.4.4/fastapi_restful/enums.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,37 @@
+from __future__ import annotations
+
 from enum import Enum
+from typing import List
 
 from .camelcase import snake2camel
 
 
 class StrEnum(str, Enum):
     """
     StrEnum subclasses that create variants using `auto()` will have values equal to their names
     Enums inheriting from this class that set values using `enum.auto()` will have variant values equal to their names
     """
 
-    # noinspection PyMethodParameters
-    def _generate_next_value_(name, start, count, last_values) -> str:  # type: ignore
+    @staticmethod
+    def _generate_next_value_(name: str, start: int, count: int, last_values: List[str]) -> str:
         """
         Uses the name as the automatic value, rather than an integer
 
         See https://docs.python.org/3/library/enum.html#using-automatic-values for reference
         """
         return name
 
 
 class CamelStrEnum(str, Enum):
     """
     CamelStrEnum subclasses that create variants using `auto()` will have values equal to their camelCase names
     """
 
-    # noinspection PyMethodParameters
-    def _generate_next_value_(name, start, count, last_values) -> str:  # type: ignore
+    @staticmethod
+    def _generate_next_value_(name: str, start: int, count: int, last_values: List[str]) -> str:
         """
         Uses the camelCase name as the automatic value, rather than an integer
 
         See https://docs.python.org/3/library/enum.html#using-automatic-values for reference
         """
         return snake2camel(name, start_lower=True)
```

### Comparing `FastApi-RESTful-0.4.3/fastapi_restful/guid_type.py` & `fastapi_restful-0.4.4/fastapi_restful/guid_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# TODO: Add tests for postgres
+from __future__ import annotations
+
 import uuid
 from typing import TYPE_CHECKING, no_type_check
 
 import sqlalchemy as sa
 from sqlalchemy.dialects.postgresql.base import UUID
 from sqlalchemy.sql.sqltypes import CHAR
 from sqlalchemy.sql.type_api import TypeDecorator
```

### Comparing `FastApi-RESTful-0.4.3/fastapi_restful/session.py` & `fastapi_restful-0.4.4/fastapi_restful/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
+from collections.abc import Iterator
 from contextlib import contextmanager
-from typing import Iterator, Optional
 
 import sqlalchemy as sa
 from sqlalchemy.orm import Session
 
 
 class FastAPISessionMaker:
     """
@@ -22,16 +24,16 @@
 
             "<scheme>://<user>:<password>@<host>:<port>/<database>"
 
         A concrete example looks like "postgresql://db_user:password@db:5432/app"
         """
         self.database_uri = database_uri
 
-        self._cached_engine: Optional[sa.engine.Engine] = None
-        self._cached_sessionmaker: Optional[sa.orm.sessionmaker] = None
+        self._cached_engine: sa.engine.Engine | None = None
+        self._cached_sessionmaker: sa.orm.sessionmaker | None = None
 
     @property
     def cached_engine(self) -> sa.engine.Engine:
         """
         Returns a lazily-cached sqlalchemy engine for the instance's database_uri.
         """
         engine = self._cached_engine
@@ -53,15 +55,15 @@
 
     def get_new_engine(self) -> sa.engine.Engine:
         """
         Returns a new sqlalchemy engine using the instance's database_uri.
         """
         return get_engine(self.database_uri)
 
-    def get_new_sessionmaker(self, engine: Optional[sa.engine.Engine]) -> sa.orm.sessionmaker:
+    def get_new_sessionmaker(self, engine: sa.engine.Engine | None) -> sa.orm.sessionmaker:
         """
         Returns a new sessionmaker for the provided sqlalchemy engine. If no engine is provided, the
         instance's (lazily-cached) engine is used.
         """
         engine = engine or self.cached_engine
         return get_sessionmaker_for_engine(engine)
```

### Comparing `FastApi-RESTful-0.4.3/fastapi_restful/timing.py` & `fastapi_restful-0.4.4/fastapi_restful/timing.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,34 @@
 
 The middleware from this module is intended for use during both development and production,
 but only reports timing data at the granularity of individual endpoint calls.
 
 For more detailed performance investigations (during development only, due to added overhead),
 consider using the coroutine-aware profiling library `yappi`.
 """
+from __future__ import annotations
+
 import os
 import time
-from typing import Any, Callable, Optional
+from collections.abc import Callable
+from typing import Any
 
 import psutil
 from fastapi import FastAPI
 from starlette.middleware.base import RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.responses import Response
 from starlette.routing import Match, Mount
 from starlette.types import Scope
 
 TIMER_ATTRIBUTE = "__fastapi_utils_timer__"
 
 
 def add_timing_middleware(
-    app: FastAPI, record: Optional[Callable[[str], None]] = None, prefix: str = "", exclude: Optional[str] = None
+    app: FastAPI, record: Callable[[str], None] | None = None, prefix: str = "", exclude: str | None = None
 ) -> None:
     """
     Adds a middleware to the provided `app` that records timing metrics using the provided `record` callable.
 
     Typically `record` would be something like `logger.info` for a `logging.Logger` instance.
 
     The provided `prefix` is used when generating route names.
@@ -45,26 +48,27 @@
         metric_name = metric_namer(request.scope)
         with _TimingStats(metric_name, record=record, exclude=exclude) as timer:
             setattr(request.state, TIMER_ATTRIBUTE, timer)
             response = await call_next(request)
         return response
 
 
-def record_timing(request: Request, note: Optional[str] = None) -> None:
+def record_timing(request: Request, note: str | None = None) -> None:
     """
     Call this function at any point that you want to display elapsed time during the handling of a single request
 
     This can help profile which piece of a request is causing a performance bottleneck.
 
     Note that for this function to succeed, the request should have been generated by a FastAPI app
     that has had timing middleware added using the `fastapi_utils.timing.add_timing_middleware` function.
     """
     timer = getattr(request.state, TIMER_ATTRIBUTE, None)
     if timer is not None:
-        assert isinstance(timer, _TimingStats)
+        if not isinstance(timer, _TimingStats):
+            raise ValueError("Timer should be of an instance of TimingStats")
         timer.emit(note)
     else:
         raise ValueError("No timer present on request")
 
 
 class _TimingStats:
     """
@@ -78,15 +82,15 @@
         The callable to call on generated messages. Defaults to `print`, but typically
         something like `logger.info` for a `logging.Logger` instance would be preferable.
     exclude:
         An optional string; if it is not None and occurs inside `name`, no stats will be emitted
     """
 
     def __init__(
-        self, name: Optional[str] = None, record: Callable[[str], None] = None, exclude: Optional[str] = None
+        self, name: str | None = None, record: Callable[[str], None] | None = None, exclude: str | None = None
     ) -> None:
         self.name = name
         self.record = record or print
 
         self.process: psutil.Process = psutil.Process(os.getpid())
         self.start_time: float = 0
         self.start_cpu_time: float = 0
@@ -109,22 +113,22 @@
     def time(self) -> float:
         return self.end_time - self.start_time
 
     @property
     def cpu_time(self) -> float:
         return self.end_cpu_time - self.start_cpu_time
 
-    def __enter__(self) -> "_TimingStats":
+    def __enter__(self) -> _TimingStats:
         self.start()
         return self
 
     def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
         self.emit()
 
-    def emit(self, note: Optional[str] = None) -> None:
+    def emit(self, note: str | None = None) -> None:
         """
         Emit timing information, optionally including a specified note
         """
         if not self.silent:
             self.take_split()
             cpu_ms = 1000 * self.cpu_time
             wall_ms = 1000 * self.time
```

### Comparing `FastApi-RESTful-0.4.3/pyproject.toml` & `fastapi_restful-0.4.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
-name = "FastApi-RESTful"
-version = "0.4.3"
+name = "fastapi-restful"
+version = "0.4.4"
 description = "Quicker FastApi developing tools"
 license = "MIT"
-authors = ["Yuval Levi"]
+authors = ["Yuval Levi <yuvall9313@gmail.com>"]
 readme = "README.md"
 homepage = "https://fastapi-restful.netlify.app"
 repository = "https://github.com/yuval9313/fastapi-utils"
 documentation = "https://fastapi-restful.netlify.app"
 keywords = ["fastapi", "OOP", "RESTful"]
 classifiers = [
     "Intended Audience :: Information Technology",
@@ -24,65 +24,55 @@
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Framework :: FastAPI",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.7"
 
-dataclasses = {version = "^0.8", python = "~3.6.2"}
-fastapi = "^0"
-pydantic = "^1"
-sqlalchemy =  { version = "^1", optional = true }
+fastapi = "^0.89"
+pydantic = "^1.0,<2.0"
+sqlalchemy =  { version = "^1.4,<2.0", optional = true }
 psutil = "^5"
 
 [tool.poetry.dev-dependencies]
 # Starlette features
-wheel = "*"
 aiofiles = "*"  # Serving static files
-requests = "*"  # TestClient
+httpx = "*"  # TestClient
 
 # Testing
 pytest = "^7.0"
 pytest-cov = "*"
 pytest-asyncio = "*"
+coverage = "*"
 
-# Python 3.6 Testing
-async-exit-stack = { version = "*", python = "~3.6" }
-async-generator = { version = "*", python = "~3.6" }
-types-dataclasses = { version = "*", python = "~3.6" }
-
-
-# CI
-codecov = "*"
 
 # Static
-isort = "*"
-autoflake = "*"
+ruff = "*"
 black = { version = "*", allow-prereleases = true }
-flake8 = "*"
 mypy = "*"
 sqlalchemy-stubs = "*"
 
 # Documentation
 mkdocs = "*"
 mkdocs-material = "*"
 markdown-include = "*"
+autoflake = "^1.4"
 
 [tool.poetry.extras]
 all = ["sqlalchemy"]
 session = ["sqlalchemy"]
 
 [tool.black]
 line-length = 120
@@ -96,21 +86,19 @@
     | \.pytest_cache
     | htmlcov
     | build
   )/
 )
 '''
 
-[tool.isort]
-line_length = 120
-known_first_party = ["fastapi-utils", "tests"]
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-combine_as_imports = true
+[tool.ruff]
+line-length = 120
+extend-select = ['RUF100', 'C90', 'I']
+isort = { known-first-party = ['FastApi-RESTful', 'tests'] }
+
 
 [tool.coverage.run]
 source = ["fastapi_restful"]
 branch = true
 
 [tool.coverage.report]
 precision = 2
@@ -119,13 +107,30 @@
     "raise NotImplementedError",
     "raise NotImplemented",
     "@overload",
     "if TYPE_CHECKING:",
     'if __name__ == "__main__":'
 ]
 
+[tool.pytest.ini_options]
+testpaths = "tests"
+filterwarnings = "ignore:.*The explicit passing of coroutine objects to asyncio.wait()*:DeprecationWarning"
+
+
+[tool.mypy]
+plugins = "pydantic.mypy,sqlmypy"
+
+follow_imports = "silent"
+strict_optional = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+disallow_any_generics = true
+check_untyped_defs = true
+ignore_missing_imports = true
+disallow_untyped_defs = true
+
 [tool.poetry-version-plugin]
 source = "init"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
-build-backend = "poetry.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `FastApi-RESTful-0.4.3/PKG-INFO` & `fastapi_restful-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: fastapi-restful
-Version: 0.4.3
+Version: 0.4.4
 Summary: Quicker FastApi developing tools
 Home-page: https://fastapi-restful.netlify.app
 License: MIT
 Keywords: fastapi,OOP,RESTful
 Author: Yuval Levi
-Requires-Python: >=3.6.2,<4.0.0
+Author-email: yuvall9313@gmail.com
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: all
 Provides-Extra: session
-Requires-Dist: dataclasses (>=0.8,<0.9); python_full_version >= "3.6.2" and python_full_version < "3.7.0"
-Requires-Dist: fastapi (>=0,<1)
+Requires-Dist: fastapi (>=0.89,<0.90)
 Requires-Dist: psutil (>=5,<6)
-Requires-Dist: pydantic (>=1,<2)
-Requires-Dist: sqlalchemy (>=1,<2); extra == "all" or extra == "session"
+Requires-Dist: pydantic (>=1.0,<2.0)
+Requires-Dist: sqlalchemy (>=1.4,<2.0) ; extra == "all" or extra == "session"
 Project-URL: Documentation, https://fastapi-restful.netlify.app
 Project-URL: Repository, https://github.com/yuval9313/fastapi-utils
 Description-Content-Type: text/markdown
 
 <p align="center">
     <em>Quicker FastApi developing tools</em>
 </p>
@@ -70,15 +70,15 @@
 
 **Source Code**: <a href="https://github.com/yuval9313/fastapi-restful" target="_blank">https://github.com/yuval9313/fastapi-restful</a>
 
 Base on: <a href="https://github.com/dmontagu/fastapi-utils" target="_blank">https://github.com/dmontagu/fastapi-utils</a>
 
 ---
 
-<a href="https://fastapi.tiangolo.com">FastAPI</a> is a modern, fast web framework for building APIs with Python 3.6+.
+<a href="https://fastapi.tiangolo.com">FastAPI</a> is a modern, fast web framework for building APIs with Python 3.7+.
 
 But if you're here, you probably already knew that!
 
 ---
 
 ## Features
 
@@ -102,15 +102,15 @@
 * **CamelCase Conversions**: Convenience functions for converting strings from `snake_case` to `camelCase` or `PascalCase` and back
 * **GUID Type**: The provided GUID type makes it easy to use UUIDs as the primary keys for your database tables
 
 See the [docs](https://fastapi-restful.netlify.app/) for more details and examples. 
 
 ## Requirements
 
-This package is intended for use with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python 3.6+.
+This package is intended for use with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python 3.7+.
 
 ## Installation
 
 ```bash
 pip install fastapi-restful  # For basic slim package :)
 
 pip install fastapi-restful[session]  # To add sqlalchemy session maker
```

#### html2text {}

```diff
@@ -1,41 +1,39 @@
-Metadata-Version: 2.1 Name: fastapi-restful Version: 0.4.3 Summary: Quicker
+Metadata-Version: 2.1 Name: fastapi-restful Version: 0.4.4 Summary: Quicker
 FastApi developing tools Home-page: https://fastapi-restful.netlify.app
-License: MIT Keywords: fastapi,OOP,RESTful Author: Yuval Levi Requires-Python:
->=3.6.2,<4.0.0 Classifier: Development Status :: 4 - Beta Classifier:
-Environment :: Web Environment Classifier: Framework :: AsyncIO Classifier:
-Framework :: FastAPI Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Information Technology Classifier: Intended Audience ::
-System Administrators Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic
-:: Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Software
-Development Classifier: Topic :: Software Development :: Libraries Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Classifier: Topic
-:: Utilities Classifier: Typing :: Typed Provides-Extra: all Provides-Extra:
-session Requires-Dist: dataclasses (>=0.8,<0.9); python_full_version >= "3.6.2"
-and python_full_version < "3.7.0" Requires-Dist: fastapi (>=0,<1) Requires-
-Dist: psutil (>=5,<6) Requires-Dist: pydantic (>=1,<2) Requires-Dist:
-sqlalchemy (>=1,<2); extra == "all" or extra == "session" Project-URL:
-Documentation, https://fastapi-restful.netlify.app Project-URL: Repository,
-https://github.com/yuval9313/fastapi-utils Description-Content-Type: text/
-markdown
+License: MIT Keywords: fastapi,OOP,RESTful Author: Yuval Levi Author-email:
+yuvall9313@gmail.com Requires-Python: >=3.7,<4.0 Classifier: Development Status
+:: 4 - Beta Classifier: Environment :: Web Environment Classifier: Framework ::
+AsyncIO Classifier: Framework :: FastAPI Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Information Technology Classifier:
+Intended Audience :: System Administrators Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic ::
+Software Development Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities Classifier: Typing :: Typed Provides-Extra: all
+Provides-Extra: session Requires-Dist: fastapi (>=0.89,<0.90) Requires-Dist:
+psutil (>=5,<6) Requires-Dist: pydantic (>=1.0,<2.0) Requires-Dist: sqlalchemy
+(>=1.4,<2.0) ; extra == "all" or extra == "session" Project-URL: Documentation,
+https://fastapi-restful.netlify.app Project-URL: Repository, https://
+github.com/yuval9313/fastapi-utils Description-Content-Type: text/markdown
                        Quicker FastApi developing tools
   [https://img.shields.io/github/last-commit/yuval9313/fastapi-restful.svg]_
                          [Build_CI] [Netlify_status]
                  [Package_version] [Python_versions]_[License]
 --- **Documentation**: https://fastapi-restful.netlify.app **Source Code**:
 https://github.com/yuval9313/fastapi-restful Base on: https://github.com/
 dmontagu/fastapi-utils --- FastAPI is a modern, fast web framework for building
-APIs with Python 3.6+. But if you're here, you probably already knew that! --
+APIs with Python 3.7+. But if you're here, you probably already knew that! --
 - ## Features This package includes a number of utilities to help reduce
 boilerplate and reuse common functionality across projects: * **Resource
 Class**: Create CRUD with ease the OOP way with `Resource` base class that lets
 you implement methods quick. * **Class Based Views**: Stop repeating the same
 dependencies over and over in the signature of related endpoints. * **Response-
 Model Inferring Router**: Let FastAPI infer the `response_model` to use based
 on your return type annotation. * **Repeated Tasks**: Easily trigger periodic
@@ -51,11 +49,11 @@
 `StrEnum` and `CamelStrEnum` classes make string-valued enums easier to
 maintain * **CamelCase Conversions**: Convenience functions for converting
 strings from `snake_case` to `camelCase` or `PascalCase` and back * **GUID
 Type**: The provided GUID type makes it easy to use UUIDs as the primary keys
 for your database tables See the [docs](https://fastapi-restful.netlify.app/
 ) for more details and examples. ## Requirements This package is intended for
 use with any recent version of FastAPI (depending on `pydantic>=1.0`), and
-Python 3.6+. ## Installation ```bash pip install fastapi-restful # For basic
+Python 3.7+. ## Installation ```bash pip install fastapi-restful # For basic
 slim package :) pip install fastapi-restful[session] # To add sqlalchemy
 session maker pip install fastapi-restful[all] # For all the packages ``` ##
 License This project is licensed under the terms of the MIT license.
```

