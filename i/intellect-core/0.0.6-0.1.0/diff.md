# Comparing `tmp/intellect_core-0.0.6.tar.gz` & `tmp/intellect_core-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellect_core-0.0.6.tar", max compression
+gzip compressed data, was "intellect_core-0.1.0.tar", max compression
```

## Comparing `intellect_core-0.0.6.tar` & `intellect_core-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      186 2023-05-29 14:14:55.721473 intellect_core-0.0.6/LICENSE
--rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 intellect_core-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-05-29 14:10:28.656955 intellect_core-0.0.6/intellect_core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 12:57:45.552839 intellect_core-0.0.6/intellect_core/dto/__init__.py
--rw-r--r--   0        0        0     2256 2023-05-31 10:07:28.656329 intellect_core-0.0.6/intellect_core/dto/dto.py
--rw-r--r--   0        0        0     1023 2023-05-29 14:54:49.902384 intellect_core-0.0.6/intellect_core/handler.py
--rw-r--r--   0        0        0     5212 2023-06-07 14:32:28.898164 intellect_core-0.0.6/intellect_core/intelletct_server.py
--rw-r--r--   0        0        0      307 2023-06-07 14:32:28.902164 intellect_core-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-05-29 14:14:55.721473 intellect_core-0.1.0/LICENSE
+-rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 intellect_core-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 14:10:28.656955 intellect_core-0.1.0/intellect_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:57:45.552839 intellect_core-0.1.0/intellect_core/dto/__init__.py
+-rw-r--r--   0        0        0     2256 2023-05-31 10:07:28.656329 intellect_core-0.1.0/intellect_core/dto/dto.py
+-rw-r--r--   0        0        0     1023 2023-05-29 14:54:49.902384 intellect_core-0.1.0/intellect_core/handler.py
+-rw-r--r--   0        0        0     5209 2023-06-07 15:02:30.337406 intellect_core-0.1.0/intellect_core/intelletct_server.py
+-rw-r--r--   0        0        0      307 2023-06-07 15:03:10.172964 intellect_core-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.1.0/PKG-INFO
```

### Comparing `intellect_core-0.0.6/intellect_core/dto/dto.py` & `intellect_core-0.1.0/intellect_core/dto/dto.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.0.6/intellect_core/handler.py` & `intellect_core-0.1.0/intellect_core/handler.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.0.6/intellect_core/intelletct_server.py` & `intellect_core-0.1.0/intellect_core/intelletct_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,17 +52,14 @@
                 self.expire_token_date = datetime.now() + timedelta(seconds=self.autarization_info.expires_in)
                 await session.close()
                 if self.log_debug:
                     logger.debug(f"\nresponse_body: {bytes(await response.read()).decode()}\nresponse: {response}")
         except OSError as e:
             await session.close()
             logger.error(f"Intellect connection error: {e}")
-
-
-
     # =====================================================================================================================
     async def init(self, intellect_config: IntellectConfigDto):
         self.config = intellect_config
 
 
     async def logic(self, object_type: ObjectType,
                     command: CoreCommand,
```

### Comparing `intellect_core-0.0.6/PKG-INFO` & `intellect_core-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellect-core
-Version: 0.0.6
+Version: 0.1.0
 Summary: Модуль интеграции с Интеллект
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

