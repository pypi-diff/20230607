# Comparing `tmp/aiostorage_orm-1.4.1.tar.gz` & `tmp/aiostorage_orm-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiostorage_orm-1.4.1.tar", last modified: Wed Jun  7 09:59:02 2023, max compression
+gzip compressed data, was "aiostorage_orm-1.4.2.tar", last modified: Wed Jun  7 10:13:26 2023, max compression
```

## Comparing `aiostorage_orm-1.4.1.tar` & `aiostorage_orm-1.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/aiostorage_orm/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/operation_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-06-07 09:59:02.000000 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 09:59:02.000000 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:59:02.000000 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 09:59:02.000000 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 09:59:02.000000 aiostorage_orm-1.4.1/aiostorage_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:59:02.452432 aiostorage_orm-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-07 09:58:47.000000 aiostorage_orm-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:13:26.750057 aiostorage_orm-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-06-07 10:13:26.750057 aiostorage_orm-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:13:26.746057 aiostorage_orm-1.4.2/aiostorage_orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/aiostorage_orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/aiostorage_orm/aiostorage_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/aiostorage_orm/aiostorage_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/aiostorage_orm/aiostorage_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/aiostorage_orm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/aiostorage_orm/operation_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:13:26.750057 aiostorage_orm-1.4.2/aiostorage_orm/redis_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/aiostorage_orm/redis_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/aiostorage_orm/redis_impl/aioredis_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20134 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/aiostorage_orm/redis_impl/aioredis_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/aiostorage_orm/redis_impl/aioredis_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:13:26.750057 aiostorage_orm-1.4.2/aiostorage_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-06-07 10:13:26.000000 aiostorage_orm-1.4.2/aiostorage_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 10:13:26.000000 aiostorage_orm-1.4.2/aiostorage_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:13:26.000000 aiostorage_orm-1.4.2/aiostorage_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 10:13:26.000000 aiostorage_orm-1.4.2/aiostorage_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 10:13:26.000000 aiostorage_orm-1.4.2/aiostorage_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:13:26.750057 aiostorage_orm-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-07 10:13:12.000000 aiostorage_orm-1.4.2/setup.py
```

### Comparing `aiostorage_orm-1.4.1/PKG-INFO` & `aiostorage_orm-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiostorage_orm
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/aiostorage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/aiostorage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiostorage_orm-1.4.1/README.md` & `aiostorage_orm-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_frame.py` & `aiostorage_orm-1.4.2/aiostorage_orm/aiostorage_frame.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_item.py` & `aiostorage_orm-1.4.2/aiostorage_orm/aiostorage_item.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.1/aiostorage_orm/aiostorage_orm.py` & `aiostorage_orm-1.4.2/aiostorage_orm/aiostorage_orm.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.1/aiostorage_orm/operation_result.py` & `aiostorage_orm-1.4.2/aiostorage_orm/operation_result.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_frame.py` & `aiostorage_orm-1.4.2/aiostorage_orm/redis_impl/aioredis_frame.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_item.py` & `aiostorage_orm-1.4.2/aiostorage_orm/redis_impl/aioredis_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,19 @@
             index.replace("{", "").replace("}", ""): key
             for key, index in enumerate(cls.Meta.table.split(KEYS_DELIMITER))
             if index.startswith("{") and index.endswith("}")
         }
         for param in cls._keys_positions.keys():
             if param in cls.__annotations__:
                 del cls.__annotations__[param]
-        # Аргумент, который используется для дальнейшей проверки и работы
+        # Аргументы, которые используются для дальнейшей проверки и работы
         if hasattr(cls.Meta, "frame_size"):
             setattr(cls, "_frame_size", cls.Meta.frame_size)
+        if hasattr(cls.Meta, "ttl") and cls.Meta.ttl:
+            setattr(cls, "_ttl", cls.Meta.ttl)
 
     @classmethod
     def _make_kwargs_from_objects(cls: Type[T], objects: list[T]) -> dict:
         """
             Конкатенация атрибутов объектов и их подготовка для
                 использования в качестве фильтров
         """
```

### Comparing `aiostorage_orm-1.4.1/aiostorage_orm/redis_impl/aioredis_orm.py` & `aiostorage_orm-1.4.2/aiostorage_orm/redis_impl/aioredis_orm.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.1/aiostorage_orm.egg-info/PKG-INFO` & `aiostorage_orm-1.4.2/aiostorage_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiostorage-orm
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/aiostorage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/aiostorage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiostorage_orm-1.4.1/aiostorage_orm.egg-info/SOURCES.txt` & `aiostorage_orm-1.4.2/aiostorage_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.4.1/setup.py` & `aiostorage_orm-1.4.2/setup.py`

 * *Files identical despite different names*

