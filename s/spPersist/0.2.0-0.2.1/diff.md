# Comparing `tmp/sppersist-0.2.0.tar.gz` & `tmp/spPersist-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "spPersist-0.2.1.tar", last modified: Wed Jun  7 09:36:28 2023, max compression
```

## Comparing `sppersist-0.2.0.tar` & `spPersist-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,19 @@
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-0.2.0/src/spPersist/DTM_filtrations.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sppersist-0.2.0/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9403 2020-02-02 00:00:00.000000 sppersist-0.2.0/src/spPersist/dp.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-0.2.0/src/spPersist/persistence_statistics.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 sppersist-0.2.0/src/spPersist/ph.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.2.0/LICENSE
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 sppersist-0.2.0/README.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sppersist-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 sppersist-0.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:36:28.544051 spPersist-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-07 09:35:54.000000 spPersist-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-06-07 09:36:28.543051 spPersist-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-06-07 09:35:54.000000 spPersist-0.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 09:36:28.544051 spPersist-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8096 2023-06-07 09:35:54.000000 spPersist-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:36:28.540051 spPersist-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:36:28.542051 spPersist-0.2.1/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-07 09:21:49.000000 spPersist-0.2.1/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-07 09:21:49.000000 spPersist-0.2.1/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-07 09:21:49.000000 spPersist-0.2.1/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-07 09:21:48.000000 spPersist-0.2.1/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-06-07 09:21:49.000000 spPersist-0.2.1/src/spPersist/ph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:36:28.543051 spPersist-0.2.1/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-06-07 09:36:28.000000 spPersist-0.2.1/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-07 09:36:28.000000 spPersist-0.2.1/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 09:36:28.000000 spPersist-0.2.1/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-07 09:36:28.000000 spPersist-0.2.1/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-07 09:36:28.000000 spPersist-0.2.1/src/spPersist.egg-info/top_level.txt
```

### Comparing `sppersist-0.2.0/src/spPersist/DTM_filtrations.py` & `spPersist-0.2.1/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `sppersist-0.2.0/src/spPersist/dp.py` & `spPersist-0.2.1/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `sppersist-0.2.0/src/spPersist/persistence_statistics.py` & `spPersist-0.2.1/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `sppersist-0.2.0/src/spPersist/ph.py` & `spPersist-0.2.1/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `sppersist-0.2.0/LICENSE` & `spPersist-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.2.0/README.md` & `spPersist-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sppersist-0.2.0/PKG-INFO` & `spPersist-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.2.0
+Version: 0.2.1
 Summary: Spatial transcriptomics with Persistent Homology
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Author-email: Lirong Yang <lirong.yang@outlook.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Home-page: https://github.com/pypa/sampleproject
+Author: Lirong Yang
+Author-email: lirong.yang@outlook.com
+Keywords: spatial transcriptomics,persistent homology,single-cell analysis
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Spatial Transcriptomics with Persistent Homology
 
 This is a package for classifying Spatial Transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
 the theory of Persistent Homology and its homology barcodes. The package so far
 contains a data processing module, called dp, allowing users to load either the
 standard datasets from Visium and MERFISH, or published datasets into desired
 annotated data format for the analysis performed in this package. The format is
 compatible with the package Squidpy.
 
 It is intended that the package will also include a pre-processing module, a 
 persistent homology module and a homological classification module, respectively
-named pp, ph and hc.
+named pp, ph and hc.
```

