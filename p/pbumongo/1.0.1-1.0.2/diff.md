# Comparing `tmp/pbumongo-1.0.1.tar.gz` & `tmp/pbumongo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbumongo-1.0.1.tar", last modified: Mon Apr  3 06:12:40 2023, max compression
+gzip compressed data, was "pbumongo-1.0.2.tar", last modified: Tue Jun  6 23:19:47 2023, max compression
```

## Comparing `pbumongo-1.0.1.tar` & `pbumongo-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-03 06:12:40.060660 pbumongo-1.0.1/
--rw-rw-r--   0 peter     (1000) peter     (1000)     9538 2023-04-03 06:12:40.060660 pbumongo-1.0.1/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     7846 2023-04-03 06:12:03.000000 pbumongo-1.0.1/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-03 06:12:40.059661 pbumongo-1.0.1/pbumongo/
--rw-r--r--   0 peter     (1000) peter     (1000)      183 2023-01-24 06:59:15.000000 pbumongo-1.0.1/pbumongo/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      436 2023-01-24 06:56:21.000000 pbumongo-1.0.1/pbumongo/mongo_connection.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2130 2023-01-24 08:05:48.000000 pbumongo-1.0.1/pbumongo/mongo_document.py
--rw-r--r--   0 peter     (1000) peter     (1000)    11994 2023-03-30 05:12:01.000000 pbumongo-1.0.1/pbumongo/mongo_store.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-03 06:12:40.060660 pbumongo-1.0.1/pbumongo.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     9538 2023-04-03 06:12:39.000000 pbumongo-1.0.1/pbumongo.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      309 2023-04-03 06:12:39.000000 pbumongo-1.0.1/pbumongo.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-04-03 06:12:39.000000 pbumongo-1.0.1/pbumongo.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-01-24 06:59:18.000000 pbumongo-1.0.1/pbumongo.egg-info/not-zip-safe
--rw-rw-r--   0 peter     (1000) peter     (1000)       19 2023-04-03 06:12:39.000000 pbumongo-1.0.1/pbumongo.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        9 2023-04-03 06:12:39.000000 pbumongo-1.0.1/pbumongo.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-04-03 06:12:40.060660 pbumongo-1.0.1/setup.cfg
--rw-r--r--   0 peter     (1000) peter     (1000)      667 2023-04-03 06:10:13.000000 pbumongo-1.0.1/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-06 23:19:47.065248 pbumongo-1.0.2/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9697 2023-06-06 23:19:47.065248 pbumongo-1.0.2/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7981 2023-06-06 23:18:57.000000 pbumongo-1.0.2/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-06 23:19:47.064248 pbumongo-1.0.2/pbumongo/
+-rw-r--r--   0 peter     (1000) peter     (1000)      183 2023-01-24 06:59:15.000000 pbumongo-1.0.2/pbumongo/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      679 2023-06-06 23:07:59.000000 pbumongo-1.0.2/pbumongo/mongo_connection.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2130 2023-01-24 08:05:48.000000 pbumongo-1.0.2/pbumongo/mongo_document.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    12202 2023-06-06 23:13:09.000000 pbumongo-1.0.2/pbumongo/mongo_store.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-06 23:19:47.065248 pbumongo-1.0.2/pbumongo.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9697 2023-06-06 23:19:46.000000 pbumongo-1.0.2/pbumongo.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      309 2023-06-06 23:19:46.000000 pbumongo-1.0.2/pbumongo.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-06 23:19:46.000000 pbumongo-1.0.2/pbumongo.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-01-24 06:59:18.000000 pbumongo-1.0.2/pbumongo.egg-info/not-zip-safe
+-rw-rw-r--   0 peter     (1000) peter     (1000)       19 2023-06-06 23:19:46.000000 pbumongo-1.0.2/pbumongo.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        9 2023-06-06 23:19:46.000000 pbumongo-1.0.2/pbumongo.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-06 23:19:47.065248 pbumongo-1.0.2/setup.cfg
+-rw-r--r--   0 peter     (1000) peter     (1000)      667 2023-06-06 23:19:08.000000 pbumongo-1.0.2/setup.py
```

### Comparing `pbumongo-1.0.1/PKG-INFO` & `pbumongo-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbumongo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Basic MongoDB wrapper for object-oriented collection handling
 Home-page: https://github.com/ilfrich/pbu-mongo
 Author: Peter Ilfrich
 Author-email: das-peter@gmx.de
 License: Apache-2.0
 Description: # Python Basic Utilities - Mongo `pbumongo`
         
