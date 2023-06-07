# Comparing `tmp/jiggybase-0.0.36.tar.gz` & `tmp/jiggybase-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.36.tar", last modified: Sat Jun  3 22:17:29 2023, max compression
+gzip compressed data, was "jiggybase-0.1.0.tar", last modified: Wed Jun  7 00:12:23 2023, max compression
```

## Comparing `jiggybase-0.0.36.tar` & `jiggybase-0.1.0.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.885012 jiggybase-0.0.36/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.36/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-06-03 22:17:29.884597 jiggybase-0.0.36/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.0.36/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.875492 jiggybase-0.0.36/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.36/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.0.36/jiggybase/chat_stream.py
--rw-r--r--   0 wsk        (501) staff       (20)     4078 2023-05-25 02:03:37.000000 jiggybase-0.0.36/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)    11142 2023-05-25 02:00:12.000000 jiggybase-0.0.36/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.878914 jiggybase-0.0.36/jiggybase/examples/
--rw-r--r--   0 wsk        (501) staff       (20)     1378 2023-05-15 15:42:51.000000 jiggybase-0.0.36/jiggybase/examples/chat_completion.py
--rw-r--r--   0 wsk        (501) staff       (20)      295 2023-05-25 02:00:08.000000 jiggybase-0.0.36/jiggybase/examples/chat_completion_stream.py
--rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.36/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.36/jiggybase/examples/upload_email_example.py
--rw-r--r--   0 wsk        (501) staff       (20)      449 2023-05-21 02:08:21.000000 jiggybase-0.0.36/jiggybase/ipython.py
--rwxr-xr-x   0 wsk        (501) staff       (20)      648 2023-05-21 02:24:20.000000 jiggybase-0.0.36/jiggybase/jiggybase_ipython.py
--rw-r--r--   0 wsk        (501) staff       (20)     5681 2023-05-28 04:35:07.000000 jiggybase-0.0.36/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.36/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.883082 jiggybase-0.0.36/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.36/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.36/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     2955 2023-05-25 00:41:27.000000 jiggybase-0.0.36/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.0.36/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.36/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.36/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.36/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.36/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2845 2023-06-03 22:11:35.000000 jiggybase-0.0.36/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     3206 2023-05-20 00:39:05.000000 jiggybase-0.0.36/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.36/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.36/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.36/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.36/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.36/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.877458 jiggybase-0.0.36/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     1050 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       78 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      752 2023-06-03 22:11:12.000000 jiggybase-0.0.36/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-06-03 22:17:29.885131 jiggybase-0.0.36/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.884029 jiggybase-0.0.36/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.36/test/test.py
--rw-r--r--   0 wsk        (501) staff       (20)    12115 2023-05-25 01:50:31.000000 jiggybase-0.0.36/test/test_extract_typed_completion.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.197262 jiggybase-0.1.0/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.1.0/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     6812 2023-06-07 00:12:23.196848 jiggybase-0.1.0/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.1.0/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.180688 jiggybase-0.1.0/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.1.0/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.1.0/jiggybase/chat_stream.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4356 2023-06-04 23:55:57.000000 jiggybase-0.1.0/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     9397 2023-06-05 00:10:11.000000 jiggybase-0.1.0/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.184847 jiggybase-0.1.0/jiggybase/examples/
+-rw-r--r--   0 wsk        (501) staff       (20)     1378 2023-05-15 15:42:51.000000 jiggybase-0.1.0/jiggybase/examples/chat_completion.py
+-rw-r--r--   0 wsk        (501) staff       (20)      295 2023-05-25 02:00:08.000000 jiggybase-0.1.0/jiggybase/examples/chat_completion_stream.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.1.0/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.1.0/jiggybase/examples/upload_email_example.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)      648 2023-05-21 02:24:20.000000 jiggybase-0.1.0/jiggybase/ijiggy.py
+-rw-r--r--   0 wsk        (501) staff       (20)     5681 2023-05-28 04:35:07.000000 jiggybase-0.1.0/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.1.0/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.194126 jiggybase-0.1.0/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.1.0/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.1.0/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2955 2023-05-25 00:41:27.000000 jiggybase-0.1.0/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.1.0/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.1.0/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1833 2023-06-04 00:49:56.000000 jiggybase-0.1.0/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.1.0/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.1.0/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2845 2023-06-03 23:09:48.000000 jiggybase-0.1.0/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4707 2023-06-03 23:40:06.000000 jiggybase-0.1.0/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3411 2023-06-03 23:48:09.000000 jiggybase-0.1.0/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.1.0/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.1.0/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.1.0/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4799 2023-06-05 00:03:48.000000 jiggybase-0.1.0/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.182710 jiggybase-0.1.0/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     6812 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     1018 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      109 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-06-07 00:12:23.000000 jiggybase-0.1.0/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      794 2023-06-04 23:57:56.000000 jiggybase-0.1.0/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-06-07 00:12:23.197393 jiggybase-0.1.0/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-07 00:12:23.195960 jiggybase-0.1.0/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.1.0/test/test.py
+-rw-r--r--   0 wsk        (501) staff       (20)    12115 2023-05-25 01:50:31.000000 jiggybase-0.1.0/test/test_extract_typed_completion.py
```

### Comparing `jiggybase-0.0.36/LICENSE` & `jiggybase-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/PKG-INFO` & `jiggybase-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.36
+Version: 0.1.0
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.36/README.md` & `jiggybase-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/chat_stream.py` & `jiggybase-0.1.0/jiggybase/chat_stream.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/client.py` & `jiggybase-0.1.0/jiggybase/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,24 +55,31 @@
         return all Collections in all Orgs that the user is a member of
         """
         resp = self.session.get("/collections")
         return [Collection(self.session, **c) for c in resp.json()]
    
     def collection_names(self) -> List[Collection]:
         """
