# Comparing `tmp/onecompiler-0.1.1.tar.gz` & `tmp/onecompiler-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onecompiler-0.1.1.tar", max compression
+gzip compressed data, was "onecompiler-0.1.11.tar", max compression
```

## Comparing `onecompiler-0.1.1.tar` & `onecompiler-0.1.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-06 14:12:34.685634 onecompiler-0.1.1/LICENSE
--rw-r--r--   0        0        0       37 2023-06-06 14:12:34.685634 onecompiler-0.1.1/README.md
--rw-r--r--   0        0        0      148 2023-06-07 19:21:32.574182 onecompiler-0.1.1/onecompiler/__init__.py
--rw-r--r--   0        0        0      143 2023-06-06 21:20:15.290434 onecompiler-0.1.1/onecompiler/api/__init__.py
--rw-r--r--   0        0        0      868 2023-06-06 21:19:36.366434 onecompiler-0.1.1/onecompiler/api/async_compiler.py
--rw-r--r--   0        0        0      889 2023-06-07 19:31:09.838182 onecompiler-0.1.1/onecompiler/api/compiler.py
--rw-r--r--   0        0        0      228 2023-06-06 18:35:35.538435 onecompiler-0.1.1/onecompiler/base_errors/LangNotFound.py
--rw-r--r--   0        0        0       89 2023-06-06 18:30:01.850435 onecompiler-0.1.1/onecompiler/base_errors/__init__.py
--rw-r--r--   0        0        0       90 2023-06-06 19:02:01.546434 onecompiler-0.1.1/onecompiler/base_models/__init__.py
--rw-r--r--   0        0        0      767 2023-06-07 14:46:49.652433 onecompiler-0.1.1/onecompiler/base_models/base_compiler.py
--rw-r--r--   0        0        0    41195 2023-06-07 19:28:23.186182 onecompiler-0.1.1/onecompiler/data.py
--rw-r--r--   0        0        0      175 2023-06-06 22:14:05.578435 onecompiler-0.1.1/onecompiler/pydantic_models/__init__.py
--rw-r--r--   0        0        0      602 2023-06-07 14:45:16.256433 onecompiler-0.1.1/onecompiler/pydantic_models/lang.py
--rw-r--r--   0        0        0      792 2023-06-07 19:19:53.794182 onecompiler-0.1.1/onecompiler/pydantic_models/response.py
--rw-r--r--   0        0        0       14 2023-06-06 18:12:06.070434 onecompiler-0.1.1/onecompiler/requirements.txt
--rw-r--r--   0        0        0      325 2023-06-07 19:03:20.846182 onecompiler-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 onecompiler-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 14:12:34.685634 onecompiler-0.1.11/LICENSE
+-rw-r--r--   0        0        0       37 2023-06-06 14:12:34.685634 onecompiler-0.1.11/README.md
+-rw-r--r--   0        0        0      148 2023-06-07 19:21:32.574182 onecompiler-0.1.11/onecompiler/__init__.py
+-rw-r--r--   0        0        0      143 2023-06-06 21:20:15.290434 onecompiler-0.1.11/onecompiler/api/__init__.py
+-rw-r--r--   0        0        0      868 2023-06-06 21:19:36.366434 onecompiler-0.1.11/onecompiler/api/async_compiler.py
+-rw-r--r--   0        0        0      889 2023-06-07 19:31:09.838182 onecompiler-0.1.11/onecompiler/api/compiler.py
+-rw-r--r--   0        0        0      228 2023-06-06 18:35:35.538435 onecompiler-0.1.11/onecompiler/base_errors/LangNotFound.py
+-rw-r--r--   0        0        0       89 2023-06-06 18:30:01.850435 onecompiler-0.1.11/onecompiler/base_errors/__init__.py
+-rw-r--r--   0        0        0       90 2023-06-06 19:02:01.546434 onecompiler-0.1.11/onecompiler/base_models/__init__.py
+-rw-r--r--   0        0        0      767 2023-06-07 14:46:49.652433 onecompiler-0.1.11/onecompiler/base_models/base_compiler.py
+-rw-r--r--   0        0        0    39084 2023-06-07 19:35:29.334182 onecompiler-0.1.11/onecompiler/data.py
+-rw-r--r--   0        0        0      175 2023-06-06 22:14:05.578435 onecompiler-0.1.11/onecompiler/pydantic_models/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-07 14:45:16.256433 onecompiler-0.1.11/onecompiler/pydantic_models/lang.py
+-rw-r--r--   0        0        0      792 2023-06-07 19:19:53.794182 onecompiler-0.1.11/onecompiler/pydantic_models/response.py
+-rw-r--r--   0        0        0       14 2023-06-06 18:12:06.070434 onecompiler-0.1.11/onecompiler/requirements.txt
+-rw-r--r--   0        0        0      326 2023-06-07 19:36:18.218182 onecompiler-0.1.11/pyproject.toml
+-rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 onecompiler-0.1.11/PKG-INFO
```

### Comparing `onecompiler-0.1.1/LICENSE` & `onecompiler-0.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `onecompiler-0.1.1/onecompiler/api/async_compiler.py` & `onecompiler-0.1.11/onecompiler/api/async_compiler.py`

 * *Files identical despite different names*

