# Comparing `tmp/anycluster-2.2.0.tar.gz` & `tmp/anycluster-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycluster-2.2.0.tar", last modified: Sun Jun  4 14:57:16 2023, max compression
+gzip compressed data, was "anycluster-2.3.0.tar", last modified: Wed Jun  7 08:30:01 2023, max compression
```

## Comparing `anycluster-2.2.0.tar` & `anycluster-2.3.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.741238 anycluster-2.2.0/
--rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.2.0/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.2.0/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-04 14:57:16.741238 anycluster-2.2.0/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.2.0/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.733238 anycluster-2.2.0/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.2.0/anycluster/ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3656 2023-05-26 12:34:24.000000 anycluster-2.2.0/anycluster/FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    36887 2023-05-30 10:03:21.000000 anycluster-2.2.0/anycluster/MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.2.0/anycluster/MapTools.py
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.2.0/anycluster/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.733238 anycluster-2.2.0/anycluster/api/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.737238 anycluster-2.2.0/anycluster/api/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.2.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.2.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3290 2023-05-26 08:56:52.000000 anycluster-2.2.0/anycluster/api/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.2.0/anycluster/api/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     7337 2023-05-26 08:42:05.000000 anycluster-2.2.0/anycluster/api/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.2.0/anycluster/api/json_schemas.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3301 2023-05-26 08:56:48.000000 anycluster-2.2.0/anycluster/api/serializers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.737238 anycluster-2.2.0/anycluster/api/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.737238 anycluster-2.2.0/anycluster/api/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.2.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.2.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     9287 2023-05-26 08:54:01.000000 anycluster-2.2.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.2.0/anycluster/api/tests/test_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)    13727 2023-05-26 08:53:58.000000 anycluster-2.2.0/anycluster/api/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.2.0/anycluster/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9493 2023-05-26 08:40:46.000000 anycluster-2.2.0/anycluster/api/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.2.0/anycluster/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/clusters.py
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.2.0/anycluster/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/globalmaptiles.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.733238 anycluster-2.2.0/anycluster/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.733238 anycluster-2.2.0/anycluster/static/anycluster/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.737238 anycluster-2.2.0/anycluster/static/anycluster/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/10.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/100.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/1000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/10000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/10000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/1000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/100_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/10_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/5.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/50.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/50_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/5_empty.png
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/pin_unknown.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.741238 anycluster-2.2.0/anycluster/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.741238 anycluster-2.2.0/anycluster/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.2.0/anycluster/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2865 2023-05-26 05:42:40.000000 anycluster-2.2.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.2.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.2.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.2.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    14813 2023-05-26 08:50:17.000000 anycluster-2.2.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.2.0/anycluster/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2230 2023-05-26 05:42:38.000000 anycluster-2.2.0/anycluster/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.2.0/anycluster/tests/test_ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.2.0/anycluster/tests/test_FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    25353 2023-05-26 08:50:15.000000 anycluster-2.2.0/anycluster/tests/test_MapClusterer.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.733238 anycluster-2.2.0/anycluster.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-04 14:57:16.000000 anycluster-2.2.0/anycluster.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2191 2023-06-04 14:57:16.000000 anycluster-2.2.0/anycluster.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-04 14:57:16.000000 anycluster-2.2.0/anycluster.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-06-04 14:57:16.000000 anycluster-2.2.0/anycluster.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-06-04 14:57:16.000000 anycluster-2.2.0/anycluster.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-06-04 14:57:16.741238 anycluster-2.2.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-06-04 14:57:01.000000 anycluster-2.2.0/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.943661 anycluster-2.3.0/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.3.0/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.3.0/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-07 08:30:01.943661 anycluster-2.3.0/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.3.0/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.935661 anycluster-2.3.0/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.3.0/anycluster/ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3656 2023-05-26 12:34:24.000000 anycluster-2.3.0/anycluster/FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    37213 2023-06-06 12:31:46.000000 anycluster-2.3.0/anycluster/MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.3.0/anycluster/MapTools.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.3.0/anycluster/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.939661 anycluster-2.3.0/anycluster/api/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.939661 anycluster-2.3.0/anycluster/api/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.3.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.3.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3918 2023-06-06 10:47:45.000000 anycluster-2.3.0/anycluster/api/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.3.0/anycluster/api/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     7868 2023-06-07 08:23:18.000000 anycluster-2.3.0/anycluster/api/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.3.0/anycluster/api/json_schemas.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3670 2023-06-06 10:10:33.000000 anycluster-2.3.0/anycluster/api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.939661 anycluster-2.3.0/anycluster/api/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.939661 anycluster-2.3.0/anycluster/api/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.3.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.3.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    10045 2023-06-07 08:21:32.000000 anycluster-2.3.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.3.0/anycluster/api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    14763 2023-06-07 08:21:29.000000 anycluster-2.3.0/anycluster/api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.3.0/anycluster/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9915 2023-06-07 08:21:53.000000 anycluster-2.3.0/anycluster/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.3.0/anycluster/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/clusters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.3.0/anycluster/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/globalmaptiles.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.935661 anycluster-2.3.0/anycluster/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.935661 anycluster-2.3.0/anycluster/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.943661 anycluster-2.3.0/anycluster/static/anycluster/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/10.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/100.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/1000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/10000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/10000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/1000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/100_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/10_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/5.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/50.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/50_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/5_empty.png
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/pin_unknown.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.943661 anycluster-2.3.0/anycluster/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.943661 anycluster-2.3.0/anycluster/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.3.0/anycluster/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2865 2023-05-26 05:42:40.000000 anycluster-2.3.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.3.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.3.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.3.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    14813 2023-05-26 08:50:17.000000 anycluster-2.3.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.3.0/anycluster/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2230 2023-05-26 05:42:38.000000 anycluster-2.3.0/anycluster/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.3.0/anycluster/tests/test_ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.3.0/anycluster/tests/test_FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    25353 2023-05-26 08:50:15.000000 anycluster-2.3.0/anycluster/tests/test_MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.3.0/anycluster/utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.939661 anycluster-2.3.0/anycluster.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-07 08:30:01.000000 anycluster-2.3.0/anycluster.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2211 2023-06-07 08:30:01.000000 anycluster-2.3.0/anycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-07 08:30:01.000000 anycluster-2.3.0/anycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-06-07 08:30:01.000000 anycluster-2.3.0/anycluster.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-06-07 08:30:01.000000 anycluster-2.3.0/anycluster.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-06-07 08:30:01.943661 anycluster-2.3.0/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-06-07 08:12:27.000000 anycluster-2.3.0/setup.py
```

### Comparing `anycluster-2.2.0/LICENSE` & `anycluster-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/PKG-INFO` & `anycluster-2.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.2.0
+Version: 2.3.0
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.2.0/README.md` & `anycluster-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/ClusterCache.py` & `anycluster-2.3.0/anycluster/ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/FilterComposer.py` & `anycluster-2.3.0/anycluster/FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/MapClusterer.py` & `anycluster-2.3.0/anycluster/MapClusterer.py`

 * *Files 2% similar despite different names*

```diff
@@ -740,40 +740,50 @@
                        kmeans_string=kmeans_string, fields=gis_fields_str)
 
         entries_queryset = Gis.objects.raw(sql)
 
         return list(entries_queryset)
 
 
-    def get_area_content(self, geojson, filters):
+    def get_area_content(self, geojson, filters, limit=None, offset=None):
 
         geomfilterstring = self.get_geom_filterstring(geojson)
 
         filter_composer = FilterComposer(filters)
         filterstring = filter_composer.as_sql()
 
         gis_fields_str = self.get_gis_fields_str()
 
