# Comparing `tmp/pybpsapi-1.2.1.tar.gz` & `tmp/pybpsapi-1.3.0.tar.gz`

## Comparing `pybpsapi-1.2.1.tar` & `pybpsapi-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 pybpsapi-1.2.1/CHANGELOG.MD
--rw-r--r--   0        0        0    10013 2020-02-02 00:00:00.000000 pybpsapi-1.2.1/pybpsapi.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pybpsapi-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pybpsapi-1.2.1/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pybpsapi-1.2.1/LICENSE
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pybpsapi-1.2.1/README.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pybpsapi-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pybpsapi-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/CHANGELOG.MD
+-rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/pybpsapi.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/README.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/PKG-INFO
```

### Comparing `pybpsapi-1.2.1/CHANGELOG.MD` & `pybpsapi-1.3.0/CHANGELOG.MD`

 * *Files 16% similar despite different names*

```diff
@@ -48,8 +48,19 @@
 ### Fixed
 - A bug with `CircularChecker` class where the database connection would be closed after a while and would report 20 new circulars
 - Minor improvements
 
 ## v1.2.1 - 17/1/2023
 
 ### Fixed
-- SQL syntax error
+- SQL syntax error
+
+## 1.3.0 - 07/6/2023
+
+### Added
+- Dynamic categories support
+
+### Removed
+- `cached` option in latest circular
+
+### Improved
+- `CircularChecker` class now returns a sorted dict of new circulars
```

### Comparing `pybpsapi-1.2.1/pybpsapi.py` & `pybpsapi-1.3.0/pybpsapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 
 class API:
     """Methods which communicate with the API"""
 
     def __init__(self, url="https://bpsapi.rajtech.me/v1/"):
         self.url = url
 
+        json = requests.get(self.url + "categories").json()
+        if json['http_status'] == 200:
+            self.categories = json['data']
+        else:
+            raise ConnectionError("Invalid API Response. API says there are no categories.")
+
     # /latest endpoint
-    def latest(self, category: str or int, cached: bool = False) -> dict or None:
+    def latest(self, category: str or int) -> dict or None:
         """The `/latest` endpoint returns the latest circular from a particular category"""
         if type(category) == int:
             category = int(category)
             if not 1 < category < 100:
                 raise ValueError("Invalid category Number")
 
         else:
-            if category not in ["ptm", "general", "exam"]:
+            if category not in self.categories:
                 raise ValueError("Invalid category Name")
 
         params = {'category': category}
-        endpoint = "latest" if not cached else "cached-latest"
 
-        request = requests.get(self.url + endpoint, params=params)
+        request = requests.get(self.url + "latest", params=params)
         json = request.json()
         try:
             json['http_status']
         except KeyError:
             raise ConnectionError("Invalid API Response")
         if json['http_status'] == 200:
             return json['data']
@@ -37,15 +42,15 @@
         """The `/list` endpoint returns a list of circulars from a particular category"""
         if type(category) == int:
             category = int(category)
             if not 1 < category < 100:
                 raise ValueError("Invalid category Number")
 
         else:
-            if category not in ["ptm", "general", "exam"]:
+            if category not in self.categories:
                 raise ValueError("Invalid category Name")
 
         if amount < -1:
             amount = -1
 
         params = {'category': category}
 
@@ -54,22 +59,22 @@
         try:
             json['http_status']
         except KeyError:
             raise ConnectionError("Invalid API Response")
         if json['http_status'] == 200:
             return json['data'] if amount == -1 else json['data'][:amount]
 
-    def search(self, query: str or int) -> dict or None:
+    def search(self, query: str or int, amount: int = 1) -> dict or None:
         """The `/search` endpoint lets you search for a circular by its name or ID"""
-        if type(query) == int:
+        if query.isdigit() and len(query) == 4:
             query = int(query)
         elif type(query) != str:
             raise ValueError("Invalid Query")
 
-        params = {'title': query}
+        params = {'title': query, 'amount': amount}
 
         request = requests.get(self.url + "search", params=params)
         json = request.json()
 
         try:
             json['http_status']
 
@@ -103,25 +108,31 @@
 class CircularChecker:
     def __init__(self, category, url: str = "https://bpsapi.rajtech.me/v1/", cache_method=None, debug: bool = False,
                  **kwargs):
         self.url = url
         self.category = category
         self._cache = []
 
