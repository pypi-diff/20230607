# Comparing `tmp/lib-dzne-blastn-0.1.1.tar.gz` & `tmp/lib-dzne-blastn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-blastn-0.1.1.tar", last modified: Sun Feb 19 10:00:16 2023, max compression
+gzip compressed data, was "lib-dzne-blastn-0.2.0.tar", last modified: Wed Jun  7 07:13:46 2023, max compression
```

## Comparing `lib-dzne-blastn-0.1.1.tar` & `lib-dzne-blastn-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 10:00:16.656372 lib-dzne-blastn-0.1.1/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-02-19 00:26:57.000000 lib-dzne-blastn-0.1.1/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-02-19 10:00:16.656372 lib-dzne-blastn-0.1.1/PKG-INFO
--rw-r--r--   0 base      (1001) base      (1001)      506 2023-02-19 01:13:39.000000 lib-dzne-blastn-0.1.1/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-02-19 10:00:16.656372 lib-dzne-blastn-0.1.1/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 10:00:16.656372 lib-dzne-blastn-0.1.1/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 10:00:16.656372 lib-dzne-blastn-0.1.1/src/lib_dzne_blastn/
--rw-r--r--   0 base      (1001) base      (1001)     1373 2023-02-19 08:52:58.000000 lib-dzne-blastn-0.1.1/src/lib_dzne_blastn/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 10:00:16.656372 lib-dzne-blastn-0.1.1/src/lib_dzne_blastn.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-02-19 10:00:16.000000 lib-dzne-blastn-0.1.1/src/lib_dzne_blastn.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      236 2023-02-19 10:00:16.000000 lib-dzne-blastn-0.1.1/src/lib_dzne_blastn.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-02-19 10:00:16.000000 lib-dzne-blastn-0.1.1/src/lib_dzne_blastn.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       16 2023-02-19 10:00:16.000000 lib-dzne-blastn-0.1.1/src/lib_dzne_blastn.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-07 07:13:46.011367 lib-dzne-blastn-0.2.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-blastn-0.2.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-06-07 07:13:46.011367 lib-dzne-blastn-0.2.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 17:36:21.000000 lib-dzne-blastn-0.2.0/README.md
+-rw-r--r--   0 base      (1001) base      (1001)      506 2023-06-06 21:53:43.000000 lib-dzne-blastn-0.2.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-07 07:13:46.011367 lib-dzne-blastn-0.2.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-07 07:13:46.011367 lib-dzne-blastn-0.2.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-07 07:13:46.011367 lib-dzne-blastn-0.2.0/src/lib_dzne_blastn/
+-rw-r--r--   0 base      (1001) base      (1001)     1426 2023-06-07 07:12:35.000000 lib-dzne-blastn-0.2.0/src/lib_dzne_blastn/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-07 07:13:46.011367 lib-dzne-blastn-0.2.0/src/lib_dzne_blastn.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-06-07 07:13:46.000000 lib-dzne-blastn-0.2.0/src/lib_dzne_blastn.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      246 2023-06-07 07:13:46.000000 lib-dzne-blastn-0.2.0/src/lib_dzne_blastn.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-07 07:13:46.000000 lib-dzne-blastn-0.2.0/src/lib_dzne_blastn.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       16 2023-06-07 07:13:46.000000 lib-dzne-blastn-0.2.0/src/lib_dzne_blastn.egg-info/top_level.txt
```

### Comparing `lib-dzne-blastn-0.1.1/LICENSE` & `lib-dzne-blastn-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-blastn-0.1.1/PKG-INFO` & `lib-dzne-blastn-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-blastn
-Version: 0.1.1
+Version: 0.2.0
 Summary: Libary for using blastn. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-blastn-0.1.1/src/lib_dzne_blastn/__init__.py` & `lib-dzne-blastn-0.2.0/src/lib_dzne_blastn/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 
-import xml.dom.minidom
+import xml.dom.minidom as _minidom
+
+import lib_dzne_filedata as _fd
+
 
 def get_cline(prog, *, query, out, db):
     return [
         prog,
         '-db', db,
         '-task', 'blastn',
         '-dust', 'no',
@@ -12,21 +15,21 @@
         '-evalue', '0.0001',
         '-sorthits', '1',
         '-query', query, 
         '-out', out,
     ]
 
 def parse(text):
-    data = xml.dom.minidom.parseString(text)
+    data = _minidom.parseString(text)
     store = dict()
     store['query-id'] = _get(data, 'BlastOutput', 'BlastOutput_iterations', 'Iteration', 'Iteration_query-def')
     store['subject-id'] = _get(data, 'BlastOutput', 'BlastOutput_iterations', 'Iteration', 'Iteration_hits', 'Hit', 'Hit_id')
     store['bit-score'] = float(_get(data, 'BlastOutput', 'BlastOutput_iterations', 'Iteration', 'Iteration_hits', 'Hit', 'Hsp', 'Hsp_bit-score'))
     store['evalue'] = float(_get(data, 'BlastOutput', 'BlastOutput_iterations', 'Iteration', 'Iteration_hits', 'Hit', 'Hsp', 'Hsp_evalue'))
-    return store
+    return _fd.TOMLData(store)
 
 def _get(data, *keys, kind=str):
     if data is None:
         return None
     ans = data
     try:
         for key in keys:
```

### Comparing `lib-dzne-blastn-0.1.1/src/lib_dzne_blastn.egg-info/PKG-INFO` & `lib-dzne-blastn-0.2.0/src/lib_dzne_blastn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-blastn
-Version: 0.1.1
+Version: 0.2.0
 Summary: Libary for using blastn. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

