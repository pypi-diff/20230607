# Comparing `tmp/blackline-mysql-0.1.0a1.tar.gz` & `tmp/blackline-mysql-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackline-mysql-0.1.0a1.tar", last modified: Tue Mar 14 15:01:55 2023, max compression
+gzip compressed data, was "blackline-mysql-0.1.1a0.tar", last modified: Wed Jun  7 13:00:12 2023, max compression
```

## Comparing `blackline-mysql-0.1.0a1.tar` & `blackline-mysql-0.1.1a0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:55.804777 blackline-mysql-0.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-14 15:01:55.804777 blackline-mysql-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-14 15:01:44.000000 blackline-mysql-0.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:55.804777 blackline-mysql-0.1.0a1/blackline/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-14 15:01:44.000000 blackline-mysql-0.1.0a1/blackline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:55.804777 blackline-mysql-0.1.0a1/blackline/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:44.000000 blackline-mysql-0.1.0a1/blackline/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-14 15:01:44.000000 blackline-mysql-0.1.0a1/blackline/adapters/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:55.804777 blackline-mysql-0.1.0a1/blackline/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:44.000000 blackline-mysql-0.1.0a1/blackline/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-14 15:01:44.000000 blackline-mysql-0.1.0a1/blackline/models/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:55.804777 blackline-mysql-0.1.0a1/blackline_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-14 15:01:55.000000 blackline-mysql-0.1.0a1/blackline_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-14 15:01:55.000000 blackline-mysql-0.1.0a1/blackline_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 15:01:55.000000 blackline-mysql-0.1.0a1/blackline_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-14 15:01:55.000000 blackline-mysql-0.1.0a1/blackline_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-14 15:01:55.000000 blackline-mysql-0.1.0a1/blackline_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-14 15:01:55.804777 blackline-mysql-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 15:01:44.000000 blackline-mysql-0.1.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:55.804777 blackline-mysql-0.1.0a1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:55.804777 blackline-mysql-0.1.0a1/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-14 15:01:44.000000 blackline-mysql-0.1.0a1/tests/adapters/test_mysql_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-03-14 15:01:44.000000 blackline-mysql-0.1.0a1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:55.804777 blackline-mysql-0.1.0a1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-14 15:01:44.000000 blackline-mysql-0.1.0a1/tests/models/test_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-14 15:01:44.000000 blackline-mysql-0.1.0a1/tests/test_mysql_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.137747 blackline-mysql-0.1.1a0/blackline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.137747 blackline-mysql-0.1.1a0/blackline/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/blackline/adapters/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/blackline/adapters/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/blackline/adapters/mysql/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.137747 blackline-mysql-0.1.1a0/blackline/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/blackline/models/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/blackline/models/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/blackline/models/mysql/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 13:00:12.000000 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-07 13:00:12.000000 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:00:12.000000 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 13:00:12.000000 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 13:00:12.000000 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/tests/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/tests/adapters/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/tests/adapters/mysql/test_mysql_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/tests/models/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/tests/models/mysql/test_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/tests/test_mysql_integration.py
```

### Comparing `blackline-mysql-0.1.0a1/PKG-INFO` & `blackline-mysql-0.1.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackline-mysql
-Version: 0.1.0a1
+Version: 0.1.1a0
 Summary: Manage personal data in your data stores.
 Home-page: https://github.com/blacklinedata/blackline-core/tree/main/blackline/mysql
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `blackline-mysql-0.1.0a1/blackline_mysql.egg-info/PKG-INFO` & `blackline-mysql-0.1.1a0/blackline_mysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackline-mysql
-Version: 0.1.0a1
+Version: 0.1.1a0
 Summary: Manage personal data in your data stores.
 Home-page: https://github.com/blacklinedata/blackline-core/tree/main/blackline/mysql
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `blackline-mysql-0.1.0a1/blackline_mysql.egg-info/SOURCES.txt` & `blackline-mysql-0.1.1a0/blackline_mysql.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 README.md
 setup.cfg
 setup.py
-./blackline/__init__.py
-./blackline/adapters/__init__.py
-./blackline/adapters/mysql.py
-./blackline/models/__init__.py
-./blackline/models/mysql.py
+./blackline/adapters/mysql/__init__.py
+./blackline/adapters/mysql/mysql.py
+./blackline/models/mysql/__init__.py
+./blackline/models/mysql/mysql.py
 ./tests/conftest.py
 ./tests/test_mysql_integration.py
-./tests/adapters/test_mysql_adapter.py
-./tests/models/test_mysql.py
+./tests/adapters/mysql/test_mysql_adapter.py
+./tests/models/mysql/test_mysql.py
 blackline_mysql.egg-info/PKG-INFO
 blackline_mysql.egg-info/SOURCES.txt
 blackline_mysql.egg-info/dependency_links.txt
 blackline_mysql.egg-info/requires.txt
 blackline_mysql.egg-info/top_level.txt
 tests/test_mysql_integration.py
