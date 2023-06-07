# Comparing `tmp/django-logpipe-1.2.0.tar.gz` & `tmp/django-logpipe-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-logpipe-1.2.0.tar", last modified: Wed Mar 15 16:59:31 2023, max compression
+gzip compressed data, was "django-logpipe-1.3.0.tar", last modified: Wed Jun  7 19:47:59 2023, max compression
```

## Comparing `django-logpipe-1.2.0.tar` & `django-logpipe-1.3.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.816942 django-logpipe-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12920 2023-03-15 16:59:31.816942 django-logpipe-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12052 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-03-15 16:59:31.817942 django-logpipe-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1913 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.794939 django-logpipe-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.802940 django-logpipe-1.2.0/src/django_logpipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12920 2023-03-15 16:59:31.000000 django-logpipe-1.2.0/src/django_logpipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1892 2023-03-15 16:59:31.000000 django-logpipe-1.2.0/src/django_logpipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 16:59:31.000000 django-logpipe-1.2.0/src/django_logpipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-03-15 16:59:31.000000 django-logpipe-1.2.0/src/django_logpipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-15 16:59:31.000000 django-logpipe-1.2.0/src/django_logpipe.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.806941 django-logpipe-1.2.0/src/logpipe/
--rw-rw-rw-   0 root         (0) root         (0)     1339 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.807941 django-logpipe-1.2.0/src/logpipe/backend/
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/backend/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4724 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/backend/kafka.py
--rw-rw-rw-   0 root         (0) root         (0)     9610 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/backend/kinesis.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/config.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     7194 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1028 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/format.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.808941 django-logpipe-1.2.0/src/logpipe/formats/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/formats/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/formats/json.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/formats/msgpack.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/formats/pickle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.796940 django-logpipe-1.2.0/src/logpipe/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.796940 django-logpipe-1.2.0/src/logpipe/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.809941 django-logpipe-1.2.0/src/logpipe/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2742 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     4806 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.809941 django-logpipe-1.2.0/src/logpipe/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.809941 django-logpipe-1.2.0/src/logpipe/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/management/commands/run_kafka_consumer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.812941 django-logpipe-1.2.0/src/logpipe/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/migrations/0002_auto_20170427_1451.py
--rw-rw-rw-   0 root         (0) root         (0)     2240 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/migrations/0003_auto_20170427_1703.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/migrations/0004_auto_20170502_1403.py
--rw-rw-rw-   0 root         (0) root         (0)     1818 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/migrations/0005_auto_20180917_1348.py
--rw-rw-rw-   0 root         (0) root         (0)     4042 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/migrations/0006_alter_kafkaoffset_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4509 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/producer.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/registry.py
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.812941 django-logpipe-1.2.0/src/logpipe/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.813941 django-logpipe-1.2.0/src/logpipe/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/integration/test_roundtrip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.814941 django-logpipe-1.2.0/src/logpipe/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.815941 django-logpipe-1.2.0/src/logpipe/tests/unit/kafka/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/unit/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8703 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/unit/kafka/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)     3527 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/unit/kafka/test_producer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:59:31.816942 django-logpipe-1.2.0/src/logpipe/tests/unit/kinesis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/unit/kinesis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7892 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/unit/kinesis/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)     4458 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/unit/kinesis/test_producer.py
--rw-rw-rw-   0 root         (0) root         (0)     2373 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/unit/test_format.py
--rw-rw-rw-   0 root         (0) root         (0)     1602 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/unit/test_producer.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2023-03-15 16:59:20.000000 django-logpipe-1.2.0/src/logpipe/tests/unit/test_settings.py
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-15 16:59:31.000000 django-logpipe-1.2.0/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.533027 django-logpipe-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13203 2023-06-07 19:47:59.533027 django-logpipe-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12335 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-07 19:47:59.533027 django-logpipe-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1913 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.524777 django-logpipe-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.526610 django-logpipe-1.3.0/src/django_logpipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13203 2023-06-07 19:47:59.000000 django-logpipe-1.3.0/src/django_logpipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-07 19:47:59.000000 django-logpipe-1.3.0/src/django_logpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 19:47:59.000000 django-logpipe-1.3.0/src/django_logpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-06-07 19:47:59.000000 django-logpipe-1.3.0/src/django_logpipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-07 19:47:59.000000 django-logpipe-1.3.0/src/django_logpipe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.527527 django-logpipe-1.3.0/src/logpipe/
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.528443 django-logpipe-1.3.0/src/logpipe/backend/
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/backend/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4724 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/backend/kafka.py
+-rw-rw-rw-   0 root         (0) root         (0)     9610 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/backend/kinesis.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/config.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     7194 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/format.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.528443 django-logpipe-1.3.0/src/logpipe/formats/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/formats/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/formats/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/formats/msgpack.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/formats/pickle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.524777 django-logpipe-1.3.0/src/logpipe/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.524777 django-logpipe-1.3.0/src/logpipe/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.529360 django-logpipe-1.3.0/src/logpipe/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2742 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     4806 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.529360 django-logpipe-1.3.0/src/logpipe/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.529360 django-logpipe-1.3.0/src/logpipe/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/management/commands/run_kafka_consumer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.531193 django-logpipe-1.3.0/src/logpipe/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/migrations/0002_auto_20170427_1451.py
+-rw-rw-rw-   0 root         (0) root         (0)     2240 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/migrations/0003_auto_20170427_1703.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/migrations/0004_auto_20170502_1403.py
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/migrations/0005_auto_20180917_1348.py
+-rw-rw-rw-   0 root         (0) root         (0)     4042 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/migrations/0006_alter_kafkaoffset_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4509 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/producer.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.531193 django-logpipe-1.3.0/src/logpipe/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.531193 django-logpipe-1.3.0/src/logpipe/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/integration/test_roundtrip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.532110 django-logpipe-1.3.0/src/logpipe/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.532110 django-logpipe-1.3.0/src/logpipe/tests/unit/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/unit/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8703 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/unit/kafka/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3527 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/unit/kafka/test_producer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 19:47:59.532110 django-logpipe-1.3.0/src/logpipe/tests/unit/kinesis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/unit/kinesis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7892 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/unit/kinesis/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4458 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/unit/kinesis/test_producer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/unit/test_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/unit/test_producer.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2023-06-07 19:47:50.000000 django-logpipe-1.3.0/src/logpipe/tests/unit/test_settings.py
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-07 19:47:59.000000 django-logpipe-1.3.0/version.txt
```

### Comparing `django-logpipe-1.2.0/LICENSE` & `django-logpipe-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/PKG-INFO` & `django-logpipe-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logpipe
-Version: 1.2.0
+Version: 1.3.0
 Summary: Move data around between Python services using Kafka and/or AWS Kinesis and Django Rest Framework serializers.
 Home-page: https://gitlab.com/thelabnyc/django-logpipe
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -73,14 +73,15 @@
         },
 
         # Optional Settings
         # 'KAFKA_SEND_TIMEOUT': 10,
         # 'KAFKA_MAX_SEND_RETRIES': 0,
         # 'MIN_MESSAGE_LAG_MS': 0,
         # 'DEFAULT_FORMAT': 'json',
