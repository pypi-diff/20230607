# Comparing `tmp/syncanyserver-0.0.4.tar.gz` & `tmp/syncanyserver-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanyserver-0.0.4.tar", last modified: Fri Jun  2 10:53:32 2023, max compression
+gzip compressed data, was "syncanyserver-0.0.5.tar", last modified: Wed Jun  7 03:06:40 2023, max compression
```

## Comparing `syncanyserver-0.0.4.tar` & `syncanyserver-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:32.528340 syncanyserver-0.0.4/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1084 2023-05-04 07:22:50.000000 syncanyserver-0.0.4/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-06-02 10:53:32.529955 syncanyserver-0.0.4/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)      215 2023-05-12 08:13:41.000000 syncanyserver-0.0.4/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-06-02 10:53:32.539965 syncanyserver-0.0.4/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2010 2023-05-31 05:37:53.000000 syncanyserver-0.0.4/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:32.189211 syncanyserver-0.0.4/syncanyserver/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      105 2023-05-31 05:37:53.000000 syncanyserver-0.0.4/syncanyserver/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4121 2023-05-12 08:47:17.000000 syncanyserver-0.0.4/syncanyserver/database.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2464 2023-05-26 07:20:59.000000 syncanyserver-0.0.4/syncanyserver/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    30117 2023-06-02 04:45:20.000000 syncanyserver-0.0.4/syncanyserver/server.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1868 2023-05-12 04:09:15.000000 syncanyserver-0.0.4/syncanyserver/table.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2325 2023-05-26 07:20:59.000000 syncanyserver-0.0.4/syncanyserver/user.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-02 10:53:32.482379 syncanyserver-0.0.4/syncanyserver.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)      439 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       60 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        2 2023-05-12 09:54:27.000000 syncanyserver-0.0.4/syncanyserver.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      363 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       14 2023-06-02 10:53:31.000000 syncanyserver-0.0.4/syncanyserver.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:40.596294 syncanyserver-0.0.5/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1084 2023-05-04 07:22:50.000000 syncanyserver-0.0.5/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-06-07 03:06:40.598294 syncanyserver-0.0.5/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      215 2023-05-12 08:13:41.000000 syncanyserver-0.0.5/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-06-07 03:06:40.611296 syncanyserver-0.0.5/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2010 2023-06-04 07:31:02.000000 syncanyserver-0.0.5/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:40.189294 syncanyserver-0.0.5/syncanyserver/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      105 2023-06-04 07:31:02.000000 syncanyserver-0.0.5/syncanyserver/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4441 2023-06-05 03:47:42.000000 syncanyserver-0.0.5/syncanyserver/database.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2464 2023-05-26 07:20:59.000000 syncanyserver-0.0.5/syncanyserver/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    31186 2023-06-04 08:10:57.000000 syncanyserver-0.0.5/syncanyserver/server.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1937 2023-06-05 06:22:17.000000 syncanyserver-0.0.5/syncanyserver/table.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2799 2023-06-04 08:09:54.000000 syncanyserver-0.0.5/syncanyserver/user.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:40.540295 syncanyserver-0.0.5/syncanyserver.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-06-07 03:06:39.000000 syncanyserver-0.0.5/syncanyserver.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      439 2023-06-07 03:06:39.000000 syncanyserver-0.0.5/syncanyserver.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-06-07 03:06:39.000000 syncanyserver-0.0.5/syncanyserver.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       60 2023-06-07 03:06:39.000000 syncanyserver-0.0.5/syncanyserver.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        2 2023-05-12 09:54:27.000000 syncanyserver-0.0.5/syncanyserver.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      363 2023-06-07 03:06:39.000000 syncanyserver-0.0.5/syncanyserver.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       14 2023-06-07 03:06:39.000000 syncanyserver-0.0.5/syncanyserver.egg-info/top_level.txt
```

### Comparing `syncanyserver-0.0.4/LICENSE` & `syncanyserver-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.4/PKG-INFO` & `syncanyserver-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanyserver
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple and easy to use SQL scripts to build virtual database tables MySQL Server
 Home-page: https://github.com/snower/syncany-server
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany-server
```

### Comparing `syncanyserver-0.0.4/setup.py` & `syncanyserver-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.0.4"
+version = "0.0.5"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -34,15 +34,15 @@
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(exclude=['*tests*']),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
         "sqlglot>=11.5.5,<12",