```

### Comparing `blackline-mysql-0.1.0a1/setup.cfg` & `blackline-mysql-0.1.1a0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = blackline-mysql
-version = 0.1.0a1
+version = 0.1.1a0
 url = https://github.com/blacklinedata/blackline-core/tree/main/blackline/mysql
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
 	mysql-connector-python==8.0.32
 tests_require = 
 	pytest>=6.0
 
 [options.packages.find]
 where = .
```

### Comparing `blackline-mysql-0.1.0a1/tests/conftest.py` & `blackline-mysql-0.1.1a0/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,116 +4,80 @@
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
-from blackline.adapters.mysql import MySQLAdapter
-from blackline.constants import PROJECT_CONFIG_FILE
-from blackline.models.catalogue import StoreCatalogue
-from blackline.models.mysql import MySQLConfig
-from blackline.parsers.catalogue import CatalogueParser
-from blackline.query.query_factory import QueryFactory
-from blackline.utils.data.mock_data import user_data, user_data_deidentified
-from blackline.utils.testing.catalogue import catalogue_yaml as raw_catalogue_yaml
+from blackline.adapters.mysql.mysql import MySQLAdapter
+from blackline.factories.query import QueryFactory
+from blackline.models.mysql.mysql import MySQLConfig
+from blackline.utils.testing.conftest_shared import *  # noqa: F403, F401
 from mysql.connector import MySQLConnection
 from mysql.connector.abstracts import MySQLConnectionAbstract
 from mysql.connector.cursor import MySQLCursor
 from pytest import MonkeyPatch
 
 
 @pytest.fixture