+        # 'PRODUCER_ID': 'my-application-name',
     }
 
 If you're using AWS Kinesis instead of Kafka, it will look like this:
 
 ::
 
     LOGPIPE = {
@@ -91,14 +92,15 @@
 
         # Optional Settings
         # 'KINESIS_REGION': 'us-east-1',
         # 'KINESIS_FETCH_LIMIT': 25,
         # 'KINESIS_SEQ_NUM_CACHE_SIZE': 1000,
         # 'MIN_MESSAGE_LAG_MS': 0,
         # 'DEFAULT_FORMAT': 'json',
+        # 'PRODUCER_ID': 'my-application-name',
     }
 
 Run migrations. This will create the model used to store Kafka log position offsets.::
 
     $ python manage.py migrate logpipe
 
 Usage
@@ -157,15 +159,15 @@
     producer = Producer('people', PersonSerializer)
     producer.send(joe)
 
 The above sample code would result in the following message being sent to the Kafka topic named `people`.
 
 ::
 
-    json:{"type":"person","version":1,"message":{"first_name":"Joe","last_name":"Schmoe","uuid":"xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx"}}
+    json:{"type":"person","version":1,"producer":"my-application-name","message":{"first_name":"Joe","last_name":"Schmoe","uuid":"xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx"}}
 
 
 Receiving Messages
 ------------------
 
 To processing incoming messages, we can reuse the same model and serializer. We just need to instantiate a Consumer object.
 
