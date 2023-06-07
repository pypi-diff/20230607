# Comparing `tmp/mysqlx-1.1.8.tar.gz` & `tmp/mysqlx-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.1.8.tar", last modified: Tue Jun  6 12:34:29 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.1.9.tar", last modified: Wed Jun  7 04:22:04 2023, max compression
```

## Comparing `mysqlx-1.1.8.tar` & `mysqlx-1.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 12:34:29.000000 mysqlx-1.1.8/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.1.8/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx/
--rw-rw-rw-   0        0        0     4695 2023-06-06 01:46:24.000000 mysqlx-1.1.8/mysqlx/coder.py
--rw-rw-rw-   0        0        0    10185 2023-06-06 12:23:19.000000 mysqlx-1.1.8/mysqlx/db.py
--rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.1.8/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     5285 2023-06-06 08:02:21.000000 mysqlx-1.1.8/mysqlx/helper.py
--rw-rw-rw-   0        0        0     9143 2023-06-06 12:33:16.000000 mysqlx-1.1.8/mysqlx/orm.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.1.8/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.1.8/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      404 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      297 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 12:34:29.000000 mysqlx-1.1.8/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      404 2023-06-06 12:34:29.000000 mysqlx-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2598 2023-06-06 12:09:45.000000 mysqlx-1.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 12:34:29.000000 mysqlx-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-06-06 12:33:16.000000 mysqlx-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:22:04.000000 mysqlx-1.1.9/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.1.9/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx/
+-rw-rw-rw-   0        0        0     4695 2023-06-07 02:19:08.000000 mysqlx-1.1.9/mysqlx/coder.py
+-rw-rw-rw-   0        0        0    10185 2023-06-07 02:33:53.000000 mysqlx-1.1.9/mysqlx/db.py
+-rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.1.9/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     5295 2023-06-06 23:27:22.000000 mysqlx-1.1.9/mysqlx/helper.py
+-rw-rw-rw-   0        0        0    10080 2023-06-07 04:19:02.000000 mysqlx-1.1.9/mysqlx/orm.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.1.9/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.1.9/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      404 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      297 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      404 2023-06-07 04:22:04.000000 mysqlx-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2598 2023-06-06 12:09:45.000000 mysqlx-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 04:22:04.000000 mysqlx-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-06-07 04:21:46.000000 mysqlx-1.1.9/setup.py
```

### Comparing `mysqlx-1.1.8/LICENSE` & `mysqlx-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.8/mysqlx/coder.py` & `mysqlx-1.1.9/mysqlx/coder.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.8/mysqlx/db.py` & `mysqlx-1.1.9/mysqlx/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,10 +335,10 @@
     if _SHOW_SQL:
         logging.info("Exec func '%s' \n\t\t  SQL: %s \n\t\t  ARGS: %s" % (function, sql, args))
     return sql.replace('?', '%s')
 
 
 def _insert_sql(table: str, **kwargs):
     cols, args = zip(*kwargs.items())
-    sql = 'insert into `%s` (%s) values (%s)' % (table, ','.join(['`%s`' % col for col in cols]), ','.join(['?' for i in range(len(cols))]))
+    sql = 'INSERT INTO `%s` (%s) VALUES (%s)' % (table, ','.join(['`%s`' % col for col in cols]), ','.join(['?' for i in range(len(cols))]))
     return sql, args
```

### Comparing `mysqlx-1.1.8/mysqlx/dbx.py` & `mysqlx-1.1.9/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.8/mysqlx/helper.py` & `mysqlx-1.1.9/mysqlx/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,19 +51,19 @@
 
     def is_not_init(self):
         return self.connection is None
 
     def init(self):
         self.transactions = 0
         self.connection = self.connect()
-        logging.debug('Use connection <%s>...' % hex(id(self.connection)))
+        logging.debug('Use connection <%s>...' % hex(id(self.connection._cnx)))
 
     def release(self):
         if self.connection:
-            logging.debug('Release connection <%s>...' % hex(id(self.connection)))
+            logging.debug('Release connection <%s>...' % hex(id(self.connection._cnx)))
             self.connection.close()
             self.connection = None
 
     def cursor(self):
         """
         Return cursor
         """
```

### Comparing `mysqlx-1.1.8/mysqlx/orm.py` & `mysqlx-1.1.9/mysqlx/orm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,36 @@
 from . import db
 from typing import Iterable
 from datetime import datetime
 
 PK, TABLE, UPDATE_TIME = '__pk__', '__table__', 'update_time'
+SYMBOLS = ['=', '>', '<']
+BETWEEN, LIKE, IN = 'between', 'like', 'in'
+
+
+def _get_condition_arg(k, v):
+    if not isinstance(v, str):
+        return "`%s`=?" % k, v
+    v_lower = v.lower()
+    if any([symbol in SYMBOLS for symbol in v_lower]):
+        return "`%s`%s" % (k, v), None
+    elif BETWEEN in v_lower or LIKE in v_lower or IN in v_lower:
+        return "`%s` %s" % (k, v), None
+    else:
+        return "`%s`=?" % k, v
+
+
+def _get_where_args(**kwargs):
+    where, args = '', []
+    if kwargs:
+        conditions, args = zip(*[_get_condition_arg(k, v) for k, v in kwargs.items()])
+        args = [arg for arg in args if arg is not None]
+        where = 'WHERE %s' % ' and '.join(conditions)
+
+    return where, args
 
 
 class Model:
 
     def __init__(self, id: int = None, create_by: int = None, create_time: datetime = None, update_time: datetime = None, update_by: int = None,
                  del_flag: int = None):
         self.id = id
@@ -181,32 +205,39 @@
             sql = 'UPDATE `%s` SET `del_flag`=1, `%s`=CURRENT_TIMESTAMP WHERE `%s` in (%s) limit %d' % (table, UPDATE_TIME, pk, ids_str, ids_size)
             return db.execute(sql)
         else:
             sql = 'UPDATE `%s` SET `del_flag`=1, `update_by`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s` in (%s) limit %d' % (table, UPDATE_TIME, pk, ids_str, ids_size)
             return db.do_execute(sql, update_by)
 
     @classmethod
-    def find_all(cls, *selection, limit=100):
+    def find(cls, *selection, **kwargs):
         """
         Return list(object) or empty list if no result.
         """
         pk, table = cls._get_pk_and_table(cls)
-        return [cls.dict2obj(d, cls, pk, table) for d in cls.select_all(*selection, limit=limit)]
+        return [cls.dict2obj(d, cls, pk, table) for d in cls.select(*selection, **kwargs)]
 
     @classmethod
-    def select_all(cls, *selection, limit=100):
+    def select(cls, *selection, **kwargs):
         """
         Return list(dict) or empty list if no result.
         """
+        limit = kwargs.get('limit')
+        if limit:
+            del kwargs['limit']
+        else:
+            limit = 1000
+
+        where, args = _get_where_args(**kwargs)
         pk, table = cls._get_pk_and_table(cls)
         if len(selection) == 0:
-            sql = 'SELECT * FROM `%s` limit %d' % (table, limit)
+            sql = 'SELECT * FROM `%s` %s limit %d' % (table, where, limit)
         else:
-            sql = 'SELECT %s FROM `%s` limit %d' % (','.join(['`%s`' % col for col in selection]), table, limit)
-        return db.do_select(sql)
+            sql = 'SELECT %s FROM `%s` %s limit %d' % (','.join(['`%s`' % col for col in selection]), table, where, limit)
+        return db.do_select(sql, *args)
 
     @staticmethod
     def _get_pk_and_table(cls):
         pk = cls._get_pk(cls)
         table = cls._get_table(cls)
         return pk, table
```

### Comparing `mysqlx-1.1.8/README.md` & `mysqlx-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.8/setup.py` & `mysqlx-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     packages=find_packages(),
     description="mysqlx is a simple python sql executor for MySQL like iBatis.",
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.1.8',
+    version='1.1.9',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'iBatis', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.txt'],
```

