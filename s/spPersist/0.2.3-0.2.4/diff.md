# Comparing `tmp/spPersist-0.2.3.tar.gz` & `tmp/spPersist-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.2.3.tar", last modified: Wed Jun  7 09:46:19 2023, max compression
+gzip compressed data, was "spPersist-0.2.4.tar", last modified: Wed Jun  7 09:55:16 2023, max compression
```

## Comparing `spPersist-0.2.3.tar` & `spPersist-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:46:19.753904 spPersist-0.2.3/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-07 09:35:54.000000 spPersist-0.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1133 2023-06-07 09:46:19.751904 spPersist-0.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-06-07 09:35:54.000000 spPersist-0.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 09:46:19.753904 spPersist-0.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8111 2023-06-07 09:45:45.000000 spPersist-0.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:46:19.743903 spPersist-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:46:19.749904 spPersist-0.2.3/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-07 09:21:49.000000 spPersist-0.2.3/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-07 09:21:49.000000 spPersist-0.2.3/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-07 09:21:49.000000 spPersist-0.2.3/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-07 09:21:48.000000 spPersist-0.2.3/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     3350 2023-06-07 09:40:39.000000 spPersist-0.2.3/src/spPersist/ph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:46:19.751904 spPersist-0.2.3/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1133 2023-06-07 09:46:19.000000 spPersist-0.2.3/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-07 09:46:19.000000 spPersist-0.2.3/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 09:46:19.000000 spPersist-0.2.3/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-07 09:46:19.000000 spPersist-0.2.3/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-07 09:46:19.000000 spPersist-0.2.3/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:55:16.020020 spPersist-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-07 09:35:54.000000 spPersist-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-06-07 09:55:16.019020 spPersist-0.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-06-07 09:35:54.000000 spPersist-0.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 09:55:16.020020 spPersist-0.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-06-07 09:54:46.000000 spPersist-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:55:16.016019 spPersist-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:55:16.018020 spPersist-0.2.4/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-07 09:21:49.000000 spPersist-0.2.4/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-07 09:21:49.000000 spPersist-0.2.4/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-06-07 09:54:33.000000 spPersist-0.2.4/src/spPersist/ph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:55:16.019020 spPersist-0.2.4/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-06-07 09:55:16.000000 spPersist-0.2.4/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-07 09:55:16.000000 spPersist-0.2.4/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 09:55:16.000000 spPersist-0.2.4/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-07 09:55:16.000000 spPersist-0.2.4/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-07 09:55:16.000000 spPersist-0.2.4/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.2.3/LICENSE` & `spPersist-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.3/PKG-INFO` & `spPersist-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.2.3
+Version: 0.2.4
 Summary: Spatial transcriptomics with Persistent Homology
 Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Keywords: spatial transcriptomics,persistent homology,single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `spPersist-0.2.3/README.md` & `spPersist-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.3/setup.py` & `spPersist-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="spPersist",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.2.3",  # Required
+    version="0.2.4",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-0.2.3/src/spPersist/dp.py` & `spPersist-0.2.4/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.3/src/spPersist/ph.py` & `spPersist-0.2.4/src/spPersist/ph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# from DTM_filtrations import *
-# import persistence_statistics as ps
+from DTM_filtrations import *
+import persistence_statistics as ps
 
 import gudhi
 import numpy as np
 import matplotlib.pyplot as plt
 
 def compute_simplicial_complex(X,ptype: str,max_dimension=2,p=1,m=0.1,is_plot=False):
   '''
```

### Comparing `spPersist-0.2.3/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.2.4/src/spPersist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.2.3
+Version: 0.2.4
 Summary: Spatial transcriptomics with Persistent Homology
 Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Keywords: spatial transcriptomics,persistent homology,single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

