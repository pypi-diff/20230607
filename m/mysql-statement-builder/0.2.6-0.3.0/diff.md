# Comparing `tmp/mysql-statement-builder-0.2.6.tar.gz` & `tmp/mysql-statement-builder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-statement-builder-0.2.6.tar", last modified: Wed May 24 19:14:12 2023, max compression
+gzip compressed data, was "mysql-statement-builder-0.3.0.tar", last modified: Wed Jun  7 11:17:57 2023, max compression
```

## Comparing `mysql-statement-builder-0.2.6.tar` & `mysql-statement-builder-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 19:14:12.317532 mysql-statement-builder-0.2.6/
--rw-rw-rw-   0        0        0     1101 2023-05-23 08:20:23.000000 mysql-statement-builder-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     2169 2023-05-24 19:14:12.317532 mysql-statement-builder-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-05-23 10:36:35.000000 mysql-statement-builder-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 19:14:12.304540 mysql-statement-builder-0.2.6/mysql_statement_builder.egg-info/
--rw-rw-rw-   0        0        0     2169 2023-05-24 19:14:12.000000 mysql-statement-builder-0.2.6/mysql_statement_builder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-24 19:14:12.000000 mysql-statement-builder-0.2.6/mysql_statement_builder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 19:14:12.000000 mysql-statement-builder-0.2.6/mysql_statement_builder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-24 19:14:12.000000 mysql-statement-builder-0.2.6/mysql_statement_builder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-24 19:14:12.000000 mysql-statement-builder-0.2.6/mysql_statement_builder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 19:14:12.312531 mysql-statement-builder-0.2.6/mysqlsb/
--rw-rw-rw-   0        0        0      188 2023-05-23 10:41:12.000000 mysql-statement-builder-0.2.6/mysqlsb/__init__.py
--rw-rw-rw-   0        0        0     7560 2023-05-23 09:07:28.000000 mysql-statement-builder-0.2.6/mysqlsb/builder.py
--rw-rw-rw-   0        0        0      219 2023-05-23 07:45:37.000000 mysql-statement-builder-0.2.6/mysqlsb/configuration.py
--rw-rw-rw-   0        0        0      112 2023-05-24 19:02:23.000000 mysql-statement-builder-0.2.6/mysqlsb/exceptions.py
--rw-rw-rw-   0        0        0     2259 2023-05-23 08:48:54.000000 mysql-statement-builder-0.2.6/mysqlsb/statements.py
--rw-rw-rw-   0        0        0     1532 2023-05-24 19:13:53.000000 mysql-statement-builder-0.2.6/mysqlsb/utils.py
--rw-rw-rw-   0        0        0       42 2023-05-24 19:14:12.318532 mysql-statement-builder-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      949 2023-05-24 19:14:07.000000 mysql-statement-builder-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:14:12.315532 mysql-statement-builder-0.2.6/tests/
--rw-rw-rw-   0        0        0        0 2023-05-23 07:33:30.000000 mysql-statement-builder-0.2.6/tests/__init__.py
--rw-rw-rw-   0        0        0      491 2023-05-23 08:55:28.000000 mysql-statement-builder-0.2.6/tests/test_builder.py
--rw-rw-rw-   0        0        0      506 2023-05-23 08:49:25.000000 mysql-statement-builder-0.2.6/tests/test_statements.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:17:57.967166 mysql-statement-builder-0.3.0/
+-rw-rw-rw-   0        0        0     1101 2023-05-23 08:20:23.000000 mysql-statement-builder-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2169 2023-06-07 11:17:57.966165 mysql-statement-builder-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2023-05-23 10:36:35.000000 mysql-statement-builder-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 11:17:57.911256 mysql-statement-builder-0.3.0/mysql_statement_builder.egg-info/
+-rw-rw-rw-   0        0        0     2169 2023-06-07 11:17:57.000000 mysql-statement-builder-0.3.0/mysql_statement_builder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-07 11:17:57.000000 mysql-statement-builder-0.3.0/mysql_statement_builder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 11:17:57.000000 mysql-statement-builder-0.3.0/mysql_statement_builder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-07 11:17:57.000000 mysql-statement-builder-0.3.0/mysql_statement_builder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 11:17:57.000000 mysql-statement-builder-0.3.0/mysql_statement_builder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 11:17:57.957168 mysql-statement-builder-0.3.0/mysqlsb/
+-rw-rw-rw-   0        0        0      188 2023-05-23 10:41:12.000000 mysql-statement-builder-0.3.0/mysqlsb/__init__.py
+-rw-rw-rw-   0        0        0     8089 2023-06-07 11:11:33.000000 mysql-statement-builder-0.3.0/mysqlsb/builder.py
+-rw-rw-rw-   0        0        0      219 2023-05-23 07:45:37.000000 mysql-statement-builder-0.3.0/mysqlsb/configuration.py
+-rw-rw-rw-   0        0        0      112 2023-05-24 19:02:23.000000 mysql-statement-builder-0.3.0/mysqlsb/exceptions.py
+-rw-rw-rw-   0        0        0     2327 2023-06-07 10:53:02.000000 mysql-statement-builder-0.3.0/mysqlsb/statements.py
+-rw-rw-rw-   0        0        0     1532 2023-05-24 19:13:53.000000 mysql-statement-builder-0.3.0/mysqlsb/utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-07 11:17:57.967166 mysql-statement-builder-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      949 2023-06-07 11:17:52.000000 mysql-statement-builder-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:17:57.963193 mysql-statement-builder-0.3.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-23 07:33:30.000000 mysql-statement-builder-0.3.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1321 2023-06-07 11:17:36.000000 mysql-statement-builder-0.3.0/tests/test_builder.py
+-rw-rw-rw-   0        0        0      620 2023-06-07 10:53:06.000000 mysql-statement-builder-0.3.0/tests/test_statements.py
```

### Comparing `mysql-statement-builder-0.2.6/LICENSE` & `mysql-statement-builder-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.6/PKG-INFO` & `mysql-statement-builder-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-statement-builder
-Version: 0.2.6
+Version: 0.3.0
 Summary: Simplifies writing MySQL statements in non-ORM environments.
 Home-page: https://github.com/johnmartins/mysql-statement-builder
 Author: Julian Martinsson Bonde
 Author-email: julianm@chalmers.se
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mysql-statement-builder-0.2.6/README.md` & `mysql-statement-builder-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.6/mysql_statement_builder.egg-info/PKG-INFO` & `mysql-statement-builder-0.3.0/mysql_statement_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-statement-builder
-Version: 0.2.6
+Version: 0.3.0
 Summary: Simplifies writing MySQL statements in non-ORM environments.
 Home-page: https://github.com/johnmartins/mysql-statement-builder
 Author: Julian Martinsson Bonde
 Author-email: julianm@chalmers.se
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mysql-statement-builder-0.2.6/mysqlsb/builder.py` & `mysql-statement-builder-0.3.0/mysqlsb/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Union
 from enum import Enum
 
 from mysqlsb.exceptions import InvalidStatementConfiguration
 from mysqlsb.configuration import Configuration as Cnf
 import mysqlsb.statements as stmnt
 
 