-        entries_queryset = Gis.objects.raw(
-            '''SELECT {fields} FROM {schema_name}.{geo_table} WHERE {geomfilterstring} {filterstring};'''.format(
+        sql = '''SELECT {fields} FROM {schema_name}.{geo_table} WHERE {geomfilterstring} {filterstring} '''.format(
                 schema_name=self.schema_name, geo_table=geo_table, geomfilterstring=geomfilterstring,
                 filterstring=filterstring, fields=gis_fields_str)
-        )
+
+        if limit != None:
+            sql = '{sql} LIMIT {limit}'.format(sql=sql, limit=limit)
+        
+        if offset != None:
+            sql = '{sql} OFFSET {offset}'.format(sql=sql, offset=offset)
+
+        sql = '{sql};'.format(sql=sql)
+
+        entries_queryset = Gis.objects.raw(sql)
 
         return entries_queryset
 
 
     def get_dataset_content(self, id):
 
-        gis_fields_str = self.get_gis_fields_str()
+        #gis_fields_str = self.get_gis_fields_str()
+
+        queryset = Gis.objects.filter(pk=id).first()
 
-        queryset = Gis.objects.raw(
-            '''SELECT {fields} FROM {schema_name}.{geo_table} WHERE id={id};'''.format(
-                schema_name=self.schema_name, geo_table=geo_table, fields=gis_fields_str, id=str(id))
-        )
+        #queryset = Gis.objects.raw(
+        #    '''SELECT {fields} FROM {schema_name}.{geo_table} WHERE id={id};'''.format(
+        #        schema_name=self.schema_name, geo_table=geo_table, fields=gis_fields_str, id=str(id))
+        #)
 
         return queryset
 
 
     def get_map_content_counts(self, geojson, geometry_type, filters, zoom, modulations):
 
         result = {
```

### Comparing `anycluster-2.2.0/anycluster/MapTools.py` & `anycluster-2.3.0/anycluster/MapTools.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc` & `anycluster-2.3.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc` & `anycluster-2.3.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/api/__pycache__/urls.cpython-38.pyc` & `anycluster-2.3.0/anycluster/api/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/api/__pycache__/views.cpython-38.pyc` & `anycluster-2.3.0/anycluster/api/__pycache__/views.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri May 26 08:40:46 2023 UTC, .py size: 9493 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,459 +1,492 @@
-00000000: 550d 0d0a 0000 0000 8e70 7064 1525 0000  U........ppd.%..
+00000000: 550d 0d0a 0000 0000 213e 8064 bb26 0000  U.......!>.d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 2c01 0000 6400  .....@...s,...d.
+00000020: 0005 0000 0040 0000 0073 6001 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
-00000080: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 0100 6408  m.Z.m.Z.m.Z...d.
-00000090: 6409 6c01 6d11 5a11 6d12 5a12 6d13 5a13  d.l.m.Z.m.Z.m.Z.
-000000a0: 6d14 5a14 0100 6400 640a 6c15 6d16 5a16  m.Z...d.d.l.m.Z.
-000000b0: 0100 6400 640b 6c17 5a17 4700 640c 640d  ..d.d.l.Z.G.d.d.
-000000c0: 8400 640d 6503 8303 5a18 4700 640e 640f  ..d.e...Z.G.d.d.
-000000d0: 8400 640f 8302 5a19 4700 6410 6411 8400  ..d...Z.G.d.d...
-000000e0: 6411 6519 6503 8304 5a1a 4700 6412 6413  d.e.e...Z.G.d.d.
-000000f0: 8400 6413 6519 6503 8304 5a1b 4700 6414  ..d.e.e...Z.G.d.
-00000100: 6415 8400 6415 6519 6503 8304 5a1c 4700  d...d.e.e...Z.G.
-00000110: 6416 6417 8400 6417 6519 6503 8304 5a1d  d.d...d.e.e...Z.
-00000120: 4700 6418 6419 8400 6419 6519 6503 8304  G.d.d...d.e.e...
-00000130: 5a1e 4700 641a 641b 8400 641b 6519 6503  Z.G.d.d...d.e.e.
-00000140: 8304 5a1f 4700 641c 641d 8400 641d 6519  ..Z.G.d.d...d.e.
-00000150: 6503 8304 5a20 640b 5300 291e e900 0000  e...Z d.S.).....
-00000160: 0029 01da 0b73 6572 6961 6c69 7a65 7273  .)...serializers
-00000170: 2901 da07 4150 4956 6965 77a9 01da 0852  )...APIView....R
-00000180: 6573 706f 6e73 6529 01da 0c4a 534f 4e52  esponse)...JSONR
-00000190: 656e 6465 7265 72a9 01da 0673 7461 7475  enderer....statu
-000001a0: 7329 01da 0c4d 6170 436c 7573 7465 7265  s)...MapClustere
-000001b0: 7229 04da 1647 454f 4d45 5452 595f 5459  r)...GEOMETRY_TY
-000001c0: 5045 5f56 4945 5750 4f52 54da 1247 454f  PE_VIEWPORT..GEO
-000001d0: 4d45 5452 595f 5459 5045 5f41 5245 41da  METRY_TYPE_AREA.
-000001e0: 1143 4c55 5354 4552 5f54 5950 455f 4752  .CLUSTER_TYPE_GR
-000001f0: 4944 da13 434c 5553 5445 525f 5459 5045  ID..CLUSTER_TYPE
-00000200: 5f4b 4d45 414e 53e9 0100 0000 2904 da18  _KMEANS.....)...
-00000210: 436c 7573 7465 7252 6571 7565 7374 5365  ClusterRequestSe
-00000220: 7269 616c 697a 6572 da1f 436c 7573 7465  rializer..Cluste
-00000230: 7243 6f6e 7465 6e74 5265 7175 6573 7453  rContentRequestS
-00000240: 6572 6961 6c69 7a65 72da 194d 6170 436f  erializer..MapCo
-00000250: 6e74 656e 7443 6f75 6e74 5365 7269 616c  ntentCountSerial
-00000260: 697a 6572 da1b 4772 6f75 7065 644d 6170  izer..GroupedMap
-00000270: 436f 6e74 656e 7453 6572 6961 6c69 7a65  ContentSerialize
-00000280: 7229 01da 0c43 6c75 7374 6572 4361 6368  r)...ClusterCach
-00000290: 654e 6300 0000 0000 0000 0000 0000 0000  eNc.............
-000002a0: 0000 0002 0000 0040 0000 0073 1400 0000  .......@...s....
-000002b0: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
-000002c0: 6403 5300 2904 da07 4150 4948 6f6d 6563  d.S.)...APIHomec
-000002d0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-000002e0: 0300 0000 4f00 0000 730c 0000 0074 0064  ....O...s....t.d
-000002f0: 0164 0269 0183 0153 0029 034e da07 7375  .d.i...S.).N..su
-00000300: 6363 6573 7354 7204 0000 0029 04da 0473  ccessTr....)...s
-00000310: 656c 66da 0772 6571 7565 7374 da04 6172  elf..request..ar
-00000320: 6773 da06 6b77 6172 6773 a900 721a 0000  gs..kwargs..r...
-00000330: 00fa 382f 686f 6d65 2f74 6f6d 2f61 6e79  ..8/home/tom/any
-00000340: 636c 7573 7465 722f 6465 6d6f 2f64 6a61  cluster/demo/dja
-00000350: 6e67 6f2f 616e 7963 6c75 7374 6572 2f61  ngo/anycluster/a
-00000360: 7069 2f76 6965 7773 2e70 79da 0367 6574  pi/views.py..get
-00000370: 1400 0000 7302 0000 0000 017a 0b41 5049  ....s......z.API
-00000380: 486f 6d65 2e67 6574 4ea9 04da 085f 5f6e  Home.getN....__n
-00000390: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-000003a0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-000003b0: 1c00 0000 721a 0000 0072 1a00 0000 721a  ....r....r....r.
-000003c0: 0000 0072 1b00 0000 7214 0000 0012 0000  ...r....r.......
-000003d0: 0073 0200 0000 0802 7214 0000 0063 0000  .s......r....c..
-000003e0: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-000003f0: 0000 4000 0000 7340 0000 0065 005a 0164  ..@...s@...e.Z.d
-00000400: 005a 0264 015a 0364 0264 0384 005a 0464  .Z.d.Z.d.d...Z.d
-00000410: 0464 0584 005a 0564 0664 0784 005a 0664  .d...Z.d.d...Z.d
-00000420: 0864 0984 005a 0764 0a64 0b84 005a 0864  .d...Z.d.d...Z.d
-00000430: 0c64 0d84 005a 0964 0e53 0029 0fda 124d  .d...Z.d.S.)...M
-00000440: 6170 436c 7573 7465 7256 6965 7742 6173  apClusterViewBas
-00000450: 65da 1061 6e79 636c 7573 7465 725f 6361  e..anycluster_ca
-00000460: 6368 6563 0200 0000 0000 0000 0000 0000  chec............
-00000470: 0300 0000 0400 0000 4300 0000 7316 0000  ........C...s...
-00000480: 0074 007c 01a0 0164 01a1 0164 0219 0083  .t.|...d...d....
-00000490: 017d 027c 0253 0029 034e fa01 3ae9 ffff  .}.|.S.).N..:...
-000004a0: ffff 2902 da03 696e 74da 0573 706c 6974  ..)...int..split
-000004b0: 2903 7216 0000 00da 0873 7269 645f 7374  ).r......srid_st
-000004c0: 72da 0b6f 7574 7075 745f 7372 6964 721a  r..output_sridr.
-000004d0: 0000 0072 1a00 0000 721b 0000 00da 0a70  ...r....r......p
-000004e0: 6172 7365 5f73 7269 641c 0000 0073 0400  arse_srid....s..
-000004f0: 0000 0001 1201 7a1d 4d61 7043 6c75 7374  ......z.MapClust
-00000500: 6572 5669 6577 4261 7365 2e70 6172 7365  erViewBase.parse
-00000510: 5f73 7269 6463 0200 0000 0000 0000 0000  _sridc..........
-00000520: 0000 0200 0000 0100 0000 4300 0000 7304  ..........C...s.
-00000530: 0000 0064 0153 0029 024e da06 7075 626c  ...d.S.).N..publ
-00000540: 6963 721a 0000 0029 0272 1600 0000 7217  icr....).r....r.
-00000550: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
-00000560: 0000 da0f 6765 745f 7363 6865 6d61 5f6e  ....get_schema_n
-00000570: 616d 6521 0000 0073 0200 0000 0001 7a22  ame!...s......z"
-00000580: 4d61 7043 6c75 7374 6572 5669 6577 4261  MapClusterViewBa
-00000590: 7365 2e67 6574 5f73 6368 656d 615f 6e61  se.get_schema_na
-000005a0: 6d65 6307 0000 0000 0000 0000 0000 000d  mec.............
-000005b0: 0000 0007 0000 004b 0000 0073 5800 0000  .......K...sX...
-000005c0: 7c07 6401 1900 7d08 7c07 6402 1900 7d09  |.d...}.|.d...}.
-000005d0: 7c04 6403 6b02 7228 7400 7c01 7c09 7c02  |.d.k.r(t.|.|.|.
-000005e0: 7c03 8304 7d0a 6e12 7c00 a001 7c01 7c09  |...}.n.|...|.|.
-000005f0: 7c02 7c06 7c03 a105 7d0a 7c00 a002 7c06  |.|.|...}.|...|.
-00000600: a101 7d0b 7403 7c0a 7c08 7c05 7c0b 6404  ..}.t.|.|.|.|.d.
-00000610: 8d04 7d0c 7c0c 5300 2905 4eda 0967 7269  ..}.|.S.).N..gri
-00000620: 645f 7369 7a65 da04 7a6f 6f6d 5429 0372  d_size..zoomT).r
-00000630: 2c00 0000 7228 0000 00da 0b73 6368 656d  ,...r(.....schem
-00000640: 615f 6e61 6d65 2904 7213 0000 00da 0967  a_name).r......g
-00000650: 6574 5f63 6163 6865 722b 0000 0072 0900  et_cacher+...r..
-00000660: 0000 290d 7216 0000 00da 0d67 656f 6d65  ..).r......geome
-00000670: 7472 795f 7479 7065 da0b 636c 7573 7465  try_type..cluste
-00000680: 7274 7970 65da 0766 696c 7465 7273 da0b  rtype..filters..
-00000690: 636c 6561 725f 6361 6368 6572 2800 0000  clear_cacher(...
-000006a0: 7217 0000 0072 1900 0000 722c 0000 0072  r....r....r,...r
-000006b0: 2d00 0000 da0d 636c 7573 7465 725f 6361  -.....cluster_ca
-000006c0: 6368 6572 2e00 0000 da09 636c 7573 7465  cher......cluste
-000006d0: 7265 7272 1a00 0000 721a 0000 0072 1b00  rerr....r....r..
-000006e0: 0000 da11 6765 745f 6d61 705f 636c 7573  ....get_map_clus
-000006f0: 7465 7265 7225 0000 0073 1000 0000 0002  terer%...s......
-00000700: 0801 0802 0801 1002 1202 0a01 1001 7a24  ..............z$
-00000710: 4d61 7043 6c75 7374 6572 5669 6577 4261  MapClusterViewBa
-00000720: 7365 2e67 6574 5f6d 6170 5f63 6c75 7374  se.get_map_clust
-00000730: 6572 6572 6306 0000 0000 0000 0000 0000  ererc...........
-00000740: 0008 0000 0005 0000 0043 0000 0073 2c00  .........C...s,.
-00000750: 0000 7c04 6a00 a001 7c00 6a02 6900 a102  ..|.j...|.j.i...
-00000760: 7d06 7403 7c01 7c02 7c03 7c05 8304 7d07  }.t.|.|.|.|...}.
-00000770: 7c07 a004 7c06 a101 0100 7c07 5300 a901  |...|.....|.S...
-00000780: 4e29 05da 0773 6573 7369 6f6e 721c 0000  N)...sessionr...
-00000790: 00da 0a63 6163 6865 5f6e 616d 6572 1300  ...cache_namer..
-000007a0: 0000 da0f 6c6f 6164 5f67 656f 6d65 7472  ....load_geometr
-000007b0: 6965 7329 0872 1600 0000 7230 0000 0072  ies).r....r0...r
-000007c0: 2d00 0000 7231 0000 0072 1700 0000 7232  -...r1...r....r2
-000007d0: 0000 00da 0663 6163 6865 6472 3400 0000  .....cachedr4...
-000007e0: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-000007f0: 2f00 0000 3400 0000 7308 0000 0000 0110  /...4...s.......
-00000800: 010e 020a 017a 1c4d 6170 436c 7573 7465  .....z.MapCluste
-00000810: 7256 6965 7742 6173 652e 6765 745f 6361  rViewBase.get_ca
-00000820: 6368 6563 0300 0000 0000 0000 0000 0000  chec............
-00000830: 0400 0000 0300 0000 4300 0000 7318 0000  ........C...s...
-00000840: 007c 02a0 00a1 007d 037c 037c 016a 017c  .|.....}.|.|.j.|
-00000850: 006a 023c 0064 0053 0072 3700 0000 2903  .j.<.d.S.r7...).
-00000860: da09 7365 7269 616c 697a 6572 3800 0000  ..serializer8...
-00000870: 7239 0000 0029 0472 1600 0000 7217 0000  r9...).r....r...
-00000880: 0072 3400 0000 5a12 636c 7573 7465 725f  .r4...Z.cluster_
-00000890: 6361 6368 655f 6a73 6f6e 721a 0000 0072  cache_jsonr....r
-000008a0: 1a00 0000 721b 0000 00da 0973 6574 5f63  ....r......set_c
-000008b0: 6163 6865 3c00 0000 7304 0000 0000 0108  ache<...s.......
-000008c0: 017a 1c4d 6170 436c 7573 7465 7256 6965  .z.MapClusterVie
-000008d0: 7742 6173 652e 7365 745f 6361 6368 6563  wBase.set_cachec
-000008e0: 0300 0000 0000 0000 0000 0000 0500 0000  ................
-000008f0: 0500 0000 4300 0000 7322 0000 007c 01a0  ....C...s"...|..
-00000900: 00a1 007d 0374 016a 0264 017c 027c 0364  ...}.t.j.d.|.|.d
-00000910: 028d 037d 0474 03a0 047c 04a1 0153 0029  ...}.t...|...S.)
-00000920: 034e da04 6a73 6f6e a901 da06 6669 656c  .N..json....fiel
-00000930: 6473 2905 da13 6765 745f 6769 735f 6669  ds)...get_gis_fi
-00000940: 656c 645f 6e61 6d65 7372 0200 0000 723c  eld_namesr....r<
-00000950: 0000 0072 3e00 0000 da05 6c6f 6164 7329  ...r>.....loads)
-00000960: 0572 1600 0000 da0d 6d61 705f 636c 7573  .r......map_clus
-00000970: 7465 7265 725a 0e69 6e73 7461 6e63 6573  tererZ.instances
-00000980: 5f6c 6973 74da 1173 6572 6961 6c69 7a65  _list..serialize
-00000990: 725f 6669 656c 6473 da04 6461 7461 721a  r_fields..datar.
-000009a0: 0000 0072 1a00 0000 721b 0000 00da 1873  ...r....r......s
-000009b0: 6572 6961 6c69 7a65 5f67 6973 5f6d 6f64  erialize_gis_mod
-000009c0: 656c 5f6c 6973 7441 0000 0073 0600 0000  el_listA...s....
-000009d0: 0002 0801 1002 7a2b 4d61 7043 6c75 7374  ......z+MapClust
-000009e0: 6572 5669 6577 4261 7365 2e73 6572 6961  erViewBase.seria
-000009f0: 6c69 7a65 5f67 6973 5f6d 6f64 656c 5f6c  lize_gis_model_l
-00000a00: 6973 744e 290a 721e 0000 0072 1f00 0000  istN).r....r....
-00000a10: 7220 0000 0072 3900 0000 7229 0000 0072  r ...r9...r)...r
-00000a20: 2b00 0000 7236 0000 0072 2f00 0000 723d  +...r6...r/...r=
-00000a30: 0000 0072 4600 0000 721a 0000 0072 1a00  ...rF...r....r..
-00000a40: 0000 721a 0000 0072 1b00 0000 7221 0000  ..r....r....r!..
-00000a50: 0018 0000 0073 0e00 0000 0802 0402 0805  .....s..........
-00000a60: 0804 080f 0808 0805 7221 0000 0063 0000  ........r!...c..
-00000a70: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00000a80: 0000 4000 0000 7322 0000 0065 005a 0164  ..@...s"...e.Z.d
-00000a90: 005a 0267 005a 0367 005a 0465 0567 015a  .Z.g.Z.g.Z.e.g.Z
-00000aa0: 0664 0164 0284 005a 0764 0353 0029 04da  .d.d...Z.d.S.)..
-00000ab0: 0b47 7269 6443 6c75 7374 6572 6302 0000  .GridClusterc...
-00000ac0: 0000 0000 0000 0000 000c 0000 0007 0000  ................
-00000ad0: 004f 0000 0073 9c00 0000 7400 7c01 6a01  .O...s....t.|.j.
-00000ae0: 6401 8d01 7d04 7c04 a002 a100 728c 7c04  d...}.|.....r.|.
-00000af0: 6a03 6402 1900 7d05 7c00 a004 7c04 6a03  j.d...}.|...|.j.
-00000b00: 6403 1900 a101 7d06 7c04 6a03 6404 1900  d.....}.|.j.d...
-00000b10: 7d07 7c00 6a05 7406 7407 7c07 7c05 7c06  }.|.j.t.t.|.|.|.
-00000b20: 7c01 6606 7c03 8e01 7d08 7c04 6a03 6405  |.f.|...}.|.j.d.
-00000b30: 1900 7d09 7c03 6406 1900 7d0a 7c08 a008  ..}.|.d...}.|...
-00000b40: 7c09 7c0a 7c07 a103 7d0b 7c00 a009 7c01  |.|.|...}.|...|.
-00000b50: 7c08 6a0a a102 0100 740b 7c0b 740c 6a0d  |.j.....t.|.t.j.
-00000b60: 6407 8d02 5300 740b 7c04 6a0e 740c 6a0f  d...S.t.|.j.t.j.
-00000b70: 6407 8d02 5300 2908 4ea9 0172 4500 0000  d...S.).N..rE...
-00000b80: 7233 0000 0072 2800 0000 7232 0000 00da  r3...r(...r2....
-00000b90: 0767 656f 6a73 6f6e 722d 0000 0072 0700  .geojsonr-...r..
-00000ba0: 0000 2910 720f 0000 0072 4500 0000 da08  ..).r....rE.....
-00000bb0: 6973 5f76 616c 6964 da0e 7661 6c69 6461  is_valid..valida
-00000bc0: 7465 645f 6461 7461 7229 0000 0072 3600  ted_datar)...r6.
-00000bd0: 0000 720a 0000 0072 0c00 0000 da0c 6772  ..r....r......gr
-00000be0: 6964 5f63 6c75 7374 6572 723d 0000 0072  id_clusterr=...r
-00000bf0: 3400 0000 7205 0000 0072 0800 0000 da0b  4...r....r......
-00000c00: 4854 5450 5f32 3030 5f4f 4bda 0665 7272  HTTP_200_OK..err
-00000c10: 6f72 73da 1448 5454 505f 3430 305f 4241  ors..HTTP_400_BA
-00000c20: 445f 5245 5155 4553 5429 0c72 1600 0000  D_REQUEST).r....
-00000c30: 7217 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00000c40: 0a73 6572 6961 6c69 7a65 7272 3300 0000  .serializerr3...
-00000c50: 7228 0000 0072 3200 0000 7243 0000 0072  r(...r2...rC...r
-00000c60: 4900 0000 722d 0000 00da 0467 7269 6472  I...r-.....gridr
-00000c70: 1a00 0000 721a 0000 0072 1b00 0000 da04  ....r....r......
-00000c80: 706f 7374 5200 0000 7322 0000 0000 020c  postR...s"......
-00000c90: 0208 020a 0110 020a 020c 0102 0002 ff02  ................
-00000ca0: 0102 ff04 030a 0108 020e 020e 010e 027a  ...............z
-00000cb0: 1047 7269 6443 6c75 7374 6572 2e70 6f73  .GridCluster.pos
-00000cc0: 744e 2908 721e 0000 0072 1f00 0000 7220  tN).r....r....r 
-00000cd0: 0000 005a 1661 7574 6865 6e74 6963 6174  ...Z.authenticat
-00000ce0: 696f 6e5f 636c 6173 7365 735a 1270 6572  ion_classesZ.per
-00000cf0: 6d69 7373 696f 6e5f 636c 6173 7365 7372  mission_classesr
-00000d00: 0600 0000 da10 7265 6e64 6572 6572 5f63  ......renderer_c
-00000d10: 6c61 7373 6573 7252 0000 0072 1a00 0000  lassesrR...r....
-00000d20: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00000d30: 4700 0000 4c00 0000 7308 0000 0008 0204  G...L...s.......
-00000d40: 0104 0106 0272 4700 0000 6300 0000 0000  .....rG...c.....
-00000d50: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
-00000d60: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000d70: 6401 6402 8400 5a03 6403 5300 2904 da0d  d.d...Z.d.S.)...
-00000d80: 4b6d 6561 6e73 436c 7573 7465 7263 0200  KmeansClusterc..
-00000d90: 0000 0000 0000 0000 0000 0d00 0000 0700  ................
-00000da0: 0000 4f00 0000 73a2 0000 0074 007c 016a  ..O...s....t.|.j
-00000db0: 0164 018d 017d 047c 04a0 02a1 0072 927c  .d...}.|.....r.|
-00000dc0: 046a 0364 0219 007d 057c 046a 0364 0319  .j.d...}.|.j.d..
-00000dd0: 007d 067c 00a0 047c 046a 0364 0419 00a1  .}.|...|.j.d....
-00000de0: 017d 077c 046a 0364 0519 007d 087c 006a  .}.|.j.d...}.|.j
-00000df0: 057c 0574 067c 087c 067c 077c 0166 067c  .|.t.|.|.|.|.f.|
-00000e00: 038e 017d 097c 046a 0364 0619 007d 0a7c  ...}.|.j.d...}.|
-00000e10: 0364 0719 007d 0b7c 09a0 077c 0a7c 057c  .d...}.|...|.|.|
-00000e20: 0b7c 08a1 047d 0c7c 00a0 087c 017c 096a  .|...}.|...|.|.j
-00000e30: 09a1 0201 0074 0a7c 0c83 0153 0074 0a7c  .....t.|...S.t.|
-00000e40: 046a 0b74 0c6a 0d64 088d 0253 0029 094e  .j.t.j.d...S.).N
-00000e50: 7248 0000 0072 3000 0000 7233 0000 0072  rH...r0...r3...r
-00000e60: 2800 0000 7232 0000 0072 4900 0000 722d  (...r2...rI...r-
-00000e70: 0000 0072 0700 0000 290e 720f 0000 0072  ...r....).r....r
-00000e80: 4500 0000 724a 0000 0072 4b00 0000 7229  E...rJ...rK...r)
-00000e90: 0000 0072 3600 0000 720d 0000 00da 0e6b  ...r6...r......k
-00000ea0: 6d65 616e 735f 636c 7573 7465 7272 3d00  means_clusterr=.
-00000eb0: 0000 7234 0000 0072 0500 0000 724e 0000  ..r4...r....rN..
-00000ec0: 0072 0800 0000 724f 0000 0029 0d72 1600  .r....rO...).r..
-00000ed0: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000ee0: 0072 5000 0000 7230 0000 0072 3300 0000  .rP...r0...r3...
-00000ef0: 7228 0000 0072 3200 0000 7243 0000 0072  r(...r2...rC...r
-00000f00: 4900 0000 722d 0000 00da 076d 6172 6b65  I...r-.....marke
-00000f10: 7273 721a 0000 0072 1a00 0000 721b 0000  rsr....r....r...
-00000f20: 0072 5200 0000 6e00 0000 7322 0000 0000  .rR...n...s"....
-00000f30: 020c 0208 020a 010a 0110 020a 020e 0102  ................
-00000f40: ff02 0102 ff04 030a 0108 0210 010e 0108  ................
-00000f50: 027a 124b 6d65 616e 7343 6c75 7374 6572  .z.KmeansCluster
-00000f60: 2e70 6f73 744e a904 721e 0000 0072 1f00  .postN..r....r..
-00000f70: 0000 7220 0000 0072 5200 0000 721a 0000  ..r ...rR...r...
-00000f80: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000f90: 7254 0000 006c 0000 0073 0200 0000 0802  rT...l...s......
-00000fa0: 7254 0000 0063 0000 0000 0000 0000 0000  rT...c..........
-00000fb0: 0000 0000 0000 0200 0000 4000 0000 7314  ..........@...s.
-00000fc0: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
-00000fd0: 005a 0364 0353 0029 04da 1147 6574 436c  .Z.d.S.)...GetCl
-00000fe0: 7573 7465 7243 6f6e 7465 6e74 6302 0000  usterContentc...
-00000ff0: 0000 0000 0000 0000 0010 0000 0009 0000  ................
-00001000: 004f 0000 0073 c200 0000 7400 7c01 6a01  .O...s....t.|.j.
-00001010: 6401 8d01 7d04 7c04 a002 a100 72b2 7c04  d...}.|.....r.|.
-00001020: 6a03 6402 1900 7d05 7c00 a004 7c04 6a03  j.d...}.|...|.j.
-00001030: 6403 1900 a101 7d06 7c00 a004 7c04 6a03  d.....}.|...|.j.
-00001040: 6404 1900 a101 7d07 7c04 6a03 6405 1900  d.....}.|.j.d...
-00001050: 7d08 7c00 6a05 7c05 7406 7c08 6406 7c06  }.|.j.|.t.|.d.|.
-00001060: 7c01 6606 7c03 8e01 7d09 7c04 6a03 6407  |.f.|...}.|.j.d.
-00001070: 1900 7d0a 7c04 6a03 6408 1900 7d0b 7c04  ..}.|.j.d...}.|.
-00001080: 6a03 6409 1900 7d0c 7c03 640a 1900 7d0d  j.d...}.|.d...}.
-00001090: 7c09 6a07 7c05 7c0a 7c0b 7c0c 7c08 7c0d  |.j.|.|.|.|.|.|.
-000010a0: 7c07 640b 8d07 7d0e 7c00 a008 7c09 7c0e  |.d...}.|...|.|.
-000010b0: a102 7d0f 7409 7c0f 8301 5300 7409 7c04  ..}.t.|...S.t.|.
-000010c0: 6a0a 740b 6a0c 640c 8d02 5300 290d 4e72  j.t.j.d...S.).Nr
-000010d0: 4800 0000 7230 0000 0072 2800 0000 da0a  H...r0...r(.....
-000010e0: 696e 7075 745f 7372 6964 7232 0000 0046  input_sridr2...F
-000010f0: da03 6964 73da 0178 da01 7972 2d00 0000  ..ids..x..yr-...
-00001100: 2901 7259 0000 0072 0700 0000 290d 7210  ).rY...r....).r.
-00001110: 0000 0072 4500 0000 724a 0000 0072 4b00  ...rE...rJ...rK.
-00001120: 0000 7229 0000 0072 3600 0000 720d 0000  ..r)...r6...r...
-00001130: 00da 1a67 6574 5f6b 6d65 616e 735f 636c  ...get_kmeans_cl
-00001140: 7573 7465 725f 636f 6e74 656e 7472 4600  uster_contentrF.
-00001150: 0000 7205 0000 0072 4e00 0000 7208 0000  ..r....rN...r...
-00001160: 0072 4f00 0000 2910 7216 0000 0072 1700  .rO...).r....r..
-00001170: 0000 7218 0000 0072 1900 0000 7250 0000  ..r....r....rP..
-00001180: 0072 3000 0000 7228 0000 0072 5900 0000  .r0...r(...rY...
-00001190: 7232 0000 0072 4300 0000 725a 0000 0072  r2...rC...rZ...r
-000011a0: 5b00 0000 725c 0000 0072 2d00 0000 da0f  [...r\...r-.....
-000011b0: 636c 7573 7465 725f 636f 6e74 656e 7472  cluster_contentr
-000011c0: 4500 0000 721a 0000 0072 1a00 0000 721b  E...r....r....r.
-000011d0: 0000 0072 5200 0000 8c00 0000 732a 0000  ...rR.......s*..
-000011e0: 0000 020c 0208 020a 0110 0110 020a 020e  ................
-000011f0: 0102 ff02 0102 ff04 030a 010a 010a 0208  ................
-00001200: 0210 0102 ff06 030c 0208 027a 1647 6574  ...........z.Get
-00001210: 436c 7573 7465 7243 6f6e 7465 6e74 2e70  ClusterContent.p
-00001220: 6f73 744e 7257 0000 0072 1a00 0000 721a  ostNrW...r....r.
-00001230: 0000 0072 1a00 0000 721b 0000 0072 5800  ...r....r....rX.
-00001240: 0000 8a00 0000 7302 0000 0008 0272 5800  ......s......rX.
-00001250: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001260: 0000 0002 0000 0040 0000 0073 1400 0000  .......@...s....
-00001270: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
-00001280: 6403 5300 2904 da0e 4765 7441 7265 6143  d.S.)...GetAreaC
-00001290: 6f6e 7465 6e74 6302 0000 0000 0000 0000  ontentc.........
-000012a0: 0000 000c 0000 0007 0000 004f 0000 0073  ...........O...s
-000012b0: 8a00 0000 7400 7c01 6a01 6401 8d01 7d04  ....t.|.j.d...}.
-000012c0: 7c04 a002 a100 727a 7c04 6a03 6402 1900  |.....rz|.j.d...
-000012d0: 7d05 7c00 a004 7c04 6a03 6403 1900 a101  }.|...|.j.d.....
-000012e0: 7d06 7c04 6a03 6404 1900 7d07 7c00 6a05  }.|.j.d...}.|.j.
-000012f0: 7c05 7406 7c07 6405 7c06 7c01 6606 7c03  |.t.|.d.|.|.f.|.
-00001300: 8e01 7d08 7c04 6a03 6406 1900 7d09 7c08  ..}.|.j.d...}.|.
-00001310: a007 7c09 7c07 a102 7d0a 7c00 a008 7c08  ..|.|...}.|...|.
-00001320: 7c0a a102 7d0b 7409 7c0b 8301 5300 7409  |...}.t.|...S.t.
-00001330: 7c04 6a0a 740b 6a0c 6407 8d02 5300 2908  |.j.t.j.d...S.).
-00001340: 4e72 4800 0000 7230 0000 0072 2800 0000  NrH...r0...r(...
-00001350: 7232 0000 0046 7249 0000 0072 0700 0000  r2...FrI...r....
-00001360: 290d 720f 0000 0072 4500 0000 724a 0000  ).r....rE...rJ..
-00001370: 0072 4b00 0000 7229 0000 0072 3600 0000  .rK...r)...r6...
-00001380: 720d 0000 00da 1067 6574 5f61 7265 615f  r......get_area_
-00001390: 636f 6e74 656e 7472 4600 0000 7205 0000  contentrF...r...
-000013a0: 0072 4e00 0000 7208 0000 0072 4f00 0000  .rN...r....rO...
-000013b0: 290c 7216 0000 0072 1700 0000 7218 0000  ).r....r....r...
-000013c0: 0072 1900 0000 7250 0000 0072 3000 0000  .r....rP...r0...
-000013d0: 7228 0000 0072 3200 0000 7243 0000 0072  r(...r2...rC...r
-000013e0: 4900 0000 5a0c 6172 6561 5f63 6f6e 7465  I...Z.area_conte
-000013f0: 6e74 7245 0000 0072 1a00 0000 721a 0000  ntrE...r....r...
-00001400: 0072 1b00 0000 7252 0000 00b1 0000 0073  .r....rR.......s
-00001410: 1e00 0000 0002 0c02 0802 0a01 1002 0a02  ................
-00001420: 0e01 02ff 0201 02ff 0403 0a02 0c02 0c02  ................
-00001430: 0802 7a13 4765 7441 7265 6143 6f6e 7465  ..z.GetAreaConte
-00001440: 6e74 2e70 6f73 744e 7257 0000 0072 1a00  nt.postNrW...r..
-00001450: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00001460: 0072 5f00 0000 af00 0000 7302 0000 0008  .r_.......s.....
-00001470: 0272 5f00 0000 6300 0000 0000 0000 0000  .r_...c.........
-00001480: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
-00001490: 1400 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
-000014a0: 8400 5a03 6403 5300 2904 da11 4765 7444  ..Z.d.S.)...GetD
-000014b0: 6174 6173 6574 436f 6e74 656e 7463 0200  atasetContentc..
-000014c0: 0000 0000 0000 0000 0000 0b00 0000 0700  ................
-000014d0: 0000 4f00 0000 7362 0000 007c 016a 00a0  ..O...sb...|.j..
-000014e0: 0164 0164 02a1 027d 0467 007d 057c 006a  .d.d...}.g.}.|.j
-000014f0: 0274 0374 047c 0564 037c 047c 0166 067c  .t.t.|.d.|.|.f.|
-00001500: 038e 017d 067c 0364 0419 007d 077c 06a0  ...}.|.d...}.|..
-00001510: 057c 07a1 017d 087c 06a0 06a1 007d 0974  .|...}.|.....}.t
-00001520: 076a 0864 057c 087c 0964 068d 037d 0a74  .j.d.|.|.d...}.t
-00001530: 0974 0aa0 0b7c 0aa1 0183 0153 0029 074e  .t...|.....S.).N
-00001540: 7228 0000 0069 e610 0000 46da 0a64 6174  r(...i....F..dat
-00001550: 6173 6574 5f69 6472 3e00 0000 723f 0000  aset_idr>...r?..
-00001560: 0029 0cda 0347 4554 721c 0000 0072 3600  .)...GETr....r6.
-00001570: 0000 720a 0000 0072 0c00 0000 da13 6765  ..r....r......ge
-00001580: 745f 6461 7461 7365 745f 636f 6e74 656e  t_dataset_conten
-00001590: 7472 4100 0000 7202 0000 0072 3c00 0000  trA...r....r<...
-000015a0: 7205 0000 0072 3e00 0000 7242 0000 0029  r....r>...rB...)
-000015b0: 0b72 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-000015c0: 7219 0000 0072 2800 0000 7232 0000 0072  r....r(...r2...r
-000015d0: 4300 0000 7262 0000 005a 0764 6174 6173  C...rb...Z.datas
-000015e0: 6574 7244 0000 0072 4500 0000 721a 0000  etrD...rE...r...
-000015f0: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00001600: cd00 0000 7318 0000 0000 020e 0204 020e  ....s...........
-00001610: 0102 ff02 0102 ff04 0308 020a 0208 0110  ................
-00001620: 027a 1547 6574 4461 7461 7365 7443 6f6e  .z.GetDatasetCon
-00001630: 7465 6e74 2e67 6574 4e72 1d00 0000 721a  tent.getNr....r.
-00001640: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
-00001650: 0000 7261 0000 00cb 0000 0073 0200 0000  ..ra.......s....
-00001660: 0802 7261 0000 0063 0000 0000 0000 0000  ..ra...c........
-00001670: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-00001680: 7314 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
-00001690: 0284 005a 0364 0353 0029 04da 1247 6574  ...Z.d.S.)...Get
-000016a0: 4d61 7043 6f6e 7465 6e74 436f 756e 7463  MapContentCountc
-000016b0: 0200 0000 0000 0000 0000 0000 0e00 0000  ................
-000016c0: 0700 0000 4f00 0000 73a0 0000 0074 007c  ....O...s....t.|
-000016d0: 016a 0164 018d 017d 047c 04a0 02a1 0072  .j.d...}.|.....r
-000016e0: 9064 027d 057c 046a 0364 0319 007d 067c  .d.}.|.j.d...}.|
-000016f0: 046a 0364 0419 007d 077c 00a0 047c 046a  .j.d...}.|...|.j
-00001700: 0364 0519 00a1 017d 087c 046a 0364 0619  .d.....}.|.j.d..
-00001710: 007d 097c 0364 0719 007d 0a7c 046a 0364  .}.|.d...}.|.j.d
-00001720: 0819 007d 0b7c 006a 057c 0774 067c 067c  ...}.|.j.|.t.|.|
-00001730: 057c 087c 0166 067c 038e 017d 0c7c 0ca0  .|.|.f.|...}.|..
-00001740: 077c 097c 077c 067c 0a7c 0ba1 057d 0d74  .|.|.|.|.|...}.t
-00001750: 087c 0d74 096a 0a64 098d 0253 0074 087c  .|.t.j.d...S.t.|
-00001760: 046a 0b74 096a 0c64 098d 0253 0029 0a4e  .j.t.j.d...S.).N
-00001770: 7248 0000 0054 7232 0000 0072 3000 0000  rH...Tr2...r0...
-00001780: 7228 0000 0072 4900 0000 722d 0000 00da  r(...rI...r-....
-00001790: 0b6d 6f64 756c 6174 696f 6e73 7207 0000  .modulationsr...
-000017a0: 0029 0d72 1100 0000 7245 0000 0072 4a00  .).r....rE...rJ.
-000017b0: 0000 724b 0000 0072 2900 0000 7236 0000  ..rK...r)...r6..
-000017c0: 0072 0d00 0000 da16 6765 745f 6d61 705f  .r......get_map_
-000017d0: 636f 6e74 656e 745f 636f 756e 7473 7205  content_countsr.
-000017e0: 0000 0072 0800 0000 724d 0000 0072 4e00  ...r....rM...rN.
-000017f0: 0000 724f 0000 0029 0e72 1600 0000 7217  ..rO...).r....r.
-00001800: 0000 0072 1800 0000 7219 0000 0072 5000  ...r....r....rP.
-00001810: 0000 7233 0000 0072 3200 0000 7230 0000  ..r3...r2...r0..
-00001820: 0072 2800 0000 7249 0000 0072 2d00 0000  .r(...rI...r-...
-00001830: 7266 0000 0072 4300 0000 5a12 6d61 705f  rf...rC...Z.map_
-00001840: 636f 6e74 656e 745f 636f 756e 7473 721a  content_countsr.
-00001850: 0000 0072 1a00 0000 721b 0000 0072 5200  ...r....r....rR.
-00001860: 0000 e200 0000 7322 0000 0000 020c 0208  ......s"........
-00001870: 0204 010a 010a 0110 020a 0108 010a 020e  ................
-00001880: 0102 ff02 0102 ff04 0312 020e 027a 1747  .............z.G
-00001890: 6574 4d61 7043 6f6e 7465 6e74 436f 756e  etMapContentCoun
-000018a0: 742e 706f 7374 4e72 5700 0000 721a 0000  t.postNrW...r...
-000018b0: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
-000018c0: 7265 0000 00e0 0000 0073 0200 0000 0802  re.......s......
-000018d0: 7265 0000 0063 0000 0000 0000 0000 0000  re...c..........
-000018e0: 0000 0000 0000 0200 0000 4000 0000 7314  ..........@...s.
-000018f0: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
-00001900: 005a 0364 0353 0029 04da 1547 6574 4772  .Z.d.S.)...GetGr
-00001910: 6f75 7065 644d 6170 436f 6e74 656e 7473  oupedMapContents
-00001920: 6302 0000 0000 0000 0000 0000 000e 0000  c...............
-00001930: 0007 0000 004f 0000 0073 a000 0000 7400  .....O...s....t.
-00001940: 7c01 6a01 6401 8d01 7d04 7c04 a002 a100  |.j.d...}.|.....
-00001950: 7290 6402 7d05 7c04 6a03 6403 1900 7d06  r.d.}.|.j.d...}.
-00001960: 7c04 6a03 6404 1900 7d07 7c00 a004 7c04  |.j.d...}.|...|.
-00001970: 6a03 6405 1900 a101 7d08 7c04 6a03 6406  j.d.....}.|.j.d.
-00001980: 1900 7d09 7c03 6407 1900 7d0a 7c04 6a03  ..}.|.d...}.|.j.
-00001990: 6408 1900 7d0b 7c00 6a05 7c07 7406 7c06  d...}.|.j.|.t.|.
-000019a0: 7c05 7c08 7c01 6606 7c03 8e01 7d0c 7c0c  |.|.|.f.|...}.|.
-000019b0: a007 7c09 7c07 7c0a 7c06 7c0b a105 7d0d  ..|.|.|.|.|...}.
-000019c0: 7408 7c0d 7409 6a0a 6409 8d02 5300 7408  t.|.t.j.d...S.t.
-000019d0: 7c04 6a0b 7409 6a0c 6409 8d02 5300 290a  |.j.t.j.d...S.).
-000019e0: 4e72 4800 0000 5472 3200 0000 7230 0000  NrH...Tr2...r0..
-000019f0: 0072 2800 0000 7249 0000 0072 2d00 0000  .r(...rI...r-...
-00001a00: da08 6772 6f75 705f 6279 7207 0000 0029  ..group_byr....)
-00001a10: 0d72 1200 0000 7245 0000 0072 4a00 0000  .r....rE...rJ...
-00001a20: 724b 0000 0072 2900 0000 7236 0000 0072  rK...r)...r6...r
-00001a30: 0d00 0000 da18 6765 745f 6772 6f75 7065  ......get_groupe
-00001a40: 645f 6d61 705f 636f 6e74 656e 7473 7205  d_map_contentsr.
-00001a50: 0000 0072 0800 0000 724d 0000 0072 4e00  ...r....rM...rN.
-00001a60: 0000 724f 0000 0029 0e72 1600 0000 7217  ..rO...).r....r.
-00001a70: 0000 0072 1800 0000 7219 0000 0072 5000  ...r....r....rP.
-00001a80: 0000 7233 0000 0072 3200 0000 7230 0000  ..r3...r2...r0..
-00001a90: 0072 2800 0000 7249 0000 0072 2d00 0000  .r(...rI...r-...
-00001aa0: 7269 0000 0072 4300 0000 da06 6772 6f75  ri...rC.....grou
-00001ab0: 7073 721a 0000 0072 1a00 0000 721b 0000  psr....r....r...
-00001ac0: 0072 5200 0000 fd00 0000 7322 0000 0000  .rR.......s"....
-00001ad0: 020c 0208 0204 010a 010a 0110 020a 0108  ................
-00001ae0: 020a 020e 0102 ff02 0102 ff04 0312 020e  ................
-00001af0: 027a 1a47 6574 4772 6f75 7065 644d 6170  .z.GetGroupedMap
-00001b00: 436f 6e74 656e 7473 2e70 6f73 744e 7257  Contents.postNrW
-00001b10: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
-00001b20: 0000 721b 0000 0072 6800 0000 fb00 0000  ..r....rh.......
-00001b30: 7302 0000 0008 0272 6800 0000 2921 da0b  s......rh...)!..
-00001b40: 646a 616e 676f 2e63 6f72 6572 0200 0000  django.corer....
-00001b50: da14 7265 7374 5f66 7261 6d65 776f 726b  ..rest_framework
-00001b60: 2e76 6965 7773 7203 0000 005a 1772 6573  .viewsr....Z.res
-00001b70: 745f 6672 616d 6577 6f72 6b2e 7265 7370  t_framework.resp
-00001b80: 6f6e 7365 7205 0000 005a 1872 6573 745f  onser....Z.rest_
-00001b90: 6672 616d 6577 6f72 6b2e 7265 6e64 6572  framework.render
-00001ba0: 6572 7372 0600 0000 da0e 7265 7374 5f66  ersr......rest_f
-00001bb0: 7261 6d65 776f 726b 7208 0000 00da 1761  rameworkr......a
-00001bc0: 6e79 636c 7573 7465 722e 4d61 7043 6c75  nycluster.MapClu
-00001bd0: 7374 6572 6572 7209 0000 00da 1661 6e79  stererr......any
-00001be0: 636c 7573 7465 722e 6465 6669 6e69 7469  cluster.definiti
-00001bf0: 6f6e 7372 0a00 0000 720b 0000 0072 0c00  onsr....r....r..
-00001c00: 0000 720d 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00001c10: 0072 1100 0000 7212 0000 00da 0a61 6e79  .r....r......any
-00001c20: 636c 7573 7465 7272 1300 0000 723e 0000  clusterr....r>..
-00001c30: 0072 1400 0000 7221 0000 0072 4700 0000  .r....r!...rG...
-00001c40: 7254 0000 0072 5800 0000 725f 0000 0072  rT...rX...r_...r
-00001c50: 6100 0000 7265 0000 0072 6800 0000 721a  a...re...rh...r.
-00001c60: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
-00001c70: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001c80: 7324 0000 000c 020c 010c 010c 010c 020c  s$..............
-00001c90: 0118 0218 030c 0208 0210 060e 3412 2012  ............4. .
-00001ca0: 1e12 2512 1c12 1512 1b                   ..%......
+00000080: 6d0e 5a0e 0100 6400 6408 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
+00000090: 6d11 5a11 6d12 5a12 6d13 5a13 0100 6409  m.Z.m.Z.m.Z...d.
+000000a0: 640a 6c03 6d14 5a14 6d15 5a15 6d16 5a16  d.l.m.Z.m.Z.m.Z.
+000000b0: 6d17 5a17 6d18 5a18 0100 6400 640b 6c19  m.Z.m.Z...d.d.l.
+000000c0: 6d1a 5a1a 0100 6400 640c 6c1b 6d1c 5a1c  m.Z...d.d.l.m.Z.
+000000d0: 0100 651d 6501 640d 640e 8303 5a1e 651c  ..e.e.d.d...Z.e.
+000000e0: 651e 8301 5a1f 6400 640f 6c20 5a20 4700  e...Z.d.d.l Z G.
+000000f0: 6410 6411 8400 6411 6505 8303 5a21 4700  d.d...d.e...Z!G.
+00000100: 6412 6413 8400 6413 8302 5a22 4700 6414  d.d...d...Z"G.d.
+00000110: 6415 8400 6415 6522 6505 8304 5a23 4700  d...d.e"e...Z#G.
+00000120: 6416 6417 8400 6417 6522 6505 8304 5a24  d.d...d.e"e...Z$
+00000130: 4700 6418 6419 8400 6419 6522 6505 8304  G.d.d...d.e"e...
+00000140: 5a25 4700 641a 641b 8400 641b 6522 6505  Z%G.d.d...d.e"e.
+00000150: 8304 5a26 4700 641c 641d 8400 641d 6522  ..Z&G.d.d...d.e"
+00000160: 6505 8304 5a27 4700 641e 641f 8400 641f  e...Z'G.d.d...d.
+00000170: 6522 6505 8304 5a28 4700 6420 6421 8400  e"e...Z(G.d d!..
+00000180: 6421 6522 6505 8304 5a29 640f 5300 2922  d!e"e...Z)d.S.)"
+00000190: e900 0000 0029 01da 0873 6574 7469 6e67  .....)...setting
+000001a0: 7329 01da 0b73 6572 6961 6c69 7a65 7273  s)...serializers
+000001b0: 2901 da07 4150 4956 6965 77a9 01da 0852  )...APIView....R
+000001c0: 6573 706f 6e73 6529 01da 0c4a 534f 4e52  esponse)...JSONR
+000001d0: 656e 6465 7265 72a9 01da 0673 7461 7475  enderer....statu
+000001e0: 7329 02da 0c4d 6170 436c 7573 7465 7265  s)...MapClustere
+000001f0: 72da 0347 6973 2904 da16 4745 4f4d 4554  r..Gis)...GEOMET
+00000200: 5259 5f54 5950 455f 5649 4557 504f 5254  RY_TYPE_VIEWPORT
+00000210: da12 4745 4f4d 4554 5259 5f54 5950 455f  ..GEOMETRY_TYPE_
+00000220: 4152 4541 da11 434c 5553 5445 525f 5459  AREA..CLUSTER_TY
+00000230: 5045 5f47 5249 44da 1343 4c55 5354 4552  PE_GRID..CLUSTER
+00000240: 5f54 5950 455f 4b4d 4541 4e53 e901 0000  _TYPE_KMEANS....
+00000250: 0029 05da 1843 6c75 7374 6572 5265 7175  .)...ClusterRequ
+00000260: 6573 7453 6572 6961 6c69 7a65 72da 1f43  estSerializer..C
+00000270: 6c75 7374 6572 436f 6e74 656e 7452 6571  lusterContentReq
+00000280: 7565 7374 5365 7269 616c 697a 6572 da19  uestSerializer..
+00000290: 4d61 7043 6f6e 7465 6e74 436f 756e 7453  MapContentCountS
+000002a0: 6572 6961 6c69 7a65 72da 1b47 726f 7570  erializer..Group
+000002b0: 6564 4d61 7043 6f6e 7465 6e74 5365 7269  edMapContentSeri
+000002c0: 616c 697a 6572 da1c 4172 6561 436f 6e74  alizer..AreaCont
+000002d0: 656e 7452 6571 7565 7374 5365 7269 616c  entRequestSerial
+000002e0: 697a 6572 2901 da0c 436c 7573 7465 7243  izer)...ClusterC
+000002f0: 6163 6865 2901 da0d 696d 706f 7274 5f6d  ache)...import_m
+00000300: 6f64 756c 655a 1f41 4e59 434c 5553 5445  oduleZ.ANYCLUSTE
+00000310: 525f 4749 535f 4d4f 4445 4c5f 5345 5249  R_GIS_MODEL_SERI
+00000320: 414c 495a 4552 7a2d 616e 7963 6c75 7374  ALIZERz-anyclust
+00000330: 6572 2e61 7069 2e73 6572 6961 6c69 7a65  er.api.serialize
+00000340: 7273 2e47 6973 4d6f 6465 6c53 6572 6961  rs.GisModelSeria
+00000350: 6c69 7a65 724e 6300 0000 0000 0000 0000  lizerNc.........
+00000360: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+00000370: 1400 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
+00000380: 8400 5a03 6403 5300 2904 da07 4150 4948  ..Z.d.S.)...APIH
+00000390: 6f6d 6563 0200 0000 0000 0000 0000 0000  omec............
+000003a0: 0400 0000 0300 0000 4f00 0000 730c 0000  ........O...s...
+000003b0: 0074 0064 0164 0269 0183 0153 0029 034e  .t.d.d.i...S.).N
+000003c0: da07 7375 6363 6573 7354 7205 0000 0029  ..successTr....)
+000003d0: 04da 0473 656c 66da 0772 6571 7565 7374  ...self..request
+000003e0: da04 6172 6773 da06 6b77 6172 6773 a900  ..args..kwargs..
+000003f0: 721e 0000 00fa 382f 686f 6d65 2f74 6f6d  r.....8/home/tom
+00000400: 2f61 6e79 636c 7573 7465 722f 6465 6d6f  /anycluster/demo
+00000410: 2f64 6a61 6e67 6f2f 616e 7963 6c75 7374  /django/anyclust
+00000420: 6572 2f61 7069 2f76 6965 7773 2e70 79da  er/api/views.py.
+00000430: 0367 6574 1900 0000 7302 0000 0000 017a  .get....s......z
+00000440: 0b41 5049 486f 6d65 2e67 6574 4ea9 04da  .APIHome.getN...
+00000450: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000460: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000470: 655f 5f72 2000 0000 721e 0000 0072 1e00  e__r ...r....r..
+00000480: 0000 721e 0000 0072 1f00 0000 7218 0000  ..r....r....r...
+00000490: 0017 0000 0073 0200 0000 0802 7218 0000  .....s......r...
+000004a0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000004b0: 0000 0200 0000 4000 0000 7340 0000 0065  ......@...s@...e
+000004c0: 005a 0164 005a 0264 015a 0364 0264 0384  .Z.d.Z.d.Z.d.d..
+000004d0: 005a 0464 0464 0584 005a 0564 0664 0784  .Z.d.d...Z.d.d..
+000004e0: 005a 0664 0864 0984 005a 0764 0a64 0b84  .Z.d.d...Z.d.d..
+000004f0: 005a 0864 0c64 0d84 005a 0964 0e53 0029  .Z.d.d...Z.d.S.)
+00000500: 0fda 124d 6170 436c 7573 7465 7256 6965  ...MapClusterVie
+00000510: 7742 6173 655a 1061 6e79 636c 7573 7465  wBaseZ.anycluste
+00000520: 725f 6361 6368 6563 0200 0000 0000 0000  r_cachec........
+00000530: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+00000540: 7316 0000 0074 007c 01a0 0164 01a1 0164  s....t.|...d...d
+00000550: 0219 0083 017d 027c 0253 0029 034e fa01  .....}.|.S.).N..
+00000560: 3ae9 ffff ffff 2902 da03 696e 74da 0573  :.....)...int..s
+00000570: 706c 6974 2903 721a 0000 005a 0873 7269  plit).r....Z.sri
+00000580: 645f 7374 72da 0b6f 7574 7075 745f 7372  d_str..output_sr
+00000590: 6964 721e 0000 0072 1e00 0000 721f 0000  idr....r....r...
+000005a0: 00da 0a70 6172 7365 5f73 7269 6421 0000  ...parse_srid!..
+000005b0: 0073 0400 0000 0001 1201 7a1d 4d61 7043  .s........z.MapC
+000005c0: 6c75 7374 6572 5669 6577 4261 7365 2e70  lusterViewBase.p
+000005d0: 6172 7365 5f73 7269 6463 0200 0000 0000  arse_sridc......
+000005e0: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+000005f0: 0000 7304 0000 0064 0153 0029 024e da06  ..s....d.S.).N..
+00000600: 7075 626c 6963 721e 0000 0029 0272 1a00  publicr....).r..
+00000610: 0000 721b 0000 0072 1e00 0000 721e 0000  ..r....r....r...
+00000620: 0072 1f00 0000 da0f 6765 745f 7363 6865  .r......get_sche
+00000630: 6d61 5f6e 616d 6526 0000 0073 0200 0000  ma_name&...s....
+00000640: 0001 7a22 4d61 7043 6c75 7374 6572 5669  ..z"MapClusterVi
+00000650: 6577 4261 7365 2e67 6574 5f73 6368 656d  ewBase.get_schem
+00000660: 615f 6e61 6d65 6307 0000 0000 0000 0000  a_namec.........
+00000670: 0000 000d 0000 0007 0000 004b 0000 0073  ...........K...s
+00000680: 5800 0000 7c07 6401 1900 7d08 7c07 6402  X...|.d...}.|.d.
+00000690: 1900 7d09 7c04 6403 6b02 7228 7400 7c01  ..}.|.d.k.r(t.|.
+000006a0: 7c09 7c02 7c03 8304 7d0a 6e12 7c00 a001  |.|.|...}.n.|...
+000006b0: 7c01 7c09 7c02 7c06 7c03 a105 7d0a 7c00  |.|.|.|.|...}.|.
+000006c0: a002 7c06 a101 7d0b 7403 7c0a 7c08 7c05  ..|...}.t.|.|.|.
+000006d0: 7c0b 6404 8d04 7d0c 7c0c 5300 2905 4eda  |.d...}.|.S.).N.
+000006e0: 0967 7269 645f 7369 7a65 da04 7a6f 6f6d  .grid_size..zoom
+000006f0: 5429 0372 2e00 0000 722a 0000 00da 0b73  T).r....r*.....s
+00000700: 6368 656d 615f 6e61 6d65 2904 7216 0000  chema_name).r...
+00000710: 00da 0967 6574 5f63 6163 6865 722d 0000  ...get_cacher-..
+00000720: 0072 0a00 0000 290d 721a 0000 00da 0d67  .r....).r......g
+00000730: 656f 6d65 7472 795f 7479 7065 da0b 636c  eometry_type..cl
+00000740: 7573 7465 7274 7970 65da 0766 696c 7465  ustertype..filte
+00000750: 7273 da0b 636c 6561 725f 6361 6368 6572  rs..clear_cacher
+00000760: 2a00 0000 721b 0000 0072 1d00 0000 722e  *...r....r....r.
+00000770: 0000 0072 2f00 0000 da0d 636c 7573 7465  ...r/.....cluste
+00000780: 725f 6361 6368 6572 3000 0000 5a09 636c  r_cacher0...Z.cl
+00000790: 7573 7465 7265 7272 1e00 0000 721e 0000  ustererr....r...
+000007a0: 0072 1f00 0000 da11 6765 745f 6d61 705f  .r......get_map_
+000007b0: 636c 7573 7465 7265 722a 0000 0073 1000  clusterer*...s..
+000007c0: 0000 0002 0801 0802 0801 1002 1202 0a01  ................
+000007d0: 1001 7a24 4d61 7043 6c75 7374 6572 5669  ..z$MapClusterVi
+000007e0: 6577 4261 7365 2e67 6574 5f6d 6170 5f63  ewBase.get_map_c
+000007f0: 6c75 7374 6572 6572 6306 0000 0000 0000  lustererc.......
+00000800: 0000 0000 0008 0000 0005 0000 0043 0000  .............C..
+00000810: 0073 2c00 0000 7c04 6a00 a001 7c00 6a02  .s,...|.j...|.j.
+00000820: 6900 a102 7d06 7403 7c01 7c02 7c03 7c05  i...}.t.|.|.|.|.
+00000830: 8304 7d07 7c07 a004 7c06 a101 0100 7c07  ..}.|...|.....|.
+00000840: 5300 a901 4e29 05da 0773 6573 7369 6f6e  S...N)...session
+00000850: 7220 0000 00da 0a63 6163 6865 5f6e 616d  r .....cache_nam
+00000860: 6572 1600 0000 da0f 6c6f 6164 5f67 656f  er......load_geo
+00000870: 6d65 7472 6965 7329 0872 1a00 0000 7232  metries).r....r2
+00000880: 0000 0072 2f00 0000 7233 0000 0072 1b00  ...r/...r3...r..
+00000890: 0000 7234 0000 00da 0663 6163 6865 6472  ..r4.....cachedr
+000008a0: 3600 0000 721e 0000 0072 1e00 0000 721f  6...r....r....r.
+000008b0: 0000 0072 3100 0000 3900 0000 7308 0000  ...r1...9...s...
+000008c0: 0000 0110 010e 020a 017a 1c4d 6170 436c  .........z.MapCl
+000008d0: 7573 7465 7256 6965 7742 6173 652e 6765  usterViewBase.ge
+000008e0: 745f 6361 6368 6563 0300 0000 0000 0000  t_cachec........
+000008f0: 0000 0000 0400 0000 0300 0000 4300 0000  ............C...
+00000900: 7318 0000 007c 02a0 00a1 007d 037c 037c  s....|.....}.|.|
+00000910: 016a 017c 006a 023c 0064 0053 0072 3800  .j.|.j.<.d.S.r8.
+00000920: 0000 2903 da09 7365 7269 616c 697a 6572  ..)...serializer
+00000930: 3900 0000 723a 0000 0029 0472 1a00 0000  9...r:...).r....
+00000940: 721b 0000 0072 3600 0000 5a12 636c 7573  r....r6...Z.clus
+00000950: 7465 725f 6361 6368 655f 6a73 6f6e 721e  ter_cache_jsonr.
+00000960: 0000 0072 1e00 0000 721f 0000 00da 0973  ...r....r......s
+00000970: 6574 5f63 6163 6865 4100 0000 7304 0000  et_cacheA...s...
+00000980: 0000 0108 017a 1c4d 6170 436c 7573 7465  .....z.MapCluste
+00000990: 7256 6965 7742 6173 652e 7365 745f 6361  rViewBase.set_ca
+000009a0: 6368 6563 0300 0000 0000 0000 0000 0000  chec............
+000009b0: 0700 0000 0400 0000 4300 0000 7332 0000  ........C...s2..
+000009c0: 0064 0164 0284 007c 0244 0083 017d 0374  .d.d...|.D...}.t
+000009d0: 006a 016a 027c 0364 038d 017d 0474 037c  .j.j.|.d...}.t.|
+000009e0: 0464 0464 058d 027d 057c 056a 047d 067c  .d.d...}.|.j.}.|
+000009f0: 0653 0029 064e 6301 0000 0000 0000 0000  .S.).Nc.........
+00000a00: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
+00000a10: 1200 0000 6700 7c00 5d0a 7d01 7c01 6a00  ....g.|.].}.|.j.
+00000a20: 9102 7104 5300 721e 0000 0029 01da 0270  ..q.S.r....)...p
+00000a30: 6b29 02da 022e 30da 0169 721e 0000 0072  k)....0..ir....r
+00000a40: 1e00 0000 721f 0000 00da 0a3c 6c69 7374  ....r......<list
+00000a50: 636f 6d70 3e48 0000 0073 0400 0000 0600  comp>H...s......
+00000a60: 0200 7a3f 4d61 7043 6c75 7374 6572 5669  ..z?MapClusterVi
+00000a70: 6577 4261 7365 2e73 6572 6961 6c69 7a65  ewBase.serialize
+00000a80: 5f67 6973 5f6d 6f64 656c 5f6c 6973 742e  _gis_model_list.
+00000a90: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00000aa0: 6d70 3e29 01da 0670 6b5f 5f69 6e54 2901  mp>)...pk__inT).
+00000ab0: da04 6d61 6e79 2905 720b 0000 00da 076f  ..many).r......o
+00000ac0: 626a 6563 7473 da06 6669 6c74 6572 da12  bjects..filter..
+00000ad0: 4769 734d 6f64 656c 5365 7269 616c 697a  GisModelSerializ
+00000ae0: 6572 da04 6461 7461 2907 721a 0000 00da  er..data).r.....
+00000af0: 0d6d 6170 5f63 6c75 7374 6572 6572 5a0e  .map_clustererZ.
+00000b00: 696e 7374 616e 6365 735f 6c69 7374 5a0d  instances_listZ.
+00000b10: 696e 7374 616e 6365 735f 706b 735a 0c67  instances_pksZ.g
+00000b20: 6973 5f71 7565 7279 7365 74da 0a73 6572  is_queryset..ser
+00000b30: 6961 6c69 7a65 7272 4800 0000 721e 0000  ializerrH...r...
+00000b40: 0072 1e00 0000 721f 0000 00da 1873 6572  .r....r......ser
+00000b50: 6961 6c69 7a65 5f67 6973 5f6d 6f64 656c  ialize_gis_model
+00000b60: 5f6c 6973 7446 0000 0073 0a00 0000 0002  _listF...s......
+00000b70: 0e02 0e02 0c01 0602 7a2b 4d61 7043 6c75  ........z+MapClu
+00000b80: 7374 6572 5669 6577 4261 7365 2e73 6572  sterViewBase.ser
+00000b90: 6961 6c69 7a65 5f67 6973 5f6d 6f64 656c  ialize_gis_model
+00000ba0: 5f6c 6973 744e 290a 7222 0000 0072 2300  _listN).r"...r#.
+00000bb0: 0000 7224 0000 0072 3a00 0000 722b 0000  ..r$...r:...r+..
+00000bc0: 0072 2d00 0000 7237 0000 0072 3100 0000  .r-...r7...r1...
+00000bd0: 723e 0000 0072 4b00 0000 721e 0000 0072  r>...rK...r....r
+00000be0: 1e00 0000 721e 0000 0072 1f00 0000 7225  ....r....r....r%
+00000bf0: 0000 001d 0000 0073 0e00 0000 0802 0402  .......s........
+00000c00: 0805 0804 080f 0808 0805 7225 0000 0063  ..........r%...c
+00000c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c20: 0200 0000 4000 0000 7322 0000 0065 005a  ....@...s"...e.Z
+00000c30: 0164 005a 0267 005a 0367 005a 0465 0567  .d.Z.g.Z.g.Z.e.g
+00000c40: 015a 0664 0164 0284 005a 0764 0353 0029  .Z.d.d...Z.d.S.)
+00000c50: 04da 0b47 7269 6443 6c75 7374 6572 6302  ...GridClusterc.
+00000c60: 0000 0000 0000 0000 0000 000c 0000 0007  ................
+00000c70: 0000 004f 0000 0073 9c00 0000 7400 7c01  ...O...s....t.|.
+00000c80: 6a01 6401 8d01 7d04 7c04 a002 a100 728c  j.d...}.|.....r.
+00000c90: 7c04 6a03 6402 1900 7d05 7c00 a004 7c04  |.j.d...}.|...|.
+00000ca0: 6a03 6403 1900 a101 7d06 7c04 6a03 6404  j.d.....}.|.j.d.
+00000cb0: 1900 7d07 7c00 6a05 7406 7407 7c07 7c05  ..}.|.j.t.t.|.|.
+00000cc0: 7c06 7c01 6606 7c03 8e01 7d08 7c04 6a03  |.|.f.|...}.|.j.
+00000cd0: 6405 1900 7d09 7c03 6406 1900 7d0a 7c08  d...}.|.d...}.|.
+00000ce0: a008 7c09 7c0a 7c07 a103 7d0b 7c00 a009  ..|.|.|...}.|...
+00000cf0: 7c01 7c08 6a0a a102 0100 740b 7c0b 740c  |.|.j.....t.|.t.
+00000d00: 6a0d 6407 8d02 5300 740b 7c04 6a0e 740c  j.d...S.t.|.j.t.
+00000d10: 6a0f 6407 8d02 5300 2908 4ea9 0172 4800  j.d...S.).N..rH.
+00000d20: 0000 7235 0000 0072 2a00 0000 7234 0000  ..r5...r*...r4..
+00000d30: 00da 0767 656f 6a73 6f6e 722f 0000 0072  ...geojsonr/...r
+00000d40: 0800 0000 2910 7211 0000 0072 4800 0000  ....).r....rH...
+00000d50: da08 6973 5f76 616c 6964 da0e 7661 6c69  ..is_valid..vali
+00000d60: 6461 7465 645f 6461 7461 722b 0000 0072  dated_datar+...r
+00000d70: 3700 0000 720c 0000 0072 0e00 0000 da0c  7...r....r......
+00000d80: 6772 6964 5f63 6c75 7374 6572 723e 0000  grid_clusterr>..
+00000d90: 0072 3600 0000 7206 0000 0072 0900 0000  .r6...r....r....
+00000da0: da0b 4854 5450 5f32 3030 5f4f 4bda 0665  ..HTTP_200_OK..e
+00000db0: 7272 6f72 73da 1448 5454 505f 3430 305f  rrors..HTTP_400_
+00000dc0: 4241 445f 5245 5155 4553 5429 0c72 1a00  BAD_REQUEST).r..
+00000dd0: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00000de0: 0072 4a00 0000 7235 0000 0072 2a00 0000  .rJ...r5...r*...
+00000df0: 7234 0000 0072 4900 0000 724e 0000 0072  r4...rI...rN...r
+00000e00: 2f00 0000 da04 6772 6964 721e 0000 0072  /.....gridr....r
+00000e10: 1e00 0000 721f 0000 00da 0470 6f73 745b  ....r......post[
+00000e20: 0000 0073 2200 0000 0002 0c02 0802 0a01  ...s"...........
+00000e30: 1002 0a02 0c01 0200 02ff 0201 02ff 0403  ................
+00000e40: 0a01 0802 0e02 0e01 0e02 7a10 4772 6964  ..........z.Grid
+00000e50: 436c 7573 7465 722e 706f 7374 4e29 0872  Cluster.postN).r
+00000e60: 2200 0000 7223 0000 0072 2400 0000 5a16  "...r#...r$...Z.
+00000e70: 6175 7468 656e 7469 6361 7469 6f6e 5f63  authentication_c
+00000e80: 6c61 7373 6573 5a12 7065 726d 6973 7369  lassesZ.permissi
+00000e90: 6f6e 5f63 6c61 7373 6573 7207 0000 005a  on_classesr....Z
+00000ea0: 1072 656e 6465 7265 725f 636c 6173 7365  .renderer_classe
+00000eb0: 7372 5600 0000 721e 0000 0072 1e00 0000  srV...r....r....
+00000ec0: 721e 0000 0072 1f00 0000 724c 0000 0055  r....r....rL...U
+00000ed0: 0000 0073 0800 0000 0802 0401 0401 0602  ...s............
+00000ee0: 724c 0000 0063 0000 0000 0000 0000 0000  rL...c..........
+00000ef0: 0000 0000 0000 0200 0000 4000 0000 7314  ..........@...s.
+00000f00: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+00000f10: 005a 0364 0353 0029 04da 0d4b 6d65 616e  .Z.d.S.)...Kmean
+00000f20: 7343 6c75 7374 6572 6302 0000 0000 0000  sClusterc.......
+00000f30: 0000 0000 000d 0000 0007 0000 004f 0000  .............O..
+00000f40: 0073 a200 0000 7400 7c01 6a01 6401 8d01  .s....t.|.j.d...
+00000f50: 7d04 7c04 a002 a100 7292 7c04 6a03 6402  }.|.....r.|.j.d.
+00000f60: 1900 7d05 7c04 6a03 6403 1900 7d06 7c00  ..}.|.j.d...}.|.
+00000f70: a004 7c04 6a03 6404 1900 a101 7d07 7c04  ..|.j.d.....}.|.
+00000f80: 6a03 6405 1900 7d08 7c00 6a05 7c05 7406  j.d...}.|.j.|.t.
+00000f90: 7c08 7c06 7c07 7c01 6606 7c03 8e01 7d09  |.|.|.|.f.|...}.
+00000fa0: 7c04 6a03 6406 1900 7d0a 7c03 6407 1900  |.j.d...}.|.d...
+00000fb0: 7d0b 7c09 a007 7c0a 7c05 7c0b 7c08 a104  }.|...|.|.|.|...
+00000fc0: 7d0c 7c00 a008 7c01 7c09 6a09 a102 0100  }.|...|.|.j.....
+00000fd0: 740a 7c0c 8301 5300 740a 7c04 6a0b 740c  t.|...S.t.|.j.t.
+00000fe0: 6a0d 6408 8d02 5300 2909 4e72 4d00 0000  j.d...S.).NrM...
+00000ff0: 7232 0000 0072 3500 0000 722a 0000 0072  r2...r5...r*...r
+00001000: 3400 0000 724e 0000 0072 2f00 0000 7208  4...rN...r/...r.
+00001010: 0000 0029 0e72 1100 0000 7248 0000 0072  ...).r....rH...r
+00001020: 4f00 0000 7250 0000 0072 2b00 0000 7237  O...rP...r+...r7
+00001030: 0000 0072 0f00 0000 da0e 6b6d 6561 6e73  ...r......kmeans
+00001040: 5f63 6c75 7374 6572 723e 0000 0072 3600  _clusterr>...r6.
+00001050: 0000 7206 0000 0072 5300 0000 7209 0000  ..r....rS...r...
+00001060: 0072 5400 0000 290d 721a 0000 0072 1b00  .rT...).r....r..
+00001070: 0000 721c 0000 0072 1d00 0000 724a 0000  ..r....r....rJ..
+00001080: 0072 3200 0000 7235 0000 0072 2a00 0000  .r2...r5...r*...
+00001090: 7234 0000 0072 4900 0000 724e 0000 0072  r4...rI...rN...r
+000010a0: 2f00 0000 da07 6d61 726b 6572 7372 1e00  /.....markersr..
+000010b0: 0000 721e 0000 0072 1f00 0000 7256 0000  ..r....r....rV..
+000010c0: 0077 0000 0073 2200 0000 0002 0c02 0802  .w...s".........
+000010d0: 0a01 0a01 1002 0a02 0e01 02ff 0201 02ff  ................
+000010e0: 0403 0a01 0802 1001 0e01 0802 7a12 4b6d  ............z.Km
+000010f0: 6561 6e73 436c 7573 7465 722e 706f 7374  eansCluster.post
+00001100: 4ea9 0472 2200 0000 7223 0000 0072 2400  N..r"...r#...r$.
+00001110: 0000 7256 0000 0072 1e00 0000 721e 0000  ..rV...r....r...
+00001120: 0072 1e00 0000 721f 0000 0072 5700 0000  .r....r....rW...
+00001130: 7500 0000 7302 0000 0008 0272 5700 0000  u...s......rW...
+00001140: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00001150: 0002 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
+00001160: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
+00001170: 5300 2904 da11 4765 7443 6c75 7374 6572  S.)...GetCluster
+00001180: 436f 6e74 656e 7463 0200 0000 0000 0000  Contentc........
+00001190: 0000 0000 1000 0000 0900 0000 4f00 0000  ............O...
+000011a0: 73c2 0000 0074 007c 016a 0164 018d 017d  s....t.|.j.d...}
+000011b0: 047c 04a0 02a1 0072 b27c 046a 0364 0219  .|.....r.|.j.d..
+000011c0: 007d 057c 00a0 047c 046a 0364 0319 00a1  .}.|...|.j.d....
+000011d0: 017d 067c 00a0 047c 046a 0364 0419 00a1  .}.|...|.j.d....
+000011e0: 017d 077c 046a 0364 0519 007d 087c 006a  .}.|.j.d...}.|.j
+000011f0: 057c 0574 067c 0864 067c 067c 0166 067c  .|.t.|.d.|.|.f.|
+00001200: 038e 017d 097c 046a 0364 0719 007d 0a7c  ...}.|.j.d...}.|
+00001210: 046a 0364 0819 007d 0b7c 046a 0364 0919  .j.d...}.|.j.d..
+00001220: 007d 0c7c 0364 0a19 007d 0d7c 096a 077c  .}.|.d...}.|.j.|
+00001230: 057c 0a7c 0b7c 0c7c 087c 0d7c 0764 0b8d  .|.|.|.|.|.|.d..
+00001240: 077d 0e7c 00a0 087c 097c 0ea1 027d 0f74  .}.|...|.|...}.t
+00001250: 097c 0f83 0153 0074 097c 046a 0a74 0b6a  .|...S.t.|.j.t.j
+00001260: 0c64 0c8d 0253 0029 0d4e 724d 0000 0072  .d...S.).NrM...r
+00001270: 3200 0000 722a 0000 00da 0a69 6e70 7574  2...r*.....input
+00001280: 5f73 7269 6472 3400 0000 46da 0369 6473  _sridr4...F..ids
+00001290: da01 78da 0179 722f 0000 0029 0172 5c00  ..x..yr/...).r\.
+000012a0: 0000 7208 0000 0029 0d72 1200 0000 7248  ..r....).r....rH
+000012b0: 0000 0072 4f00 0000 7250 0000 0072 2b00  ...rO...rP...r+.
+000012c0: 0000 7237 0000 0072 0f00 0000 da1a 6765  ..r7...r......ge
+000012d0: 745f 6b6d 6561 6e73 5f63 6c75 7374 6572  t_kmeans_cluster
+000012e0: 5f63 6f6e 7465 6e74 724b 0000 0072 0600  _contentrK...r..
+000012f0: 0000 7253 0000 0072 0900 0000 7254 0000  ..rS...r....rT..
+00001300: 0029 1072 1a00 0000 721b 0000 0072 1c00  .).r....r....r..
+00001310: 0000 721d 0000 0072 4a00 0000 7232 0000  ..r....rJ...r2..
+00001320: 0072 2a00 0000 725c 0000 0072 3400 0000  .r*...r\...r4...
+00001330: 7249 0000 0072 5d00 0000 725e 0000 0072  rI...r]...r^...r
+00001340: 5f00 0000 722f 0000 005a 0f63 6c75 7374  _...r/...Z.clust
+00001350: 6572 5f63 6f6e 7465 6e74 7248 0000 0072  er_contentrH...r
+00001360: 1e00 0000 721e 0000 0072 1f00 0000 7256  ....r....r....rV
+00001370: 0000 0095 0000 0073 2a00 0000 0002 0c02  .......s*.......
+00001380: 0802 0a01 1001 1002 0a02 0e01 02ff 0201  ................
+00001390: 02ff 0403 0a01 0a01 0a02 0802 1001 02ff  ................
+000013a0: 0603 0c02 0802 7a16 4765 7443 6c75 7374  ......z.GetClust
+000013b0: 6572 436f 6e74 656e 742e 706f 7374 4e72  erContent.postNr
+000013c0: 5a00 0000 721e 0000 0072 1e00 0000 721e  Z...r....r....r.
+000013d0: 0000 0072 1f00 0000 725b 0000 0093 0000  ...r....r[......
+000013e0: 0073 0200 0000 0802 725b 0000 0063 0000  .s......r[...c..
+000013f0: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+00001400: 0000 4000 0000 7314 0000 0065 005a 0164  ..@...s....e.Z.d
+00001410: 005a 0264 0164 0284 005a 0364 0353 0029  .Z.d.d...Z.d.S.)
+00001420: 04da 0e47 6574 4172 6561 436f 6e74 656e  ...GetAreaConten
+00001430: 7463 0200 0000 0000 0000 0000 0000 0e00  tc..............
+00001440: 0000 0700 0000 4f00 0000 73aa 0000 0074  ......O...s....t
+00001450: 007c 016a 0164 018d 017d 047c 04a0 02a1  .|.j.d...}.|....
+00001460: 0072 9a7c 046a 0364 0219 007d 057c 00a0  .r.|.j.d...}.|..
+00001470: 047c 046a 0364 0319 00a1 017d 067c 046a  .|.j.d.....}.|.j
+00001480: 03a0 0564 0464 00a1 027d 077c 046a 03a0  ...d.d...}.|.j..
+00001490: 0564 0564 00a1 027d 087c 046a 0364 0619  .d.d...}.|.j.d..
+000014a0: 007d 097c 006a 067c 0574 077c 0964 077c  .}.|.j.|.t.|.d.|
+000014b0: 067c 0166 067c 038e 017d 0a7c 046a 0364  .|.f.|...}.|.j.d
+000014c0: 0819 007d 0b7c 0aa0 087c 0b7c 097c 077c  ...}.|...|.|.|.|
+000014d0: 08a1 047d 0c7c 00a0 097c 0a7c 0ca1 027d  ...}.|...|.|...}
+000014e0: 0d74 0a7c 0d83 0153 0074 0a7c 046a 0b74  .t.|...S.t.|.j.t
+000014f0: 0c6a 0d64 098d 0253 0029 0a4e 724d 0000  .j.d...S.).NrM..
+00001500: 0072 3200 0000 722a 0000 00da 056c 696d  .r2...r*.....lim
+00001510: 6974 da06 6f66 6673 6574 7234 0000 0046  it..offsetr4...F
+00001520: 724e 0000 0072 0800 0000 290e 7215 0000  rN...r....).r...
+00001530: 0072 4800 0000 724f 0000 0072 5000 0000  .rH...rO...rP...
+00001540: 722b 0000 0072 2000 0000 7237 0000 0072  r+...r ...r7...r
+00001550: 0f00 0000 da10 6765 745f 6172 6561 5f63  ......get_area_c
+00001560: 6f6e 7465 6e74 724b 0000 0072 0600 0000  ontentrK...r....
+00001570: 7253 0000 0072 0900 0000 7254 0000 0029  rS...r....rT...)
+00001580: 0e72 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00001590: 721d 0000 0072 4a00 0000 7232 0000 0072  r....rJ...r2...r
+000015a0: 2a00 0000 7262 0000 0072 6300 0000 7234  *...rb...rc...r4
+000015b0: 0000 0072 4900 0000 724e 0000 005a 0c61  ...rI...rN...Z.a
+000015c0: 7265 615f 636f 6e74 656e 7472 4800 0000  rea_contentrH...
+000015d0: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+000015e0: 5600 0000 ba00 0000 7322 0000 0000 020c  V.......s"......
+000015f0: 0208 020a 0110 020e 010e 020a 020e 0102  ................
+00001600: ff02 0102 ff04 030a 0210 020c 0208 027a  ...............z
+00001610: 1347 6574 4172 6561 436f 6e74 656e 742e  .GetAreaContent.
+00001620: 706f 7374 4e72 5a00 0000 721e 0000 0072  postNrZ...r....r
+00001630: 1e00 0000 721e 0000 0072 1f00 0000 7261  ....r....r....ra
+00001640: 0000 00b8 0000 0073 0200 0000 0802 7261  .......s......ra
+00001650: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001660: 0000 0000 0200 0000 4000 0000 7314 0000  ........@...s...
+00001670: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+00001680: 0364 0353 0029 04da 1147 6574 4461 7461  .d.S.)...GetData
+00001690: 7365 7443 6f6e 7465 6e74 6302 0000 0000  setContentc.....
+000016a0: 0000 0000 0000 000b 0000 0007 0000 004f  ...............O
+000016b0: 0000 0073 5200 0000 7c01 6a00 a001 6401  ...sR...|.j...d.
+000016c0: 6402 a102 7d04 6700 7d05 7c00 6a02 7403  d...}.g.}.|.j.t.
+000016d0: 7404 7c05 6403 7c04 7c01 6606 7c03 8e01  t.|.d.|.|.f.|...
+000016e0: 7d06 7c03 6404 1900 7d07 7c06 a005 7c07  }.|.d...}.|...|.
+000016f0: a101 7d08 7406 7c08 8301 7d09 7c09 6a07  ..}.t.|...}.|.j.
+00001700: 7d0a 7408 7c0a 8301 5300 2905 4e72 2a00  }.t.|...S.).Nr*.
+00001710: 0000 69e6 1000 0046 da0a 6461 7461 7365  ..i....F..datase
+00001720: 745f 6964 2909 da03 4745 5472 2000 0000  t_id)...GETr ...
+00001730: 7237 0000 0072 0c00 0000 720e 0000 00da  r7...r....r.....
+00001740: 1367 6574 5f64 6174 6173 6574 5f63 6f6e  .get_dataset_con
+00001750: 7465 6e74 7247 0000 0072 4800 0000 7206  tentrG...rH...r.
+00001760: 0000 0029 0b72 1a00 0000 721b 0000 0072  ...).r....r....r
+00001770: 1c00 0000 721d 0000 0072 2a00 0000 7234  ....r....r*...r4
+00001780: 0000 0072 4900 0000 7266 0000 005a 0764  ...rI...rf...Z.d
+00001790: 6174 6173 6574 724a 0000 0072 4800 0000  atasetrJ...rH...
+000017a0: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+000017b0: 2000 0000 d900 0000 7318 0000 0000 020e   .......s.......
+000017c0: 0204 020e 0102 ff02 0102 ff04 0308 020a  ................
+000017d0: 0208 0106 027a 1547 6574 4461 7461 7365  .....z.GetDatase
+000017e0: 7443 6f6e 7465 6e74 2e67 6574 4e72 2100  tContent.getNr!.
+000017f0: 0000 721e 0000 0072 1e00 0000 721e 0000  ..r....r....r...
+00001800: 0072 1f00 0000 7265 0000 00d7 0000 0073  .r....re.......s
+00001810: 0200 0000 0802 7265 0000 0063 0000 0000  ......re...c....
+00001820: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00001830: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00001840: 0264 0164 0284 005a 0364 0353 0029 04da  .d.d...Z.d.S.)..
+00001850: 1247 6574 4d61 7043 6f6e 7465 6e74 436f  .GetMapContentCo
+00001860: 756e 7463 0200 0000 0000 0000 0000 0000  untc............
+00001870: 0e00 0000 0700 0000 4f00 0000 73a0 0000  ........O...s...
+00001880: 0074 007c 016a 0164 018d 017d 047c 04a0  .t.|.j.d...}.|..
+00001890: 02a1 0072 9064 027d 057c 046a 0364 0319  ...r.d.}.|.j.d..
+000018a0: 007d 067c 046a 0364 0419 007d 077c 00a0  .}.|.j.d...}.|..
+000018b0: 047c 046a 0364 0519 00a1 017d 087c 046a  .|.j.d.....}.|.j
+000018c0: 0364 0619 007d 097c 0364 0719 007d 0a7c  .d...}.|.d...}.|
+000018d0: 046a 0364 0819 007d 0b7c 006a 057c 0774  .j.d...}.|.j.|.t
+000018e0: 067c 067c 057c 087c 0166 067c 038e 017d  .|.|.|.|.f.|...}
+000018f0: 0c7c 0ca0 077c 097c 077c 067c 0a7c 0ba1  .|...|.|.|.|.|..
+00001900: 057d 0d74 087c 0d74 096a 0a64 098d 0253  .}.t.|.t.j.d...S
+00001910: 0074 087c 046a 0b74 096a 0c64 098d 0253  .t.|.j.t.j.d...S
+00001920: 0029 0a4e 724d 0000 0054 7234 0000 0072  .).NrM...Tr4...r
+00001930: 3200 0000 722a 0000 0072 4e00 0000 722f  2...r*...rN...r/
+00001940: 0000 00da 0b6d 6f64 756c 6174 696f 6e73  .....modulations
+00001950: 7208 0000 0029 0d72 1300 0000 7248 0000  r....).r....rH..
+00001960: 0072 4f00 0000 7250 0000 0072 2b00 0000  .rO...rP...r+...
+00001970: 7237 0000 0072 0f00 0000 5a16 6765 745f  r7...r....Z.get_
+00001980: 6d61 705f 636f 6e74 656e 745f 636f 756e  map_content_coun
+00001990: 7473 7206 0000 0072 0900 0000 7252 0000  tsr....r....rR..
+000019a0: 0072 5300 0000 7254 0000 0029 0e72 1a00  .rS...rT...).r..
+000019b0: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+000019c0: 0072 4a00 0000 7235 0000 0072 3400 0000  .rJ...r5...r4...
+000019d0: 7232 0000 0072 2a00 0000 724e 0000 0072  r2...r*...rN...r
+000019e0: 2f00 0000 726a 0000 0072 4900 0000 5a12  /...rj...rI...Z.
+000019f0: 6d61 705f 636f 6e74 656e 745f 636f 756e  map_content_coun
+00001a00: 7473 721e 0000 0072 1e00 0000 721f 0000  tsr....r....r...
+00001a10: 0072 5600 0000 ee00 0000 7322 0000 0000  .rV.......s"....
+00001a20: 020c 0208 0204 010a 010a 0110 020a 0108  ................
+00001a30: 010a 020e 0102 ff02 0102 ff04 0312 020e  ................
+00001a40: 027a 1747 6574 4d61 7043 6f6e 7465 6e74  .z.GetMapContent
+00001a50: 436f 756e 742e 706f 7374 4e72 5a00 0000  Count.postNrZ...
+00001a60: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
+00001a70: 1f00 0000 7269 0000 00ec 0000 0073 0200  ....ri.......s..
+00001a80: 0000 0802 7269 0000 0063 0000 0000 0000  ....ri...c......
+00001a90: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00001aa0: 0000 7314 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00001ab0: 0164 0284 005a 0364 0353 0029 04da 1547  .d...Z.d.S.)...G
+00001ac0: 6574 4772 6f75 7065 644d 6170 436f 6e74  etGroupedMapCont
+00001ad0: 656e 7473 6302 0000 0000 0000 0000 0000  entsc...........
+00001ae0: 000e 0000 0007 0000 004f 0000 0073 a000  .........O...s..
+00001af0: 0000 7400 7c01 6a01 6401 8d01 7d04 7c04  ..t.|.j.d...}.|.
+00001b00: a002 a100 7290 6402 7d05 7c04 6a03 6403  ....r.d.}.|.j.d.
+00001b10: 1900 7d06 7c04 6a03 6404 1900 7d07 7c00  ..}.|.j.d...}.|.
+00001b20: a004 7c04 6a03 6405 1900 a101 7d08 7c04  ..|.j.d.....}.|.
+00001b30: 6a03 6406 1900 7d09 7c03 6407 1900 7d0a  j.d...}.|.d...}.
+00001b40: 7c04 6a03 6408 1900 7d0b 7c00 6a05 7c07  |.j.d...}.|.j.|.
+00001b50: 7406 7c06 7c05 7c08 7c01 6606 7c03 8e01  t.|.|.|.|.f.|...
+00001b60: 7d0c 7c0c a007 7c09 7c07 7c0a 7c06 7c0b  }.|...|.|.|.|.|.
+00001b70: a105 7d0d 7408 7c0d 7409 6a0a 6409 8d02  ..}.t.|.t.j.d...
+00001b80: 5300 7408 7c04 6a0b 7409 6a0c 6409 8d02  S.t.|.j.t.j.d...
+00001b90: 5300 290a 4e72 4d00 0000 5472 3400 0000  S.).NrM...Tr4...
+00001ba0: 7232 0000 0072 2a00 0000 724e 0000 0072  r2...r*...rN...r
+00001bb0: 2f00 0000 da08 6772 6f75 705f 6279 7208  /.....group_byr.
+00001bc0: 0000 0029 0d72 1400 0000 7248 0000 0072  ...).r....rH...r
+00001bd0: 4f00 0000 7250 0000 0072 2b00 0000 7237  O...rP...r+...r7
+00001be0: 0000 0072 0f00 0000 da18 6765 745f 6772  ...r......get_gr
+00001bf0: 6f75 7065 645f 6d61 705f 636f 6e74 656e  ouped_map_conten
+00001c00: 7473 7206 0000 0072 0900 0000 7252 0000  tsr....r....rR..
+00001c10: 0072 5300 0000 7254 0000 0029 0e72 1a00  .rS...rT...).r..
+00001c20: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00001c30: 0072 4a00 0000 7235 0000 0072 3400 0000  .rJ...r5...r4...
+00001c40: 7232 0000 0072 2a00 0000 724e 0000 0072  r2...r*...rN...r
+00001c50: 2f00 0000 726c 0000 0072 4900 0000 da06  /...rl...rI.....
+00001c60: 6772 6f75 7073 721e 0000 0072 1e00 0000  groupsr....r....
+00001c70: 721f 0000 0072 5600 0000 0901 0000 7322  r....rV.......s"
+00001c80: 0000 0000 020c 0208 0204 010a 010a 0110  ................
+00001c90: 020a 0108 020a 020e 0102 ff02 0102 ff04  ................
+00001ca0: 0312 020e 027a 1a47 6574 4772 6f75 7065  .....z.GetGroupe
+00001cb0: 644d 6170 436f 6e74 656e 7473 2e70 6f73  dMapContents.pos
+00001cc0: 744e 725a 0000 0072 1e00 0000 721e 0000  tNrZ...r....r...
+00001cd0: 0072 1e00 0000 721f 0000 0072 6b00 0000  .r....r....rk...
+00001ce0: 0701 0000 7302 0000 0008 0272 6b00 0000  ....s......rk...
+00001cf0: 292a da0b 646a 616e 676f 2e63 6f6e 6672  )*..django.confr
+00001d00: 0200 0000 da0b 646a 616e 676f 2e63 6f72  ......django.cor
+00001d10: 6572 0300 0000 5a14 7265 7374 5f66 7261  er....Z.rest_fra
+00001d20: 6d65 776f 726b 2e76 6965 7773 7204 0000  mework.viewsr...
+00001d30: 005a 1772 6573 745f 6672 616d 6577 6f72  .Z.rest_framewor
+00001d40: 6b2e 7265 7370 6f6e 7365 7206 0000 005a  k.responser....Z
+00001d50: 1872 6573 745f 6672 616d 6577 6f72 6b2e  .rest_framework.
+00001d60: 7265 6e64 6572 6572 7372 0700 0000 da0e  renderersr......
+00001d70: 7265 7374 5f66 7261 6d65 776f 726b 7209  rest_frameworkr.
+00001d80: 0000 005a 1761 6e79 636c 7573 7465 722e  ...Z.anycluster.
+00001d90: 4d61 7043 6c75 7374 6572 6572 720a 0000  MapClustererr...
+00001da0: 0072 0b00 0000 da16 616e 7963 6c75 7374  .r......anyclust
+00001db0: 6572 2e64 6566 696e 6974 696f 6e73 720c  er.definitionsr.
+00001dc0: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
+00001dd0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00001de0: 0072 1400 0000 7215 0000 00da 0a61 6e79  .r....r......any
+00001df0: 636c 7573 7465 7272 1600 0000 5a10 616e  clusterr....Z.an
+00001e00: 7963 6c75 7374 6572 2e75 7469 6c73 7217  ycluster.utilsr.
+00001e10: 0000 00da 0767 6574 6174 7472 5a13 6769  .....getattrZ.gi
+00001e20: 735f 7365 7269 616c 697a 6572 5f70 6174  s_serializer_pat
+00001e30: 6872 4700 0000 da04 6a73 6f6e 7218 0000  hrG.....jsonr...
+00001e40: 0072 2500 0000 724c 0000 0072 5700 0000  .r%...rL...rW...
+00001e50: 725b 0000 0072 6100 0000 7265 0000 0072  r[...ra...re...r
+00001e60: 6900 0000 726b 0000 0072 1e00 0000 721e  i...rk...r....r.
+00001e70: 0000 0072 1e00 0000 721f 0000 00da 083c  ...r....r......<
+00001e80: 6d6f 6475 6c65 3e01 0000 0073 2c00 0000  module>....s,...
+00001e90: 0c01 0c02 0c01 0c01 0c01 0c02 1001 1802  ................
+00001ea0: 1c03 0c01 0c02 0c01 0802 0802 1006 0e38  ...............8
+00001eb0: 1220 121e 1225 121f 1215 121b            . ...%......
```

### Comparing `anycluster-2.2.0/anycluster/api/json_schemas.py` & `anycluster-2.3.0/anycluster/api/json_schemas.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/api/serializers.py` & `anycluster-2.3.0/anycluster/api/serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from rest_framework import serializers
 
 import jsonschema
 
 from .json_schemas import FEATURE_OR_FEATURECOLLECTION_SCHEMA
 
 from anycluster.definitions import GEOMETRY_TYPES, GEOMETRY_TYPE_VIEWPORT
+from anycluster.MapClusterer import Gis
 
 
 def filters_are_allowed(filters):
 
     for filter in filters:
 
         is_nested = 'filters' in filter
@@ -57,14 +58,21 @@
         return value
 
     def validate_filters(self, value):
         filters_are_allowed(value)
         return value
 
 
+
+class AreaContentRequestSerializer(ClusterRequestSerializer):
+
+    limit = serializers.IntegerField(required=False, write_only=True)
+    offset = serializers.IntegerField(required=False, write_only=True)
+
+
 class MapContentCountSerializer(ClusterRequestSerializer):
     # additional filters, which are applied on top of filters, only for the count query
     modulations = serializers.JSONField(required=False, default={}, write_only=True)
 
     def validate_modulations(self, value):
 
         if value:
@@ -89,8 +97,16 @@
     ids = serializers.ListField(child=serializers.IntegerField(), write_only=True)
     x = serializers.FloatField(write_only=True)
     y = serializers.FloatField(write_only=True)
     filters = serializers.ListField(required=False, default=[], write_only=True)
 
     def validate_filters(self, value):
         filters_are_allowed(value)
-        return value
+        return value
+
+
+
+class GisModelSerializer(serializers.ModelSerializer):
+
+    class Meta:
+        model = Gis
+        fields = '__all__'
```

### Comparing `anycluster-2.2.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.3.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc` & `anycluster-2.3.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc` & `anycluster-2.3.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri May 26 08:53:58 2023 UTC, .py size: 13727 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 550d 0d0a 0000 0000 a673 7064 9f35 0000  U........spd.5..
+00000000: 550d 0d0a 0000 0000 093e 8064 ab39 0000  U........>.d.9..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 5a01 0000 6400  .....@...sZ...d.
+00000020: 0006 0000 0040 0000 0073 6e01 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
 00000080: 6d0f 5a0f 6d10 5a10 6d11 5a11 0100 6400  m.Z.m.Z.m.Z...d.
 00000090: 6407 6c12 6d13 5a13 6d14 5a14 6d15 5a15  d.l.m.Z.m.Z.m.Z.
@@ -16,566 +16,613 @@
 000000f0: 5a25 640c 5a26 640d 5a27 4700 640e 640f  Z%d.Z&d.Z'G.d.d.
 00000100: 8400 640f 6514 6504 8304 5a28 4700 6410  ..d.e.e...Z(G.d.
 00000110: 6411 8400 6411 6513 6514 6504 8305 5a29  d...d.e.e.e...Z)
 00000120: 4700 6412 6413 8400 6413 6513 6514 6504  G.d.d...d.e.e.e.
 00000130: 8305 5a2a 4700 6414 6415 8400 6415 6513  ..Z*G.d.d...d.e.
 00000140: 6514 6504 8305 5a2b 4700 6416 6417 8400  e.e...Z+G.d.d...
 00000150: 6417 6513 6514 6504 8305 5a2c 4700 6418  d.e.e.e...Z,G.d.
-00000160: 6419 8400 6419 6515 6514 6504 8305 5a2d  d...d.e.e.e...Z-
+00000160: 6419 8400 6419 6513 6514 6504 8305 5a2d  d...d.e.e.e...Z-
 00000170: 4700 641a 641b 8400 641b 6515 6514 6504  G.d.d...d.e.e.e.
-00000180: 8305 5a2e 640b 5300 291c e900 0000 0029  ..Z.d.S.)......)
-00000190: 01da 0772 6576 6572 7365 2902 da11 4150  ...reverse)...AP
-000001a0: 4952 6571 7565 7374 4661 6374 6f72 79da  IRequestFactory.
-000001b0: 0b41 5049 5465 7374 4361 7365 2901 da06  .APITestCase)...
-000001c0: 7374 6174 7573 2901 da0c 436c 7573 7465  status)...Cluste
-000001d0: 7243 6163 6865 2901 da0c 4d61 7043 6c75  rCache)...MapClu
-000001e0: 7374 6572 6572 2906 da0d 434c 5553 5445  sterer)...CLUSTE
-000001f0: 525f 5459 5045 53da 1647 454f 4d45 5452  R_TYPES..GEOMETR
-00000200: 595f 5459 5045 5f56 4945 5750 4f52 54da  Y_TYPE_VIEWPORT.
-00000210: 1247 454f 4d45 5452 595f 5459 5045 5f41  .GEOMETRY_TYPE_A
-00000220: 5245 41da 0e47 454f 4d45 5452 595f 5459  REA..GEOMETRY_TY
-00000230: 5045 53da 1343 4c55 5354 4552 5f54 5950  PES..CLUSTER_TYP
-00000240: 455f 4b4d 4541 4e53 da11 434c 5553 5445  E_KMEANS..CLUSTE
-00000250: 525f 5459 5045 5f47 5249 4429 03da 0757  R_TYPE_GRID)...W
-00000260: 6974 6847 4953 da0b 5769 7468 4669 6c74  ithGIS..WithFilt
-00000270: 6572 73da 0b57 6974 6847 6172 6465 6e73  ers..WithGardens
-00000280: 2904 da11 4745 4f4a 534f 4e5f 5245 4354  )...GEOJSON_RECT
-00000290: 414e 474c 45da 0f47 454f 4a53 4f4e 5f50  ANGLE..GEOJSON_P
-000002a0: 4f4c 5947 4f4e da14 4745 4f4a 534f 4e5f  OLYGON..GEOJSON_
-000002b0: 4d55 4c54 4950 4f4c 5947 4f4e da19 4745  MULTIPOLYGON..GE
-000002c0: 4f4a 534f 4e5f 4645 4154 5552 4543 4f4c  OJSON_FEATURECOL
-000002d0: 4c45 4354 494f 4e29 06da 124d 6170 436c  LECTION)...MapCl
-000002e0: 7573 7465 7256 6965 7742 6173 65da 0d4b  usterViewBase..K
-000002f0: 6d65 616e 7343 6c75 7374 6572 da0b 4772  meansCluster..Gr
-00000300: 6964 436c 7573 7465 72da 1147 6574 436c  idCluster..GetCl
-00000310: 7573 7465 7243 6f6e 7465 6e74 da0e 4765  usterContent..Ge
-00000320: 7441 7265 6143 6f6e 7465 6e74 da12 4765  tAreaContent..Ge
-00000330: 744d 6170 436f 6e74 656e 7443 6f75 6e74  tMapContentCount
-00000340: 2901 da07 4761 7264 656e 734e e900 0100  )...GardensN....
-00000350: 00e9 0a00 0000 6300 0000 0000 0000 0000  ......c.........
-00000360: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
-00000370: 3400 0000 6500 5a01 6400 5a02 6401 6402  4...e.Z.d.Z.d.d.
-00000380: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
-00000390: 8400 5a05 6407 6408 8400 5a06 6409 640a  ..Z.d.d...Z.d.d.
-000003a0: 8400 5a07 640b 5300 290c da16 5465 7374  ..Z.d.S.)...Test
-000003b0: 4d61 7043 6c75 7374 6572 5669 6577 4261  MapClusterViewBa
-000003c0: 7365 6301 0000 0000 0000 0000 0000 0002  sec.............
-000003d0: 0000 0003 0000 0043 0000 0073 0e00 0000  .......C...s....
-000003e0: 7400 7401 6401 9c02 7d01 7c01 5300 a902  t.t.d...}.|.S...
-000003f0: 4ea9 02da 047a 6f6f 6d5a 0967 7269 645f  N....zoomZ.grid_
-00000400: 7369 7a65 a902 da04 5a4f 4f4d da09 4752  size....ZOOM..GR
-00000410: 4944 5f53 495a 45a9 02da 0473 656c 66da  ID_SIZE....self.
-00000420: 0a75 726c 5f6b 7761 7267 73a9 0072 2800  .url_kwargs..r(.
-00000430: 0000 fa43 2f68 6f6d 652f 746f 6d2f 616e  ...C/home/tom/an
-00000440: 7963 6c75 7374 6572 2f64 656d 6f2f 646a  ycluster/demo/dj
-00000450: 616e 676f 2f61 6e79 636c 7573 7465 722f  ango/anycluster/
-00000460: 6170 692f 7465 7374 732f 7465 7374 5f76  api/tests/test_v
-00000470: 6965 7773 2e70 79da 0e67 6574 5f75 726c  iews.py..get_url
-00000480: 5f6b 7761 7267 731c 0000 0073 0800 0000  _kwargs....s....
-00000490: 0003 0201 02fe 0605 7a25 5465 7374 4d61  ........z%TestMa
-000004a0: 7043 6c75 7374 6572 5669 6577 4261 7365  pClusterViewBase
-000004b0: 2e67 6574 5f75 726c 5f6b 7761 7267 7363  .get_url_kwargsc
-000004c0: 0100 0000 0000 0000 0000 0000 0500 0000  ................
-000004d0: 0400 0000 4300 0000 7330 0000 0074 0083  ....C...s0...t..
-000004e0: 007d 017c 00a0 01a1 007d 0274 0264 017c  .}.|.....}.t.d.|
-000004f0: 0264 028d 027d 037c 01a0 037c 0369 00a1  .d...}.|...|.i..
-00000500: 027d 0469 007c 045f 047c 0453 00a9 034e  .}.i.|._.|.S...N
-00000510: da0e 6b6d 6561 6e73 5f63 6c75 7374 6572  ..kmeans_cluster
-00000520: a901 da06 6b77 6172 6773 2905 7203 0000  ....kwargs).r...
-00000530: 0072 2a00 0000 7202 0000 00da 0470 6f73  .r*...r......pos
-00000540: 74da 0773 6573 7369 6f6e 2905 7226 0000  t..session).r&..
-00000550: 00da 0766 6163 746f 7279 7227 0000 00da  ...factoryr'....
-00000560: 0375 726c da07 7265 7175 6573 7472 2800  .url..requestr(.
-00000570: 0000 7228 0000 0072 2900 0000 da0b 6765  ..r(...r).....ge
-00000580: 745f 7265 7175 6573 7426 0000 0073 0c00  t_request&...s..
-00000590: 0000 0002 0602 0801 0c01 0c02 0602 7a22  ..............z"
-000005a0: 5465 7374 4d61 7043 6c75 7374 6572 5669  TestMapClusterVi
-000005b0: 6577 4261 7365 2e67 6574 5f72 6571 7565  ewBase.get_reque
-000005c0: 7374 6301 0000 0000 0000 0000 0000 000b  stc.............
-000005d0: 0000 000a 0000 0043 0000 0073 7000 0000  .......C...sp...
-000005e0: 7c00 a000 a100 7d01 7401 8300 7d02 7c00  |.....}.t...}.|.
-000005f0: a002 a100 7d03 6401 7d04 6402 7d05 7c00  ....}.d.}.d.}.|.
-00000600: a003 a100 7d06 7404 4400 5d40 7d07 7405  ....}.t.D.]@}.t.
-00000610: 4400 5d36 7d08 7c06 4400 5d2c 7d09 7c02  D.]6}.|.D.],}.|.
-00000620: 6a06 7c07 7c08 7c09 7c04 7c05 7c01 6606  j.|.|.|.|.|.|.f.
-00000630: 7c03 8e01 7d0a 7c00 a007 7408 7c0a 7409  |...}.|...t.|.t.
-00000640: 8302 a101 0100 713a 7132 712a 6400 5300  ......q:q2q*d.S.
-00000650: 2903 4e46 69e6 1000 0029 0a72 3400 0000  ).NFi....).r4...
-00000660: 7215 0000 0072 2a00 0000 da10 6765 745f  r....r*.....get_
-00000670: 7465 7374 5f66 696c 7465 7273 720b 0000  test_filtersr...
-00000680: 0072 0800 0000 5a11 6765 745f 6d61 705f  .r....Z.get_map_
-00000690: 636c 7573 7465 7265 72da 0a61 7373 6572  clusterer..asser
-000006a0: 7454 7275 65da 0a69 7369 6e73 7461 6e63  tTrue..isinstanc
-000006b0: 6572 0700 0000 290b 7226 0000 0072 3300  er....).r&...r3.
-000006c0: 0000 da04 6261 7365 722e 0000 00da 0b63  ....baser......c
-000006d0: 6c65 6172 5f63 6163 6865 5a0b 6f75 7470  lear_cacheZ.outp
-000006e0: 7574 5f73 7269 64da 0c66 696c 7465 725f  ut_srid..filter_
-000006f0: 6c69 7374 73da 0d67 656f 6d65 7472 795f  lists..geometry_
-00000700: 7479 7065 da0b 636c 7573 7465 7274 7970  type..clustertyp
-00000710: 65da 0766 696c 7465 7273 5a09 636c 7573  e..filtersZ.clus
-00000720: 7465 7265 7272 2800 0000 7228 0000 0072  tererr(...r(...r
-00000730: 2900 0000 da16 7465 7374 5f67 6574 5f6d  ).....test_get_m
-00000740: 6170 5f63 6c75 7374 6572 6572 3300 0000  ap_clusterer3...
-00000750: 731e 0000 0000 0208 0206 0108 0204 0204  s...............
-00000760: 0108 0208 0108 0208 010e 0102 ff02 0102  ................
-00000770: ff04 027a 2d54 6573 744d 6170 436c 7573  ...z-TestMapClus
-00000780: 7465 7256 6965 7742 6173 652e 7465 7374  terViewBase.test
-00000790: 5f67 6574 5f6d 6170 5f63 6c75 7374 6572  _get_map_cluster
-000007a0: 6572 6301 0000 0000 0000 0000 0000 0008  erc.............
-000007b0: 0000 000a 0000 0043 0000 0073 5a00 0000  .......C...sZ...
-000007c0: 7c00 a000 a100 7d01 7401 8300 7d02 7c00  |.....}.t...}.|.
-000007d0: a002 a100 7d03 7403 4400 5d3a 7d04 7404  ....}.t.D.]:}.t.
-000007e0: 4400 5d30 7d05 7c03 4400 5d26 7d06 7c02  D.]0}.|.D.]&}.|.
-000007f0: a005 7c04 7406 7c05 7c01 7c06 a105 7d07  ..|.t.|.|.|...}.
-00000800: 7c00 a007 7408 7c07 7409 8302 a101 0100  |...t.|.t.......
-00000810: 712a 7122 711a 6400 5300 2901 4e29 0a72  q*q"q.d.S.).N).r
-00000820: 3400 0000 7215 0000 0072 3500 0000 720b  4...r....r5...r.
-00000830: 0000 0072 0800 0000 da09 6765 745f 6361  ...r......get_ca
-00000840: 6368 6572 2300 0000 7236 0000 0072 3700  cher#...r6...r7.
-00000850: 0000 7206 0000 0029 0872 2600 0000 7233  ..r....).r&...r3
-00000860: 0000 0072 3800 0000 723a 0000 0072 3b00  ...r8...r:...r;.
-00000870: 0000 723c 0000 0072 3d00 0000 da05 6361  ..r<...r=.....ca
-00000880: 6368 6572 2800 0000 7228 0000 0072 2900  cher(...r(...r).
-00000890: 0000 da0e 7465 7374 5f67 6574 5f63 6163  ....test_get_cac
-000008a0: 6865 4800 0000 7310 0000 0000 0208 0206  heH...s.........
-000008b0: 0208 0208 0108 0208 0112 027a 2554 6573  ...........z%Tes
-000008c0: 744d 6170 436c 7573 7465 7256 6965 7742  tMapClusterViewB
-000008d0: 6173 652e 7465 7374 5f67 6574 5f63 6163  ase.test_get_cac
-000008e0: 6865 6301 0000 0000 0000 0000 0000 0009  hec.............
-000008f0: 0000 000a 0000 0043 0000 0073 8e00 0000  .......C...s....
-00000900: 7c00 a000 a100 7d01 7401 8300 7d02 7c00  |.....}.t...}.|.
-00000910: a002 a100 7d03 7403 4400 5d6e 7d04 7404  ....}.t.D.]n}.t.
-00000920: 4400 5d64 7d05 7c03 4400 5d5a 7d06 7c02  D.]d}.|.D.]Z}.|.
-00000930: a005 7c04 7406 7c05 7c01 7c06 a105 7d07  ..|.t.|.|.|...}.
-00000940: 7c02 a007 7c01 7c07 a102 0100 7c00 a008  |...|.|.....|...
-00000950: 7c02 6a09 7c01 6a0a a102 0100 6401 4400  |.j.|.j.....d.D.
-00000960: 5d22 7d08 7c00 a00b 740c 7c07 7c08 8302  ]"}.|...t.|.|...
-00000970: 7c01 6a0a 7c02 6a09 1900 7c08 1900 a102  |.j.|.j...|.....
-00000980: 0100 7160 712a 7122 711a 6400 5300 2902  ..q`q*q"q.d.S.).
-00000990: 4e29 0472 3b00 0000 7221 0000 0072 3c00  N).r;...r!...r<.
-000009a0: 0000 723d 0000 0029 0d72 3400 0000 7215  ..r=...).r4...r.
-000009b0: 0000 0072 3500 0000 720b 0000 0072 0800  ...r5...r....r..
-000009c0: 0000 723f 0000 0072 2300 0000 5a09 7365  ..r?...r#...Z.se
-000009d0: 745f 6361 6368 65da 0861 7373 6572 7449  t_cache..assertI
-000009e0: 6eda 0a63 6163 6865 5f6e 616d 6572 3000  n..cache_namer0.
-000009f0: 0000 da0b 6173 7365 7274 4571 7561 6cda  ....assertEqual.
-00000a00: 0767 6574 6174 7472 2909 7226 0000 0072  .getattr).r&...r
-00000a10: 3300 0000 7238 0000 0072 3a00 0000 723b  3...r8...r:...r;
-00000a20: 0000 0072 3c00 0000 723d 0000 00da 0d63  ...r<...r=.....c
-00000a30: 6c75 7374 6572 5f63 6163 6865 da04 6174  luster_cache..at
-00000a40: 7472 7228 0000 0072 2800 0000 7229 0000  trr(...r(...r)..
-00000a50: 00da 0e74 6573 745f 7365 745f 6361 6368  ...test_set_cach
-00000a60: 6559 0000 0073 1600 0000 0002 0802 0602  eY...s..........
-00000a70: 0802 0801 0802 0802 1202 0c02 1002 0802  ................
-00000a80: 7a25 5465 7374 4d61 7043 6c75 7374 6572  z%TestMapCluster
-00000a90: 5669 6577 4261 7365 2e74 6573 745f 7365  ViewBase.test_se
-00000aa0: 745f 6361 6368 654e 2908 da08 5f5f 6e61  t_cacheN)...__na
-00000ab0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000ac0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 722a  ..__qualname__r*
-00000ad0: 0000 0072 3400 0000 723e 0000 0072 4100  ...r4...r>...rA.
-00000ae0: 0000 7248 0000 0072 2800 0000 7228 0000  ..rH...r(...r(..
-00000af0: 0072 2800 0000 7229 0000 0072 1e00 0000  .r(...r)...r....
-00000b00: 1900 0000 730a 0000 0008 0308 0a08 0d08  ....s...........
-00000b10: 1508 1172 1e00 0000 6300 0000 0000 0000  ...r....c.......
-00000b20: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000b30: 0073 2800 0000 6500 5a01 6400 5a02 6401  .s(...e.Z.d.Z.d.
-00000b40: 6402 8400 5a03 6700 6601 6403 6404 8401  d...Z.g.f.d.d...
-00000b50: 5a04 6405 6406 8400 5a05 6407 5300 2908  Z.d.d...Z.d.S.).
-00000b60: da0f 5465 7374 4772 6964 436c 7573 7465  ..TestGridCluste
-00000b70: 7263 0100 0000 0000 0000 0000 0000 0200  rc..............
-00000b80: 0000 0300 0000 4300 0000 730e 0000 0074  ......C...s....t
-00000b90: 0074 0164 019c 027d 017c 0153 0072 1f00  .t.d...}.|.S.r..
-00000ba0: 0000 7222 0000 0072 2500 0000 7228 0000  ..r"...r%...r(..
-00000bb0: 0072 2800 0000 7229 0000 0072 2a00 0000  .r(...r)...r*...
-00000bc0: 7400 0000 7308 0000 0000 0302 0102 fe06  t...s...........
-00000bd0: 057a 1e54 6573 7447 7269 6443 6c75 7374  .z.TestGridClust
-00000be0: 6572 2e67 6574 5f75 726c 5f6b 7761 7267  er.get_url_kwarg
-00000bf0: 7363 0200 0000 0000 0000 0000 0000 0300  sc..............
-00000c00: 0000 0400 0000 4300 0000 7310 0000 0074  ......C...s....t
-00000c10: 007c 0174 0164 019c 037d 027c 0253 00a9  .|.t.d...}.|.S..
-00000c20: 024e a903 da07 6765 6f6a 736f 6e72 3d00  .N....geojsonr=.
-00000c30: 0000 723b 0000 0029 0272 1100 0000 7209  ..r;...).r....r.
-00000c40: 0000 0029 0372 2600 0000 723d 0000 00da  ...).r&...r=....
-00000c50: 0970 6f73 745f 6461 7461 7228 0000 0072  .post_datar(...r
-00000c60: 2800 0000 7229 0000 00da 0d67 6574 5f70  (...r).....get_p
-00000c70: 6f73 745f 6461 7461 7d00 0000 730a 0000  ost_data}...s...
-00000c80: 0000 0302 0102 0102 fd06 067a 1d54 6573  ...........z.Tes
-00000c90: 7447 7269 6443 6c75 7374 6572 2e67 6574  tGridCluster.get
-00000ca0: 5f70 6f73 745f 6461 7461 6301 0000 0000  _post_datac.....
-00000cb0: 0000 0000 0000 0007 0000 0006 0000 0043  ...............C
-00000cc0: 0000 0073 5600 0000 7c00 a000 a100 7d01  ...sV...|.....}.
-00000cd0: 7c00 a001 a100 7d02 7402 6401 7c02 6402  |.....}.t.d.|.d.
-00000ce0: 8d02 7d03 7c01 4400 5d30 7d04 7c00 a003  ..}.|.D.]0}.|...
-00000cf0: 7c04 a101 7d05 7c00 6a04 6a05 7c03 7c05  |...}.|.j.j.|.|.
-00000d00: 6403 6404 8d03 7d06 7c00 a006 7c06 6a07  d.d...}.|...|.j.
-00000d10: 7408 6a09 a102 0100 7120 6400 5300 2905  t.j.....q d.S.).
-00000d20: 4e5a 0c67 7269 645f 636c 7573 7465 7272  NZ.grid_clusterr
-00000d30: 2d00 0000 da04 6a73 6f6e a901 da06 666f  -.....json....fo
-00000d40: 726d 6174 290a 7235 0000 0072 2a00 0000  rmat).r5...r*...
-00000d50: 7202 0000 0072 5100 0000 da06 636c 6965  r....rQ.....clie
-00000d60: 6e74 722f 0000 0072 4400 0000 da0b 7374  ntr/...rD.....st
-00000d70: 6174 7573 5f63 6f64 6572 0500 0000 da0b  atus_coder......
-00000d80: 4854 5450 5f32 3030 5f4f 4b29 0772 2600  HTTP_200_OK).r&.
-00000d90: 0000 723a 0000 0072 2700 0000 7232 0000  ..r:...r'...r2..
-00000da0: 0072 3d00 0000 7250 0000 00da 0872 6573  .r=...rP.....res
-00000db0: 706f 6e73 6572 2800 0000 7228 0000 0072  ponser(...r(...r
-00000dc0: 2900 0000 da09 7465 7374 5f70 6f73 7488  ).....test_post.
-00000dd0: 0000 0073 0e00 0000 0002 0802 0801 0c02  ...s............
-00000de0: 0802 0a02 1202 7a19 5465 7374 4772 6964  ......z.TestGrid
-00000df0: 436c 7573 7465 722e 7465 7374 5f70 6f73  Cluster.test_pos
-00000e00: 744e 2906 7249 0000 0072 4a00 0000 724b  tN).rI...rJ...rK
-00000e10: 0000 0072 2a00 0000 7251 0000 0072 5900  ...r*...rQ...rY.
-00000e20: 0000 7228 0000 0072 2800 0000 7228 0000  ..r(...r(...r(..
-00000e30: 0072 2900 0000 724c 0000 0072 0000 0073  .r)...rL...r...s
-00000e40: 0600 0000 0802 0809 0c0b 724c 0000 0063  ..........rL...c
-00000e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000e60: 0300 0000 4000 0000 7330 0000 0065 005a  ....@...s0...e.Z
-00000e70: 0164 005a 0264 0164 0284 005a 0364 0364  .d.Z.d.d...Z.d.d
-00000e80: 0484 005a 0467 0066 0164 0564 0684 015a  ...Z.g.f.d.d...Z
-00000e90: 0564 0764 0884 005a 0664 0953 0029 0ada  .d.d...Z.d.S.)..
-00000ea0: 1154 6573 744b 6d65 616e 7343 6c75 7374  .TestKmeansClust
-00000eb0: 6572 6301 0000 0000 0000 0000 0000 0002  erc.............
-00000ec0: 0000 0003 0000 0043 0000 0073 0e00 0000  .......C...s....
-00000ed0: 7400 7401 6401 9c02 7d01 7c01 5300 721f  t.t.d...}.|.S.r.
-00000ee0: 0000 0072 2200 0000 7225 0000 0072 2800  ...r"...r%...r(.
-00000ef0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
-00000f00: 009b 0000 0073 0800 0000 0003 0201 02fe  .....s..........
-00000f10: 0605 7a20 5465 7374 4b6d 6561 6e73 436c  ..z TestKmeansCl
-00000f20: 7573 7465 722e 6765 745f 7572 6c5f 6b77  uster.get_url_kw
-00000f30: 6172 6773 6301 0000 0000 0000 0000 0000  argsc...........
-00000f40: 0003 0000 0004 0000 0043 0000 0073 1800  .........C...s..
-00000f50: 0000 7c00 a000 a100 7d01 7401 6401 7c01  ..|.....}.t.d.|.
-00000f60: 6402 8d02 7d02 7c02 5300 722b 0000 0029  d...}.|.S.r+...)
-00000f70: 0272 2a00 0000 7202 0000 0029 0372 2600  .r*...r....).r&.
-00000f80: 0000 7227 0000 0072 3200 0000 7228 0000  ..r'...r2...r(..
-00000f90: 0072 2800 0000 7229 0000 00da 0767 6574  .r(...r).....get
-00000fa0: 5f75 726c a500 0000 7306 0000 0000 0208  _url....s.......
-00000fb0: 010c 017a 1954 6573 744b 6d65 616e 7343  ...z.TestKmeansC
-00000fc0: 6c75 7374 6572 2e67 6574 5f75 726c 6304  luster.get_urlc.
-00000fd0: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00000fe0: 0000 0043 0000 0073 1000 0000 7c02 7c03  ...C...s....|.|.
-00000ff0: 7c01 6401 9c03 7d04 7c04 5300 724d 0000  |.d...}.|.S.rM..
-00001000: 0072 2800 0000 2905 7226 0000 0072 3b00  .r(...).r&...r;.
-00001010: 0000 724f 0000 0072 3d00 0000 7250 0000  ..rO...r=...rP..
-00001020: 0072 2800 0000 7228 0000 0072 2900 0000  .r(...r(...r)...
-00001030: 7251 0000 00ac 0000 0073 0a00 0000 0003  rQ.......s......
-00001040: 0201 0201 02fd 0606 7a1f 5465 7374 4b6d  ........z.TestKm
-00001050: 6561 6e73 436c 7573 7465 722e 6765 745f  eansCluster.get_
-00001060: 706f 7374 5f64 6174 6163 0100 0000 0000  post_datac......
-00001070: 0000 0000 0000 0700 0000 0700 0000 4300  ..............C.
-00001080: 0000 73c2 0000 007c 00a0 00a1 007d 017c  ..s....|.....}.|
-00001090: 00a0 0174 0274 03a1 027d 027c 006a 046a  ...t.t...}.|.j.j
-000010a0: 057c 017c 0264 0164 028d 037d 037c 036a  .|.|.d.d...}.|.j
-000010b0: 0674 076a 086b 0372 3c74 097c 036a 0a83  .t.j.k.r<t.|.j..
-000010c0: 0101 007c 00a0 0b7c 036a 0674 076a 08a1  ...|...|.j.t.j..
-000010d0: 0201 007c 00a0 0ca1 007d 0474 0374 0d74  ...|.....}.t.t.t
-000010e0: 0e74 0f66 0444 005d 5c7d 057c 0444 005d  .t.f.D.]\}.|.D.]
-000010f0: 527d 067c 00a0 0174 107c 057c 06a1 037d  R}.|...t.|.|...}
-00001100: 027c 006a 046a 057c 017c 0264 0164 028d  .|.j.j.|.|.d.d..
-00001110: 037d 037c 036a 0674 076a 086b 0372 aa74  .}.|.j.t.j.k.r.t
-00001120: 097c 0583 0101 0074 097c 036a 0a83 0101  .|.....t.|.j....
-00001130: 007c 00a0 0b7c 036a 0674 076a 08a1 0201  .|...|.j.t.j....
-00001140: 0071 6871 6064 0053 0029 034e 7252 0000  .qhq`d.S.).NrR..
-00001150: 0072 5300 0000 2911 725b 0000 0072 5100  .rS...).r[...rQ.
-00001160: 0000 7209 0000 0072 1100 0000 7255 0000  ..r....r....rU..
-00001170: 0072 2f00 0000 7256 0000 0072 0500 0000  .r/...rV...r....
-00001180: 7257 0000 00da 0570 7269 6e74 da04 6461  rW.....print..da
-00001190: 7461 7244 0000 0072 3500 0000 7212 0000  tarD...r5...r...
-000011a0: 0072 1300 0000 7214 0000 0072 0a00 0000  .r....r....r....
-000011b0: 2907 7226 0000 0072 3200 0000 7250 0000  ).r&...r2...rP..
-000011c0: 0072 5800 0000 723a 0000 0072 4f00 0000  .rX...r:...rO...
-000011d0: 723d 0000 0072 2800 0000 7228 0000 0072  r=...r(...r(...r
-000011e0: 2900 0000 7259 0000 00b7 0000 0073 1e00  )...rY.......s..
-000011f0: 0000 0002 0803 0c02 1202 0c01 0a01 1002  ................
-00001200: 0801 1002 0802 0e02 1202 0c01 0801 0a01  ................
-00001210: 7a1b 5465 7374 4b6d 6561 6e73 436c 7573  z.TestKmeansClus
-00001220: 7465 722e 7465 7374 5f70 6f73 744e 2907  ter.test_postN).
-00001230: 7249 0000 0072 4a00 0000 724b 0000 0072  rI...rJ...rK...r
-00001240: 2a00 0000 725b 0000 0072 5100 0000 7259  *...r[...rQ...rY
-00001250: 0000 0072 2800 0000 7228 0000 0072 2800  ...r(...r(...r(.
-00001260: 0000 7229 0000 0072 5a00 0000 9900 0000  ..r)...rZ.......
-00001270: 7308 0000 0008 0208 0a08 070c 0b72 5a00  s............rZ.
-00001280: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001290: 0000 0002 0000 0040 0000 0073 1400 0000  .......@...s....
-000012a0: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
-000012b0: 6403 5300 2904 da1b 5465 7374 4765 744b  d.S.)...TestGetK
-000012c0: 6d65 616e 7343 6c75 7374 6572 436f 6e74  meansClusterCont
-000012d0: 656e 7463 0100 0000 0000 0000 0000 0000  entc............
-000012e0: 1800 0000 0b00 0000 4300 0000 73ee 0100  ........C...s...
-000012f0: 007c 00a0 00a1 007d 0174 0144 0090 015d  .|.....}.t.D...]
-00001300: da7d 027c 0144 0090 015d ce7d 0374 0274  .}.|.D...].}.t.t
-00001310: 0364 019c 027d 0474 0464 027c 0464 038d  .d...}.t.d.|.d..
-00001320: 027d 0574 057c 037c 0264 049c 037d 0674  .}.t.|.|.d...}.t
-00001330: 0683 007d 077c 076a 077c 057c 0664 0564  ...}.|.j.|.|.d.d
-00001340: 068d 037d 0869 007c 085f 0874 09a0 0aa1  ...}.i.|._.t....
-00001350: 007d 097c 097c 0866 017c 048e 017d 0a7c  .}.|.|.f.|...}.|
-00001360: 0274 0b6b 0272 907c 00a0 0c74 0d7c 086a  .t.k.r.|...t.|.j
-00001370: 0864 0719 0064 0819 0083 0164 09a1 0201  .d...d.....d....
-00001380: 007c 0a6a 0e64 0a19 007d 0b74 0f7c 0274  .|.j.d...}.t.|.t
-00001390: 0274 107c 0383 047d 0c7c 0ca0 117c 086a  .t.|...}.|...|.j
-000013a0: 0864 0719 00a1 0101 007c 00a0 0c7c 0c6a  .d.......|...|.j
-000013b0: 127c 086a 0864 0719 0064 0819 00a1 0201  .|.j.d...d......
-000013c0: 007c 0274 0b6b 0290 0172 067c 00a0 0c74  .|.t.k...r.|...t
-000013d0: 0d7c 0c6a 1283 0164 09a1 0201 007c 0c6a  .|.j...d.....|.j
-000013e0: 1264 0a19 007d 0d7c 00a0 0c74 137c 0d83  .d...}.|...t.|..
-000013f0: 0174 14a1 0201 0074 157c 0c83 017d 0e7c  .t.....t.|...}.|
-00001400: 0b64 0b19 007d 0f7c 0b64 0c19 0064 0d19  .d...}.|.d...d..
-00001410: 007d 107c 0b64 0c19 0064 0e19 007d 117c  .}.|.d...d...}.|
-00001420: 00a0 0c7c 0e6a 166a 127c 086a 0864 0719  ...|.j.j.|.j.d..
-00001430: 0064 0819 00a1 0201 0074 177c 0ea0 187c  .d.......t.|...|
-00001440: 027c 0f7c 107c 117c 0374 02a1 0683 017d  .|.|.|.|.t.....}
-00001450: 127c 00a0 1974 0d74 177c 1283 0183 0164  .|...t.t.|.....d
-00001460: 0a6b 04a1 0101 007c 00a0 0c74 0d74 177c  .k.....|...t.t.|
-00001470: 1283 0183 017c 0b64 0f19 00a1 0201 0074  .....|.d.......t
-00001480: 0464 107c 0464 038d 027d 137c 027c 0f7c  .d.|.d...}.|.|.|
-00001490: 107c 117c 0364 119c 057d 147c 076a 077c  .|.|.d...}.|.j.|
-000014a0: 137c 1464 0564 068d 037d 157c 086a 087c  .|.d.d...}.|.j.|
-000014b0: 155f 0874 1aa0 0aa1 007d 167c 167c 1566  ._.t.....}.|.|.f
-000014c0: 017c 048e 017d 177c 00a0 0c7c 176a 1b74  .|...}.|...|.j.t
-000014d0: 1c6a 1da1 0201 0071 1671 0c64 0053 0029  .j.....q.q.d.S.)
-000014e0: 124e 7220 0000 0072 2c00 0000 722d 0000  .Nr ...r,...r-..
-000014f0: 0072 4e00 0000 7252 0000 0072 5300 0000  .rN...rR...rS...
-00001500: 5a10 616e 7963 6c75 7374 6572 5f63 6163  Z.anycluster_cac
-00001510: 6865 da0a 6765 6f6d 6574 7269 6573 e901  he..geometries..
-00001520: 0000 0072 0100 0000 da03 6964 73da 0663  ...r......ids..c
-00001530: 656e 7465 72da 0178 da01 79da 0563 6f75  enter..x..y..cou
-00001540: 6e74 da1a 6765 745f 6b6d 6561 6e73 5f63  nt..get_kmeans_c
-00001550: 6c75 7374 6572 5f63 6f6e 7465 6e74 2905  luster_content).
-00001560: 723b 0000 0072 6100 0000 7263 0000 0072  r;...ra...rc...r
-00001570: 6400 0000 723d 0000 0029 1e72 3500 0000  d...r=...).r5...
-00001580: 720b 0000 0072 2300 0000 7224 0000 0072  r....r#...r$...r
-00001590: 0200 0000 7211 0000 0072 0300 0000 722f  ....r....r....r/
-000015a0: 0000 0072 3000 0000 7216 0000 00da 0761  ...r0...r......a
-000015b0: 735f 7669 6577 720a 0000 0072 4400 0000  s_viewr....rD...
-000015c0: da03 6c65 6e72 5d00 0000 7206 0000 0072  ..lenr]...r....r
-000015d0: 0c00 0000 da0f 6c6f 6164 5f67 656f 6d65  ......load_geome
-000015e0: 7472 6965 7372 5f00 0000 da04 7479 7065  triesr_.....type
-000015f0: da03 7374 7272 0700 0000 7246 0000 00da  ..strr....rF....
-00001600: 046c 6973 7472 6600 0000 7236 0000 0072  .listrf...r6...r
-00001610: 1800 0000 7256 0000 0072 0500 0000 7257  ....rV...r....rW
-00001620: 0000 0029 1872 2600 0000 723a 0000 0072  ...).r&...r:...r
-00001630: 3b00 0000 723d 0000 0072 2700 0000 5a0a  ;...r=...r'...Z.
-00001640: 6b6d 6561 6e73 5f75 726c 5a10 6b6d 6561  kmeans_urlZ.kmea
-00001650: 6e73 5f70 6f73 745f 6461 7461 7231 0000  ns_post_datar1..
-00001660: 005a 0e6b 6d65 616e 735f 7265 7175 6573  .Z.kmeans_reques
-00001670: 745a 0b6b 6d65 616e 735f 7669 6577 5a0f  tZ.kmeans_viewZ.
-00001680: 6b6d 6561 6e73 5f72 6573 706f 6e73 655a  kmeans_responseZ
-00001690: 0763 6c75 7374 6572 7246 0000 00da 0467  .clusterrF.....g
-000016a0: 656f 6d5a 0d6d 6170 5f63 6c75 7374 6572  eomZ.map_cluster
-000016b0: 6572 7261 0000 0072 6300 0000 7264 0000  erra...rc...rd..
-000016c0: 005a 0f63 6c75 7374 6572 5f63 6f6e 7465  .Z.cluster_conte
-000016d0: 6e74 7232 0000 0072 5000 0000 7233 0000  ntr2...rP...r3..
-000016e0: 00da 0476 6965 7772 5800 0000 7228 0000  ...viewrX...r(..
-000016f0: 0072 2800 0000 7229 0000 0072 5900 0000  .r(...r)...rY...
-00001700: d500 0000 735c 0000 0000 0208 020a 020a  ....s\..........
-00001710: 0302 0102 fe06 050c 0302 0102 0102 fd06  ................
-00001720: 0606 0110 0106 0208 020c 0208 011a 020a  ................
-00001730: 030e 0110 0218 020a 0112 020a 0210 0208  ................
-00001740: 0208 010c 010c 021a 0218 0216 0118 040c  ................
-00001750: 0302 0102 0102 0102 0102 fb06 0810 0108  ................
-00001760: 0208 010c 027a 2554 6573 7447 6574 4b6d  .....z%TestGetKm
-00001770: 6561 6e73 436c 7573 7465 7243 6f6e 7465  eansClusterConte
-00001780: 6e74 2e74 6573 745f 706f 7374 4ea9 0472  nt.test_postN..r
-00001790: 4900 0000 724a 0000 0072 4b00 0000 7259  I...rJ...rK...rY
-000017a0: 0000 0072 2800 0000 7228 0000 0072 2800  ...r(...r(...r(.
-000017b0: 0000 7229 0000 0072 5e00 0000 d300 0000  ..r)...r^.......
-000017c0: 7302 0000 0008 0272 5e00 0000 6300 0000  s......r^...c...
-000017d0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-000017e0: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
-000017f0: 5a02 6401 6402 8400 5a03 6403 5300 2904  Z.d.d...Z.d.S.).
-00001800: da12 5465 7374 4765 7441 7265 6143 6f6e  ..TestGetAreaCon
-00001810: 7465 6e74 6301 0000 0000 0000 0000 0000  tentc...........
-00001820: 0008 0000 0007 0000 0043 0000 0073 8a00  .........C...s..
-00001830: 0000 7400 7401 6401 9c02 7d01 7402 6402  ..t.t.d...}.t.d.
-00001840: 7c01 6403 8d02 7d02 7c00 a003 a100 7d03  |.d...}.|.....}.
-00001850: 7404 7405 7406 7407 6604 4400 5d5a 7d04  t.t.t.t.f.D.]Z}.
-00001860: 7c03 4400 5d50 7d05 7408 7c04 7c05 6404  |.D.]P}.t.|.|.d.
-00001870: 9c03 7d06 7c00 6a09 6a0a 7c02 7c06 6405  ..}.|.j.j.|.|.d.
-00001880: 6406 8d03 7d07 7c07 6a0b 740c 6a0d 6b03  d...}.|.j.t.j.k.
-00001890: 7272 740e 7c04 8301 0100 740e 7c07 6a0f  rrt.|.....t.|.j.
-000018a0: 8301 0100 7c00 a010 7c07 6a0b 740c 6a0d  ....|...|.j.t.j.
-000018b0: a102 0100 7132 712a 6400 5300 2907 4e72  ....q2q*d.S.).Nr
-000018c0: 2000 0000 5a10 6765 745f 6172 6561 5f63   ...Z.get_area_c
-000018d0: 6f6e 7465 6e74 722d 0000 00a9 0372 3b00  ontentr-.....r;.
-000018e0: 0000 724f 0000 0072 3d00 0000 7252 0000  ..rO...r=...rR..
-000018f0: 0072 5300 0000 2911 7223 0000 0072 2400  .rS...).r#...r$.
-00001900: 0000 7202 0000 0072 3500 0000 7211 0000  ..r....r5...r...
-00001910: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-00001920: 720a 0000 0072 5500 0000 722f 0000 0072  r....rU...r/...r
-00001930: 5600 0000 7205 0000 0072 5700 0000 725c  V...r....rW...r\
-00001940: 0000 0072 5d00 0000 7244 0000 00a9 0872  ...r]...rD.....r
-00001950: 2600 0000 7227 0000 0072 3200 0000 723a  &...r'...r2...r:
-00001960: 0000 0072 4f00 0000 723d 0000 0072 5000  ...rO...r=...rP.
-00001970: 0000 7258 0000 0072 2800 0000 7228 0000  ..rX...r(...r(..
-00001980: 0072 2900 0000 7259 0000 0028 0100 0073  .r)...rY...(...s
-00001990: 2000 0000 0003 0201 02fe 0605 0c02 0802   ...............
-000019a0: 1002 0803 0201 0201 02fd 0606 1202 0c01  ................
-000019b0: 0801 0a02 7a1c 5465 7374 4765 7441 7265  ....z.TestGetAre
-000019c0: 6143 6f6e 7465 6e74 2e74 6573 745f 706f  aContent.test_po
-000019d0: 7374 4e72 6f00 0000 7228 0000 0072 2800  stNro...r(...r(.
-000019e0: 0000 7228 0000 0072 2900 0000 7270 0000  ..r(...r)...rp..
-000019f0: 0026 0100 0073 0200 0000 0802 7270 0000  .&...s......rp..
-00001a00: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001a10: 0000 0200 0000 4000 0000 731c 0000 0065  ......@...s....e
-00001a20: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
-00001a30: 0364 0484 005a 0464 0553 0029 06da 1654  .d...Z.d.S.)...T
-00001a40: 6573 7447 6574 4d61 7043 6f6e 7465 6e74  estGetMapContent
-00001a50: 436f 756e 7463 0100 0000 0000 0000 0000  Countc..........
-00001a60: 0000 0800 0000 0700 0000 4300 0000 7392  ..........C...s.
-00001a70: 0000 007c 00a0 00a1 0001 0074 0174 0264  ...|.......t.t.d
-00001a80: 019c 027d 0174 0364 027c 0164 038d 027d  ...}.t.d.|.d...}
-00001a90: 027c 00a0 04a1 007d 0374 0574 0674 0774  .|.....}.t.t.t.t
-00001aa0: 0866 0444 005d 5a7d 047c 0344 005d 507d  .f.D.]Z}.|.D.]P}
-00001ab0: 0574 097c 047c 0564 049c 037d 067c 006a  .t.|.|.d...}.|.j
-00001ac0: 0a6a 0b7c 027c 0664 0564 068d 037d 077c  .j.|.|.d.d...}.|
-00001ad0: 076a 0c74 0d6a 0e6b 0372 7a74 0f7c 0483  .j.t.j.k.rzt.|..
-00001ae0: 0101 0074 0f7c 076a 1083 0101 007c 00a0  ...t.|.j.....|..
-00001af0: 117c 076a 0c74 0d6a 0ea1 0201 0071 3a71  .|.j.t.j.....q:q
-00001b00: 3264 0053 0029 074e 7220 0000 00da 1567  2d.S.).Nr .....g
-00001b10: 6574 5f6d 6170 5f63 6f6e 7465 6e74 5f63  et_map_content_c
-00001b20: 6f75 6e74 722d 0000 0072 7100 0000 7252  ountr-...rq...rR
-00001b30: 0000 0072 5300 0000 2912 da0d 6372 6561  ...rS...)...crea
-00001b40: 7465 5f70 6f69 6e74 7372 2300 0000 7224  te_pointsr#...r$
-00001b50: 0000 0072 0200 0000 7235 0000 0072 1100  ...r....r5...r..
-00001b60: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00001b70: 0072 0a00 0000 7255 0000 0072 2f00 0000  .r....rU...r/...
-00001b80: 7256 0000 0072 0500 0000 7257 0000 0072  rV...r....rW...r
-00001b90: 5c00 0000 725d 0000 0072 4400 0000 7272  \...r]...rD...rr
-00001ba0: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
-00001bb0: 0000 7259 0000 0049 0100 0073 2200 0000  ..rY...I...s"...
-00001bc0: 0002 0803 0201 02fe 0605 0c02 0802 1002  ................
-00001bd0: 0803 0201 0201 02fd 0606 1202 0c01 0801  ................
-00001be0: 0a04 7a20 5465 7374 4765 744d 6170 436f  ..z TestGetMapCo
-00001bf0: 6e74 656e 7443 6f75 6e74 2e74 6573 745f  ntentCount.test_
-00001c00: 706f 7374 6301 0000 0000 0000 0000 0000  postc...........
-00001c10: 000a 0000 0007 0000 0043 0000 0073 f200  .........C...s..
-00001c20: 0000 6401 6402 6403 6404 6405 9c03 6701  ..d.d.d.d.d...g.
-00001c30: 6901 6401 6402 6406 6404 6405 9c03 6701  i.d.d.d.d.d...g.
-00001c40: 6901 6407 9c02 7d01 7c00 a000 a100 0100  i.d...}.|.......
-00001c50: 7401 7402 6408 9c02 7d02 7403 6409 7c02  t.t.d...}.t.d.|.
-00001c60: 640a 8d02 7d03 7404 7405 7406 7407 6604  d...}.t.t.t.t.f.
-00001c70: 4400 5d9c 7d04 7c00 a008 a100 7d05 7c05  D.].}.|.....}.|.
-00001c80: 4400 5d8a 7d06 7409 7c04 7c06 7c01 640b  D.].}.t.|.|.|.d.
-00001c90: 9c04 7d07 7c00 6a0a 6a0b 7c03 7c07 640c  ..}.|.j.j.|.|.d.
-00001ca0: 640d 8d03 7d08 7c08 6a0c 740d 6a0e 6b03  d...}.|.j.t.j.k.
-00001cb0: 72a2 740f 7c04 8301 0100 740f 7c08 6a10  r.t.|.....t.|.j.
-00001cc0: 8301 0100 7411 a012 7c08 6a13 a101 7d09  ....t...|.j...}.
-00001cd0: 7c00 a014 640e 7c09 a102 0100 7c00 a014  |...d.|.....|...
-00001ce0: 6403 7c09 640e 1900 a102 0100 7c00 a014  d.|.d.......|...
-00001cf0: 6406 7c09 640e 1900 a102 0100 7c00 a015  d.|.d.......|...
-00001d00: 7c08 6a0c 740d 6a0e a102 0100 7160 7150  |.j.t.j.....q`qP
-00001d10: 6400 5300 290f 4e72 3d00 0000 da05 7374  d.S.).Nr=.....st
-00001d20: 796c 65da 0573 746f 6e65 fa01 3d29 03da  yle..stone..=)..
-00001d30: 0663 6f6c 756d 6eda 0576 616c 7565 da08  .column..value..
-00001d40: 6f70 6572 6174 6f72 da06 666c 6f77 6572  operator..flower
-00001d50: 2902 7277 0000 0072 7c00 0000 7220 0000  ).rw...r|...r ..
-00001d60: 0072 7400 0000 722d 0000 0029 0472 3b00  .rt...r-...).r;.
-00001d70: 0000 724f 0000 0072 3d00 0000 da0b 6d6f  ..rO...r=.....mo
-00001d80: 6475 6c61 7469 6f6e 7372 5200 0000 7253  dulationsrR...rS
-00001d90: 0000 0072 7d00 0000 2916 7275 0000 0072  ...r}...).ru...r
-00001da0: 2300 0000 7224 0000 0072 0200 0000 7211  #...r$...r....r.
-00001db0: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
-00001dc0: 0000 7235 0000 0072 0a00 0000 7255 0000  ..r5...r....rU..
-00001dd0: 0072 2f00 0000 7256 0000 0072 0500 0000  .r/...rV...r....
-00001de0: 7257 0000 0072 5c00 0000 725d 0000 0072  rW...r\...r]...r
-00001df0: 5200 0000 da05 6c6f 6164 73da 0763 6f6e  R.....loads..con
-00001e00: 7465 6e74 7242 0000 0072 4400 0000 290a  tentrB...rD...).
-00001e10: 7226 0000 0072 7d00 0000 7227 0000 0072  r&...r}...r'...r
-00001e20: 3200 0000 724f 0000 0072 3a00 0000 723d  2...rO...r:...r=
-00001e30: 0000 0072 5000 0000 7258 0000 00da 0f70  ...rP...rX.....p
-00001e40: 6172 7365 645f 7265 7370 6f6e 7365 7228  arsed_responser(
-00001e50: 0000 0072 2800 0000 7229 0000 00da 1374  ...r(...r).....t
-00001e60: 6573 745f 706f 7374 5f6d 6f64 756c 6174  est_post_modulat
-00001e70: 6564 6b01 0000 734a 0000 0000 0402 0202  edk...sJ........
-00001e80: 0102 0102 fd04 ff02 ff02 0a02 0202 0102  ................
-00001e90: 0102 fd04 ff02 ff02 f606 1508 0302 0102  ................
-00001ea0: fe06 050c 0210 0208 0208 0302 0102 0102  ................
-00001eb0: 0102 fc06 0712 020c 0108 010a 020c 020c  ................
-00001ec0: 0110 0110 027a 2a54 6573 7447 6574 4d61  .....z*TestGetMa
-00001ed0: 7043 6f6e 7465 6e74 436f 756e 742e 7465  pContentCount.te
-00001ee0: 7374 5f70 6f73 745f 6d6f 6475 6c61 7465  st_post_modulate
-00001ef0: 644e 2905 7249 0000 0072 4a00 0000 724b  dN).rI...rJ...rK
-00001f00: 0000 0072 5900 0000 7281 0000 0072 2800  ...rY...r....r(.
-00001f10: 0000 7228 0000 0072 2800 0000 7229 0000  ..r(...r(...r)..
-00001f20: 0072 7300 0000 4701 0000 7304 0000 0008  .rs...G...s.....
-00001f30: 0208 2272 7300 0000 6300 0000 0000 0000  .."rs...c.......
-00001f40: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-00001f50: 0073 1400 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00001f60: 6402 8400 5a03 6403 5300 2904 da19 5465  d...Z.d.S.)...Te
-00001f70: 7374 4765 7447 726f 7570 6564 4d61 7043  stGetGroupedMapC
-00001f80: 6f6e 7465 6e74 7363 0100 0000 0000 0000  ontentsc........
-00001f90: 0000 0000 0b00 0000 0600 0000 4300 0000  ............C...
-00001fa0: 73dc 0000 007c 00a0 00a1 0001 0074 0174  s....|.......t.t
-00001fb0: 0264 019c 027d 0174 0364 027c 0164 038d  .d...}.t.d.|.d..
-00001fc0: 027d 0267 007d 0374 046a 056a 0664 0464  .}.g.}.t.j.j.d.d
-00001fd0: 058d 017d 047c 00a0 077c 04a0 08a1 0064  ...}.|...|.....d
-00001fe0: 066b 04a1 0101 0074 0974 0a74 0b74 0c66  .k.....t.t.t.t.f
-00001ff0: 0444 005d 887d 0574 0d7c 057c 0364 0764  .D.].}.t.|.|.d.d
-00002000: 089c 047d 067c 006a 0e6a 0f7c 027c 0664  ...}.|.j.j.|.|.d
-00002010: 0964 0a8d 037d 077c 076a 1074 116a 126b  .d...}.|.j.t.j.k
-00002020: 0372 9074 137c 0583 0101 0074 137c 076a  .r.t.|.....t.|.j
-00002030: 1483 0101 0074 15a0 167c 076a 17a1 017d  .....t...|.j...}
-00002040: 0874 046a 05a0 18a1 006a 1964 0764 0b64  .t.j.....j.d.d.d
-00002050: 0c8d 027d 097c 0944 005d 107d 0a7c 00a0  ...}.|.D.].}.|..
-00002060: 1a7c 0a7c 08a1 0201 0071 b47c 00a0 1b7c  .|.|.....q.|...|
-00002070: 076a 1074 116a 12a1 0201 0071 4e64 0053  .j.t.j.....qNd.S
-00002080: 0029 0d4e 7220 0000 005a 1867 6574 5f67  .).Nr ...Z.get_g
-00002090: 726f 7570 6564 5f6d 6170 5f63 6f6e 7465  rouped_map_conte
-000020a0: 6e74 7372 2d00 0000 7277 0000 0029 0172  ntsr-...rw...).r
-000020b0: 7600 0000 7201 0000 0072 7600 0000 2904  v...r....rv...).
-000020c0: 723b 0000 0072 4f00 0000 723d 0000 00da  r;...rO...r=....
-000020d0: 0867 726f 7570 5f62 7972 5200 0000 7253  .group_byrR...rS
-000020e0: 0000 0054 2901 da04 666c 6174 291c 7275  ...T)...flat).ru
-000020f0: 0000 0072 2300 0000 7224 0000 0072 0200  ...r#...r$...r..
-00002100: 0000 721b 0000 00da 076f 626a 6563 7473  ..r......objects
-00002110: da06 6669 6c74 6572 7236 0000 0072 6500  ..filterr6...re.
-00002120: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00002130: 0072 1400 0000 720a 0000 0072 5500 0000  .r....r....rU...
-00002140: 722f 0000 0072 5600 0000 7205 0000 0072  r/...rV...r....r
-00002150: 5700 0000 725c 0000 0072 5d00 0000 7252  W...r\...r]...rR
-00002160: 0000 0072 7e00 0000 727f 0000 00da 0361  ...r~...r......a
-00002170: 6c6c da0b 7661 6c75 6573 5f6c 6973 7472  ll..values_listr
-00002180: 4200 0000 7244 0000 0029 0b72 2600 0000  B...rD...).r&...
-00002190: 7227 0000 0072 3200 0000 723d 0000 005a  r'...r2...r=...Z
-000021a0: 0d73 746f 6e65 5f67 6172 6465 6e73 724f  .stone_gardensrO
-000021b0: 0000 0072 5000 0000 7258 0000 0072 8000  ...rP...rX...r..
-000021c0: 0000 da06 7374 796c 6573 7276 0000 0072  ....stylesrv...r
-000021d0: 2800 0000 7228 0000 0072 2900 0000 7259  (...r(...r)...rY
-000021e0: 0000 00a9 0100 0073 2e00 0000 0002 0803  .......s........
-000021f0: 0201 02fe 0605 0c02 0402 0e01 1202 1003  ................
-00002200: 0201 0201 0201 02fc 0607 1202 0c01 0801  ................
-00002210: 0a02 0c01 1402 0801 0e02 7a23 5465 7374  ..........z#Test
-00002220: 4765 7447 726f 7570 6564 4d61 7043 6f6e  GetGroupedMapCon
-00002230: 7465 6e74 732e 7465 7374 5f70 6f73 744e  tents.test_postN
-00002240: 726f 0000 0072 2800 0000 7228 0000 0072  ro...r(...r(...r
-00002250: 2800 0000 7229 0000 0072 8200 0000 a701  (...r)...r......
-00002260: 0000 7302 0000 0008 0272 8200 0000 292f  ..s......r....)/
-00002270: da0b 646a 616e 676f 2e75 726c 7372 0200  ..django.urlsr..
-00002280: 0000 5a13 7265 7374 5f66 7261 6d65 776f  ..Z.rest_framewo
-00002290: 726b 2e74 6573 7472 0300 0000 7204 0000  rk.testr....r...
-000022a0: 00da 0e72 6573 745f 6672 616d 6577 6f72  ...rest_framewor
-000022b0: 6b72 0500 0000 da0a 616e 7963 6c75 7374  kr......anyclust
-000022c0: 6572 7206 0000 005a 1761 6e79 636c 7573  err....Z.anyclus
-000022d0: 7465 722e 4d61 7043 6c75 7374 6572 6572  ter.MapClusterer
-000022e0: 7207 0000 00da 1661 6e79 636c 7573 7465  r......anycluste
-000022f0: 722e 6465 6669 6e69 7469 6f6e 7372 0800  r.definitionsr..
-00002300: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00002310: 0072 0c00 0000 720d 0000 005a 1761 6e79  .r....r....Z.any
-00002320: 636c 7573 7465 722e 7465 7374 732e 6d69  cluster.tests.mi
-00002330: 7869 6e73 720e 0000 0072 0f00 0000 7210  xinsr....r....r.
-00002340: 0000 005a 1761 6e79 636c 7573 7465 722e  ...Z.anycluster.
-00002350: 7465 7374 732e 636f 6d6d 6f6e 7211 0000  tests.commonr...
-00002360: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-00002370: 5a14 616e 7963 6c75 7374 6572 2e61 7069  Z.anycluster.api
-00002380: 2e76 6965 7773 7215 0000 0072 1600 0000  .viewsr....r....
-00002390: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-000023a0: 1a00 0000 5a0d 616e 796d 6170 2e6d 6f64  ....Z.anymap.mod
-000023b0: 656c 7372 1b00 0000 7252 0000 005a 0c4d  elsr....rR...Z.M
-000023c0: 4150 5f54 494c 4553 495a 4572 2400 0000  AP_TILESIZEr$...
-000023d0: 7223 0000 0072 1e00 0000 724c 0000 0072  r#...r....rL...r
-000023e0: 5a00 0000 725e 0000 0072 7000 0000 7273  Z...r^...rp...rs
-000023f0: 0000 0072 8200 0000 7228 0000 0072 2800  ...r....r(...r(.
-00002400: 0000 7228 0000 0072 2900 0000 da08 3c6d  ..r(...r).....<m
-00002410: 6f64 756c 653e 0100 0000 7328 0000 000c  odule>....s(....
-00002420: 0110 010c 020c 010c 0120 0314 0118 0220  ......... ..... 
-00002430: 040c 0208 0204 0104 0104 0212 5914 2714  ............Y.'.
-00002440: 3a14 5314 2114 60                        :.S.!.`
+00000180: 8305 5a2e 4700 641c 641d 8400 641d 6515  ..Z.G.d.d...d.e.
+00000190: 6514 6504 8305 5a2f 640b 5300 291e e900  e.e...Z/d.S.)...
+000001a0: 0000 0029 01da 0772 6576 6572 7365 2902  ...)...reverse).
+000001b0: da11 4150 4952 6571 7565 7374 4661 6374  ..APIRequestFact
+000001c0: 6f72 79da 0b41 5049 5465 7374 4361 7365  ory..APITestCase
+000001d0: 2901 da06 7374 6174 7573 2901 da0c 436c  )...status)...Cl
+000001e0: 7573 7465 7243 6163 6865 2901 da0c 4d61  usterCache)...Ma
+000001f0: 7043 6c75 7374 6572 6572 2906 da0d 434c  pClusterer)...CL
+00000200: 5553 5445 525f 5459 5045 53da 1647 454f  USTER_TYPES..GEO
+00000210: 4d45 5452 595f 5459 5045 5f56 4945 5750  METRY_TYPE_VIEWP
+00000220: 4f52 54da 1247 454f 4d45 5452 595f 5459  ORT..GEOMETRY_TY
+00000230: 5045 5f41 5245 41da 0e47 454f 4d45 5452  PE_AREA..GEOMETR
+00000240: 595f 5459 5045 53da 1343 4c55 5354 4552  Y_TYPES..CLUSTER
+00000250: 5f54 5950 455f 4b4d 4541 4e53 da11 434c  _TYPE_KMEANS..CL
+00000260: 5553 5445 525f 5459 5045 5f47 5249 4429  USTER_TYPE_GRID)
+00000270: 03da 0757 6974 6847 4953 da0b 5769 7468  ...WithGIS..With
+00000280: 4669 6c74 6572 73da 0b57 6974 6847 6172  Filters..WithGar
+00000290: 6465 6e73 2904 da11 4745 4f4a 534f 4e5f  dens)...GEOJSON_
+000002a0: 5245 4354 414e 474c 45da 0f47 454f 4a53  RECTANGLE..GEOJS
+000002b0: 4f4e 5f50 4f4c 5947 4f4e da14 4745 4f4a  ON_POLYGON..GEOJ
+000002c0: 534f 4e5f 4d55 4c54 4950 4f4c 5947 4f4e  SON_MULTIPOLYGON
+000002d0: da19 4745 4f4a 534f 4e5f 4645 4154 5552  ..GEOJSON_FEATUR
+000002e0: 4543 4f4c 4c45 4354 494f 4e29 06da 124d  ECOLLECTION)...M
+000002f0: 6170 436c 7573 7465 7256 6965 7742 6173  apClusterViewBas
+00000300: 65da 0d4b 6d65 616e 7343 6c75 7374 6572  e..KmeansCluster
+00000310: da0b 4772 6964 436c 7573 7465 72da 1147  ..GridCluster..G
+00000320: 6574 436c 7573 7465 7243 6f6e 7465 6e74  etClusterContent
+00000330: da0e 4765 7441 7265 6143 6f6e 7465 6e74  ..GetAreaContent
+00000340: da12 4765 744d 6170 436f 6e74 656e 7443  ..GetMapContentC
+00000350: 6f75 6e74 2901 da07 4761 7264 656e 734e  ount)...GardensN
+00000360: e900 0100 00e9 0a00 0000 6300 0000 0000  ..........c.....
+00000370: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
+00000380: 0000 0073 3400 0000 6500 5a01 6400 5a02  ...s4...e.Z.d.Z.
+00000390: 6401 6402 8400 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
+000003a0: 6405 6406 8400 5a05 6407 6408 8400 5a06  d.d...Z.d.d...Z.
+000003b0: 6409 640a 8400 5a07 640b 5300 290c da16  d.d...Z.d.S.)...
+000003c0: 5465 7374 4d61 7043 6c75 7374 6572 5669  TestMapClusterVi
+000003d0: 6577 4261 7365 6301 0000 0000 0000 0000  ewBasec.........
+000003e0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+000003f0: 0e00 0000 7400 7401 6401 9c02 7d01 7c01  ....t.t.d...}.|.
+00000400: 5300 a902 4ea9 02da 047a 6f6f 6dda 0967  S...N....zoom..g
+00000410: 7269 645f 7369 7a65 a902 da04 5a4f 4f4d  rid_size....ZOOM
+00000420: da09 4752 4944 5f53 495a 45a9 02da 0473  ..GRID_SIZE....s
+00000430: 656c 66da 0a75 726c 5f6b 7761 7267 73a9  elf..url_kwargs.
+00000440: 0072 2900 0000 fa43 2f68 6f6d 652f 746f  .r)....C/home/to
+00000450: 6d2f 616e 7963 6c75 7374 6572 2f64 656d  m/anycluster/dem
+00000460: 6f2f 646a 616e 676f 2f61 6e79 636c 7573  o/django/anyclus
+00000470: 7465 722f 6170 692f 7465 7374 732f 7465  ter/api/tests/te
+00000480: 7374 5f76 6965 7773 2e70 79da 0e67 6574  st_views.py..get
+00000490: 5f75 726c 5f6b 7761 7267 731c 0000 0073  _url_kwargs....s
+000004a0: 0800 0000 0003 0201 02fe 0605 7a25 5465  ............z%Te
+000004b0: 7374 4d61 7043 6c75 7374 6572 5669 6577  stMapClusterView
+000004c0: 4261 7365 2e67 6574 5f75 726c 5f6b 7761  Base.get_url_kwa
+000004d0: 7267 7363 0100 0000 0000 0000 0000 0000  rgsc............
+000004e0: 0500 0000 0400 0000 4300 0000 7330 0000  ........C...s0..
+000004f0: 0074 0083 007d 017c 00a0 01a1 007d 0274  .t...}.|.....}.t
+00000500: 0264 017c 0264 028d 027d 037c 01a0 037c  .d.|.d...}.|...|
+00000510: 0369 00a1 027d 0469 007c 045f 047c 0453  .i...}.i.|._.|.S
+00000520: 00a9 034e da0e 6b6d 6561 6e73 5f63 6c75  ...N..kmeans_clu
+00000530: 7374 6572 a901 da06 6b77 6172 6773 2905  ster....kwargs).
+00000540: 7203 0000 0072 2b00 0000 7202 0000 00da  r....r+...r.....
+00000550: 0470 6f73 74da 0773 6573 7369 6f6e 2905  .post..session).
+00000560: 7227 0000 00da 0766 6163 746f 7279 7228  r'.....factoryr(
+00000570: 0000 00da 0375 726c da07 7265 7175 6573  .....url..reques
+00000580: 7472 2900 0000 7229 0000 0072 2a00 0000  tr)...r)...r*...
+00000590: da0b 6765 745f 7265 7175 6573 7426 0000  ..get_request&..
+000005a0: 0073 0c00 0000 0002 0602 0801 0c01 0c02  .s..............
+000005b0: 0602 7a22 5465 7374 4d61 7043 6c75 7374  ..z"TestMapClust
+000005c0: 6572 5669 6577 4261 7365 2e67 6574 5f72  erViewBase.get_r
+000005d0: 6571 7565 7374 6301 0000 0000 0000 0000  equestc.........
+000005e0: 0000 000b 0000 000a 0000 0043 0000 0073  ...........C...s
+000005f0: 7000 0000 7c00 a000 a100 7d01 7401 8300  p...|.....}.t...
+00000600: 7d02 7c00 a002 a100 7d03 6401 7d04 6402  }.|.....}.d.}.d.
+00000610: 7d05 7c00 a003 a100 7d06 7404 4400 5d40  }.|.....}.t.D.]@
+00000620: 7d07 7405 4400 5d36 7d08 7c06 4400 5d2c  }.t.D.]6}.|.D.],
+00000630: 7d09 7c02 6a06 7c07 7c08 7c09 7c04 7c05  }.|.j.|.|.|.|.|.
+00000640: 7c01 6606 7c03 8e01 7d0a 7c00 a007 7408  |.f.|...}.|...t.
+00000650: 7c0a 7409 8302 a101 0100 713a 7132 712a  |.t.......q:q2q*
+00000660: 6400 5300 2903 4e46 69e6 1000 0029 0a72  d.S.).NFi....).r
+00000670: 3500 0000 7215 0000 0072 2b00 0000 da10  5...r....r+.....
+00000680: 6765 745f 7465 7374 5f66 696c 7465 7273  get_test_filters
+00000690: 720b 0000 0072 0800 0000 5a11 6765 745f  r....r....Z.get_
+000006a0: 6d61 705f 636c 7573 7465 7265 72da 0a61  map_clusterer..a
+000006b0: 7373 6572 7454 7275 65da 0a69 7369 6e73  ssertTrue..isins
+000006c0: 7461 6e63 6572 0700 0000 290b 7227 0000  tancer....).r'..
+000006d0: 0072 3400 0000 da04 6261 7365 722f 0000  .r4.....baser/..
+000006e0: 00da 0b63 6c65 6172 5f63 6163 6865 5a0b  ...clear_cacheZ.
+000006f0: 6f75 7470 7574 5f73 7269 64da 0c66 696c  output_srid..fil
+00000700: 7465 725f 6c69 7374 73da 0d67 656f 6d65  ter_lists..geome
+00000710: 7472 795f 7479 7065 da0b 636c 7573 7465  try_type..cluste
+00000720: 7274 7970 65da 0766 696c 7465 7273 5a09  rtype..filtersZ.
+00000730: 636c 7573 7465 7265 7272 2900 0000 7229  clustererr)...r)
+00000740: 0000 0072 2a00 0000 da16 7465 7374 5f67  ...r*.....test_g
+00000750: 6574 5f6d 6170 5f63 6c75 7374 6572 6572  et_map_clusterer
+00000760: 3300 0000 731e 0000 0000 0208 0206 0108  3...s...........
+00000770: 0204 0204 0108 0208 0108 0208 010e 0102  ................
+00000780: ff02 0102 ff04 027a 2d54 6573 744d 6170  .......z-TestMap
+00000790: 436c 7573 7465 7256 6965 7742 6173 652e  ClusterViewBase.
+000007a0: 7465 7374 5f67 6574 5f6d 6170 5f63 6c75  test_get_map_clu
+000007b0: 7374 6572 6572 6301 0000 0000 0000 0000  stererc.........
+000007c0: 0000 0008 0000 000a 0000 0043 0000 0073  ...........C...s
+000007d0: 5a00 0000 7c00 a000 a100 7d01 7401 8300  Z...|.....}.t...
+000007e0: 7d02 7c00 a002 a100 7d03 7403 4400 5d3a  }.|.....}.t.D.]:
+000007f0: 7d04 7404 4400 5d30 7d05 7c03 4400 5d26  }.t.D.]0}.|.D.]&
+00000800: 7d06 7c02 a005 7c04 7406 7c05 7c01 7c06  }.|...|.t.|.|.|.
+00000810: a105 7d07 7c00 a007 7408 7c07 7409 8302  ..}.|...t.|.t...
+00000820: a101 0100 712a 7122 711a 6400 5300 2901  ....q*q"q.d.S.).
+00000830: 4e29 0a72 3500 0000 7215 0000 0072 3600  N).r5...r....r6.
+00000840: 0000 720b 0000 0072 0800 0000 da09 6765  ..r....r......ge
+00000850: 745f 6361 6368 6572 2400 0000 7237 0000  t_cacher$...r7..
+00000860: 0072 3800 0000 7206 0000 0029 0872 2700  .r8...r....).r'.
+00000870: 0000 7234 0000 0072 3900 0000 723b 0000  ..r4...r9...r;..
+00000880: 0072 3c00 0000 723d 0000 0072 3e00 0000  .r<...r=...r>...
+00000890: da05 6361 6368 6572 2900 0000 7229 0000  ..cacher)...r)..
+000008a0: 0072 2a00 0000 da0e 7465 7374 5f67 6574  .r*.....test_get
+000008b0: 5f63 6163 6865 4800 0000 7310 0000 0000  _cacheH...s.....
+000008c0: 0208 0206 0208 0208 0108 0208 0112 027a  ...............z
+000008d0: 2554 6573 744d 6170 436c 7573 7465 7256  %TestMapClusterV
+000008e0: 6965 7742 6173 652e 7465 7374 5f67 6574  iewBase.test_get
+000008f0: 5f63 6163 6865 6301 0000 0000 0000 0000  _cachec.........
+00000900: 0000 0009 0000 000a 0000 0043 0000 0073  ...........C...s
+00000910: 8e00 0000 7c00 a000 a100 7d01 7401 8300  ....|.....}.t...
+00000920: 7d02 7c00 a002 a100 7d03 7403 4400 5d6e  }.|.....}.t.D.]n
+00000930: 7d04 7404 4400 5d64 7d05 7c03 4400 5d5a  }.t.D.]d}.|.D.]Z
+00000940: 7d06 7c02 a005 7c04 7406 7c05 7c01 7c06  }.|...|.t.|.|.|.
+00000950: a105 7d07 7c02 a007 7c01 7c07 a102 0100  ..}.|...|.|.....
+00000960: 7c00 a008 7c02 6a09 7c01 6a0a a102 0100  |...|.j.|.j.....
+00000970: 6401 4400 5d22 7d08 7c00 a00b 740c 7c07  d.D.]"}.|...t.|.
+00000980: 7c08 8302 7c01 6a0a 7c02 6a09 1900 7c08  |...|.j.|.j...|.
+00000990: 1900 a102 0100 7160 712a 7122 711a 6400  ......q`q*q"q.d.
+000009a0: 5300 2902 4e29 0472 3c00 0000 7221 0000  S.).N).r<...r!..
+000009b0: 0072 3d00 0000 723e 0000 0029 0d72 3500  .r=...r>...).r5.
+000009c0: 0000 7215 0000 0072 3600 0000 720b 0000  ..r....r6...r...
+000009d0: 0072 0800 0000 7240 0000 0072 2400 0000  .r....r@...r$...
+000009e0: 5a09 7365 745f 6361 6368 65da 0861 7373  Z.set_cache..ass
+000009f0: 6572 7449 6eda 0a63 6163 6865 5f6e 616d  ertIn..cache_nam
+00000a00: 6572 3100 0000 da0b 6173 7365 7274 4571  er1.....assertEq
+00000a10: 7561 6cda 0767 6574 6174 7472 2909 7227  ual..getattr).r'
+00000a20: 0000 0072 3400 0000 7239 0000 0072 3b00  ...r4...r9...r;.
+00000a30: 0000 723c 0000 0072 3d00 0000 723e 0000  ..r<...r=...r>..
+00000a40: 00da 0d63 6c75 7374 6572 5f63 6163 6865  ...cluster_cache
+00000a50: da04 6174 7472 7229 0000 0072 2900 0000  ..attrr)...r)...
+00000a60: 722a 0000 00da 0e74 6573 745f 7365 745f  r*.....test_set_
+00000a70: 6361 6368 6559 0000 0073 1600 0000 0002  cacheY...s......
+00000a80: 0802 0602 0802 0801 0802 0802 1202 0c02  ................
+00000a90: 1002 0802 7a25 5465 7374 4d61 7043 6c75  ....z%TestMapClu
+00000aa0: 7374 6572 5669 6577 4261 7365 2e74 6573  sterViewBase.tes
+00000ab0: 745f 7365 745f 6361 6368 654e 2908 da08  t_set_cacheN)...
+00000ac0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000ad0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000ae0: 5f5f 722b 0000 0072 3500 0000 723f 0000  __r+...r5...r?..
+00000af0: 0072 4200 0000 7249 0000 0072 2900 0000  .rB...rI...r)...
+00000b00: 7229 0000 0072 2900 0000 722a 0000 0072  r)...r)...r*...r
+00000b10: 1e00 0000 1900 0000 730a 0000 0008 0308  ........s.......
+00000b20: 0a08 0d08 1508 1172 1e00 0000 6300 0000  .......r....c...
+00000b30: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000b40: 0040 0000 0073 2800 0000 6500 5a01 6400  .@...s(...e.Z.d.
+00000b50: 5a02 6401 6402 8400 5a03 6700 6601 6403  Z.d.d...Z.g.f.d.
+00000b60: 6404 8401 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
+00000b70: 5300 2908 da0f 5465 7374 4772 6964 436c  S.)...TestGridCl
+00000b80: 7573 7465 7263 0100 0000 0000 0000 0000  usterc..........
+00000b90: 0000 0200 0000 0300 0000 4300 0000 730e  ..........C...s.
+00000ba0: 0000 0074 0074 0164 019c 027d 017c 0153  ...t.t.d...}.|.S
+00000bb0: 0072 1f00 0000 7223 0000 0072 2600 0000  .r....r#...r&...
+00000bc0: 7229 0000 0072 2900 0000 722a 0000 0072  r)...r)...r*...r
+00000bd0: 2b00 0000 7400 0000 7308 0000 0000 0302  +...t...s.......
+00000be0: 0102 fe06 057a 1e54 6573 7447 7269 6443  .....z.TestGridC
+00000bf0: 6c75 7374 6572 2e67 6574 5f75 726c 5f6b  luster.get_url_k
+00000c00: 7761 7267 7363 0200 0000 0000 0000 0000  wargsc..........
+00000c10: 0000 0300 0000 0400 0000 4300 0000 7310  ..........C...s.
+00000c20: 0000 0074 007c 0174 0164 019c 037d 027c  ...t.|.t.d...}.|
+00000c30: 0253 00a9 024e a903 da07 6765 6f6a 736f  .S...N....geojso
+00000c40: 6e72 3e00 0000 723c 0000 0029 0272 1100  nr>...r<...).r..
+00000c50: 0000 7209 0000 0029 0372 2700 0000 723e  ..r....).r'...r>
+00000c60: 0000 00da 0970 6f73 745f 6461 7461 7229  .....post_datar)
+00000c70: 0000 0072 2900 0000 722a 0000 00da 0d67  ...r)...r*.....g
+00000c80: 6574 5f70 6f73 745f 6461 7461 7d00 0000  et_post_data}...
+00000c90: 730a 0000 0000 0302 0102 0102 fd06 067a  s..............z
+00000ca0: 1d54 6573 7447 7269 6443 6c75 7374 6572  .TestGridCluster
+00000cb0: 2e67 6574 5f70 6f73 745f 6461 7461 6301  .get_post_datac.
+00000cc0: 0000 0000 0000 0000 0000 0007 0000 0006  ................
+00000cd0: 0000 0043 0000 0073 5600 0000 7c00 a000  ...C...sV...|...
+00000ce0: a100 7d01 7c00 a001 a100 7d02 7402 6401  ..}.|.....}.t.d.
+00000cf0: 7c02 6402 8d02 7d03 7c01 4400 5d30 7d04  |.d...}.|.D.]0}.
+00000d00: 7c00 a003 7c04 a101 7d05 7c00 6a04 6a05  |...|...}.|.j.j.
+00000d10: 7c03 7c05 6403 6404 8d03 7d06 7c00 a006  |.|.d.d...}.|...
+00000d20: 7c06 6a07 7408 6a09 a102 0100 7120 6400  |.j.t.j.....q d.
+00000d30: 5300 2905 4e5a 0c67 7269 645f 636c 7573  S.).NZ.grid_clus
+00000d40: 7465 7272 2e00 0000 da04 6a73 6f6e a901  terr......json..
+00000d50: da06 666f 726d 6174 290a 7236 0000 0072  ..format).r6...r
+00000d60: 2b00 0000 7202 0000 0072 5200 0000 da06  +...r....rR.....
+00000d70: 636c 6965 6e74 7230 0000 0072 4500 0000  clientr0...rE...
+00000d80: da0b 7374 6174 7573 5f63 6f64 6572 0500  ..status_coder..
+00000d90: 0000 da0b 4854 5450 5f32 3030 5f4f 4b29  ....HTTP_200_OK)
+00000da0: 0772 2700 0000 723b 0000 0072 2800 0000  .r'...r;...r(...
+00000db0: 7233 0000 0072 3e00 0000 7251 0000 00da  r3...r>...rQ....
+00000dc0: 0872 6573 706f 6e73 6572 2900 0000 7229  .responser)...r)
+00000dd0: 0000 0072 2a00 0000 da09 7465 7374 5f70  ...r*.....test_p
+00000de0: 6f73 7488 0000 0073 0e00 0000 0002 0802  ost....s........
+00000df0: 0801 0c02 0802 0a02 1202 7a19 5465 7374  ..........z.Test
+00000e00: 4772 6964 436c 7573 7465 722e 7465 7374  GridCluster.test
+00000e10: 5f70 6f73 744e 2906 724a 0000 0072 4b00  _postN).rJ...rK.
+00000e20: 0000 724c 0000 0072 2b00 0000 7252 0000  ..rL...r+...rR..
+00000e30: 0072 5a00 0000 7229 0000 0072 2900 0000  .rZ...r)...r)...
+00000e40: 7229 0000 0072 2a00 0000 724d 0000 0072  r)...r*...rM...r
+00000e50: 0000 0073 0600 0000 0802 0809 0c0b 724d  ...s..........rM
+00000e60: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000e70: 0000 0000 0300 0000 4000 0000 7330 0000  ........@...s0..
+00000e80: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+00000e90: 0364 0364 0484 005a 0467 0066 0164 0564  .d.d...Z.g.f.d.d
+00000ea0: 0684 015a 0564 0764 0884 005a 0664 0953  ...Z.d.d...Z.d.S
+00000eb0: 0029 0ada 1154 6573 744b 6d65 616e 7343  .)...TestKmeansC
+00000ec0: 6c75 7374 6572 6301 0000 0000 0000 0000  lusterc.........
+00000ed0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00000ee0: 0e00 0000 7400 7401 6401 9c02 7d01 7c01  ....t.t.d...}.|.
+00000ef0: 5300 721f 0000 0072 2300 0000 7226 0000  S.r....r#...r&..
+00000f00: 0072 2900 0000 7229 0000 0072 2a00 0000  .r)...r)...r*...
+00000f10: 722b 0000 009b 0000 0073 0800 0000 0003  r+.......s......
+00000f20: 0201 02fe 0605 7a20 5465 7374 4b6d 6561  ......z TestKmea
+00000f30: 6e73 436c 7573 7465 722e 6765 745f 7572  nsCluster.get_ur
+00000f40: 6c5f 6b77 6172 6773 6301 0000 0000 0000  l_kwargsc.......
+00000f50: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00000f60: 0073 1800 0000 7c00 a000 a100 7d01 7401  .s....|.....}.t.
+00000f70: 6401 7c01 6402 8d02 7d02 7c02 5300 722c  d.|.d...}.|.S.r,
+00000f80: 0000 0029 0272 2b00 0000 7202 0000 0029  ...).r+...r....)
+00000f90: 0372 2700 0000 7228 0000 0072 3300 0000  .r'...r(...r3...
+00000fa0: 7229 0000 0072 2900 0000 722a 0000 00da  r)...r)...r*....
+00000fb0: 0767 6574 5f75 726c a500 0000 7306 0000  .get_url....s...
+00000fc0: 0000 0208 010c 017a 1954 6573 744b 6d65  .......z.TestKme
+00000fd0: 616e 7343 6c75 7374 6572 2e67 6574 5f75  ansCluster.get_u
+00000fe0: 726c 6304 0000 0000 0000 0000 0000 0005  rlc.............
+00000ff0: 0000 0004 0000 0043 0000 0073 1000 0000  .......C...s....
+00001000: 7c02 7c03 7c01 6401 9c03 7d04 7c04 5300  |.|.|.d...}.|.S.
+00001010: 724e 0000 0072 2900 0000 2905 7227 0000  rN...r)...).r'..
+00001020: 0072 3c00 0000 7250 0000 0072 3e00 0000  .r<...rP...r>...
+00001030: 7251 0000 0072 2900 0000 7229 0000 0072  rQ...r)...r)...r
+00001040: 2a00 0000 7252 0000 00ac 0000 0073 0a00  *...rR.......s..
+00001050: 0000 0003 0201 0201 02fd 0606 7a1f 5465  ............z.Te
+00001060: 7374 4b6d 6561 6e73 436c 7573 7465 722e  stKmeansCluster.
+00001070: 6765 745f 706f 7374 5f64 6174 6163 0100  get_post_datac..
+00001080: 0000 0000 0000 0000 0000 0700 0000 0700  ................
+00001090: 0000 4300 0000 73c2 0000 007c 00a0 00a1  ..C...s....|....
+000010a0: 007d 017c 00a0 0174 0274 03a1 027d 027c  .}.|...t.t...}.|
+000010b0: 006a 046a 057c 017c 0264 0164 028d 037d  .j.j.|.|.d.d...}
+000010c0: 037c 036a 0674 076a 086b 0372 3c74 097c  .|.j.t.j.k.r<t.|
+000010d0: 036a 0a83 0101 007c 00a0 0b7c 036a 0674  .j.....|...|.j.t
+000010e0: 076a 08a1 0201 007c 00a0 0ca1 007d 0474  .j.....|.....}.t
+000010f0: 0374 0d74 0e74 0f66 0444 005d 5c7d 057c  .t.t.t.f.D.]\}.|
+00001100: 0444 005d 527d 067c 00a0 0174 107c 057c  .D.]R}.|...t.|.|
+00001110: 06a1 037d 027c 006a 046a 057c 017c 0264  ...}.|.j.j.|.|.d
+00001120: 0164 028d 037d 037c 036a 0674 076a 086b  .d...}.|.j.t.j.k
+00001130: 0372 aa74 097c 0583 0101 0074 097c 036a  .r.t.|.....t.|.j
+00001140: 0a83 0101 007c 00a0 0b7c 036a 0674 076a  .....|...|.j.t.j
+00001150: 08a1 0201 0071 6871 6064 0053 0029 034e  .....qhq`d.S.).N
+00001160: 7253 0000 0072 5400 0000 2911 725c 0000  rS...rT...).r\..
+00001170: 0072 5200 0000 7209 0000 0072 1100 0000  .rR...r....r....
+00001180: 7256 0000 0072 3000 0000 7257 0000 0072  rV...r0...rW...r
+00001190: 0500 0000 7258 0000 00da 0570 7269 6e74  ....rX.....print
+000011a0: da04 6461 7461 7245 0000 0072 3600 0000  ..datarE...r6...
+000011b0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+000011c0: 0a00 0000 2907 7227 0000 0072 3300 0000  ....).r'...r3...
+000011d0: 7251 0000 0072 5900 0000 723b 0000 0072  rQ...rY...r;...r
+000011e0: 5000 0000 723e 0000 0072 2900 0000 7229  P...r>...r)...r)
+000011f0: 0000 0072 2a00 0000 725a 0000 00b7 0000  ...r*...rZ......
+00001200: 0073 1e00 0000 0002 0803 0c02 1202 0c01  .s..............
+00001210: 0a01 1002 0801 1002 0802 0e02 1202 0c01  ................
+00001220: 0801 0a01 7a1b 5465 7374 4b6d 6561 6e73  ....z.TestKmeans
+00001230: 436c 7573 7465 722e 7465 7374 5f70 6f73  Cluster.test_pos
+00001240: 744e 2907 724a 0000 0072 4b00 0000 724c  tN).rJ...rK...rL
+00001250: 0000 0072 2b00 0000 725c 0000 0072 5200  ...r+...r\...rR.
+00001260: 0000 725a 0000 0072 2900 0000 7229 0000  ..rZ...r)...r)..
+00001270: 0072 2900 0000 722a 0000 0072 5b00 0000  .r)...r*...r[...
+00001280: 9900 0000 7308 0000 0008 0208 0a08 070c  ....s...........
+00001290: 0b72 5b00 0000 6300 0000 0000 0000 0000  .r[...c.........
+000012a0: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+000012b0: 1400 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
+000012c0: 8400 5a03 6403 5300 2904 da1b 5465 7374  ..Z.d.S.)...Test
+000012d0: 4765 744b 6d65 616e 7343 6c75 7374 6572  GetKmeansCluster
+000012e0: 436f 6e74 656e 7463 0100 0000 0000 0000  Contentc........
+000012f0: 0000 0000 1800 0000 0b00 0000 4300 0000  ............C...
+00001300: 73ee 0100 007c 00a0 00a1 007d 0174 0144  s....|.....}.t.D
+00001310: 0090 015d da7d 027c 0144 0090 015d ce7d  ...].}.|.D...].}
+00001320: 0374 0274 0364 019c 027d 0474 0464 027c  .t.t.d...}.t.d.|
+00001330: 0464 038d 027d 0574 057c 037c 0264 049c  .d...}.t.|.|.d..
+00001340: 037d 0674 0683 007d 077c 076a 077c 057c  .}.t...}.|.j.|.|
+00001350: 0664 0564 068d 037d 0869 007c 085f 0874  .d.d...}.i.|._.t
+00001360: 09a0 0aa1 007d 097c 097c 0866 017c 048e  .....}.|.|.f.|..
+00001370: 017d 0a7c 0274 0b6b 0272 907c 00a0 0c74  .}.|.t.k.r.|...t
+00001380: 0d7c 086a 0864 0719 0064 0819 0083 0164  .|.j.d...d.....d
+00001390: 09a1 0201 007c 0a6a 0e64 0a19 007d 0b74  .....|.j.d...}.t
+000013a0: 0f7c 0274 0274 107c 0383 047d 0c7c 0ca0  .|.t.t.|...}.|..
+000013b0: 117c 086a 0864 0719 00a1 0101 007c 00a0  .|.j.d.......|..
+000013c0: 0c7c 0c6a 127c 086a 0864 0719 0064 0819  .|.j.|.j.d...d..
+000013d0: 00a1 0201 007c 0274 0b6b 0290 0172 067c  .....|.t.k...r.|
+000013e0: 00a0 0c74 0d7c 0c6a 1283 0164 09a1 0201  ...t.|.j...d....
+000013f0: 007c 0c6a 1264 0a19 007d 0d7c 00a0 0c74  .|.j.d...}.|...t
+00001400: 137c 0d83 0174 14a1 0201 0074 157c 0c83  .|...t.....t.|..
+00001410: 017d 0e7c 0b64 0b19 007d 0f7c 0b64 0c19  .}.|.d...}.|.d..
+00001420: 0064 0d19 007d 107c 0b64 0c19 0064 0e19  .d...}.|.d...d..
+00001430: 007d 117c 00a0 0c7c 0e6a 166a 127c 086a  .}.|...|.j.j.|.j
+00001440: 0864 0719 0064 0819 00a1 0201 0074 177c  .d...d.......t.|
+00001450: 0ea0 187c 027c 0f7c 107c 117c 0374 02a1  ...|.|.|.|.|.t..
+00001460: 0683 017d 127c 00a0 1974 0d74 177c 1283  ...}.|...t.t.|..
+00001470: 0183 0164 0a6b 04a1 0101 007c 00a0 0c74  ...d.k.....|...t
+00001480: 0d74 177c 1283 0183 017c 0b64 0f19 00a1  .t.|.....|.d....
+00001490: 0201 0074 0464 107c 0464 038d 027d 137c  ...t.d.|.d...}.|
+000014a0: 027c 0f7c 107c 117c 0364 119c 057d 147c  .|.|.|.|.d...}.|
+000014b0: 076a 077c 137c 1464 0564 068d 037d 157c  .j.|.|.d.d...}.|
+000014c0: 086a 087c 155f 0874 1aa0 0aa1 007d 167c  .j.|._.t.....}.|
+000014d0: 167c 1566 017c 048e 017d 177c 00a0 0c7c  .|.f.|...}.|...|
+000014e0: 176a 1b74 1c6a 1da1 0201 0071 1671 0c64  .j.t.j.....q.q.d
+000014f0: 0053 0029 124e 7220 0000 0072 2d00 0000  .S.).Nr ...r-...
+00001500: 722e 0000 0072 4f00 0000 7253 0000 0072  r....rO...rS...r
+00001510: 5400 0000 5a10 616e 7963 6c75 7374 6572  T...Z.anycluster
+00001520: 5f63 6163 6865 da0a 6765 6f6d 6574 7269  _cache..geometri
+00001530: 6573 e901 0000 0072 0100 0000 da03 6964  es.....r......id
+00001540: 73da 0663 656e 7465 72da 0178 da01 79da  s..center..x..y.
+00001550: 0563 6f75 6e74 da1a 6765 745f 6b6d 6561  .count..get_kmea
+00001560: 6e73 5f63 6c75 7374 6572 5f63 6f6e 7465  ns_cluster_conte
+00001570: 6e74 2905 723c 0000 0072 6200 0000 7264  nt).r<...rb...rd
+00001580: 0000 0072 6500 0000 723e 0000 0029 1e72  ...re...r>...).r
+00001590: 3600 0000 720b 0000 0072 2400 0000 7225  6...r....r$...r%
+000015a0: 0000 0072 0200 0000 7211 0000 0072 0300  ...r....r....r..
+000015b0: 0000 7230 0000 0072 3100 0000 7216 0000  ..r0...r1...r...
+000015c0: 00da 0761 735f 7669 6577 720a 0000 0072  ...as_viewr....r
+000015d0: 4500 0000 da03 6c65 6e72 5e00 0000 7206  E.....lenr^...r.
+000015e0: 0000 0072 0c00 0000 da0f 6c6f 6164 5f67  ...r......load_g
+000015f0: 656f 6d65 7472 6965 7372 6000 0000 da04  eometriesr`.....
+00001600: 7479 7065 da03 7374 7272 0700 0000 7247  type..strr....rG
+00001610: 0000 00da 046c 6973 7472 6700 0000 7237  .....listrg...r7
+00001620: 0000 0072 1800 0000 7257 0000 0072 0500  ...r....rW...r..
+00001630: 0000 7258 0000 0029 1872 2700 0000 723b  ..rX...).r'...r;
+00001640: 0000 0072 3c00 0000 723e 0000 0072 2800  ...r<...r>...r(.
+00001650: 0000 5a0a 6b6d 6561 6e73 5f75 726c 5a10  ..Z.kmeans_urlZ.
+00001660: 6b6d 6561 6e73 5f70 6f73 745f 6461 7461  kmeans_post_data
+00001670: 7232 0000 005a 0e6b 6d65 616e 735f 7265  r2...Z.kmeans_re
+00001680: 7175 6573 745a 0b6b 6d65 616e 735f 7669  questZ.kmeans_vi
+00001690: 6577 5a0f 6b6d 6561 6e73 5f72 6573 706f  ewZ.kmeans_respo
+000016a0: 6e73 655a 0763 6c75 7374 6572 7247 0000  nseZ.clusterrG..
+000016b0: 00da 0467 656f 6d5a 0d6d 6170 5f63 6c75  ...geomZ.map_clu
+000016c0: 7374 6572 6572 7262 0000 0072 6400 0000  stererrb...rd...
+000016d0: 7265 0000 005a 0f63 6c75 7374 6572 5f63  re...Z.cluster_c
+000016e0: 6f6e 7465 6e74 7233 0000 0072 5100 0000  ontentr3...rQ...
+000016f0: 7234 0000 00da 0476 6965 7772 5900 0000  r4.....viewrY...
+00001700: 7229 0000 0072 2900 0000 722a 0000 0072  r)...r)...r*...r
+00001710: 5a00 0000 d500 0000 735c 0000 0000 0208  Z.......s\......
+00001720: 020a 020a 0302 0102 fe06 050c 0302 0102  ................
+00001730: 0102 fd06 0606 0110 0106 0208 020c 0208  ................
+00001740: 011a 020a 030e 0110 0218 020a 0112 020a  ................
+00001750: 0210 0208 0208 010c 010c 021a 0218 0216  ................
+00001760: 0118 040c 0302 0102 0102 0102 0102 fb06  ................
+00001770: 0810 0108 0208 010c 027a 2554 6573 7447  .........z%TestG
+00001780: 6574 4b6d 6561 6e73 436c 7573 7465 7243  etKmeansClusterC
+00001790: 6f6e 7465 6e74 2e74 6573 745f 706f 7374  ontent.test_post
+000017a0: 4ea9 0472 4a00 0000 724b 0000 0072 4c00  N..rJ...rK...rL.
+000017b0: 0000 725a 0000 0072 2900 0000 7229 0000  ..rZ...r)...r)..
+000017c0: 0072 2900 0000 722a 0000 0072 5f00 0000  .r)...r*...r_...
+000017d0: d300 0000 7302 0000 0008 0272 5f00 0000  ....s......r_...
+000017e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000017f0: 0002 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
+00001800: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
+00001810: 5300 2904 da12 5465 7374 4765 7441 7265  S.)...TestGetAre
+00001820: 6143 6f6e 7465 6e74 6301 0000 0000 0000  aContentc.......
+00001830: 0000 0000 0008 0000 0007 0000 0043 0000  .............C..
+00001840: 0073 e200 0000 7400 7401 6401 9c02 7d01  .s....t.t.d...}.
+00001850: 7402 6402 7c01 6403 8d02 7d02 7c00 a003  t.d.|.d...}.|...
+00001860: a100 7d03 7404 7405 7406 7407 6604 4400  ..}.t.t.t.t.f.D.
+00001870: 5db2 7d04 7c03 4400 5da8 7d05 7408 7c04  ].}.|.D.].}.t.|.
+00001880: 7c05 6404 9c03 7d06 7c00 6a09 6a0a 7c02  |.d...}.|.j.j.|.
+00001890: 7c06 6405 6406 8d03 7d07 7c07 6a0b 740c  |.d.d...}.|.j.t.
+000018a0: 6a0d 6b03 7272 740e 7c04 8301 0100 740e  j.k.rrt.|.....t.
+000018b0: 7c07 6a0f 8301 0100 7c00 a010 7c07 6a0b  |.j.....|...|.j.
+000018c0: 740c 6a0d a102 0100 7c00 a011 7412 7c07  t.j.....|...t.|.
+000018d0: 6a0f 8301 6407 6b04 a101 0100 7c06 a013  j...d.k.....|...
+000018e0: 6408 6407 6409 9c02 a101 0100 7c00 6a09  d.d.d.......|.j.
+000018f0: 6a0a 7c02 7c06 6405 6406 8d03 7d07 7c00  j.|.|.d.d...}.|.
+00001900: a010 7412 7c07 6a0f 8301 6408 a102 0100  ..t.|.j...d.....
+00001910: 7c00 a010 7c07 6a0b 740c 6a0d a102 0100  |...|.j.t.j.....
+00001920: 7132 712a 6400 5300 290a 4e72 2000 0000  q2q*d.S.).Nr ...
+00001930: 5a10 6765 745f 6172 6561 5f63 6f6e 7465  Z.get_area_conte
+00001940: 6e74 722e 0000 00a9 0372 3c00 0000 7250  ntr......r<...rP
+00001950: 0000 0072 3e00 0000 7253 0000 0072 5400  ...r>...rS...rT.
+00001960: 0000 7201 0000 0072 6100 0000 2902 da05  ..r....ra...)...
+00001970: 6c69 6d69 74da 066f 6666 7365 7429 1472  limit..offset).r
+00001980: 2400 0000 7225 0000 0072 0200 0000 7236  $...r%...r....r6
+00001990: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
+000019a0: 0000 7214 0000 0072 0a00 0000 7256 0000  ..r....r....rV..
+000019b0: 0072 3000 0000 7257 0000 0072 0500 0000  .r0...rW...r....
+000019c0: 7258 0000 0072 5d00 0000 725e 0000 0072  rX...r]...r^...r
+000019d0: 4500 0000 7237 0000 0072 6900 0000 da06  E...r7...ri.....
+000019e0: 7570 6461 7465 a908 7227 0000 0072 2800  update..r'...r(.
+000019f0: 0000 7233 0000 0072 3b00 0000 7250 0000  ..r3...r;...rP..
+00001a00: 0072 3e00 0000 7251 0000 0072 5900 0000  .r>...rQ...rY...
+00001a10: 7229 0000 0072 2900 0000 722a 0000 0072  r)...r)...r*...r
+00001a20: 5a00 0000 2801 0000 7330 0000 0000 0302  Z...(...s0......
+00001a30: 0102 fe06 050c 0208 0210 0208 0302 0102  ................
+00001a40: 0102 fd06 0612 020c 0108 010a 0210 0214  ................
+00001a50: 0304 0102 0102 fe08 0612 0212 017a 1c54  .............z.T
+00001a60: 6573 7447 6574 4172 6561 436f 6e74 656e  estGetAreaConten
+00001a70: 742e 7465 7374 5f70 6f73 744e 7270 0000  t.test_postNrp..
+00001a80: 0072 2900 0000 7229 0000 0072 2900 0000  .r)...r)...r)...
+00001a90: 722a 0000 0072 7100 0000 2601 0000 7302  r*...rq...&...s.
+00001aa0: 0000 0008 0272 7100 0000 6300 0000 0000  .....rq...c.....
+00001ab0: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
+00001ac0: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00001ad0: 6401 6402 8400 5a03 6403 5300 2904 da15  d.d...Z.d.S.)...
+00001ae0: 5465 7374 4765 7444 6174 6173 6574 436f  TestGetDatasetCo
+00001af0: 6e74 656e 7463 0100 0000 0000 0000 0000  ntentc..........
+00001b00: 0000 0600 0000 0400 0000 4300 0000 737c  ..........C...s|
+00001b10: 0000 0074 006a 01a0 02a1 00a0 03a1 007d  ...t.j.........}
+00001b20: 0174 0474 057c 016a 0664 019c 037d 0274  .t.t.|.j.d...}.t
+00001b30: 0764 027c 0264 038d 027d 037c 006a 086a  .d.|.d...}.|.j.j
+00001b40: 097c 0364 0464 058d 027d 047c 00a0 0a7c  .|.d.d...}.|...|
+00001b50: 046a 0b74 0c6a 0da1 0201 0074 0ea0 0f7c  .j.t.j.....t...|
+00001b60: 046a 10a1 017d 057c 00a0 0a7c 0564 0619  .j...}.|...|.d..
+00001b70: 007c 016a 06a1 0201 007c 00a0 0a7c 0564  .|.j.....|...|.d
+00001b80: 0719 007c 016a 11a1 0201 0064 0053 0029  ...|.j.....d.S.)
+00001b90: 084e 2903 7221 0000 0072 2200 0000 5a0a  .N).r!...r"...Z.
+00001ba0: 6461 7461 7365 745f 6964 5a13 6765 745f  dataset_idZ.get_
+00001bb0: 6461 7461 7365 745f 636f 6e74 656e 7472  dataset_contentr
+00001bc0: 2e00 0000 7253 0000 0072 5400 0000 da02  ....rS...rT.....
+00001bd0: 6964 da05 7374 796c 6529 1272 1b00 0000  id..style).r....
+00001be0: da07 6f62 6a65 6374 73da 0361 6c6c da04  ..objects..all..
+00001bf0: 6c61 7374 7224 0000 0072 2500 0000 7278  lastr$...r%...rx
+00001c00: 0000 0072 0200 0000 7256 0000 00da 0367  ...r....rV.....g
+00001c10: 6574 7245 0000 0072 5700 0000 7205 0000  etrE...rW...r...
+00001c20: 0072 5800 0000 7253 0000 00da 056c 6f61  .rX...rS.....loa
+00001c30: 6473 da07 636f 6e74 656e 7472 7900 0000  ds..contentry...
+00001c40: 2906 7227 0000 005a 0764 6174 6173 6574  ).r'...Z.dataset
+00001c50: 7228 0000 0072 3300 0000 7259 0000 00da  r(...r3...rY....
+00001c60: 0f70 6172 7365 645f 7265 7370 6f6e 7365  .parsed_response
+00001c70: 7229 0000 0072 2900 0000 722a 0000 00da  r)...r)...r*....
+00001c80: 0874 6573 745f 6765 7456 0100 0073 1600  .test_getV...s..
+00001c90: 0000 0002 0e03 0201 0201 04fd 0606 0c02  ................
+00001ca0: 1002 1002 0c01 1201 7a1e 5465 7374 4765  ........z.TestGe
+00001cb0: 7444 6174 6173 6574 436f 6e74 656e 742e  tDatasetContent.
+00001cc0: 7465 7374 5f67 6574 4e29 0472 4a00 0000  test_getN).rJ...
+00001cd0: 724b 0000 0072 4c00 0000 7281 0000 0072  rK...rL...r....r
+00001ce0: 2900 0000 7229 0000 0072 2900 0000 722a  )...r)...r)...r*
+00001cf0: 0000 0072 7700 0000 5401 0000 7302 0000  ...rw...T...s...
+00001d00: 0008 0272 7700 0000 6300 0000 0000 0000  ...rw...c.......
+00001d10: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
+00001d20: 0073 1c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00001d30: 6402 8400 5a03 6403 6404 8400 5a04 6405  d...Z.d.d...Z.d.
+00001d40: 5300 2906 da16 5465 7374 4765 744d 6170  S.)...TestGetMap
+00001d50: 436f 6e74 656e 7443 6f75 6e74 6301 0000  ContentCountc...
+00001d60: 0000 0000 0000 0000 0008 0000 0007 0000  ................
+00001d70: 0043 0000 0073 9200 0000 7c00 a000 a100  .C...s....|.....
+00001d80: 0100 7401 7402 6401 9c02 7d01 7403 6402  ..t.t.d...}.t.d.
+00001d90: 7c01 6403 8d02 7d02 7c00 a004 a100 7d03  |.d...}.|.....}.
+00001da0: 7405 7406 7407 7408 6604 4400 5d5a 7d04  t.t.t.t.f.D.]Z}.
+00001db0: 7c03 4400 5d50 7d05 7409 7c04 7c05 6404  |.D.]P}.t.|.|.d.
+00001dc0: 9c03 7d06 7c00 6a0a 6a0b 7c02 7c06 6405  ..}.|.j.j.|.|.d.
+00001dd0: 6406 8d03 7d07 7c07 6a0c 740d 6a0e 6b03  d...}.|.j.t.j.k.
+00001de0: 727a 740f 7c04 8301 0100 740f 7c07 6a10  rzt.|.....t.|.j.
+00001df0: 8301 0100 7c00 a011 7c07 6a0c 740d 6a0e  ....|...|.j.t.j.
+00001e00: a102 0100 713a 7132 6400 5300 2907 4e72  ....q:q2d.S.).Nr
+00001e10: 2000 0000 da15 6765 745f 6d61 705f 636f   .....get_map_co
+00001e20: 6e74 656e 745f 636f 756e 7472 2e00 0000  ntent_countr....
+00001e30: 7272 0000 0072 5300 0000 7254 0000 0029  rr...rS...rT...)
+00001e40: 12da 0d63 7265 6174 655f 706f 696e 7473  ...create_points
+00001e50: 7224 0000 0072 2500 0000 7202 0000 0072  r$...r%...r....r
+00001e60: 3600 0000 7211 0000 0072 1200 0000 7213  6...r....r....r.
+00001e70: 0000 0072 1400 0000 720a 0000 0072 5600  ...r....r....rV.
+00001e80: 0000 7230 0000 0072 5700 0000 7205 0000  ..r0...rW...r...
+00001e90: 0072 5800 0000 725d 0000 0072 5e00 0000  .rX...r]...r^...
+00001ea0: 7245 0000 0072 7600 0000 7229 0000 0072  rE...rv...r)...r
+00001eb0: 2900 0000 722a 0000 0072 5a00 0000 6d01  )...r*...rZ...m.
+00001ec0: 0000 7322 0000 0000 0208 0302 0102 fe06  ..s"............
+00001ed0: 050c 0208 0210 0208 0302 0102 0102 fd06  ................
+00001ee0: 0612 020c 0108 010a 047a 2054 6573 7447  .........z TestG
+00001ef0: 6574 4d61 7043 6f6e 7465 6e74 436f 756e  etMapContentCoun
+00001f00: 742e 7465 7374 5f70 6f73 7463 0100 0000  t.test_postc....
+00001f10: 0000 0000 0000 0000 0a00 0000 0700 0000  ................
+00001f20: 4300 0000 73f2 0000 0064 0164 0264 0364  C...s....d.d.d.d
+00001f30: 0464 059c 0367 0169 0164 0164 0264 0664  .d...g.i.d.d.d.d
+00001f40: 0464 059c 0367 0169 0164 079c 027d 017c  .d...g.i.d...}.|
+00001f50: 00a0 00a1 0001 0074 0174 0264 089c 027d  .......t.t.d...}
+00001f60: 0274 0364 097c 0264 0a8d 027d 0374 0474  .t.d.|.d...}.t.t
+00001f70: 0574 0674 0766 0444 005d 9c7d 047c 00a0  .t.t.f.D.].}.|..
+00001f80: 08a1 007d 057c 0544 005d 8a7d 0674 097c  ...}.|.D.].}.t.|
+00001f90: 047c 067c 0164 0b9c 047d 077c 006a 0a6a  .|.|.d...}.|.j.j
+00001fa0: 0b7c 037c 0764 0c64 0d8d 037d 087c 086a  .|.|.d.d...}.|.j
+00001fb0: 0c74 0d6a 0e6b 0372 a274 0f7c 0483 0101  .t.j.k.r.t.|....
+00001fc0: 0074 0f7c 086a 1083 0101 0074 11a0 127c  .t.|.j.....t...|
+00001fd0: 086a 13a1 017d 097c 00a0 1464 0e7c 09a1  .j...}.|...d.|..
+00001fe0: 0201 007c 00a0 1464 037c 0964 0e19 00a1  ...|...d.|.d....
+00001ff0: 0201 007c 00a0 1464 067c 0964 0e19 00a1  ...|...d.|.d....
+00002000: 0201 007c 00a0 157c 086a 0c74 0d6a 0ea1  ...|...|.j.t.j..
+00002010: 0201 0071 6071 5064 0053 0029 0f4e 723e  ...q`qPd.S.).Nr>
+00002020: 0000 0072 7900 0000 da05 7374 6f6e 65fa  ...ry.....stone.
+00002030: 013d 2903 da06 636f 6c75 6d6e da05 7661  .=)...column..va
+00002040: 6c75 65da 086f 7065 7261 746f 72da 0666  lue..operator..f
+00002050: 6c6f 7765 7229 0272 8500 0000 728a 0000  lower).r....r...
+00002060: 0072 2000 0000 7283 0000 0072 2e00 0000  .r ...r....r....
+00002070: 2904 723c 0000 0072 5000 0000 723e 0000  ).r<...rP...r>..
+00002080: 00da 0b6d 6f64 756c 6174 696f 6e73 7253  ...modulationsrS
+00002090: 0000 0072 5400 0000 728b 0000 0029 1672  ...rT...r....).r
+000020a0: 8400 0000 7224 0000 0072 2500 0000 7202  ....r$...r%...r.
+000020b0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
+000020c0: 0000 7214 0000 0072 3600 0000 720a 0000  ..r....r6...r...
+000020d0: 0072 5600 0000 7230 0000 0072 5700 0000  .rV...r0...rW...
+000020e0: 7205 0000 0072 5800 0000 725d 0000 0072  r....rX...r]...r
+000020f0: 5e00 0000 7253 0000 0072 7e00 0000 727f  ^...rS...r~...r.
+00002100: 0000 0072 4300 0000 7245 0000 0029 0a72  ...rC...rE...).r
+00002110: 2700 0000 728b 0000 0072 2800 0000 7233  '...r....r(...r3
+00002120: 0000 0072 5000 0000 723b 0000 0072 3e00  ...rP...r;...r>.
+00002130: 0000 7251 0000 0072 5900 0000 7280 0000  ..rQ...rY...r...
+00002140: 0072 2900 0000 7229 0000 0072 2a00 0000  .r)...r)...r*...
+00002150: da13 7465 7374 5f70 6f73 745f 6d6f 6475  ..test_post_modu
+00002160: 6c61 7465 648f 0100 0073 4a00 0000 0004  lated....sJ.....
+00002170: 0202 0201 0201 02fd 04ff 02ff 020a 0202  ................
+00002180: 0201 0201 02fd 04ff 02ff 02f6 0615 0803  ................
+00002190: 0201 02fe 0605 0c02 1002 0802 0803 0201  ................
+000021a0: 0201 0201 02fc 0607 1202 0c01 0801 0a02  ................
+000021b0: 0c02 0c01 1001 1002 7a2a 5465 7374 4765  ........z*TestGe
+000021c0: 744d 6170 436f 6e74 656e 7443 6f75 6e74  tMapContentCount
+000021d0: 2e74 6573 745f 706f 7374 5f6d 6f64 756c  .test_post_modul
+000021e0: 6174 6564 4e29 0572 4a00 0000 724b 0000  atedN).rJ...rK..
+000021f0: 0072 4c00 0000 725a 0000 0072 8c00 0000  .rL...rZ...r....
+00002200: 7229 0000 0072 2900 0000 7229 0000 0072  r)...r)...r)...r
+00002210: 2a00 0000 7282 0000 006b 0100 0073 0400  *...r....k...s..
+00002220: 0000 0802 0822 7282 0000 0063 0000 0000  ....."r....c....
+00002230: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00002240: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00002250: 0264 0164 0284 005a 0364 0353 0029 04da  .d.d...Z.d.S.)..
+00002260: 1954 6573 7447 6574 4772 6f75 7065 644d  .TestGetGroupedM
+00002270: 6170 436f 6e74 656e 7473 6301 0000 0000  apContentsc.....
+00002280: 0000 0000 0000 000b 0000 0006 0000 0043  ...............C
+00002290: 0000 0073 dc00 0000 7c00 a000 a100 0100  ...s....|.......
+000022a0: 7401 7402 6401 9c02 7d01 7403 6402 7c01  t.t.d...}.t.d.|.
+000022b0: 6403 8d02 7d02 6700 7d03 7404 6a05 6a06  d...}.g.}.t.j.j.
+000022c0: 6404 6405 8d01 7d04 7c00 a007 7c04 a008  d.d...}.|...|...
+000022d0: a100 6406 6b04 a101 0100 7409 740a 740b  ..d.k.....t.t.t.
+000022e0: 740c 6604 4400 5d88 7d05 740d 7c05 7c03  t.f.D.].}.t.|.|.
+000022f0: 6407 6408 9c04 7d06 7c00 6a0e 6a0f 7c02  d.d...}.|.j.j.|.
+00002300: 7c06 6409 640a 8d03 7d07 7c07 6a10 7411  |.d.d...}.|.j.t.
+00002310: 6a12 6b03 7290 7413 7c05 8301 0100 7413  j.k.r.t.|.....t.
+00002320: 7c07 6a14 8301 0100 7415 a016 7c07 6a17  |.j.....t...|.j.
+00002330: a101 7d08 7404 6a05 a018 a100 6a19 6407  ..}.t.j.....j.d.
+00002340: 640b 640c 8d02 7d09 7c09 4400 5d10 7d0a  d.d...}.|.D.].}.
+00002350: 7c00 a01a 7c0a 7c08 a102 0100 71b4 7c00  |...|.|.....q.|.
+00002360: a01b 7c07 6a10 7411 6a12 a102 0100 714e  ..|.j.t.j.....qN
+00002370: 6400 5300 290d 4e72 2000 0000 5a18 6765  d.S.).Nr ...Z.ge
+00002380: 745f 6772 6f75 7065 645f 6d61 705f 636f  t_grouped_map_co
+00002390: 6e74 656e 7473 722e 0000 0072 8500 0000  ntentsr....r....
+000023a0: 2901 7279 0000 0072 0100 0000 7279 0000  ).ry...r....ry..
+000023b0: 0029 0472 3c00 0000 7250 0000 0072 3e00  .).r<...rP...r>.
+000023c0: 0000 da08 6772 6f75 705f 6279 7253 0000  ....group_byrS..
+000023d0: 0072 5400 0000 5429 01da 0466 6c61 7429  .rT...T)...flat)
+000023e0: 1c72 8400 0000 7224 0000 0072 2500 0000  .r....r$...r%...
+000023f0: 7202 0000 0072 1b00 0000 727a 0000 00da  r....r....rz....
+00002400: 0666 696c 7465 7272 3700 0000 7266 0000  .filterr7...rf..
+00002410: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00002420: 7214 0000 0072 0a00 0000 7256 0000 0072  r....r....rV...r
+00002430: 3000 0000 7257 0000 0072 0500 0000 7258  0...rW...r....rX
+00002440: 0000 0072 5d00 0000 725e 0000 0072 5300  ...r]...r^...rS.
+00002450: 0000 727e 0000 0072 7f00 0000 727b 0000  ..r~...r....r{..
+00002460: 00da 0b76 616c 7565 735f 6c69 7374 7243  ...values_listrC
+00002470: 0000 0072 4500 0000 290b 7227 0000 0072  ...rE...).r'...r
+00002480: 2800 0000 7233 0000 0072 3e00 0000 5a0d  (...r3...r>...Z.
+00002490: 7374 6f6e 655f 6761 7264 656e 7372 5000  stone_gardensrP.
+000024a0: 0000 7251 0000 0072 5900 0000 7280 0000  ..rQ...rY...r...
+000024b0: 00da 0673 7479 6c65 7372 7900 0000 7229  ...stylesry...r)
+000024c0: 0000 0072 2900 0000 722a 0000 0072 5a00  ...r)...r*...rZ.
+000024d0: 0000 cd01 0000 732e 0000 0000 0208 0302  ......s.........
+000024e0: 0102 fe06 050c 0204 020e 0112 0210 0302  ................
+000024f0: 0102 0102 0102 fc06 0712 020c 0108 010a  ................
+00002500: 020c 0114 0208 010e 027a 2354 6573 7447  .........z#TestG
+00002510: 6574 4772 6f75 7065 644d 6170 436f 6e74  etGroupedMapCont
+00002520: 656e 7473 2e74 6573 745f 706f 7374 4e72  ents.test_postNr
+00002530: 7000 0000 7229 0000 0072 2900 0000 7229  p...r)...r)...r)
+00002540: 0000 0072 2a00 0000 728d 0000 00cb 0100  ...r*...r.......
+00002550: 0073 0200 0000 0802 728d 0000 0029 30da  .s......r....)0.
+00002560: 0b64 6a61 6e67 6f2e 7572 6c73 7202 0000  .django.urlsr...
+00002570: 005a 1372 6573 745f 6672 616d 6577 6f72  .Z.rest_framewor
+00002580: 6b2e 7465 7374 7203 0000 0072 0400 0000  k.testr....r....
+00002590: da0e 7265 7374 5f66 7261 6d65 776f 726b  ..rest_framework
+000025a0: 7205 0000 00da 0a61 6e79 636c 7573 7465  r......anycluste
+000025b0: 7272 0600 0000 5a17 616e 7963 6c75 7374  rr....Z.anyclust
+000025c0: 6572 2e4d 6170 436c 7573 7465 7265 7272  er.MapClustererr
+000025d0: 0700 0000 da16 616e 7963 6c75 7374 6572  ......anycluster
+000025e0: 2e64 6566 696e 6974 696f 6e73 7208 0000  .definitionsr...
+000025f0: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00002600: 720c 0000 0072 0d00 0000 5a17 616e 7963  r....r....Z.anyc
+00002610: 6c75 7374 6572 2e74 6573 7473 2e6d 6978  luster.tests.mix
+00002620: 696e 7372 0e00 0000 720f 0000 0072 1000  insr....r....r..
+00002630: 0000 5a17 616e 7963 6c75 7374 6572 2e74  ..Z.anycluster.t
+00002640: 6573 7473 2e63 6f6d 6d6f 6e72 1100 0000  ests.commonr....
+00002650: 7212 0000 0072 1300 0000 7214 0000 005a  r....r....r....Z
+00002660: 1461 6e79 636c 7573 7465 722e 6170 692e  .anycluster.api.
+00002670: 7669 6577 7372 1500 0000 7216 0000 0072  viewsr....r....r
+00002680: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
+00002690: 0000 005a 0d61 6e79 6d61 702e 6d6f 6465  ...Z.anymap.mode
+000026a0: 6c73 721b 0000 0072 5300 0000 5a0c 4d41  lsr....rS...Z.MA
+000026b0: 505f 5449 4c45 5349 5a45 7225 0000 0072  P_TILESIZEr%...r
+000026c0: 2400 0000 721e 0000 0072 4d00 0000 725b  $...r....rM...r[
+000026d0: 0000 0072 5f00 0000 7271 0000 0072 7700  ...r_...rq...rw.
+000026e0: 0000 7282 0000 0072 8d00 0000 7229 0000  ..r....r....r)..
+000026f0: 0072 2900 0000 7229 0000 0072 2a00 0000  .r)...r)...r*...
+00002700: da08 3c6d 6f64 756c 653e 0100 0000 732a  ..<module>....s*
+00002710: 0000 000c 0110 010c 020c 010c 0120 0314  ............. ..
+00002720: 0118 0220 040c 0208 0204 0104 0104 0212  ... ............
+00002730: 5914 2714 3a14 5314 2e14 1714 60         Y.'.:.S.....`
```

### Comparing `anycluster-2.2.0/anycluster/api/tests/test_serializers.py` & `anycluster-2.3.0/anycluster/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/api/tests/test_views.py` & `anycluster-2.3.0/anycluster/api/tests/test_views.py`

 * *Files 5% similar despite different names*

```diff
@@ -318,14 +318,50 @@
 
                 if response.status_code != status.HTTP_200_OK:
                     print(geojson)
                     print(response.data)
                     
                 self.assertEqual(response.status_code, status.HTTP_200_OK)
 
