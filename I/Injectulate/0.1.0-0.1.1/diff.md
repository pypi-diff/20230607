# Comparing `tmp/Injectulate-0.1.0.tar.gz` & `tmp/Injectulate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Injectulate-0.1.0.tar", last modified: Wed Jun  7 18:57:34 2023, max compression
+gzip compressed data, was "Injectulate-0.1.1.tar", last modified: Wed Jun  7 19:26:27 2023, max compression
```

## Comparing `Injectulate-0.1.0.tar` & `Injectulate-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:57:34.942634 Injectulate-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:57:34.942634 Injectulate-0.1.0/Injectulate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-07 18:57:34.000000 Injectulate-0.1.0/Injectulate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-07 18:57:34.000000 Injectulate-0.1.0/Injectulate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:57:34.000000 Injectulate-0.1.0/Injectulate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 18:57:34.000000 Injectulate-0.1.0/Injectulate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-07 18:57:23.000000 Injectulate-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-07 18:57:34.942634 Injectulate-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-07 18:57:23.000000 Injectulate-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:57:34.942634 Injectulate-0.1.0/injectulate/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 18:57:23.000000 Injectulate-0.1.0/injectulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-07 18:57:23.000000 Injectulate-0.1.0/injectulate/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 18:57:23.000000 Injectulate-0.1.0/injectulate/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:57:34.942634 Injectulate-0.1.0/injectulate/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:57:23.000000 Injectulate-0.1.0/injectulate/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-07 18:57:23.000000 Injectulate-0.1.0/injectulate/test/container_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-07 18:57:23.000000 Injectulate-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:57:34.942634 Injectulate-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:26:27.915418 Injectulate-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:26:27.915418 Injectulate-0.1.1/Injectulate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42714 2023-06-07 19:26:27.000000 Injectulate-0.1.1/Injectulate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-07 19:26:27.000000 Injectulate-0.1.1/Injectulate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:26:27.000000 Injectulate-0.1.1/Injectulate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 19:26:27.000000 Injectulate-0.1.1/Injectulate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-07 19:26:18.000000 Injectulate-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42714 2023-06-07 19:26:27.915418 Injectulate-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-07 19:26:18.000000 Injectulate-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:26:27.915418 Injectulate-0.1.1/injectulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 19:26:18.000000 Injectulate-0.1.1/injectulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-07 19:26:18.000000 Injectulate-0.1.1/injectulate/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 19:26:18.000000 Injectulate-0.1.1/injectulate/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:26:27.915418 Injectulate-0.1.1/injectulate/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:26:18.000000 Injectulate-0.1.1/injectulate/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-07 19:26:18.000000 Injectulate-0.1.1/injectulate/test/container_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-07 19:26:18.000000 Injectulate-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:26:27.915418 Injectulate-0.1.1/setup.cfg
```

### Comparing `Injectulate-0.1.0/Injectulate.egg-info/PKG-INFO` & `Injectulate-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: Injectulate
-Version: 0.1.0
-Summary: Lightweight dependency injection container.
-Author-email: Henrik Hjalmarsson <henrik.hjalmarsson.lazy@gmail.com>
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Injectulate
 Lightweight dependency injection framework relying on type annotations for dependency resolution.
 
 ## Installation
 `pip install injectulate`
 
 ## Usage
@@ -91,8 +82,8 @@
 builder.bind(AbstractClass).to(lambda c: Implementation(c))
 container = builder.build()
 
 impl = container.get(AbstractClass)
 ```
 
 ### Suggestions
-Are welcomed
+Are welcomed
```

### Comparing `Injectulate-0.1.0/LICENSE` & `Injectulate-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Injectulate-0.1.0/injectulate/container.py` & `Injectulate-0.1.1/injectulate/container.py`

 * *Files identical despite different names*

### Comparing `Injectulate-0.1.0/injectulate/test/container_test.py` & `Injectulate-0.1.1/injectulate/test/container_test.py`

 * *Files identical despite different names*

### Comparing `Injectulate-0.1.0/pyproject.toml` & `Injectulate-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,27 @@
 name = "Injectulate"
 dynamic = ["version"]
 authors = [
     { name = "Henrik Hjalmarsson", email = "henrik.hjalmarsson.lazy@gmail.com" }
 ]
 description = "Lightweight dependency injection container."
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
+license = {file = "LICENSE"}
+keywords = ["DI", "Dependency Injection", "IoC", "Injection", "Lightweight", "Type annotation"]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Natural Language :: English",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: Utilities",
+    "Typing :: Typed",
+]
 
 [build-system]
 requires = ["setuptools>=67", "wheel", "setuptools-git-versioning>=1.13.3"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools-git-versioning]
 enabled = true
```

