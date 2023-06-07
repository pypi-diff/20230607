# Comparing `tmp/espnfantasyfootball-0.1.0.tar.gz` & `tmp/espnfantasyfootball-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espnfantasyfootball-0.1.0.tar", last modified: Wed Jun  7 00:07:34 2023, max compression
+gzip compressed data, was "espnfantasyfootball-0.1.1.tar", last modified: Wed Jun  7 15:24:25 2023, max compression
```

## Comparing `espnfantasyfootball-0.1.0.tar` & `espnfantasyfootball-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 timothybryan   (501) staff       (20)        0 2023-06-07 00:07:34.891363 espnfantasyfootball-0.1.0/
--rw-r--r--   0 timothybryan   (501) staff       (20)      250 2023-06-07 00:07:34.891078 espnfantasyfootball-0.1.0/PKG-INFO
--rw-r--r--   0 timothybryan   (501) staff       (20)     1599 2023-06-06 18:29:44.000000 espnfantasyfootball-0.1.0/README.md
-drwxr-xr-x   0 timothybryan   (501) staff       (20)        0 2023-06-07 00:07:34.887973 espnfantasyfootball-0.1.0/espnfantasyfootball/
--rw-r--r--   0 timothybryan   (501) staff       (20)        0 2023-06-06 18:36:55.000000 espnfantasyfootball-0.1.0/espnfantasyfootball/__init__.py
--rw-r--r--   0 timothybryan   (501) staff       (20)    12077 2023-06-06 18:29:44.000000 espnfantasyfootball-0.1.0/espnfantasyfootball/espnfantasyfootball.py
-drwxr-xr-x   0 timothybryan   (501) staff       (20)        0 2023-06-07 00:07:34.890358 espnfantasyfootball-0.1.0/espnfantasyfootball.egg-info/
--rw-r--r--   0 timothybryan   (501) staff       (20)      250 2023-06-07 00:07:34.000000 espnfantasyfootball-0.1.0/espnfantasyfootball.egg-info/PKG-INFO
--rw-r--r--   0 timothybryan   (501) staff       (20)      307 2023-06-07 00:07:34.000000 espnfantasyfootball-0.1.0/espnfantasyfootball.egg-info/SOURCES.txt
--rw-r--r--   0 timothybryan   (501) staff       (20)        1 2023-06-07 00:07:34.000000 espnfantasyfootball-0.1.0/espnfantasyfootball.egg-info/dependency_links.txt
--rw-r--r--   0 timothybryan   (501) staff       (20)       16 2023-06-07 00:07:34.000000 espnfantasyfootball-0.1.0/espnfantasyfootball.egg-info/requires.txt
--rw-r--r--   0 timothybryan   (501) staff       (20)       20 2023-06-07 00:07:34.000000 espnfantasyfootball-0.1.0/espnfantasyfootball.egg-info/top_level.txt
--rw-r--r--   0 timothybryan   (501) staff       (20)       38 2023-06-07 00:07:34.891491 espnfantasyfootball-0.1.0/setup.cfg
--rw-r--r--   0 timothybryan   (501) staff       (20)      355 2023-06-07 00:06:56.000000 espnfantasyfootball-0.1.0/setup.py
+drwxr-xr-x   0 timothybryan   (501) staff       (20)        0 2023-06-07 15:24:25.473152 espnfantasyfootball-0.1.1/
+-rw-r--r--   0 timothybryan   (501) staff       (20)      250 2023-06-07 15:24:25.472786 espnfantasyfootball-0.1.1/PKG-INFO
+-rw-r--r--   0 timothybryan   (501) staff       (20)     1599 2023-06-06 18:29:44.000000 espnfantasyfootball-0.1.1/README.md
+drwxr-xr-x   0 timothybryan   (501) staff       (20)        0 2023-06-07 15:24:25.469079 espnfantasyfootball-0.1.1/espnfantasyfootball/
+-rw-r--r--   0 timothybryan   (501) staff       (20)      166 2023-06-07 14:56:28.000000 espnfantasyfootball-0.1.1/espnfantasyfootball/__init__.py
+-rw-r--r--   0 timothybryan   (501) staff       (20)    12077 2023-06-06 18:29:44.000000 espnfantasyfootball-0.1.1/espnfantasyfootball/espnfantasyfootball.py
+drwxr-xr-x   0 timothybryan   (501) staff       (20)        0 2023-06-07 15:24:25.472033 espnfantasyfootball-0.1.1/espnfantasyfootball.egg-info/
+-rw-r--r--   0 timothybryan   (501) staff       (20)      250 2023-06-07 15:24:25.000000 espnfantasyfootball-0.1.1/espnfantasyfootball.egg-info/PKG-INFO
+-rw-r--r--   0 timothybryan   (501) staff       (20)      307 2023-06-07 15:24:25.000000 espnfantasyfootball-0.1.1/espnfantasyfootball.egg-info/SOURCES.txt
+-rw-r--r--   0 timothybryan   (501) staff       (20)        1 2023-06-07 15:24:25.000000 espnfantasyfootball-0.1.1/espnfantasyfootball.egg-info/dependency_links.txt
+-rw-r--r--   0 timothybryan   (501) staff       (20)       16 2023-06-07 15:24:25.000000 espnfantasyfootball-0.1.1/espnfantasyfootball.egg-info/requires.txt
+-rw-r--r--   0 timothybryan   (501) staff       (20)       20 2023-06-07 15:24:25.000000 espnfantasyfootball-0.1.1/espnfantasyfootball.egg-info/top_level.txt
+-rw-r--r--   0 timothybryan   (501) staff       (20)       38 2023-06-07 15:24:25.473266 espnfantasyfootball-0.1.1/setup.cfg
+-rw-r--r--   0 timothybryan   (501) staff       (20)      355 2023-06-07 15:24:08.000000 espnfantasyfootball-0.1.1/setup.py
```

### Comparing `espnfantasyfootball-0.1.0/README.md` & `espnfantasyfootball-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `espnfantasyfootball-0.1.0/espnfantasyfootball/espnfantasyfootball.py` & `espnfantasyfootball-0.1.1/espnfantasyfootball/espnfantasyfootball.py`

 * *Files identical despite different names*