-        return the unique collection name for all collections in all Orgs that the user is a member of
+        return the collection display names for all collections in all Orgs that the user is a member of
         """
-        return [c.name for c in self.collections()]
+        return [c.disply_name for c in self.collections()]
+
+    def collection_hostnames(self) -> List[Collection]:
+        """
+        return the unique collection hostname for all collections in all Orgs that the user is a member of
+        """
+        return [c.hostname for c in self.collections()]
+
             
     def collection(self, name : str) -> Collection:        
         """
-        return a collection of the specified name
+        return a collection of the specified display name or hostname
         """
         for collection in self.collections():
-            if collection.name == name or collection.display_name.lower() == name.lower():
+            if collection.hostname == name or collection.display_name.lower() == name.lower():
                 return collection
         raise ValueError(f'Collection "{name}" not found')
 
 
     def _extract_typed_completion(self,
                                  messages       : List[Message],
                                  pydantic_model : BaseModel,
```

### Comparing `jiggybase-0.0.36/jiggybase/collection.py` & `jiggybase-0.1.0/jiggybase/collection.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,56 +4,18 @@
 from enum import Enum
 from .models import collection, CollectionChatConfig, PatchCollectionChatConfig
 from .jiggybase_session import JiggyBaseSession
 from .models import UpsertResponse,  Query, QueryRequest, QueryResponse, UpsertRequest, Document, DocumentChunk, DeleteRequest, DeleteResponse, DocumentMetadataFilter, DocChunksResponse
 from .models import Message, CompletionRequest, ChatCompletion, ChatUsage
 from .chat_stream import extract_content_from_sse_bytes
 from .models import ExtractMetadataConfig
-
+from .models import CollectionPatchRequest, PluginAuthConfigOAuth, PatchPluginOAuthConfigRequest
 
 from typing import Union, List
-class PluginAuthType(Enum):
-    bearer :str = "bearer"
-    none   :str = "none"
-    oauth  :str = "oauth"
-
-        
-class CollectionPostRequest(BaseModel):
-    """
-    Used to create a new Collection service
-    """
-    name:         str                      = Field(description="The globally unique hostname for the collection. Subject to DNS naming rules. ")
-    display_name: Optional[str]            = Field(description="The human friendly display name for the collection.")
-    description:  Optional[str]            = Field(description="A description of the collection.")
-    plugin_auth:  Optional[PluginAuthType] = Field(default=PluginAuthType.bearer, description="The authentication type to use for this collection's ChatGPT plugin.")
-
-
-class CollectionPatchRequest(BaseModel):
-    """
-    Used to modify an existing service
-    """
-    description:  Optional[str] = Field(description="A description of the collection.")
-    plugin_auth:  Optional[str] = Field(description='The auth plugin to use for this org.')
-    display_name: Optional[str] = Field(description="The human friendly display name for the collection.")
-
-
-
-class PluginAuthConfigOAuth(BaseModel):
-    """
-    The Plugin Oauth configuration as managed by GPT-Gateway
-    """    
-    client_url:                 HttpUrl     = Field(description="ChatGPT will direct the user’s browser to this url to log in to the plugin")
-    authorization_url:          HttpUrl     = Field(description="After successful login ChatGPT will complete the OAuth flow by making a POST request to this URL")
-    scope:                      str         = Field(description="The scope used for the OAuth flow")
-    client_id:                  str         = Field(unique=True, index=True, description="The client id to send to OpenAI for the plugin")
-    client_secret:              str         = Field(description="The client secret to send to OpenAI for the plugin")
-    openai_verification_token:  str         = Field(description="The verification token specified by OpenAI to configure in the plugin")
 
-class PatchPluginOAuthConfigRequest(BaseModel):
-    openai_verification_token: str  
 
         
 class Collection(collection.Collection):
     """
     derived from models.collection.Collection data model for purposes of adding management methods
     """
     class Config(BaseConfig):
@@ -67,15 +29,16 @@
         
     def set_description(self, description:str) -> "Collection":
         """
         Update an existing collection using its ID and the provided description.
         """
         patch_request = CollectionPatchRequest(description=description)
         rsp = self.session.patch(f"/orgs/{self.org_id}/collections/{self.id}", model=patch_request)
-        return Collection(**rsp.json())
+        self.description = rsp.json()['description']
+
 
     def set_oauth_verification_token(self, openai_verification_token: str) -> PluginAuthConfigOAuth:
         """
         Set the OpenAI verification token for this collection's plugin.
         This is the token that OpenAI provides during while registering a plugin configured to use Oauth.
         """
         patch_request = PatchPluginOAuthConfigRequest(openai_verification_token=openai_verification_token)
@@ -227,8 +190,15 @@
         return ExtractMetadataConfig(**rsp.json())
 
     def patch_extract_metadata_config(self, config: ExtractMetadataConfig):
         """
         Get the metadata configuration for this collection.
         """
         rsp = self.session.patch(f"/orgs/{self.org_id}/collections/{self.id}/extract_metadata_config", model=config)
-        return ExtractMetadataConfig(**rsp.json())    
+        return ExtractMetadataConfig(**rsp.json())    
+
+    def __str__(self) -> str:
+        return f"Collection(id={self.id:4}, name={self.display_name:30}, hostname={self.hostname:30}, org_id={self.org_id:4},\n" \
+               f"           description='{self.description}')"
+
+    def __repr__(self) -> str:
+        return str(self)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jiggybase-0.0.36/jiggybase/examples/chat_completion.py` & `jiggybase-0.1.0/jiggybase/examples/chat_completion.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.1.0/jiggybase/examples/jiggybase_upload.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/examples/upload_email_example.py` & `jiggybase-0.1.0/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/jiggybase_ipython.py` & `jiggybase-0.1.0/jiggybase/ijiggy.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/jiggybase_session.py` & `jiggybase-0.1.0/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/login.py` & `jiggybase-0.1.0/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/models/auth.py` & `jiggybase-0.1.0/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/models/chat.py` & `jiggybase-0.1.0/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/models/chunk.py` & `jiggybase-0.1.0/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/models/metadata.py` & `jiggybase-0.1.0/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/models/org.py` & `jiggybase-0.1.0/jiggybase/models/org.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,13 +37,13 @@
 
 class Org(BaseModel):
     id:                  int           = Field(escription="Internal org id")
     name:                str           = Field(max_length=39, description='Unique name for this org.')
     description:         Optional[str] = Field(max_length=255, description='Optional user supplied description.')
     created_at:          float         = Field(description='The epoch timestamp when the org was created.')
     updated_at:          float         = Field(description='The epoch timestamp when the org was updated.')
-    created_by:          int           = Field(description='The user_id of the user that created the org.')
+    created_by:          Optional[int] = Field(description='The user_id of the user that created the org.')
     subscription_id:     str           = Field(description='The subscription_id for the org.')    
     gpt4_credits:        int           = Field(description='The number of GPT-4 message credits currently available to the org users for chat.jiggy.ai.')
     gpt3_5_credits:      int           = Field(description='The number of GPT-3 message credits currently available to the org users for chat.jiggy.ai.')
-    subscription_status: Optional[str] = Field(description='The stripe subscription status.')
+    subscription_status: str           = Field(description='The stripe subscription status.')
```

### Comparing `jiggybase-0.0.36/jiggybase/models/plugin_config.py` & `jiggybase-0.1.0/jiggybase/models/plugin_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from pydantic import BaseModel, HttpUrl, Field, validator
 from typing import List, Optional
 from enum import Enum
-from .collection import PluginAuthType        
+from .plugin import PluginAuthType        
 import re
 
 MODELNAME = re.compile("[a-zA-Z][a-zA-Z0-9_]*")
 
 class PluginConfig(BaseModel): 
     """
     The user-customizable part of PluginConfig
