# Comparing `tmp/indxr-0.1.3.tar.gz` & `tmp/indxr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/indxr-0.1.3.tar", last modified: Tue Apr 18 09:08:49 2023, max compression
+gzip compressed data, was "dist/indxr-0.1.4.tar", last modified: Wed Jun  7 19:09:35 2023, max compression
```

## Comparing `indxr-0.1.3.tar` & `indxr-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-18 09:08:49.000000 indxr-0.1.3/
--rw-r--r--   0 elias      (501) staff       (20)     1069 2022-12-02 22:32:06.000000 indxr-0.1.3/LICENSE
--rw-r--r--   0 elias      (501) staff       (20)     7240 2023-04-18 09:08:49.000000 indxr-0.1.3/PKG-INFO
--rw-r--r--   0 elias      (501) staff       (20)     6598 2022-12-02 22:32:06.000000 indxr-0.1.3/README.md
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr/
--rw-r--r--   0 elias      (501) staff       (20)       53 2022-12-02 22:32:06.000000 indxr-0.1.3/indxr/__init__.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr/handlers/
--rw-r--r--   0 elias      (501) staff       (20)        0 2022-12-02 22:32:06.000000 indxr-0.1.3/indxr/handlers/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     2542 2022-12-02 22:32:06.000000 indxr-0.1.3/indxr/handlers/csv_handler.py
--rw-r--r--   0 elias      (501) staff       (20)      966 2022-12-02 22:32:06.000000 indxr-0.1.3/indxr/handlers/custom_handler.py
--rw-r--r--   0 elias      (501) staff       (20)     1062 2022-12-02 22:32:06.000000 indxr-0.1.3/indxr/handlers/jsonl_handler.py
--rw-r--r--   0 elias      (501) staff       (20)      788 2023-04-18 08:53:58.000000 indxr-0.1.3/indxr/handlers/multi_vector_handler.py
--rw-r--r--   0 elias      (501) staff       (20)     1106 2023-02-15 14:36:56.000000 indxr-0.1.3/indxr/handlers/numpy_handler.py
--rw-r--r--   0 elias      (501) staff       (20)      978 2023-02-15 13:58:15.000000 indxr-0.1.3/indxr/handlers/txt_handler.py
--rw-r--r--   0 elias      (501) staff       (20)     7396 2023-04-18 09:05:15.000000 indxr-0.1.3/indxr/indxr.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/
--rw-r--r--   0 elias      (501) staff       (20)     7240 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/PKG-INFO
--rw-r--r--   0 elias      (501) staff       (20)      426 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/SOURCES.txt
--rw-r--r--   0 elias      (501) staff       (20)        1 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/dependency_links.txt
--rw-r--r--   0 elias      (501) staff       (20)       13 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/requires.txt
--rw-r--r--   0 elias      (501) staff       (20)        6 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/top_level.txt
--rw-r--r--   0 elias      (501) staff       (20)       38 2023-04-18 09:08:49.000000 indxr-0.1.3/setup.cfg
--rw-r--r--   0 elias      (501) staff       (20)     1010 2023-04-18 09:08:12.000000 indxr-0.1.3/setup.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-06-07 19:09:35.000000 indxr-0.1.4/
+-rw-r--r--   0 elias      (501) staff       (20)     1069 2022-12-02 22:32:06.000000 indxr-0.1.4/LICENSE
+-rw-r--r--   0 elias      (501) staff       (20)     7240 2023-06-07 19:09:35.000000 indxr-0.1.4/PKG-INFO
+-rw-r--r--   0 elias      (501) staff       (20)     6598 2022-12-02 22:32:06.000000 indxr-0.1.4/README.md
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-06-07 19:09:35.000000 indxr-0.1.4/indxr/
+-rw-r--r--   0 elias      (501) staff       (20)       53 2022-12-02 22:32:06.000000 indxr-0.1.4/indxr/__init__.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-06-07 19:09:35.000000 indxr-0.1.4/indxr/handlers/
+-rw-r--r--   0 elias      (501) staff       (20)        0 2022-12-02 22:32:06.000000 indxr-0.1.4/indxr/handlers/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     2512 2023-06-07 19:04:36.000000 indxr-0.1.4/indxr/handlers/csv_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      966 2023-06-07 19:04:37.000000 indxr-0.1.4/indxr/handlers/custom_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)     1062 2023-06-07 19:04:38.000000 indxr-0.1.4/indxr/handlers/jsonl_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      782 2023-06-07 19:04:39.000000 indxr-0.1.4/indxr/handlers/multi_vector_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)     1106 2023-06-07 19:04:39.000000 indxr-0.1.4/indxr/handlers/numpy_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      978 2023-06-07 19:04:40.000000 indxr-0.1.4/indxr/handlers/txt_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)     7131 2023-06-07 19:08:49.000000 indxr-0.1.4/indxr/indxr.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-06-07 19:09:35.000000 indxr-0.1.4/indxr.egg-info/
+-rw-r--r--   0 elias      (501) staff       (20)     7240 2023-06-07 19:09:35.000000 indxr-0.1.4/indxr.egg-info/PKG-INFO
+-rw-r--r--   0 elias      (501) staff       (20)      426 2023-06-07 19:09:35.000000 indxr-0.1.4/indxr.egg-info/SOURCES.txt
+-rw-r--r--   0 elias      (501) staff       (20)        1 2023-06-07 19:09:35.000000 indxr-0.1.4/indxr.egg-info/dependency_links.txt
+-rw-r--r--   0 elias      (501) staff       (20)       13 2023-06-07 19:09:35.000000 indxr-0.1.4/indxr.egg-info/requires.txt
+-rw-r--r--   0 elias      (501) staff       (20)        6 2023-06-07 19:09:35.000000 indxr-0.1.4/indxr.egg-info/top_level.txt
+-rw-r--r--   0 elias      (501) staff       (20)       38 2023-06-07 19:09:35.000000 indxr-0.1.4/setup.cfg
+-rw-r--r--   0 elias      (501) staff       (20)     1010 2023-06-07 19:05:59.000000 indxr-0.1.4/setup.py
```

### Comparing `indxr-0.1.3/LICENSE` & `indxr-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `indxr-0.1.3/PKG-INFO` & `indxr-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indxr
-Version: 0.1.3
+Version: 0.1.4
 Summary: indxr: A Python utility for indexing long files.
 Home-page: https://github.com/AmenRa/indxr
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: text index,file index,index,indexer,indexing,information retrieval,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `indxr-0.1.3/README.md` & `indxr-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `indxr-0.1.3/indxr/handlers/csv_handler.py` & `indxr-0.1.4/indxr/handlers/csv_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,12 @@
     with open(path, "rb") as file:
         for i in sorting_indices:
             file.seek(positions[i])
             lines[i] = file.readline()
 
     if return_dict:
         return [
-            csv_line_to_dict(
-                line=line, fieldnames=fieldnames, delimiter=delimiter
-            )
+            csv_line_to_dict(line=line, fieldnames=fieldnames, delimiter=delimiter)
             for line in lines
         ]
 
     return [csv_line_to_list(line=line, delimiter=delimiter) for line in lines]
```

