# Comparing `tmp/autotraders-1.4.1.tar.gz` & `tmp/autotraders-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.4.1.tar", last modified: Sun Jun  4 21:26:41 2023, max compression
+gzip compressed data, was "autotraders-1.4.2.tar", last modified: Wed Jun  7 02:54:04 2023, max compression
```

## Comparing `autotraders-1.4.1.tar` & `autotraders-1.4.2.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:26:41.587286 autotraders-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-04 21:26:27.000000 autotraders-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 21:26:41.587286 autotraders-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-04 21:26:27.000000 autotraders-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:26:41.583286 autotraders-1.4.1/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:26:41.583286 autotraders-1.4.1/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:26:41.583286 autotraders-1.4.1/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:26:41.587286 autotraders-1.4.1/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:26:41.587286 autotraders-1.4.1/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:26:41.587286 autotraders-1.4.1/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-04 21:26:27.000000 autotraders-1.4.1/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:26:41.583286 autotraders-1.4.1/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 21:26:41.000000 autotraders-1.4.1/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-04 21:26:41.000000 autotraders-1.4.1/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:26:41.000000 autotraders-1.4.1/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 21:26:41.000000 autotraders-1.4.1/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 21:26:41.000000 autotraders-1.4.1/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-04 21:26:27.000000 autotraders-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 21:26:41.587286 autotraders-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:26:41.587286 autotraders-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-04 21:26:27.000000 autotraders-1.4.1/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-04 21:26:27.000000 autotraders-1.4.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-04 21:26:27.000000 autotraders-1.4.1/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-04 21:26:27.000000 autotraders-1.4.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.384961 autotraders-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-07 02:53:48.000000 autotraders-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-07 02:54:04.384961 autotraders-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-07 02:53:48.000000 autotraders-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.376960 autotraders-1.4.2/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.380960 autotraders-1.4.2/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.380960 autotraders-1.4.2/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.380960 autotraders-1.4.2/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.384961 autotraders-1.4.2/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.384961 autotraders-1.4.2/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 02:53:48.000000 autotraders-1.4.2/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.380960 autotraders-1.4.2/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-07 02:54:04.000000 autotraders-1.4.2/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-07 02:54:04.000000 autotraders-1.4.2/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:54:04.000000 autotraders-1.4.2/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 02:54:04.000000 autotraders-1.4.2/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 02:54:04.000000 autotraders-1.4.2/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-07 02:53:48.000000 autotraders-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 02:54:04.384961 autotraders-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:54:04.384961 autotraders-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-07 02:53:48.000000 autotraders-1.4.2/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-07 02:53:48.000000 autotraders-1.4.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-07 02:53:48.000000 autotraders-1.4.2/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 02:53:48.000000 autotraders-1.4.2/tests/test_util.py
```

### Comparing `autotraders-1.4.1/LICENSE` & `autotraders-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/PKG-INFO` & `autotraders-1.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.4.1
+Version: 1.4.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.4.1/README.md` & `autotraders-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/agent.py` & `autotraders-1.4.2/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/faction/__init__.py` & `autotraders-1.4.2/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/faction/contract.py` & `autotraders-1.4.2/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/map/system.py` & `autotraders-1.4.2/autotraders/map/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
                 session.base_url
                 + "systems?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()["data"]
+            if "error" in j:
+                raise IOError(j["error"]["message"])
             systems = []
             for system in j:
                 s = System(system["symbol"], session, system)
                 systems.append(s)
             return systems, r.json()["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.4.1/autotraders/map/waypoint.py` & `autotraders-1.4.2/autotraders/map/waypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,26 +44,28 @@
             len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
         )
         self.shipyard = (
             len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
         )
 
     @staticmethod
