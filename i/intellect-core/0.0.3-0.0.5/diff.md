# Comparing `tmp/intellect_core-0.0.3.tar.gz` & `tmp/intellect_core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellect_core-0.0.3.tar", max compression
+gzip compressed data, was "intellect_core-0.0.5.tar", max compression
```

## Comparing `intellect_core-0.0.3.tar` & `intellect_core-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      186 2023-05-29 14:14:55.721473 intellect_core-0.0.3/LICENSE
--rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 intellect_core-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-29 14:10:28.656955 intellect_core-0.0.3/intellect_core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 12:57:45.552839 intellect_core-0.0.3/intellect_core/dto/__init__.py
--rw-r--r--   0        0        0     2206 2023-05-29 13:41:30.018001 intellect_core-0.0.3/intellect_core/dto/dto.py
--rw-r--r--   0        0        0     1054 2023-05-29 13:52:44.564262 intellect_core-0.0.3/intellect_core/handler.py
--rw-r--r--   0        0        0     4949 2023-05-29 14:22:25.988170 intellect_core-0.0.3/intellect_core/intelletct_server.py
--rw-r--r--   0        0        0      307 2023-05-29 14:22:25.996170 intellect_core-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-05-29 14:14:55.721473 intellect_core-0.0.5/LICENSE
+-rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 intellect_core-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 14:10:28.656955 intellect_core-0.0.5/intellect_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:57:45.552839 intellect_core-0.0.5/intellect_core/dto/__init__.py
+-rw-r--r--   0        0        0     2256 2023-05-31 10:07:28.656329 intellect_core-0.0.5/intellect_core/dto/dto.py
+-rw-r--r--   0        0        0     1023 2023-05-29 14:54:49.902384 intellect_core-0.0.5/intellect_core/handler.py
+-rw-r--r--   0        0        0     5326 2023-06-05 13:45:54.484953 intellect_core-0.0.5/intellect_core/intelletct_server.py
+-rw-r--r--   0        0        0      307 2023-06-07 13:25:06.883999 intellect_core-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.0.5/PKG-INFO
```

### Comparing `intellect_core-0.0.3/intellect_core/dto/dto.py` & `intellect_core-0.0.5/intellect_core/dto/dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 class IntellectConfigDto(BaseModel):
     intellect_host: str
     intellect_port: int
     host_user: str
     host_password: str
     token_expires: int  # seconds
     access_level: int
+    access_department_id: int  # for temp pass
 
 
 class IntellectVisitDto:
     class Create(BaseModel):
         objid: int
         name: str | None  # second_name
         surname: str | None  # first_name
@@ -75,13 +76,13 @@
         level_id: str | None
         region_id: str | None
         external_id: str | None
         owner_id: str | None
 
     class Update(BaseModel):
         schedule_id: str | None
-        id: str | None
+        objid: str | None
         name: str | None
         level_id: str | None
         region_id: str | None
         external_id: str | None
         owner_id: str | None
```

### Comparing `intellect_core-0.0.3/intellect_core/handler.py` & `intellect_core-0.0.5/intellect_core/handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from enum import Enum
 from typing import Dict
 
-from pydantic import BaseModel
 
 
 class IntellectError(Exception):
     error_type: str = "IntellectIntegrationError"
     default_class: int = 999
     default_subclass: int = 999
     context: Dict[str, str | int] = None
```

### Comparing `intellect_core-0.0.3/intellect_core/intelletct_server.py` & `intellect_core-0.0.5/intellect_core/intelletct_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import json
-
+from datetime import datetime, timedelta
 from aiohttp import ClientSession, ClientTimeout, ClientResponse
 from loguru import logger
 
 from intellect_core.dto.dto import IntellectConfigDto, \
     CoreCommand, \
     ObjectType, \
     IntellectVisitDto, \
     AutarizationInfo, \
     IntellectDepartmentDto
