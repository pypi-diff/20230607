# Comparing `tmp/shipyard_clickup-0.1.1a0.tar.gz` & `tmp/shipyard_clickup-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_clickup-0.1.1a0.tar", max compression
+gzip compressed data, was "shipyard_clickup-0.1.1a1.tar", max compression
```

## Comparing `shipyard_clickup-0.1.1a0.tar` & `shipyard_clickup-0.1.1a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-06-06 18:57:29.881322 shipyard_clickup-0.1.1a0/README.md
--rw-r--r--   0        0        0      493 2023-06-06 20:38:38.846617 shipyard_clickup-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-06-06 19:37:34.627359 shipyard_clickup-0.1.1a0/shipyard_clickup/__init__.py
--rw-r--r--   0        0        0       59 2023-06-06 20:38:22.923524 shipyard_clickup-0.1.1a0/shipyard_clickup/cli/add_comment.py
--rw-r--r--   0        0        0        0 2023-06-06 19:35:30.786721 shipyard_clickup-0.1.1a0/shipyard_clickup/cli/create_task.py
--rw-r--r--   0        0        0        0 2023-06-06 19:35:21.397740 shipyard_clickup-0.1.1a0/shipyard_clickup/cli/edit_task.py
--rw-r--r--   0        0        0     6365 2023-06-06 18:57:29.882745 shipyard_clickup-0.1.1a0/shipyard_clickup/clickup.py
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 shipyard_clickup-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 18:57:29.881322 shipyard_clickup-0.1.1a1/README.md
+-rw-r--r--   0        0        0      497 2023-06-07 13:53:50.666465 shipyard_clickup-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-06-06 19:37:34.627359 shipyard_clickup-0.1.1a1/shipyard_clickup/__init__.py
+-rw-r--r--   0        0        0     1183 2023-06-07 13:32:49.075282 shipyard_clickup-0.1.1a1/shipyard_clickup/cli/add_comment.py
+-rw-r--r--   0        0        0     1380 2023-06-07 13:32:49.072399 shipyard_clickup-0.1.1a1/shipyard_clickup/cli/create_task.py
+-rw-r--r--   0        0        0     1380 2023-06-07 13:38:04.029507 shipyard_clickup-0.1.1a1/shipyard_clickup/cli/edit_task.py
+-rw-r--r--   0        0        0     6365 2023-06-06 18:57:29.882745 shipyard_clickup-0.1.1a1/shipyard_clickup/clickup.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 shipyard_clickup-0.1.1a1/PKG-INFO
```

### Comparing `shipyard_clickup-0.1.1a0/shipyard_clickup/clickup.py` & `shipyard_clickup-0.1.1a1/shipyard_clickup/clickup.py`

 * *Files identical despite different names*

