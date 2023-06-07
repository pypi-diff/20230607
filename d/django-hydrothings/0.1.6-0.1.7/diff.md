# Comparing `tmp/django-hydrothings-0.1.6.tar.gz` & `tmp/django-hydrothings-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hydrothings-0.1.6.tar", last modified: Fri Jun  2 16:22:04 2023, max compression
+gzip compressed data, was "django-hydrothings-0.1.7.tar", last modified: Wed Jun  7 19:59:48 2023, max compression
```

## Comparing `django-hydrothings-0.1.6.tar` & `django-hydrothings-0.1.7.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.182488 django-hydrothings-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.186488 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:22:04.000000 django-hydrothings-0.1.6/src/django_hydrothings.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.186488 django-hydrothings-0.1.6/src/hydrothings/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.186488 django-hydrothings-0.1.6/src/hydrothings/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/odm2/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/datastreams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/datastreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/datastreams/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/datastreams/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/locations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/locations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/locations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.190488 django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/src/hydrothings/components/root/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/root/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/root/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/root/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/src/hydrothings/components/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/sensors/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/sensors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/sensors/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/src/hydrothings/components/things/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/things/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/things/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/components/things/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/src/hydrothings/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/extras/iso_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/src/hydrothings/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:22:04.194488 django-hydrothings-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_allow_partial_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_iso_interval_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_iso_time_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_metadata_field_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_resolve_chained_entity_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_sensorthings_abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-02 16:21:45.000000 django-hydrothings-0.1.6/tests/test_whitespace_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.560166 django-hydrothings-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 19:59:48.560166 django-hydrothings-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-07 19:59:48.560166 django-hydrothings-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.548166 django-hydrothings-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.552166 django-hydrothings-0.1.7/src/django_hydrothings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 19:59:48.000000 django-hydrothings-0.1.7/src/django_hydrothings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-07 19:59:48.000000 django-hydrothings-0.1.7/src/django_hydrothings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:59:48.000000 django-hydrothings-0.1.7/src/django_hydrothings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-07 19:59:48.000000 django-hydrothings-0.1.7/src/django_hydrothings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 19:59:48.000000 django-hydrothings-0.1.7/src/django_hydrothings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:59:48.000000 django-hydrothings-0.1.7/src/django_hydrothings.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.552166 django-hydrothings-0.1.7/src/hydrothings/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.552166 django-hydrothings-0.1.7/src/hydrothings/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.556166 django-hydrothings-0.1.7/src/hydrothings/backends/frostserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/frostserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/frostserver/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/frostserver/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/frostserver/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/frostserver/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.556166 django-hydrothings-0.1.7/src/hydrothings/backends/odm2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/odm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/odm2/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/odm2/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/odm2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/odm2/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/odm2/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.556166 django-hydrothings-0.1.7/src/hydrothings/backends/sensorthings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/sensorthings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/sensorthings/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/sensorthings/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/sensorthings/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/backends/sensorthings/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.556166 django-hydrothings-0.1.7/src/hydrothings/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.556166 django-hydrothings-0.1.7/src/hydrothings/components/datastreams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/datastreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/datastreams/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/datastreams/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.556166 django-hydrothings-0.1.7/src/hydrothings/components/featuresofinterest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/featuresofinterest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/featuresofinterest/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/featuresofinterest/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.556166 django-hydrothings-0.1.7/src/hydrothings/components/historicallocations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/historicallocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/historicallocations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/historicallocations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.556166 django-hydrothings-0.1.7/src/hydrothings/components/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/locations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/locations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.556166 django-hydrothings-0.1.7/src/hydrothings/components/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/observations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/observations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.560166 django-hydrothings-0.1.7/src/hydrothings/components/observedproperties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/observedproperties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/observedproperties/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/observedproperties/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.560166 django-hydrothings-0.1.7/src/hydrothings/components/root/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/root/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/root/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/root/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.560166 django-hydrothings-0.1.7/src/hydrothings/components/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/sensors/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/sensors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/sensors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.560166 django-hydrothings-0.1.7/src/hydrothings/components/things/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/things/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/things/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/components/things/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.560166 django-hydrothings-0.1.7/src/hydrothings/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/extras/iso_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/src/hydrothings/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:59:48.560166 django-hydrothings-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/tests/test_allow_partial_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/tests/test_iso_interval_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/tests/test_iso_time_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/tests/test_metadata_field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/tests/test_resolve_chained_entity_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/tests/test_sensorthings_abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-07 19:59:32.000000 django-hydrothings-0.1.7/tests/test_whitespace_validator.py
```

### Comparing `django-hydrothings-0.1.6/LICENSE.txt` & `django-hydrothings-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/README.md` & `django-hydrothings-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/django_hydrothings.egg-info/SOURCES.txt` & `django-hydrothings-0.1.7/src/django_hydrothings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/backends/frostserver/engine.py` & `django-hydrothings-0.1.7/src/hydrothings/backends/frostserver/engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/backends/odm2/engine.py` & `django-hydrothings-0.1.7/src/hydrothings/backends/odm2/engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/backends/sensorthings/engine.py` & `django-hydrothings-0.1.7/src/hydrothings/backends/sensorthings/engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/__init__.py` & `django-hydrothings-0.1.7/src/hydrothings/components/__init__.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/datastreams/schemas.py` & `django-hydrothings-0.1.7/src/hydrothings/components/datastreams/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/datastreams/views.py` & `django-hydrothings-0.1.7/src/hydrothings/components/datastreams/views.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/schemas.py` & `django-hydrothings-0.1.7/src/hydrothings/components/featuresofinterest/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/featuresofinterest/views.py` & `django-hydrothings-0.1.7/src/hydrothings/components/featuresofinterest/views.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/schemas.py` & `django-hydrothings-0.1.7/src/hydrothings/components/historicallocations/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/historicallocations/views.py` & `django-hydrothings-0.1.7/src/hydrothings/components/historicallocations/views.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/locations/schemas.py` & `django-hydrothings-0.1.7/src/hydrothings/components/locations/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/locations/views.py` & `django-hydrothings-0.1.7/src/hydrothings/components/locations/views.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/observations/schemas.py` & `django-hydrothings-0.1.7/src/hydrothings/components/observations/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/observations/utils.py` & `django-hydrothings-0.1.7/src/hydrothings/components/observations/utils.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/observations/views.py` & `django-hydrothings-0.1.7/src/hydrothings/components/observations/views.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/schemas.py` & `django-hydrothings-0.1.7/src/hydrothings/components/observedproperties/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/observedproperties/views.py` & `django-hydrothings-0.1.7/src/hydrothings/components/observedproperties/views.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/root/views.py` & `django-hydrothings-0.1.7/src/hydrothings/components/root/views.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/sensors/schemas.py` & `django-hydrothings-0.1.7/src/hydrothings/components/sensors/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/sensors/utils.py` & `django-hydrothings-0.1.7/src/hydrothings/components/sensors/utils.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/sensors/views.py` & `django-hydrothings-0.1.7/src/hydrothings/components/sensors/views.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/things/schemas.py` & `django-hydrothings-0.1.7/src/hydrothings/components/things/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/components/things/views.py` & `django-hydrothings-0.1.7/src/hydrothings/components/things/views.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/engine.py` & `django-hydrothings-0.1.7/src/hydrothings/engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/extras/iso_types.py` & `django-hydrothings-0.1.7/src/hydrothings/extras/iso_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import pytz
 from dateutil.parser import isoparse
 
 
 class ISOTime(str):
 
