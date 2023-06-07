# Comparing `tmp/better-translation-0.4.3.tar.gz` & `tmp/better-translation-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better-translation-0.4.3.tar", last modified: Thu May 11 16:45:01 2023, max compression
+gzip compressed data, was "better-translation-0.4.4.tar", last modified: Wed Jun  7 21:14:34 2023, max compression
```

## Comparing `better-translation-0.4.3.tar` & `better-translation-0.4.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.171024 better-translation-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 16:45:01.171024 better-translation-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 16:44:56.000000 better-translation-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.167024 better-translation-0.4.3/better_translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.167024 better-translation-0.4.3/better_translation/_babel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/_babel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/_babel/lazy_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.167024 better-translation-0.4.3/better_translation/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.171024 better-translation-0.4.3/better_translation/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/integrations/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/integrations/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/integrations/django/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-11 16:44:56.000000 better-translation-0.4.3/better_translation/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:01.167024 better-translation-0.4.3/better_translation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 16:45:01.000000 better-translation-0.4.3/better_translation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-11 16:45:01.000000 better-translation-0.4.3/better_translation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:45:01.000000 better-translation-0.4.3/better_translation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 16:45:01.000000 better-translation-0.4.3/better_translation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-11 16:44:56.000000 better-translation-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:45:01.171024 better-translation-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 16:44:59.000000 better-translation-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:14:34.527711 better-translation-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 21:14:34.527711 better-translation-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-07 21:14:30.000000 better-translation-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:14:34.523711 better-translation-0.4.4/better_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:14:34.527711 better-translation-0.4.4/better_translation/_babel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/_babel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/_babel/lazy_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:14:34.527711 better-translation-0.4.4/better_translation/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:14:34.527711 better-translation-0.4.4/better_translation/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/integrations/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/integrations/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/integrations/django/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-07 21:14:30.000000 better-translation-0.4.4/better_translation/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:14:34.523711 better-translation-0.4.4/better_translation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 21:14:34.000000 better-translation-0.4.4/better_translation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-07 21:14:34.000000 better-translation-0.4.4/better_translation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:14:34.000000 better-translation-0.4.4/better_translation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 21:14:34.000000 better-translation-0.4.4/better_translation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-07 21:14:30.000000 better-translation-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:14:34.527711 better-translation-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-07 21:14:32.000000 better-translation-0.4.4/setup.py
```

### Comparing `better-translation-0.4.3/better_translation/_babel/lazy_proxy.py` & `better-translation-0.4.4/better_translation/_babel/lazy_proxy.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.3/better_translation/extractor.py` & `better-translation-0.4.4/better_translation/extractor.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.3/better_translation/integrations/django/admin.py` & `better-translation-0.4.4/better_translation/integrations/django/admin.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.3/better_translation/integrations/django/models.py` & `better-translation-0.4.4/better_translation/integrations/django/models.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.3/better_translation/integrations/django/storage.py` & `better-translation-0.4.4/better_translation/integrations/django/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,25 @@
                 )
                 continue
 
             logger.info("Adding message '%s' to the storage", message)
             self.storage[message.id] = message
             messages_to_create.add(self._get_message_model(message))
 
-        await self.message_model.objects.abulk_create(messages_to_create)
+        already_in_storage = self.message_model.objects.filter(
+            id__in={message.id for message in messages_to_create},
+        ).values_list("id", flat=True)
+
+        await self.message_model.objects.abulk_create(
+            [
+                message
+                for message in messages_to_create
+                if message.id not in already_in_storage
+            ],
+        )
 
     async def add_messages_from_dirs(
         self,
         *dirs: Path,
         update_messages_usage: bool = False,
     ) -> list[StorageMessage]:
         messages: list[StorageMessage] = []
```

### Comparing `better-translation-0.4.3/better_translation/provider.py` & `better-translation-0.4.4/better_translation/provider.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.3/better_translation/storage.py` & `better-translation-0.4.4/better_translation/storage.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.3/better_translation/translator.py` & `better-translation-0.4.4/better_translation/translator.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.3/better_translation.egg-info/SOURCES.txt` & `better-translation-0.4.4/better_translation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.3/pyproject.toml` & `better-translation-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `better-translation-0.4.3/setup.py` & `better-translation-0.4.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 _version = (
-    "0.4.3"  # Version will be replaced by the CD pipeline
+    "0.4.4"  # Version will be replaced by the CD pipeline
 )
 VERSION = "0.0.0" if _version.startswith("{{") else _version
 
 
 def get_readme() -> str:
     readme = Path("README.md")
     return readme.read_text(encoding="utf-8")
```

