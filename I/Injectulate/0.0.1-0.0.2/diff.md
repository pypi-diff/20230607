# Comparing `tmp/Injectulate-0.0.1.tar.gz` & `tmp/Injectulate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Injectulate-0.0.1.tar", last modified: Mon Jun  5 22:18:46 2023, max compression
+gzip compressed data, was "Injectulate-0.0.2.tar", last modified: Wed Jun  7 05:00:36 2023, max compression
```

## Comparing `Injectulate-0.0.1.tar` & `Injectulate-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:18:46.543469 Injectulate-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:18:46.543469 Injectulate-0.0.1/Injectulate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-05 22:18:46.000000 Injectulate-0.0.1/Injectulate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 22:18:46.000000 Injectulate-0.0.1/Injectulate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 22:18:46.000000 Injectulate-0.0.1/Injectulate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 22:18:46.000000 Injectulate-0.0.1/Injectulate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 22:18:36.000000 Injectulate-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-05 22:18:46.543469 Injectulate-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 22:18:36.000000 Injectulate-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:18:46.543469 Injectulate-0.0.1/injectulate/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-05 22:18:36.000000 Injectulate-0.0.1/injectulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-05 22:18:36.000000 Injectulate-0.0.1/injectulate/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-05 22:18:36.000000 Injectulate-0.0.1/injectulate/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:18:46.543469 Injectulate-0.0.1/injectulate/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:18:36.000000 Injectulate-0.0.1/injectulate/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-05 22:18:36.000000 Injectulate-0.0.1/injectulate/test/container_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-05 22:18:36.000000 Injectulate-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 22:18:46.543469 Injectulate-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:00:36.857765 Injectulate-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:00:36.857765 Injectulate-0.0.2/Injectulate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-07 05:00:36.000000 Injectulate-0.0.2/Injectulate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-07 05:00:36.000000 Injectulate-0.0.2/Injectulate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:00:36.000000 Injectulate-0.0.2/Injectulate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 05:00:36.000000 Injectulate-0.0.2/Injectulate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-07 05:00:26.000000 Injectulate-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-07 05:00:36.857765 Injectulate-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-07 05:00:26.000000 Injectulate-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:00:36.857765 Injectulate-0.0.2/injectulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 05:00:26.000000 Injectulate-0.0.2/injectulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-07 05:00:26.000000 Injectulate-0.0.2/injectulate/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 05:00:26.000000 Injectulate-0.0.2/injectulate/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:00:36.857765 Injectulate-0.0.2/injectulate/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:00:26.000000 Injectulate-0.0.2/injectulate/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-07 05:00:26.000000 Injectulate-0.0.2/injectulate/test/container_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-07 05:00:26.000000 Injectulate-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 05:00:36.857765 Injectulate-0.0.2/setup.cfg
```

### Comparing `Injectulate-0.0.1/LICENSE` & `Injectulate-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Injectulate-0.0.1/injectulate/container.py` & `Injectulate-0.0.2/injectulate/container.py`

 * *Files identical despite different names*

### Comparing `Injectulate-0.0.1/injectulate/test/container_test.py` & `Injectulate-0.0.2/injectulate/test/container_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC
 
 from pytest import fixture, raises
 
-from ..container import Container, Builder
-from ..errors import TypeAnnotationError
+from injectulate import Builder, Container
+from injectulate.errors import TypeAnnotationError
 
 
 @fixture
 def target(builder) -> Container:
     return builder.build()
```

### Comparing `Injectulate-0.0.1/pyproject.toml` & `Injectulate-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Injectulate"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Henrik Hjalmarsson", email = "henrik.hjalmarsson.lazy@gmail.com" }
 ]
 description = "Lightweight dependency injection container."
 readme = "README.md"
 requires-python = ">=3.11"
```

