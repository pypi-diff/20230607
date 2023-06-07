# Comparing `tmp/autotraders-1.4.2.tar.gz` & `tmp/autotraders-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.4.2.tar", last modified: Wed Jun  7 02:54:04 2023, max compression
+gzip compressed data, was "autotraders-1.4.3.tar", last modified: Wed Jun  7 02:59:56 2023, max compression
```

## Comparing `autotraders-1.4.2.tar` & `autotraders-1.4.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.384961 autotraders-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-07 02:53:48.000000 autotraders-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-07 02:54:04.384961 autotraders-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-07 02:53:48.000000 autotraders-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.376960 autotraders-1.4.2/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.380960 autotraders-1.4.2/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.380960 autotraders-1.4.2/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.380960 autotraders-1.4.2/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.384961 autotraders-1.4.2/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.384961 autotraders-1.4.2/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.380960 autotraders-1.4.2/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-07 02:54:04.000000 autotraders-1.4.2/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-07 02:54:04.000000 autotraders-1.4.2/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:54:04.000000 autotraders-1.4.2/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 02:54:04.000000 autotraders-1.4.2/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 02:54:04.000000 autotraders-1.4.2/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-07 02:53:48.000000 autotraders-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 02:54:04.384961 autotraders-1.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.384961 autotraders-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-07 02:53:48.000000 autotraders-1.4.2/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-07 02:53:48.000000 autotraders-1.4.2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-07 02:53:48.000000 autotraders-1.4.2/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 02:53:48.000000 autotraders-1.4.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.004780 autotraders-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-07 02:59:41.000000 autotraders-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-07 02:59:56.004780 autotraders-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-07 02:59:41.000000 autotraders-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-07 02:59:55.000000 autotraders-1.4.3/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-07 02:59:55.000000 autotraders-1.4.3/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:59:55.000000 autotraders-1.4.3/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 02:59:55.000000 autotraders-1.4.3/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 02:59:55.000000 autotraders-1.4.3/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-07 02:59:41.000000 autotraders-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 02:59:56.004780 autotraders-1.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.004780 autotraders-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-07 02:59:41.000000 autotraders-1.4.3/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-07 02:59:41.000000 autotraders-1.4.3/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-07 02:59:41.000000 autotraders-1.4.3/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 02:59:41.000000 autotraders-1.4.3/tests/test_util.py
```

### Comparing `autotraders-1.4.2/LICENSE` & `autotraders-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/PKG-INFO` & `autotraders-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.4.2
+Version: 1.4.3
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.4.2/README.md` & `autotraders-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/agent.py` & `autotraders-1.4.3/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/faction/__init__.py` & `autotraders-1.4.3/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/faction/contract.py` & `autotraders-1.4.3/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/map/system.py` & `autotraders-1.4.3/autotraders/map/system.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/map/waypoint.py` & `autotraders-1.4.3/autotraders/map/waypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,12 +60,13 @@
             j = r.json()
             if "error" in j:
                 raise IOError(j["error"]["message"])
             waypoints = []
             for w in j["data"]:
                 waypoint = Waypoint(w["symbol"], session, w)
                 waypoints.append(waypoint)
+            return waypoints, j["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
 
     def __eq__(self, other):
         return self.symbol == other.symbol
```

### Comparing `autotraders-1.4.2/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.4.3/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.4.3/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.4.3/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.4.3/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/paginated_list.py` & `autotraders-1.4.3/autotraders/paginated_list.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/session.py` & `autotraders-1.4.3/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/shared_models/map_symbol.py` & `autotraders-1.4.3/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/shared_models/transaction.py` & `autotraders-1.4.3/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/ship/__init__.py` & `autotraders-1.4.3/autotraders/ship/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/ship/cargo.py` & `autotraders-1.4.3/autotraders/ship/cargo.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/ship/nav.py` & `autotraders-1.4.3/autotraders/ship/nav.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/ship/ship_components.py` & `autotraders-1.4.3/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/space_traders_entity.py` & `autotraders-1.4.3/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/status.py` & `autotraders-1.4.3/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders/util.py` & `autotraders-1.4.3/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/autotraders.egg-info/PKG-INFO` & `autotraders-1.4.3/autotraders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.4.2
+Version: 1.4.3
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.4.2/autotraders.egg-info/SOURCES.txt` & `autotraders-1.4.3/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/pyproject.toml` & `autotraders-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.4.2"
+version = "1.4.3"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.4.2/tests/test_init.py` & `autotraders-1.4.3/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/tests/test_ship.py` & `autotraders-1.4.3/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.2/tests/test_util.py` & `autotraders-1.4.3/tests/test_util.py`

 * *Files identical despite different names*

