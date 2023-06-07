# Comparing `tmp/insituTEM-0.1.3.tar.gz` & `tmp/insituTEM-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insituTEM-0.1.3.tar", last modified: Wed Jun  7 01:56:31 2023, max compression
+gzip compressed data, was "insituTEM-0.1.4.tar", last modified: Wed Jun  7 01:58:24 2023, max compression
```

## Comparing `insituTEM-0.1.3.tar` & `insituTEM-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:56:31.792085 insituTEM-0.1.3/
--rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 01:56:31.791864 insituTEM-0.1.3/PKG-INFO
-drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:56:31.790777 insituTEM-0.1.3/insituTEM/
--rw-r--r--   0 monali     (501) staff       (20)        0 2023-06-07 00:56:09.000000 insituTEM-0.1.3/insituTEM/__ init __.py
--rw-r--r--   0 monali     (501) staff       (20)     4228 2021-08-11 23:48:44.000000 insituTEM-0.1.3/insituTEM/insitu_DP.py
--rw-r--r--   0 monali     (501) staff       (20)    12479 2023-02-20 17:08:48.000000 insituTEM-0.1.3/insituTEM/insitu_IO.py
--rw-r--r--   0 monali     (501) staff       (20)     6070 2023-02-07 23:34:02.000000 insituTEM-0.1.3/insituTEM/insitu_Preprocess.py
--rw-r--r--   0 monali     (501) staff       (20)     8779 2023-02-20 21:40:28.000000 insituTEM-0.1.3/insituTEM/insitu_alignment.py
-drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:56:31.791581 insituTEM-0.1.3/insituTEM.egg-info/
--rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 01:56:31.000000 insituTEM-0.1.3/insituTEM.egg-info/PKG-INFO
--rw-r--r--   0 monali     (501) staff       (20)      303 2023-06-07 01:56:31.000000 insituTEM-0.1.3/insituTEM.egg-info/SOURCES.txt
--rw-r--r--   0 monali     (501) staff       (20)        1 2023-06-07 01:56:31.000000 insituTEM-0.1.3/insituTEM.egg-info/dependency_links.txt
--rw-r--r--   0 monali     (501) staff       (20)       63 2023-06-07 01:56:31.000000 insituTEM-0.1.3/insituTEM.egg-info/requires.txt
--rw-r--r--   0 monali     (501) staff       (20)       10 2023-06-07 01:56:31.000000 insituTEM-0.1.3/insituTEM.egg-info/top_level.txt
--rw-r--r--   0 monali     (501) staff       (20)       38 2023-06-07 01:56:31.792163 insituTEM-0.1.3/setup.cfg
--rw-r--r--   0 monali     (501) staff       (20)      381 2023-06-07 01:56:20.000000 insituTEM-0.1.3/setup.py
+drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:58:24.543040 insituTEM-0.1.4/
+-rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 01:58:24.542874 insituTEM-0.1.4/PKG-INFO
+drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:58:24.541849 insituTEM-0.1.4/insituTEM/
+-rw-r--r--   0 monali     (501) staff       (20)        0 2023-06-07 00:56:09.000000 insituTEM-0.1.4/insituTEM/__ init __.py
+-rw-r--r--   0 monali     (501) staff       (20)     4228 2021-08-11 23:48:44.000000 insituTEM-0.1.4/insituTEM/insitu_DP.py
+-rw-r--r--   0 monali     (501) staff       (20)    12479 2023-02-20 17:08:48.000000 insituTEM-0.1.4/insituTEM/insitu_IO.py
+-rw-r--r--   0 monali     (501) staff       (20)     6070 2023-02-07 23:34:02.000000 insituTEM-0.1.4/insituTEM/insitu_Preprocess.py
+-rw-r--r--   0 monali     (501) staff       (20)     8779 2023-02-20 21:40:28.000000 insituTEM-0.1.4/insituTEM/insitu_alignment.py
+drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:58:24.542622 insituTEM-0.1.4/insituTEM.egg-info/
+-rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 01:58:24.000000 insituTEM-0.1.4/insituTEM.egg-info/PKG-INFO
+-rw-r--r--   0 monali     (501) staff       (20)      303 2023-06-07 01:58:24.000000 insituTEM-0.1.4/insituTEM.egg-info/SOURCES.txt
+-rw-r--r--   0 monali     (501) staff       (20)        1 2023-06-07 01:58:24.000000 insituTEM-0.1.4/insituTEM.egg-info/dependency_links.txt
+-rw-r--r--   0 monali     (501) staff       (20)       59 2023-06-07 01:58:24.000000 insituTEM-0.1.4/insituTEM.egg-info/requires.txt
+-rw-r--r--   0 monali     (501) staff       (20)       10 2023-06-07 01:58:24.000000 insituTEM-0.1.4/insituTEM.egg-info/top_level.txt
+-rw-r--r--   0 monali     (501) staff       (20)       38 2023-06-07 01:58:24.543095 insituTEM-0.1.4/setup.cfg
+-rw-r--r--   0 monali     (501) staff       (20)      366 2023-06-07 01:58:11.000000 insituTEM-0.1.4/setup.py
```

### Comparing `insituTEM-0.1.3/insituTEM/insitu_DP.py` & `insituTEM-0.1.4/insituTEM/insitu_DP.py`

 * *Files identical despite different names*

### Comparing `insituTEM-0.1.3/insituTEM/insitu_IO.py` & `insituTEM-0.1.4/insituTEM/insitu_IO.py`

 * *Files identical despite different names*

### Comparing `insituTEM-0.1.3/insituTEM/insitu_Preprocess.py` & `insituTEM-0.1.4/insituTEM/insitu_Preprocess.py`

 * *Files identical despite different names*

### Comparing `insituTEM-0.1.3/insituTEM/insitu_alignment.py` & `insituTEM-0.1.4/insituTEM/insitu_alignment.py`

 * *Files identical despite different names*

