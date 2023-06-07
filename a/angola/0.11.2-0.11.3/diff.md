# Comparing `tmp/angola-0.11.2.tar.gz` & `tmp/angola-0.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.11.2.tar", last modified: Tue Jun  6 03:59:47 2023, max compression
+gzip compressed data, was "angola-0.11.3.tar", last modified: Wed Jun  7 07:05:25 2023, max compression
```

## Comparing `angola-0.11.2.tar` & `angola-0.11.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-06 03:59:47.548185 angola-0.11.2/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.11.2/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.11.2/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-06-06 03:59:47.548263 angola-0.11.2/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      877 2022-11-30 18:28:40.000000 angola-0.11.2/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-06 03:59:47.548534 angola-0.11.2/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-06 03:59:34.000000 angola-0.11.2/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-06 03:59:47.542195 angola-0.11.2/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-06 03:59:47.545549 angola-0.11.2/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      314 2023-04-30 19:58:20.000000 angola-0.11.2/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    48027 2023-05-30 03:49:44.000000 angola-0.11.2/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.11.2/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.11.2/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.11.2/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    19000 2023-06-06 03:59:22.000000 angola-0.11.2/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-06 03:59:47.546494 angola-0.11.2/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-06-06 03:59:47.000000 angola-0.11.2/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-06 03:59:47.000000 angola-0.11.2/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-06 03:59:47.000000 angola-0.11.2/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-06 03:59:47.000000 angola-0.11.2/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-06 03:59:47.000000 angola-0.11.2/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-06 03:59:47.548015 angola-0.11.2/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.11.2/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.11.2/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.11.2/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.11.2/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.11.2/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-07 07:05:25.608914 angola-0.11.3/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.11.3/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.11.3/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-06-07 07:05:25.608986 angola-0.11.3/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      877 2022-11-30 18:28:40.000000 angola-0.11.3/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-07 07:05:25.609221 angola-0.11.3/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-07 07:05:15.000000 angola-0.11.3/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-07 07:05:25.602844 angola-0.11.3/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-07 07:05:25.606395 angola-0.11.3/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      314 2023-04-30 19:58:20.000000 angola-0.11.3/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    48027 2023-05-30 03:49:44.000000 angola-0.11.3/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.11.3/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.11.3/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.11.3/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18970 2023-06-07 07:05:05.000000 angola-0.11.3/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-07 07:05:25.607373 angola-0.11.3/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-06-07 07:05:25.000000 angola-0.11.3/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-07 07:05:25.000000 angola-0.11.3/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-07 07:05:25.000000 angola-0.11.3/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-07 07:05:25.000000 angola-0.11.3/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-07 07:05:25.000000 angola-0.11.3/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-07 07:05:25.608815 angola-0.11.3/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.11.3/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.11.3/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.11.3/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.11.3/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.11.3/tests/test_query.py
```

### Comparing `angola-0.11.2/LICENSE` & `angola-0.11.3/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.11.2/PKG-INFO` & `angola-0.11.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.11.2
+Version: 0.11.3
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.11.2/README.md` & `angola-0.11.3/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.11.2/setup.py` & `angola-0.11.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.11.2"
+VERSION = "0.11.3"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.11.2/src/angola/database.py` & `angola-0.11.3/src/angola/database.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.2/src/angola/dict_mutator.py` & `angola-0.11.3/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.2/src/angola/dict_query.py` & `angola-0.11.3/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.2/src/angola/lib.py` & `angola-0.11.3/src/angola/lib.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.2/src/angola/lib_xql.py` & `angola-0.11.3/src/angola/lib_xql.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,30 +18,30 @@
         :param ALIAS: str = alias
         :param FILTERS: dict = filters
         :param SORT: list/str = sort 
         :param OFFSET: int = the offset of the limit, default=0
         :param LIMIT: int = the limit of result, default=10
         :param PAGE: int = help calculate the skip by using a page number. 
         :param JOIN: list[XQL]
