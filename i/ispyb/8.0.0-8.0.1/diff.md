# Comparing `tmp/ispyb-8.0.0.tar.gz` & `tmp/ispyb-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ispyb-8.0.0.tar", last modified: Mon May 15 10:42:05 2023, max compression
+gzip compressed data, was "ispyb-8.0.1.tar", last modified: Wed Jun  7 15:35:34 2023, max compression
```

## Comparing `ispyb-8.0.0.tar` & `ispyb-8.0.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.878270 ispyb-8.0.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     9479 2023-05-15 10:41:58.000000 ispyb-8.0.0/HISTORY.rst
--rw-r--r--   0 vsts      (1001) docker     (122)    11362 2023-05-15 10:41:58.000000 ispyb-8.0.0/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (122)      119 2023-05-15 10:41:58.000000 ispyb-8.0.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1236 2023-05-15 10:42:05.878270 ispyb-8.0.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3601 2023-05-15 10:41:58.000000 ispyb-8.0.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.874270 ispyb-8.0.0/bin/
--rwxr-xr-x   0 vsts      (1001) docker     (122)     4623 2023-05-15 10:41:58.000000 ispyb-8.0.0/bin/dimple2ispyb.py
--rwxr-xr-x   0 vsts      (1001) docker     (122)     1651 2023-05-15 10:41:58.000000 ispyb-8.0.0/bin/mxdatareduction2ispyb.py
--rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-05-15 10:41:58.000000 ispyb-8.0.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     2006 2023-05-15 10:42:05.878270 ispyb-8.0.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)       69 2023-05-15 10:41:58.000000 ispyb-8.0.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.874270 ispyb-8.0.0/src/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.874270 ispyb-8.0.0/src/ispyb/
--rw-r--r--   0 vsts      (1001) docker     (122)     2741 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.874270 ispyb-8.0.0/src/ispyb/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16685 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/cli/job.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6047 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/cli/last_data_collections_on.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.874270 ispyb-8.0.0/src/ispyb/connector/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/connector/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.878270 ispyb-8.0.0/src/ispyb/connector/mysqlsp/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/connector/mysqlsp/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6011 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/connector/mysqlsp/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.878270 ispyb-8.0.0/src/ispyb/connector/ws/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/connector/ws/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      516 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/connector/ws/main.py
--rw-r--r--   0 vsts      (1001) docker     (122)      706 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/factory.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.878270 ispyb-8.0.0/src/ispyb/interface/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/interface/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      526 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/interface/acquisition.py
--rw-r--r--   0 vsts      (1001) docker     (122)      754 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/interface/connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2080 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/interface/core.py
--rw-r--r--   0 vsts      (1001) docker     (122)      287 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/interface/dataarea.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1516 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/interface/factory.py
--rw-r--r--   0 vsts      (1001) docker     (122)      320 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/interface/processing.py
--rw-r--r--   0 vsts      (1001) docker     (122)      668 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/interface/screening.py
--rw-r--r--   0 vsts      (1001) docker     (122)       77 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/interface/shipping.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.878270 ispyb-8.0.0/src/ispyb/sp/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/sp/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7310 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/sp/acquisition.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9383 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/sp/core.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7883 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/sp/emacquisition.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8734 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/sp/mxacquisition.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13646 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/sp/mxprocessing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6880 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/sp/mxscreening.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2786 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/sp/shipping.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4167 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/sp/xtalimaging.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.878270 ispyb-8.0.0/src/ispyb/sqlalchemy/
--rw-r--r--   0 vsts      (1001) docker     (122)     5068 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/sqlalchemy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)   209812 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/sqlalchemy/_auto_db_schema.py
--rw-r--r--   0 vsts      (1001) docker     (122)      821 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/strictordereddict.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.878270 ispyb-8.0.0/src/ispyb/ws/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/ws/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13124 2023-05-15 10:41:58.000000 ispyb-8.0.0/src/ispyb/xmltools.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-15 10:42:05.874270 ispyb-8.0.0/src/ispyb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1236 2023-05-15 10:42:05.000000 ispyb-8.0.0/src/ispyb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-05-15 10:42:05.000000 ispyb-8.0.0/src/ispyb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-15 10:42:05.000000 ispyb-8.0.0/src/ispyb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      271 2023-05-15 10:42:05.000000 ispyb-8.0.0/src/ispyb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       53 2023-05-15 10:42:05.000000 ispyb-8.0.0/src/ispyb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-05-15 10:42:05.000000 ispyb-8.0.0/src/ispyb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.465050 ispyb-8.0.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9633 2023-06-07 15:35:23.000000 ispyb-8.0.1/HISTORY.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    11362 2023-06-07 15:35:23.000000 ispyb-8.0.1/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      119 2023-06-07 15:35:23.000000 ispyb-8.0.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1236 2023-06-07 15:35:34.465050 ispyb-8.0.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3601 2023-06-07 15:35:23.000000 ispyb-8.0.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.457050 ispyb-8.0.1/bin/
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     4623 2023-06-07 15:35:23.000000 ispyb-8.0.1/bin/dimple2ispyb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1651 2023-06-07 15:35:23.000000 ispyb-8.0.1/bin/mxdatareduction2ispyb.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-06-07 15:35:23.000000 ispyb-8.0.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1942 2023-06-07 15:35:34.465050 ispyb-8.0.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)       69 2023-06-07 15:35:23.000000 ispyb-8.0.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.457050 ispyb-8.0.1/src/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.461050 ispyb-8.0.1/src/ispyb/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2741 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.461050 ispyb-8.0.1/src/ispyb/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16685 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/cli/job.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6047 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/cli/last_data_collections_on.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.461050 ispyb-8.0.1/src/ispyb/connector/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/connector/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.461050 ispyb-8.0.1/src/ispyb/connector/mysqlsp/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/connector/mysqlsp/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6011 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/connector/mysqlsp/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.461050 ispyb-8.0.1/src/ispyb/connector/ws/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/connector/ws/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      516 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/connector/ws/main.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      706 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/factory.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.461050 ispyb-8.0.1/src/ispyb/interface/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/interface/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      526 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/interface/acquisition.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      754 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/interface/connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2080 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/interface/core.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      287 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/interface/dataarea.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1516 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/interface/factory.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      320 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/interface/processing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      668 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/interface/screening.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       77 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/interface/shipping.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.465050 ispyb-8.0.1/src/ispyb/sp/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/sp/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7310 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/sp/acquisition.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9383 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/sp/core.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7883 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/sp/emacquisition.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8734 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/sp/mxacquisition.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13646 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/sp/mxprocessing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6880 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/sp/mxscreening.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2786 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/sp/shipping.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4167 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/sp/xtalimaging.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.465050 ispyb-8.0.1/src/ispyb/sqlalchemy/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5068 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/sqlalchemy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   209812 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/sqlalchemy/_auto_db_schema.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      821 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/strictordereddict.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.465050 ispyb-8.0.1/src/ispyb/ws/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/ws/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13124 2023-06-07 15:35:23.000000 ispyb-8.0.1/src/ispyb/xmltools.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 15:35:34.461050 ispyb-8.0.1/src/ispyb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1236 2023-06-07 15:35:34.000000 ispyb-8.0.1/src/ispyb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-06-07 15:35:34.000000 ispyb-8.0.1/src/ispyb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-07 15:35:34.000000 ispyb-8.0.1/src/ispyb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      271 2023-06-07 15:35:34.000000 ispyb-8.0.1/src/ispyb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       53 2023-06-07 15:35:34.000000 ispyb-8.0.1/src/ispyb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-06-07 15:35:34.000000 ispyb-8.0.1/src/ispyb.egg-info/top_level.txt
```

### Comparing `ispyb-8.0.0/HISTORY.rst` & `ispyb-8.0.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 =======
 History
 =======
 
 Unreleased / main
 -------------------
 