### Comparing `indxr-0.1.3/indxr/handlers/custom_handler.py` & `indxr-0.1.4/indxr/handlers/custom_handler.py`

 * *Files identical despite different names*

### Comparing `indxr-0.1.3/indxr/handlers/jsonl_handler.py` & `indxr-0.1.4/indxr/handlers/jsonl_handler.py`

 * *Files identical despite different names*

### Comparing `indxr-0.1.3/indxr/handlers/multi_vector_handler.py` & `indxr-0.1.4/indxr/handlers/multi_vector_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,11 +22,9 @@
         dtype=index["dtype"],
         mode="r",
         shape=(mapping[idx]["length"], index["dim"]),
         offset=index[idx],
     )
 
 
-def mget(
-    path: str, index: Dict, mapping: Dict, indices: List[str]
-) -> np.ndarray:
+def mget(path: str, index: Dict, mapping: Dict, indices: List[str]) -> np.ndarray:
     return [get(path, index, mapping, idx) for idx in indices]
```

### Comparing `indxr-0.1.3/indxr/handlers/numpy_handler.py` & `indxr-0.1.4/indxr/handlers/numpy_handler.py`

 * *Files identical despite different names*

### Comparing `indxr-0.1.3/indxr/handlers/txt_handler.py` & `indxr-0.1.4/indxr/handlers/txt_handler.py`

 * *Files identical despite different names*

### Comparing `indxr-0.1.3/indxr/indxr.py` & `indxr-0.1.4/indxr/indxr.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,32 +12,30 @@
     numpy_handler,
     txt_handler,
 )
 
 
 class Indxr:
     def __init__(
-        self, path: str, kind="infer", callback: Callable = None, **kwargs: Dict
+        self, path: str, kind: str = "infer", callback: Callable = None, **kwargs: Dict
     ):
         # Init  ----------------------------------------------------------------
         self.kind = kind