+    def __datetime__(self):
+        return isoparse(self)
+
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         if not isinstance(v, str):
```

### Comparing `django-hydrothings-0.1.6/src/hydrothings/main.py` & `django-hydrothings-0.1.7/src/hydrothings/main.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/middleware.py` & `django-hydrothings-0.1.7/src/hydrothings/middleware.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/schemas.py` & `django-hydrothings-0.1.7/src/hydrothings/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/settings.py` & `django-hydrothings-0.1.7/src/hydrothings/settings.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/utils.py` & `django-hydrothings-0.1.7/src/hydrothings/utils.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/src/hydrothings/validators.py` & `django-hydrothings-0.1.7/src/hydrothings/validators.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/tests/test_allow_partial_decorator.py` & `django-hydrothings-0.1.7/tests/test_allow_partial_decorator.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/tests/test_iso_interval_type.py` & `django-hydrothings-0.1.7/tests/test_iso_interval_type.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/tests/test_iso_time_type.py` & `django-hydrothings-0.1.7/tests/test_iso_time_type.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/tests/test_metadata_field_validator.py` & `django-hydrothings-0.1.7/tests/test_metadata_field_validator.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/tests/test_resolve_chained_entity_url.py` & `django-hydrothings-0.1.7/tests/test_resolve_chained_entity_url.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/tests/test_sensorthings_abstract_engine.py` & `django-hydrothings-0.1.7/tests/test_sensorthings_abstract_engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.6/tests/test_whitespace_validator.py` & `django-hydrothings-0.1.7/tests/test_whitespace_validator.py`

 * *Files identical despite different names*