@@ -287,14 +289,18 @@
 
 Finally, after all the old version 1 messages have been dropped (by log compaction), the `PersonSerializerV1` class can be removed form the code base.
 
 
 Changelog
 =========
 
+1.3.0
+------------------
+- Add PRODUCER_ID setting to aid in debugging which systems sent which messages, especially when interrogating logged messages.
+
 1.2.0
 ------------------
 - Add Python 3.10 and 3.11 to test suite.
 - Add Django 4.0 and 4.1 to test suite.
 - Drop Python 3.8 from test suite.
 - Drop Django 2.2, 3.0, and 3.1 from test suite.
 - Added missing DB migrations (though no actual DB changes exist).
```

### Comparing `django-logpipe-1.2.0/README.rst` & `django-logpipe-1.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         },
 
         # Optional Settings
         # 'KAFKA_SEND_TIMEOUT': 10,
         # 'KAFKA_MAX_SEND_RETRIES': 0,
         # 'MIN_MESSAGE_LAG_MS': 0,
         # 'DEFAULT_FORMAT': 'json',
+        # 'PRODUCER_ID': 'my-application-name',
     }
 
 If you're using AWS Kinesis instead of Kafka, it will look like this:
 
 ::
 
     LOGPIPE = {
@@ -67,14 +68,15 @@
 
         # Optional Settings
         # 'KINESIS_REGION': 'us-east-1',
         # 'KINESIS_FETCH_LIMIT': 25,
         # 'KINESIS_SEQ_NUM_CACHE_SIZE': 1000,
         # 'MIN_MESSAGE_LAG_MS': 0,
         # 'DEFAULT_FORMAT': 'json',
+        # 'PRODUCER_ID': 'my-application-name',
     }
 
 Run migrations. This will create the model used to store Kafka log position offsets.::
 
     $ python manage.py migrate logpipe
 
 Usage
@@ -133,15 +135,15 @@
     producer = Producer('people', PersonSerializer)
     producer.send(joe)
 
 The above sample code would result in the following message being sent to the Kafka topic named `people`.
 
 ::
 
-    json:{"type":"person","version":1,"message":{"first_name":"Joe","last_name":"Schmoe","uuid":"xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx"}}
+    json:{"type":"person","version":1,"producer":"my-application-name","message":{"first_name":"Joe","last_name":"Schmoe","uuid":"xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx"}}
 
 
 Receiving Messages
 ------------------
 
 To processing incoming messages, we can reuse the same model and serializer. We just need to instantiate a Consumer object.
 
@@ -263,14 +265,18 @@
 
 Finally, after all the old version 1 messages have been dropped (by log compaction), the `PersonSerializerV1` class can be removed form the code base.
 
 
 Changelog
 =========
 
