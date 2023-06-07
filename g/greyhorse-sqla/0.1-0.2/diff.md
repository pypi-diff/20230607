# Comparing `tmp/greyhorse_sqla-0.1.tar.gz` & `tmp/greyhorse_sqla-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse_sqla-0.1.tar", max compression
+gzip compressed data, was "greyhorse_sqla-0.2.tar", max compression
```

## Comparing `greyhorse_sqla-0.1.tar` & `greyhorse_sqla-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       96 2023-05-06 23:35:23.266980 greyhorse_sqla-0.1/greyhorse_sqla/__init__.py
--rw-r--r--   0        0        0     3254 2023-04-26 11:42:15.504046 greyhorse_sqla-0.1/greyhorse_sqla/config.py
--rw-r--r--   0        0        0     4266 2023-04-26 17:19:18.163605 greyhorse_sqla-0.1/greyhorse_sqla/containers.py
--rw-r--r--   0        0        0     5482 2023-05-06 23:38:34.825861 greyhorse_sqla-0.1/greyhorse_sqla/engine.py
--rw-r--r--   0        0        0     5138 2023-05-06 23:38:34.861859 greyhorse_sqla-0.1/greyhorse_sqla/factory.py
--rw-r--r--   0        0        0     9656 2023-05-06 20:40:59.938582 greyhorse_sqla-0.1/greyhorse_sqla/model.py
--rw-r--r--   0        0        0     1422 2023-05-06 20:57:55.966776 greyhorse_sqla-0.1/greyhorse_sqla/query.py
--rw-r--r--   0        0        0     8122 2023-05-06 20:39:27.389483 greyhorse_sqla-0.1/greyhorse_sqla/repository.py
--rw-r--r--   0        0        0     2874 2023-04-26 15:29:49.359126 greyhorse_sqla-0.1/greyhorse_sqla/resources.py
--rw-r--r--   0        0        0      237 2023-05-06 23:37:41.048322 greyhorse_sqla-0.1/greyhorse_sqla/translations.toml
--rw-r--r--   0        0        0     1444 2023-05-06 23:39:44.874752 greyhorse_sqla-0.1/pyproject.toml
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 greyhorse_sqla-0.1/PKG-INFO
+-rw-r--r--   0        0        0       96 2023-05-06 23:35:23.266980 greyhorse_sqla-0.2/greyhorse_sqla/__init__.py
+-rw-r--r--   0        0        0     3254 2023-04-26 11:42:15.504046 greyhorse_sqla-0.2/greyhorse_sqla/config.py
+-rw-r--r--   0        0        0     4266 2023-04-26 17:19:18.163605 greyhorse_sqla-0.2/greyhorse_sqla/containers.py
+-rw-r--r--   0        0        0     5421 2023-06-07 18:56:59.071498 greyhorse_sqla-0.2/greyhorse_sqla/engine.py
+-rw-r--r--   0        0        0     5138 2023-05-06 23:38:34.861859 greyhorse_sqla-0.2/greyhorse_sqla/factory.py
+-rw-r--r--   0        0        0     3155 2023-06-07 18:56:58.679510 greyhorse_sqla-0.2/greyhorse_sqla/model.py
+-rw-r--r--   0        0        0     1422 2023-05-06 20:57:55.966776 greyhorse_sqla-0.2/greyhorse_sqla/query.py
+-rw-r--r--   0        0        0    13372 2023-06-07 18:53:02.342965 greyhorse_sqla-0.2/greyhorse_sqla/repository.py
+-rw-r--r--   0        0        0     2874 2023-04-26 15:29:49.359126 greyhorse_sqla-0.2/greyhorse_sqla/resources.py
+-rw-r--r--   0        0        0      237 2023-05-06 23:37:41.048322 greyhorse_sqla-0.2/greyhorse_sqla/translations.toml
+-rw-r--r--   0        0        0     1444 2023-06-07 18:55:03.467141 greyhorse_sqla-0.2/pyproject.toml
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 greyhorse_sqla-0.2/PKG-INFO
```

### Comparing `greyhorse_sqla-0.1/greyhorse_sqla/config.py` & `greyhorse_sqla-0.2/greyhorse_sqla/config.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.1/greyhorse_sqla/containers.py` & `greyhorse_sqla-0.2/greyhorse_sqla/containers.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.1/greyhorse_sqla/engine.py` & `greyhorse_sqla-0.2/greyhorse_sqla/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import asyncio
 import sys
 import threading
 from abc import ABC, abstractmethod
 from contextlib import contextmanager, AbstractContextManager, asynccontextmanager, AbstractAsyncContextManager
 from datetime import timedelta
