# Comparing `tmp/kbib-0.1.8.tar.gz` & `tmp/kbib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbib-0.1.8.tar", last modified: Wed Jun  7 12:57:41 2023, max compression
+gzip compressed data, was "kbib-0.1.9.tar", last modified: Wed Jun  7 13:24:39 2023, max compression
```

## Comparing `kbib-0.1.8.tar` & `kbib-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:57:41.454111 kbib-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 12:57:21.000000 kbib-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-07 12:57:21.000000 kbib-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-07 12:57:41.454111 kbib-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-07 12:57:21.000000 kbib-0.1.8/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:57:41.454111 kbib-0.1.8/kbib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:57:21.000000 kbib-0.1.8/kbib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-07 12:57:21.000000 kbib-0.1.8/kbib/parseRefs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-06-07 12:57:21.000000 kbib-0.1.8/kbib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:57:41.454111 kbib-0.1.8/kbib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:57:41.454111 kbib-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-07 12:57:21.000000 kbib-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:24:39.867376 kbib-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 13:24:18.000000 kbib-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-07 13:24:18.000000 kbib-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-07 13:24:39.867376 kbib-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-07 13:24:18.000000 kbib-0.1.9/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:24:39.863376 kbib-0.1.9/kbib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:24:18.000000 kbib-0.1.9/kbib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-07 13:24:18.000000 kbib-0.1.9/kbib/parseRefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-06-07 13:24:18.000000 kbib-0.1.9/kbib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:24:39.867376 kbib-0.1.9/kbib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-07 13:24:39.000000 kbib-0.1.9/kbib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-07 13:24:39.000000 kbib-0.1.9/kbib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:24:39.000000 kbib-0.1.9/kbib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 13:24:39.000000 kbib-0.1.9/kbib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 13:24:39.000000 kbib-0.1.9/kbib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 13:24:39.000000 kbib-0.1.9/kbib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:24:39.000000 kbib-0.1.9/kbib.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:24:39.867376 kbib-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-07 13:24:18.000000 kbib-0.1.9/setup.py
```

### Comparing `kbib-0.1.8/LICENSE` & `kbib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kbib-0.1.8/PKG-INFO` & `kbib-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbib
-Version: 0.1.8
+Version: 0.1.9
 Summary: A command line tool to get bibtex information from DOIs and PDFs
 Author: Koushik Naskar
 Author-email: koushik.naskar9@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Koushikphy/kbib
 Keywords: bibtex references doi crossref
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kbib-0.1.8/Readme.md` & `kbib-0.1.9/Readme.md`

 * *Files identical despite different names*

### Comparing `kbib-0.1.8/kbib/parseRefs.py` & `kbib-0.1.9/kbib/parseRefs.py`

 * *Files identical despite different names*

### Comparing `kbib-0.1.8/kbib/utils.py` & `kbib-0.1.9/kbib/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -333,32 +333,37 @@
         checkTex = True
 
 
 
     bib_db = bibtexparser.loads('\n'.join(open(f).read() for f in bibFiles))
     entries = bib_db.entries
 
-    dat = defaultdict(list)
+    dat = defaultdict(set)
     # duplication will be decided based only on these keys
     keysToMatch = ['year','volume','pages']  
 
 
     for en in entries:
         it = tuple(en.get(i,'') for i in keysToMatch)
         idd = en.get('ID')
         if checkTex:
             if idd in cites:  # only references that are cited
-                dat[it].append(en.get('ID'))
+                dat[it].add(en.get('ID'))
         else:
-            dat[it].append(en.get('ID'))
+            dat[it].add(en.get('ID'))
 
 
-    for k,v in dat.items():
-        if len(v)>1:
-            print(v)
+    dupList = [list(v) for _,v in dat.items() if len(v)>1 ]
+    if len(dupList)==0:
+        print('No duplicate reference found.')
+        return
+    print("The following bib entries may be duplicate. Please check:\n")
+    for i,el in enumerate(dupList,start=1):
+        print(f"{i}. {', '.join(el)}")
+
 
 
 # progress = Progress()
 
 # progress.start()
 # task = progress.add_task("Getting references-------------",total=124)
```

### Comparing `kbib-0.1.8/kbib.egg-info/PKG-INFO` & `kbib-0.1.9/kbib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbib
-Version: 0.1.8
+Version: 0.1.9
 Summary: A command line tool to get bibtex information from DOIs and PDFs
 Author: Koushik Naskar
 Author-email: koushik.naskar9@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Koushikphy/kbib
 Keywords: bibtex references doi crossref
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kbib-0.1.8/setup.py` & `kbib-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('Readme.md') as f:
     txt = f.read()
 
 setup(name='kbib',
-    version='0.1.8',
+    version='0.1.9',
     description='A command line tool to get bibtex information from DOIs and PDFs',
     long_description=txt,
     long_description_content_type='text/markdown',
     author='Koushik Naskar',
     author_email='koushik.naskar9@gmail.com',
     license="MIT",
     classifiers=[
```