+8.0.1 (2023-06-07)
+-------------------
+* Require ``mysql-connector-python>=8.0.32`` (`#203 <https://github.com/DiamondLightSource/ispyb-api/pull/203>`_)
+
 8.0.0 (2023-05-15)
 -------------------
 * Update SQLAlchemy ORM models for ispyb-database v2.0.0
 * Remove ``mxacquisition.upsert_xray_centring_result`` (stored procedure removed in ispyb-database v2.0.0)
 
 7.2.0 (2023-03-02)
 -------------------
```

### Comparing `ispyb-8.0.0/LICENSE.md` & `ispyb-8.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/PKG-INFO` & `ispyb-8.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ispyb
-Version: 8.0.0
+Version: 8.0.1
 Summary: Python package to access ISPyB database
 Home-page: UNKNOWN
 Author: Diamond Light Source
 Author-email: scientificsoftware@diamond.ac.uk
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://ispyb.readthedocs.io
 Project-URL: GitHub, https://github.com/DiamondLightSource/ispyb-api
```

### Comparing `ispyb-8.0.0/README.md` & `ispyb-8.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/bin/dimple2ispyb.py` & `ispyb-8.0.1/bin/dimple2ispyb.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/bin/mxdatareduction2ispyb.py` & `ispyb-8.0.1/bin/mxdatareduction2ispyb.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/setup.cfg` & `ispyb-8.0.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ispyb
-version = 8.0.0
+version = 8.0.1
 description = Python package to access ISPyB database
 description-file = README.md
 long_description = This package provides a Python interface to ISPyB. It can access the ISPyB database directly or (in future versions) run on top of the official ISPyB webservices API.
 author = Diamond Light Source
 author_email = scientificsoftware@diamond.ac.uk
 license = Apache License, Version 2.0
 classifiers = 
