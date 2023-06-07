# Comparing `tmp/chainingiterator-0.1.7.tar.gz` & `tmp/chainingiterator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainingiterator-0.1.7.tar", max compression
+gzip compressed data, was "chainingiterator-0.1.9.tar", max compression
```

## Comparing `chainingiterator-0.1.7.tar` & `chainingiterator-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       94 2023-03-17 12:44:12.230203 chainingiterator-0.1.7/chainingiterator/__init__.py
--rw-r--r--   0        0        0    10915 2023-03-28 10:24:05.686754 chainingiterator-0.1.7/chainingiterator/chainingiterator.py
--rw-r--r--   0        0        0     1088 2023-03-24 11:41:59.907811 chainingiterator-0.1.7/LICENSE
--rw-r--r--   0        0        0      675 2023-03-28 10:24:29.382201 chainingiterator-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      190 2023-03-24 11:41:27.511254 chainingiterator-0.1.7/README.md
--rw-r--r--   0        0        0      908 2023-03-28 10:25:00.263937 chainingiterator-0.1.7/setup.py
--rw-r--r--   0        0        0      988 2023-03-28 10:25:00.263937 chainingiterator-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-03-17 12:44:12.230203 chainingiterator-0.1.9/chainingiterator/__init__.py
+-rw-r--r--   0        0        0    11003 2023-06-07 07:42:52.876106 chainingiterator-0.1.9/chainingiterator/chainingiterator.py
+-rw-r--r--   0        0        0        0 2023-03-29 13:28:20.992175 chainingiterator-0.1.9/chainingiterator/py.typed
+-rw-r--r--   0        0        0     1088 2023-03-24 11:41:59.907811 chainingiterator-0.1.9/LICENSE
+-rw-r--r--   0        0        0      718 2023-06-07 07:29:46.152554 chainingiterator-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-03-24 11:41:27.511254 chainingiterator-0.1.9/README.md
+-rw-r--r--   0        0        0     1039 1970-01-01 00:00:00.000000 chainingiterator-0.1.9/PKG-INFO
```

### Comparing `chainingiterator-0.1.7/chainingiterator/chainingiterator.py` & `chainingiterator-0.1.9/chainingiterator/chainingiterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,17 +277,17 @@
                 else:
                     yield elem
 
         self.__consumed_guard()
         self._iter = choosy_map(self._iter, constraint, transformation)
         return self
 
-    def flatten(self) -> "ChainingIterator":
+    def flatten(self, stop_condition: Optional[Callable]=None) -> "ChainingIterator":
         def inner_flatter(target: Any) -> Iterator:
-            if not isinstance(target, Iterable):
+            if not isinstance(target, Iterable) or (stop_condition and stop_condition(target)):
                 yield target
                 return
             for sub in target:
                 yield from inner_flatter(sub)
 
         self.__consumed_guard()
         self._iter = inner_flatter(self._iter)
```

### Comparing `chainingiterator-0.1.7/LICENSE` & `chainingiterator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chainingiterator-0.1.7/pyproject.toml` & `chainingiterator-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "chainingiterator"
-version = "0.1.7"
+version = "0.1.9"
 description = "A python wrapper-library for iterators to be usable via chaining(such as C#, Java streams or Rust iterators). Extended functionality based on Rust's buit-in iterators."
 authors = ["Adam Ruman <ruman.adam@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/addam128/chainingiterator"
 repository = "https://github.com/addam128/chainingiterator"
+include = ["chainingiterator/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.991"
 pytest = "^7.2.2"
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chainingiterator-0.1.7/PKG-INFO` & `chainingiterator-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: chainingiterator
-Version: 0.1.7
+Version: 0.1.9
 Summary: A python wrapper-library for iterators to be usable via chaining(such as C#, Java streams or Rust iterators). Extended functionality based on Rust's buit-in iterators.
 Home-page: https://github.com/addam128/chainingiterator
 License: MIT
 Author: Adam Ruman
 Author-email: ruman.adam@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/addam128/chainingiterator
 Description-Content-Type: text/markdown
 
 # chainingiterator
 A python wrapper-library for iterators to be usable via chaining(such as C#, Java streams or Rust iterators). Extended functionality based on Rust's buit-in iterators.
```