-from typing import Callable
 
-from sqlalchemy import create_engine as create_sync_engine
-from sqlalchemy.ext.asyncio import AsyncSession as SqlaAsyncSession, async_scoped_session, create_async_engine, async_sessionmaker
+from sqlalchemy.ext.asyncio import AsyncSession as SqlaAsyncSession, async_scoped_session, async_sessionmaker
 from sqlalchemy.orm import Session as SqlaSyncSession, scoped_session, sessionmaker
 
 from greyhorse_core.context import get_context
 from greyhorse_core.engines.base import SyncEngine, AsyncEngine
 from greyhorse_core.i18n import tr
 from greyhorse_core.logging import logger
 from greyhorse_sqla.config import SqlEngineType
@@ -51,15 +49,17 @@
 class SqlaSyncEngine(SyncEngine[SqlaSyncSession], SqlaEngine):
     def __init__(self, name: str, engine, db_type: SqlEngineType, timeout: timedelta):
         SyncEngine.__init__(self, name)
         SqlaEngine.__init__(self, engine, db_type, timeout)
 
         self._counter = 0
         self._lock = threading.Lock()
-        self._session_factory = sessionmaker(bind=engine, autoflush=False)
+        self._session_factory = sessionmaker(
+            bind=engine, autoflush=False, expire_on_commit=False,
+        )
         self._scoped_session = scoped_session(
             self._session_factory, scopefunc=lambda: get_context().session_id
         )
 
     @property
     def connection_class(self):
         return SqlaSyncSession
```

### Comparing `greyhorse_sqla-0.1/greyhorse_sqla/factory.py` & `greyhorse_sqla-0.2/greyhorse_sqla/factory.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.1/greyhorse_sqla/query.py` & `greyhorse_sqla-0.2/greyhorse_sqla/query.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.1/greyhorse_sqla/resources.py` & `greyhorse_sqla-0.2/greyhorse_sqla/resources.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.1/pyproject.toml` & `greyhorse_sqla-0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "greyhorse-sqla"
-version = "0.1"
+version = "0.2"
 description = "Greyhorse SqlAlchemy library"
 license = "MIT"
 repository = "https://gitlab.com/max-plutonium/greyhorse"
 authors = ["Max Plutonium <plutonium.max@gmail.com>"]
 maintainers = ["Max Plutonium <plutonium.max@gmail.com>"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `greyhorse_sqla-0.1/PKG-INFO` & `greyhorse_sqla-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greyhorse-sqla
-Version: 0.1
+Version: 0.2
 Summary: Greyhorse SqlAlchemy library
 Home-page: https://gitlab.com/max-plutonium/greyhorse
 License: MIT
 Author: Max Plutonium
 Author-email: plutonium.max@gmail.com
 Maintainer: Max Plutonium
 Maintainer-email: plutonium.max@gmail.com
@@ -17,13 +17,13 @@
 Provides-Extra: mysql
 Provides-Extra: pg
 Provides-Extra: sqlite
 Requires-Dist: aiomysql (>=0.1,<0.2) ; extra == "mysql"
 Requires-Dist: aiosqlite (>=0.18,<0.19) ; extra == "sqlite"
 Requires-Dist: alembic (>=1.10,<2.0)
 Requires-Dist: asyncpg (>=0.27,<0.28) ; extra == "pg"
-Requires-Dist: greyhorse-core (==0.1)
+Requires-Dist: greyhorse-core (==0.2)
 Requires-Dist: psycopg2 (>=2.9,<3.0) ; extra == "pg"
 Requires-Dist: pymysql[rsa] (>=1.0,<2.0) ; extra == "mysql"
 Requires-Dist: sqlalchemy-utils (>=0.41,<0.42)
 Requires-Dist: sqlalchemy[asyncio,mypy] (>=2.0,<3.0)
 Project-URL: Repository, https://gitlab.com/max-plutonium/greyhorse
```