-        "syncanysql>=0.1.6",
+        "syncanysql>=0.1.7",
         "mysql-mimic>=2.2.3"
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
         "pymysql": ['PyMySQL>=0.8.1'],
         "openpyxl": ["openpyxl>=2.5.0"],
         "postgresql": ["psycopg2>=2.8.6"],
```

### Comparing `syncanyserver-0.0.4/syncanyserver/database.py` & `syncanyserver-0.0.5/syncanyserver/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,14 +77,17 @@
                         continue
                     for tasker in executor.runners:
                         if not isinstance(tasker, QueryTasker):
                             continue
                         if ("&.--." + table_name) in tasker.config["output"]:
                             table_name = tasker.config["output"].split("&.--.")[-1].split("::")[0]
                             tables.append(Table(table_name, filename, Table.parse_schema(tasker)))
+                        elif tasker.reduce_config and ("&.--." + table_name) in tasker.reduce_config["output"]:
+                            table_name = tasker.reduce_config["output"].split("&.--.")[-1].split("::")[0]
+                            tables.append(Table(table_name, filename, Table.parse_schema(tasker)))
                         tasker.tasker.close()
                 except Exception as e:
                     get_logger().warning("load database file error %s %s", filename, str(e))
             if not tables:
                 continue
             new_databases[database_name] = Database(database_name, tables)
         databases.clear()
```

### Comparing `syncanyserver-0.0.4/syncanyserver/main.py` & `syncanyserver-0.0.5/syncanyserver/main.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.4/syncanyserver/server.py` & `syncanyserver-0.0.5/syncanyserver/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 # 2023/5/4
 # create by: snower
 
 import sys
+import os
 import time
 from collections import defaultdict
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
 from sqlglot import expressions as sqlglot_expressions
 from mysql_mimic import Session, MysqlServer
 from mysql_mimic.errors import MysqlError, ErrorCode
@@ -187,15 +188,18 @@
             return [], []
         if "performance_schema" in sql:
             return [], []
         start_time = time.time()
         try:
             self.execute_index += 1
             get_logger().info("session[%d-%d] query SQL: %s", id(self), self.execute_index, sql.replace("\n", " "))
-            return await self.loop.run_in_executor(self.thread_pool_executor, self.execute_query, expression, start_time)
+            result = await self.loop.run_in_executor(self.thread_pool_executor, self.execute_query, expression, start_time)
+            if isinstance(result, Exception):
+                raise result
+            return result
         finally:
             get_logger().info("session[%d-%d] query SQL finish %.2fms", id(self), self.execute_index,
                               (time.time() - start_time) * 1000)
 
     def execute_query(self, expression, start_time):
         executor_wait_timeout = self.variables.values.get("wait_timeout") or self.executor_wait_timeout
         if start_time + int(executor_wait_timeout) <= time.time():
@@ -216,19 +220,27 @@
                 self.execute_tables(executer_context, primary_tables, self.parse_primary_variable_sqls(expression))
             joins_tables = self.parse_join_tables(expression, defaultdict(list))
             if joins_tables:
                 self.execute_tables(executer_context, joins_tables, self.parse_joins_variable_sqls(expression))
 
             if isinstance(expression, sqlglot_expressions.Insert):
                 database_name, table_name = self.parse_insert_table(expression)