-        self.path = path
+        self.path = str(path)
         self.kwargs = kwargs
         self.callback = callback
         self.index = None  # Dict : k -> file position
         self.index_keys = None  # List of index keys
 
         # Infer file extension -------------------------------------------------
         if self.kind == "infer":
             self.kind = os.path.splitext(self.path)[1][1:]
 
         if self.kind not in {"txt", "jsonl", "csv", "tsv", "custom", "dat"}:
-            raise NotImplementedError(
-                f"Specified `kind` not supported. {self.kind}"
-            )
+            raise NotImplementedError(f"Specified `kind` not supported. {self.kind}")
 
         # Init kwargs ----------------------------------------------------------
         if not self.kwargs:
             self.kwargs = {}
 
         if "delimiter" not in self.kwargs:
             self.kwargs["delimiter"] = "\t" if self.kind == "tsv" else ","
@@ -74,17 +72,15 @@
             if "mapping" in self.kwargs:
                 return multi_vector_handler.index(
                     self.kwargs["dtype"],
                     self.kwargs["shape"],
                     self.kwargs["mapping"],
                 )
             else:
-                return numpy_handler.index(
-                    self.kwargs["dtype"], self.kwargs["shape"]
-                )
+                return numpy_handler.index(self.kwargs["dtype"], self.kwargs["shape"])
 
         elif self.kind == "custom":
             return custom_handler.index(self.path)
 
         raise NotImplementedError("Specified `kind` not supported.")
 
     def get(self, idx: Union[str, int]) -> Union[str, Dict, np.ndarray]:
@@ -109,39 +105,30 @@
                 x = multi_vector_handler.get(
                     path=self.path,
                     index=self.index,
                     mapping=self.kwargs["mapping"],
                     idx=str(idx),
                 )
             else:
-                x = numpy_handler.get(
-                    path=self.path, index=self.index, idx=str(idx)
-                )
+                x = numpy_handler.get(path=self.path, index=self.index, idx=str(idx))
 
         elif self.kind == "custom":
             x = custom_handler.get(path=self.path, index=self.index, idx=idx)
 
         else:
             raise NotImplementedError()
 
         return self.callback(x) if self.callback else x
 
     def mget(self, indices: List[str]) -> List[Union[str, Dict, np.ndarray]]:
         if self.kind == "txt":
-            xs = txt_handler.mget(
-                path=self.path,
-                index=self.index,
-                mapping=self.kwargs["mapping"],
-                indices=indices,
-            )
+            xs = txt_handler.mget(path=self.path, index=self.index, indices=indices)
 
         elif self.kind == "jsonl":
-            xs = jsonl_handler.mget(
-                path=self.path, index=self.index, indices=indices
-            )
+            xs = jsonl_handler.mget(path=self.path, index=self.index, indices=indices)
 
         elif self.kind in {"csv", "tsv"}:
             xs = csv_handler.mget(
                 path=self.path,
                 index=self.index,
                 indices=indices,
                 delimiter=self.kwargs["delimiter"],
@@ -161,17 +148,15 @@
                 xs = numpy_handler.mget(
                     path=self.path,
                     index=self.index,
                     indices=[str(idx) for idx in indices],
                 )
 
         elif self.kind == "custom":
-            xs = custom_handler.mget(
-                path=self.path, index=self.index, indices=indices
-            )
+            xs = custom_handler.mget(path=self.path, index=self.index, indices=indices)
 
         else:
             raise NotImplementedError()
 
         return [self.callback(x) for x in xs] if self.callback else xs
 
     def get_slice(self, start: int, stop: int) -> np.ndarray:
```

### Comparing `indxr-0.1.3/indxr.egg-info/PKG-INFO` & `indxr-0.1.4/indxr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indxr
-Version: 0.1.3
+Version: 0.1.4
 Summary: indxr: A Python utility for indexing long files.
 Home-page: https://github.com/AmenRa/indxr
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: text index,file index,index,indexer,indexing,information retrieval,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `indxr-0.1.3/setup.py` & `indxr-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="indxr",
-    version="0.1.3",
+    version="0.1.4",
     author="Elias Bassani",
     author_email="elias.bssn@gmail.com",
     description="indxr: A Python utility for indexing long files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AmenRa/indxr",
     packages=setuptools.find_packages(),
```