-    def all(session, page: int = 1) -> PaginatedList:
+    def all(session, system_symbol, page: int = 1) -> PaginatedList:
         def paginated_func(p, num_per_page):
             r = session.get(
                 session.base_url
-                + "systems/waypoints?limit="
+                + "systems/" + system_symbol + "/waypoints?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
-            data = r.json()["data"]
+            j = r.json()
+            if "error" in j:
+                raise IOError(j["error"]["message"])
             waypoints = []
-            for w in data:
+            for w in j["data"]:
                 waypoint = Waypoint(w["symbol"], session, w)
                 waypoints.append(waypoint)
 
         return PaginatedList(paginated_func, page)
 
     def __eq__(self, other):
         return self.symbol == other.symbol
```

### Comparing `autotraders-1.4.1/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.4.2/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.4.2/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.4.2/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.4.2/autotraders/map/waypoint_types/shipyard.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,8 +38,10 @@
                 self.ships.append(ShipyardShip(ship))
 
     def purchase(self, ship_type: str):
         j = self.session.post(
             self.session.base_url + "my/ships",
             data={"shipType": ship_type, "waypointSymbol": self.location},
         ).json()
-        return Ship(j["data"]["ship"], self.session), ShipyardTransaction(j["data"]["transaction"])
+        return Ship(j["data"]["ship"], self.session), ShipyardTransaction(
+            j["data"]["transaction"]
+        )
```

### Comparing `autotraders-1.4.1/autotraders/paginated_list.py` & `autotraders-1.4.2/autotraders/paginated_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import math
 
 
 class PaginatedList:
     def __init__(self, func, page, num_per_page=20):
         """
         A paginated list with caching
-        :param func: Function to get page (must accept two ints denoting the page number and number of items per page and should return the data and total number of items)
+        :param func: Function to get page (must accept two ints denoting the page number and number of items per page
+        and should return the data and total number of items)
         :param page: Page to start on
         :param num_per_page: How many items per a page
         """
         self.page = page
         self.func = func
         self.num_per_page = num_per_page
         data, total = self.func(self.page, self.num_per_page)
         self.inner = {self.page: data}
         self.total = total
         self.pages = math.ceil(self.total // self.num_per_page)
 
+    def clear_cache(self):
+        self.inner = {}
+
     def next(self):
         self.page += 1
         return self.current()
 
     def prev(self):
         self.page -= 1
         return self.current()
```

### Comparing `autotraders-1.4.1/autotraders/session.py` & `autotraders-1.4.2/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/shared_models/map_symbol.py` & `autotraders-1.4.2/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/shared_models/transaction.py` & `autotraders-1.4.2/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/ship/__init__.py` & `autotraders-1.4.2/autotraders/ship/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import asyncio
-from datetime import datetime, timezone
 from typing import Union, Optional
 
 from autotraders.paginated_list import PaginatedList
 from autotraders.shared_models.item import Item
 from autotraders.shared_models.transaction import MarketTransaction
+from autotraders.ship.cargo import Cargo
+from autotraders.ship.nav import Nav
+from autotraders.ship.nav import Nav
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.map.system import System
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.ship.ship_components import Frame, Reactor, Engine, Module, Mount
 from autotraders.ship.survey import Survey
 from autotraders.util import parse_time
@@ -20,45 +22,14 @@
         self.current = current
         self.total = total
 
     def __str__(self):
         return str(self.current) + "/" + str(self.total)
 
 
-class Cargo:
-    def __init__(self, j):
-        self.capacity = j["capacity"]
-        inventory = j["inventory"]
-        self.inventory = []
-        self.current = 0
-        for symbol in inventory:
-            self.inventory.append(
-                Item(symbol["symbol"], symbol["units"], symbol["description"])
-            )
-            self.current += symbol["units"]
-
-
-class Route:
-    def __init__(self, data):
-        self.destination = MapSymbol(data["destination"]["symbol"])
-        self.departure = MapSymbol(data["departure"]["symbol"])
-        self.departure_time = parse_time(data["departureTime"])
-        self.arrival = parse_time(data["arrival"])
-        self.moving = self.arrival > datetime.now(timezone.utc)
-
-
-class Nav:
-    def __init__(self, data):
-        self.status = data["status"]
-        self.location = MapSymbol(data["waypointSymbol"])
-        self.flight_mode = data["flightMode"]
-        self.route = Route(data["route"])
-        self.moving = self.route.moving
-
-
 class Crew:
     def __init__(self, data):
         self.current = data["current"]
         self.required = data["required"]
         self.capacity = data["capacity"]
         self.morale = data["morale"]
         self.wages = data["wages"]
@@ -82,18 +53,15 @@
         self.engine: Optional[Engine] = None
         self.modules: Optional[list[Module]] = None
         self.mounts: Optional[list[Mount]] = None
         self.crew: Optional[Crew] = None
         self.registration: Optional[Registration] = None
         super().__init__(session, "my/ships/" + self.symbol, data)
 
-    def update(self, data: dict = None, hard=False) -> None:  # TODO: Hard is deprecated
-        """
-        :param hard: deprecated does not do anything
-        """
+    def update(self, data: dict = None) -> None:
         if data is None:
             data = self.get()["data"]
 
         if "crew" in data:
             self.crew = Crew(data["crew"])
         if "frame" in data:
             self.frame = Frame(data["frame"])
@@ -102,19 +70,19 @@
         if "engine" in data:
             self.engine = Engine(data["engine"])
         if "modules" in data:
             self.modules = [Module(d) for d in data["modules"]]
         if "mounts" in data:
             self.mounts = [Mount(d) for d in data["mounts"]]
         if "nav" in data:
-            self.nav = Nav(data["nav"])
+            self.nav = Nav(self.symbol, self.session, data["nav"])
         if "fuel" in data:
             self.fuel = Fuel(data["fuel"]["current"], data["fuel"]["capacity"])
         if "cargo" in data:
-            self.cargo = Cargo(data["cargo"])
+            self.cargo = Cargo(self.symbol, self.session, data["cargo"])
         if "registration" in data:
             self.registration = Registration(data["registration"])
 
     async def navigate_async(self, waypoint: Union[str, MapSymbol], interval=1):
         """Attempts to move ship to the provided waypoint.
         If the request succeeds, this function waits for the ship to arrive.
         :param interval: Frequency of updates in seconds (default: 1)
@@ -215,19 +183,15 @@
     def refine(self, output_symbol: str):
         j = self.post(
             "refine",
             data={"produce": output_symbol},
         )
         self.update(j["data"])
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
-        return Item(
-            j["data"]["produced"]["symbol"],
-            j["data"]["produced"]["units"],
-            None
-        )
+        return [Item(i["tradeSymbol"], i["units"], None) for i in j["data"]["produced"]]
 
     def chart(self) -> Waypoint:
         """
         Charts the current waypoint
 
         :returns: The info about the waypoint that has been charted
         """
```

### Comparing `autotraders-1.4.1/autotraders/ship/ship_components.py` & `autotraders-1.4.2/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/space_traders_entity.py` & `autotraders-1.4.2/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/status.py` & `autotraders-1.4.2/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders/util.py` & `autotraders-1.4.2/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/autotraders.egg-info/PKG-INFO` & `autotraders-1.4.2/autotraders.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.4.1
+Version: 1.4.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.4.1/autotraders.egg-info/SOURCES.txt` & `autotraders-1.4.2/autotraders.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,13 +23,15 @@
 autotraders/map/waypoint_types/marketplace.py
 autotraders/map/waypoint_types/shipyard.py
 autotraders/shared_models/item.py
 autotraders/shared_models/map_symbol.py
 autotraders/shared_models/trait.py
 autotraders/shared_models/transaction.py
 autotraders/ship/__init__.py
+autotraders/ship/cargo.py
+autotraders/ship/nav.py
 autotraders/ship/ship_components.py
 autotraders/ship/survey.py
 tests/test_contract.py
 tests/test_init.py
 tests/test_ship.py
 tests/test_util.py
```

### Comparing `autotraders-1.4.1/pyproject.toml` & `autotraders-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.4.1"
+version = "1.4.2"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.4.1/tests/test_init.py` & `autotraders-1.4.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.1/tests/test_ship.py` & `autotraders-1.4.2/tests/test_ship.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,38 +31,42 @@
     s.jettison("FUEL", 42)
 
 
 def test_ship_nav(session):
     start = datetime.now(timezone.utc) - timedelta(seconds=5)
     end = datetime.now(timezone.utc) + timedelta(seconds=5)
     n = Nav(
+        "MOCK_SHIP_SYMBOL",
+        session,
         {
             "status": "IN_TRANSIT",
             "waypointSymbol": "X1-TEST-TEST2",
             "flightMode": "CRUISE",
             "route": {
                 "destination": {"symbol": "X1-TEST-TEST2"},
                 "departure": {"symbol": "X1-TEST-TEST"},
                 "departureTime": start.strftime("%Y-%m-%dT%H:%M:%SZ"),
                 "arrival": end.strftime("%Y-%m-%dT%H:%M:%SZ"),
             },
-        }
+        },
     )
     assert n.status == "IN_TRANSIT"
     assert n.moving
     start2 = datetime.now(timezone.utc) - timedelta(seconds=10)
     end2 = datetime.now(timezone.utc) - timedelta(seconds=5)
     n2 = Nav(
+        "MOCK_SHIP_SYMBOL",
+        session,
         {
             "status": "ORBIT",
             "waypointSymbol": "X1-TEST-TEST2",
             "flightMode": "CRUISE",
             "route": {
                 "destination": {"symbol": "X1-TEST-TEST2"},
                 "departure": {"symbol": "X1-TEST-TEST"},
                 "departureTime": start2.strftime("%Y-%m-%dT%H:%M:%SZ"),
                 "arrival": end2.strftime("%Y-%m-%dT%H:%M:%SZ"),
             },
-        }
+        },
     )
     assert n2.status == "ORBIT"
     assert not n2.moving
```

### Comparing `autotraders-1.4.1/tests/test_util.py` & `autotraders-1.4.2/tests/test_util.py`

 * *Files identical despite different names*

