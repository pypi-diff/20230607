# Comparing `tmp/xt_st_common-0.6.0.tar.gz` & `tmp/xt_st_common-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.6.0.tar", max compression
+gzip compressed data, was "xt_st_common-0.6.1.tar", max compression
```

## Comparing `xt_st_common-0.6.0.tar` & `xt_st_common-0.6.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      720 2023-06-07 01:40:04.921259 xt_st_common-0.6.0/README.md
--rw-r--r--   0        0        0     2603 2023-06-07 01:40:04.921259 xt_st_common-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6128 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/__init__.py
--rw-r--r--   0        0        0      180 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/.env
--rw-r--r--   0        0        0       67 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/.prettierrc
--rw-r--r--   0        0        0      859 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2052 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/index.html
--rw-r--r--   0        0        0      564 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
--rw-r--r--   0        0        0     1183 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/service-worker.js
--rw-r--r--   0        0        0  4138182 2023-06-07 01:39:18.369642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
--rw-r--r--   0        0        0     3326 2023-06-07 01:39:18.369642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 16152785 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
--rw-r--r--   0        0        0     1442 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
--rw-r--r--   0        0        0     3848 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
--rw-r--r--   0        0        0     1598 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0        0        0     8317 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0        0        0     1141 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/package.json
--rw-r--r--   0        0        0      839 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/public/index.html
--rw-r--r--   0        0        0     1922 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
--rw-r--r--   0        0        0      274 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/tsconfig.json
--rw-r--r--   0        0        0       22 2023-06-07 01:40:04.921259 xt_st_common-0.6.0/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/components.py
--rw-r--r--   0        0        0     2371 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/config.py
--rw-r--r--   0        0        0     3177 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/database.py
--rw-r--r--   0        0        0     6303 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0    25276 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/project_components.py
--rw-r--r--   0        0        0     6518 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/project_models.py
--rw-r--r--   0        0        0     5976 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/session.py
--rw-r--r--   0        0        0     6251 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1957 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-06-07 01:57:03.161414 xt_st_common-0.6.1/README.md
+-rw-r--r--   0        0        0     2603 2023-06-07 01:57:03.161414 xt_st_common-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6128 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2023-06-07 01:56:21.524751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2023-06-07 01:56:21.524751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2023-06-07 01:57:03.161414 xt_st_common-0.6.1/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     2371 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3177 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6303 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    25276 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0     6518 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5976 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     6380 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1957 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.6.1/PKG-INFO
```

### Comparing `xt_st_common-0.6.0/README.md` & `xt_st_common-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.6.0
+# XT-STREAMLIT - 0.6.1
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

### Comparing `xt_st_common-0.6.0/pyproject.toml` & `xt_st_common-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.6.0"
+version = "0.6.1"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}, {include = "streamlit_plotly_events", from= "src"}]
 
 [tool.poe.tasks]
 test = { cmd="pytest --cov=src/xt_st_common", help="Run unit tests"}
```

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/__init__.py` & `xt_st_common-0.6.1/src/streamlit_plotly_events/__init__.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/asset-manifest.json` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/index.html` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/service-worker.js` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/package.json` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/package.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/public/index.html` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx` & `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/xt_st_common/components.py` & `xt_st_common-0.6.1/src/xt_st_common/components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/xt_st_common/config.py` & `xt_st_common-0.6.1/src/xt_st_common/config.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/xt_st_common/database.py` & `xt_st_common-0.6.1/src/xt_st_common/database.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.6.1/src/xt_st_common/fs_upload_page.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/xt_st_common/project_components.py` & `xt_st_common-0.6.1/src/xt_st_common/project_components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/xt_st_common/project_models.py` & `xt_st_common-0.6.1/src/xt_st_common/project_models.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/xt_st_common/session.py` & `xt_st_common-0.6.1/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/src/xt_st_common/storage.py` & `xt_st_common-0.6.1/src/xt_st_common/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,21 @@
 
     @abstractmethod
     def file_exists(self, file_path: str):
         pass
 
 
 class MinioStorageClient(StorageClient):
-    def __init__(self, bucket: str, endpoint="s3.amazonaws.com", credentials: Provider = IamAwsProvider(), secure=True):
+    def __init__(
+        self,
+        bucket: str,
+        endpoint="s3.amazonaws.com",
+        credentials: Provider = IamAwsProvider(),
+        secure=True,
+    ):
         if not bucket:
             raise ValueError("bucket name must be set")
 
         self.__bucket = bucket
         # Check environment variables have been set
         if isinstance(credentials, IamAwsProvider):
             for var in ["AWS_WEB_IDENTITY_TOKEN_FILE", "AWS_REGION", "AWS_ROLE_ARN"]:
@@ -82,15 +88,20 @@
         if not exists:
             __client.make_bucket(bucket)
             logging.info(f"Minio Bucket created: {bucket}")
 
         self.__client = __client
 
     @classmethod
-    def object_to_file(cls, obj: ObjectWriteResult, file_length: int = 0, content_type: str = "text/plain") -> FileRef:
+    def object_to_file(
+        cls,
+        obj: ObjectWriteResult,
+        file_length: int = 0,
+        content_type: str = "text/plain",
+    ) -> FileRef:
         path = obj.object_name
         path_segments = path.split("/")
         name = path_segments[-1]
 
         return FileRef(
             url=obj.bucket_name + obj.object_name,
             size=sizeof_fmt(file_length),
@@ -125,14 +136,15 @@
 
     def get_file(self, file_path: str):
         response_data = None
         try:
             response = self.__client.get_object(self.__bucket, file_path)
             # Read data from response.
             response_data = BytesIO(response.read())
+            response_data.name = file_path
         finally:
             response.close()
             response.release_conn()
 
         return response_data
 
     def delete_file(self, file_path: str):
```

### Comparing `xt_st_common-0.6.0/src/xt_st_common/utils.py` & `xt_st_common-0.6.1/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.0/PKG-INFO` & `xt_st_common-0.6.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.6.0
+Version: 0.6.1
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >3.9.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,15 +19,15 @@
 Requires-Dist: pymongo (>=4.3.3) ; extra == "databases"
 Requires-Dist: pymongo-auth-aws (>=1.1.0) ; extra == "databases"
 Requires-Dist: streamlit (>=1.22.0)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.6.0
+# XT-STREAMLIT - 0.6.1
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