-def github_actions_pg() -> bool:
+def github_actions_mysql() -> bool:
     if os.getenv("GITHUB_ACTIONS") == "true":
         """This will help testing the monkeypatches locally.
         If set to true, the connections to mysql will fail if not correctly mocked.
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
 def mysql_store_name() -> str:
     return "test_mysql"
 
 
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
 def mysql_user() -> str:
-    return os.environ.get("MYSQL_USER")
+    return os.environ.get("MYSQL_USER", "no_user_set")
 
 
 @pytest.fixture
 def mysql_password() -> str:
-    return os.environ.get("MYSQL_PASSWORD")
+    return os.environ.get("MYSQL_PASSWORD", "no_password_set")
 
 
 @pytest.fixture
 def mysql_host() -> str:
-    return os.environ.get("MYSQL_HOST")
+    return os.environ.get("MYSQL_HOST", "127.0.0.1")
 
 
 @pytest.fixture
-def mysql_port() -> str:
+def mysql_port() -> int:
     if os.getenv("GITHUB_ACTIONS") == "true":
         """This will help testing the monkeypatches locally.
         If set to true, the connections to mysql will fail if not correctly mocked.
         """
         return 5555
-    return int(os.environ.get("MYSQL_PORT"))
+    return int(os.environ.get("MYSQL_PORT", 3306))
 
 
 @pytest.fixture
 def mysql_db() -> str:
-    return os.environ.get("MYSQL_DB")
+    return os.environ.get("MYSQL_DB", "no_db_set")
 
 
 @pytest.fixture
 def stores_yaml(
     mysql_store_name: str,
     mysql_user: str,
     mysql_password: str,
     mysql_host: str,
-    mysql_port: str,
+    mysql_port: int,
     mysql_db: str,
 ) -> str:
     """https://www.mysqlql.org/docs/current/libpq-connect.html#LIBPQ-PARAMKEYWORDS"""
     return f"""
     name: {mysql_store_name}
     profiles:
       dev:
@@ -125,71 +89,76 @@
             database: {mysql_db}
             host: {mysql_host}
             port: {mysql_port}
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
 def mysql_connection(
     mysql_user: str,
     mysql_password: str,
     mysql_host: str,
     mysql_port: str,
     mysql_db: str,
-    github_actions_pg: bool,
+    github_actions_mysql: bool,
     monkeypatch: MonkeyPatch,
 ) -> MySQLConnection:
-    if github_actions_pg:
+    if github_actions_mysql:
 
         def __init__(self, **kwargs):
-            self._consume_results: bool = False
-            self._unread_result: bool = False
+            self._consume_results = False
+            self._unread_result = False
             if kwargs:
                 self.connect(**kwargs)
 
         def cursor(self, *args, **kwargs) -> MySQLCursor:
             return MySQLCursor(self)
 
         monkeypatch.setattr(MySQLConnection, "__init__", __init__)
         monkeypatch.setattr(MySQLConnection, "close", lambda self: None)
         monkeypatch.setattr(MySQLConnection, "cursor", cursor)
         monkeypatch.setattr(MySQLConnection, "commit", lambda self: None)
         monkeypatch.setattr(MySQLConnection, "is_connected", lambda self: True)
         monkeypatch.setattr(
             MySQLConnectionAbstract, "connect", lambda self, **kwargs: None
         )
+        monkeypatch.setattr(MySQLCursor, "execute", lambda self, *args, **kwargs: None)
+        monkeypatch.setattr(
+            MySQLCursor, "executemany", lambda self, *args, **kwargs: None
+        )
 
     return MySQLConnection(
         user=mysql_user,
         password=mysql_password,
         host=mysql_host,
         port=mysql_port,
         database=mysql_db,
     )
 
 
 @pytest.fixture
 def load_database(
-    mysql_connection: MySQLConnection, mock_data: List, test_table: str
-) -> MySQLConnection:
+    mysql_connection: MySQLConnection, mock_data: list, test_table: str
+) -> Generator[MySQLConnectionAbstract, None, None]:
     with mysql_connection as conn:
         with conn.cursor() as cursor:
             cursor.execute(f"DROP TABLE IF EXISTS {test_table}")
             cursor.execute(
-                f"CREATE TABLE {test_table} (created_at TIMESTAMP, name VARCHAR(255), email VARCHAR(255), postal_code VARCHAR(15), active BOOLEAN, ip VARCHAR(15))"  # noqa: E501
+                f"""
+                CREATE TABLE {test_table} (
+                    id CHAR(36) DEFAULT (UUID()) UNIQUE,
+                    created_at TIMESTAMP,
+                    name VARCHAR(255),
+                    email VARCHAR(255) NOT NULL,
+                    postal_code VARCHAR(15) UNIQUE,
+                    active BOOLEAN,
+                    ip VARCHAR(15),
+                    CHECK (created_at > '2020-01-01 00:00:00'),
+                    PRIMARY KEY (`id`)
+                    )"""
             )
             cursor.executemany(
                 f"INSERT INTO {test_table} (created_at, name, email, postal_code, active, ip) VALUES (%s, %s, %s, %s, %s, %s)",  # noqa: E501
                 mock_data,
             )
             conn.commit()
 
@@ -206,40 +175,12 @@
     store_obj = yaml.safe_load(stores_yaml)
     mysql_obj = store_obj["profiles"]["dev"]
     pg_config = MySQLConfig.parse_obj(mysql_obj)
     return MySQLAdapter(config=pg_config.config)
 
 
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
 def mysql_query_factory(
+    query_factory_factory: Callable,
     mysql_adapter: MySQLAdapter,
-    catalogue_parser: CatalogueParser,
-    test_table: str,
-    start_date: datetime,
 ) -> QueryFactory:
-    table = catalogue_parser.catalogue.stores[0].tables[test_table]
-    return QueryFactory(adapter=mysql_adapter, table=table, start_date=start_date)
+    return query_factory_factory(adapter=mysql_adapter)
```

### Comparing `blackline-mysql-0.1.0a1/tests/models/test_mysql.py` & `blackline-mysql-0.1.1a0/tests/models/mysql/test_mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import yaml
-from blackline.models.mysql import MySQLConfig
+from blackline.models.mysql.mysql import MySQLConfig
 from pydantic.types import SecretStr
 
 
 def test_MySQLConfig(
     stores_yaml: str,
     mysql_user: str,
     mysql_password: SecretStr,
```

### Comparing `blackline-mysql-0.1.0a1/tests/test_mysql_integration.py` & `blackline-mysql-0.1.1a0/tests/test_mysql_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import os
 from typing import List
 
 import pytest
 import yaml
-from blackline.models.mysql import MySQLConfig
-from blackline.models.store import StoreConfig
-from blackline.query.query_factory import QueryFactory
+from blackline.factories.query import QueryFactory
+from blackline.models.datastores import DataStore
+from blackline.models.mysql.mysql import MySQLConfig
 from mysql.connector import MySQLConnection
 
 
-def test_postgrest_store_config(stores_yaml: str):
+def test_mysql_store_config(stores_yaml: str):
     # Setup
     pg_store_info = yaml.safe_load(stores_yaml)
 
     # Run
-    store_config = StoreConfig.parse_obj(pg_store_info)
+    store_config = DataStore.parse_obj(pg_store_info)
 
     # Assert
     isinstance(store_config.profiles["dev"], MySQLConfig)
 
 
-def test_query_factory_postgres_queries(
+def test_query_factory_mysql_queries(
     mysql_query_factory: QueryFactory,
 ):
     # Run
     queries = mysql_query_factory.queries()
 
     # Assert
     assert (
         queries[0].sql
-        == "UPDATE test_table\nSET\n  name = null,\n  email = %(email_value)s\nWHERE created_at < %(cutoff)s"  # noqa: E501
+        == "UPDATE test_table\nSET\n  email = %(email_value)s,\n  name = null\nWHERE created_at < %(cutoff)s"  # noqa: E501
     )
     assert (
         queries[1].sql
         == "UPDATE test_table\nSET\n  ip = REGEXP_REPLACE(ip,'[:alnum:]',%(ip_value)s)\nWHERE created_at < %(cutoff)s"  # noqa: E501
     )
 
 
@@ -54,8 +54,12 @@
 
     # Assert
     with queries[0].adapter.connection() as conn:
         with conn.cursor() as cursor:
             cursor.execute(f"SELECT * FROM {test_table}")
             rows = cursor.fetchall()
 
+    # Remove the UUIS from the rows
+    rows = [row[1:] for row in rows]
+
+    # breakpoint()
     assert set(deidentified_mock_data) == set(rows)
```

