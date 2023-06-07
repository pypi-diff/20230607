# Comparing `tmp/blackline-postgres-0.1.0a1.tar.gz` & `tmp/blackline-postgres-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackline-postgres-0.1.0a1.tar", last modified: Tue Mar 14 15:01:59 2023, max compression
+gzip compressed data, was "blackline-postgres-0.1.1a0.tar", last modified: Wed Jun  7 13:00:17 2023, max compression
```

## Comparing `blackline-postgres-0.1.0a1.tar` & `blackline-postgres-0.1.1a0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:59.243106 blackline-postgres-0.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-14 15:01:59.243106 blackline-postgres-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-14 15:01:45.000000 blackline-postgres-0.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:59.243106 blackline-postgres-0.1.0a1/blackline/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-14 15:01:45.000000 blackline-postgres-0.1.0a1/blackline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:59.243106 blackline-postgres-0.1.0a1/blackline/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:45.000000 blackline-postgres-0.1.0a1/blackline/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-14 15:01:45.000000 blackline-postgres-0.1.0a1/blackline/adapters/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:59.243106 blackline-postgres-0.1.0a1/blackline/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:45.000000 blackline-postgres-0.1.0a1/blackline/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-14 15:01:45.000000 blackline-postgres-0.1.0a1/blackline/models/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:59.243106 blackline-postgres-0.1.0a1/blackline_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-14 15:01:59.000000 blackline-postgres-0.1.0a1/blackline_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:01:59.000000 blackline-postgres-0.1.0a1/blackline_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 15:01:59.000000 blackline-postgres-0.1.0a1/blackline_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-14 15:01:59.000000 blackline-postgres-0.1.0a1/blackline_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-14 15:01:59.000000 blackline-postgres-0.1.0a1/blackline_postgres.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-14 15:01:59.243106 blackline-postgres-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 15:01:45.000000 blackline-postgres-0.1.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:59.243106 blackline-postgres-0.1.0a1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:59.243106 blackline-postgres-0.1.0a1/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-14 15:01:45.000000 blackline-postgres-0.1.0a1/tests/adapters/test_postgres_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-03-14 15:01:45.000000 blackline-postgres-0.1.0a1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:59.243106 blackline-postgres-0.1.0a1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-14 15:01:45.000000 blackline-postgres-0.1.0a1/tests/models/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-14 15:01:45.000000 blackline-postgres-0.1.0a1/tests/test_postgrest_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.960065 blackline-postgres-0.1.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 13:00:17.960065 blackline-postgres-0.1.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.948064 blackline-postgres-0.1.1a0/blackline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.948064 blackline-postgres-0.1.1a0/blackline/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.956065 blackline-postgres-0.1.1a0/blackline/adapters/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/blackline/adapters/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/blackline/adapters/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.948064 blackline-postgres-0.1.1a0/blackline/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.956065 blackline-postgres-0.1.1a0/blackline/models/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/blackline/models/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/blackline/models/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.960065 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 13:00:17.000000 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-07 13:00:17.000000 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:00:17.000000 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-07 13:00:17.000000 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 13:00:17.000000 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-07 13:00:17.960065 blackline-postgres-0.1.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.956065 blackline-postgres-0.1.1a0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.952064 blackline-postgres-0.1.1a0/tests/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.956065 blackline-postgres-0.1.1a0/tests/adapters/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/tests/adapters/postgres/test_postgres_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.952064 blackline-postgres-0.1.1a0/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.956065 blackline-postgres-0.1.1a0/tests/models/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/tests/models/postgres/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/tests/test_postgrest_integration.py
```

### Comparing `blackline-postgres-0.1.0a1/PKG-INFO` & `blackline-postgres-0.1.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackline-postgres
-Version: 0.1.0a1
+Version: 0.1.1a0
 Summary: Manage personal data in your data stores.
 Home-page: https://github.com/blacklinedata/blackline-core/tree/main/blackline/postgres
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `blackline-postgres-0.1.0a1/blackline/models/postgres.py` & `blackline-postgres-0.1.1a0/blackline/models/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `blackline-postgres-0.1.0a1/blackline_postgres.egg-info/PKG-INFO` & `blackline-postgres-0.1.1a0/blackline_postgres.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackline-postgres
-Version: 0.1.0a1
+Version: 0.1.1a0
 Summary: Manage personal data in your data stores.
 Home-page: https://github.com/blacklinedata/blackline-core/tree/main/blackline/postgres
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `blackline-postgres-0.1.0a1/blackline_postgres.egg-info/SOURCES.txt` & `blackline-postgres-0.1.1a0/blackline_postgres.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 README.md
 setup.cfg
 setup.py
-./blackline/__init__.py
-./blackline/adapters/__init__.py
-./blackline/adapters/postgres.py
-./blackline/models/__init__.py
-./blackline/models/postgres.py
+./blackline/adapters/postgres/__init__.py
+./blackline/adapters/postgres/postgres.py
+./blackline/models/postgres/__init__.py
+./blackline/models/postgres/postgres.py
 ./tests/conftest.py
 ./tests/test_postgrest_integration.py
-./tests/adapters/test_postgres_adapter.py
-./tests/models/test_postgres.py
+./tests/adapters/postgres/test_postgres_adapter.py
+./tests/models/postgres/test_postgres.py
 blackline_postgres.egg-info/PKG-INFO
 blackline_postgres.egg-info/SOURCES.txt
 blackline_postgres.egg-info/dependency_links.txt
 blackline_postgres.egg-info/requires.txt
 blackline_postgres.egg-info/top_level.txt
 tests/test_postgrest_integration.py
```

