# Comparing `tmp/watchmen_storage_postgresql-16.5.6.tar.gz` & `tmp/watchmen_storage_postgresql-16.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_postgresql-16.5.6.tar", max compression
+gzip compressed data, was "watchmen_storage_postgresql-16.5.7.tar", max compression
```

## Comparing `watchmen_storage_postgresql-16.5.6.tar` & `watchmen_storage_postgresql-16.5.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/LICENSE
--rw-r--r--   0        0        0      478 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/pyproject.toml
--rw-r--r--   0        0        0      309 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/__init__.py
--rw-r--r--   0        0        0     3557 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/data_source_postgresql.py
--rw-r--r--   0        0        0     2485 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/script_builder_postgresql.py
--rw-r--r--   0        0        0     7620 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/storage_postgresql.py
--rw-r--r--   0        0        0     2045 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/storage_postgresql_configuration.py
--rw-r--r--   0        0        0     7816 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/table_creator.py
--rw-r--r--   0        0        0    12688 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/where_build.py
--rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 watchmen_storage_postgresql-16.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-07 11:34:15.659987 watchmen_storage_postgresql-16.5.7/LICENSE
+-rw-r--r--   0        0        0      478 2023-06-07 11:34:15.659987 watchmen_storage_postgresql-16.5.7/pyproject.toml
+-rw-r--r--   0        0        0      309 2023-06-07 11:34:15.663987 watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/__init__.py
+-rw-r--r--   0        0        0     3557 2023-06-07 11:34:15.663987 watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/data_source_postgresql.py
+-rw-r--r--   0        0        0     2485 2023-06-07 11:34:15.663987 watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/script_builder_postgresql.py
+-rw-r--r--   0        0        0     7620 2023-06-07 11:34:15.663987 watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/storage_postgresql.py
+-rw-r--r--   0        0        0     2045 2023-06-07 11:34:15.663987 watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/storage_postgresql_configuration.py
+-rw-r--r--   0        0        0     7816 2023-06-07 11:34:15.663987 watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/table_creator.py
+-rw-r--r--   0        0        0    12688 2023-06-07 11:34:15.663987 watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/where_build.py
+-rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 watchmen_storage_postgresql-16.5.7/PKG-INFO
```

### Comparing `watchmen_storage_postgresql-16.5.6/LICENSE` & `watchmen_storage_postgresql-16.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/data_source_postgresql.py` & `watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/data_source_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/script_builder_postgresql.py` & `watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/script_builder_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/storage_postgresql.py` & `watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/storage_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/storage_postgresql_configuration.py` & `watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/storage_postgresql_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/table_creator.py` & `watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/table_creator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/where_build.py` & `watchmen_storage_postgresql-16.5.7/src/watchmen_storage_postgresql/where_build.py`

 * *Files identical despite different names*

