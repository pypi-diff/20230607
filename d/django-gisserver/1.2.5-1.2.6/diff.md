# Comparing `tmp/django-gisserver-1.2.5.tar.gz` & `tmp/django-gisserver-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-gisserver-1.2.5.tar", last modified: Wed Jan 11 09:33:57 2023, max compression
+gzip compressed data, was "django-gisserver-1.2.6.tar", last modified: Wed Jun  7 10:52:10 2023, max compression
```

## Comparing `django-gisserver-1.2.5.tar` & `django-gisserver-1.2.6.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/
--rw-rw-r--   0 lars      (1000) lars      (1000)    12806 2023-01-11 08:52:17.000000 django-gisserver-1.2.5/CHANGES.md
--rw-rw-r--   0 lars      (1000) lars      (1000)    16725 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/LICENSE
--rw-rw-r--   0 lars      (1000) lars      (1000)      227 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/MANIFEST.in
--rw-rw-r--   0 lars      (1000) lars      (1000)     5482 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/PKG-INFO
--rw-rw-r--   0 lars      (1000) lars      (1000)     4043 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/README.md
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.564056 django-gisserver-1.2.5/django_gisserver.egg-info/
--rw-rw-r--   0 lars      (1000) lars      (1000)     5482 2023-01-11 09:33:57.000000 django-gisserver-1.2.5/django_gisserver.egg-info/PKG-INFO
--rw-rw-r--   0 lars      (1000) lars      (1000)     1915 2023-01-11 09:33:57.000000 django-gisserver-1.2.5/django_gisserver.egg-info/SOURCES.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)        1 2023-01-11 09:33:57.000000 django-gisserver-1.2.5/django_gisserver.egg-info/dependency_links.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)        1 2023-01-11 09:33:57.000000 django-gisserver-1.2.5/django_gisserver.egg-info/not-zip-safe
--rw-rw-r--   0 lars      (1000) lars      (1000)      180 2023-01-11 09:33:57.000000 django-gisserver-1.2.5/django_gisserver.egg-info/requires.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)       10 2023-01-11 09:33:57.000000 django-gisserver-1.2.5/django_gisserver.egg-info/top_level.txt
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.564056 django-gisserver-1.2.5/gisserver/
--rw-rw-r--   0 lars      (1000) lars      (1000)       40 2023-01-11 08:52:36.000000 django-gisserver-1.2.5/gisserver/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     2108 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/conf.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     5329 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/db.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     4596 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/exceptions.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    32232 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/features.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    13066 2023-01-11 08:49:39.000000 django-gisserver-1.2.5/gisserver/geometries.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.564056 django-gisserver-1.2.5/gisserver/operations/
--rw-rw-r--   0 lars      (1000) lars      (1000)        0 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/operations/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    16697 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/operations/base.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    17941 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/operations/wfs20.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/gisserver/output/
--rw-rw-r--   0 lars      (1000) lars      (1000)     2048 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/output/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     7954 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/output/base.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     1542 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/output/buffer.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     6198 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/output/csv.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    11236 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/output/geojson.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    26899 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/output/gml32.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     9189 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/output/results.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     6113 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/output/utils.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     4603 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/output/xmlschema.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/gisserver/parsers/
--rw-rw-r--   0 lars      (1000) lars      (1000)      290 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     4864 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/base.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/gisserver/parsers/fes20/
--rw-rw-r--   0 lars      (1000) lars      (1000)      624 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/fes20/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     9747 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/fes20/expressions.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     3507 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/fes20/filters.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     8726 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/fes20/functions.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     2863 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/fes20/identifiers.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    23601 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/fes20/operators.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    10083 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/fes20/query.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     2176 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/fes20/sorting.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/gisserver/parsers/gml/
--rw-rw-r--   0 lars      (1000) lars      (1000)     1462 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/gml/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     1065 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/gml/base.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     3171 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/gml/geometries.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     3553 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/tags.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     1038 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/parsers/values.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/gisserver/queries/
--rw-rw-r--   0 lars      (1000) lars      (1000)      892 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/queries/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     7146 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/queries/adhoc.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     5943 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/queries/base.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     7095 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/queries/stored.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.564056 django-gisserver-1.2.5/gisserver/static/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/gisserver/static/gisserver/
--rw-rw-r--   0 lars      (1000) lars      (1000)      163 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/static/gisserver/index.css
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.564056 django-gisserver-1.2.5/gisserver/templates/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/gisserver/templates/gisserver/
--rw-rw-r--   0 lars      (1000) lars      (1000)      866 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/templates/gisserver/index.html
--rw-rw-r--   0 lars      (1000) lars      (1000)      993 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/templates/gisserver/service_description.html
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/2.0.0/
--rw-rw-r--   0 lars      (1000) lars      (1000)     1041 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml
--rw-rw-r--   0 lars      (1000) lars      (1000)     8675 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml
--rw-rw-r--   0 lars      (1000) lars      (1000)      636 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml
--rw-rw-r--   0 lars      (1000) lars      (1000)      538 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/feature_field.html
--rw-rw-r--   0 lars      (1000) lars      (1000)      788 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/feature_type.html
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/gisserver/templatetags/
--rw-rw-r--   0 lars      (1000) lars      (1000)        0 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/templatetags/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)      204 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/templatetags/gisserver_tags.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    34202 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/types.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    13252 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/gisserver/views.py
--rw-rw-r--   0 lars      (1000) lars      (1000)      496 2023-01-11 09:33:57.568056 django-gisserver-1.2.5/setup.cfg
--rwxrwxr-x   0 lars      (1000) lars      (1000)     2585 2023-01-11 08:47:11.000000 django-gisserver-1.2.5/setup.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.704781 django-gisserver-1.2.6/
+-rw-rw-r--   0 jan       (1000) jan       (1000)    12992 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/CHANGES.md
+-rw-rw-r--   0 jan       (1000) jan       (1000)    16725 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/LICENSE
+-rw-rw-r--   0 jan       (1000) jan       (1000)      227 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/MANIFEST.in
+-rw-rw-r--   0 jan       (1000) jan       (1000)     5369 2023-06-07 10:52:10.704781 django-gisserver-1.2.6/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4027 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/README.md
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.696781 django-gisserver-1.2.6/django_gisserver.egg-info/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     5369 2023-06-07 10:52:10.000000 django-gisserver-1.2.6/django_gisserver.egg-info/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1915 2023-06-07 10:52:10.000000 django-gisserver-1.2.6/django_gisserver.egg-info/SOURCES.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        1 2023-06-07 10:52:10.000000 django-gisserver-1.2.6/django_gisserver.egg-info/dependency_links.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        1 2022-09-07 10:15:14.000000 django-gisserver-1.2.6/django_gisserver.egg-info/not-zip-safe
+-rw-rw-r--   0 jan       (1000) jan       (1000)      180 2023-06-07 10:52:10.000000 django-gisserver-1.2.6/django_gisserver.egg-info/requires.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       10 2023-06-07 10:52:10.000000 django-gisserver-1.2.6/django_gisserver.egg-info/top_level.txt
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/
+-rw-rw-r--   0 jan       (1000) jan       (1000)       40 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2108 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/conf.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     5329 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/db.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4596 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/exceptions.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    32232 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/features.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    12619 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/geometries.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/operations/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/operations/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    16780 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/operations/base.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    18240 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/operations/wfs20.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/output/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1950 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     7954 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/base.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1542 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/buffer.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     6198 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/csv.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    11236 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/output/geojson.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    26913 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/gml32.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     9189 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/results.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     6113 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/utils.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4603 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/xmlschema.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/parsers/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      290 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4864 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/base.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/parsers/fes20/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      624 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     9747 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/expressions.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3507 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/filters.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     8726 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/functions.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2863 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/identifiers.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    23601 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/operators.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    10083 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/query.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2176 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/sorting.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/parsers/gml/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1462 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/gml/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1065 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/parsers/gml/base.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3171 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/gml/geometries.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3553 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/tags.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1038 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/parsers/values.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/queries/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      892 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/queries/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     7146 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/queries/adhoc.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     5943 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/queries/base.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     7095 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/queries/stored.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.696781 django-gisserver-1.2.6/gisserver/static/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/static/gisserver/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      163 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/static/gisserver/index.css
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.696781 django-gisserver-1.2.6/gisserver/templates/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/templates/gisserver/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      866 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/index.html
+-rw-rw-r--   0 jan       (1000) jan       (1000)      993 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/service_description.html
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1041 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml
+-rw-rw-r--   0 jan       (1000) jan       (1000)     8675 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml
+-rw-rw-r--   0 jan       (1000) jan       (1000)      636 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml
+-rw-rw-r--   0 jan       (1000) jan       (1000)      538 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/feature_field.html
+-rw-rw-r--   0 jan       (1000) jan       (1000)      788 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/feature_type.html
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.704781 django-gisserver-1.2.6/gisserver/templatetags/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templatetags/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      204 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templatetags/gisserver_tags.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    34202 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/types.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    13252 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/views.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      496 2023-06-07 10:52:10.704781 django-gisserver-1.2.6/setup.cfg
+-rwxrwxr-x   0 jan       (1000) jan       (1000)     2471 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/setup.py
```

### Comparing `django-gisserver-1.2.5/CHANGES.md` & `django-gisserver-1.2.6/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# 2023-06-07 (1.2.6)
+
+* Workaround for FME doing a DescribeFeatureType with the wrong outputformat.
+* Dropped support for Django versions < 3.2 and Python < 3.9.
+* Minor optimizations.
+
 # 2023-01-11 (1.2.5)
 
 * CRS parsing no longer raises SyntaxErrors.
 
 # 2022-11-01 (1.2.4)
 
 * Fixed type assertion when `django.contrib.postgres` was not installed.
