# Comparing `tmp/flask_sqlalchemy_whoosh-0.1.2.tar.gz` & `tmp/flask_sqlalchemy_whoosh-0.1.3.tar.gz`

## Comparing `flask_sqlalchemy_whoosh-0.1.2.tar` & `flask_sqlalchemy_whoosh-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/src/flask_sqlalchemy_whoosh/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/src/flask_sqlalchemy_whoosh/mixin.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/src/flask_sqlalchemy_whoosh/searcher.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/LICENSE
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.3/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.3/src/flask_sqlalchemy_whoosh/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.3/src/flask_sqlalchemy_whoosh/mixin.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.3/src/flask_sqlalchemy_whoosh/searcher.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.3/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 flask_sqlalchemy_whoosh-0.1.3/PKG-INFO
```

### Comparing `flask_sqlalchemy_whoosh-0.1.2/src/flask_sqlalchemy_whoosh/mixin.py` & `flask_sqlalchemy_whoosh-0.1.3/src/flask_sqlalchemy_whoosh/mixin.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_whoosh-0.1.2/src/flask_sqlalchemy_whoosh/searcher.py` & `flask_sqlalchemy_whoosh-0.1.3/src/flask_sqlalchemy_whoosh/searcher.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_whoosh-0.1.2/LICENSE` & `flask_sqlalchemy_whoosh-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_whoosh-0.1.2/README.md` & `flask_sqlalchemy_whoosh-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,12 +55,12 @@
 
 
 # If you want to index a table that  already has entries, use the reindex method
 # It will index all entries in the table
 Product.reindex()
 
 # Use the search method to search a table
-results, total = Product.search("name", "nails", 1)
+results, total = Product.search("name", "nails")
 ```
```

### Comparing `flask_sqlalchemy_whoosh-0.1.2/pyproject.toml` & `flask_sqlalchemy_whoosh-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Flask-SQLalchemy-Whoosh"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Nick" },
 ]
 description = "A flask extension that adds full text search capabilites to your SQLAlchemy models using the Whoosh search engine"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `flask_sqlalchemy_whoosh-0.1.2/PKG-INFO` & `flask_sqlalchemy_whoosh-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SQLalchemy-Whoosh
-Version: 0.1.2
+Version: 0.1.3
 Summary: A flask extension that adds full text search capabilites to your SQLAlchemy models using the Whoosh search engine
 Project-URL: Homepage, https://github.com/Momo8289/Flask-SQLAlchemy-Whoosh
 Project-URL: Bug Tracker, https://github.com/Momo8289/Flask-SQLAlchemy-Whoosh/issues
 Project-URL: Documentation, https://github.com/Momo8289/Flask-SQLAlchemy-Whoosh/wiki/Docs
 Author: Nick
 License-File: LICENSE
 Classifier: Framework :: Flask
@@ -72,12 +72,12 @@
 
 
 # If you want to index a table that  already has entries, use the reindex method
 # It will index all entries in the table
 Product.reindex()
 
 # Use the search method to search a table
-results, total = Product.search("name", "nails", 1)
+results, total = Product.search("name", "nails")
 ```
```

