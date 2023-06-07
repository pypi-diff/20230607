# Comparing `tmp/foc-0.1.0.tar.gz` & `tmp/foc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foc-0.1.0.tar", last modified: Wed Jun  7 00:03:37 2023, max compression
+gzip compressed data, was "foc-0.1.1.tar", last modified: Wed Jun  7 00:38:12 2023, max compression
```

## Comparing `foc-0.1.0.tar` & `foc-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-07 00:03:37.747258 foc-0.1.0/
--rw-r--r--   0 thyeem     (501) staff       (20)       31 2023-06-06 23:58:42.000000 foc-0.1.0/ChangeLog.md
--rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-05-15 21:22:31.000000 foc-0.1.0/LICENSE
--rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-06 23:18:02.000000 foc-0.1.0/MANIFEST.in
--rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-07 00:03:37.747352 foc-0.1.0/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)    16005 2023-06-06 23:52:11.000000 foc-0.1.0/README.md
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-07 00:03:37.745551 foc-0.1.0/foc/
--rw-r--r--   0 thyeem     (501) staff       (20)    15894 2023-06-06 23:58:42.000000 foc-0.1.0/foc/__init__.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-07 00:03:37.747044 foc-0.1.0/foc.egg-info/
--rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-07 00:03:37.000000 foc-0.1.0/foc.egg-info/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)      185 2023-06-07 00:03:37.000000 foc-0.1.0/foc.egg-info/SOURCES.txt
--rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-06-07 00:03:37.000000 foc-0.1.0/foc.egg-info/dependency_links.txt
--rw-r--r--   0 thyeem     (501) staff       (20)        4 2023-06-07 00:03:37.000000 foc-0.1.0/foc.egg-info/top_level.txt
--rw-r--r--   0 thyeem     (501) staff       (20)      131 2023-06-07 00:03:37.747767 foc-0.1.0/setup.cfg
--rw-r--r--   0 thyeem     (501) staff       (20)      696 2023-06-07 00:00:34.000000 foc-0.1.0/setup.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-07 00:38:12.376820 foc-0.1.1/
+-rw-r--r--   0 thyeem     (501) staff       (20)       31 2023-06-07 00:37:35.000000 foc-0.1.1/ChangeLog.md
+-rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-05-15 21:22:31.000000 foc-0.1.1/LICENSE
+-rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-06 23:18:02.000000 foc-0.1.1/MANIFEST.in
+-rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-07 00:38:12.376919 foc-0.1.1/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)    16005 2023-06-07 00:35:01.000000 foc-0.1.1/README.md
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-07 00:38:12.375446 foc-0.1.1/foc/
+-rw-r--r--   0 thyeem     (501) staff       (20)    15894 2023-06-06 23:58:42.000000 foc-0.1.1/foc/__init__.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-07 00:38:12.376594 foc-0.1.1/foc.egg-info/
+-rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-07 00:38:12.000000 foc-0.1.1/foc.egg-info/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)      185 2023-06-07 00:38:12.000000 foc-0.1.1/foc.egg-info/SOURCES.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-06-07 00:38:12.000000 foc-0.1.1/foc.egg-info/dependency_links.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)        4 2023-06-07 00:38:12.000000 foc-0.1.1/foc.egg-info/top_level.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-06-07 00:38:12.377327 foc-0.1.1/setup.cfg
+-rw-r--r--   0 thyeem     (501) staff       (20)      696 2023-06-07 00:37:27.000000 foc-0.1.1/setup.py
```

### Comparing `foc-0.1.0/LICENSE` & `foc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `foc-0.1.0/README.md` & `foc-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -381,18 +381,18 @@
 # 'flat' returns a generator. flatl = cfd(list)(flat)
 >>> flatl(data)    # list
 [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
 
 >>> flatt(data)    # tuple
 (1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15)
 
->>> flatt(data)    # set
+>>> flats(data)    # set
 {1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15}
 
->>> flatt(data)    # deque
+>>> flatd(data)    # deque
 deque([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15])
 
 # regardless of the number of arguments
 >>> flatl(1,[2,{3}],[[[[[4]],5]]], "sofia", "maria")
 [1, 2, 3, 4, 5, 'sofia', 'maria']
 ```
```

### Comparing `foc-0.1.0/foc/__init__.py` & `foc-0.1.1/foc/__init__.py`

 * *Files identical despite different names*

### Comparing `foc-0.1.0/setup.py` & `foc-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_decription = f.read()
 
 setuptools.setup(
     name="foc",
-    version="0.1.0",
+    version="0.1.1",
     author="Francis Lim",
     author_email="thyeem@gmail.com",
     description="A collection of python functions for somebody's sanity",
     long_decription=long_decription,
     long_decription_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/thyeem/foc",
```