+                self.assertTrue(len(response.data) > 0)
+
+
+                post_data.update({
+                    'limit': 1,
+                    'offset': 0,
+                })
+
+
+                response = self.client.post(url, post_data, format='json')
+
+                self.assertEqual(len(response.data), 1)
+                self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+
+class TestGetDatasetContent(WithGIS, WithFilters, APITestCase):
+
+    def test_get(self):
+
+        dataset = Gardens.objects.all().last()
+
+        url_kwargs = {
+            'zoom': ZOOM,
+            'grid_size': GRID_SIZE,
+            'dataset_id': dataset.id,
+        }
+
+        url = reverse('get_dataset_content', kwargs=url_kwargs)
+
+        response = self.client.get(url, format='json')      
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+        parsed_response = json.loads(response.content)
+        self.assertEqual(parsed_response['id'], dataset.id)
+        self.assertEqual(parsed_response['style'], dataset.style)
 
 
 class TestGetMapContentCount(WithGardens, WithFilters, APITestCase):
 
     def test_post(self):
 
         self.create_points()
```

### Comparing `anycluster-2.2.0/anycluster/api/urls.py` & `anycluster-2.3.0/anycluster/api/urls.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/api/views.py` & `anycluster-2.3.0/anycluster/api/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+from django.conf import settings
 from django.core import serializers
 
 from rest_framework.views import APIView
 from rest_framework.response import Response
 from rest_framework.renderers import JSONRenderer
 from rest_framework import status
 
