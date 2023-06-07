# Comparing `tmp/pikanetwork.py-0.0.1.tar.gz` & `tmp/pikanetwork.py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikanetwork.py-0.0.1.tar", last modified: Wed Jun  7 11:55:41 2023, max compression
+gzip compressed data, was "pikanetwork.py-0.0.2.tar", last modified: Wed Jun  7 12:48:27 2023, max compression
```

## Comparing `pikanetwork.py-0.0.1.tar` & `pikanetwork.py-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 11:55:41.806462 pikanetwork.py-0.0.1/
--rw-rw-rw-   0        0        0     1070 2023-06-07 11:42:00.000000 pikanetwork.py-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      144 2023-06-07 11:55:41.805463 pikanetwork.py-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1531 2023-06-07 11:49:13.000000 pikanetwork.py-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 11:55:41.793159 pikanetwork.py-0.0.1/pikanetwork/
--rw-rw-rw-   0        0        0      311 2023-06-07 11:26:13.000000 pikanetwork.py-0.0.1/pikanetwork/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-07 11:49:13.000000 pikanetwork.py-0.0.1/pikanetwork/api.py
--rw-rw-rw-   0        0        0     2481 2023-06-07 11:27:56.000000 pikanetwork.py-0.0.1/pikanetwork/builders.py
--rw-rw-rw-   0        0        0     1747 2023-06-07 10:59:44.000000 pikanetwork.py-0.0.1/pikanetwork/models.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:55:41.802463 pikanetwork.py-0.0.1/pikanetwork.py.egg-info/
--rw-rw-rw-   0        0        0      144 2023-06-07 11:55:41.000000 pikanetwork.py-0.0.1/pikanetwork.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-07 11:55:41.000000 pikanetwork.py-0.0.1/pikanetwork.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 11:55:41.000000 pikanetwork.py-0.0.1/pikanetwork.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 11:55:41.000000 pikanetwork.py-0.0.1/pikanetwork.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 11:55:41.806462 pikanetwork.py-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      197 2023-06-07 11:52:49.000000 pikanetwork.py-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:48:27.254301 pikanetwork.py-0.0.2/
+-rw-rw-rw-   0        0        0     1070 2023-06-07 11:42:00.000000 pikanetwork.py-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1776 2023-06-07 12:48:27.252293 pikanetwork.py-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1531 2023-06-07 11:49:13.000000 pikanetwork.py-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 12:48:27.241297 pikanetwork.py-0.0.2/pikanetwork/
+-rw-rw-rw-   0        0        0      311 2023-06-07 11:26:13.000000 pikanetwork.py-0.0.2/pikanetwork/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-07 11:49:13.000000 pikanetwork.py-0.0.2/pikanetwork/api.py
+-rw-rw-rw-   0        0        0     2481 2023-06-07 11:27:56.000000 pikanetwork.py-0.0.2/pikanetwork/builders.py
+-rw-rw-rw-   0        0        0     1747 2023-06-07 10:59:44.000000 pikanetwork.py-0.0.2/pikanetwork/models.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:48:27.249293 pikanetwork.py-0.0.2/pikanetwork.py.egg-info/
+-rw-rw-rw-   0        0        0     1776 2023-06-07 12:48:27.000000 pikanetwork.py-0.0.2/pikanetwork.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-07 12:48:27.000000 pikanetwork.py-0.0.2/pikanetwork.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 12:48:27.000000 pikanetwork.py-0.0.2/pikanetwork.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 12:48:27.000000 pikanetwork.py-0.0.2/pikanetwork.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 12:48:27.256297 pikanetwork.py-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      478 2023-06-07 12:47:45.000000 pikanetwork.py-0.0.2/setup.py
```

### Comparing `pikanetwork.py-0.0.1/LICENSE` & `pikanetwork.py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pikanetwork.py-0.0.1/README.md` & `pikanetwork.py-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pikanetwork.py-0.0.1/pikanetwork/api.py` & `pikanetwork.py-0.0.2/pikanetwork/api.py`

 * *Files identical despite different names*

### Comparing `pikanetwork.py-0.0.1/pikanetwork/builders.py` & `pikanetwork.py-0.0.2/pikanetwork/builders.py`

 * *Files identical despite different names*

### Comparing `pikanetwork.py-0.0.1/pikanetwork/models.py` & `pikanetwork.py-0.0.2/pikanetwork/models.py`

 * *Files identical despite different names*