### Comparing `blackline-postgres-0.1.0a1/setup.cfg` & `blackline-postgres-0.1.1a0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = blackline-postgres
-version = 0.1.0a1
+version = 0.1.1a0
 url = https://github.com/blacklinedata/blackline-core/tree/main/blackline/postgres
 description = Manage personal data in your data stores.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
@@ -20,15 +20,15 @@
 [options]
 python_requires = >=3.9, <3.12
 package_dir = 
 	=.
 packages = find_namespace:
 include_package_data = True
 install_requires = 
-	blackline-core==0.1.0a1
+	blackline-core==0.1.1a0
 	psycopg[binary]>=3.1
 tests_require = 
 	pytest>=6.0
 
 [options.packages.find]
 where = .
```

### Comparing `blackline-postgres-0.1.0a1/tests/conftest.py` & `blackline-postgres-0.1.1a0/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,106 +4,71 @@
 The database is not available when running tests on github actions.
 The envionment variable GITHUB_ACTIONS is set to true when running on github actions.
 https://docs.github.com/en/actions/learn-github-actions/variables#default-environment-variables
 """
 
 
 import os
-from datetime import datetime
-from pathlib import Path
-from typing import List
+from typing import Callable, Generator
 
 import pytest
 import yaml
-from blackline.adapters.postgres import PostgresAdapter
-from blackline.constants import PROJECT_CONFIG_FILE
-from blackline.models.catalogue import StoreCatalogue
-from blackline.models.postgres import PostgresConfig
-from blackline.parsers.catalogue import CatalogueParser
-from blackline.query.query_factory import QueryFactory
-from blackline.utils.data.mock_data import user_data, user_data_deidentified
-from blackline.utils.testing.catalogue import catalogue_yaml as raw_catalogue_yaml
-from psycopg import Connection
+from blackline.adapters.postgres.postgres import PostgresAdapter
+from blackline.factories.query import QueryFactory
+from blackline.models.postgres.postgres import PostgresConfig
+from blackline.utils.testing.conftest_shared import *  # noqa: F403, F401
+from psycopg import Connection, Cursor
 from psycopg.pq import PGconn
+from psycopg.sql import SQL, Identifier
 from pytest import MonkeyPatch
 
 
 @pytest.fixture
 def github_actions_pg() -> bool:
     if os.getenv("GITHUB_ACTIONS") == "true":
         """This will help testing the monkeypatches locally.
         If set to true, the connections to postgres will fail if not correctly mocked.
         """
         return True
     return False
 
 
 @pytest.fixture
-def project_root() -> Path:
-    return Path("foo/bar")
-
-
-@pytest.fixture
-def fake_project_name() -> str:
-    return "fake-project"
-
-
-@pytest.fixture
 def postgres_store_name() -> str:
     return "test_postgres"
 
 
 @pytest.fixture
-def test_table() -> str:
-    return "test_table"
-
-
-@pytest.fixture
-def project_config_file() -> Path:
-    return Path(PROJECT_CONFIG_FILE)
-
-
-@pytest.fixture
-def profile() -> str:
-    return "dev"
-
-
-@pytest.fixture
-def start_date() -> str:
-    return datetime(2023, 1, 1)
-
-
-@pytest.fixture
 def postgres_user() -> str:
-    return os.environ.get("POSTGRES_USER")
+    return os.environ.get("POSTGRES_USER", "no_user_set")
 
 
 @pytest.fixture
 def postgres_password() -> str:
-    return os.environ.get("POSTGRES_PASSWORD")
+    return os.environ.get("POSTGRES_PASSWORD", "no_password_set")
 
 
 @pytest.fixture
 def postgres_host() -> str:
-    return os.environ.get("POSTGRES_HOST")
+    return os.environ.get("POSTGRES_HOST", "127.0.0.1")
 
 
 @pytest.fixture
-def postgres_port() -> str:
+def postgres_port() -> int:
     if os.getenv("GITHUB_ACTIONS") == "true":
         """This will help testing the monkeypatches locally.
         If set to true, the connections to postgres will fail if not correctly mocked.
         """
         return 5555
-    return os.environ.get("POSTGRES_PORT")
+    return int(os.environ.get("POSTGRES_PORT", 5432))
 
 
 @pytest.fixture
 def postgres_db() -> str:
-    return os.environ.get("POSTGRES_DB")
+    return os.environ.get("POSTGRES_DB", "no_db_set")
 
 
 @pytest.fixture
 def stores_yaml(
     postgres_store_name: str,
     postgres_user: str,
     postgres_password: str,
@@ -125,24 +90,14 @@
               dbname: {postgres_db}
               user: {postgres_user}
               password: {postgres_password}
         """
 
 
 @pytest.fixture
