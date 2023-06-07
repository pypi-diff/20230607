# Comparing `tmp/googleapiutils2-0.8.5.tar.gz` & `tmp/googleapiutils2-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.8.5.tar", max compression
+gzip compressed data, was "googleapiutils2-0.9.1.tar", max compression
```

## Comparing `googleapiutils2-0.8.5.tar` & `googleapiutils2-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.8.5/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.8.5/README.md
--rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.8.5/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.8.5/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.8.5/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.8.5/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.8.5/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.8.5/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.8.5/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.8.5/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     9618 2023-06-02 19:09:36.958908 googleapiutils2-0.8.5/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    33788 2023-06-02 18:38:16.312935 googleapiutils2-0.8.5/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     5219 2023-06-02 18:15:23.863635 googleapiutils2-0.8.5/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     8927 2023-06-02 01:08:13.754688 googleapiutils2-0.8.5/googleapiutils2/utils.py
--rw-r--r--   0        0        0     1067 2023-06-02 19:09:48.641713 googleapiutils2-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.9.1/README.md
+-rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.9.1/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.9.1/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    21607 2023-06-07 18:11:07.739854 googleapiutils2-0.9.1/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-06-07 16:12:16.848980 googleapiutils2-0.9.1/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.9.1/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.9.1/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.9.1/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.9.1/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     9618 2023-06-02 19:09:36.958908 googleapiutils2-0.9.1/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    33736 2023-06-07 18:16:28.569445 googleapiutils2-0.9.1/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     5219 2023-06-02 18:15:23.863635 googleapiutils2-0.9.1/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     9382 2023-06-07 18:28:48.824156 googleapiutils2-0.9.1/googleapiutils2/utils.py
+-rw-r--r--   0        0        0     1089 2023-06-07 18:29:05.357587 googleapiutils2-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.9.1/PKG-INFO
```

### Comparing `googleapiutils2-0.8.5/LICENSE` & `googleapiutils2-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.5/README.md` & `googleapiutils2-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.5/googleapiutils2/drive/drive.py` & `googleapiutils2-0.9.1/googleapiutils2/drive/drive.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 class Drive:
     def __init__(self, creds: Credentials):
         self.creds = creds
         self.service: DriveResource = discovery.build(
             "drive", VERSION, credentials=self.creds
-        )
+        )  # type: ignore
         self.files: DriveResource.FilesResource = self.service.files()
 
     def get(self, file_id: str, fields: str = "*", **kwargs: Any) -> File:
         """Get a file by its ID."""
         file_id = parse_file_id(file_id)
         return self.files.get(fileId=file_id, fields=fields, **kwargs).execute()
 
