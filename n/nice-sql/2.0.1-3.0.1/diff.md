# Comparing `tmp/nice-sql-2.0.1.tar.gz` & `tmp/nice-sql-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice-sql-2.0.1.tar", last modified: Wed May 31 07:38:24 2023, max compression
+gzip compressed data, was "nice-sql-3.0.1.tar", last modified: Wed Jun  7 09:01:02 2023, max compression
```

## Comparing `nice-sql-2.0.1.tar` & `nice-sql-3.0.1.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.280526 nice-sql-2.0.1/
--rw-r--r--   0 lichengming   (502) staff       (20)     2619 2023-05-31 07:38:24.280076 nice-sql-2.0.1/PKG-INFO
--rw-r--r--   0 lichengming   (502) staff       (20)     2318 2023-05-31 07:31:09.000000 nice-sql-2.0.1/README.md
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.273349 nice-sql-2.0.1/nice_sql.egg-info/
--rw-r--r--   0 lichengming   (502) staff       (20)     2619 2023-05-31 07:38:24.000000 nice-sql-2.0.1/nice_sql.egg-info/PKG-INFO
--rw-r--r--   0 lichengming   (502) staff       (20)      496 2023-05-31 07:38:24.000000 nice-sql-2.0.1/nice_sql.egg-info/SOURCES.txt
--rw-r--r--   0 lichengming   (502) staff       (20)        1 2023-05-31 07:38:24.000000 nice-sql-2.0.1/nice_sql.egg-info/dependency_links.txt
--rw-r--r--   0 lichengming   (502) staff       (20)       44 2023-05-31 07:38:24.000000 nice-sql-2.0.1/nice_sql.egg-info/requires.txt
--rw-r--r--   0 lichengming   (502) staff       (20)        8 2023-05-31 07:38:24.000000 nice-sql-2.0.1/nice_sql.egg-info/top_level.txt
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.273721 nice-sql-2.0.1/nicesql/
--rw-r--r--   0 lichengming   (502) staff       (20)        0 2023-05-30 06:32:39.000000 nice-sql-2.0.1/nicesql/__init__.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.276084 nice-sql-2.0.1/nicesql/engine/
--rw-r--r--   0 lichengming   (502) staff       (20)      213 2023-05-30 12:32:57.000000 nice-sql-2.0.1/nicesql/engine/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)     2226 2023-05-31 02:40:04.000000 nice-sql-2.0.1/nicesql/engine/_engines.py
--rw-r--r--   0 lichengming   (502) staff       (20)      400 2023-05-31 02:47:34.000000 nice-sql-2.0.1/nicesql/engine/_execute.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1629 2023-05-30 12:29:17.000000 nice-sql-2.0.1/nicesql/engine/_register.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1128 2023-05-30 07:03:46.000000 nice-sql-2.0.1/nicesql/engine/_result.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.277086 nice-sql-2.0.1/nicesql/shortcut/
--rw-r--r--   0 lichengming   (502) staff       (20)       80 2023-05-30 08:54:09.000000 nice-sql-2.0.1/nicesql/shortcut/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)     3147 2023-05-30 08:59:16.000000 nice-sql-2.0.1/nicesql/shortcut/_shortcut.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.278066 nice-sql-2.0.1/nicesql/sqlconv/
--rw-r--r--   0 lichengming   (502) staff       (20)       50 2023-05-29 08:40:55.000000 nice-sql-2.0.1/nicesql/sqlconv/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1355 2023-05-29 11:43:20.000000 nice-sql-2.0.1/nicesql/sqlconv/_convert.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.279230 nice-sql-2.0.1/nicesql/utils/
--rw-r--r--   0 lichengming   (502) staff       (20)       54 2023-05-31 02:46:13.000000 nice-sql-2.0.1/nicesql/utils/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)      326 2023-05-23 10:10:49.000000 nice-sql-2.0.1/nicesql/utils/error.py
--rw-r--r--   0 lichengming   (502) staff       (20)       38 2023-05-31 07:38:24.280690 nice-sql-2.0.1/setup.cfg
--rw-r--r--   0 lichengming   (502) staff       (20)      749 2023-05-31 07:33:11.000000 nice-sql-2.0.1/setup.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.406733 nice-sql-3.0.1/
+-rw-r--r--   0 lichengming   (502) staff       (20)     2618 2023-06-07 09:01:02.406087 nice-sql-3.0.1/PKG-INFO
+-rw-r--r--   0 lichengming   (502) staff       (20)     2303 2023-06-07 08:10:43.000000 nice-sql-3.0.1/README.md
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.386022 nice-sql-3.0.1/nice_sql.egg-info/
+-rw-r--r--   0 lichengming   (502) staff       (20)     2618 2023-06-07 09:01:02.000000 nice-sql-3.0.1/nice_sql.egg-info/PKG-INFO
+-rw-r--r--   0 lichengming   (502) staff       (20)      629 2023-06-07 09:01:02.000000 nice-sql-3.0.1/nice_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)        1 2023-06-07 09:01:02.000000 nice-sql-3.0.1/nice_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)       53 2023-06-07 09:01:02.000000 nice-sql-3.0.1/nice_sql.egg-info/requires.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)        8 2023-06-07 09:01:02.000000 nice-sql-3.0.1/nice_sql.egg-info/top_level.txt
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.386326 nice-sql-3.0.1/nicesql/
+-rw-r--r--   0 lichengming   (502) staff       (20)        0 2023-05-31 15:43:52.000000 nice-sql-3.0.1/nicesql/__init__.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.393185 nice-sql-3.0.1/nicesql/db/
+-rw-r--r--   0 lichengming   (502) staff       (20)      167 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/db/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1175 2023-06-03 08:26:25.000000 nice-sql-3.0.1/nicesql/db/_driver.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     2091 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/db/_driver_mysql.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1868 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/db/_execute.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1527 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/db/_register.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1128 2023-05-30 07:03:46.000000 nice-sql-3.0.1/nicesql/db/_result.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1355 2023-05-29 11:43:20.000000 nice-sql-3.0.1/nicesql/db/_sqlconv.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.400848 nice-sql-3.0.1/nicesql/shortcut/
+-rw-r--r--   0 lichengming   (502) staff       (20)      215 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      841 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/_base.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      344 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/_delete.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      368 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/_insert.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      875 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/_select.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      344 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/_update.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      628 2023-06-07 06:55:37.000000 nice-sql-3.0.1/nicesql/shortcut/_utils.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.404791 nice-sql-3.0.1/nicesql/utils/
+-rw-r--r--   0 lichengming   (502) staff       (20)       74 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/utils/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)       55 2023-06-02 08:01:20.000000 nice-sql-3.0.1/nicesql/utils/_logger.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      347 2023-06-05 14:24:21.000000 nice-sql-3.0.1/nicesql/utils/_tls.py
+-rw-r--r--   0 lichengming   (502) staff       (20)       38 2023-06-07 09:01:02.406910 nice-sql-3.0.1/setup.cfg
+-rw-r--r--   0 lichengming   (502) staff       (20)      783 2023-06-07 08:05:45.000000 nice-sql-3.0.1/setup.py
```

### Comparing `nice-sql-2.0.1/PKG-INFO` & `nice-sql-3.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nice-sql
-Version: 2.0.1
-Summary: easy nice sql: decorator with sql
+Version: 3.0.1
+Summary: easy/lite/simple db query for python db api 2.0
 Home-page: https://github.com/minusli/nicesql
 Author: minusli
 Author-email: minusli@foxmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -19,29 +19,29 @@
 `pip install nice-sql==2.0.0`
 
 # 如何使用？
 
 ### Step 1: 添加 db 配置
 
 ```python
-from nicesql.engine import add_db
+from nicesql.db import add_db
 
 if __name__ == '__main__':
-    add_db("mysql://localhost:3306/test_db?user=test&password=test&charset=utf8mb4")
+    add_db("mysql://test:test@localhost:3306/test_db?charset=utf8mb4")
 ```
 
 ### step2: 执行 sql
 
 ```python
-from nicesql.shortcut import select, update, insert, delete, ddl
+from nicesql.shortcut import select, update, insert, delete, sql
 
 
 # 方式 1：直接查询
 def way1():
-    result = select("select * from t where a={a} and b in ({b})", {"a": 1, "b": ["1", "2"]}).execute()
+    result = select("select * from t where a={a} and b in ({b})", a=1, b=["1", "2"]).execute()
 
 
 # 方式 2：装饰器查询
 @select("select * from t where a={a}")
 def get(a=1):
     pass
 
@@ -63,15 +63,15 @@
     def __init__(self):
         self.id = None
         self.name = None
 
 
 if __name__ == '__main__':
     # 使用 model(T) 方法设置数据模型
-    users = select("select * from user where id in ({ids})", {"ids": [1, 2, 3]}).model(User).execute()
+    users = select("select * from user where id in ({ids})", id=[1, 2, 3]).model(User).execute()
 ```
 
 - 支持 sql 中扩展列表:
 
 ```sql
 /*
 ids 对应的传参，可以是列表，会被展开成  v1,v2,v3...
@@ -92,42 +92,42 @@
     def __init__(self):
         self.id = None
         self.name = None
 
 
 if __name__ == '__main__':
     # 使用 first(T=None) 控制只获取第一条数据, 同时也可以设置 model
-    user = select("select * from user where id={id}", {"id": 1}).first(User).execute()
+    user = select("select * from user where id={id}", id=1).first(User).execute()
 ```
 
 - 支持设置多 DB
 
 ```python
-from nicesql.engine import add_db
+from nicesql.db import add_db
 
 if __name__ == '__main__':
     # 通过设置别名参数，创建多个 db；
-    add_db("mysql://localhost:3306/test1", "db1")
-    add_db("mysql://localhost:3306/test2", "db2")
+    add_db("mysql://username:password@localhost:3306/test1", "db1")
+    add_db("mysql://username:passwprd@localhost:3306/test2", "db2")
 
     # 使用是通过 db(alias) 指定需要使用的 db 
     from nicesql.shortcut import insert
 
-    insert("insert into t(name) values({name})", {"name": "hello"}).db("db1").execute()
+    insert("insert into t(name) values({name})", name="hello").db("db1").execute()
 ```
 
 - 占位符支持递归查询，同时支持管道进行数据处理
 
 ```python
 from nicesql.shortcut import select
 
 
 class User:
     def __init__(self):
         self.id = 5
 
 
 if __name__ == '__main__':
-    select("select * from t where id={user.id|str}", {"user": User()})
+    select("select * from t where id={user.id|str}", user=User())
 ```