+        json = requests.get(self.url + "categories").json()
+        if json['http_status'] == 200:
+            self.categories = json['data']
+        else:
+            raise ConnectionError("Invalid API Response. API says there are no categories.")
+
         if debug:
             self.set_cache = self._set_cache
             self.refresh_cache = self._refresh_cache
 
         if type(category) == int:
             category = int(category)
             if not 1 < category < 100:
                 raise ValueError("Invalid category Number")
 
         else:
-            if category not in ["ptm", "general", "exam"]:
+            if category not in self.categories:
                 raise ValueError("Invalid category Name")
 
         self._params = {'category': category}
         self.cache_method = cache_method
 
         if cache_method is not None:
             if cache_method == "database":
@@ -137,17 +148,23 @@
 
                 if not os.path.exists(self.db_path + f"/{self.db_name}.db"):
                     os.mkdir(self.db_path)
 
                 self._con = sqlite3.connect(self.db_path + f"/{self.db_name}.db")
                 self._cur = self._con.cursor()
 
-                self._cur.execute(f"CREATE TABLE IF NOT EXISTS {self.db_table} (title TEXT, category TEXT, data BLOB)")
-                self._cur.execute(f"INSERT INTO {self.db_table} VALUES (?, ?, ?)",
-                                  ("circular_list", self.category, pickle.dumps([])))
+                self._cur.execute(
+                    f"CREATE TABLE IF NOT EXISTS {self.db_table} (title TEXT, category TEXT, data BLOB)")
+
+                # check if the cache exists
+                self._cur.execute(f"SELECT * FROM {self.db_table} WHERE title = ? AND category = ?",
+                                  ("circular_list", self.category))
+                if self._cur.fetchone() is None:
+                    self._cur.execute(f"INSERT INTO {self.db_table} VALUES (?, ?, ?)",
+                                      ("circular_list", self.category, pickle.dumps([])))
                 self._con.commit()
 
             elif cache_method == "pickle":
                 try:
                     self.pickle_path = kwargs['pickle_path']
                     self.pickle_name = kwargs['pickle_name']
                 except KeyError:
@@ -155,34 +172,25 @@
 
                 if self.pickle_name.endswith(".pickle"):
                     self.pickle_name = self.pickle_name[:-7]
 
                 import os
                 if not os.path.exists(self.pickle_path):
                     os.mkdir(self.pickle_path)
+
                 # create a pickle file if it doesn't exist
                 if not os.path.exists(self.pickle_path + f"/{self.pickle_name}.pickle"):
                     with open(self.pickle_path + f"/{self.pickle_name}.pickle", "wb") as f:
                         pickle.dump([], f)
 
             else:
                 raise ValueError("Invalid Cache Method")
 
-    def refresh_db_con(self):
-        if not self.cache_method == "database":
-            return
-
-        import sqlite3
-
-        self._con = sqlite3.connect(self.db_path + f"/{self.db_name}.db")
-        self._cur = self._con.cursor()
-
     def get_cache(self) -> list[list]:
         if self.cache_method == "database":
-            self.refresh_db_con()
             self._cur.execute(f"SELECT * FROM {self.db_table} WHERE category = ?", (self.category,))
             res = self._cur.fetchone()
             if res is None:
                 return []
             else:
                 return pickle.loads(res[2])
 
@@ -192,15 +200,14 @@
                 return pickle.load(f)
 
         else:
             return self._cache
 
     def _set_cache(self, data, title: str = "circular_list"):
         if self.cache_method == "database":
-            self.refresh_db_con()
             self._cur.execute(f"DELETE FROM {self.db_table} WHERE category = ?", (self.category,))
             self._cur.execute(f"INSERT INTO {self.db_table} VALUES (?, ?, ?)",
                               (title, self.category, pickle.dumps(data)))
             self._con.commit()
 
         elif self.cache_method == "pickle":
             with open(self.pickle_path + f"/{self.pickle_name}.pickle", "wb") as f:
@@ -208,54 +215,65 @@
 
         else:
             self._cache = data
 
     def _refresh_cache(self):
         request = requests.get(self.url + "list", params=self._params)
         json = request.json()