-def mock_data() -> List:
-    return user_data()
-
-
-@pytest.fixture
-def deidentified_mock_data() -> List:
-    return user_data_deidentified()
-
-
-@pytest.fixture
 def postgres_connection(
     postgres_user: str,
     postgres_password: str,
     postgres_host: str,
     postgres_port: str,
     postgres_db: str,
     github_actions_pg: bool,
@@ -155,80 +110,84 @@
         def _connect(*args, **kwargs):
             conn_url = f"postgresql://{postgres_user}:{postgres_password}@{postgres_host}:{postgres_port}/{postgres_db}"  # noqa: E501
             conn_str = f"host={postgres_host} port={postgres_port} dbname={postgres_db} user={postgres_user} password={postgres_password}"  # noqa: E501
             if args:
                 assert args[0] == conn_str or args[0] == conn_url
             if kwargs:
                 assert kwargs["conninfo"] == conn_str or kwargs["conninfo"] == conn_url
-            return Connection(pgconn=PGconn(None))
+            return Connection(pgconn=PGconn())
 
         monkeypatch.setattr(Connection, "connect", _connect)
+        monkeypatch.setattr(Connection, "commit", lambda self: None)
+        monkeypatch.setattr(Connection, "close", lambda self: None)
+        monkeypatch.setattr(
+            Connection, "cursor", lambda self, *args, **kwargs: Cursor(self)
+        )
+        monkeypatch.setattr(
+            Connection, "execute", lambda self, *args, **kwargs: Cursor(self)
+        )
+        monkeypatch.setattr(Cursor, "execute", lambda self, *args, **kwargs: None)
+        monkeypatch.setattr(Cursor, "executemany", lambda self, *args, **kwargs: None)
 
     return Connection.connect(conninfo)
 
 
 @pytest.fixture
 def load_database(
-    postgres_connection: Connection, mock_data: List, test_table: str
-) -> Connection:
+    postgres_connection: Connection, mock_data: list, test_table: str
+) -> Generator[Connection, None, None]:
     with postgres_connection as conn:
         with conn.cursor() as cursor:
-            cursor.execute(f"DROP TABLE IF EXISTS {test_table}")
+            cursor.execute(SQL("DROP TABLE IF EXISTS {table}").format(table=test_table))
             cursor.execute(
-                f"CREATE TABLE {test_table} (created_at TIMESTAMP, name VARCHAR(255), email VARCHAR(255), postal_code VARCHAR(15), active BOOLEAN, ip VARCHAR(15))"  # noqa: E501
+                SQL(
+                    """
+                CREATE EXTENSION IF NOT EXISTS "uuid-ossp";
+                CREATE TABLE {table} (
+                    id UUID DEFAULT uuid_generate_v4() ,
+                    created_at TIMESTAMP NOT NULL CHECK (created_at > '2020-01-01'),
+                    name VARCHAR(255),
+                    email VARCHAR(255) NOT NULL UNIQUE,
+                    postal_code VARCHAR(15),
+                    active BOOLEAN,
+                    ip VARCHAR(15) NOT NULL,
+                    CONSTRAINT pkey_tbl PRIMARY KEY ( id )
+                    )"""
+                ).format(table=Identifier(test_table))
             )
             cursor.executemany(
-                f"INSERT INTO {test_table} (created_at, name, email, postal_code, active, ip) VALUES (%s, %s, %s, %s, %s, %s)",  # noqa: E501
+                SQL(
+                    """INSERT INTO {table} (
+                    created_at,
+                    name,
+                    email,
+                    postal_code,
+                    active,
+                    ip
+                    ) VALUES (%s, %s, %s, %s, %s, %s)"""
+                ).format(table=Identifier(test_table)),
                 mock_data,
             )
             conn.commit()
 
             yield conn
 
