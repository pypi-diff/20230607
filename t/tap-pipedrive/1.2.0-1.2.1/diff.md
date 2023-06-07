# Comparing `tmp/tap-pipedrive-1.2.0.tar.gz` & `tmp/tap-pipedrive-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-pipedrive-1.2.0.tar", last modified: Tue Apr 25 13:06:09 2023, max compression
+gzip compressed data, was "dist/tap-pipedrive-1.2.1.tar", last modified: Wed Jun  7 05:16:17 2023, max compression
```

## Comparing `tap-pipedrive-1.2.0.tar` & `tap-pipedrive-1.2.1.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/MANIFEST.in
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      696 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/deal_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      411 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/deal_products.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      193 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/notes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      278 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/filters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      275 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/stages.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/files.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      762 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/users.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      521 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/products.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/notes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/organizations.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1520 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/deals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1377 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/persons.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3590 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/activities.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1221 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/currencies.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      298 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/activity_types.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      748 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/dealflow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/pipelines.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      988 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6582 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/stream.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      756 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/stages.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/deal_fields.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      659 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/dealflow.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      683 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/filters.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3740 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/persons.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2238 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/activities.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/notes.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1685 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/products.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/deals.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3402 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/organizations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1876 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/files.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1405 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/users.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      678 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/activity_types.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/pipelines.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      444 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/currency.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1759 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/deal_products.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16806 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.0/tap_pipedrive/tap.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      817 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.0/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1536 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      696 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/deal_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      411 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/deal_products.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      193 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/notes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      278 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/filters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      275 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/stages.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/files.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      762 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/users.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      521 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/products.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/notes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/organizations.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1520 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/deals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1377 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/persons.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3590 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/activities.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1221 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/currencies.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      298 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/activity_types.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      748 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/dealflow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/streams/pipelines.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1166 2023-06-07 04:53:20.000000 tap-pipedrive-1.2.1/tap_pipedrive/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6582 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/stream.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      756 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/stages.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/deal_fields.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      659 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/dealflow.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      683 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/filters.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 05:16:17.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3740 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/persons.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2238 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/activities.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/notes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1685 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/deals.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3402 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/organizations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1876 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/files.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1405 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      678 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/activity_types.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/pipelines.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      444 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/currency.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1759 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/schemas/deal_products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/tap_pipedrive/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17209 2023-06-07 04:53:20.000000 tap-pipedrive-1.2.1/tap_pipedrive/tap.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      817 2023-06-07 04:53:20.000000 tap-pipedrive-1.2.1/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.1/LICENSE
```

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive.egg-info/SOURCES.txt` & `tap-pipedrive-1.2.1/tap_pipedrive.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 MANIFEST.in
-README.md
 setup.py
 tap_pipedrive/__init__.py
 tap_pipedrive/cli.py
 tap_pipedrive/config.py
 tap_pipedrive/exceptions.py
 tap_pipedrive/stream.py
 tap_pipedrive/tap.py
```

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/cli.py` & `tap-pipedrive-1.2.1/tap_pipedrive/cli.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/users.py` & `tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/users.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/products.py` & `tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/products.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/notes.py` & `tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/notes.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/organizations.py` & `tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/organizations.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/deals.py` & `tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/deals.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/persons.py` & `tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/persons.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/__init__.py` & `tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/activities.py` & `tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/dynamic_typing/activities.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/__init__.py` & `tap-pipedrive-1.2.1/tap_pipedrive/streams/recents/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/streams/__init__.py` & `tap-pipedrive-1.2.1/tap_pipedrive/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/streams/dealflow.py` & `tap-pipedrive-1.2.1/tap_pipedrive/streams/dealflow.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/exceptions.py` & `tap-pipedrive-1.2.1/tap_pipedrive/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 class PipedriveError(Exception):
     def __init__(self, message=None, response=None):
         super().__init__(message)
         self.message = message
         self.response = response
 
+# Reference: https://pipedrive.readme.io/docs/core-api-concepts-http-status-codes
+class Pipedrive5xxError(PipedriveError):
+    pass
+
 class PipedriveNotFoundError(PipedriveError):
     pass
 
 class PipedriveBadRequestError(PipedriveError):
     pass
 
 class PipedriveUnauthorizedError(PipedriveError):
@@ -32,15 +36,15 @@
 
 class PipedriveTooManyRequestsError(PipedriveError):
     pass
 
 class PipedriveTooManyRequestsInSecondError(PipedriveError):
     pass
 
-class PipedriveInternalServiceError(PipedriveError):
+class PipedriveInternalServiceError(Pipedrive5xxError): # 500 error
     pass
 
-class PipedriveNotImplementedError(PipedriveError):
+class PipedriveNotImplementedError(Pipedrive5xxError): # 501 error
     pass
 
-class PipedriveServiceUnavailableError(PipedriveError):
+class PipedriveServiceUnavailableError(Pipedrive5xxError): # 503 error
     pass
