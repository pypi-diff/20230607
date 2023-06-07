# Comparing `tmp/pipd-0.1.3.tar.gz` & `tmp/pipd-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.1.3.tar", last modified: Tue Jun  6 22:47:44 2023, max compression
+gzip compressed data, was "pipd-0.1.4.tar", last modified: Wed Jun  7 08:09:59 2023, max compression
```

## Comparing `pipd-0.1.3.tar` & `pipd-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:47:44.509311 pipd-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-06 22:47:44.509311 pipd-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-06 22:47:31.000000 pipd-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:47:44.501311 pipd-0.1.3/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:47:44.509311 pipd-0.1.3/pipd/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/filter_cached.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/read_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/unbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/functions/write_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:47:44.509311 pipd-0.1.3/pipd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-06 22:47:31.000000 pipd-0.1.3/pipd/tests/test_pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:47:44.505311 pipd-0.1.3/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-06 22:47:44.000000 pipd-0.1.3/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-06 22:47:44.000000 pipd-0.1.3/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 22:47:44.000000 pipd-0.1.3/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 22:47:44.000000 pipd-0.1.3/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 22:47:44.509311 pipd-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-06 22:47:31.000000 pipd-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:09:59.193997 pipd-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-07 08:09:59.193997 pipd-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-07 08:09:47.000000 pipd-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:09:59.189997 pipd-0.1.4/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:09:59.193997 pipd-0.1.4/pipd/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/filter_cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/read_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/unbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/functions/write_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:09:59.193997 pipd-0.1.4/pipd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-07 08:09:47.000000 pipd-0.1.4/pipd/tests/test_pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:09:59.189997 pipd-0.1.4/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-07 08:09:59.000000 pipd-0.1.4/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-07 08:09:59.000000 pipd-0.1.4/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:09:59.000000 pipd-0.1.4/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 08:09:59.000000 pipd-0.1.4/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 08:09:59.193997 pipd-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-07 08:09:47.000000 pipd-0.1.4/setup.py
```

### Comparing `pipd-0.1.3/README.md` & `pipd-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/functions/batch.py` & `pipd-0.1.4/pipd/functions/batch.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/functions/filter.py` & `pipd-0.1.4/pipd/functions/filter.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/functions/filter_cached.py` & `pipd-0.1.4/pipd/functions/filter_cached.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/functions/map.py` & `pipd-0.1.4/pipd/functions/map.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/functions/read_csv.py` & `pipd-0.1.4/pipd/functions/read_csv.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/functions/read_files.py` & `pipd-0.1.4/pipd/functions/read_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import glob
 import os
+import random
 from typing import Iterable, Iterator, Optional, Sequence, TypeVar
 
 from pipd import Function, Pipe
 
 from .read_lines import read_lines
 from .write_lines import write_lines
 
@@ -25,31 +26,38 @@
         for change, filepath in loop.run_until_complete(async_generator.__anext__()):
             if change in changes:
                 yield filepath
 
 
 class ReadFiles(Function):
     def __init__(
-        self, cache_filepath: Optional[str] = None, watch: bool = False
+        self,
+        cache_filepath: Optional[str] = None,
+        watch: bool = False,
+        shuffle: bool = False,
     ) -> None:
         self.cache_filepath = cache_filepath
         self.watch = watch
+        self.shuffle = shuffle
 
     def __call__(self, items: Iterable[str]) -> Iterator[str]:
         for filepath in items:
             files = []
             if self.cache_filepath is not None:
                 if os.path.exists(self.cache_filepath):
                     files = list(read_lines(filepath=self.cache_filepath))
                 else:
                     files = glob.glob(filepath)
                     list(write_lines(files, filepath=self.cache_filepath))
             else:
                 files = glob.glob(filepath)
 
+            if self.shuffle:
+                random.shuffle(files)
+
             for file in files:
                 yield file
             if self.watch:
                 yield from watchdir(os.path.dirname(filepath))
 
 
 Pipe.add_fn(ReadFiles)
```

### Comparing `pipd-0.1.3/pipd/functions/read_lines.py` & `pipd-0.1.4/pipd/functions/read_lines.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/functions/shuffle.py` & `pipd-0.1.4/pipd/functions/shuffle.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/functions/side.py` & `pipd-0.1.4/pipd/functions/side.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/functions/tqdm.py` & `pipd-0.1.4/pipd/functions/tqdm.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/functions/write_csv.py` & `pipd-0.1.4/pipd/functions/write_csv.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/pipe.py` & `pipd-0.1.4/pipd/pipe.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd/tests/test_functions.py` & `pipd-0.1.4/pipd/tests/test_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -154,7 +154,18 @@
         assert list(pipe) == [f1.name, f2.name]
         # Check content of cache
         with open(f"{d}/cache.txt", "r") as f:
             assert f.read() == f"{f1.name}\n{f2.name}\n"
         pipe = Pipe([f"{d}/*.txt"]).read_files(cache_filepath=f"{d}/cache.txt")
         assert list(pipe) == [f1.name, f2.name]
         os.remove(f"{d}/cache.txt")
+
+    # Test shuffle
+    with tempfile.TemporaryDirectory() as d:
+        with open(os.path.join(d, "f1.txt"), "w") as f1:
+            f1.write("a")
+        with open(os.path.join(d, "f2.txt"), "w") as f2:
+            f2.write("b")
+        pipe = Pipe([f"{d}/*.txt"]).read_files(shuffle=True)
+        assert sorted(list(pipe)) == sorted([f1.name, f2.name])
+        os.remove(f1.name)
+        os.remove(f2.name)
```

### Comparing `pipd-0.1.3/pipd/tests/test_pipe.py` & `pipd-0.1.4/pipd/tests/test_pipe.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.3/pipd.egg-info/SOURCES.txt` & `pipd-0.1.4/pipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