-from anycluster.MapClusterer import MapClusterer
+from anycluster.MapClusterer import MapClusterer, Gis
 from anycluster.definitions import GEOMETRY_TYPE_VIEWPORT, GEOMETRY_TYPE_AREA, CLUSTER_TYPE_GRID, CLUSTER_TYPE_KMEANS
 
 from .serializers import (ClusterRequestSerializer, ClusterContentRequestSerializer, MapContentCountSerializer,
-                            GroupedMapContentSerializer)
+                            GroupedMapContentSerializer, AreaContentRequestSerializer)
 
 from anycluster import ClusterCache
+from anycluster.utils import import_module
+
+gis_serializer_path = getattr(settings, 'ANYCLUSTER_GIS_MODEL_SERIALIZER', 'anycluster.api.serializers.GisModelSerializer')
+GisModelSerializer = import_module(gis_serializer_path)
 
 import json
 
 class APIHome(APIView):
 
     def get(self, request, *args, **kwargs):
         return Response({'success':True})
@@ -60,18 +65,22 @@
     def set_cache(self, request, cluster_cache):
         cluster_cache_json = cluster_cache.serialize()
         request.session[self.cache_name] = cluster_cache_json
 
 
     def serialize_gis_model_list(self, map_clusterer, instances_list):
 