```

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/stream.py` & `tap-pipedrive-1.2.1/tap_pipedrive/stream.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/stages.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/stages.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/deal_fields.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/deal_fields.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/dealflow.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/dealflow.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/filters.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/filters.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/persons.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/persons.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/activities.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/activities.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/notes.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/notes.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/products.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/products.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/deals.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/deals.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/organizations.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/dynamic_typing/organizations.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/files.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/files.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/users.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/recents/users.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/activity_types.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/activity_types.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/pipelines.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/pipelines.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/schemas/deal_products.json` & `tap-pipedrive-1.2.1/tap_pipedrive/schemas/deal_products.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.2.0/tap_pipedrive/tap.py` & `tap-pipedrive-1.2.1/tap_pipedrive/tap.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from requests.exceptions import ConnectionError, RequestException, Timeout
 from json import JSONDecodeError
 from singer import set_currently_syncing, metadata
 from singer.catalog import Catalog, CatalogEntry, Schema
 from .config import BASE_URL, CONFIG_DEFAULTS
 from .exceptions import (PipedriveError, PipedriveNotFoundError, PipedriveBadRequestError, PipedriveUnauthorizedError, PipedrivePaymentRequiredError, 
                         PipedriveForbiddenError, PipedriveGoneError, PipedriveUnsupportedMediaError, PipedriveUnprocessableEntityError, PipedriveTooManyRequestsError, 
-                        PipedriveTooManyRequestsInSecondError,PipedriveInternalServiceError, PipedriveNotImplementedError, PipedriveServiceUnavailableError)
+                        PipedriveTooManyRequestsInSecondError,PipedriveInternalServiceError, PipedriveNotImplementedError, PipedriveServiceUnavailableError, Pipedrive5xxError)
 from .streams import (CurrenciesStream, ActivityTypesStream, FiltersStream, StagesStream, PipelinesStream,
                       RecentNotesStream, RecentUsersStream, RecentActivitiesStream, RecentDealsStream,
                       RecentFilesStream, RecentOrganizationsStream, RecentPersonsStream, RecentProductsStream,
                       DealStageChangeStream, DealsProductsStream, DealFields)
 
 
 logger = singer.get_logger()
@@ -296,16 +296,16 @@
         params = {
             'start': stream.start,
             'limit': stream.limit
         }
         params = stream.update_request_params(params)
         return self.execute_request(stream.endpoint, params=params)
 
-    @backoff.on_exception(backoff.expo, (Timeout, ConnectionError, PipedriveNull200Error), max_tries = 5, factor = 2)
-    @backoff.on_exception(backoff.expo, (PipedriveInternalServiceError, simplejson.scanner.JSONDecodeError), max_tries = 3)
+    @backoff.on_exception(backoff.expo, (Timeout, Pipedrive5xxError, ConnectionError, PipedriveNull200Error), max_tries=5, factor=2)
+    @backoff.on_exception(backoff.expo, simplejson.scanner.JSONDecodeError, max_tries=3)
     @backoff.on_exception(retry_after_wait_gen, (PipedriveTooManyRequestsInSecondError, PipedriveBadRequestError), giveup=is_not_status_code_fn([429]), jitter=None, max_tries=3)
     def execute_request(self, endpoint, params=None):
         headers = {
             'User-Agent': self.config['user-agent'],
             'Accept-Encoding': 'application/json'
         }
         _params = {
@@ -384,11 +384,18 @@
                 except Exception:
                     json_resp = {}
 
                 message_text = json_resp.get("error", ERROR_CODE_EXCEPTION_MAPPING.get(error_code, {}).get("message", "Unknown Error"))
                 message = "HTTP-error-code: {}, Error: {}".format(error_code, message_text)
 
             exc = ERROR_CODE_EXCEPTION_MAPPING.get(error_code, {}).get("raise_exception", PipedriveError)
+
+            # Pipedrive doc has only mentioned 500, 501 and 503 errors but while executing
+            # we encounter errors apart form the doc like 524 error. So handling the same
+            #   Doc: https://pipedrive.readme.io/docs/core-api-concepts-http-status-codes
+            if error_code > 500 and error_code not in ERROR_CODE_EXCEPTION_MAPPING.keys():
+                exc = Pipedrive5xxError
+
             raise exc(message, response) from None
 
         except (ValueError, TypeError):
             raise PipedriveError(error) from None
```

### Comparing `tap-pipedrive-1.2.0/setup.py` & `tap-pipedrive-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name="tap-pipedrive",
-      version="1.2.0",
+      version="1.2.1",
       description="Singer.io tap for extracting data from the Pipedrive API",
       author="Stitch",
       author_email="dev@stitchdata.com",
       url="http://singer.io",
       classifiers=["Programming Language :: Python :: 3 :: Only"],
       py_modules=["tap_pipedrive"],
       install_requires=[
```

### Comparing `tap-pipedrive-1.2.0/LICENSE` & `tap-pipedrive-1.2.1/LICENSE`

 * *Files identical despite different names*