-from handler import IntellectError, ErrorClass, ErrorSubClass
+from intellect_core.handler import IntellectError, ErrorClass, ErrorSubClass
 
 
 class IntellectWebServer:
     log_debug: bool = False
-    session: ClientSession
     config: IntellectConfigDto
     autarization_info: AutarizationInfo
-
+    expire_token_date: str
     # =====================================================================================================================
 
     async def _wrap_response(self, response: ClientResponse):
         await response.read()
         if (await response.json()).get("Status") == "ERROR":
             logger.error(await response.json())
         if self.log_debug:
@@ -39,63 +38,71 @@
 
             return url[0:-1]
         else:
             url = url + f"objid<{objid}>"
             return url
 
     # =====================================================================================================================
-    async def _autorization(self):
+    async def autorization(self):
+        session = ClientSession()
         url = f"http://{self.config.host_user}:{self.config.host_password}@{self.config.intellect_host}:{self.config.intellect_port}/token?expires_in={self.config.token_expires}"
         try:
-            async with self.session.request(method="GET", url=url) as response:
+            async with session.request(method="GET", url=url) as response:
                 string = "{" + (await response.text()).replace("\n", ",")[2:-2] + "}"
                 self.autarization_info = AutarizationInfo(**json.loads(string))
+                self.expire_token_date = datetime.now() + timedelta(seconds=self.autarization_info.expires_in)
+                await session.close()
                 if self.log_debug:
                     logger.debug(f"\nresponse_body: {bytes(await response.read()).decode()}\nresponse: {response}")
         except OSError as e:
+            await session.close()
             logger.error(f"Intellect connection error: {e}")
+        if response.status == 200:
+            logger.info("Starting intellect_core")
+        await session.close()
 
     # =====================================================================================================================
     async def init(self, intellect_config: IntellectConfigDto):
-        self.session = ClientSession()
         self.config = intellect_config
-        self.session._timeout = ClientTimeout(total=intellect_config.token_expires)
-        await self._autorization()
-        logger.info("Starting intellect_core")
+
 
     async def logic(self, object_type: ObjectType,
                     command: CoreCommand,
                     dto: IntellectVisitDto.Create |
                          IntellectVisitDto.Update |
                          IntellectDepartmentDto.Create |
                          IntellectDepartmentDto.Update = None,
                     objid: int = None) -> None:
-
+        session = ClientSession()
         match command:
             case CoreCommand.CREATE | CoreCommand.UPDATE:
                 if dto:
                     dto.level_id = self.config.access_level
                     url = self._get_url(object_type, command, dto, None)
                     try:
-                        async with self.session.request(method="GET", url=url) as response:
+                        async with session.request(method="GET", url=url) as response:
                             await self._wrap_response(response)
+                            await session.close()
                     except OSError as e:
+                        await session.close()
                         logger.error(f"Intellect connection error: {e}")
                 else:
-                    await self.session.close()
+                    await session.close()
                     raise IntellectError(message="You need set dto for update or create object",
                                          context={"class": ErrorClass.CREATE_OR_UPDATE,
                                                   "subclass": ErrorSubClass.DTO_NOT_FOUND})
             case CoreCommand.DELETE:
                 if objid:
                     url = self._get_url(object_type, command, None, objid)
                     try:
-                        async with self.session.request(method="GET",
-                                                        url=url) as response:
+                        async with session.request(method="GET",
+                                                   url=url) as response:
                             await self._wrap_response(response)
+                            await session.close()
                     except OSError as e:
+                        await session.close()
                         logger.error(f"Intellect connection error: {e}")
                 else:
-                    await self.session.close()
+                    await session.close()
                     raise IntellectError(message="You need set object id for delete object",
                                          context={"class": ErrorClass.DELETE,
                                                   "subclass": ErrorSubClass.OBJECT_ID_NOT_FOUND})
```

### Comparing `intellect_core-0.0.3/PKG-INFO` & `intellect_core-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellect-core
-Version: 0.0.3
+Version: 0.0.5
 Summary: Модуль интеграции с Интеллект
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