-        serializer_fields = map_clusterer.get_gis_field_names()
-        data = serializers.serialize('json', instances_list, fields=serializer_fields)
+        instances_pks = [i.pk for i in instances_list]
+
+        gis_queryset = Gis.objects.filter(pk__in=instances_pks)
+
+        serializer = GisModelSerializer(gis_queryset, many=True)
+        data = serializer.data
 
-        return json.loads(data)
+        return data
 
 
 '''
     GridCluster only supports GEOMETRY_TYPE_VIEWPORT
 '''
 class GridCluster(MapClusterViewBase, APIView):
 
@@ -172,29 +181,32 @@
 '''
     Get contents of an area or grid cluster
 '''
 class GetAreaContent(MapClusterViewBase, APIView):
 
     def post(self, request, *args, **kwargs):
 
-        serializer = ClusterRequestSerializer(data=request.data)
+        serializer = AreaContentRequestSerializer(data=request.data)
 
         if serializer.is_valid():
 
             geometry_type = serializer.validated_data['geometry_type']
             output_srid = self.parse_srid(serializer.validated_data['output_srid'])
 
+            limit = serializer.validated_data.get('limit', None)
+            offset = serializer.validated_data.get('offset', None)
+
             filters = serializer.validated_data['filters']
 
             map_clusterer = self.get_map_clusterer(geometry_type, CLUSTER_TYPE_KMEANS, filters, False, output_srid,
                 request, **kwargs)
 
             geojson = serializer.validated_data['geojson']
 