```

### Comparing `nice-sql-2.0.1/README.md` & `nice-sql-3.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 `pip install nice-sql==2.0.0`
 
 # 如何使用？
 
 ### Step 1: 添加 db 配置
 
 ```python
-from nicesql.engine import add_db
+from nicesql.db import add_db
 
 if __name__ == '__main__':
-    add_db("mysql://localhost:3306/test_db?user=test&password=test&charset=utf8mb4")
+    add_db("mysql://test:test@localhost:3306/test_db?charset=utf8mb4")
 ```
 
 ### step2: 执行 sql
 
 ```python
-from nicesql.shortcut import select, update, insert, delete, ddl
+from nicesql.shortcut import select, update, insert, delete, sql
 
 
 # 方式 1：直接查询
 def way1():
-    result = select("select * from t where a={a} and b in ({b})", {"a": 1, "b": ["1", "2"]}).execute()
+    result = select("select * from t where a={a} and b in ({b})", a=1, b=["1", "2"]).execute()
 
 
 # 方式 2：装饰器查询
 @select("select * from t where a={a}")
 def get(a=1):
     pass
 
@@ -51,15 +51,15 @@
     def __init__(self):
         self.id = None
         self.name = None
 
 
 if __name__ == '__main__':
     # 使用 model(T) 方法设置数据模型
-    users = select("select * from user where id in ({ids})", {"ids": [1, 2, 3]}).model(User).execute()
+    users = select("select * from user where id in ({ids})", id=[1, 2, 3]).model(User).execute()
 ```
 
 - 支持 sql 中扩展列表:
 
 ```sql
 /*
 ids 对应的传参，可以是列表，会被展开成  v1,v2,v3...
@@ -80,40 +80,40 @@
     def __init__(self):
         self.id = None
         self.name = None
 
 
 if __name__ == '__main__':
     # 使用 first(T=None) 控制只获取第一条数据, 同时也可以设置 model
-    user = select("select * from user where id={id}", {"id": 1}).first(User).execute()
+    user = select("select * from user where id={id}", id=1).first(User).execute()
 ```
 
 - 支持设置多 DB
 
 ```python
-from nicesql.engine import add_db
+from nicesql.db import add_db
 
 if __name__ == '__main__':
     # 通过设置别名参数，创建多个 db；
-    add_db("mysql://localhost:3306/test1", "db1")
-    add_db("mysql://localhost:3306/test2", "db2")
+    add_db("mysql://username:password@localhost:3306/test1", "db1")
+    add_db("mysql://username:passwprd@localhost:3306/test2", "db2")
 
     # 使用是通过 db(alias) 指定需要使用的 db 
     from nicesql.shortcut import insert
 
-    insert("insert into t(name) values({name})", {"name": "hello"}).db("db1").execute()
+    insert("insert into t(name) values({name})", name="hello").db("db1").execute()
 ```
 
 - 占位符支持递归查询，同时支持管道进行数据处理
 
 ```python
 from nicesql.shortcut import select
 
 
 class User:
     def __init__(self):
         self.id = 5
 
 
 if __name__ == '__main__':
-    select("select * from t where id={user.id|str}", {"user": User()})
+    select("select * from t where id={user.id|str}", user=User())
 ```
