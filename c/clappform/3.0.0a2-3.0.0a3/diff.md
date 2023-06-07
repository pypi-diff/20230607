# Comparing `tmp/clappform-3.0.0a2.tar.gz` & `tmp/clappform-3.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clappform-3.0.0a2.tar", last modified: Tue Jun  6 12:26:01 2023, max compression
+gzip compressed data, was "clappform-3.0.0a3.tar", last modified: Wed Jun  7 13:45:35 2023, max compression
```

## Comparing `clappform-3.0.0a2.tar` & `clappform-3.0.0a3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:26:01.975703 clappform-3.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-06 12:25:46.000000 clappform-3.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-06 12:26:01.975703 clappform-3.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 12:25:46.000000 clappform-3.0.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-06 12:25:46.000000 clappform-3.0.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:26:01.975703 clappform-3.0.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:26:01.975703 clappform-3.0.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:26:01.975703 clappform-3.0.0a2/src/clappform/
--rw-r--r--   0 runner    (1001) docker     (123)    22106 2023-06-06 12:25:46.000000 clappform-3.0.0a2/src/clappform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-06-06 12:25:46.000000 clappform-3.0.0a2/src/clappform/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-06 12:25:46.000000 clappform-3.0.0a2/src/clappform/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:26:01.975703 clappform-3.0.0a2/src/clappform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-06 12:26:01.000000 clappform-3.0.0a2/src/clappform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-06 12:26:01.000000 clappform-3.0.0a2/src/clappform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:26:01.000000 clappform-3.0.0a2/src/clappform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 12:26:01.000000 clappform-3.0.0a2/src/clappform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 12:26:01.000000 clappform-3.0.0a2/src/clappform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-06 12:25:46.000000 clappform-3.0.0a2/src/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:45:35.886432 clappform-3.0.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 13:45:21.000000 clappform-3.0.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-07 13:45:35.886432 clappform-3.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 13:45:21.000000 clappform-3.0.0a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-07 13:45:21.000000 clappform-3.0.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:45:35.886432 clappform-3.0.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:45:35.886432 clappform-3.0.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:45:35.886432 clappform-3.0.0a3/src/clappform/
+-rw-r--r--   0 runner    (1001) docker     (123)    24500 2023-06-07 13:45:21.000000 clappform-3.0.0a3/src/clappform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-06-07 13:45:21.000000 clappform-3.0.0a3/src/clappform/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-07 13:45:21.000000 clappform-3.0.0a3/src/clappform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:45:35.886432 clappform-3.0.0a3/src/clappform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-07 13:45:35.000000 clappform-3.0.0a3/src/clappform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-07 13:45:35.000000 clappform-3.0.0a3/src/clappform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:45:35.000000 clappform-3.0.0a3/src/clappform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 13:45:35.000000 clappform-3.0.0a3/src/clappform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 13:45:35.000000 clappform-3.0.0a3/src/clappform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 13:45:21.000000 clappform-3.0.0a3/src/debug.py
```

### Comparing `clappform-3.0.0a2/LICENSE` & `clappform-3.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a2/PKG-INFO` & `clappform-3.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clappform-3.0.0a2/README.md` & `clappform-3.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a2/pyproject.toml` & `clappform-3.0.0a3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clappform"
-version = "3.0.0-alpha.2"
+version = "3.0.0-alpha.3"
 authors= [
     { name="Clappform B.V.", email="info@clappform.com" },
 ]
 description = "Clappform Python API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -50,16 +50,10 @@
                      # the root of the project
 )
 '''
 
 [tool.pylint]
 max-line-length = 88
 disable = [
-    "C0301", # (line-too-long)
-    "C0116", # (missing-function-docstring)
     "C0103", # (invalid-name)
     "R0902", # (too-many-instance-attributes)
-    "R0913", # (too-many-arguments)
-    "R0904", # (too-many-public-methods)
-    "R0903", # (too-few-public-methods)
-    "C0302", # (too-many-lines)
 ]
```

### Comparing `clappform-3.0.0a2/src/clappform/__init__.py` & `clappform-3.0.0a3/src/clappform/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     HTTPError,
     PaginationTotalError,
     PaginationKeyError,
 )
 
 
 # Metadata
-__version__ = "3.0.0-alpha.2"
+__version__ = "3.0.0-alpha.3"
 __author__ = "Clappform B.V."
 __email__ = "info@clappform.com"
 __license__ = "MIT"
 __doc__ = "Clappform Python API wrapper"
 
 
 class Clappform:
@@ -220,15 +220,42 @@
         if isinstance(document["data"], dict):
             return type(resource)(**document["data"])
         raise TypeError(
             "'data' key-value is not {list} or {dict}, got {type(document['data'])}"
         )
 
     def create(self, resource, item=None):
-        # Custom behavior when arguments are specific types.
+        """Crete a resource.
+
+        :param resource: Any object of :class:`clappform.dataclasses.ResourceType`
+        :param item: Optional only useful when resource argument is of type
+            :class:`clappform.dataclasses.Collection`.
+        :type item: dict
+
+        Usage::
+
+            >>> from clappform import Clappform
+            >>> import clappform.dataclasses as r
+            >>> c = Clappform(
+            ...     "https://app.clappform.com",
+            ...     "j.doe@clappform.com",
+            ...     "S3cr3tP4ssw0rd!"
+            ... )
+            >>> new_app = r.App(
+            ...     id="uspresidents",
+            ...     name="US Presidents",
+            ...     description="US Presidents Dashboard",
+            ...     settings={}
+            ... )
+            >>> c.create(new_app)
+            App(collections=0, default_page='', description='US Presidents Dashboard...
+
+        :returns: Newly created resource
+        """
+        # Custom behavior when arguments are of a specific type.
         if isinstance(resource, dc.Collection) and isinstance(item, dict):
             document = self._private_request(
                 "POST", resource.create_item_path(), json={"data": item}
             )
             return document["data"]
         if isinstance(resource, dc.Questionnaire):
             document = self._private_request(
@@ -239,14 +266,37 @@
             return dc.Questionnaire(**document["data"])
 
         payload = self._remove_nones(asdict(resource))
         document = self._private_request("POST", resource.create_path(), json=payload)
         return type(resource)(**document["data"])
 
     def update(self, resource, item=None):
+        """Update a resource.
+
+        :param resource: Any object of :class:`clappform.dataclasses.ResourceType`
+        :param item: Optional only useful when resource argument is of type
+            :class:`clappform.dataclasses.Collection`.
+        :type item: dict
+
+        Usage::
+
+            >>> from clappform import Clappform
+            >>> import clappform.dataclasses as r
+            >>> c = Clappform(
+            ...     "https://app.clappform.com",
+            ...     "j.doe@clappform.com",
+            ...     "S3cr3tP4ssw0rd!"
+            ... )
+            >>> app = c.get(r.App(id="uspresidents"))
+            >>> app.description = "Dashboard of US Presidents"
+            >>> c.update(app)
+            App(collections=0, default_page='', description='Dashboard of US Preside...
+
+        :returns: Updated resource
+        """
         # Custom behavior when arguments are specific types.
         if isinstance(resource, dc.Collection) and isinstance(item, dict):
             item_id, item = self._seperate_id_from_item(item)
             document = self._private_request(
                 "PUT", resource.one_item_path(item_id), json={"data": item}
             )
             document["data"]["_id"] = item_id  # Adding item's id back into response.
@@ -263,14 +313,32 @@
         if isinstance(resource, dc.User):
             del payload["email"]
 
         document = self._private_request("PUT", resource.one_path(), json=payload)
         return type(resource)(**document["data"])
 
     def delete(self, resource, item=None):
+        """Delete a resource.
+
+        Usage::
+
+            >>> from clappform import Clappform
+            >>> import clappform.dataclasses as r
+            >>> c = Clappform(
+            ...     "https://app.clappform.com",
+            ...     "j.doe@clappform.com",
+            ...     "S3cr3tP4ssw0rd!",
+            ... )
+            >>> app = c.get(r.App(id="uspresidents"))
+            >>> c.delete(app)
+            ApiResponse(code=200, message='Successfully deleted app with ID: uspresi...
+
+        :returns: Confirmation of deletion.
+        :rtype: :class:`clappform.dataclasses.ApiResponse`
+        """
         # Custom behavior when arguments are specific types.
         if isinstance(resource, dc.Collection) and item is not None:
             oids: list[str] = None
             if isinstance(item, list):
                 # `0` element of `_seperate_id_from_item` is an item's id.
                 oids = [self._seperate_id_from_item(x)[0] for x in item]
             if isinstance(item, dict):
@@ -417,42 +485,41 @@
                 )  # Prevent Denial Of Service (dos) flagging.
                 document = self._private_request(**params)
 
     def write_dataframe(
         self,
         df: DataFrame,
         collection: dc.Collection,
-        chunk_size: int = 100,
+        size: int = 100,
         interval_timeout: int = 0,
     ):
         """Write Pandas DataFrame to collection.
 
         :param df: Pandas DataFrame to write to collection
         :type df: :class:`pandas.DataFrame`
         :param collection: Collection to hold DataFrame records
         :type collection: :class:`clappform.dataclasses.Collection`
-        :param int chunk_size: defaults to: ``100``
+        :param int size: Size of each chunk. Defaults to: ``100``
         :param interval_timeout: Optional time to sleep per request, defaults to:
             ``0.0``.
         :type interval_timeout: int
         """
         # Transform DataFrame to be JSON serializable
         for col in df.columns:
             if df[col].dtype == "datetime64[ns, UTC]":
                 df[col] = df[col].astype("datetime64[s, UTC]").astype("int")
             df[col] = df[col].replace([np.nan, np.inf, -np.inf], None)
         df = df.replace([np.nan, np.inf, -np.inf], None)
 
         # Split DataFrame up into chunks.
-        list_df = [df[i : i + chunk_size] for i in range(0, df.shape[0], chunk_size)]
-        for i in range(len(list_df)):
+        for chunk in [df[i : i + size] for i in range(0, df.shape[0], size)]:
             # `TemporaryFile` And `force_ascii=False` force the chunck to be `UTF-8`
             # encoded.
             with tempfile.TemporaryFile(mode="w+", encoding="utf-8") as fd:
-                df.to_json(fd, orient="records", force_ascii=False)
+                chunk.to_json(fd, orient="records", force_ascii=False)
                 fd.seek(0)  # Reset pointer to begin of file for reading.
                 self._private_request(
                     "POST", collection.dataframe_path(), data=fd.read()
                 )
             time.sleep(interval_timeout)
 
     def empty_dataframe(self, collection) -> dc.ApiResponse:
```

### Comparing `clappform-3.0.0a2/src/clappform/dataclasses.py` & `clappform-3.0.0a3/src/clappform/dataclasses.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,18 +181,18 @@
         >>> new_app = r.App(
         ...     id="uspresidents",
         ...     name="US Presidents",
         ...     description="US Presidents Dashboard",
         ...     settings={}
         ... )
         >>> c.create(new_app)
-        App(collections=0, default_page='', description='US Presidents Dashboard', groups=0, id='uspresidents', name='US Presidents', settings={})
+        App(collections=0, default_page='', description='US Presidents Dashboard', g...
         >>> app = c.get(r.App(id="uspresidents"))
         >>> c.delete(app)
-        ApiResponse(code=200, message='Successfully deleted app with ID: uspresidents.', response_id='647de8f97416cc352603a431')
+        ApiResponse(code=200, message='Successfully deleted app with ID: uspresident...
         >>> for app in c.get(r.App()):
         ...     print(app.name)
     """
 
     #: Number of collections this app has. If ``extended=True`` this will be a list
     #: of collections.
     collections: int = None
@@ -300,18 +300,18 @@
         ...     app=app,
         ...     database="MONGO",
         ...     name="United States Presidents",
         ...     slug="presidents",
         ...     description="All presidents of the United Stated of America"
         ... )
         >>> c.create(new_collection)
-        Collection(app='uspresidents', slug='presidents', database='MONGO', name='United States Presidents', items=None, description='All presidents of the United Stated of America', is_encrypted=False, is_locked=False, is_logged=False, queries=None, sources=[], id=473)
+        Collection(app='uspresidents', slug='presidents', database='MONGO', name='Un...
         >>> collection = c.get(r.Collection(app="uspresidents", slug="presidents"))
         >>> c.delete(collection)
-        ApiResponse(code=200, message='Successfully deleted collection with slug: presidents.', response_id='647df8477416cc352603a447')
+        ApiResponse(code=200, message='Successfully deleted collection with slug: pr...
         >>> for collection in c.get(r.Collection()):
         ...     print(f"{collection.app}: {collection.slug}")
     """
 
     #: App id this collection belong to. This can be of type
     #: :class:`clappform.dataclasses.App` or :class:`str`.
     app: str = None
@@ -427,32 +427,37 @@
         if self.app is None:
             raise TypeError("app attribute can not be None")
         return f"/collection/{self.app}"
 
     def one_item_path(self, item: str) -> str:
         """Return the route used for creating and deleting items.
 
-        :returns: Item HTTP resource path
+        :returns: Item HTTP path
         :rtype: str
         """
         if self.app is None or self.slug is None:
             raise TypeError("both 'app' and 'slug' attributes can not be {None}")
         if not isinstance(item, str):
             raise TypeError(f"item arg is not of type {str}, got {type(item)}")
         return f"/item/{self.app}/{self.slug}/{item}"
 
     def create_item_path(self) -> str:
+        """Return the route used to create an item.
+
+        :returns: Item HTTP path
+        :rtype: str
+        """
         if self.app is None or self.slug is None:
             raise TypeError(f"both 'app' and 'slug' attributes can not be {None}")
         return f"/item/{self.app}/{self.slug}"
 
     def dataframe_path(self) -> str:
         """Return the route used to retreive the Dataframe.
 
-        :returns: Collection's Dataframe HTTP resource path
+        :returns: Collection's Dataframe HTTP path
         :rtype: str
         """
         if self.app is None or self.slug is None:
             raise TypeError(f"'app' and 'slug' attributes can not be {None}")
         return f"/dataframe/{self.app}/{self.slug}"
 
 
@@ -474,53 +479,68 @@
         ...     collection=collection,
         ...     data_source="app",
         ...     query=[],
         ...     name="all presidents",
         ...     slug="f1cb2ba5-64a7-4056-99d5-7d639557970f",
         ... )
         >>> c.create(new_collection)
-        Query(app='uspresidets', collection='presidents', data_source='app', export=False, id=3601, name='all presidents', query=[], slug='f1cb2ba5-64a7-4056-99d5-7d639557970f', source_query='', modules=[], primary=True, settings={})
+        Query(app='uspresidets', collection='presidents', data_source='app', export=...
         >>> query = c.get(r.Query(slug="f1cb2ba5-64a7-4056-99d5-7d639557970f"))
         >>> c.delete(query)
-        ApiResponse(code=200, message='Successfully deleted query with slug: f1cb2ba5-64a7-4056-99d5-7d639557970f.', response_id='')
+        ApiResponse(code=200, message='Successfully deleted query with slug: f1cb2ba...
         >>> for query in c.get(r.Query()):
         ...     print(f"{query.app}/{query.collection}: {query.slug}")
     """
 
+    #: App id this query belong to. This can be of type
+    #: :class:`clappform.dataclasses.App` or :class:`str`.
     app: str = None
     _app: str = field(init=False, repr=False, default=None)
+    #: Collection slug this query refers to. This can be of type
+    #: :class:`clappform.dataclasses.Collection` or :class:`str`.
     collection: str = None
     _collection: str = field(init=False, repr=False, default=None)
     data_source: str = None
     export: bool = None
+    #: Numeric id used for internal identication
     id: int = None
     name: str = None
     query: list = None
     slug: str = None
     source_query: str = None
     modules: list = None
     primary: bool = None
     settings: dict = None
 
     @property
     def app(self) -> str:
+        """Return the app property.
+
+        :returns: app Property
+        :rtype: str
+        """
         return self._app
 
     @app.setter
     def app(self, value) -> None:
         assert isinstance(value, (property, str, App, type(None)))
         if isinstance(value, property):
             # initial value not specified, use default
             value = self._app
         if isinstance(value, App):
             value = value.id
         self._app = value
 
     @property
     def collection(self) -> str:
+        """Return the collection property.
+
+        :returns: collection Property
+        :rtype: str
+        """
         return self._collection
 
     @collection.setter
     def collection(self, value: str) -> None:
         assert isinstance(value, (property, str, Collection, type(None)))
         if isinstance(value, property):
             # initial value not specified, use default
@@ -569,15 +589,37 @@
                 f"slug attribute is not of type {str}, got {type(self.slug)}"
             )
         return f"/source_query/{self.slug}"
 
 
 @dataclass
 class Actionflow(ResourceType):
-    """Actionflow dataclass."""
+    """Actionflow resource type.
+
+    Usage::
+
+        >>> from clappform import Clappform
+        >>> import clappform.dataclasses as r
+        >>> c = Clappform(
+        ...     "https://app.clappform.com",
+        ...     "j.doe@clappform.com",
+        ...     "S3cr3tP4ssw0rd!",
+        ... )
+        >>> new_actionflow = r.Actionflow(
+        ...     name="Periodic housekeeping",
+        ...     settings={},
+        ... )
+        >>> c.create(new_collection)
+        Actionflow(id=48, name='Periodic housekeeping', settings={}, cronjobs=None, ...
+        >>> actionflow = c.get(r.Actionflow(id=48))
+        >>> c.delete(actionflow)
+        ApiResponse(code=200, message='Deleted action flow.', response_id='648083113...v
+        >>> for af in c.get(r.Actionflow()):
+        ...     print(f"{af.id}: {af.name}")
+    """
 
     id: int = None
     name: str = None
     settings: dict = None
     cronjobs: list = None
     tasks: list = None
 
@@ -627,41 +669,101 @@
 
     def create_path(self) -> str:
         return "/questionnaire"
 
 
 @dataclass
 class User(ResourceType):
-    """User dataclass."""
+    """User resource type.
+
+    Usage::
 
+        >>> from clappform import Clappform
+        >>> import clappform.dataclasses as r
+        >>> c = Clappform(
+        ...     "https://app.clappform.com",
+        ...     "j.doe@clappform.com",
+        ...     "S3cr3tP4ssw0rd!",
+        ... )
+        >>> user = c.get(r.User(email="j.doe@clappform.com")
+        >>> new_user = r.User(
+        ...     email="g.washington@clappform.com",
+        ...     first_name="George",
+        ...     last_name="Washington",
+        ...     password="HavntGotWoodenTeeth",
+        ... )
+        >>> c.create(new_user)
+        User(email='g.washington@clappform.com', extra_information={}, first_name='G...
+        >>> query = c.get(r.Query(slug="f1cb2ba5-64a7-4056-99d5-7d639557970f"))
+        >>> c.delete(query)
+        ApiResponse(code=200, message='Successfully deactivated user, with email: g....
+        >>> for user in c.get(r.User()):
+        ...     print(f"{user.email}: {user.first_name} {user.last_name}")
+    """
+
+    #: Email address of the user.
     email: str = None
+    #: Dictionary object describing extra related information about the user.
     extra_information: dict = None
+    #: User's first name.
     first_name: str = None
+    #: User's last name.
     last_name: str = None
+    #: Whether user can authenticate or not.
     is_active: bool = None
+    #: Numeric id used for internal identifaction.
     id: int = None
+    #: User's phone number.
     phone: str = None
+    #: Dictionary object containing notifications, emails, sms or whatsapp messages.
+    #: ``extended=True``
     messages: dict = None
+    #: Unix timestamp of when the user was last online. ``extended=True``
     last_online: int = None
+    #: List of permissions this user has. ``extended=True``
     permissions: list[str] = None
+    #: ``extended=True``
     roles: list[dict] = None
+    #: Password of the user. Only used when creating a user.
+    password: str = field(init=True, repr=False, default=None)
+    #: Used by ``get`` to gauge whether to fetch fully expanded user object.
     extended: bool = field(init=True, repr=False, default=False)
 
     def one_or_all_path(self) -> str:
+        """Return the path to retreive this User.
+
+        :returns: User HTTP path
+        :rtype: str
+        """
         if self.email is None:
             return self.all_path()
         return self.one_path()
 
     def all_path(self) -> str:
+        """Return the path to retreive all Users.
+
+        :returns: User HTTP path
+        :rtype: str
+        """
         extended = self.bool_to_lower(bool(self.extended))
         return f"/users?extended={extended}"
 
     def one_path(self) -> str:
+        """Return the path to retreive this User.
+
+        :returns: User HTTP path
+        :rtype: str
+        """
         extended = self.bool_to_lower(bool(self.extended))
         if not isinstance(self.email, str):
             raise TypeError(
                 f"email attribute is not of type {str}, got {type(self.email)}"
             )
         return f"/user/{self.email}?extended={extended}"
 
     def create_path(self) -> str:
+        """Return the path to create a Collection.
+
+        :returns: Collection HTTP path
+        :rtype: str
+        """
         return "/user"
```

### Comparing `clappform-3.0.0a2/src/clappform/exceptions.py` & `clappform-3.0.0a3/src/clappform/exceptions.py`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a2/src/clappform.egg-info/PKG-INFO` & `clappform-3.0.0a3/src/clappform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

