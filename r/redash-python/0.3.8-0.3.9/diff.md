# Comparing `tmp/redash-python-0.3.8.tar.gz` & `tmp/redash-python-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redash-python-0.3.8.tar", last modified: Tue Sep  6 08:34:38 2022, max compression
+gzip compressed data, was "redash-python-0.3.9.tar", last modified: Tue Sep  6 08:45:45 2022, max compression
```

## Comparing `redash-python-0.3.8.tar` & `redash-python-0.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:34:38.644575 redash-python-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-09-06 08:34:15.000000 redash-python-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3880 2022-09-06 08:34:38.644575 redash-python-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3160 2022-09-06 08:34:15.000000 redash-python-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-09-06 08:34:15.000000 redash-python-0.3.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:34:38.640575 redash-python-0.3.8/redash_python/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/redash.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:34:38.644575 redash-python-0.3.8/redash_python/services/
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/alerts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3039 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/data_sources.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/destinations.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     5256 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     3412 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/queries.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/query_snippets.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/users.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-09-06 08:34:15.000000 redash-python-0.3.8/redash_python/services/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:34:38.644575 redash-python-0.3.8/redash_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3880 2022-09-06 08:34:38.000000 redash-python-0.3.8/redash_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-09-06 08:34:38.000000 redash-python-0.3.8/redash_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 08:34:38.000000 redash-python-0.3.8/redash_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-06 08:34:38.000000 redash-python-0.3.8/redash_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-06 08:34:38.000000 redash-python-0.3.8/redash_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 08:34:38.644575 redash-python-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:45:45.307768 redash-python-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-09-06 08:45:22.000000 redash-python-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3880 2022-09-06 08:45:45.307768 redash-python-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3160 2022-09-06 08:45:22.000000 redash-python-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-09-06 08:45:22.000000 redash-python-0.3.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:45:45.303768 redash-python-0.3.9/redash_python/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/redash.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:45:45.307768 redash-python-0.3.9/redash_python/services/
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3039 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5142 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3412 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/queries.py
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/query_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/users.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-09-06 08:45:22.000000 redash-python-0.3.9/redash_python/services/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:45:45.303768 redash-python-0.3.9/redash_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3880 2022-09-06 08:45:45.000000 redash-python-0.3.9/redash_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      687 2022-09-06 08:45:45.000000 redash-python-0.3.9/redash_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 08:45:45.000000 redash-python-0.3.9/redash_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-06 08:45:45.000000 redash-python-0.3.9/redash_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-06 08:45:45.000000 redash-python-0.3.9/redash_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 08:45:45.307768 redash-python-0.3.9/setup.cfg
```

### Comparing `redash-python-0.3.8/LICENSE` & `redash-python-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `redash-python-0.3.8/PKG-INFO` & `redash-python-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redash-python
-Version: 0.3.8
+Version: 0.3.9
 Summary: A more complete Python client for the Redash API
 Author-email: blacksuan19 <py@blacksuan19.dev>
 License: BSD-2-Clause
 Project-URL: Homepage, https://blacksuan19.dev/redash-python
 Project-URL: Documentation, https://blacksuan19.dev/redash-python
 Project-URL: Repository, https://github.com/blacksuan19/redash-python/
 Project-URL: Issues, https://github.com/blacksuan19/redash-python/issues
```

### Comparing `redash-python-0.3.8/README.md` & `redash-python-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `redash-python-0.3.8/pyproject.toml` & `redash-python-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "redash-python"
-version = "0.3.8"
+version = "0.3.9"
 description = "A more complete Python client for the Redash API"
 readme = "README.md"
 authors = [{ name = "blacksuan19", email = "py@blacksuan19.dev" }]
 license = {text = "BSD-2-Clause"}
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -25,15 +25,15 @@
 Homepage = "https://blacksuan19.dev/redash-python"
 Documentation = "https://blacksuan19.dev/redash-python"
 Repository = "https://github.com/blacksuan19/redash-python/"
 Issues = "https://github.com/blacksuan19/redash-python/issues"
 
 
 [tool.bumpver]
-current_version = "0.3.8"
+current_version = "0.3.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `redash-python-0.3.8/redash_python/redash.py` & `redash-python-0.3.9/redash_python/redash.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     GroupsService,
     QSnipsService,
     QueriesService,
     UsersService,
     WidgetsService,
 )
 
-version = "0.3.8"
+version = "0.3.9"
 
 
 class Redash:
     """
     Top Class of The Redash API Client hierarchy.
 
     Args:
```

### Comparing `redash-python-0.3.8/redash_python/services/base.py` & `redash-python-0.3.9/redash_python/services/base.py`

 * *Files identical despite different names*

### Comparing `redash-python-0.3.8/redash_python/services/dashboards.py` & `redash-python-0.3.9/redash_python/services/dashboards.py`

 * *Files identical despite different names*

### Comparing `redash-python-0.3.8/redash_python/services/mixins.py` & `redash-python-0.3.9/redash_python/services/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,20 +68,15 @@
         if obj_id is None:
             return None
 
         return self.get(obj_id)
 
     def get_id(self, name_or_slug: str) -> Optional[int]:
         """Get the ID for an object by name or slug, returns None if not found"""
-        all_obj: List[Dict] = self.get_all()
-
-        if "results" in all_obj:
-            all_obj = all_obj["results"]
-
-        for obj in all_obj:
+        for obj in self.get_all():
             if obj.get("name") == name_or_slug or obj.get("slug") == name_or_slug:
                 return obj.get("id")
 
         return None
 
 
 class TagsMixin:
```

### Comparing `redash-python-0.3.8/redash_python/services/queries.py` & `redash-python-0.3.9/redash_python/services/queries.py`

 * *Files identical despite different names*

### Comparing `redash-python-0.3.8/redash_python/services/users.py` & `redash-python-0.3.9/redash_python/services/users.py`

 * *Files identical despite different names*

### Comparing `redash-python-0.3.8/redash_python/services/widgets.py` & `redash-python-0.3.9/redash_python/services/widgets.py`

 * *Files identical despite different names*

### Comparing `redash-python-0.3.8/redash_python.egg-info/PKG-INFO` & `redash-python-0.3.9/redash_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redash-python
-Version: 0.3.8
+Version: 0.3.9
 Summary: A more complete Python client for the Redash API
 Author-email: blacksuan19 <py@blacksuan19.dev>
 License: BSD-2-Clause
 Project-URL: Homepage, https://blacksuan19.dev/redash-python
 Project-URL: Documentation, https://blacksuan19.dev/redash-python
 Project-URL: Repository, https://github.com/blacksuan19/redash-python/
 Project-URL: Issues, https://github.com/blacksuan19/redash-python/issues
```

### Comparing `redash-python-0.3.8/redash_python.egg-info/SOURCES.txt` & `redash-python-0.3.9/redash_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