+1.3.0
+------------------
+- Add PRODUCER_ID setting to aid in debugging which systems sent which messages, especially when interrogating logged messages.
+
 1.2.0
 ------------------
 - Add Python 3.10 and 3.11 to test suite.
 - Add Django 4.0 and 4.1 to test suite.
 - Drop Python 3.8 from test suite.
 - Drop Django 2.2, 3.0, and 3.1 from test suite.
 - Added missing DB migrations (though no actual DB changes exist).
```

### Comparing `django-logpipe-1.2.0/requirements.txt` & `django-logpipe-1.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/setup.py` & `django-logpipe-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/django_logpipe.egg-info/PKG-INFO` & `django-logpipe-1.3.0/src/django_logpipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logpipe
-Version: 1.2.0
+Version: 1.3.0
 Summary: Move data around between Python services using Kafka and/or AWS Kinesis and Django Rest Framework serializers.
 Home-page: https://gitlab.com/thelabnyc/django-logpipe
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -73,14 +73,15 @@
         },
 
         # Optional Settings
         # 'KAFKA_SEND_TIMEOUT': 10,
         # 'KAFKA_MAX_SEND_RETRIES': 0,
         # 'MIN_MESSAGE_LAG_MS': 0,
         # 'DEFAULT_FORMAT': 'json',
+        # 'PRODUCER_ID': 'my-application-name',
     }
 
 If you're using AWS Kinesis instead of Kafka, it will look like this:
 
 ::
 
     LOGPIPE = {
@@ -91,14 +92,15 @@
 
         # Optional Settings
         # 'KINESIS_REGION': 'us-east-1',
         # 'KINESIS_FETCH_LIMIT': 25,
         # 'KINESIS_SEQ_NUM_CACHE_SIZE': 1000,
         # 'MIN_MESSAGE_LAG_MS': 0,
         # 'DEFAULT_FORMAT': 'json',
+        # 'PRODUCER_ID': 'my-application-name',
     }
 
 Run migrations. This will create the model used to store Kafka log position offsets.::
 
     $ python manage.py migrate logpipe
 
 Usage
@@ -157,15 +159,15 @@
     producer = Producer('people', PersonSerializer)
     producer.send(joe)
 
 The above sample code would result in the following message being sent to the Kafka topic named `people`.
 
 ::
 
-    json:{"type":"person","version":1,"message":{"first_name":"Joe","last_name":"Schmoe","uuid":"xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx"}}
+    json:{"type":"person","version":1,"producer":"my-application-name","message":{"first_name":"Joe","last_name":"Schmoe","uuid":"xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx"}}
 
 
 Receiving Messages
 ------------------
 
 To processing incoming messages, we can reuse the same model and serializer. We just need to instantiate a Consumer object.
 
@@ -287,14 +289,18 @@
 
 Finally, after all the old version 1 messages have been dropped (by log compaction), the `PersonSerializerV1` class can be removed form the code base.
 
 
 Changelog
 =========
 
+1.3.0
+------------------
+- Add PRODUCER_ID setting to aid in debugging which systems sent which messages, especially when interrogating logged messages.
+
 1.2.0
 ------------------
 - Add Python 3.10 and 3.11 to test suite.
 - Add Django 4.0 and 4.1 to test suite.
 - Drop Python 3.8 from test suite.
 - Drop Django 2.2, 3.0, and 3.1 from test suite.
 - Added missing DB migrations (though no actual DB changes exist).