@@ -25,15 +25,15 @@
 	Documentation = https://ispyb.readthedocs.io
 	GitHub = https://github.com/DiamondLightSource/ispyb-api
 	Bug-Tracker = https://github.com/DiamondLightSource/ispyb-api/issues
 
 [options]
 include_package_data = True
 install_requires = 
-	mysql-connector-python<=8.0.29 #See https://github.com/DiamondLightSource/ispyb-api/issues/183
+	mysql-connector-python>=8.0.32
 	sqlalchemy<2
 	tabulate
 packages = find:
 package_dir = 
 	=src
 python_requires = >=3.7
 scripts =
```

### Comparing `ispyb-8.0.0/src/ispyb/__init__.py` & `ispyb-8.0.1/src/ispyb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import configparser
 import logging
 import os
 import warnings
 
-__version__ = "8.0.0"
+__version__ = "8.0.1"
 
 _log = logging.getLogger("ispyb")
 
 
 def open(credentials=None, configuration_file=None):
     """Create an ISPyB connection.
```

### Comparing `ispyb-8.0.0/src/ispyb/cli/job.py` & `ispyb-8.0.1/src/ispyb/cli/job.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/cli/last_data_collections_on.py` & `ispyb-8.0.1/src/ispyb/cli/last_data_collections_on.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/connector/mysqlsp/main.py` & `ispyb-8.0.1/src/ispyb/connector/mysqlsp/main.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/connector/ws/main.py` & `ispyb-8.0.1/src/ispyb/connector/ws/main.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/factory.py` & `ispyb-8.0.1/src/ispyb/factory.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/interface/acquisition.py` & `ispyb-8.0.1/src/ispyb/interface/acquisition.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/interface/connection.py` & `ispyb-8.0.1/src/ispyb/interface/connection.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/interface/core.py` & `ispyb-8.0.1/src/ispyb/interface/core.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/interface/factory.py` & `ispyb-8.0.1/src/ispyb/interface/factory.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/interface/screening.py` & `ispyb-8.0.1/src/ispyb/interface/screening.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/sp/acquisition.py` & `ispyb-8.0.1/src/ispyb/sp/acquisition.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/sp/core.py` & `ispyb-8.0.1/src/ispyb/sp/core.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/sp/emacquisition.py` & `ispyb-8.0.1/src/ispyb/sp/emacquisition.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/sp/mxacquisition.py` & `ispyb-8.0.1/src/ispyb/sp/mxacquisition.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/sp/mxprocessing.py` & `ispyb-8.0.1/src/ispyb/sp/mxprocessing.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/sp/mxscreening.py` & `ispyb-8.0.1/src/ispyb/sp/mxscreening.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/sp/shipping.py` & `ispyb-8.0.1/src/ispyb/sp/shipping.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/sp/xtalimaging.py` & `ispyb-8.0.1/src/ispyb/sp/xtalimaging.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/sqlalchemy/__init__.py` & `ispyb-8.0.1/src/ispyb/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/sqlalchemy/_auto_db_schema.py` & `ispyb-8.0.1/src/ispyb/sqlalchemy/_auto_db_schema.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/strictordereddict.py` & `ispyb-8.0.1/src/ispyb/strictordereddict.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb/xmltools.py` & `ispyb-8.0.1/src/ispyb/xmltools.py`

 * *Files identical despite different names*

### Comparing `ispyb-8.0.0/src/ispyb.egg-info/PKG-INFO` & `ispyb-8.0.1/src/ispyb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ispyb
-Version: 8.0.0
+Version: 8.0.1
 Summary: Python package to access ISPyB database
 Home-page: UNKNOWN
 Author: Diamond Light Source
 Author-email: scientificsoftware@diamond.ac.uk
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://ispyb.readthedocs.io
 Project-URL: GitHub, https://github.com/DiamondLightSource/ispyb-api
```

### Comparing `ispyb-8.0.0/src/ispyb.egg-info/SOURCES.txt` & `ispyb-8.0.1/src/ispyb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