-
         try:
             json['http_status']
         except KeyError:
             raise ValueError("Invalid API Response")
-
         if json['http_status'] == 200:
             self._set_cache(json['data'])
 
     def check(self) -> list[dict] or list[None]:
         return_dict = []
         old_cached = self.get_cache()
 
         if not old_cached:
             self._refresh_cache()
             return []
 
+        self._cur.execute(f"SELECT * FROM {self.db_table} WHERE category = ?", (self.category,))
+        res = self._cur.fetchone()
+        if res is None:
+            cache = []
+        else:
+            cache = pickle.loads(res[2])
+
         self._refresh_cache()
         final_dict = self.get_cache()
 
         if final_dict != old_cached:  # If the old and new dict are not the same
-
             new_circular_objects = [i for i in final_dict if i not in old_cached]
 
-            # print(f"{len(new_circular_objects)} new circular(s) found")
-
             for circular in new_circular_objects:
+                # check if they are in the database
+                if circular in cache:
+                    continue
+
                 return_dict.append(circular)
 
+            # sort the return_dict by circular id in ascending order
+            return_dict.sort(key=lambda x: x['circular_id'])
             return return_dict
 
         else:
             return []
 
 
 class CircularCheckerGroup:
-    def __init__(self, *args, debug: bool = False):
+    def __init__(self, *args, **kwargs):
         self._checkers = []
 
-        self.debug = debug
+        if kwargs.get("debug"):
+            self.debug = True
+        else:
+            self.debug = False
 
         for arg in args:
             if type(arg) != CircularChecker:
                 raise ValueError("Invalid CircularChecker Object")
             self._checkers.append(arg)
 
         if self.debug:
```

### Comparing `pybpsapi-1.2.1/.github/workflows/python-publish.yml` & `pybpsapi-1.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pybpsapi-1.2.1/LICENSE` & `pybpsapi-1.3.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 BPS Circular API
+Copyright (c) 2023 BPS Circular API
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pybpsapi-1.2.1/README.md` & `pybpsapi-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,29 @@
 
 `pybpsapi` can be installed using pip:
 
 ```bash
 pip install pybpsapi
 ```
 
+## Building
+
+To build the package, you can use the following command:
+
+```bash
+py -m build
+```
+
+And to upload, 
+
+```bash
+py -m twine upload dist/*
+```
+
+
 ## Contributing
 
 Contributions are welcome! Please feel free to open an issue or a pull request on the [GitHub repository](https://bpsapi.rajtech.me/r/python-package)
 
 
 ## Documentation
```

### Comparing `pybpsapi-1.2.1/pyproject.toml` & `pybpsapi-1.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pybpsapi"
-version = "1.2.1"
+version = "1.3.0"
 description = "This package is a Python wrapper for the BPS API. It supports all the five endpoints of the API, and also contains a good circular-checking system."
 author = "Raj Dave"
 author-email = "rajdave8002@gmail.com"
 homepage = "https://bpsapi.rajtech.me/"
 license = "MIT"
 keywords = ["bpsapi", "bps", "api", "wrapper", "python", "python3"]
 requires-python = ">=3.6"
```

### Comparing `pybpsapi-1.2.1/PKG-INFO` & `pybpsapi-1.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybpsapi
-Version: 1.2.1
+Version: 1.3.0
 Summary: This package is a Python wrapper for the BPS API. It supports all the five endpoints of the API, and also contains a good circular-checking system.
 License-Expression: MIT
 License-File: LICENSE
 Keywords: api,bps,bpsapi,python,python3,wrapper
 Requires-Python: >=3.6
 Requires-Dist: requests
 Description-Content-Type: text/markdown
@@ -28,14 +28,29 @@
 
 `pybpsapi` can be installed using pip:
 
 ```bash
 pip install pybpsapi
 ```
 
+## Building
+
+To build the package, you can use the following command:
+
+```bash
+py -m build
+```
+
+And to upload, 
+
+```bash
+py -m twine upload dist/*
+```
+
+
 ## Contributing
 
 Contributions are welcome! Please feel free to open an issue or a pull request on the [GitHub repository](https://bpsapi.rajtech.me/r/python-package)
 
 
 ## Documentation
```