```

### Comparing `jiggybase-0.0.36/jiggybase/models/prompt.py` & `jiggybase-0.1.0/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/models/providers.py` & `jiggybase-0.1.0/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/models/user.py` & `jiggybase-0.1.0/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/jiggybase/org.py` & `jiggybase-0.1.0/jiggybase/org.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 
-from typing import Optional, List
+from typing import Any, Optional, List
 from pydantic import BaseConfig, EmailStr
 import enum
 
-from .collection import Collection, CollectionPostRequest
+from .models import  CollectionPostRequest
 
 from .models.org import Org as OrgModel
 from .models.org import OrgRole, OrgMember, OrgPatchRequest
 from .models import PromptTask, PromptMessage, PromptTaskPostRequest, PromptTaskType
 
+from .collection import Collection
     
 ###
 ## Org
 ###
 class Org(OrgModel):
 
     class Config(BaseConfig):
         extra = "allow"
 
     def __init__(self, session, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.session = session
         
     def create_collection(self, 
-                          name: str, 
                           display_name: str,
-                          plugin_auth: Optional[str] = "bearer",
                           description: Optional[str] = None) -> Collection:
         rsp = self.session.post(f"/orgs/{self.id}/collections", model=CollectionPostRequest(**locals()))
+        print(rsp.json())
         return Collection(self.session, **rsp.json())
 
     def collections(self) -> list[Collection]:
         rsp = self.session.get(f"/orgs/{self.id}/collections")
         return [Collection(self.session, **c) for c in rsp.json()]
 
     def collection(self, name: str) -> Collection:
@@ -103,8 +103,14 @@
                                 prompts     = prompts)
         
     def get_prompt_task(self, prompt_task_id: int) -> PromptTask:
         
         return PromptTask(**self.session.get(f"/orgs/{self.id}/prompt_tasks/{prompt_task_id}").json())
 
     def delete_prompt_task(self, prompt_task_id: int):
