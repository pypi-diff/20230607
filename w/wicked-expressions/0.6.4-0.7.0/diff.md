# Comparing `tmp/wicked_expressions-0.6.4.tar.gz` & `tmp/wicked_expressions-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicked_expressions-0.6.4.tar", max compression
+gzip compressed data, was "wicked_expressions-0.7.0.tar", max compression
```

## Comparing `wicked_expressions-0.6.4.tar` & `wicked_expressions-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1061 2023-05-31 23:05:29.547076 wicked_expressions-0.6.4/LICENSE
--rw-r--r--   0        0        0     2119 2023-05-31 23:05:29.547076 wicked_expressions-0.6.4/README.md
--rw-r--r--   0        0        0     1219 2023-05-31 23:07:27.083832 wicked_expressions-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      321 2023-05-31 23:07:27.055832 wicked_expressions-0.6.4/wicked_expressions/__init__.py
--rw-r--r--   0        0        0      709 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/api.bolt
--rw-r--r--   0        0        0     9403 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/comparison.bolt
--rw-r--r--   0        0        0      305 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/config.bolt
--rw-r--r--   0        0        0     1850 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/internal_api.bolt
--rw-r--r--   0        0        0      341 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/nbtlib.bolt
--rw-r--r--   0        0        0     8436 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/raw_operations.bolt
--rw-r--r--   0        0        0      375 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/rebindable.bolt
--rw-r--r--   0        0        0      596 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/safe_load.bolt
--rw-r--r--   0        0        0     3118 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/sources.bolt
--rw-r--r--   0        0        0     1181 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/utils.bolt
--rw-r--r--   0        0        0     1221 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/var.bolt
--rw-r--r--   0        0        0     6215 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/modules/var_sources.bolt
--rw-r--r--   0        0        0        0 2023-05-31 23:05:29.559076 wicked_expressions-0.6.4/wicked_expressions/py.typed
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 22:52:39.484761 wicked_expressions-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2119 2023-06-06 22:52:39.484761 wicked_expressions-0.7.0/README.md
+-rw-r--r--   0        0        0     1219 2023-06-06 22:54:04.418242 wicked_expressions-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-06-06 22:54:04.398242 wicked_expressions-0.7.0/wicked_expressions/__init__.py
+-rw-r--r--   0        0        0      714 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/api.bolt
+-rw-r--r--   0        0        0     9403 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/comparison.bolt
+-rw-r--r--   0        0        0      305 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/config.bolt
+-rw-r--r--   0        0        0     1850 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/internal_api.bolt
+-rw-r--r--   0        0        0      360 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/nbtlib.bolt
+-rw-r--r--   0        0        0     8436 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/raw_operations.bolt
+-rw-r--r--   0        0        0      375 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/rebindable.bolt
+-rw-r--r--   0        0        0      596 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/safe_load.bolt
+-rw-r--r--   0        0        0     3118 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/sources.bolt
+-rw-r--r--   0        0        0     1181 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/utils.bolt
+-rw-r--r--   0        0        0     1333 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/var.bolt
+-rw-r--r--   0        0        0     6303 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/var_sources.bolt
+-rw-r--r--   0        0        0        0 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/py.typed
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.7.0/PKG-INFO
```

### Comparing `wicked_expressions-0.6.4/LICENSE` & `wicked_expressions-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.4/README.md` & `wicked_expressions-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.4/pyproject.toml` & `wicked_expressions-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wicked_expressions"
-version = "0.6.4"
+version = "0.7.0"
 description = "Extension of bolt-expressions written in Bolt."
 authors = ["Yeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/wicked-expressions"
 readme = "README.md"
```

### Comparing `wicked_expressions-0.6.4/wicked_expressions/modules/api.bolt` & `wicked_expressions-0.7.0/wicked_expressions/modules/api.bolt`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from bolt_expressions.node import ExpressionNode
 from bolt_expressions import Expression
 
 from ./sources import ScoreSource, DataSource
 from ./comparison import ExpressionComparison
 from ./raw_operations import StoreExpressionValue, GetExpressionValue
 from ./var import Var, StaticVar
-from ./nbtlib import Bool, Byte, Short, Int, Long, Float, Double, String, List
+from ./nbtlib import Any, Bool, Byte, Short, Int, Long, Float, Double, String, List
 # from ./datastash import DataStash
 from ./rebindable import Rebindable
 
 import ./internal_api as internal_api
 
 
 Scoreboard = ctx.inject(internal_api.Scoreboard)
```

### Comparing `wicked_expressions-0.6.4/wicked_expressions/modules/comparison.bolt` & `wicked_expressions-0.7.0/wicked_expressions/modules/comparison.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.4/wicked_expressions/modules/internal_api.bolt` & `wicked_expressions-0.7.0/wicked_expressions/modules/internal_api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.4/wicked_expressions/modules/raw_operations.bolt` & `wicked_expressions-0.7.0/wicked_expressions/modules/raw_operations.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.4/wicked_expressions/modules/safe_load.bolt` & `wicked_expressions-0.7.0/wicked_expressions/modules/safe_load.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.4/wicked_expressions/modules/sources.bolt` & `wicked_expressions-0.7.0/wicked_expressions/modules/sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.4/wicked_expressions/modules/utils.bolt` & `wicked_expressions-0.7.0/wicked_expressions/modules/utils.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.4/wicked_expressions/modules/var.bolt` & `wicked_expressions-0.7.0/wicked_expressions/modules/var.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import ./var_sources as sources
-from ./nbtlib import Bool, Byte, Short, Int, Long, Float, Double, String, List
+from ./nbtlib import Bool, Byte, Short, Int, Long, Float, Double, String, List, Any
 
 
 class Var:
     is_static = False
 
     def __new__(self, type_annotation):
-        if type_annotation == Bool: 
+        if type_annotation == Any:
+            return sources.AnySource.create(is_static=self.is_static)
+        elif type_annotation == Bool: 
             return sources.BoolSource.create(is_static=self.is_static)
         elif type_annotation == Byte:
             return sources.ByteSource.create(is_static=self.is_static)
         elif type_annotation == Short:
             return sources.ShortSource.create(is_static=self.is_static)
         elif type_annotation == Int:
             return sources.IntSource.create(is_static=self.is_static)
```

### Comparing `wicked_expressions-0.6.4/wicked_expressions/modules/var_sources.bolt` & `wicked_expressions-0.7.0/wicked_expressions/modules/var_sources.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,19 @@
 
     #         for n in range(slot_block_size):
     #             slot_block.append(cls._default_slot_value)
 
     #         with safe_load(f"flush_variable/{cls._var_type}", append=True):
     #             data modify storage Config.STORAGE_ROOT full_location append value slot_block
 
+
+class AnySource(VarStorageSource):
+    _var_type = 'any'
+    _default_slot_value = {}
+
 class BoolSource(VarScoreSource):
     _var_type = 'bool'
 
     def _rebind(self, score, value):
         if not isinstance(value, ExpressionNode):
             value = int(value)
```

### Comparing `wicked_expressions-0.6.4/PKG-INFO` & `wicked_expressions-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicked-expressions
-Version: 0.6.4
+Version: 0.7.0
 Summary: Extension of bolt-expressions written in Bolt.
 Home-page: https://github.com/reapermc/wicked-expressions
 License: MIT
 Keywords: beet,bolt,minecraft,minecraft-commands,mcfunction
 Author: Yeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

