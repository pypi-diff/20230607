# Comparing `tmp/blackline-core-0.1.0a1.tar.gz` & `tmp/blackline-core-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackline-core-0.1.0a1.tar", last modified: Tue Mar 14 15:02:00 2023, max compression
+gzip compressed data, was "blackline-core-0.1.1a0.tar", last modified: Wed Jun  7 13:00:13 2023, max compression
```

## Comparing `blackline-core-0.1.0a1.tar` & `blackline-core-0.1.1a0.tar`

### file list

```diff
@@ -1,110 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.626817 blackline-core-0.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-14 15:02:00.626817 blackline-core-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.614816 blackline-core-0.1.0a1/blackline/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.618816 blackline-core-0.1.0a1/blackline/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/adapters/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/adapters/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.618816 blackline-core-0.1.0a1/blackline/catalogue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/catalogue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/catalogue/catalogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.618816 blackline-core-0.1.0a1/blackline/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.618816 blackline-core-0.1.0a1/blackline/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/execution/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/execution/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/execution/deidentify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/execution/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/execution/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.618816 blackline-core-0.1.0a1/blackline/models/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/models/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/models/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/models/project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/models/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/models/store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.618816 blackline-core-0.1.0a1/blackline/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/parsers/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/parsers/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/parsers/stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.618816 blackline-core-0.1.0a1/blackline/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/project/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.618816 blackline-core-0.1.0a1/blackline/project/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/project/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/project/templates/blackline_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/blackline/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/query/query_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/query/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/query/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.614816 blackline-core-0.1.0a1/blackline/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/blackline/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/utils/data/mock_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/blackline/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/blackline/utils/testing/catalogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.626817 blackline-core-0.1.0a1/blackline_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-14 15:02:00.000000 blackline-core-0.1.0a1/blackline_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-14 15:02:00.000000 blackline-core-0.1.0a1/blackline_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 15:02:00.000000 blackline-core-0.1.0a1/blackline_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-14 15:02:00.000000 blackline-core-0.1.0a1/blackline_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-14 15:02:00.000000 blackline-core-0.1.0a1/blackline_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-14 15:02:00.000000 blackline-core-0.1.0a1/blackline_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-14 15:02:00.626817 blackline-core-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/adapters/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/adapters/test_sqlite_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/catalogue/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/catalogue/test_catalogue_catalogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/conftest_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/execution/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/execution/test_deifentify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/execution/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/execution/test_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.614816 blackline-core-0.1.0a1/tests/mock_projects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/mock_projects/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/mock_projects/core/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/mock_projects/core/adapters/core.yml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/mock_projects/core/adapters/sqllite.yml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/mock_projects/core/blackline_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.614816 blackline-core-0.1.0a1/tests/mock_projects/core/catalogue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/mock_projects/core/catalogue/core/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/mock_projects/core/catalogue/core/example.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/mock_projects/postgres/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/mock_projects/postgres/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/mock_projects/postgres/adapters/postgres.yml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/mock_projects/postgres/blackline_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/mock_projects/postgres/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/mock_projects/postgres/catalog/postgres.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.622817 blackline-core-0.1.0a1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/models/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/models/test_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.626817 blackline-core-0.1.0a1/tests/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/parsers/test_catalogue_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/parsers/test_project_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/parsers/test_stores_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.626817 blackline-core-0.1.0a1/tests/project/
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/project/test_init_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/project/test_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:02:00.626817 blackline-core-0.1.0a1/tests/query/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/query/test_factory_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/query/test_query_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-14 15:01:45.000000 blackline-core-0.1.0a1/tests/query/test_template_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.590956 blackline-core-0.1.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-07 13:00:13.590956 blackline-core-0.1.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/adapters/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/adapters/sql/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/adapters/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/adapters/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/adapters/sqlite/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/deidentify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/factories/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/factories/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/project_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/models/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/sqlite/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/project/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/project/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/project/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/project/templates/blackline_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/blackline/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/query/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/query/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/blackline/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/default_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/doc_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/blackline/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/testing/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/testing/conftest_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/testing/raw_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.590956 blackline-core-0.1.1a0/blackline_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-07 13:00:13.590956 blackline-core-0.1.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/adapters/test_sqlite_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/conftest_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/execution/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/execution/test_deifentify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/execution/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/execution/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/execution/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/factories/test_adapter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/factories/test_query_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/models/test_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/models/test_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/models/test_project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/models/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/models/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/project/test_init_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/query/test_query_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/query/test_template_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/utils/test_doc_examples.py
```

### Comparing `blackline-core-0.1.0a1/PKG-INFO` & `blackline-core-0.1.1a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackline-core
-Version: 0.1.0a1
+Version: 0.1.1a0
 Summary: Manage personal data in your data stores.
 Home-page: https://github.com/blacklinedata/blackline-core
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
@@ -12,11 +12,12 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 
 # blackline-core
 
 [blackline](www.getblackline.com) Allows teams to easily manage and catelog their retention periods for [Person Identifying Information](https://gdpr.eu/eu-gdpr-personal-data/)
```

### Comparing `blackline-core-0.1.0a1/blackline/adapters/base.py` & `blackline-core-0.1.1a0/blackline/adapters/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Optional
 
+from blackline.models.catalogue import Dataset
+from blackline.models.validation import DatasetCollectionValidation
+
 # from blackline.models.adapter import AdapterConfig
-# TODO: Add type hinting for AdapterConfig, it current causes a circular import.
+# TODO: Add type hinting for AdapterConfig, it currently causes a circular import.
 
 
 class AdapterBase(ABC):
     date_format = "%Y-%m-%d"
 
     def __init__(self, config) -> None:
         # def __init__(self, config: AdapterConfig) -> None:
@@ -61,7 +64,11 @@
     @abstractmethod
     def mask_template(self) -> str:
         pass
 
     @abstractmethod
     def where_template(self) -> str:
         pass
+
+    # @abstractmethod
+    def validate_dataset(self, dataset: Dataset) -> DatasetCollectionValidation:
+        return DatasetCollectionValidation()
```

### Comparing `blackline-core-0.1.0a1/blackline/adapters/factory.py` & `blackline-core-0.1.1a0/blackline/factories/adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,44 +9,38 @@
 
 
 class AdapterFactory:
     def __init__(self) -> None:
         self.adapters: Dict[str, AdapterBase] = {}
 
     def adapter(self, name: str) -> AdapterBase:
-        adapter = self.adapters.get(name)
-        if adapter is not None:
-            return adapter
-        _cls = self.load_adapter(name)
-        self.adapters[name] = _cls
-        return _cls
+        return self.adapters.setdefault(name, self.load_adapter(name))
 
     @staticmethod
     def load_adapter(name: str) -> AdapterBase:
         mod = AdapterFactory._import_module(submodule=ADAPTER_SUBMODULE, name=name)
         return AdapterFactory._filter_class_from_module(mod)
 
     @staticmethod
     def _import_module(
         submodule: str, name: str, suffix: Optional[str] = None
     ) -> ModuleType:
-        _name = f"blackline.{submodule}.{name}"
+        _name = f"blackline.{submodule}.{name}.{name}"
         if suffix is not None:
             _name += f"_{suffix}"
         try:
             return import_module(_name)
         except ModuleNotFoundError as e:
             if e.name and "blackline" in e.name:
                 raise ModuleNotFoundError(
                     f"Could not import plugin: {_name}. Have you install the blackline-{name} package?"  # noqa: E501
                 )
             raise e
 
     @staticmethod
     def _filter_class_from_module(mod):
-
         return inspect.getmembers(
             mod,
             lambda member: inspect.isclass(member)
             and member.__module__ == mod.__name__,
         )[0][1]
         # noqa: E501 getmembers returns a list of tuples, where the first element is the name of the class and the second is the class itself.
```

### Comparing `blackline-core-0.1.0a1/blackline/adapters/sqlite.py` & `blackline-core-0.1.1a0/blackline/adapters/sqlite/sqlite.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import string
 from sqlite3 import Connection, Cursor, connect
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Optional, Union
 
-from blackline.adapters.sql import SQLAdapter
-from blackline.models.sqlite import SQLiteConfig
+from blackline.adapters.sql.sql import SQLAdapter
+from blackline.models.collection import Column
+from blackline.models.sqlite.sqlite import SQLiteConfig
+from sqlglot import exp, parse_one
 
 
 class SQLiteAdapter(SQLAdapter):
     config_model = SQLiteConfig
 
     def __init__(self, config: SQLiteConfig.Config, *args, **kwargs):
         super().__init__(config=config, *args, **kwargs)
 
     def connection(self) -> Connection:
         return connect(**self.config.connection.dict())
 
-    def execute(self, sql: str, values: Optional[Dict[str, Any]] = None) -> Any:
+    def execute(self, sql: str, values: Optional[dict[str, Any]] = None) -> Any:
         with self.connection() as conn:
             return conn.execute(sql, values or ())
 
-    def fetchall(self, results: Cursor) -> List[Tuple]:
+    def fetchall(self, results: Cursor) -> list[tuple]:
         return results.fetchall()
 
     def update_template(self) -> str:
         return "UPDATE {{ table }}"
 
     def set_template(self) -> str:
         return "SET"
@@ -51,27 +53,83 @@
             replace_str = f"REPLACE({replace_str}, '{c}', :{{{{ value }}}})"
 
         return f"{{{{ name }}}} = {replace_str}"
 
     def where_template(self) -> str:
         return "WHERE {{ datetime_column }} < :cutoff"
 
-    def columns(self, name: str) -> List[Tuple[str, str]]:
+    def test_connection(self) -> bool:
+        try:
+            with self.connection() as conn:
+                conn.execute("SELECT 1")
+                return True
+        except Exception:
+            return False
+
+    def table_exists(self, table: str) -> bool:
+        """Check if a table exists.
+
+        Args:
+            table (str): Table name.
+
+        Returns:
+            bool: True if the table exists.
+        """
+        with self.connection() as conn:
+            results = conn.execute(
+                "SELECT name FROM sqlite_master WHERE type='table' AND name=:table",
+                {"table": table},
+            ).fetchall()
+        return len(results) > 0
+
+    def columns(self, table: str) -> list[Column]:
         """
         Return a list of columns for a given table.
 
         Args:
-            name (str): Table name.
+            table: Table name.
 
         Returns:
-            List[Tuple[str, str]]: A list of (column name, type) tuple pairs.
+            A list of Column.
+        """
+        info = self.column_table_info(table=table)
+        check_info = self.column_check_info(table=table)
+        for column, check in check_info.items():
+            info[column]["check"] = check
+        return [Column.parse_obj(result) for result in info.values()]
+
+    def column_table_info(
+        self, table: str
+    ) -> dict[str, dict[str, Union[str, bool, None]]]:
         """
-        results = self.connection().execute(f"PRAGMA table_info({name})").fetchall()
-        return [(column[1], column[2]) for column in results]
+        Return a dictionary of columns for a given table.
 
-    def test_connection(self) -> bool:
-        try:
-            with self.connection() as conn:
-                conn.execute("SELECT 1")
-                return True
-        except Exception:
-            return False
+        Args:
+            table: Table name.
+
+        Returns:
+            A dictionary of column info.
+        """
+        with self.connection() as con:
+            info = con.execute(f"PRAGMA table_info({table})").fetchall()
+        return {
+            result[1]: {
+                "name": result[1],
+                "data_type": result[2],
+                "nullable": not bool(result[3]),
+                "default": result[4],
+                "primary_key": bool(result[5]),
+            }
+            for result in info
+        }
+
+    def column_check_info(self, table: str) -> dict[str, str]:
+        with self.connection() as con:
+            schema = con.execute(
+                f"select sql from sqlite_master where type='table' and name='{table}'"
+            ).fetchone()
+        if schema is None:
+            return {}
+        return {
+            constraint.find(exp.Identifier).name: constraint.sql()
+            for constraint in parse_one(schema[0]).find_all(exp.CheckColumnConstraint)
+        }
```

### Comparing `blackline-core-0.1.0a1/blackline/models/adapter.py` & `blackline-core-0.1.1a0/blackline/models/adapter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from datetime import datetime
-from typing import Any, List
+from typing import Any
 
-from blackline.adapters.factory import AdapterFactory
-from blackline.query.query import Query
-from blackline.query.query_factory import QueryFactory
+from blackline.factories.adapter import AdapterFactory
 from pydantic import BaseModel, root_validator, validator
 
 
 class ConnectionConfig(BaseModel):
     ...
 
 
@@ -15,24 +13,18 @@
     type: str
     adapter: Any = None
 
     @validator("adapter", pre=True, always=True)
     def load_adapter_cls(cls, value, values):
         return AdapterFactory.load_adapter(name=values["type"])
 
-    @root_validator
+    @root_validator(pre=False)
     def initialize_adapter(cls, values):
+        """
+        Shit design patter. The values["config"] is only added by the subclass.
+        This model cannot exist on it's on and is not labeled as an ABC.
+        """
         values["adapter"] = values["adapter"](values["config"])
         return values
 
     def deidentify(self, catalogue, start_date: datetime = datetime.now()):
-        for table in catalogue.tables.values():
-            queries = QueryFactory(
-                adapter=self.adapter,
-                table=table,
-                start_date=start_date,
-            ).queries()
-            self.execute_queries(queries=queries)
-
-    def execute_queries(self, queries: List[Query]) -> None:
-        for query in queries:
-            query.execute()
+        self.adapter.deidentify(catalogue=catalogue, start_date=start_date)
```

### Comparing `blackline-core-0.1.0a1/blackline/query/query.py` & `blackline-core-0.1.1a0/blackline/query/query.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from datetime import datetime
-from typing import Any, Dict, List, Union
+from typing import Any, Optional
 
 from blackline.adapters.base import AdapterBase
-from blackline.models.catalogue import ColumnRetention
+from blackline.models.catalogue import DatasetField
 
 
 class Query:
     def __init__(
         self,
         adapter: AdapterBase,
         sql: str,
-        columns: List[ColumnRetention],
+        fields: list[DatasetField],
         cutoff_date: datetime,
     ) -> None:
         self.adapter = adapter
         self.sql = sql
-        self.columns = columns
+        self.fields = fields
         self.cutoff_date = cutoff_date
 
     def __str__(self) -> str:
         return f"{self.sql}"
 
     def execute(self) -> Any:
-        values: Dict[str, Union[str, None]] = {
-            f"{column.name}_value": column.deidentifier.value for column in self.columns
+        values: dict[str, Optional[str]] = {
+            f"{field.name}_value": field.deidentifier.value
+            for field in self.fields
+            if field.deidentifier is not None
         }
         values["cutoff"] = self.cutoff_date.strftime(self.adapter.date_format)
         return self.adapter.execute(self.sql, values)
```

### Comparing `blackline-core-0.1.0a1/blackline/query/template.py` & `blackline-core-0.1.1a0/blackline/query/template.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.0a1/blackline/query/templates.py` & `blackline-core-0.1.1a0/blackline/query/templates.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.0a1/blackline/utils/testing/catalogue.py` & `blackline-core-0.1.1a0/blackline/utils/testing/catalogue.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.0a1/blackline_core.egg-info/PKG-INFO` & `blackline-core-0.1.1a0/blackline_core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackline-core
-Version: 0.1.0a1
+Version: 0.1.1a0
 Summary: Manage personal data in your data stores.
 Home-page: https://github.com/blacklinedata/blackline-core
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
@@ -12,11 +12,12 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 
 # blackline-core
 
 [blackline](www.getblackline.com) Allows teams to easily manage and catelog their retention periods for [Person Identifying Information](https://gdpr.eu/eu-gdpr-personal-data/)
```

### Comparing `blackline-core-0.1.0a1/tests/adapters/test_factory.py` & `blackline-core-0.1.1a0/tests/factories/test_adapter_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
-from blackline.adapters.factory import AdapterFactory
-from blackline.adapters.sqlite import SQLiteAdapter
-from blackline.models.sqlite import SQLiteConnectionConfig
+from blackline.adapters.sqlite.sqlite import SQLiteAdapter
+from blackline.factories.adapter import AdapterFactory
+from blackline.models.sqlite.sqlite import SQLiteConnectionConfig
 
 
 def test__init__() -> None:
     """Test that the factory is initialised correctly."""
     # Run
     factory = AdapterFactory()
```

### Comparing `blackline-core-0.1.0a1/tests/conftest_sqlite.py` & `blackline-core-0.1.1a0/tests/conftest_sqlite.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,23 @@
-import datetime
 import sqlite3
 from sqlite3 import Connection
 from typing import List
 
 import pytest
-from blackline.adapters.sqlite import SQLiteAdapter
-from blackline.parsers.stores import StoresParser
+from blackline.adapters.sqlite.sqlite import SQLiteAdapter
+from blackline.models.datastores import DataStore
 
 
 @pytest.fixture
 def sqlite_store_name() -> str:
     return "test_sqlite"
 
 
 @pytest.fixture
-def mock_data() -> List:
-    return [
-        (
-            datetime.datetime(2021, 1, 1),
-            "Dave",
-            "dave@example.com",
-            "12345",
-            True,
-            "127.0.0.1",
-        ),
-        (
-            datetime.datetime(2021, 6, 1),
-            "Alison",
-            "alison@example.com",
-            "23456",
-            True,
-            "127.0.0.2",
-        ),
-        (
-            datetime.datetime(2022, 3, 1),
-            "Chris",
-            "chris@example.com",
-            "34567",
-            False,
-            "127.0.0.3",
-        ),
-        (
-            datetime.datetime(2022, 4, 1),
-            "Megan",
-            "megan@example.com",
-            "45678",
-            True,
-            "127.0.0.4",
-        ),
-    ]
-
-
-@pytest.fixture
-def deidentified_mock_data() -> List:
+def deidentified_mock_data_sqlite() -> List:
     return [
         ("2021-01-01 00:00:00", None, "fake@email.com", "12345", 1, "###.#.#.#"),
         ("2021-06-01 00:00:00", None, "fake@email.com", "23456", 1, "###.#.#.#"),
         ("2022-03-01 00:00:00", "Chris", "chris@example.com", "34567", 0, "###.#.#.#"),
         (
             "2022-04-01 00:00:00",
             "Megan",
@@ -95,24 +56,23 @@
 
     con.cursor().execute(f"DROP TABLE {test_table}")
     con.close()
 
 
 @pytest.fixture
 def sqlite_adapter(
-    stores_parser: StoresParser, mock_sqlite_store: Connection, store_name: str
+    store: DataStore, mock_sqlite_store: Connection, store_name: str
 ) -> SQLiteAdapter:
-    store = stores_parser.store(name=store_name).profiles["dev"]
     return store.adapter
 
 
 @pytest.fixture
 def sqlite_store_yml() -> str:
     return """
     profiles:
       dev:
         type: sqlite
         config:
           connection:
-            database: "file::memory:?cache=shared"
+            database: "file::memory:"
             uri: true
     """
```

### Comparing `blackline-core-0.1.0a1/tests/execution/test_debug.py` & `blackline-core-0.1.1a0/tests/execution/test_debug.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from pathlib import Path
+from typing import Callable
 
 from blackline.execution.debug import Debug
 
 
-def test__init__(project_root: Path, profile: str):
+def test__init__(project_root: Path, sample_project: Callable, profile: str):
     """Test the __init__ method."""
     # Run
     debug = Debug(path=project_root, profile=profile)
 
     # Assert
     assert isinstance(debug, Debug)
 
 
-def test_debug(project_root: Path, profile: str):
+def test_debug(project_root: Path, sample_project: Callable, profile: str):
     """Test the debug method."""
     # Setup
     debug = Debug(path=project_root, profile=profile)
 
     # Run
     result = debug.debug()
```

### Comparing `blackline-core-0.1.0a1/tests/execution/test_report.py` & `blackline-core-0.1.1a0/tests/execution/test_report.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from pathlib import Path
+from typing import Callable
 
 from blackline.execution.report import create_report
 from blackline.models.catalogue import Catalogue
+from blackline.models.datastores import DataStore
 from blackline.models.project_config import ProjectConfig
-from blackline.models.store import StoreConfig
 
 
-def test_create_report(project_root: Path):
+def test_create_report(project_root: Path, sample_project: Callable):
+    # Setup
+
     # Run
     project, stores, catalogue = create_report(path=project_root)
 
     # Assert
     assert isinstance(project, ProjectConfig)
     for store in stores:
-        assert isinstance(store, StoreConfig)
+        assert isinstance(store, DataStore)
     assert isinstance(catalogue, Catalogue)
```

### Comparing `blackline-core-0.1.0a1/tests/models/test_sqlite.py` & `blackline-core-0.1.1a0/tests/models/test_sqlite.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from blackline.adapters.sqlite import SQLiteAdapter
-from blackline.models.sqlite import SQLiteConfig, SQLiteConnectionConfig
+from blackline.adapters.sqlite.sqlite import SQLiteAdapter
+from blackline.models.sqlite.sqlite import SQLiteConfig, SQLiteConnectionConfig
 from yaml import safe_load
 
 
 def test_SQLiteConnectionConfig(profile: str, sqlite_store_yml: str) -> None:
     info = safe_load(sqlite_store_yml)
     info = info["profiles"][profile]["config"]["connection"]
     config = SQLiteConnectionConfig.parse_obj(info)
-    assert config.database == "file::memory:?cache=shared"
+    assert config.database == "file::memory:"
     assert config.uri is True
 
 
 def test_SQLLiteConfig(profile: str, sqlite_store_yml: str) -> None:
     info = safe_load(sqlite_store_yml)
     sqlite_info = info["profiles"][profile]
     config = SQLiteConfig.parse_obj(sqlite_info)
```

### Comparing `blackline-core-0.1.0a1/tests/project/test_init_project.py` & `blackline-core-0.1.1a0/tests/project/test_init_project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,97 @@
 from pathlib import Path
 
 from blackline.constants import (
     DEFAULT_ADAPTERS_FOLDER,
     DEFAULT_CATALOGUE_FOLDER,
     PROJECT_CONFIG_FILE,
-    PROJECT_CONFIG_VERSION,
-    PROJECT_VERSION,
 )
-from blackline.models.project_config import ProjectConfig
-from blackline.project.init import create_project_yml, init_project
+from blackline.project.init import (
+    INIT_DATASET_FILENAME,
+    INIT_DATASET_FOLDER,
+    INIT_ORGANIZATION_FILENAME,
+    INIT_ORGANIZATION_FOLDER,
+    INIT_RESOURCE_FILENAME,
+    INIT_RESOURCE_FOLDER,
+    INIT_SYSTEM_FILENAME,
+    INIT_SYSTEM_FOLDER,
+    InitProject,
+)
 from yaml import Loader, load
 
 
 def test_init_project(tmp_path: Path, fake_project_name: str) -> None:
     """Test that the project is initialised correctly."""
     # Setup
-    project_config_path = Path(tmp_path, fake_project_name, PROJECT_CONFIG_FILE)
+    project_config_path = Path(tmp_path, PROJECT_CONFIG_FILE)
+    init_project = InitProject(path=tmp_path, name=fake_project_name)
+    project_config = init_project.project_config
 
     # Run
-    project_config = init_project(path=tmp_path, name=fake_project_name)
+    init_project.init_project()
 
     # Assert
     assert project_config_path.is_file()
     assert project_config.catalogue_path.is_dir()
     assert project_config.adapters_path.is_dir()
-    assert (
-        Path(tmp_path, fake_project_name, DEFAULT_ADAPTERS_FOLDER)
-        == project_config.adapters_path
-    )
-    assert (
-        Path(tmp_path, fake_project_name, DEFAULT_CATALOGUE_FOLDER)
-        == project_config.catalogue_path
-    )
+    assert Path(tmp_path, DEFAULT_ADAPTERS_FOLDER) == project_config.adapters_path
+    assert Path(tmp_path, DEFAULT_CATALOGUE_FOLDER) == project_config.catalogue_path
+    adapter_path = project_config.adapters_path
+    catalogue_path = project_config.catalogue_path
+
+    assert Path(
+        adapter_path,
+        INIT_ORGANIZATION_FOLDER,
+        INIT_SYSTEM_FOLDER,
+        INIT_RESOURCE_FOLDER,
+        INIT_DATASET_FILENAME,
+    ).is_file()
+
+    assert Path(
+        catalogue_path, INIT_ORGANIZATION_FOLDER, INIT_ORGANIZATION_FILENAME
+    ).is_file()
+    assert Path(
+        catalogue_path,
+        INIT_ORGANIZATION_FOLDER,
+        INIT_SYSTEM_FOLDER,
+        INIT_SYSTEM_FILENAME,
+    ).is_file()
+    assert Path(
+        catalogue_path,
+        INIT_ORGANIZATION_FOLDER,
+        INIT_SYSTEM_FOLDER,
+        INIT_RESOURCE_FOLDER,
+        INIT_RESOURCE_FILENAME,
+    ).is_file()
+    assert Path(
+        catalogue_path,
+        INIT_ORGANIZATION_FOLDER,
+        INIT_SYSTEM_FOLDER,
+        INIT_RESOURCE_FOLDER,
+        INIT_DATASET_FOLDER,
+        INIT_DATASET_FILENAME,
+    ).is_file()
 
 
 def test_create_project_yml(tmp_path: Path, fake_project_name: str) -> None:
     """Test that the project is initialised correctly."""
     # Setup
-    project_config_path = Path(tmp_path, PROJECT_CONFIG_FILE)
-    project_config = ProjectConfig(
-        name=fake_project_name,
-        config_version=PROJECT_CONFIG_VERSION,
-        version=PROJECT_VERSION,
-        default_profile="default",
-        catalogue_path=Path(DEFAULT_CATALOGUE_FOLDER),
-        adapters_path=Path(DEFAULT_ADAPTERS_FOLDER),
-        project_root=tmp_path,
-    )
+    project = InitProject(path=tmp_path, name=fake_project_name)
+    project_config = project.project_config
+    project_config_path = Path(project.path, PROJECT_CONFIG_FILE)
 
     # Run
-    create_project_yml(path=tmp_path, project_config=project_config)
+    project.create_project_yaml()
 
     # Assert
     project_text = project_config_path.read_text()
     project_obj = load(project_text, Loader=Loader)
 
     assert project_config_path.is_file()
     assert project_config.name == project_obj["name"]
     assert project_config.config_version == project_obj["config-version"]
     assert project_config.version == project_obj["version"]
     assert project_config.default_profile == project_obj["default-profile"]
-    assert project_config.catalogue_path == Path(project_obj["catalogue-path"])
-    assert project_config.adapters_path == Path(project_obj["adapters-path"])
+    assert Path(project_config.catalogue_path.name) == Path(
+        project_obj["catalogue-path"]
+    )
+    assert Path(project_config.adapters_path.name) == Path(project_obj["adapters-path"])
```

### Comparing `blackline-core-0.1.0a1/tests/query/test_factory_query.py` & `blackline-core-0.1.1a0/tests/factories/test_query_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 from datetime import timedelta
 
-from blackline.catalogue.catalogue import Catalogue
-from blackline.models.catalogue import ColumnRetention
-from blackline.models.store import StoreConfig
+from blackline.factories.query import QueryFactory
+from blackline.models.catalogue import Catalogue, DatasetField
+from blackline.models.datastores import DataStore
 from blackline.query.query import Query
-from blackline.query.query_factory import QueryFactory
 
 
 def test__init__(
-    catalogue: Catalogue, store: StoreConfig, test_table: str, store_name: str
+    catalogue: Catalogue, store: DataStore, test_table: str, store_name: str
 ) -> None:
     """Test init method."""
     # Setup
-    store_catalogue = [store for store in catalogue.stores if store.name == store_name][
-        0
-    ]
-    table = store_catalogue.tables[test_table]
+    store_catalogue = catalogue["organization_foo.system_foo.resource_foo.dataset_foo"]
+    collection = [
+        collection
+        for collection in store_catalogue.collections
+        if collection.name == test_table
+    ][0]
 
     # Run
-    factory = QueryFactory(adapter=store.adapter, table=table)
+    factory = QueryFactory(adapter=store.adapter, collection=collection)
 
     # Assert
     assert isinstance(factory, QueryFactory)
     assert factory.adapter == store.adapter
-    assert factory.table == table
+    assert factory.collection == collection
 
 
 def test_queries(query_factory: QueryFactory) -> None:
     """Test query construction."""
 
-    sql_0 = """UPDATE test_table\nSET\n  name = null,\n  email = :email_value\nWHERE created_at < :cutoff"""  # noqa E501
+    sql_0 = """UPDATE test_table\nSET\n  email = :email_value,\n  name = null\nWHERE created_at < :cutoff"""  # noqa E501
     sql_1 = """UPDATE test_table\nSET\n  ip = REPLACE(REPLACE(REPLACE(REPLACE(REPLACE(REPLACE(REPLACE(REPLACE(REPLACE(REPLACE(ip, '0', :ip_value), '1', :ip_value), '2', :ip_value), '3', :ip_value), '4', :ip_value), '5', :ip_value), '6', :ip_value), '7', :ip_value), '8', :ip_value), '9', :ip_value)\nWHERE created_at < :cutoff"""  # noqa E501
 
     # Run
     queries = query_factory.queries()
 
     # Assert
-    assert len(queries) == len(query_factory.columns_by_period())
+    assert len(queries) == len(query_factory.fields_by_period())
     assert queries[0].sql == sql_0
     assert queries[1].sql == sql_1
     for query in queries:
         assert isinstance(query, Query)
         assert query.adapter == query_factory.adapter
 
 
 def test_columns_by_period(query_factory: QueryFactory) -> None:
     """Test columns by retention period method."""
     # Run
-    columns = query_factory.columns_by_period()
+    columns = query_factory.fields_by_period()
 
     # Assert
     assert isinstance(columns, dict)
     assert len(columns) == 2
     for key, value in columns.items():
         assert isinstance(key, timedelta)
         assert isinstance(value, list)
         for column in value:
-            assert isinstance(column, ColumnRetention)
+            assert isinstance(column, DatasetField)
```

### Comparing `blackline-core-0.1.0a1/tests/query/test_query_query.py` & `blackline-core-0.1.1a0/tests/query/test_query_query.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from datetime import datetime
 
+from blackline.factories.query import QueryFactory
 from blackline.query.query import Query
-from blackline.query.query_factory import QueryFactory
 
 
 def test__init__(query_factory: QueryFactory) -> None:
     """Test that the Query class is initialised correctly."""
     # Setup
     adapter = query_factory.adapter
-    colums_by_period = query_factory.columns_by_period()
-    period = list(colums_by_period.keys())[0]
-    columns = colums_by_period[period]
-    sql = query_factory.render_sql(columns=columns)
+    fields_by_period = query_factory.fields_by_period()
+    period = list(fields_by_period.keys())[0]
+    fields = fields_by_period[period]
+    sql = query_factory.render_sql(fields=fields)
     cuttoff_date = query_factory.cutoff_date(period=period)
 
     # Run
 
-    query = Query(adapter=adapter, sql=sql, columns=columns, cutoff_date=cuttoff_date)
+    query = Query(adapter=adapter, sql=sql, fields=fields, cutoff_date=cuttoff_date)
 
     # Run & Assert
     assert isinstance(query, Query)
 
 
 def test_execute(query_factory: QueryFactory) -> None:
     """Test that a query is executed correctly."""
     # Setup
     adapter = query_factory.adapter
-    colums_by_period = query_factory.columns_by_period()
-    period = list(colums_by_period.keys())[0]
-    columns = colums_by_period[period]
-    sql = query_factory.render_sql(columns=columns)
+    fields_by_period = query_factory.fields_by_period()
+    period = list(fields_by_period.keys())[0]
+    fields = fields_by_period[period]
+    sql = query_factory.render_sql(fields=fields)
     cuttoff_date = query_factory.cutoff_date(period=period)
-    query = Query(adapter=adapter, sql=sql, columns=columns, cutoff_date=cuttoff_date)
+    query = Query(adapter=adapter, sql=sql, fields=fields, cutoff_date=cuttoff_date)
     old_data = query.adapter.execute(sql="SELECT * FROM test_table").fetchall()
     cutoff = query_factory.start_date - period
 
     # Run
     query.execute()
 
     # Assert
@@ -45,9 +45,9 @@
     diff = [new_data[i] for i, row in enumerate(old_data) if row != new_data[i]]
 
     diff_date_above_cutoff = [
         row for row in diff if datetime.strptime(row[0], "%Y-%m-%d %H:%M:%S") > cutoff
     ]
 
     assert not diff_date_above_cutoff
-    assert list({row[1] for row in diff})[0] == columns[0].deidentifier.value
-    assert list({row[2] for row in diff})[0] == columns[1].deidentifier.value
+    assert list({row[1] for row in diff})[0] == fields[1].deidentifier.value
+    assert list({row[2] for row in diff})[0] == fields[0].deidentifier.value
```

### Comparing `blackline-core-0.1.0a1/tests/query/test_template_query.py` & `blackline-core-0.1.1a0/tests/query/test_template_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 # from blackline.catalogue.catalogue import Catalogue
-from blackline.models.store import StoreConfig
-from blackline.query.template import Template
-
 # from blackline.store.store import Store
+from blackline.models.datastores import DataStore
+from blackline.query.template import Template
 from jinja2 import Template as JinjaTemplate
 from jinja2.runtime import Macro
 
 
-def test__init__(store: StoreConfig) -> None:
+def test__init__(store: DataStore) -> None:
     # Setup
     adapter = store.adapter
 
     # Run
     template = Template(adapter=adapter)
 
     # Assert
     assert isinstance(template, Template)
     assert isinstance(template.env.globals["redact"], Macro)
     assert isinstance(template.env.globals["replace"], Macro)
     assert isinstance(template.env.globals["mask"], Macro)
 
 
-def test_template_str(store: StoreConfig) -> None:
+def test_template_str(store: DataStore) -> None:
     # Setup
     adapter = store.adapter
     template = Template(adapter=adapter)
     expected = """UPDATE {{ table }}\nSET\n{% for column in columns %}\n  {% set value = column.name + "_value" %}\n  {{ redact(cls=column.deidentifier, name=column.name, value=value) -}}\n  {{ replace(cls=column.deidentifier, name=column.name, value=value) -}}\n  {{ mask(cls=column.deidentifier, name=column.name, value=value) -}}\n  {{ "," if not loop.last }}\n{% endfor %}\nWHERE {{ datetime_column }} < :cutoff\n"""  # noqa E501
 
     # Run
     _template = template.template_str()
 
     # Assert
     assert _template == expected
 
 
-def test_template(store: StoreConfig) -> None:
+def test_template(store: DataStore) -> None:
     # Setup
     adapter = store.adapter
     template = Template(adapter=adapter)
 
     # Run
     _template = template.template
```