-        self.session.delete(f"/orgs/{self.id}/prompt_tasks/{prompt_task_id}")
+        self.session.delete(f"/orgs/{self.id}/prompt_tasks/{prompt_task_id}")
+
+    def __str__(self) -> str:
+        return f"Org(id={self.id:4}, status={self.subscription_status:8}, gpt4_credts={self.gpt4_credits:4}, name={self.name:20}, description={self.description})"
+
+    def __repr__(self) -> str:
+        return str(self)
```

### Comparing `jiggybase-0.0.36/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.1.0/jiggybase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.36
+Version: 0.1.0
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.36/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.1.0/jiggybase.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 jiggybase/__init__.py
 jiggybase/chat_stream.py
 jiggybase/client.py
 jiggybase/collection.py
-jiggybase/ipython.py
-jiggybase/jiggybase_ipython.py
+jiggybase/ijiggy.py
 jiggybase/jiggybase_session.py
 jiggybase/login.py
 jiggybase/org.py
 jiggybase.egg-info/PKG-INFO
 jiggybase.egg-info/SOURCES.txt
 jiggybase.egg-info/dependency_links.txt
 jiggybase.egg-info/entry_points.txt
```

### Comparing `jiggybase-0.0.36/pyproject.toml` & `jiggybase-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.36"
+version = "0.1.0"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
@@ -22,7 +22,8 @@
 [project.urls]
 "Homepage"    = "https://github.com/jiggy-ai/jiggybase"
 "Bug Tracker" = "https://github.com/jiggy-ai/issues"
 
 
 [project.scripts]
 jiggybase_upload = "jiggybase.examples.jiggybase_upload:main"
+ijiggy           = "jiggybase.ijiggy:main"
```

### Comparing `jiggybase-0.0.36/test/test.py` & `jiggybase-0.1.0/test/test.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.36/test/test_extract_typed_completion.py` & `jiggybase-0.1.0/test/test_extract_typed_completion.py`

 * *Files identical despite different names*