### Comparing `onecompiler-0.1.1/onecompiler/api/compiler.py` & `onecompiler-0.1.11/onecompiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `onecompiler-0.1.1/onecompiler/base_models/base_compiler.py` & `onecompiler-0.1.11/onecompiler/base_models/base_compiler.py`

 * *Files identical despite different names*

### Comparing `onecompiler-0.1.1/onecompiler/data.py` & `onecompiler-0.1.11/onecompiler/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1014,15 +1014,15 @@
                 "language": "postgresql",
                 "docs": false,
                 "tutorials": false,
                 "cheatsheets": false,
                 "files": [
                 {
                     "name": "commands.sql",
-                    "content": "\n-- create\nCREATE TABLE EMPLOYEE (\n  empId INTEGER PRIMARY KEY,\n  name TEXT NOT NULL,\n  dept TEXT NOT NULL\n);\n\n-- insert\nINSERT INTO EMPLOYEE VALUES (0001, 'Clark', 'Sales');\nINSERT INTO EMPLOYEE VALUES (0002, 'Dave', 'Accounting');\nINSERT INTO EMPLOYEE VALUES (0003, 'Ava', 'Sales');\n\n-- fetch \nSELECT * FROM EMPLOYEE WHERE dept = 'Sales';\n"
+                    "content": "{code}"
                 }
                 ]
             },
             "visibility": "public"
             },
         "redis": {
             "name": "Redis",
@@ -1036,15 +1036,15 @@
                 "language": "redis",
                 "docs": true,
                 "tutorials": false,
                 "cheatsheets": false,
                 "files": [
                 {
                     "name": "commands.redis",
-                    "content": "lpush k1 v1\nlpush k1 v2\nlpop k1"
+                    "content": "{code}"
                 }
                 ]
             },
             "visibility": "public"
             },
         "mysql": {
             "name": "MySQL",
@@ -1058,24 +1058,17 @@
                 "language": "mysql",
                 "docs": false,
                 "tutorials": false,
                 "cheatsheets": false,
                 "files": [
                 {
                     "name": "queries.sql",
-                    "content": "\n-- create\nCREATE TABLE EMPLOYEE (\n  empId INTEGER PRIMARY KEY,\n  name TEXT NOT NULL,\n  dept TEXT NOT NULL\n);\n\n-- insert\nINSERT INTO EMPLOYEE VALUES (0001, 'Clark', 'Sales');\nINSERT INTO EMPLOYEE VALUES (0002, 'Dave', 'Accounting');\nINSERT INTO EMPLOYEE VALUES (0003, 'Ava', 'Sales');\n\n-- fetch \nSELECT * FROM EMPLOYEE WHERE dept = 'Sales';\n"
+                    "content": "{code}"
                 }
                 ],
-                "newFileOptions": [
-                {
-                    "helpText": "Add init schema",
-                    "name": "init.sql",
-                    "content": "CREATE TABLE continents (\n    id INT AUTO_INCREMENT PRIMARY KEY,\n    name VARCHAR(50) NOT NULL\n);\n\nINSERT INTO continents (name) VALUES\n('Africa'),\n('Antarctica'),\n('Asia'),\n('Europe'),\n('North America'),\n('South America'),\n('Australia');"
-                }
-                ]
             },
             "visibility": "public"
             },
         "mongo": {
             "name": "MongoDB",
             "title": "MongoDB",
             "mode": "javascript",
@@ -1087,15 +1080,15 @@
                 "language": "mongodb",
                 "docs": false,
                 "tutorials": false,
                 "cheatsheets": false,
                 "files": [
                 {
                     "name": "script.js",
-                    "content": "\ndb.employees.insertMany([\n  {empId: 1, name: 'Clark', dept: 'Sales' },\n  {empId: 2, name: 'Dave', dept: 'Accounting' },\n  {empId: 3, name: 'Ava', dept: 'Sales' }\n]);\n\ndb.employees.find({dept: 'Sales'});"
+                    "content": "{code}"
                 }
                 ]
             },
             "visibility": "public"
             },
         "maria": {
             "name": "MariaDB",
@@ -1109,15 +1102,15 @@
                 "language": "mariadb",
                 "docs": true,
                 "tutorials": false,
                 "cheatsheets": false,
                 "files": [
                 {
                     "name": "commands.sql",
-                    "content": "\n-- create\nCREATE TABLE EMPLOYEE (\n  empId INTEGER PRIMARY KEY,\n  name TEXT NOT NULL,\n  dept TEXT NOT NULL\n);\n\n-- insert\nINSERT INTO EMPLOYEE VALUES (0001, 'Clark', 'Sales');\nINSERT INTO EMPLOYEE VALUES (0002, 'Dave', 'Accounting');\nINSERT INTO EMPLOYEE VALUES (0003, 'Ava', 'Sales');\n\n-- fetch \nSELECT * FROM EMPLOYEE WHERE dept = 'Sales';\n"
+                    "content": "{code}"
                 }
                 ]
             },
             "visibility": "public"
             },
         "ms_sql":{
             "name": "Microsoft SQL Server",
@@ -1131,15 +1124,15 @@
                 "language": "sqlserver",
                 "docs": false,
                 "tutorials": false,
                 "cheatsheets": false,
                 "files": [
                 {
                     "name": "queries.sql",
-                    "content": "\n-- create\nCREATE TABLE EMPLOYEE (\n  empId int,\n  name varchar(100),\n  dept varchar(50)\n);\n\n-- insert\nINSERT INTO EMPLOYEE(empId,name,dept) VALUES (0001, 'Clark', 'Sales');\nINSERT INTO EMPLOYEE(empId,name,dept) VALUES (0002, 'Dave', 'Accounting');\nINSERT INTO EMPLOYEE(empId,name,dept) VALUES (0003, 'Ava', 'Sales');\n\n-- fetch \nSELECT * FROM EMPLOYEE;\nGO\n"
+                    "content": "{code}"
                 }
                 ]
             },
             "concurrentJobs": 5,
             "visibility": "public"
             }
 	}
```

### Comparing `onecompiler-0.1.1/onecompiler/pydantic_models/lang.py` & `onecompiler-0.1.11/onecompiler/pydantic_models/lang.py`

 * *Files identical despite different names*

### Comparing `onecompiler-0.1.1/onecompiler/pydantic_models/response.py` & `onecompiler-0.1.11/onecompiler/pydantic_models/response.py`

 * *Files identical despite different names*

### Comparing `onecompiler-0.1.1/PKG-INFO` & `onecompiler-0.1.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onecompiler
-Version: 0.1.1
+Version: 0.1.11
 Summary: 
 License: Apache
 Author: pokedim13
 Author-email: skinxedovich@vk.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