@@ -54,33 +54,36 @@
             parents (List[str]): The ID(s) of the parent folder(s).
             q (str, optional): A query string to filter the results. Defaults to None.
         """
         parents = list(map(parse_file_id, parents)) if parents is not None else []
         return next(self._query_children(name=name, parents=parents, q=q), None)
 
     def _download(self, file_id: str, out_filepath: Path, mime_type: GoogleMimeTypes):
-        request = self.files.export_media(fileId=file_id, mimeType=mime_type.value)
+        request = self.files.export_media(fileId=file_id, mimeType=mime_type.value)  # type: ignore
         with out_filepath.open("wb") as out_file:
             downloader = googleapiclient.http.MediaIoBaseDownload(out_file, request)
             done = False
             while done is False:
                 status, done = downloader.next_chunk()
+
         return out_filepath
 
     def _download_nested_filepath(
         self,
         out_filepath: FilePath,
         file_id: str,
-    ) -> None:
+    ) -> Path:
         """Internal usage function. Download a folder given by "out_filepath" and its contents recursively.
 
         Args:
             out_filepath (FilePath): The path to the folder to download to.
             file_id (str): The ID of the folder to download.
         """
+        out_filepath = Path(out_filepath)
+
         for file in self.list_children(file_id):
             t_name, t_file_id, t_mime_type = (
                 file["name"],
                 file["id"],
                 GoogleMimeTypes(file["mimeType"]),
             )
             t_out_filepath = out_filepath.joinpath(t_name)
@@ -104,15 +107,15 @@
         file_id: str,
         mime_type: GoogleMimeTypes,
         recursive: bool = False,
         conversion_map: dict[
             GoogleMimeTypes, tuple[GoogleMimeTypes, str]
         ] = DEFAULT_DOWNLOAD_CONVERSION_MAP,
     ) -> Path:
-        """Download a file from Google Drive. If the file is larger than 10MB, it will be downloaded in chunks.
+        """Download a file from Google Drive. If the file is larger than 10MB, it's downloaded in chunks.
 
         Args:
             out_filepath (FilePath): The path to the file to download to.
             file_id (str): The ID of the file to download.
             mime_type (GoogleMimeTypes): The mime type of the file to download.
             recursive (bool, optional): If the file is a folder, download its contents recursively. Defaults to False.
             conversion_map (dict[GoogleMimeTypes, tuple[GoogleMimeTypes, str]], optional): A dictionary mapping mime types to their corresponding file extensions. Defaults to DEFAULT_DOWNLOAD_CONVERSION_MAP.
@@ -131,66 +134,44 @@
 
         if float(file["size"]) >= DOWNLOAD_LIMIT:
             link = file["exportLinks"].get(mime_type.value, "")
             return download_large_file(url=link, filepath=out_filepath)
         else:
             return self._download(file_id, out_filepath, mime_type)
 
-    @staticmethod
-    def _upload_file_body(
-        name: str,
-        parents: List[str] | None = None,
-        body: File | None = None,
-        **kwargs: Any,
-    ) -> dict[str, File | Any]:
-        body = body if body is not None else {}
-        body = {"name": name, **body, **kwargs}
-        kwargs = {"body": body}
-
-        if parents is not None:
-            kwargs["body"].setdefault("parents", parents)
-
-        return kwargs
-
     def copy(
         self,
-        file_id: str,
-        to_filename: str,
+        from_file_id: str,
         to_folder_id: str,
+        to_filename: str | None = None,
         body: File | None = None,
         **kwargs: Any,
     ) -> File:
-        file_id = parse_file_id(file_id)
+        """Copy a file on Google Drive.
+
+        Args:
+            from_file_id (str): The ID of the file to copy.
+            to_folder_id (str): The ID of the folder to copy the file to.
+            to_filename (str, optional): The name of the copied file. Defaults to None, results in the same name as the original file.
+            body (File, optional): The body of the copied file. Defaults to None.
+            **kwargs (Any): Additional keyword arguments to pass to the API call.
+        """
+        from_file_id = parse_file_id(from_file_id)
         to_folder_id = parse_file_id(to_folder_id)
 
         kwargs = {
-            "fileId": file_id,
-            **self._upload_file_body(
-                name=to_filename, parents=[to_folder_id], body=body
-            ),
+            "fileId": from_file_id,
+            "body": body if body is not None else {},
             **kwargs,
         }
-        return self.files.copy(**kwargs).execute()
 
-    def update(
-        self,
-        file_id: str,
-        filepath: FilePath,
-        body: File | None = None,
-        **kwargs: Any,
-    ) -> File:
-        file_id = parse_file_id(file_id)
-        body = body if body is not None else {}
+        if to_filename is not None:
+            kwargs["body"]["name"] = to_filename
 
-        return self.files.update(
-            fileId=file_id,
-            media_body=str(filepath),
-            body=body,
-            **kwargs,
-        ).execute()
+        return self.files.copy(**kwargs).execute()
 
     @staticmethod
     def _list_fields(fields: str) -> str:
         if "*" in fields:
             return fields
 
         REQUIRED_FIELDS = ["nextPageToken", "kind"]
@@ -245,15 +226,15 @@
             pageToken=x,
             fields=self._list_fields(fields),
             orderBy=order_by,
             **kwargs,
         ).execute()
 
         for response in self._list(list_func):
-            yield from response.get("files", [])
+            yield from response.get("files", [])  # type: ignore
 
     def list_children(
         self, parent_id: str, fields: str = "*", **kwargs: Any
     ) -> Iterable[File]:
         """List files in a folder.
 
         Args:
@@ -280,27 +261,14 @@
 
         queries = [parents_list, names_list, "trashed = false"]
         if q is not None:
             queries.append(q)
         query = " and ".join((f"({i})" for i in queries))
         return self.list(query=query)
 
-    def _update_if_exists(
-        self,
-        name: str,
-        filepath: FilePath,
-        parents: List[str] | None = None,
-        team_drives: bool = True,
-    ) -> File | None:
-        if parents is None:
-            return None
-        for file in self._query_children(name=name, parents=parents):
-            return self.update(file["id"], filepath, supportsAllDrives=team_drives)
-        return None
-
     def _create_nested_folders(
         self, filepath: Path, parents: List[str], update: bool = True
     ) -> List[str]:
         """Create nested folders in Google Drive. Walks up the filepath creating folders as it goes.
 
         Args:
             filepath (Path): The filepath to create folders for.
@@ -313,101 +281,125 @@
                 name=name,
                 parents=parents,
                 q=f"mimeType='{GoogleMimeTypes.folder.value}'",
             )
             if update and (folder := next(folders, None)) is not None:
                 return folder
 
+            body: File = {
+                "name": dirname,
+                "parents": parents,
+                "mimeType": GoogleMimeTypes.folder.value,
+            }
             return self.files.create(
-                **self._upload_file_body(
-                    name=dirname,
-                    parents=parents,
-                    mimeType=GoogleMimeTypes.folder.value,
-                )
+                body=body,
             ).execute()
 
         for dirname in filepath.parts[:-1]:
             folder = create_or_get_if_exists(dirname, parents)
             parents = [folder["id"]]
 
         return parents
 
     def create(
         self,
         filepath: FilePath,
         mime_type: GoogleMimeTypes,
         parents: List[str] | None = None,
         create_folders: bool = False,
-        update: bool = False,
+        get_extant: bool = False,
         fields: str = "*",
         **kwargs: Any,
     ) -> File:
         """Create's a file on Google Drive.
 
+        For more information, see: https://developers.google.com/drive/api/v3/reference/files/create
+
         Args:
             filepath (FilePath): Filepath to the file to be uploaded.
             mime_type (GoogleMimeTypes): Mime type of the file.
             parents (List[str], optional): List of parent folder IDs wherein the file will be created. Defaults to None.
             create_folders (bool, optional): Create parent folders if they don't exist. Defaults to False.
