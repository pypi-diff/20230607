# Comparing `tmp/zrouter-0.2.1.tar.gz` & `tmp/zrouter-0.3.1.tar.gz`

## Comparing `zrouter-0.2.1.tar` & `zrouter-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 zrouter-0.2.1/src/zrouter/__init__.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 zrouter-0.2.1/src/zrouter/decorator.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.2.1/src/zrouter/exception.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.2.1/LICENSE
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.2.1/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 zrouter-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 zrouter-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 zrouter-0.3.1/src/zrouter/__init__.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 zrouter-0.3.1/src/zrouter/decorator.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.3.1/src/zrouter/exception.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.3.1/LICENSE
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.3.1/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 zrouter-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 zrouter-0.3.1/PKG-INFO
```

### Comparing `zrouter-0.2.1/src/zrouter/decorator.py` & `zrouter-0.3.1/src/zrouter/decorator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import time
+from functools import wraps 
+
 
 def paginate(func):
     """数组分页"""
     def wrapper(params):
         data = func(params)
         page_size = params.get('page_size')
         page_num = params.get('page_num')
@@ -18,14 +20,15 @@
 
 
 def trans_type(type_map):
     """ 类型转化
     { 'a': 'int' }
     """
     def decorator(func):
+        @wraps(func)
         def wrapper(params, *args, **kwargs):
             params_ = {}
             for k, v in params.items():
                 if not v:
                     continue
                 if type_map.get(k) == 'int':
                     params_[k] = int(v)
@@ -37,14 +40,15 @@
 
 
 def truncate(keys):
     """ 类型转化
     ['task_id', 'instr_id']
     """
     def decorator(func):
+        @wraps(func)
         def wrapper(params, *args, **kwargs):
             params_ = {}
             for k, v in params.items():
                 if k in keys:
                     params_[k] = v
             return func(params_, *args, **kwargs)
         return wrapper
```

### Comparing `zrouter-0.2.1/LICENSE` & `zrouter-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.2.1/pyproject.toml` & `zrouter-0.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.2.1"
+version = "0.3.1"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zrouter-0.2.1/PKG-INFO` & `zrouter-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrouter
-Version: 0.2.1
+Version: 0.3.1
 Summary: zen router library
 Project-URL: Homepage, https://github.com/inspirare6/zrouter
 Project-URL: Bug Tracker, https://github.com/inspirare6/zrouter/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