-            cursor.execute(f"DROP TABLE IF EXISTS {test_table}")
+            cursor.execute(SQL("DROP TABLE IF EXISTS {table}").format(table=test_table))
 
 
 @pytest.fixture
 def postgres_adapter(
     stores_yaml: str,
     postgres_connection: Connection,
 ) -> PostgresAdapter:
     store_obj = yaml.safe_load(stores_yaml)
     postgres_obj = store_obj["profiles"]["dev"]
     pg_config = PostgresConfig.parse_obj(postgres_obj)
     return PostgresAdapter(config=pg_config.config)
 
 
 @pytest.fixture
-def catalogue_yaml() -> str:
-    return raw_catalogue_yaml()
-
-
-@pytest.fixture
-def catalogue_parser(catalogue_yaml: str, monkeypatch: MonkeyPatch) -> CatalogueParser:
-    path = Path("foo", "bar")
-
-    def _parse_store_catalogues(self, *args, **kwargs) -> List[StoreCatalogue]:
-        return [self._parse_yml()]
-
-    def _parse_yml(self, *args, **kwargs) -> StoreCatalogue:
-        info = yaml.safe_load(catalogue_yaml)
-        info = {"name": self._store_name(path=path), "tables": info}
-        return StoreCatalogue.parse_obj(info)
-
-    monkeypatch.setattr(
-        CatalogueParser, "_parse_store_catalogues", _parse_store_catalogues
-    )
-    monkeypatch.setattr(CatalogueParser, "_parse_yml", _parse_yml)
-
-    return CatalogueParser(path=path)
-
-
-@pytest.fixture
 def postgres_query_factory(
+    query_factory_factory: Callable,
     postgres_adapter: PostgresAdapter,
-    catalogue_parser: CatalogueParser,
-    test_table: str,
-    start_date: datetime,
 ) -> QueryFactory:
-    table = catalogue_parser.catalogue.stores[0].tables[test_table]
-    return QueryFactory(adapter=postgres_adapter, table=table, start_date=start_date)
+    return query_factory_factory(adapter=postgres_adapter)
```

### Comparing `blackline-postgres-0.1.0a1/tests/models/test_postgres.py` & `blackline-postgres-0.1.1a0/tests/models/postgres/test_postgres.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import yaml
-from blackline.models.postgres import PostgresConfig
+from blackline.models.postgres.postgres import PostgresConfig
 from pydantic.types import SecretStr
 
 
 def test_PostgresConfig(stores_yaml: str) -> None:
     # Setup
     store_obj = yaml.safe_load(stores_yaml)
     postgres_obj = store_obj["profiles"]["dev"]
```

### Comparing `blackline-postgres-0.1.0a1/tests/test_postgrest_integration.py` & `blackline-postgres-0.1.1a0/tests/test_postgrest_integration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import os
 from typing import List
 
 import pytest
 import yaml
-from blackline.models.postgres import PostgresConfig
-from blackline.models.store import StoreConfig
-from blackline.query.query_factory import QueryFactory
+from blackline.factories.query import QueryFactory
+from blackline.models.datastores import DataStore
+from blackline.models.postgres.postgres import PostgresConfig
 from psycopg import Connection
 
 
 def test_postgrest_store_config(stores_yaml: str):
     # Setup
     pg_store_info = yaml.safe_load(stores_yaml)
 
     # Run
-    store_config = StoreConfig.parse_obj(pg_store_info)
+    store_config = DataStore.parse_obj(pg_store_info)
 
     # Assert
     isinstance(store_config.profiles["dev"], PostgresConfig)
 
 
 def test_query_factory_postgres_queries(
     postgres_query_factory: QueryFactory,
 ):
     # Run
     queries = postgres_query_factory.queries()
 
     # Assert
     assert (
         queries[0].sql
-        == "UPDATE test_table\nSET\n  name = null,\n  email = %(email_value)s\nWHERE created_at < %(cutoff)s"  # noqa: E501
+        == "UPDATE test_table\nSET\n  email = %(email_value)s,\n  name = null\nWHERE created_at < %(cutoff)s"  # noqa: E501
     )
     assert (
         queries[1].sql
         == "UPDATE test_table\nSET\n  ip = REGEXP_REPLACE(ip,'\\w',%(ip_value)s,'g')\nWHERE created_at < %(cutoff)s"  # noqa: E501
     )
 
 
@@ -53,8 +53,11 @@
     queries[1].execute()
 
     # Assert
     with queries[0].adapter.connection() as conn:
         cur = conn.execute(f"SELECT * FROM {test_table}")
         rows = cur.fetchall()
 
+    # Remove the id UUID from the rows
+    rows = [row[1:] for row in rows]
+
     assert set(deidentified_mock_data) == set(rows)
```

