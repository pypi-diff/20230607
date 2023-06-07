# Comparing `tmp/apapi-0.4.0.tar.gz` & `tmp/apapi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apapi-0.4.0.tar", last modified: Sun Feb  5 21:48:52 2023, max compression
+gzip compressed data, was "apapi-0.5.0.tar", last modified: Wed Jun  7 07:31:22 2023, max compression
```

## Comparing `apapi-0.4.0.tar` & `apapi-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-02-05 21:48:52.081288 apapi-0.4.0/
--rw-rw-rw-   0        0        0    11358 2022-03-13 09:53:51.000000 apapi-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     4067 2023-02-05 21:48:52.081288 apapi-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2718 2023-02-05 18:19:32.000000 apapi-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-05 21:48:52.050034 apapi-0.4.0/apapi/
--rw-rw-rw-   0        0        0      702 2023-02-05 17:26:39.000000 apapi-0.4.0/apapi/__init__.py
--rw-rw-rw-   0        0        0     9579 2023-02-05 17:26:39.000000 apapi-0.4.0/apapi/__main__.py
--rw-rw-rw-   0        0        0      377 2023-02-05 18:26:54.000000 apapi-0.4.0/apapi/__version__.py
--rw-rw-rw-   0        0        0     6448 2022-05-08 10:49:16.000000 apapi-0.4.0/apapi/alm.py
--rw-rw-rw-   0        0        0     2544 2023-02-05 13:02:03.000000 apapi-0.4.0/apapi/audit.py
--rw-rw-rw-   0        0        0     8142 2023-02-05 17:26:39.000000 apapi-0.4.0/apapi/authentication.py
--rw-rw-rw-   0        0        0     1722 2023-02-05 13:02:03.000000 apapi-0.4.0/apapi/basic_connection.py
--rw-rw-rw-   0        0        0    13674 2023-02-05 18:19:32.000000 apapi-0.4.0/apapi/bulk.py
--rw-rw-rw-   0        0        0      467 2023-02-05 13:02:03.000000 apapi-0.4.0/apapi/connection.py
--rw-rw-rw-   0        0        0    19430 2023-02-05 13:02:03.000000 apapi-0.4.0/apapi/transactional.py
--rw-rw-rw-   0        0        0     4408 2023-02-05 13:02:03.000000 apapi-0.4.0/apapi/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-05 21:48:52.065664 apapi-0.4.0/apapi.egg-info/
--rw-rw-rw-   0        0        0     4067 2023-02-05 21:48:51.000000 apapi-0.4.0/apapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-02-05 21:48:51.000000 apapi-0.4.0/apapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-05 21:48:51.000000 apapi-0.4.0/apapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-02-05 21:48:51.000000 apapi-0.4.0/apapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-02-05 21:48:51.000000 apapi-0.4.0/apapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-05 21:48:51.000000 apapi-0.4.0/apapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      121 2022-05-08 10:49:16.000000 apapi-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-05 21:48:52.081288 apapi-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2397 2023-02-05 17:42:44.000000 apapi-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:31:22.350196 apapi-0.5.0/
+-rw-rw-rw-   0        0        0    11358 2022-03-13 09:53:51.000000 apapi-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     4065 2023-06-07 07:31:22.350196 apapi-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2716 2023-06-07 07:08:13.000000 apapi-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 07:31:22.328044 apapi-0.5.0/apapi/
+-rw-rw-rw-   0        0        0      702 2023-02-05 17:26:39.000000 apapi-0.5.0/apapi/__init__.py
+-rw-rw-rw-   0        0        0     9579 2023-02-05 17:26:39.000000 apapi-0.5.0/apapi/__main__.py
+-rw-rw-rw-   0        0        0      377 2023-06-07 06:28:57.000000 apapi-0.5.0/apapi/__version__.py
+-rw-rw-rw-   0        0        0     6448 2022-05-08 10:49:16.000000 apapi-0.5.0/apapi/alm.py
+-rw-rw-rw-   0        0        0     2544 2023-02-05 13:02:03.000000 apapi-0.5.0/apapi/audit.py
+-rw-rw-rw-   0        0        0     8191 2023-04-23 18:48:27.000000 apapi-0.5.0/apapi/authentication.py
+-rw-rw-rw-   0        0        0     1722 2023-02-05 13:02:03.000000 apapi-0.5.0/apapi/basic_connection.py
+-rw-rw-rw-   0        0        0    14779 2023-04-23 15:00:47.000000 apapi-0.5.0/apapi/bulk.py
+-rw-rw-rw-   0        0        0      467 2023-02-05 13:02:03.000000 apapi-0.5.0/apapi/connection.py
+-rw-rw-rw-   0        0        0    19813 2023-04-23 14:50:48.000000 apapi-0.5.0/apapi/transactional.py
+-rw-rw-rw-   0        0        0     4408 2023-02-05 13:02:03.000000 apapi-0.5.0/apapi/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:31:22.350196 apapi-0.5.0/apapi.egg-info/
+-rw-rw-rw-   0        0        0     4065 2023-06-07 07:31:21.000000 apapi-0.5.0/apapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-07 07:31:22.000000 apapi-0.5.0/apapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 07:31:21.000000 apapi-0.5.0/apapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-07 07:31:21.000000 apapi-0.5.0/apapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-06-07 07:31:22.000000 apapi-0.5.0/apapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 07:31:22.000000 apapi-0.5.0/apapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      121 2022-05-08 10:49:16.000000 apapi-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 07:31:22.350196 apapi-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     2397 2023-02-05 17:42:44.000000 apapi-0.5.0/setup.py
```

### Comparing `apapi-0.4.0/LICENSE` & `apapi-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apapi-0.4.0/PKG-INFO` & `apapi-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apapi
-Version: 0.4.0
+Version: 0.5.0
 Summary: Unofficial Anaplan API Python client library
 Home-page: https://github.com/DLZaan/apapi
 Author: Milosz Kierepka
 Author-email: milosz.kierepka+work@gmail.com
 Maintainer: Milosz Kierepka
 Maintainer-email: milosz.kierepka+work@gmail.com
 License: Apache 2.0