-            update (bool, optional): Update the file if it already exists. Defaults to False.
+            get_extant (bool, optional): If a file with the same name already exists, return it. Defaults to False.
             fields (str, optional): Fields to be returned. Defaults to "*".
         """
         filepath = Path(filepath)
         parents = list(map(parse_file_id, parents)) if parents is not None else []
 
         if create_folders:
             parents = self._create_nested_folders(
-                filepath=filepath, parents=parents, update=update
+                filepath=filepath, parents=parents, update=get_extant
             )
+
         if (
-            update
-            and (file := next(self._query_children(filepath.name, parents), None))
+            get_extant
+            and (file := self.get_by_filename(filepath.name, parents=parents))
             is not None
         ):
             return file
 
-        kwargs = {
-            **self._upload_file_body(
-                name=filepath.name, parents=parents, mimeType=mime_type.value
-            ),
-            **kwargs,
+        kwargs |= {
+            "body": {
+                "name": filepath.name,
+            },
             "fields": fields,
         }
+        if parents is not None:
+            kwargs["body"]["parents"] = parents
+        if mime_type is not None:
+            kwargs["body"]["mimeType"] = mime_type.value
+
         file = self.files.create(**kwargs).execute()
         return file
 
     def delete(self, file_id: str, **kwargs: Any):
+        """Delete a file from Google Drive.
+        For more information, see: https://developers.google.com/drive/api/v3/reference/files/delete
+
+        Args:
+            file_id (str): The ID of the file to delete.
+        """
+        file_id = parse_file_id(file_id)
         return self.files.delete(fileId=file_id, **kwargs).execute()
 
     def _upload(
         self,
-        uploader: Callable,
+        uploader: Callable[[GoogleMimeTypes], Any],
         name: str,
         filepath: FilePath,
         mime_type: GoogleMimeTypes | None = None,
         parents: List[str] | None = None,
         body: File | None = None,
         update: bool = True,
         **kwargs,
     ) -> File:
         filepath = Path(filepath)
         parents = list(map(parse_file_id, parents)) if parents is not None else []
-        if (
-            update
-            and (file := self._update_if_exists(name, filepath, parents)) is not None
-        ):
-            return file
+        mime_type = (
+            mime_type
+            if mime_type is not None
+            else GoogleMimeTypes[filepath.suffix.lstrip(".")]
+        )
 
-        kwargs = {
-            **self._upload_file_body(
-                name=name, parents=parents, body=body, mimeType=mime_type.value
-            ),
-            **kwargs,
+        kwargs |= {
+            "body": body if body is not None else {},
+            "media_body": uploader(mime_type),
         }
-        kwargs["media_body"] = uploader()
+
+        if update and (file := self.get_by_filename(name, parents=parents)):
+            kwargs["fileId"] = file["id"]
+            return self.files.update(**kwargs).execute()
+
+        if name is not None:
+            kwargs["body"]["name"] = name
+        if parents is not None:
+            kwargs["body"]["parents"] = parents
+        if mime_type is not None:
+            kwargs["body"]["mimeType"] = mime_type.value
+
         return self.files.create(**kwargs).execute()
 
     def upload_file(
         self,
         filepath: FilePath,
         name: str | None = None,
         mime_type: GoogleMimeTypes | None = None,
@@ -426,22 +418,19 @@
             name (str, optional): The name of the file. Defaults to None, which will use the name of the file at the filepath.
             mime_type (GoogleMimeTypes, optional): The mime type of the file. Defaults to None, which will use the mime type of the file at the filepath.
             parents (List[str], optional): The list of parent IDs. Defaults to None.
             body (File, optional): The body of the file. Defaults to None.
             update (bool, optional): Whether to update the file if it already exists. Defaults to True.
         """
         filepath = Path(filepath)
-        mime_type = (
-            mime_type
-            if mime_type is not None
-            else GoogleMimeTypes[filepath.suffix.lstrip(".")]
-        )
 
-        def uploader():
-            return googleapiclient.http.MediaFileUpload(str(filepath), resumable=True)
+        def uploader(mime_type: GoogleMimeTypes):
+            return googleapiclient.http.MediaFileUpload(
+                str(filepath), resumable=True, mimetype=mime_type.value
+            )
 
         return self._upload(
             uploader=uploader,
             name=name if name is not None else filepath.name,
             filepath=filepath,
             mime_type=mime_type,
             parents=parents,
@@ -458,63 +447,91 @@
         parents: List[str] | None = None,
         body: File | None = None,
         update: bool = True,
         **kwargs: Any,
     ) -> File:
         """Uploads data to Google Drive. Bytes variant of `upload_file`
 
-        For more information on the File object (for the body, etc.), see https://developers.google.com/drive/api/v3/reference/files#resource
-
         Args:
             data (bytes): Data to upload
             name (str): Name of the file
             mime_type (GoogleMimeTypes): Mime type of the file
             parents (List[str], optional): List of parent IDs. Defaults to None.
             body (File, optional): File body. Defaults to None.
             update (bool, optional): Whether to update the file if it exists. Defaults to True.
         """
         with BytesIO(data) as tio:
 
-            def uploader():
-                return googleapiclient.http.MediaIoBaseUpload(tio, resumable=True)
+            def uploader(mime_type: GoogleMimeTypes):
+                return googleapiclient.http.MediaIoBaseUpload(
+                    tio, resumable=True, mimetype=mime_type.value
+                )
 
             return self._upload(
                 uploader=uploader,
                 name=name,
                 filepath=tio.name,
                 mime_type=mime_type,
                 parents=parents,
                 body=body,
                 update=update,
                 **kwargs,
             )
 
