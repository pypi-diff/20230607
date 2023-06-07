# Comparing `tmp/basicqiwip2p-0.0.1.tar.gz` & `tmp/basicqiwip2p-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicqiwip2p-0.0.1.tar", last modified: Wed Jun  7 20:39:39 2023, max compression
+gzip compressed data, was "basicqiwip2p-0.0.2.tar", last modified: Wed Jun  7 20:44:35 2023, max compression
```

## Comparing `basicqiwip2p-0.0.1.tar` & `basicqiwip2p-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 20:39:39.378468 basicqiwip2p-0.0.1/
--rw-rw-rw-   0        0        0      194 2023-06-07 20:39:39.379614 basicqiwip2p-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-07 20:00:29.000000 basicqiwip2p-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 20:39:39.314112 basicqiwip2p-0.0.1/basicqiwip2p/
--rw-rw-rw-   0        0        0      133 2023-06-07 20:28:42.000000 basicqiwip2p-0.0.1/basicqiwip2p/__init__.py
--rw-rw-rw-   0        0        0     1880 2023-06-07 20:31:15.000000 basicqiwip2p-0.0.1/basicqiwip2p/aiobasicqiwip2p.py
--rw-rw-rw-   0        0        0     1814 2023-06-07 20:21:24.000000 basicqiwip2p-0.0.1/basicqiwip2p/basicqiwip2p.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:39:39.365058 basicqiwip2p-0.0.1/basicqiwip2p.egg-info/
--rw-rw-rw-   0        0        0      194 2023-06-07 20:39:38.000000 basicqiwip2p-0.0.1/basicqiwip2p.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-07 20:39:39.000000 basicqiwip2p-0.0.1/basicqiwip2p.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 20:39:38.000000 basicqiwip2p-0.0.1/basicqiwip2p.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-07 20:39:38.000000 basicqiwip2p-0.0.1/basicqiwip2p.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-07 20:39:38.000000 basicqiwip2p-0.0.1/basicqiwip2p.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 20:39:39.384179 basicqiwip2p-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      339 2023-06-07 20:33:05.000000 basicqiwip2p-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:44:35.234386 basicqiwip2p-0.0.2/
+-rw-rw-rw-   0        0        0      194 2023-06-07 20:44:35.235782 basicqiwip2p-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-07 20:00:29.000000 basicqiwip2p-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 20:44:35.191832 basicqiwip2p-0.0.2/basicqiwip2p/
+-rw-rw-rw-   0        0        0      159 2023-06-07 20:43:26.000000 basicqiwip2p-0.0.2/basicqiwip2p/__init__.py
+-rw-rw-rw-   0        0        0     1880 2023-06-07 20:31:15.000000 basicqiwip2p-0.0.2/basicqiwip2p/aiobasicqiwip2p.py
+-rw-rw-rw-   0        0        0     1814 2023-06-07 20:21:24.000000 basicqiwip2p-0.0.2/basicqiwip2p/basicqiwip2p.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:44:35.232164 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/
+-rw-rw-rw-   0        0        0      194 2023-06-07 20:44:34.000000 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-07 20:44:34.000000 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 20:44:34.000000 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-07 20:39:38.000000 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-07 20:44:34.000000 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 20:44:35.250935 basicqiwip2p-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      339 2023-06-07 20:44:15.000000 basicqiwip2p-0.0.2/setup.py
```

### Comparing `basicqiwip2p-0.0.1/basicqiwip2p/aiobasicqiwip2p.py` & `basicqiwip2p-0.0.2/basicqiwip2p/aiobasicqiwip2p.py`

 * *Files identical despite different names*

### Comparing `basicqiwip2p-0.0.1/basicqiwip2p/basicqiwip2p.py` & `basicqiwip2p-0.0.2/basicqiwip2p/basicqiwip2p.py`

 * *Files identical despite different names*