@@ -43,15 +43,15 @@
 As an abstract example, here we export some CSV and import it back to Anaplan:
 
 ```python
 >> > import apapi
 >> > with apapi.BasicAuth(f"{email}:{password}") as authentication:
     >> > my_connection = apapi.BulkConnection(authentication)
 >> > my_connection.run_export(model_id, export_id)
->> > data = my_connection.download_file(model_id, export_id)
+>> > data = my_connection.get_file(model_id, export_id)
 >> > print(data.decode())
 Versions, Data, Text
 Actual, 1, test
 Budget, 2.5, ąćęłńśżź
 Forecast, -3,😂
 >> > my_connection.put_file(model_id, file_id, data)
 >> > my_connection.run_import(model_id, import_id)
@@ -68,15 +68,15 @@
 $ python -m pip install apapi
 ```
 APAPI supports Python 3.9+.
 
 ## More Info
 - [Official Anaplan APIs Postman Collection](https://www.postman.com/apiplan/workspace/official-anaplan-collection/overview)
 - [Official documentation of Anaplan APIs](https://help.anaplan.com/da432e9b-24dd-4884-a70e-a3e409201e5c-Anaplan-API)
-- [Official documentation of Anaplan Connect V4 (Java)](https://anaplanenablement.s3.amazonaws.com/Community/Anapedia/Anaplan_Connect._User_Guide_v4.0.3.pdf)
+- [Official documentation of Anaplan Connect V4 (Java)](https://anaplanenablement.s3.amazonaws.com/Community/Anapedia/Anaplan-Connector-Informatica-V.4.2.1.pdf)
 - [Official Anaplan Connect repository](https://github.com/anaplaninc/anaplan-java-client)
 
 ## How to Contribute
 
 Contributions are welcome, even if you can't code it - in such case, please submit 
 an issue if you need any additional feature (preferably in the form of User Story, 
 like *"As {who} I need {what} because {why}"*).
```

### Comparing `apapi-0.4.0/README.md` & `apapi-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 As an abstract example, here we export some CSV and import it back to Anaplan:
 
 ```python
 >> > import apapi
 >> > with apapi.BasicAuth(f"{email}:{password}") as authentication:
     >> > my_connection = apapi.BulkConnection(authentication)
 >> > my_connection.run_export(model_id, export_id)
->> > data = my_connection.download_file(model_id, export_id)
+>> > data = my_connection.get_file(model_id, export_id)
 >> > print(data.decode())
 Versions, Data, Text
 Actual, 1, test
 Budget, 2.5, ąćęłńśżź
 Forecast, -3,😂
 >> > my_connection.put_file(model_id, file_id, data)
 >> > my_connection.run_import(model_id, import_id)
@@ -34,15 +34,15 @@
 $ python -m pip install apapi
 ```
 APAPI supports Python 3.9+.
 
 ## More Info
 - [Official Anaplan APIs Postman Collection](https://www.postman.com/apiplan/workspace/official-anaplan-collection/overview)
 - [Official documentation of Anaplan APIs](https://help.anaplan.com/da432e9b-24dd-4884-a70e-a3e409201e5c-Anaplan-API)
-- [Official documentation of Anaplan Connect V4 (Java)](https://anaplanenablement.s3.amazonaws.com/Community/Anapedia/Anaplan_Connect._User_Guide_v4.0.3.pdf)
+- [Official documentation of Anaplan Connect V4 (Java)](https://anaplanenablement.s3.amazonaws.com/Community/Anapedia/Anaplan-Connector-Informatica-V.4.2.1.pdf)
 - [Official Anaplan Connect repository](https://github.com/anaplaninc/anaplan-java-client)
 
 ## How to Contribute
 
 Contributions are welcome, even if you can't code it - in such case, please submit 
 an issue if you need any additional feature (preferably in the form of User Story, 
 like *"As {who} I need {what} because {why}"*).
```

### Comparing `apapi-0.4.0/apapi/__init__.py` & `apapi-0.5.0/apapi/__init__.py`

 * *Files identical despite different names*

### Comparing `apapi-0.4.0/apapi/__main__.py` & `apapi-0.5.0/apapi/__main__.py`

 * *Files identical despite different names*

### Comparing `apapi-0.4.0/apapi/alm.py` & `apapi-0.5.0/apapi/alm.py`

 * *Files identical despite different names*

### Comparing `apapi-0.4.0/apapi/audit.py` & `apapi-0.5.0/apapi/audit.py`

 * *Files identical despite different names*

### Comparing `apapi-0.4.0/apapi/authentication.py` & `apapi-0.5.0/apapi/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 
     def close(self) -> None:
         """Logout from Anaplan Authentication Service."""
         try:
             if self._timer:
                 self._timer.cancel()
             self.session.post(f"{self._auth_url}/token/logout")
+            logging.info(f"Logout successful!")
         finally:
             self.session.close()
 
 
 class BasicAuth(AbstractAuth):
     """Basic Authentication - use email and password to obtain API token."""
```

### Comparing `apapi-0.4.0/apapi/basic_connection.py` & `apapi-0.5.0/apapi/basic_connection.py`

 * *Files identical despite different names*

### Comparing `apapi-0.4.0/apapi/bulk.py` & `apapi-0.5.0/apapi/bulk.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,37 +65,39 @@
             {"showImportDataSource": self.details if details is None else details},
         )
 
     # Files manipulation
     def put_file(self, model_id: str, file_id: str, data: bytes) -> Response:
         """Upload file in one go.
 
-        **WARNING**: For bigger files (or if this method fails) methods that upload file
-        chunk by chunk should be used instead.
+        **WARNING**: For bigger files (or if this method fails)
+        BulkConnection.upload_file() should be used instead.
         """
         return self.request(
             "PUT",
             f"{self._api_main_url}/models/{model_id}/files/{file_id}",
             data=data,
             headers={"Content-Type": MIMEType.APP_8STREAM.value},
         )
 
-    def set_file_chunk_count(self, model_id: str, file_id: str, count: int) -> Response:
+    def _set_file_chunk_count(
+        self, model_id: str, file_id: str, count: int
+    ) -> Response:
         """Set file chunk count before uploading content in chunks.
 
         If you don't know how many chunks the file will have, set count to -1.
         Chunks should have size between 1 and 50 MBs.
         """
         return self.request(
             "POST",
             f"{self._api_main_url}/models/{model_id}/files/{file_id}",
             data=json.dumps({"chunkCount": count}),
         )
 
-    def upload_file_chunk(
+    def _upload_file_chunk(
         self,
         model_id: str,
         file_id: str,
         data: bytes,
         chunk: int,
         content_type: MIMEType = MIMEType.APP_8STREAM,
     ) -> Response:
@@ -103,50 +105,73 @@
         return self.request(
             "PUT",
             f"{self._api_main_url}/models/{model_id}/files/{file_id}/chunks/{chunk}",
             data=data,
             headers={"Content-Type": content_type.value},
         )
 
-    def set_file_upload_complete(self, model_id: str, file_id: str) -> Response:
+    def _set_file_upload_complete(self, model_id: str, file_id: str) -> Response:
         """Finalize upload in chunks by setting it as complete."""
         return self.request(
             "POST",
             f"{self._api_main_url}/models/{model_id}/files/{file_id}/complete",
             data=json.dumps({"id": file_id}),
         )
 
+    def upload_file(
+        self,
+        model_id: str,
+        file_id: str,
+        data: [bytes],
+        content_type: MIMEType = MIMEType.APP_8STREAM,
+    ) -> Response:
+        """Upload file (to be used by an import action) chunk by chunk.
+
+        Tip: For smaller files, much faster method (only one request is sent)
+        BulkConnection.put_file() can be used instead.
+        """
+        self._set_file_chunk_count(model_id, file_id, -1)
+        for chunk_count, chunk in enumerate(data):
+            self._upload_file_chunk(model_id, file_id, chunk, chunk_count, content_type)
+        return self._set_file_upload_complete(model_id, file_id)
+
     def get_file(self, model_id: str, file_id: str) -> Response:
         """Download file (uploaded or generated by an export action) in one go.
 
         **WARNING**: For bigger files (or if this method fails)
         BulkConnection.download_file() should be used instead.
         """
         return self.request(
             "GET",
             f"{self._api_main_url}/models/{model_id}/files/{file_id}",
             headers={"Accept": MIMEType.APP_8STREAM.value},
         )
 
-    def download_file(self, model_id: str, file_id: str) -> bytes:
+    def _get_chunks(self, model_id: str, file_id: str) -> Response:
+        """Get number of chunks available for an export."""
+        url = f"{self._api_main_url}/models/{model_id}/files/{file_id}/chunks"
+        response = self.request("GET", url)
+        if not response.json()["meta"]["paging"]["currentPageSize"]:
+            raise Exception("Missing part in request response", url, response.text)
+        return response
+
+    def _get_chunk(self, model_id: str, file_id: str, chunk: int) -> Response:
+        """Get number of chunks available for an export."""
+        url = f"{self._api_main_url}/models/{model_id}/files/{file_id}/chunks/{chunk}"
+        return self.request("GET", url, headers={"Accept": MIMEType.APP_8STREAM.value})
+
+    def download_file(self, model_id: str, file_id: str) -> [bytes]:
         """Download file (uploaded or generated by an export action) chunk by chunk.
 
         Tip: For smaller files, much faster method (only one request is sent)
         BulkConnection.get_file() can be used instead.
         """
-        url = f"{self._api_main_url}/models/{model_id}/files/{file_id}/chunks"
-        response = self.request("GET", url)
-        if not response.json()["meta"]["paging"]["currentPageSize"]:
-            raise Exception("Missing part in request response", url, response.text)
-        return b"".join(
-            self.request(
-                "GET",
-                f"{url}/{chunk_id['id']}",
-                headers={"Accept": MIMEType.APP_8STREAM.value},
-            ).content
+        response = self._get_chunks(model_id, file_id)
+        return (
+            self._get_chunk(model_id, file_id, int(chunk_id["id"])).content
             for chunk_id in response.json()["chunks"]
         )
 
     def delete_file(self, model_id: str, file_id: str) -> Response:
         """Delete previously uploaded file from the model's memory."""
         return self.request(
             "DELETE",
```

### Comparing `apapi-0.4.0/apapi/transactional.py` & `apapi-0.5.0/apapi/transactional.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,26 @@
             {"modelDetails": self.details if details is None else details},
         )
 
     def get_user_models(self, user_id: str) -> Response:
         """Get info about all models to which a specified user has access."""
         return self.request("GET", f"{self._api_main_url}/users/{user_id}/models")
 
+    def delete_models(self, workspace_id: str, models_ids: [str]) -> Response:
+        """Delete models from a workspace.
+
+        **WARNING**: This query is destructive - use with caution! It will only work on
+        closed models - you can close a model in Anaplan web interface via Manage Tasks.
+        """
+        return self.request(
+            "POST",
+            f"{self._api_main_url}/workspaces/{workspace_id}/bulkDeleteModels",
+            data=json.dumps({"modelIdsToDelete": models_ids}),
+        )
+
     # Calendar
     def get_fiscal_year(self, model_id: str):
         """Get current fiscal year setting for a specified model."""
         return self.request(
             "GET", f"{self._api_main_url}/models/{model_id}/modelCalendar"
         )
 
@@ -263,19 +275,17 @@
             "POST",
             f"{self._api_main_url}/models/{model_id}/lists/{list_id}/items",
             {"action": "delete"},
             json.dumps({"items": data}),
         )
 
     def reset_list_index(self, model_id: str, list_id: str) -> Response:
-        """Try to reset index of a specified numbered list.
+        """Reset index of a specified numbered list.
 
-        **WARNING**: This action works only for numbered lists, and only if the index
-        is at least 900 million. You can check current value of nextItemIndex using
-        TransactionalConnection.get_list().
+        **WARNING**: This action works only for numbered lists that are empty.
         """
         return self.request(
             "POST", f"{self._api_main_url}/models/{model_id}/lists/{list_id}/resetIndex"
         )
 
     # Modules
     def get_modules(self, model_id: str) -> Response:
```

### Comparing `apapi-0.4.0/apapi/utils.py` & `apapi-0.5.0/apapi/utils.py`

 * *Files identical despite different names*

### Comparing `apapi-0.4.0/apapi.egg-info/PKG-INFO` & `apapi-0.5.0/apapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apapi
-Version: 0.4.0
+Version: 0.5.0
 Summary: Unofficial Anaplan API Python client library
 Home-page: https://github.com/DLZaan/apapi
 Author: Milosz Kierepka
 Author-email: milosz.kierepka+work@gmail.com
 Maintainer: Milosz Kierepka
 Maintainer-email: milosz.kierepka+work@gmail.com
 License: Apache 2.0
@@ -43,15 +43,15 @@
 As an abstract example, here we export some CSV and import it back to Anaplan:
 
 ```python
 >> > import apapi
 >> > with apapi.BasicAuth(f"{email}:{password}") as authentication:
     >> > my_connection = apapi.BulkConnection(authentication)
 >> > my_connection.run_export(model_id, export_id)
->> > data = my_connection.download_file(model_id, export_id)
+>> > data = my_connection.get_file(model_id, export_id)
 >> > print(data.decode())
 Versions, Data, Text
 Actual, 1, test
 Budget, 2.5, ąćęłńśżź
 Forecast, -3,😂
 >> > my_connection.put_file(model_id, file_id, data)
 >> > my_connection.run_import(model_id, import_id)
@@ -68,15 +68,15 @@
 $ python -m pip install apapi
 ```
 APAPI supports Python 3.9+.
 
 ## More Info
 - [Official Anaplan APIs Postman Collection](https://www.postman.com/apiplan/workspace/official-anaplan-collection/overview)
 - [Official documentation of Anaplan APIs](https://help.anaplan.com/da432e9b-24dd-4884-a70e-a3e409201e5c-Anaplan-API)
-- [Official documentation of Anaplan Connect V4 (Java)](https://anaplanenablement.s3.amazonaws.com/Community/Anapedia/Anaplan_Connect._User_Guide_v4.0.3.pdf)
+- [Official documentation of Anaplan Connect V4 (Java)](https://anaplanenablement.s3.amazonaws.com/Community/Anapedia/Anaplan-Connector-Informatica-V.4.2.1.pdf)
 - [Official Anaplan Connect repository](https://github.com/anaplaninc/anaplan-java-client)
 
 ## How to Contribute
 
 Contributions are welcome, even if you can't code it - in such case, please submit 
 an issue if you need any additional feature (preferably in the form of User Story, 
 like *"As {who} I need {what} because {why}"*).
```

### Comparing `apapi-0.4.0/setup.py` & `apapi-0.5.0/setup.py`

 * *Files identical despite different names*

