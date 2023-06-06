# Comparing `tmp/pipd-0.1.1.tar.gz` & `tmp/pipd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.1.1.tar", last modified: Tue Jun  6 17:25:54 2023, max compression
+gzip compressed data, was "pipd-0.1.2.tar", last modified: Tue Jun  6 22:14:10 2023, max compression
```

## Comparing `pipd-0.1.1.tar` & `pipd-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:25:54.882620 pipd-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-06 17:25:54.882620 pipd-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-06 17:25:44.000000 pipd-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:25:54.878620 pipd-0.1.1/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:25:54.882620 pipd-0.1.1/pipd/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/filter_cached.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/read_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/unbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/functions/write_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:25:54.882620 pipd-0.1.1/pipd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-06 17:25:44.000000 pipd-0.1.1/pipd/tests/test_pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:25:54.878620 pipd-0.1.1/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-06 17:25:54.000000 pipd-0.1.1/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-06 17:25:54.000000 pipd-0.1.1/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:25:54.000000 pipd-0.1.1/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 17:25:54.000000 pipd-0.1.1/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:25:54.882620 pipd-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-06 17:25:44.000000 pipd-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:14:10.443258 pipd-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-06 22:14:10.443258 pipd-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-06 22:13:59.000000 pipd-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:14:10.435258 pipd-0.1.2/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:14:10.443258 pipd-0.1.2/pipd/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/filter_cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/read_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/unbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/functions/write_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:14:10.443258 pipd-0.1.2/pipd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-06 22:13:59.000000 pipd-0.1.2/pipd/tests/test_pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:14:10.435258 pipd-0.1.2/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-06 22:14:10.000000 pipd-0.1.2/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-06 22:14:10.000000 pipd-0.1.2/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 22:14:10.000000 pipd-0.1.2/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 22:14:10.000000 pipd-0.1.2/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 22:14:10.443258 pipd-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-06 22:13:59.000000 pipd-0.1.2/setup.py
```

### Comparing `pipd-0.1.1/README.md` & `pipd-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pipd-0.1.1/pipd/functions/filter.py` & `pipd-0.1.2/pipd/functions/filter.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.1/pipd/functions/filter_cached.py` & `pipd-0.1.2/pipd/functions/filter_cached.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.1/pipd/functions/map.py` & `pipd-0.1.2/pipd/functions/map.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.1/pipd/functions/read_csv.py` & `pipd-0.1.2/pipd/functions/read_csv.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.1/pipd/functions/read_files.py` & `pipd-0.1.2/pipd/functions/read_files.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.1/pipd/functions/read_lines.py` & `pipd-0.1.2/pipd/functions/read_lines.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.1/pipd/functions/shuffle.py` & `pipd-0.1.2/pipd/functions/shuffle.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.1/pipd/functions/side.py` & `pipd-0.1.2/pipd/functions/side.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.1/pipd/functions/tqdm.py` & `pipd-0.1.2/pipd/functions/tqdm.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.1/pipd/functions/write_csv.py` & `pipd-0.1.2/pipd/functions/write_csv.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.1/pipd/tests/test_functions.py` & `pipd-0.1.2/pipd/tests/test_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 def test_unbatch():
     pipe = Pipe([[0, 1], [2, 3], [4]]).unbatch()
     assert list(pipe) == [0, 1, 2, 3, 4]
 
 
 def test_shuffle():
     pipe = Pipe(range(5)).shuffle(2)
-    assert list(pipe) != [0, 1, 2, 3, 4]
+    assert sorted(pipe) == [0, 1, 2, 3, 4]
 
 
 def test_limit():
     pipe = Pipe(range(5)).limit(3)
     assert list(pipe) == [0, 1, 2]
```

### Comparing `pipd-0.1.1/pipd/tests/test_pipe.py` & `pipd-0.1.2/pipd/tests/test_pipe.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,7 +22,14 @@
 
 
 def test_add():
     pipe0 = Pipe(0, 1, 2, 3)
     pipe1 = Pipe(4, 5, 6, 7)
     pipe = pipe0 + pipe1
     assert list(pipe) == [0, 1, 2, 3, 4, 5, 6, 7]
+
+
+def test_merge():
+    pipe0 = Pipe(0, 0, 0, 0, 0, 0)
+    pipe1 = Pipe(1, 1, 1, 1, 1, 1)
+    pipe = Pipe.merge(pipe0, pipe1, weights=[3, 1])
+    print(list(pipe))
```

### Comparing `pipd-0.1.1/pipd.egg-info/SOURCES.txt` & `pipd-0.1.2/pipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