```

### Comparing `django-logpipe-1.2.0/src/django_logpipe.egg-info/SOURCES.txt` & `django-logpipe-1.3.0/src/django_logpipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/__init__.py` & `django-logpipe-1.3.0/src/logpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/admin.py` & `django-logpipe-1.3.0/src/logpipe/admin.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/backend/__init__.py` & `django-logpipe-1.3.0/src/logpipe/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/backend/kafka.py` & `django-logpipe-1.3.0/src/logpipe/backend/kafka.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/backend/kinesis.py` & `django-logpipe-1.3.0/src/logpipe/backend/kinesis.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/consumer.py` & `django-logpipe-1.3.0/src/logpipe/consumer.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/format.py` & `django-logpipe-1.3.0/src/logpipe/format.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/formats/msgpack.py` & `django-logpipe-1.3.0/src/logpipe/formats/msgpack.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/formats/pickle.py` & `django-logpipe-1.3.0/src/logpipe/formats/pickle.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/locale/es/LC_MESSAGES/django.mo` & `django-logpipe-1.3.0/src/logpipe/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/locale/es/LC_MESSAGES/django.po` & `django-logpipe-1.3.0/src/logpipe/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/migrations/0001_initial.py` & `django-logpipe-1.3.0/src/logpipe/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/migrations/0003_auto_20170427_1703.py` & `django-logpipe-1.3.0/src/logpipe/migrations/0003_auto_20170427_1703.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/migrations/0004_auto_20170502_1403.py` & `django-logpipe-1.3.0/src/logpipe/migrations/0004_auto_20170502_1403.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/migrations/0005_auto_20180917_1348.py` & `django-logpipe-1.3.0/src/logpipe/migrations/0005_auto_20180917_1348.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/migrations/0006_alter_kafkaoffset_options_and_more.py` & `django-logpipe-1.3.0/src/logpipe/migrations/0006_alter_kafkaoffset_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/models.py` & `django-logpipe-1.3.0/src/logpipe/models.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/producer.py` & `django-logpipe-1.3.0/src/logpipe/producer.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Producer(object):
     _client = None
 
-    def __init__(self, topic_name, serializer_class):
+    def __init__(self, topic_name, serializer_class, producer_id=None):
         self.client = get_producer_backend()
         self.topic_name = topic_name
         self.serializer_class = serializer_class
+        self.producer_id = producer_id
+        if not self.producer_id:
+            self.producer_id = settings.get("PRODUCER_ID", "")
 
     def send(self, instance, renderer=None):
         # Instantiate the serialize
         ser = self.serializer_class(instance=instance)
 
         # Get the message type and version
         message_type = self.serializer_class.MESSAGE_TYPE
@@ -33,14 +36,16 @@
         # Render everything into a string
         renderer = settings.get("DEFAULT_FORMAT", FORMAT_JSON)
         body = {
             "type": message_type,
             "version": version,
             "message": ser.data,
         }
+        if self.producer_id:
+            body["producer"] = self.producer_id
         serialized_data = render(renderer, body)
 
         # Send the message data into the backend
         record_metadata = self.client.send(
             self.topic_name, key=key, value=serialized_data
         )
         logger.debug(
```

### Comparing `django-logpipe-1.2.0/src/logpipe/settings.py` & `django-logpipe-1.3.0/src/logpipe/settings.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/tests/common.py` & `django-logpipe-1.3.0/src/logpipe/tests/common.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/tests/integration/test_roundtrip.py` & `django-logpipe-1.3.0/src/logpipe/tests/integration/test_roundtrip.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/tests/unit/kafka/test_consumer.py` & `django-logpipe-1.3.0/src/logpipe/tests/unit/kafka/test_consumer.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/tests/unit/kafka/test_producer.py` & `django-logpipe-1.3.0/src/logpipe/tests/unit/kafka/test_producer.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/tests/unit/kinesis/test_consumer.py` & `django-logpipe-1.3.0/src/logpipe/tests/unit/kinesis/test_consumer.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/tests/unit/kinesis/test_producer.py` & `django-logpipe-1.3.0/src/logpipe/tests/unit/kinesis/test_producer.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/tests/unit/test_format.py` & `django-logpipe-1.3.0/src/logpipe/tests/unit/test_format.py`

 * *Files identical despite different names*

### Comparing `django-logpipe-1.2.0/src/logpipe/tests/unit/test_settings.py` & `django-logpipe-1.3.0/src/logpipe/tests/unit/test_settings.py`

 * *Files identical despite different names*

