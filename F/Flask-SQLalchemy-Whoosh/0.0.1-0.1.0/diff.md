# Comparing `tmp/flask_sqlalchemy_whoosh-0.0.1.tar.gz` & `tmp/flask_sqlalchemy_whoosh-0.1.0.tar.gz`

## Comparing `flask_sqlalchemy_whoosh-0.0.1.tar` & `flask_sqlalchemy_whoosh-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.0.1/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.0.1/src/flask_sqlalchemy_whoosh/__init__.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.0.1/src/flask_sqlalchemy_whoosh/mixin.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.0.1/src/flask_sqlalchemy_whoosh/searcher.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.0.1/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.0/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.0/src/flask_sqlalchemy_whoosh/__init__.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.0/src/flask_sqlalchemy_whoosh/mixin.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.0/src/flask_sqlalchemy_whoosh/searcher.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.0/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.0/PKG-INFO
```

### Comparing `flask_sqlalchemy_whoosh-0.0.1/src/flask_sqlalchemy_whoosh/mixin.py` & `flask_sqlalchemy_whoosh-0.1.0/src/flask_sqlalchemy_whoosh/mixin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from whoosh.qparser import QueryParser
 import sqlalchemy.sql
 from flask_sqlalchemy import SQLAlchemy
+from flask_sqlalchemy.query import Query
 
 from .searcher import WhooshSearcher
 
 
 class SearchableMixin():
     @classmethod
     def init_search(cls, searcher: WhooshSearcher, db: SQLAlchemy):
         cls.searcher = searcher
         cls.db = db
 
         cls.db.event.listen(db.session, 'before_commit', cls.before_commit)
         cls.db.event.listen(db.session, 'after_commit', cls.after_commit)
 
     @classmethod
-    def search(cls, field, term, page, per_page=20):
+    def search(cls, field: str, term: str, page: int=1, per_page: int=20) -> tuple(Query, int):
         ix = cls.searcher.get_index(cls)
         with ix.searcher() as searcher:
             parser = QueryParser(field, ix.schema)
             query = parser.parse(term)
             results = searcher.search_page(query, page, pagelen=per_page)
             total = len(results)
             ids = [r["id"] for r in results]
@@ -28,15 +29,14 @@
                 return cls.query.filter(sqlalchemy.sql.false()), 0
             
             when = {ids[i]: i for i in range(len(ids))}
             query = (cls.query.filter(cls.id.in_(ids)).order_by(
                 cls.db.case(when, value=cls.id)), total)
             return query
 
-
     @classmethod
     def before_commit(cls, session):
         session._changes = {
             'add': list(session.new),
             'update': list(session.dirty),
             'delete': list(session.deleted)
         }
```

### Comparing `flask_sqlalchemy_whoosh-0.0.1/src/flask_sqlalchemy_whoosh/searcher.py` & `flask_sqlalchemy_whoosh-0.1.0/src/flask_sqlalchemy_whoosh/searcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
 
 from whoosh.fields import Schema
 from whoosh.index import create_in, open_dir, FileIndex
 from whoosh.writing import AsyncWriter
 from flask_sqlalchemy.model import Model
+from flask import Flask
 
 
 class WhooshSearcher:
-    def __init__(self, app):
+    def __init__(self, app: Flask):
         if app is not None:
             self.init_app(app)
         
 
-    def init_app(self, app):
-        self._index_path = app.config.get("WHOOSH_INDEX_PATH") or "./whoosh"
+    def init_app(self, app: Flask, index_path="./whoosh"):
+        self._index_path = app.config.get("WHOOSH_INDEX_PATH") or index_path
 
-    def _check_index_exists(self, name):
+    def _check_index_exists(self, name: str):
         return os.path.exists(os.path.join(self._index_path, name))
 
     def _create_index(self, name: str, searchables: dict):
         schema = Schema()
         os.mkdir(os.path.join(self._index_path, name))
         # Create the search index
         ix = create_in(os.path.join(self._index_path, name), schema)
```

### Comparing `flask_sqlalchemy_whoosh-0.0.1/LICENSE` & `flask_sqlalchemy_whoosh-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_whoosh-0.0.1/pyproject.toml` & `flask_sqlalchemy_whoosh-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "flask-sqlalchemy-whoosh"
-version = "0.0.1"
+name = "Flask-SQLalchemy-Whoosh"
+version = "0.1.0"
 authors = [
   { name="Nick" },
 ]
 description = "A flask extension that adds full text search capabilites to your SQLAlchemy models using the Whoosh search engine"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -19,8 +19,9 @@
 dependencies = [
     "Flask-SQLAlchemy>=3.0.3",
     "Whoosh>=2.7.4"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Momo8289/Flask-SQLAlchemy-Whoosh"
-"Bug Tracker" = "https://github.com/Momo8289/Flask-SQLAlchemy-Whoosh/issues"
+"Bug Tracker" = "https://github.com/Momo8289/Flask-SQLAlchemy-Whoosh/issues"
+"Documentation" = "https://github.com/Momo8289/Flask-SQLAlchemy-Whoosh/wiki/Docs"
```

