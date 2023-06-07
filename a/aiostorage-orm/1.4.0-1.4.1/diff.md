# Comparing `tmp/aiostorage_orm-1.4.0.tar.gz` & `tmp/aiostorage_orm-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiostorage_orm-1.4.0.tar", last modified: Wed Apr 19 07:12:35 2023, max compression
+gzip compressed data, was "aiostorage_orm-1.4.1.tar", last modified: Wed Jun  7 09:59:02 2023, max compression
```

## Comparing `aiostorage_orm-1.4.0.tar` & `aiostorage_orm-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:12:35.805313 aiostorage_orm-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-04-19 07:12:35.805313 aiostorage_orm-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:12:35.801313 aiostorage_orm-1.4.0/aiostorage_orm/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/operation_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:12:35.805313 aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:12:35.805313 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-04-19 07:12:35.000000 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-19 07:12:35.000000 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:12:35.000000 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 07:12:35.000000 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 07:12:35.000000 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 07:12:35.805313 aiostorage_orm-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/aiostorage_orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/operation_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-06-07 09:59:02.000000 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 09:59:02.000000 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:59:02.000000 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 09:59:02.000000 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 09:59:02.000000 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/setup.py
```

### Comparing `aiostorage_orm-1.4.0/PKG-INFO` & `aiostorage_orm-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiostorage_orm
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/aiostorage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/aiostorage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiostorage_orm-1.4.0/README.md` & `aiostorage_orm-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_frame.py` & `aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_frame.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_item.py` & `aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_item.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_orm.py` & `aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_orm.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.0/aiostorage_orm/operation_result.py` & `aiostorage_orm-1.4.1/aiostorage_orm/operation_result.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_frame.py` & `aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_frame.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_item.py` & `aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 import re
 import copy
+import uuid
 import pickle
 from contextlib import suppress
 
 import redis.asyncio as redis
 from redis.exceptions import ConnectionError
 import itertools
 from typing import (
@@ -244,15 +245,18 @@
 
     @classmethod
     def _get_src_values_for_meta(cls: Type[T], table: str) -> dict:
         """ Получение значений данных Meta класса"""
         src_values_for_meta: dict = dict()
         src_values: list[str] = table.split(".")
         for key, position in cls._keys_positions.items():
-            src_values_for_meta[key] = int(src_values[position])
+            if len(src_values[position]) == 36:  # UUID
+                src_values_for_meta[key] = uuid.UUID(src_values[position])
+            else:  # int
+                src_values_for_meta[key] = int(src_values[position])
         return src_values_for_meta
 
     @classmethod
     def _objects_from_db_items(cls: Type[T], items: dict[bytes, bytes]) -> list[T]:
         """ Формирование cls(RedisItem)-объектов из данных базы """
         class_fields: dict = {}
         for redis_key, src_value in items.items():
```

### Comparing `aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_orm.py` & `aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_orm.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.0/aiostorage_orm.egg-info/PKG-INFO` & `aiostorage_orm-1.4.1/aiostorage_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiostorage-orm
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/aiostorage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/aiostorage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiostorage_orm-1.4.0/aiostorage_orm.egg-info/SOURCES.txt` & `aiostorage_orm-1.4.1/aiostorage_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.0/setup.py` & `aiostorage_orm-1.4.1/setup.py`

 * *Files identical despite different names*