@@ -12,14 +12,15 @@
         
         **Table of Contents**
         
         1. [Installation](#installation)
         2. [Usage](#usage)
         3. [Classes](#classes)
             1. [AbstractMongoStore](#abstractmongostore) - abstract class for handling MongoDB collection access
+               1. [MongoConnection](#mongoconnection) - a helper class to assist with creating multiple store instances 
             2. [AbstractMongoDocument](#abstractmongodocument) - abstract class for wrapping MongoDB BSON documents
         
         
         ## Installation
         
         Install via pip:
         
@@ -97,14 +98,16 @@
                 user.username = username
                 user.password = crypt.crypt(password, crypt.METHOD_MD5)
                 # store in database and return document
                 user_id = self.create(user)
                 return self.get(user_id)
         ```
         
+        #### MongoConnection
+        
         To use these classes in your application, you can use the MongoConnection helper or create the `UserStore` class
         instance directly. The `MongoConnection` helper is useful, when you have a lot of collections and don't want to repeat
         the mongo connection URL and DB name for every constructor.
         
         ```python
         from pbumongo import MongoConnection
         from mypackage import UserStore  # see implementation above
```

### Comparing `pbumongo-1.0.1/README.md` & `pbumongo-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 **Table of Contents**
 
 1. [Installation](#installation)
 2. [Usage](#usage)
 3. [Classes](#classes)
     1. [AbstractMongoStore](#abstractmongostore) - abstract class for handling MongoDB collection access
+       1. [MongoConnection](#mongoconnection) - a helper class to assist with creating multiple store instances 
     2. [AbstractMongoDocument](#abstractmongodocument) - abstract class for wrapping MongoDB BSON documents
 
 
 ## Installation
 
 Install via pip:
 
@@ -89,14 +90,16 @@
         user.username = username
         user.password = crypt.crypt(password, crypt.METHOD_MD5)
         # store in database and return document
         user_id = self.create(user)
         return self.get(user_id)
 ```
 
+#### MongoConnection
+
 To use these classes in your application, you can use the MongoConnection helper or create the `UserStore` class
 instance directly. The `MongoConnection` helper is useful, when you have a lot of collections and don't want to repeat
 the mongo connection URL and DB name for every constructor.
 
 ```python
 from pbumongo import MongoConnection
 from mypackage import UserStore  # see implementation above
```

### Comparing `pbumongo-1.0.1/pbumongo/mongo_document.py` & `pbumongo-1.0.2/pbumongo/mongo_document.py`

 * *Files identical despite different names*

### Comparing `pbumongo-1.0.1/pbumongo/mongo_store.py` & `pbumongo-1.0.2/pbumongo/mongo_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,25 +25,27 @@
 class AbstractMongoStore(ABC):
     """
     Abstract base class for MongoDB stores. A store is represented by a collection in MongoDB and contains one type of
     documents, which can be represented by a MongoDocument sub-class.
     """
 
     @abstractmethod
-    def __init__(self, mongo_url: str, db_name: str, collection_name: str,
-                 deserialised_class: Type[AbstractMongoDocument], data_model_version=1):
+    def __init__(self, mongo_url: str = "mongodb://localhost:27017", db_name: str = None, collection_name: str = None,
+                 deserialised_class: Type[AbstractMongoDocument] = None, data_model_version=1):
         """
         Creates a new instance of this store providing credentials and behaviour parameters.
         :param mongo_url: the url to the mongo database (including credentials)
         :param db_name: the database name on the mongo database server
         :param collection_name: the collection name within the database selected
         :param deserialised_class: a sub-class of AbstractMongoDocument, which can be used to de-serialise documents in
         MongoDB into objects that can be handled easier.
         :param data_model_version: the data model version of this store.
         """
+        if None in [db_name, collection_name]:
+            raise ValueError("Parameters db_name and collection_name are mandatory and have to be provided.")
         # e.g. mongodb://localhost:27017
         self.mongo_url = mongo_url
 
         # connect
         client = pymongo.MongoClient(self.mongo_url)
         self.db = client[db_name]
         self.collection = self.db[collection_name]
```

### Comparing `pbumongo-1.0.1/pbumongo.egg-info/PKG-INFO` & `pbumongo-1.0.2/pbumongo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbumongo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Basic MongoDB wrapper for object-oriented collection handling
 Home-page: https://github.com/ilfrich/pbu-mongo
 Author: Peter Ilfrich
 Author-email: das-peter@gmx.de
 License: Apache-2.0
 Description: # Python Basic Utilities - Mongo `pbumongo`
         
@@ -12,14 +12,15 @@
         
         **Table of Contents**
         
         1. [Installation](#installation)
         2. [Usage](#usage)
         3. [Classes](#classes)
             1. [AbstractMongoStore](#abstractmongostore) - abstract class for handling MongoDB collection access
+               1. [MongoConnection](#mongoconnection) - a helper class to assist with creating multiple store instances 
             2. [AbstractMongoDocument](#abstractmongodocument) - abstract class for wrapping MongoDB BSON documents
         
         
         ## Installation
         
         Install via pip:
         
@@ -97,14 +98,16 @@
                 user.username = username
                 user.password = crypt.crypt(password, crypt.METHOD_MD5)
                 # store in database and return document
                 user_id = self.create(user)
                 return self.get(user_id)
         ```
         
+        #### MongoConnection
+        
         To use these classes in your application, you can use the MongoConnection helper or create the `UserStore` class
         instance directly. The `MongoConnection` helper is useful, when you have a lot of collections and don't want to repeat
         the mongo connection URL and DB name for every constructor.
         
         ```python
         from pbumongo import MongoConnection
         from mypackage import UserStore  # see implementation above
```

### Comparing `pbumongo-1.0.1/setup.py` & `pbumongo-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="pbumongo",
-      version="1.0.1",
+      version="1.0.2",
       description="Basic MongoDB wrapper for object-oriented collection handling",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/ilfrich/pbu-mongo",
       author="Peter Ilfrich",
       author_email="das-peter@gmx.de",
       license="Apache-2.0",
```