+                if self.identity_provider.is_readonly(self.username):
+                    if not self.identity_provider.has_permission(self.username, "temporary_memory_table"):
+                        raise MysqlError("no temporary_memory_table permission", code=ErrorCode.ACCESS_DENIED_ERROR)
+                    if database_name and database_name not in ("-", "--"):
+                        raise MysqlError("readonly", code=ErrorCode.ACCESS_DENIED_ERROR)
+                    if not table_name or table_name in (".txt", ".csv", ".json") or table_name.lower().startswith("file://") \
+                            or os.path.splitext(os.path.split(table_name)[-1])[-1] in (".txt", ".json", ".csv", ".xls", ".xlsx"):
+                        raise MysqlError("readonly", code=ErrorCode.ACCESS_DENIED_ERROR)
                 executer_context.execute_expression(expression)
                 if (database_name is None or database_name in self.databases) and table_name:
                     datas = executer_context.pop_memory_datas(table_name)
                     if datas:
-                        self.executer_context.memory_database[table_name] = datas
+                        self.executer_context.memory_database_collection[table_name] = datas
                 return [], []
             if isinstance(expression, sqlglot_expressions.Delete):
                 executer_context.execute_expression(expression)
                 return [], []
 
             collection_name = "__session_execute_%d_%d" % (id(self), self.execute_index)
             executer_context.execute_expression(expression, "--." + collection_name)
@@ -309,17 +321,19 @@
             self.parse_join_tables(expression.args["this"], tables)
             self.parse_join_tables(expression.args["expression"], tables)
         return tables
 
     def parse_insert_table(self, expression):
         if not isinstance(expression, sqlglot_expressions.Insert):
             return None, None
+        if isinstance(expression.args["this"], sqlglot_expressions.Schema):
+            expression = expression.args["this"]
         if isinstance(expression.args["this"], sqlglot_expressions.Table):
             table_expression = expression.args["this"]
-            return ((table_expression.args["db"].name if "db" in table_expression.args else None),
+            return ((table_expression.args["db"].name if table_expression.args.get("db") else None),
                     table_expression.args["this"].name)
         return None, None
 
     def parse_primary_variable_sqls(self, expression):
         if not isinstance(expression, sqlglot_expressions.Select):
             return defaultdict(list)
         primary_variable_sqls = defaultdict(list)
```

### Comparing `syncanyserver-0.0.4/syncanyserver/table.py` & `syncanyserver-0.0.5/syncanyserver/table.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,16 @@
         self.filename = filename
         self.schema = schema
 
     @classmethod
     def parse_schema(cls, tasker):
         schema = {}
         for name, valuer in tasker.tasker.outputer.schema.items():
+            if name == "_aggregate_key_":
+                continue
             final_filter = valuer.get_final_filter()
             if isinstance(final_filter, IntFilter):
                 schema[name] = ColumnType.LONG
             elif isinstance(final_filter, FloatFilter):
                 schema[name] = ColumnType.DOUBLE
             elif isinstance(final_filter, StringFilter):
                 schema[name] = ColumnType.VARCHAR
```

### Comparing `syncanyserver-0.0.4/syncanyserver/user.py` & `syncanyserver-0.0.5/syncanyserver/user.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,14 +33,26 @@
 
     async def get_databases(self, username):
         if self.users is None:
             self.load_users()
         user = self.users.get(username)
         return user["databases"] if user and "databases" in user else None
 
+    def is_readonly(self, username):
+        if self.users is None:
+            self.load_users()
+        user = self.users.get(username)
+        return user["readonly"] if user and "readonly" in user else True
+
+    def has_permission(self, username, permission):
+        if self.users is None:
+            self.load_users()
+        user = self.users.get(username)
+        return (permission in user["permissions"]) if user and "permissions" in user else False
+
     def load_users(self):
         users = {}
         for filename in (os.path.join(self.config_path, "user.json"), os.path.join(self.config_path, "user.yaml")):
             if not os.path.exists(filename):
                 continue
             config = load_config(filename)
             if not config or not isinstance(config, (dict, list)):
```

### Comparing `syncanyserver-0.0.4/syncanyserver.egg-info/PKG-INFO` & `syncanyserver-0.0.5/syncanyserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanyserver
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple and easy to use SQL scripts to build virtual database tables MySQL Server
 Home-page: https://github.com/snower/syncany-server
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany-server
```