+    def export(
+        self,
+        file_id: str,
+        mime_type: GoogleMimeTypes,
+    ) -> bytes:
+        """Exports a Google Drive file to a different mime type. The exported content is limited to 10MB.
+
+        See https://developers.google.com/drive/api/reference/rest/v3/files/export for more information.
+
+        Args:
+            file_id (str): The ID of the file to export.
+            mime_type (GoogleMimeTypes): The mime type to export to.
+        """
+        file_id = parse_file_id(file_id)
+        return self.files.export(fileId=file_id, mimeType=mime_type.value).execute()
+
     def permissions_get(
         self, file_id: str, permission_id: str, **kwargs: Any
     ) -> Permission:
+        """Gets a permission by ID.
+
+        Args:
+            file_id (str): The ID of the file.
+            permission_id (str): The ID of the permission.
+        """
         file_id = parse_file_id(file_id)
         return (
             self.service.permissions()
             .get(fileId=file_id, permissionId=permission_id, **kwargs)
             .execute()
         )
 
     def permissions_list(
         self, file_id: str, fields: str = "*", **kwargs: Any
     ) -> Iterable[Permission]:
+        """Lists permissions for a file.
+
+        Args:
+            file_id (str): The ID of the file.
+            fields (str, optional): The fields to return. Defaults to "*".
+        """
         file_id = parse_file_id(file_id)
         list_func = (
             lambda x: self.service.permissions()
             .list(
                 fileId=file_id, pageToken=x, fields=self._list_fields(fields), **kwargs
             )
             .execute()
         )
         for response in self._list(list_func):
-            yield from response.get("permissions", [])
+            yield from response.get("permissions", [])  # type: ignore
 
     def _permission_update_if_exists(
         self, file_id: str, user_permission: Permission
     ) -> Permission | None:
         for p in self.permissions_list(file_id):
             if p["emailAddress"].strip().lower() == user_permission["emailAddress"]:
                 return p
@@ -566,13 +583,19 @@
                 sendNotificationEmail=sendNotificationEmail,
                 **kwargs,
             )
             .execute()
         )
 
     def permissions_delete(self, file_id: str, permission_id: str, **kwargs: Any):
+        """Deletes a permission from a file.
+
+        Args:
+            file_id (str): The ID of the file.
+            permission_id (str): The ID of the permission.
+        """
         file_id = parse_file_id(file_id)
         return (
             self.service.permissions()
             .delete(fileId=file_id, permissionId=permission_id, **kwargs)
             .execute()
         )
```

### Comparing `googleapiutils2-0.8.5/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.9.1/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.5/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.9.1/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.5/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.9.1/googleapiutils2/sheets/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.5/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.9.1/googleapiutils2/sheets/sheets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import logging
 import operator
 import time
 from collections import defaultdict
 from typing import *
 
 import pandas as pd
 from cachetools import TTLCache, cachedmethod
@@ -44,15 +43,14 @@
         Spreadsheet,
         SpreadsheetProperties,
         TextFormat,
         UpdateValuesResponse,
         ValueRange,
     )
 
-logger = logging.getLogger(__name__)
 
 SheetsRange = str | SheetSliceT | Any
 
 
 class Sheets:
     def __init__(self, creds: Credentials, throttle_time: float = THROTTLE_TIME):
         self.creds = creds
```

### Comparing `googleapiutils2-0.8.5/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.9.1/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.5/googleapiutils2/utils.py` & `googleapiutils2-0.9.1/googleapiutils2/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 from enum import Enum
 from functools import cache
 from pathlib import Path
 from typing import *
 
 import googleapiclient.http
 import requests
-
 from google.auth.transport.requests import Request
 from google.oauth2 import service_account
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 
 FilePath = str | Path
 
 if TYPE_CHECKING:
     from googleapiclient._apis.drive.v3.resources import File
