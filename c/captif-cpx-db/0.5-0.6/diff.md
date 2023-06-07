# Comparing `tmp/captif_cpx_db-0.5.tar.gz` & `tmp/captif_cpx_db-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_db-0.5.tar", max compression
+gzip compressed data, was "captif_cpx_db-0.6.tar", max compression
```

## Comparing `captif_cpx_db-0.5.tar` & `captif_cpx_db-0.6.tar`

### file list

```diff
@@ -1,10 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-05-24 02:35:39.737841 captif_cpx_db-0.5/LICENSE
--rw-r--r--   0        0        0       16 2023-05-24 02:35:39.737841 captif_cpx_db-0.5/README.md
--rw-r--r--   0        0        0      257 2023-05-24 02:35:39.737841 captif_cpx_db-0.5/captif_cpx_db/__init__.py
--rw-r--r--   0        0        0       30 2023-05-24 02:35:39.737841 captif_cpx_db-0.5/captif_cpx_db/constants.py
--rw-r--r--   0        0        0     3284 2023-05-24 02:35:39.737841 captif_cpx_db-0.5/captif_cpx_db/models/__init__.py
--rw-r--r--   0        0        0      244 2023-05-24 02:35:39.741841 captif_cpx_db-0.5/captif_cpx_db/models/sa_helpers.py
--rw-r--r--   0        0        0    11303 2023-05-24 02:35:39.741841 captif_cpx_db-0.5/captif_cpx_db/models/segment.py
--rw-r--r--   0        0        0     7437 2023-05-24 02:35:39.741841 captif_cpx_db-0.5/captif_cpx_db/models/session.py
--rw-r--r--   0        0        0      504 2023-05-24 02:35:39.741841 captif_cpx_db-0.5/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-07 04:06:38.965736 captif_cpx_db-0.6/LICENSE
+-rw-r--r--   0        0        0       16 2023-06-07 04:06:38.965736 captif_cpx_db-0.6/README.md
+-rw-r--r--   0        0        0       20 2023-06-07 04:06:38.965736 captif_cpx_db-0.6/captif_cpx_db/__init__.py
+-rw-r--r--   0        0        0    28571 2023-06-07 04:06:38.965736 captif_cpx_db-0.6/captif_cpx_db/models.py
+-rw-r--r--   0        0        0      504 2023-06-07 04:06:38.965736 captif_cpx_db-0.6/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.6/PKG-INFO
```

### Comparing `captif_cpx_db-0.5/LICENSE` & `captif_cpx_db-0.6/LICENSE`

 * *Files identical despite different names*