-            area_content = map_clusterer.get_area_content(geojson, filters)
+            area_content = map_clusterer.get_area_content(geojson, filters, limit, offset)
 
             data = self.serialize_gis_model_list(map_clusterer, area_content)
 
             return Response(data)
 
         return Response(serializer.errors, status=status.HTTP_400_BAD_REQUEST)
         
@@ -211,18 +223,18 @@
         map_clusterer = self.get_map_clusterer(GEOMETRY_TYPE_VIEWPORT, CLUSTER_TYPE_GRID, filters, False, output_srid,
             request, **kwargs)
 
         dataset_id = kwargs['dataset_id']
 
         dataset = map_clusterer.get_dataset_content(dataset_id)
 
-        serializer_fields = map_clusterer.get_gis_field_names()
-        data = serializers.serialize('json', dataset, fields=serializer_fields)
+        serializer = GisModelSerializer(dataset)
+        data = serializer.data
 
-        return Response(json.loads(data))
+        return Response(data)
 
 
 class GetMapContentCount(MapClusterViewBase, APIView):
 
     def post(self, request, *args, **kwargs):
 
         serializer = MapContentCountSerializer(data=request.data)
```

### Comparing `anycluster-2.2.0/anycluster/clusters.py` & `anycluster-2.3.0/anycluster/clusters.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/definitions.py` & `anycluster-2.3.0/anycluster/definitions.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/globalmaptiles.py` & `anycluster-2.3.0/anycluster/globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/10.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/10.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/100.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/100.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/1000.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/1000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/10000.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/10000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/10000_empty.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/10000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/1000_empty.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/1000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/100_empty.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/100_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/10_empty.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/10_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/5.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/5.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/50.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/50.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/50_empty.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/50_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/5_empty.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/5_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/static/anycluster/images/pin_unknown.png` & `anycluster-2.3.0/anycluster/static/anycluster/images/pin_unknown.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.3.0/anycluster/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc` & `anycluster-2.3.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc` & `anycluster-2.3.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc` & `anycluster-2.3.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc` & `anycluster-2.3.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc` & `anycluster-2.3.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/tests/common.py` & `anycluster-2.3.0/anycluster/tests/common.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/tests/mixins.py` & `anycluster-2.3.0/anycluster/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/tests/test_ClusterCache.py` & `anycluster-2.3.0/anycluster/tests/test_ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/tests/test_FilterComposer.py` & `anycluster-2.3.0/anycluster/tests/test_FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster/tests/test_MapClusterer.py` & `anycluster-2.3.0/anycluster/tests/test_MapClusterer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.2.0/anycluster.egg-info/PKG-INFO` & `anycluster-2.3.0/anycluster.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.2.0
+Version: 2.3.0
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.2.0/anycluster.egg-info/SOURCES.txt` & `anycluster-2.3.0/anycluster.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 anycluster/MapClusterer.py
 anycluster/MapTools.py
 anycluster/__init__.py
 anycluster/apps.py
 anycluster/clusters.py
 anycluster/definitions.py
 anycluster/globalmaptiles.py
+anycluster/utils.py
 anycluster.egg-info/PKG-INFO
 anycluster.egg-info/SOURCES.txt
 anycluster.egg-info/dependency_links.txt
 anycluster.egg-info/requires.txt
 anycluster.egg-info/top_level.txt
 anycluster/api/json_schemas.py
 anycluster/api/serializers.py
```

### Comparing `anycluster-2.2.0/setup.py` & `anycluster-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'psycopg2',
     'djangorestframework',
     'jsonschema',
 ]
 
 setup(
     name="anycluster",
-    version='2.2.0',
+    version='2.3.0',
     description='anycluster provides Server-Side clustering of map markers for Geodjango',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, cluster, kmeans, grid, server-side clustering',
     author='Thomas Uher',
```

