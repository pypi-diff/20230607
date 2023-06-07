# Comparing `tmp/databaseRestoreIntegrity-1.0.4.tar.gz` & `tmp/databaseRestoreIntegrity-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databaseRestoreIntegrity-1.0.4.tar", last modified: Mon Jun  5 09:49:07 2023, max compression
+gzip compressed data, was "databaseRestoreIntegrity-1.0.5.tar", last modified: Wed Jun  7 15:03:06 2023, max compression
```

## Comparing `databaseRestoreIntegrity-1.0.4.tar` & `databaseRestoreIntegrity-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:49:07.879921 databaseRestoreIntegrity-1.0.4/
--rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 02:34:52.000000 databaseRestoreIntegrity-1.0.4/LICENSE.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 03:13:57.000000 databaseRestoreIntegrity-1.0.4/MANIFEST.in
--rw-r--r--   0 mhasan     (502) staff       (20)     3651 2023-06-05 09:49:07.880046 databaseRestoreIntegrity-1.0.4/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)     1959 2023-06-05 09:48:07.000000 databaseRestoreIntegrity-1.0.4/README.md
--rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 03:25:16.000000 databaseRestoreIntegrity-1.0.4/pyproject.toml
--rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-05 09:49:07.881384 databaseRestoreIntegrity-1.0.4/setup.cfg
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:49:07.866582 databaseRestoreIntegrity-1.0.4/src/
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:49:07.876012 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity/
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 03:23:11.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity/__init__.py
--rw-r--r--   0 mhasan     (502) staff       (20)     2558 2023-06-05 09:35:28.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity/mysql.py
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:49:07.879468 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/
--rw-r--r--   0 mhasan     (502) staff       (20)     3651 2023-06-05 09:49:07.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)      345 2023-06-05 09:49:07.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-05 09:49:07.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
--rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-05 09:49:07.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/top_level.txt
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-07 15:03:06.273056 databaseRestoreIntegrity-1.0.5/
+-rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.5/LICENSE.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.5/MANIFEST.in
+-rw-r--r--   0 mhasan     (502) staff       (20)     3651 2023-06-07 15:03:06.273154 databaseRestoreIntegrity-1.0.5/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)     1959 2023-06-05 09:52:54.000000 databaseRestoreIntegrity-1.0.5/README.md
+-rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.5/pyproject.toml
+-rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-07 15:03:06.278064 databaseRestoreIntegrity-1.0.5/setup.cfg
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-07 15:03:06.263358 databaseRestoreIntegrity-1.0.5/src/
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-07 15:03:06.266918 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity/
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity/__init__.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     2970 2023-06-07 12:36:19.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity/mysql.py
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-07 15:03:06.272654 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/
+-rw-r--r--   0 mhasan     (502) staff       (20)     3651 2023-06-07 15:03:06.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)      345 2023-06-07 15:03:06.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-07 15:03:06.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-07 15:03:06.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/top_level.txt
```

### Comparing `databaseRestoreIntegrity-1.0.4/LICENSE.txt` & `databaseRestoreIntegrity-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.4/PKG-INFO` & `databaseRestoreIntegrity-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `databaseRestoreIntegrity-1.0.4/README.md` & `databaseRestoreIntegrity-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.4/setup.cfg` & `databaseRestoreIntegrity-1.0.5/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = databaseRestoreIntegrity
-version = 1.0.4
+version = 1.0.5
 author = Maihraj Hasan
 author_email = maihrajhasan@gmail.com
 description = A package to check mysql restore integrity check
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity/mysql.py` & `databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity/mysql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,93 @@
 #!/usr/bin/env python3
 
 import mysql.connector
 import re
 import csv
 import os
 
-class mysqlRestroeCheck:
+class mysqlReadData:
 
     def __init__(self, host, user, password):
         self.host = host
         self.user = user
-        self.password = password 
+        self.password = password
 
     def connection(self):
         try:
             mydb = mysql.connector.connect(
                 host = self.host,
                 user = self.user,
                 password = self.password
-            )
+        )
         except:
             print(f'Connection is not successful')
-
         return mydb
 
     def _db_list(self):
         dbs = []
         sql_query = "show databases"
-        try: 
+        try:
             conn = self.connection()
-            mycursor = conn.cursor()  
+            mycursor = conn.cursor()
             mycursor.execute(sql_query)
             # mycursor.execute('show databases')
             for x in mycursor:
                 dbs.append(*x)
-        except: 
+        except:
             print(f'database list not succedd')
         return dbs
-    
-    def _table_list(self): 
+
+    def _table_list(self):
         tables_names = []
         conn = self.connection()
         dbs = self._db_list()
         for x in dbs:
             sql_query = "USE " + x
             tables = conn.cursor()
             tables.execute(sql_query)
             tables.execute("show tables")
             for t in tables:
-                tables_names.append("{}.{}".format(x, *t))
+                tables_names.append("{}.{}".format(x, *t))   
         return tables_names
 
     def _records_count(self):
         records_count = []
         conn = self.connection()
         t_name = self._table_list()
         for c in t_name:
             sql_query = "select count(*) from " + c
             r = conn.cursor()
             r.execute(sql_query)
             for count in r:
-                records_count.append("{},{}".format(c, *count))
-        return records_count
-    
-    def _create_tmp_table(self, name):
-        conn = self.connection()
+                records_count.append("{},{}".format(c, *count))  
+        return records_count   
+
+    def _create_tmp_file(self, name):
         self.name = name
         records = self._records_count()
+        f = open(self.name, 'w+')
+        for data in records:
+            sql_query = ("{}{}{}{}".format('INSERT INTO ', self.name, ' (tables_name, records_count, hostname) VALUES ', (data.split(",")[0], data.split(",")[1], self.host)))
+            f.write("{}\n".format(sql_query))
+        f.close()
+        
+    def _insert_data(self, name):
+        conn = self.connection()
+        self.name = name
         ct = conn.cursor()
         table_drop_query = ("{}{}".format('DROP TABLE IF EXISTS ', self.name))
-        ct.execute("CREATE DATABASE IF NOT EXISTS restore_consistency")
-        ct.execute("USE restore_consistency")
+        ct.execute("CREATE DATABASE IF NOT EXISTS CheckDBsTableConsistency")
+        ct.execute("USE CheckDBsTableConsistency")
         ct.execute(table_drop_query)
         ct.execute("{}{}{}".format('CREATE TABLE IF NOT EXISTS ', self.name, ' (tables_name VARCHAR(255), records_count VARCHAR(255), hostname VARCHAR(244))'))
-        for data in records:
-            sql_query = ("{}{}{}{}".format('INSERT INTO ', self.name, ' (tables_name, records_count, hostname) VALUES ', (data.split(",")[0], data.split(",")[1], self.host)))
+        f = open(self.name, 'r')
+        lines = f.readlines()
+        count = 0
+        for line in lines:
+            count += 1
+            sql_query = ("{}".format(line.strip()))
             ct.execute(sql_query)
-            conn.commit()
+            conn.commit()
+        f.close()
+        os.remove(self.name)
+        conn.close()
```

### Comparing `databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/PKG-INFO` & `databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
```