```

### Comparing `django-gisserver-1.2.5/LICENSE` & `django-gisserver-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/PKG-INFO` & `django-gisserver-1.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 Metadata-Version: 2.1
 Name: django-gisserver
-Version: 1.2.5
+Version: 1.2.6
 Summary: Django speaking WFS 2.0 (exposing GeoDjango model fields)
 Home-page: https://github.com/amsterdam/django-gisserver
 Author: Diederik van der Boor
 Author-email: opensource@edoburu.nl
 License: Mozilla Public License 2.0
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires: Django (>=2.0)
+Requires: Django (>=3.2)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 [![Documentation](https://readthedocs.org/projects/django-gisserver/badge/?version=latest)](https://django-gisserver.readthedocs.io/en/latest/?badge=latest)
-[![Actions](https://github.com/django-fluent/django-fluent-contents/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/Amsterdam/django-gisserver/actions/workflows/tests.yaml)
+[![Actions](https://github.com/Amsterdam/django-gisserver/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/Amsterdam/django-gisserver/actions/workflows/tests.yaml)
 [![PyPI](https://img.shields.io/pypi/v/django-gisserver.svg)](https://pypi.python.org/pypi/django-gisserver)
 [![MPL License](https://img.shields.io/badge/license-MPL%202.0-blue.svg)](https://pypi.python.org/pypi/django-gisserver)
-[![Coverage](https://img.shields.io/codecov/c/github/amsterdam/django-gisserver/master.svg)](https://codecov.io/github/amsterdam/django-gisserver?branch=master)
+[![Coverage](https://img.shields.io/codecov/c/github/amsterdam/django-gisserver/main.svg)](https://codecov.io/github/amsterdam/django-gisserver?branch=main)
 
 # django-gisserver
 
 Django speaking WFS 2.0 to expose geo data.
 
 ## Features
 
@@ -155,7 +153,9 @@
 Much of this software is then published as Open Source so that other municipalities,
 organizations and citizens can use the software as a basis and inspiration to develop
 similar software themselves. The Municipality of Amsterdam considers it important that
 software developed with public money is also publicly available.
 
 This package is initially developed by the City of Amsterdam, but the tools
 and concepts created in this project can be used in any city.
+
+
```

### Comparing `django-gisserver-1.2.5/README.md` & `django-gisserver-1.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Documentation](https://readthedocs.org/projects/django-gisserver/badge/?version=latest)](https://django-gisserver.readthedocs.io/en/latest/?badge=latest)
-[![Actions](https://github.com/django-fluent/django-fluent-contents/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/Amsterdam/django-gisserver/actions/workflows/tests.yaml)
+[![Actions](https://github.com/Amsterdam/django-gisserver/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/Amsterdam/django-gisserver/actions/workflows/tests.yaml)
 [![PyPI](https://img.shields.io/pypi/v/django-gisserver.svg)](https://pypi.python.org/pypi/django-gisserver)
 [![MPL License](https://img.shields.io/badge/license-MPL%202.0-blue.svg)](https://pypi.python.org/pypi/django-gisserver)
-[![Coverage](https://img.shields.io/codecov/c/github/amsterdam/django-gisserver/master.svg)](https://codecov.io/github/amsterdam/django-gisserver?branch=master)
+[![Coverage](https://img.shields.io/codecov/c/github/amsterdam/django-gisserver/main.svg)](https://codecov.io/github/amsterdam/django-gisserver?branch=main)
 
 # django-gisserver
 
 Django speaking WFS 2.0 to expose geo data.
 
 ## Features
```

### Comparing `django-gisserver-1.2.5/django_gisserver.egg-info/PKG-INFO` & `django-gisserver-1.2.6/django_gisserver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 Metadata-Version: 2.1
 Name: django-gisserver
-Version: 1.2.5
+Version: 1.2.6
 Summary: Django speaking WFS 2.0 (exposing GeoDjango model fields)
 Home-page: https://github.com/amsterdam/django-gisserver
 Author: Diederik van der Boor
 Author-email: opensource@edoburu.nl
 License: Mozilla Public License 2.0
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires: Django (>=2.0)
+Requires: Django (>=3.2)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 [![Documentation](https://readthedocs.org/projects/django-gisserver/badge/?version=latest)](https://django-gisserver.readthedocs.io/en/latest/?badge=latest)
-[![Actions](https://github.com/django-fluent/django-fluent-contents/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/Amsterdam/django-gisserver/actions/workflows/tests.yaml)
+[![Actions](https://github.com/Amsterdam/django-gisserver/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/Amsterdam/django-gisserver/actions/workflows/tests.yaml)
 [![PyPI](https://img.shields.io/pypi/v/django-gisserver.svg)](https://pypi.python.org/pypi/django-gisserver)
 [![MPL License](https://img.shields.io/badge/license-MPL%202.0-blue.svg)](https://pypi.python.org/pypi/django-gisserver)
-[![Coverage](https://img.shields.io/codecov/c/github/amsterdam/django-gisserver/master.svg)](https://codecov.io/github/amsterdam/django-gisserver?branch=master)
+[![Coverage](https://img.shields.io/codecov/c/github/amsterdam/django-gisserver/main.svg)](https://codecov.io/github/amsterdam/django-gisserver?branch=main)
 
 # django-gisserver
 
 Django speaking WFS 2.0 to expose geo data.
 
 ## Features
 
@@ -155,7 +153,9 @@
 Much of this software is then published as Open Source so that other municipalities,
 organizations and citizens can use the software as a basis and inspiration to develop
 similar software themselves. The Municipality of Amsterdam considers it important that
 software developed with public money is also publicly available.
 
 This package is initially developed by the City of Amsterdam, but the tools
 and concepts created in this project can be used in any city.
+
+
```

### Comparing `django-gisserver-1.2.5/django_gisserver.egg-info/SOURCES.txt` & `django-gisserver-1.2.6/django_gisserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/conf.py` & `django-gisserver-1.2.6/gisserver/conf.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/db.py` & `django-gisserver-1.2.6/gisserver/db.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/exceptions.py` & `django-gisserver-1.2.6/gisserver/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/features.py` & `django-gisserver-1.2.6/gisserver/features.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/geometries.py` & `django-gisserver-1.2.6/gisserver/geometries.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,19 @@
 from __future__ import annotations
 
 import re
 from dataclasses import dataclass, field
 from decimal import Decimal
 from functools import lru_cache
 
-from django.contrib.gis.gdal import CoordTransform, SpatialReference
+from django.contrib.gis.gdal import AxisOrder, CoordTransform, SpatialReference
 from django.contrib.gis.geos import GEOSGeometry, Polygon
 
 from gisserver.exceptions import ExternalParsingError, ExternalValueError
 
-try:
-    from django.contrib.gis.gdal import AxisOrder  # Django 3.1+
-except ImportError:
-    AxisOrder = None
-
 CRS_URN_REGEX = re.compile(
     r"^urn:(?P<domain>[a-z]+)"
     r":def:crs:(?P<authority>[a-z]+)"
     r":(?P<version>[0-9]+\.[0-9]+(\.[0-9]+)?)?"
     r":(?P<id>[0-9]+|crs84)"
     r"$",
     re.IGNORECASE,
@@ -36,21 +31,15 @@
 ]
 
 
 @lru_cache(maxsize=200)
 def _get_spatial_reference(srs_input, srs_type="user", axis_order=None):
     """Construct an GDAL object reference"""
     # Using lru-cache to avoid repeated GDAL c-object construction
-    if AxisOrder is not None:
-        # Django 3.1+ only, allow to define the axis ordering with GDAL 3.0
-        # https://gdal.org/tutorials/osr_api_tut.html#crs-and-axis-order
-        # https://github.com/django/django/commit/58f1b07e49a98bb391c9e38b91f078ab2c302703
-        return SpatialReference(srs_input, srs_type=srs_type, axis_order=axis_order)
-    else:
-        return SpatialReference(srs_input, srs_type=srs_type)
+    return SpatialReference(srs_input, srs_type=srs_type, axis_order=axis_order)
 
 
 @lru_cache(maxsize=100)
 def _get_coord_transform(
     source: int | SpatialReference, target: int | SpatialReference
 ) -> CoordTransform:
     """Get an efficient coordinate transformation object.
```

### Comparing `django-gisserver-1.2.5/gisserver/operations/base.py` & `django-gisserver-1.2.6/gisserver/operations/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,22 +254,24 @@
                 )
             ]
 
         return parameters
 
     def _parse_output_format(self, value) -> OutputFormat:
         """Select the proper OutputFormat object based on the input value"""
-        value = value.replace(" ", "+")  # allow application/gml+xml on the KVP.
-        try:
-            return next(o for o in self.output_formats if o.matches(value))
-        except StopIteration:
-            raise InvalidParameterValue(
-                "outputformat",
-                f"'{value}' is not a permitted output format for this operation.",
-            ) from None
+        # The str.replace is here to "allow application/gml+xml on the KVP",
+        # but I'm not sure what that comment was supposed to mean.
+        for v in [value, value.replace(" ", "+")]:
+            for o in self.output_formats:
+                if o.matches(v):
+                    return o
+        raise InvalidParameterValue(
+            "outputformat",
+            f"'{value}' is not a permitted output format for this operation.",
+        ) from None
 
     def _parse_namespaces(self, value) -> dict[str, str]:
         """Parse the namespaces definition.
 
         The NAMESPACES parameter defines which namespaces are used in the KVP request.
         When this parameter is not given, the default namespaces are assumed.
         """
```

### Comparing `django-gisserver-1.2.5/gisserver/operations/wfs20.py` & `django-gisserver-1.2.6/gisserver/operations/wfs20.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,19 @@
 class DescribeFeatureType(WFSTypeNamesMethod):
     """This returns an XML Schema for the provided objects.
     Each feature is exposed as an XSD definition with it's fields.
     """
 
     output_formats = [
         OutputFormat("XMLSCHEMA", renderer_class=output.XMLSchemaRenderer),
+        # At least one version of FME seems to sends a DescribeFeatureType
+        # request with this output format. Do what mapserver does and just
+        # send it XML Schema.
+        OutputFormat("application/gml+xml; version=3.2",
+                     renderer_class=output.XMLSchemaRenderer)
         # OutputFormat("text/xml", subtype="gml/3.1.1"),
     ]
 
     def get_context_data(self, typeNames, **params):
         if self.view.KVP.get("TYPENAMES") == "" or self.view.KVP.get("TYPENAME") == "":
             # Using TYPENAMES= does result in an error.
             raise MissingParameterValue("typeNames", "Empty TYPENAMES parameter")
@@ -432,15 +437,15 @@
             charset="utf-8",
             renderer_class=output.geojson_renderer,
             title="GeoJSON",
         ),
         OutputFormat(
             # Alias needed to make ESRI ArcGIS online accept the WFS.
             # It does not recognize the "subtype" as an alias.
-            "geojson",
+            "GEOJSON",
             renderer_class=output.geojson_renderer,
         ),
         OutputFormat(
             "text/csv",
             subtype="csv",
             charset="utf-8",
             renderer_class=output.csv_renderer,
```

### Comparing `django-gisserver-1.2.5/gisserver/output/__init__.py` & `django-gisserver-1.2.6/gisserver/output/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,15 @@
     DBGML32ValueRenderer,
     GML32Renderer,
     GML32ValueRenderer,
 )
 from .results import FeatureCollection, SimpleFeatureCollection
 from .xmlschema import XMLSchemaRenderer
 
-try:
-    from django.utils.functional import classproperty  # Django 3.1+
-except ImportError:
-    from django.utils.decorators import classproperty
+from django.utils.functional import classproperty
 
 __all__ = [
     "OutputRenderer",
     "FeatureCollection",
     "SimpleFeatureCollection",
     "DBCSVRenderer",
     "DBGeoJsonRenderer",
```

### Comparing `django-gisserver-1.2.5/gisserver/output/base.py` & `django-gisserver-1.2.6/gisserver/output/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/output/buffer.py` & `django-gisserver-1.2.6/gisserver/output/buffer.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/output/csv.py` & `django-gisserver-1.2.6/gisserver/output/csv.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/output/geojson.py` & `django-gisserver-1.2.6/gisserver/output/geojson.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/output/gml32.py` & `django-gisserver-1.2.6/gisserver/output/gml32.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,24 +84,24 @@
             feature_type=sub_collection.feature_type,
             instance=instance,
             extra_xmlns=self.render_xmlns_standalone(),
         ).lstrip(" ")
 
         if body.startswith("<"):
             return HttpResponse(
-                content=f'<?xml version="1.0" encoding="UTF-8"?>\n{body.lstrip()}',
+                content=f'<?xml version="1.0" encoding="UTF-8"?>\n{body}',
                 content_type=self.content_type,
             )
         else:
             # Best guess for GetFeatureById combined with
             # GetPropertyValue&VALUEREFERENCE=@gml:id
             return HttpResponse(body, content_type="text/plain")
 
     def render_xmlns(self):
-        """Generate the xmlns block that the documente needs"""
+        """Generate the xmlns block that the document needs"""
         xsd_typenames = ",".join(
             sub_collection.feature_type.name
             for sub_collection in self.collection.results
         )
         schema_location = [
             f"{self.app_xml_namespace} {self.server_url}?SERVICE=WFS&VERSION=2.0.0&REQUEST=DescribeFeatureType&TYPENAMES={xsd_typenames}",  # noqa: E501
             "http://www.opengis.net/wfs/2.0 http://schemas.opengis.net/wfs/2.0/wfs.xsd",
@@ -368,21 +368,22 @@
             f"</gml:Point>"
         )
 
     @register_geos_type(geos.Polygon)
     def render_gml_polygon(self, value: geos.Polygon, base_attrs=""):
         # lol: http://erouault.blogspot.com/2014/04/gml-madness.html
         ext_ring = self.render_gml_linear_ring(value.exterior_ring)
-        tags = [f"<gml:Polygon{base_attrs}><gml:exterior>{ext_ring}</gml:exterior>"]
+        buf = StringBuffer()
+        buf.write(f"<gml:Polygon{base_attrs}><gml:exterior>{ext_ring}</gml:exterior>")
         for i in range(value.num_interior_rings):
-            tags.append("<gml:interior>")
-            tags.append(self.render_gml_linear_ring(value[i + 1]))
-            tags.append("</gml:interior>")
-        tags.append("</gml:Polygon>")
-        return "".join(tags)
+            buf.write("<gml:interior>")
+            buf.write(self.render_gml_linear_ring(value[i + 1]))
+            buf.write("</gml:interior>")
+        buf.write("</gml:Polygon>")
+        return buf.getvalue()
 
     @register_geos_type(geos.MultiPolygon)
     def render_gml_multi_geometry(self, value: geos.GeometryCollection, base_attrs):
         children = "".join(self._render_gml_type(child) for child in value)
         return f"<gml:MultiGeometry{base_attrs}>{children}</gml:MultiGeometry>"
 
     @register_geos_type(geos.MultiLineString)
```

### Comparing `django-gisserver-1.2.5/gisserver/output/results.py` & `django-gisserver-1.2.6/gisserver/output/results.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/output/utils.py` & `django-gisserver-1.2.6/gisserver/output/utils.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/output/xmlschema.py` & `django-gisserver-1.2.6/gisserver/output/xmlschema.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/base.py` & `django-gisserver-1.2.6/gisserver/parsers/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/fes20/__init__.py` & `django-gisserver-1.2.6/gisserver/parsers/fes20/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/fes20/expressions.py` & `django-gisserver-1.2.6/gisserver/parsers/fes20/expressions.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/fes20/filters.py` & `django-gisserver-1.2.6/gisserver/parsers/fes20/filters.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/fes20/functions.py` & `django-gisserver-1.2.6/gisserver/parsers/fes20/functions.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/fes20/identifiers.py` & `django-gisserver-1.2.6/gisserver/parsers/fes20/identifiers.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/fes20/operators.py` & `django-gisserver-1.2.6/gisserver/parsers/fes20/operators.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/fes20/query.py` & `django-gisserver-1.2.6/gisserver/parsers/fes20/query.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/fes20/sorting.py` & `django-gisserver-1.2.6/gisserver/parsers/fes20/sorting.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/gml/__init__.py` & `django-gisserver-1.2.6/gisserver/parsers/gml/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/gml/base.py` & `django-gisserver-1.2.6/gisserver/parsers/gml/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/gml/geometries.py` & `django-gisserver-1.2.6/gisserver/parsers/gml/geometries.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/tags.py` & `django-gisserver-1.2.6/gisserver/parsers/tags.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/parsers/values.py` & `django-gisserver-1.2.6/gisserver/parsers/values.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/queries/__init__.py` & `django-gisserver-1.2.6/gisserver/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/queries/adhoc.py` & `django-gisserver-1.2.6/gisserver/queries/adhoc.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/queries/base.py` & `django-gisserver-1.2.6/gisserver/queries/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/queries/stored.py` & `django-gisserver-1.2.6/gisserver/queries/stored.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/templates/gisserver/index.html` & `django-gisserver-1.2.6/gisserver/templates/gisserver/index.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/templates/gisserver/service_description.html` & `django-gisserver-1.2.6/gisserver/templates/gisserver/service_description.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml` & `django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml` & `django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml` & `django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/feature_field.html` & `django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/feature_field.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/templates/gisserver/wfs/feature_type.html` & `django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/feature_type.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/types.py` & `django-gisserver-1.2.6/gisserver/types.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/gisserver/views.py` & `django-gisserver-1.2.6/gisserver/views.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.5/setup.py` & `django-gisserver-1.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 
 
 setup(
     name="django-gisserver",
     version=find_version("gisserver", "__init__.py"),
     license="Mozilla Public License 2.0",
     install_requires=[
-        "Django >= 2.0",
+        "Django >= 3.2",
         "defusedxml >= 0.6.0",
         "lru_dict >= 1.1.7",
         "orjson >= 2.4.0",
     ],
     tests_require=tests_require,
     extras_require={
         "tests": tests_require,
     },
-    requires=["Django (>=2.0)"],
+    requires=["Django (>=3.2)"],
     description="Django speaking WFS 2.0 (exposing GeoDjango model fields)",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="Diederik van der Boor",
     author_email="opensource@edoburu.nl",
     url="https://github.com/amsterdam/django-gisserver",
     packages=find_packages(exclude=("tests*", "example*"), include=("gisserver*")),
@@ -61,20 +61,17 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.0",
-        "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
-        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3.6",
 )
```

