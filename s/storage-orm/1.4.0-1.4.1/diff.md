# Comparing `tmp/storage_orm-1.4.0.tar.gz` & `tmp/storage_orm-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage_orm-1.4.0.tar", last modified: Wed Apr 19 07:11:40 2023, max compression
+gzip compressed data, was "storage_orm-1.4.1.tar", last modified: Wed Jun  7 09:58:31 2023, max compression
```

## Comparing `storage_orm-1.4.0.tar` & `storage_orm-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:11:40.321634 storage_orm-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-04-19 07:11:40.321634 storage_orm-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-04-19 07:11:29.000000 storage_orm-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 07:11:40.321634 storage_orm-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-19 07:11:29.000000 storage_orm-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:11:40.321634 storage_orm-1.4.0/storage_orm/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/operation_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:11:40.321634 storage_orm-1.4.0/storage_orm/redis_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/redis_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/redis_impl/redis_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/redis_impl/redis_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/redis_impl/redis_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/storage_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/storage_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/storage_orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:11:40.321634 storage_orm-1.4.0/storage_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-04-19 07:11:40.000000 storage_orm-1.4.0/storage_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 07:11:40.000000 storage_orm-1.4.0/storage_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:11:40.000000 storage_orm-1.4.0/storage_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 07:11:40.000000 storage_orm-1.4.0/storage_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 07:11:40.000000 storage_orm-1.4.0/storage_orm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:58:31.414667 storage_orm-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-06-07 09:58:31.414667 storage_orm-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-07 09:58:20.000000 storage_orm-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:58:31.414667 storage_orm-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-07 09:58:20.000000 storage_orm-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:58:31.410667 storage_orm-1.4.1/storage_orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/operation_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:58:31.414667 storage_orm-1.4.1/storage_orm/redis_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/redis_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/redis_impl/redis_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19713 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/redis_impl/redis_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/redis_impl/redis_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/storage_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/storage_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/storage_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:58:31.414667 storage_orm-1.4.1/storage_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-06-07 09:58:31.000000 storage_orm-1.4.1/storage_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-07 09:58:31.000000 storage_orm-1.4.1/storage_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:58:31.000000 storage_orm-1.4.1/storage_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 09:58:31.000000 storage_orm-1.4.1/storage_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 09:58:31.000000 storage_orm-1.4.1/storage_orm.egg-info/top_level.txt
```

### Comparing `storage_orm-1.4.0/PKG-INFO` & `storage_orm-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storage_orm
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/storage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/storage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `storage_orm-1.4.0/README.md` & `storage_orm-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.0/setup.py` & `storage_orm-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.0/storage_orm/operation_result.py` & `storage_orm-1.4.1/storage_orm/operation_result.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.0/storage_orm/redis_impl/redis_frame.py` & `storage_orm-1.4.1/storage_orm/redis_impl/redis_frame.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.0/storage_orm/redis_impl/redis_item.py` & `storage_orm-1.4.1/storage_orm/redis_impl/redis_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from contextlib import suppress
-import logging
 import re
 import copy
+import uuid
 import itertools
 import pickle
 
 from typing import Any
 from typing import Callable
 from typing import Mapping
 from typing import Type
@@ -236,15 +236,18 @@
 
     @classmethod
     def _get_src_values_for_meta(cls: Type[T], table: str) -> dict:
         """ Получение значений данных Meta класса"""
         src_values_for_meta: dict = dict()
         src_values: list[str] = table.split(".")
         for key, position in cls._keys_positions.items():
-            src_values_for_meta[key] = int(src_values[position])
+            if len(src_values[position]) == 36:  # UUID
+                src_values_for_meta[key] = uuid.UUID(src_values[position])
+            else:
+                src_values_for_meta[key] = int(src_values[position])
         return src_values_for_meta
 
     @classmethod
     def _objects_from_db_items(cls: Type[T], items: dict[bytes, bytes]) -> list[T]:
         """ Формирование cls(RedisItem)-объектов из данных базы """
         class_fields: dict = {}
         for redis_key, src_value in items.items():
```

### Comparing `storage_orm-1.4.0/storage_orm/redis_impl/redis_orm.py` & `storage_orm-1.4.1/storage_orm/redis_impl/redis_orm.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.0/storage_orm/storage_frame.py` & `storage_orm-1.4.1/storage_orm/storage_frame.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.0/storage_orm/storage_item.py` & `storage_orm-1.4.1/storage_orm/storage_item.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.0/storage_orm/storage_orm.py` & `storage_orm-1.4.1/storage_orm/storage_orm.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.0/storage_orm.egg-info/PKG-INFO` & `storage_orm-1.4.1/storage_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storage-orm
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/storage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/storage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