@@ -36,17 +36,28 @@
         :param table:
         :param columns:
         :return:
         """
         self.query += stmnt.create_insert_statement(table, columns)
         return self
 
-    def set_values(self, values: List[str]):
-        self.query += stmnt.create_prepared_values_statement(len(values))
-        self.values.extend(values)
+    def set_values(self, values: List):
+        """
+        :param values: A list of values of type str, bool, int or float.
+        For multiple insertions, nest lists inside the list. E.g., List[List[int]].
+        :return: SQL VALUES statement string, example: "VALUES (1,2,3), ('a','b', 'c') "
+        """
+        if isinstance(values[0], list):
+            self.query += stmnt.create_prepared_values_statement(len(values[0]), times=len(values))
+            for val_array in values:
+                self.values.extend(val_array)
+        else:
+            self.query += stmnt.create_prepared_values_statement(len(values))
+            self.values.extend(values)
+
         return self
 
     def select(self, table: str, columns: List[str]):
         """
         Create a select statement
 
         :param table:
```

### Comparing `mysql-statement-builder-0.2.6/mysqlsb/statements.py` & `mysql-statement-builder-0.3.0/mysqlsb/statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,19 @@
     return f"DELETE FROM {table} "
 
 
 def create_update_statement(table: str, set_statement: str):
     return f"UPDATE {table} SET {set_statement} "
 
 
-def create_prepared_values_statement(count: int):
+def create_prepared_values_statement(count: int, times=1):
     placeholder_array = ['%s'] * count
     placeholder_str = ', '.join(placeholder_array)
-    return f"VALUES ({placeholder_str}) "
+    placeholders = [f'({placeholder_str})'] * times
+    return f"VALUES {', '.join(placeholders)} "
 
 
 def create_prepared_where_statement(condition):
     return f"WHERE {condition} "
 
 
 def create_limit_statement(n):
```

### Comparing `mysql-statement-builder-0.2.6/mysqlsb/utils.py` & `mysql-statement-builder-0.3.0/mysqlsb/utils.py`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.6/setup.py` & `mysql-statement-builder-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.6'
+VERSION = '0.3.0'
 DESCRIPTION = 'Simplifies writing MySQL statements in non-ORM environments.'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='mysql-statement-builder',
```

