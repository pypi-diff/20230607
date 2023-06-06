# Comparing `tmp/fyCursor-0.1.0.tar.gz` & `tmp/fyCursor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyCursor-0.1.0.tar", last modified: Tue Jun  6 21:46:49 2023, max compression
+gzip compressed data, was "fyCursor-0.1.1.tar", last modified: Tue Jun  6 22:06:14 2023, max compression
```

## Comparing `fyCursor-0.1.0.tar` & `fyCursor-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:46:49.078052 fyCursor-0.1.0/
--rw-r--r--   0 danielkay   (503) staff       (20)     1067 2023-05-18 03:38:19.000000 fyCursor-0.1.0/LICENSE
--rw-r--r--   0 danielkay   (503) staff       (20)      821 2023-06-06 21:46:49.077894 fyCursor-0.1.0/PKG-INFO
--rw-r--r--   0 danielkay   (503) staff       (20)      569 2023-06-06 21:46:19.000000 fyCursor-0.1.0/README.md
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:46:49.059445 fyCursor-0.1.0/fyCursor/
--rw-r--r--   0 danielkay   (503) staff       (20)     1374 2023-06-06 21:46:36.000000 fyCursor-0.1.0/fyCursor/__init__.py
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:46:49.077500 fyCursor-0.1.0/fyCursor/core/
--rw-r--r--   0 danielkay   (503) staff       (20)      148 2023-06-06 20:42:16.000000 fyCursor-0.1.0/fyCursor/core/__init__.py
--rw-r--r--   0 danielkay   (503) staff       (20)     4342 2023-06-06 21:01:22.000000 fyCursor-0.1.0/fyCursor/core/cursor.py
--rw-r--r--   0 danielkay   (503) staff       (20)      708 2023-05-30 01:08:38.000000 fyCursor-0.1.0/fyCursor/core/fields.py
--rw-r--r--   0 danielkay   (503) staff       (20)     2269 2023-06-06 21:44:41.000000 fyCursor-0.1.0/fyCursor/core/table.py
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:46:49.062302 fyCursor-0.1.0/fyCursor.egg-info/
--rw-r--r--   0 danielkay   (503) staff       (20)      821 2023-06-06 21:46:49.000000 fyCursor-0.1.0/fyCursor.egg-info/PKG-INFO
--rw-r--r--   0 danielkay   (503) staff       (20)      272 2023-06-06 21:46:49.000000 fyCursor-0.1.0/fyCursor.egg-info/SOURCES.txt
--rw-r--r--   0 danielkay   (503) staff       (20)        1 2023-06-06 21:46:49.000000 fyCursor-0.1.0/fyCursor.egg-info/dependency_links.txt
--rw-r--r--   0 danielkay   (503) staff       (20)        9 2023-06-06 21:46:49.000000 fyCursor-0.1.0/fyCursor.egg-info/top_level.txt
--rw-r--r--   0 danielkay   (503) staff       (20)       38 2023-06-06 21:46:49.078104 fyCursor-0.1.0/setup.cfg
--rw-r--r--   0 danielkay   (503) staff       (20)      645 2023-06-06 21:46:27.000000 fyCursor-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:06:14.532587 fyCursor-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 22:06:04.000000 fyCursor-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-06 22:06:14.532587 fyCursor-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-06 22:06:04.000000 fyCursor-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:06:14.532587 fyCursor-0.1.1/fyCursor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:06:14.532587 fyCursor-0.1.1/fyCursor/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/core/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/core/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:06:14.532587 fyCursor-0.1.1/fyCursor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-06 22:06:14.000000 fyCursor-0.1.1/fyCursor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-06 22:06:14.000000 fyCursor-0.1.1/fyCursor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 22:06:14.000000 fyCursor-0.1.1/fyCursor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 22:06:14.000000 fyCursor-0.1.1/fyCursor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 22:06:14.532587 fyCursor-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-06 22:06:04.000000 fyCursor-0.1.1/setup.py
```

### Comparing `fyCursor-0.1.0/LICENSE` & `fyCursor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.0/PKG-INFO` & `fyCursor-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fyCursor-0.1.0/README.md` & `fyCursor-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.0/fyCursor/__init__.py` & `fyCursor-0.1.1/fyCursor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         database=database,
     )
     return connection.cursor(fyCursor)  # type: ignore
 
 
 __title__ = "fyCursor"
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 __author__ = "felixyeahh"
 __author_email__ = "<felixyeah@outlook.com>"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Baffu Team"
```

### Comparing `fyCursor-0.1.0/fyCursor/core/cursor.py` & `fyCursor-0.1.1/fyCursor/core/cursor.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.0/fyCursor/core/fields.py` & `fyCursor-0.1.1/fyCursor/core/fields.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,12 +16,14 @@
         self.name = name
         self.primary_key = primary_key
         self.default = default
         self.nullable = nullable
 
     def _generate_field(self) -> str:
         self._field = self.name or ''
-        self._field = " PRIMARY KEY" if self.primary_key else _pass()
-        self._field = f"DEFAULT {self.default}" if self.default else _pass()
+        self._field += " PRIMARY KEY" if self.primary_key else _pass()
+        self._field += (
+            f"DEFAULT \"{self.default}\"" if self.default else _pass()
+        )
         self._field += _pass() if self.nullable else " NOT NULL"
 
         return self._field
```

### Comparing `fyCursor-0.1.0/fyCursor/core/table.py` & `fyCursor-0.1.1/fyCursor/core/table.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.0/fyCursor.egg-info/PKG-INFO` & `fyCursor-0.1.1/fyCursor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fyCursor-0.1.0/setup.py` & `fyCursor-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 # Setting up
 setup(
     name="fyCursor",
-    version="0.1.0",
+    version="0.1.1",
     description='Simple sqlite3 cursor',
     author="felixyeahh",
     author_email="<felixyeah@outlook.com>",
     license="MIT",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
```

