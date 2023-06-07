# Comparing `tmp/insituTEM-0.1.2.tar.gz` & `tmp/insituTEM-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insituTEM-0.1.2.tar", last modified: Wed Jun  7 01:54:56 2023, max compression
+gzip compressed data, was "insituTEM-0.1.3.tar", last modified: Wed Jun  7 01:56:31 2023, max compression
```

## Comparing `insituTEM-0.1.2.tar` & `insituTEM-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:54:56.058812 insituTEM-0.1.2/
--rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 01:54:56.058631 insituTEM-0.1.2/PKG-INFO
-drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:54:56.057570 insituTEM-0.1.2/insituTEM/
--rw-r--r--   0 monali     (501) staff       (20)        0 2023-06-07 00:56:09.000000 insituTEM-0.1.2/insituTEM/__ init __.py
--rw-r--r--   0 monali     (501) staff       (20)     4228 2021-08-11 23:48:44.000000 insituTEM-0.1.2/insituTEM/insitu_DP.py
--rw-r--r--   0 monali     (501) staff       (20)    12479 2023-02-20 17:08:48.000000 insituTEM-0.1.2/insituTEM/insitu_IO.py
--rw-r--r--   0 monali     (501) staff       (20)     6070 2023-02-07 23:34:02.000000 insituTEM-0.1.2/insituTEM/insitu_Preprocess.py
--rw-r--r--   0 monali     (501) staff       (20)     8779 2023-02-20 21:40:28.000000 insituTEM-0.1.2/insituTEM/insitu_alignment.py
-drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:54:56.058363 insituTEM-0.1.2/insituTEM.egg-info/
--rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 01:54:55.000000 insituTEM-0.1.2/insituTEM.egg-info/PKG-INFO
--rw-r--r--   0 monali     (501) staff       (20)      303 2023-06-07 01:54:56.000000 insituTEM-0.1.2/insituTEM.egg-info/SOURCES.txt
--rw-r--r--   0 monali     (501) staff       (20)        1 2023-06-07 01:54:55.000000 insituTEM-0.1.2/insituTEM.egg-info/dependency_links.txt
--rw-r--r--   0 monali     (501) staff       (20)       70 2023-06-07 01:54:55.000000 insituTEM-0.1.2/insituTEM.egg-info/requires.txt
--rw-r--r--   0 monali     (501) staff       (20)       10 2023-06-07 01:54:55.000000 insituTEM-0.1.2/insituTEM.egg-info/top_level.txt
--rw-r--r--   0 monali     (501) staff       (20)       38 2023-06-07 01:54:56.058872 insituTEM-0.1.2/setup.cfg
--rw-r--r--   0 monali     (501) staff       (20)      388 2023-06-07 01:54:39.000000 insituTEM-0.1.2/setup.py
+drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:56:31.792085 insituTEM-0.1.3/
+-rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 01:56:31.791864 insituTEM-0.1.3/PKG-INFO
+drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:56:31.790777 insituTEM-0.1.3/insituTEM/
+-rw-r--r--   0 monali     (501) staff       (20)        0 2023-06-07 00:56:09.000000 insituTEM-0.1.3/insituTEM/__ init __.py
+-rw-r--r--   0 monali     (501) staff       (20)     4228 2021-08-11 23:48:44.000000 insituTEM-0.1.3/insituTEM/insitu_DP.py
+-rw-r--r--   0 monali     (501) staff       (20)    12479 2023-02-20 17:08:48.000000 insituTEM-0.1.3/insituTEM/insitu_IO.py
+-rw-r--r--   0 monali     (501) staff       (20)     6070 2023-02-07 23:34:02.000000 insituTEM-0.1.3/insituTEM/insitu_Preprocess.py
+-rw-r--r--   0 monali     (501) staff       (20)     8779 2023-02-20 21:40:28.000000 insituTEM-0.1.3/insituTEM/insitu_alignment.py
+drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:56:31.791581 insituTEM-0.1.3/insituTEM.egg-info/
+-rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 01:56:31.000000 insituTEM-0.1.3/insituTEM.egg-info/PKG-INFO
+-rw-r--r--   0 monali     (501) staff       (20)      303 2023-06-07 01:56:31.000000 insituTEM-0.1.3/insituTEM.egg-info/SOURCES.txt
+-rw-r--r--   0 monali     (501) staff       (20)        1 2023-06-07 01:56:31.000000 insituTEM-0.1.3/insituTEM.egg-info/dependency_links.txt
+-rw-r--r--   0 monali     (501) staff       (20)       63 2023-06-07 01:56:31.000000 insituTEM-0.1.3/insituTEM.egg-info/requires.txt
+-rw-r--r--   0 monali     (501) staff       (20)       10 2023-06-07 01:56:31.000000 insituTEM-0.1.3/insituTEM.egg-info/top_level.txt
+-rw-r--r--   0 monali     (501) staff       (20)       38 2023-06-07 01:56:31.792163 insituTEM-0.1.3/setup.cfg
+-rw-r--r--   0 monali     (501) staff       (20)      381 2023-06-07 01:56:20.000000 insituTEM-0.1.3/setup.py
```

### Comparing `insituTEM-0.1.2/insituTEM/insitu_DP.py` & `insituTEM-0.1.3/insituTEM/insitu_DP.py`

 * *Files identical despite different names*

### Comparing `insituTEM-0.1.2/insituTEM/insitu_IO.py` & `insituTEM-0.1.3/insituTEM/insitu_IO.py`

 * *Files identical despite different names*

### Comparing `insituTEM-0.1.2/insituTEM/insitu_Preprocess.py` & `insituTEM-0.1.3/insituTEM/insitu_Preprocess.py`

 * *Files identical despite different names*

### Comparing `insituTEM-0.1.2/insituTEM/insitu_alignment.py` & `insituTEM-0.1.3/insituTEM/insitu_alignment.py`

 * *Files identical despite different names*