-    from googleapiclient._apis.sheets.v4.resources import Spreadsheet, Color
+    from googleapiclient._apis.sheets.v4.resources import Color, Spreadsheet
 
 
 THROTTLE_TIME = 30
 
 SCOPES = [
     "https://www.googleapis.com/auth/spreadsheets",
     "https://www.googleapis.com/auth/drive.file",
@@ -111,22 +110,38 @@
     php = "application/x-httpd-php"
     json = "application/vnd.google-apps.script+json"
 
     default = "application/octet-stream"
 
 
 def hex_to_rgb(hex_code: str) -> Color:
-    """Converts a hex color code to RGB."""
+    """Converts a hex color code to RGB(A).
+
+    Args:
+        hex_code (str): Hex color code to convert. Can be 3, 4, 6, or 8 characters long (optional alpha is supported).
+    """
     hex_code = hex_code.lstrip("#")
-    return {
+
+    if len(hex_code) == 3 or len(hex_code) == 4:
+        hex_code = "".join([2 * c for c in hex_code])
+
+    rgb: Color = {
         "red": int(hex_code[:2], 16),
         "green": int(hex_code[2:4], 16),
-        "blue": int(hex_code[4:], 16),
+        "blue": int(hex_code[4:6], 16),
+        "alpha": 1.0,
     }
 
+    if len(hex_code) == 8:
+        rgb["alpha"] = round(int(hex_code[6:8], 16) / 255.0, 2)
+    elif len(hex_code) != 6:
+        raise ValueError("Invalid hex code")
+
+    return rgb
+
 
 def url_components(url: str) -> dict[str, List[str]]:
     return urllib.parse.parse_qs(urllib.parse.urlparse(url).query)
 
 
 def update_url_params(url: str, params: dict) -> str:
     url_obj = urllib.parse.urlparse(url)
@@ -154,17 +169,17 @@
 def get_oauth2_creds(
     client_config: FilePath | dict = CONFIG_PATH,
     token_path: FilePath = TOKEN_PATH,
     scopes: List[str] = SCOPES,
 ) -> Credentials:
     """Get OAuth2 credentials for Google API.
 
-    This will automatically detect if the credentials are for a service account.
-    If it's not, it will try to load the token from the token path (defaults to TOKEN_PATH)
-    and refresh it. The token will be saved to the token path.
+    If the client config provided is for a service account, we return the credentials.
+    Otherwise, we return the credentials from the token file if it exists, or we
+    authenticate the user and save the credentials to the token file.
 
     Args:
         client_config: Path to client config file or dict with client config.
         token_path: Path to token file.
         scopes: List of scopes. For more information on scopes, see:
             https://developers.google.com/identity/protocols/oauth2/scopes
     """
```

### Comparing `googleapiutils2-0.8.5/pyproject.toml` & `googleapiutils2-0.9.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.8.5"
+version = "0.9.1"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
@@ -15,31 +15,30 @@
 mypy = "^1.3.0"
 google-api-python-client-stubs = "^1.17.0"
 google-api-python-client = "^2.88.0"
 google-auth-oauthlib = "^1.0.0"
 requests = "^2.31.0"
 cachetools = "^5.3.1"
 google-auth-httplib2 = "^0.1.0"
-google-auth = "^2.19.0"
+google-auth = "^2.19.1"
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.31.0.1"
 types-cachetools = "^5.3.0.5"
 pytest = "^7.3.1"
-pandas-stubs = "^2.0.1.230501"
+pandas-stubs = "^2.0.2.230605"
 black = "^23.3.0"
 
 [tool.mypy]
 python_version = "3.10"
 warn_return_any = false
 warn_unused_configs = false
 disallow_untyped_defs = false
 check_untyped_defs = true
 
-
 [[tool.mypy.overrides]]
-module = "google.*"
+module = "google.*,google_auth_oauthlib.*"
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `googleapiutils2-0.8.5/PKG-INFO` & `googleapiutils2-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.8.5
+Version: 0.9.1
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: google-api-python-client (>=2.88.0,<3.0.0)
 Requires-Dist: google-api-python-client-stubs (>=1.17.0,<2.0.0)
-Requires-Dist: google-auth (>=2.19.0,<3.0.0)
+Requires-Dist: google-auth (>=2.19.1,<3.0.0)
 Requires-Dist: google-auth-httplib2 (>=0.1.0,<0.2.0)
 Requires-Dist: google-auth-oauthlib (>=1.0.0,<2.0.0)
 Requires-Dist: mypy (>=1.3.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/mkbabb/googleapiutils2
 Description-Content-Type: text/markdown
```