```

### Comparing `nice-sql-2.0.1/nice_sql.egg-info/PKG-INFO` & `nice-sql-3.0.1/nice_sql.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nice-sql
-Version: 2.0.1
-Summary: easy nice sql: decorator with sql
+Version: 3.0.1
+Summary: easy/lite/simple db query for python db api 2.0
 Home-page: https://github.com/minusli/nicesql
 Author: minusli
 Author-email: minusli@foxmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -19,29 +19,29 @@
 `pip install nice-sql==2.0.0`
 
 # 如何使用？
 
 ### Step 1: 添加 db 配置
 
 ```python
-from nicesql.engine import add_db
+from nicesql.db import add_db
 
 if __name__ == '__main__':
-    add_db("mysql://localhost:3306/test_db?user=test&password=test&charset=utf8mb4")
+    add_db("mysql://test:test@localhost:3306/test_db?charset=utf8mb4")
 ```
 
 ### step2: 执行 sql
 
 ```python
-from nicesql.shortcut import select, update, insert, delete, ddl
+from nicesql.shortcut import select, update, insert, delete, sql
 
 
 # 方式 1：直接查询
 def way1():
-    result = select("select * from t where a={a} and b in ({b})", {"a": 1, "b": ["1", "2"]}).execute()
+    result = select("select * from t where a={a} and b in ({b})", a=1, b=["1", "2"]).execute()
 
 
 # 方式 2：装饰器查询
 @select("select * from t where a={a}")
 def get(a=1):
     pass
 
@@ -63,15 +63,15 @@
     def __init__(self):
         self.id = None
         self.name = None
 
 
 if __name__ == '__main__':
     # 使用 model(T) 方法设置数据模型
-    users = select("select * from user where id in ({ids})", {"ids": [1, 2, 3]}).model(User).execute()
+    users = select("select * from user where id in ({ids})", id=[1, 2, 3]).model(User).execute()
 ```
 
 - 支持 sql 中扩展列表:
 
 ```sql
 /*
 ids 对应的传参，可以是列表，会被展开成  v1,v2,v3...
@@ -92,42 +92,42 @@
     def __init__(self):
         self.id = None
         self.name = None
 
 
 if __name__ == '__main__':
     # 使用 first(T=None) 控制只获取第一条数据, 同时也可以设置 model
-    user = select("select * from user where id={id}", {"id": 1}).first(User).execute()
+    user = select("select * from user where id={id}", id=1).first(User).execute()
 ```
 
 - 支持设置多 DB
 
 ```python
-from nicesql.engine import add_db
+from nicesql.db import add_db
 
 if __name__ == '__main__':
     # 通过设置别名参数，创建多个 db；
-    add_db("mysql://localhost:3306/test1", "db1")
-    add_db("mysql://localhost:3306/test2", "db2")
+    add_db("mysql://username:password@localhost:3306/test1", "db1")
+    add_db("mysql://username:passwprd@localhost:3306/test2", "db2")
 
     # 使用是通过 db(alias) 指定需要使用的 db 
     from nicesql.shortcut import insert
 
-    insert("insert into t(name) values({name})", {"name": "hello"}).db("db1").execute()
+    insert("insert into t(name) values({name})", name="hello").db("db1").execute()
 ```
 
 - 占位符支持递归查询，同时支持管道进行数据处理
 
 ```python
 from nicesql.shortcut import select
 
 
 class User:
     def __init__(self):
         self.id = 5
 
 
 if __name__ == '__main__':
-    select("select * from t where id={user.id|str}", {"user": User()})
+    select("select * from t where id={user.id|str}", user=User())
 ```
```

### Comparing `nice-sql-2.0.1/nicesql/engine/_result.py` & `nice-sql-3.0.1/nicesql/db/_result.py`

 * *Files identical despite different names*

### Comparing `nice-sql-2.0.1/nicesql/sqlconv/_convert.py` & `nice-sql-3.0.1/nicesql/db/_sqlconv.py`

 * *Files identical despite different names*

### Comparing `nice-sql-2.0.1/setup.py` & `nice-sql-3.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 
 # upload pypi
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
 
 setup(
     name='nice-sql',
-    version='2.0.1',
+    version='3.0.1',
     author='minusli',
     author_email='minusli@foxmail.com',
     url='https://github.com/minusli/nicesql',
-    description='easy nice sql: decorator with sql',
+    description='easy/lite/simple db query for python db api 2.0',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
     python_requires='>=3',
     install_requires=[
         "pytest",
         "pymysql",
         "DBUtils",
+        "dsnparse",
         "nice-datapath==0.0.1",
     ],
     entry_points={},
     license="Apache License 2.0"
 )
```

