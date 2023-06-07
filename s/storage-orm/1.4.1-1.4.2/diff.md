# Comparing `tmp/storage_orm-1.4.1.tar.gz` & `tmp/storage_orm-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage_orm-1.4.1.tar", last modified: Wed Jun  7 09:58:31 2023, max compression
+gzip compressed data, was "storage_orm-1.4.2.tar", last modified: Wed Jun  7 10:14:16 2023, max compression
```

## Comparing `storage_orm-1.4.1.tar` & `storage_orm-1.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:58:31.414667 storage_orm-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-06-07 09:58:31.414667 storage_orm-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-07 09:58:20.000000 storage_orm-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:58:31.414667 storage_orm-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-07 09:58:20.000000 storage_orm-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:58:31.410667 storage_orm-1.4.1/storage_orm/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/operation_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:58:31.414667 storage_orm-1.4.1/storage_orm/redis_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/redis_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/redis_impl/redis_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    19713 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/redis_impl/redis_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/redis_impl/redis_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/storage_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/storage_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-07 09:58:20.000000 storage_orm-1.4.1/storage_orm/storage_orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:58:31.414667 storage_orm-1.4.1/storage_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-06-07 09:58:31.000000 storage_orm-1.4.1/storage_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-07 09:58:31.000000 storage_orm-1.4.1/storage_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:58:31.000000 storage_orm-1.4.1/storage_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 09:58:31.000000 storage_orm-1.4.1/storage_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 09:58:31.000000 storage_orm-1.4.1/storage_orm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:16.729122 storage_orm-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-06-07 10:14:16.729122 storage_orm-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-07 10:14:06.000000 storage_orm-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:14:16.729122 storage_orm-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-07 10:14:06.000000 storage_orm-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:16.725122 storage_orm-1.4.2/storage_orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-07 10:14:06.000000 storage_orm-1.4.2/storage_orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 10:14:06.000000 storage_orm-1.4.2/storage_orm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-07 10:14:06.000000 storage_orm-1.4.2/storage_orm/operation_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:16.729122 storage_orm-1.4.2/storage_orm/redis_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 10:14:06.000000 storage_orm-1.4.2/storage_orm/redis_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-06-07 10:14:06.000000 storage_orm-1.4.2/storage_orm/redis_impl/redis_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-06-07 10:14:06.000000 storage_orm-1.4.2/storage_orm/redis_impl/redis_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-07 10:14:06.000000 storage_orm-1.4.2/storage_orm/redis_impl/redis_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-07 10:14:06.000000 storage_orm-1.4.2/storage_orm/storage_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-07 10:14:06.000000 storage_orm-1.4.2/storage_orm/storage_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-07 10:14:06.000000 storage_orm-1.4.2/storage_orm/storage_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:16.729122 storage_orm-1.4.2/storage_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-06-07 10:14:16.000000 storage_orm-1.4.2/storage_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-07 10:14:16.000000 storage_orm-1.4.2/storage_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:14:16.000000 storage_orm-1.4.2/storage_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 10:14:16.000000 storage_orm-1.4.2/storage_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 10:14:16.000000 storage_orm-1.4.2/storage_orm.egg-info/top_level.txt
```

### Comparing `storage_orm-1.4.1/PKG-INFO` & `storage_orm-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storage_orm
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/storage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/storage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `storage_orm-1.4.1/README.md` & `storage_orm-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.1/setup.py` & `storage_orm-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.1/storage_orm/operation_result.py` & `storage_orm-1.4.2/storage_orm/operation_result.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.1/storage_orm/redis_impl/redis_frame.py` & `storage_orm-1.4.2/storage_orm/redis_impl/redis_frame.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.1/storage_orm/redis_impl/redis_item.py` & `storage_orm-1.4.2/storage_orm/redis_impl/redis_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,17 +52,19 @@
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

### Comparing `storage_orm-1.4.1/storage_orm/redis_impl/redis_orm.py` & `storage_orm-1.4.2/storage_orm/redis_impl/redis_orm.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.1/storage_orm/storage_frame.py` & `storage_orm-1.4.2/storage_orm/storage_frame.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.1/storage_orm/storage_item.py` & `storage_orm-1.4.2/storage_orm/storage_item.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.1/storage_orm/storage_orm.py` & `storage_orm-1.4.2/storage_orm/storage_orm.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.4.1/storage_orm.egg-info/PKG-INFO` & `storage_orm-1.4.2/storage_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storage-orm
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/storage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/storage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