-        :param COUNT_AS: str =  To count all the document, and return the value. Alias to `COLLECT WITH COUNT INTO`
+        :param RETURN_COUNT: bool =  Will return a count of all matched documents
         :param RETURN: str = string representation
         :param MERGE: str = on JOIN, to merge the data.
             ie: MERGE: "{__profile: profile}" 
             Can be done manually with RETURN MERGE(doc, {data})
 
     """
     FROM: str = None
     ALIAS: str = None
     FILTERS: dict = {}
     SORT: list = []
     OFFSET: int = 0
     LIMIT: int = 10
     PAGE: int = 1
     JOIN: list = []
-    COUNT_AS: str = None
+    RETURN_COUNT: str = None
     RETURN: str = None
     MERGE: str = None
 
 
 # -----------------------------------------------------------------------------
 # === MACROS ------------------------------------------------------------------
 
@@ -368,15 +368,15 @@
 def prepare_xql(xql: dict) -> dict:
     _defaults = {
         "FROM": None,
         "ALIAS": "root__",
         "FILTERS": {},
         "SORT": None,
         "OFFSET": None,
-        "COUNT_AS": None,
+        "RETURN_COUNT": False,
         "LIMIT": 10,
         "PAGE": 1,
         "JOIN": [],
         "RETURN": None,
         "RETURN_WITH": None,
         **xql
     }
@@ -436,15 +436,15 @@
         ALIAS: str = alias
         FILTERS: dict = filters
         SORT: list/str = sort 
         OFFSET: int = the offset of the limit, default=0
         LIMIT: int = the limit of result, default=10
         PAGE: int = help calculate the offset by using a page number. 
         JOIN: list[XQL]
-        COUNT_AS: str =  To count all the document, and return the value. Alias to `COLLECT WITH COUNT INTO`
+        RETURN_COUNT: str =  To count all the document, and return the value. Alias to `COLLECT WITH COUNT INTO`
         RETURN: str = string representation
         MERGE: str = on JOIN, to merge the data.
             ie: MERGE: "{__profile: profile}" 
             Can be done manually with RETURN MERGE(doc, {data})
 
         # TODO
         - WHEN: ? = a conditional to evaluate before running
@@ -529,15 +529,15 @@
     COLLECTION = xql.get("FROM")
     FILTERS = xql.get("FILTERS") or {}
     SORTS = xql.get("SORT")
     OFFSET = xql.get("OFFSET")
     LIMIT = xql.get("LIMIT") or 10
     PAGE = xql.get("PAGE") or 1
     JOINS = xql.get("JOIN") or []
-    COUNT_AS = xql.get("COUNT_AS")
+    RETURN_COUNT = xql.get("RETURN_COUNT")
     COLLECTS = xql.get("COLLECT") or []
     RETURN = xql.get("RETURN") or ALIAS
 
     # work with take/skip
     if OFFSET is None:
         page = PAGE or 1
         per_page = max_limit if per_page > max_limit else LIMIT
@@ -548,16 +548,14 @@
 
 
     # unique num to give each field to prevent name collision
     num_ = lib.gen_number(6)
     aql_filter, filter_vars = filter_builder(FILTERS, propkey=ALIAS)
     aql_sorting = sort_builder(SORTS, propkey=ALIAS)
     aql_collects = collects_builder(COLLECTS, propkey=ALIAS)
-    if COUNT_AS:
-        aql_collects += " COLLECT WITH COUNT INTO %s " % COUNT_AS
 
     bind_vars = {}
 
     # SUBQUERY/JOINS
     subquery = ""
     for xql2 in JOINS:
         xql2 = prepare_xql(xql2)
@@ -570,14 +568,17 @@
     query += aql_filter
     query += subquery
     query += aql_collects
     query += " LIMIT @offset_%s, @limit_%s " % (num_, num_)
     query += aql_sorting
     query += "RETURN UNSET_RECURSIVE(%s, ['_id', '_rev', '_old_rev'])" % RETURN
 
+    if RETURN_COUNT:
+        query = "RETURN LENGTH(%s)" % query
+
     bind_vars.update({
         **filter_vars,
         "offset_%s" % num_: OFFSET,
         "limit_%s" % num_: LIMIT,
         "@collection_%s" % num_: COLLECTION
     })
     return query, bind_vars
```

### Comparing `angola-0.11.2/src/angola.egg-info/PKG-INFO` & `angola-0.11.3/src/angola.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.11.2
+Version: 0.11.3
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.11.2/tests/test_database.py` & `angola-0.11.3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.2/tests/test_dict_mutator.py` & `angola-0.11.3/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.2/tests/test_lib.py` & `angola-0.11.3/tests/test_lib.py`

 * *Files identical despite different names*

