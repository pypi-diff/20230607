# Comparing `tmp/flask_sqlalchemy_whoosh-0.1.1.tar.gz` & `tmp/flask_sqlalchemy_whoosh-0.1.2.tar.gz`

## Comparing `flask_sqlalchemy_whoosh-0.1.1.tar` & `flask_sqlalchemy_whoosh-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.1/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.1/src/flask_sqlalchemy_whoosh/__init__.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.1/src/flask_sqlalchemy_whoosh/mixin.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.1/src/flask_sqlalchemy_whoosh/searcher.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.1/LICENSE
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.1/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/src/flask_sqlalchemy_whoosh/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/src/flask_sqlalchemy_whoosh/mixin.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/src/flask_sqlalchemy_whoosh/searcher.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/PKG-INFO
```

### Comparing `flask_sqlalchemy_whoosh-0.1.1/src/flask_sqlalchemy_whoosh/mixin.py` & `flask_sqlalchemy_whoosh-0.1.2/src/flask_sqlalchemy_whoosh/mixin.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,20 +12,28 @@
         cls.searcher = searcher
         cls.db = db
 
         cls.db.event.listen(db.session, 'before_commit', cls.before_commit)
         cls.db.event.listen(db.session, 'after_commit', cls.after_commit)
 
     @classmethod
-    def search(cls, field: str, term: str, page: int=1, per_page: int=20) -> tuple[Query, int]:
+    def search(cls, field: str, term: str, **kwargs) -> tuple[Query, int]:
+        paged = kwargs.get("paged", False)
+        page = kwargs.get("page", 1)
+        per_page = kwargs.get("per_page", 10)
+        limit = kwargs.get("limit", None)
+
         ix = cls.searcher.get_index(cls)
         with ix.searcher() as searcher:
             parser = QueryParser(field, ix.schema)
             query = parser.parse(term)
-            results = searcher.search_page(query, page, pagelen=per_page)
+            if paged:
+                results = searcher.search_page(query, page, pagelen=per_page)
+            else:
+                results = searcher.search(query, limit=limit)
             total = len(results)
             ids = [r["id"] for r in results]
 
             if total == 0:
                 return cls.query.filter(sqlalchemy.sql.false()), 0
             
             when = {ids[i]: i for i in range(len(ids))}
```

### Comparing `flask_sqlalchemy_whoosh-0.1.1/src/flask_sqlalchemy_whoosh/searcher.py` & `flask_sqlalchemy_whoosh-0.1.2/src/flask_sqlalchemy_whoosh/searcher.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_whoosh-0.1.1/LICENSE` & `flask_sqlalchemy_whoosh-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_whoosh-0.1.1/README.md` & `flask_sqlalchemy_whoosh-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_whoosh-0.1.1/pyproject.toml` & `flask_sqlalchemy_whoosh-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Flask-SQLalchemy-Whoosh"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Nick" },
 ]
 description = "A flask extension that adds full text search capabilites to your SQLAlchemy models using the Whoosh search engine"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `flask_sqlalchemy_whoosh-0.1.1/PKG-INFO` & `flask_sqlalchemy_whoosh-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SQLalchemy-Whoosh
-Version: 0.1.1
+Version: 0.1.2
 Summary: A flask extension that adds full text search capabilites to your SQLAlchemy models using the Whoosh search engine
 Project-URL: Homepage, https://github.com/Momo8289/Flask-SQLAlchemy-Whoosh
 Project-URL: Bug Tracker, https://github.com/Momo8289/Flask-SQLAlchemy-Whoosh/issues
 Project-URL: Documentation, https://github.com/Momo8289/Flask-SQLAlchemy-Whoosh/wiki/Docs
 Author: Nick
 License-File: LICENSE
 Classifier: Framework :: Flask
```

