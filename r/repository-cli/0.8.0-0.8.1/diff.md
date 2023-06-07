# Comparing `tmp/repository-cli-0.8.0.tar.gz` & `tmp/repository-cli-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repository-cli-0.8.0.tar", last modified: Thu Jun  1 10:48:17 2023, max compression
+gzip compressed data, was "repository-cli-0.8.1.tar", last modified: Wed Jun  7 09:23:18 2023, max compression
```

## Comparing `repository-cli-0.8.0.tar` & `repository-cli-0.8.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.629273 repository-cli-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 10:48:11.000000 repository-cli-0.8.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.625273 repository-cli-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.625273 repository-cli-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-01 10:48:11.000000 repository-cli-0.8.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 10:48:11.000000 repository-cli-0.8.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 10:48:11.000000 repository-cli-0.8.0/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 10:48:11.000000 repository-cli-0.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-01 10:48:11.000000 repository-cli-0.8.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-01 10:48:11.000000 repository-cli-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-01 10:48:11.000000 repository-cli-0.8.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-01 10:48:11.000000 repository-cli-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 10:48:11.000000 repository-cli-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-01 10:48:17.629273 repository-cli-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-01 10:48:11.000000 repository-cli-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.625273 repository-cli-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-01 10:48:11.000000 repository-cli-0.8.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.629273 repository-cli-0.8.0/repository_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/click_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/click_param_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    20795 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/records.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-01 10:48:11.000000 repository-cli-0.8.0/repository_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.629273 repository-cli-0.8.0/repository_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 10:48:17.000000 repository-cli-0.8.0/repository_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-01 10:48:11.000000 repository-cli-0.8.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-06-01 10:48:11.000000 repository-cli-0.8.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-01 10:48:17.629273 repository-cli-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 10:48:11.000000 repository-cli-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:48:17.629273 repository-cli-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-01 10:48:11.000000 repository-cli-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-01 10:48:11.000000 repository-cli-0.8.0/tests/test_rdmrecords.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-01 10:48:11.000000 repository-cli-0.8.0/tests/test_rdmrecords_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-01 10:48:11.000000 repository-cli-0.8.0/tests/test_rdmrecords_pids.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-01 10:48:11.000000 repository-cli-0.8.0/tests/test_repository_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.364529 repository-cli-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 09:23:12.000000 repository-cli-0.8.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.360529 repository-cli-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.360529 repository-cli-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-07 09:23:12.000000 repository-cli-0.8.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-07 09:23:12.000000 repository-cli-0.8.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-07 09:23:12.000000 repository-cli-0.8.1/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-07 09:23:12.000000 repository-cli-0.8.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-07 09:23:12.000000 repository-cli-0.8.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-07 09:23:12.000000 repository-cli-0.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-07 09:23:12.000000 repository-cli-0.8.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-07 09:23:12.000000 repository-cli-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 09:23:12.000000 repository-cli-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-07 09:23:18.364529 repository-cli-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-07 09:23:12.000000 repository-cli-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.364529 repository-cli-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.364529 repository-cli-0.8.1/repository_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/click_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/click_param_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19389 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.364529 repository-cli-0.8.1/repository_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-07 09:23:12.000000 repository-cli-0.8.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-06-07 09:23:12.000000 repository-cli-0.8.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-07 09:23:18.364529 repository-cli-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-07 09:23:12.000000 repository-cli-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.364529 repository-cli-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-07 09:23:12.000000 repository-cli-0.8.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-07 09:23:12.000000 repository-cli-0.8.1/tests/test_rdmrecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-07 09:23:12.000000 repository-cli-0.8.1/tests/test_rdmrecords_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-07 09:23:12.000000 repository-cli-0.8.1/tests/test_rdmrecords_pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-07 09:23:12.000000 repository-cli-0.8.1/tests/test_repository_cli.py
```

### Comparing `repository-cli-0.8.0/.github/workflows/tests.yml` & `repository-cli-0.8.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/CHANGES.rst` & `repository-cli-0.8.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.1 (release 2023-06-07)
+
+- refactor: move json validation into JSON
+- refactor: get_record_or_draft
+
+
 Version v0.8.0 (release 2023-06-01)
 
 - records: make arguments ready for drafts too
 - records: add argument delete-file
 
 
 Version v0.7.0 (release 2023-05-30)
```

### Comparing `repository-cli-0.8.0/CONTRIBUTING.rst` & `repository-cli-0.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/LICENSE` & `repository-cli-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/MANIFEST.in` & `repository-cli-0.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/PKG-INFO` & `repository-cli-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-cli
-Version: 0.8.0
+Version: 0.8.1
 Summary: "CLI utilities for TU Graz Repository."
 Home-page: https://github.com/inveniosoftware/repository-cli
 Author: Graz University of Technology
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio repository cli
 Platform: any
@@ -52,14 +52,20 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.1 (release 2023-06-07)
+
+- refactor: move json validation into JSON
+- refactor: get_record_or_draft
+
+
 Version v0.8.0 (release 2023-06-01)
 
 - records: make arguments ready for drafts too
 - records: add argument delete-file
 
 
 Version v0.7.0 (release 2023-05-30)
```

### Comparing `repository-cli-0.8.0/README.rst` & `repository-cli-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/docs/Makefile` & `repository-cli-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/docs/api.rst` & `repository-cli-0.8.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/docs/conf.py` & `repository-cli-0.8.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,8 +338,9 @@
     ("py:class", "sqlalchemy.orm.decl_api.Model"),
     ("py:class", "flask.app.Flask"),
     ("py:class", "RecordService"),
     ("py:class", "Identity"),
     ("py:class", "Draft"),
     ("py:class", "db.Model"),
     ("py:class", "Record"),
+    ("py:class", "RecordItem"),
 ]
```

### Comparing `repository-cli-0.8.0/docs/index.rst` & `repository-cli-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/docs/make.bat` & `repository-cli-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/repository_cli/cli.py` & `repository-cli-0.8.1/repository_cli/cli.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/repository_cli/click_options.py` & `repository-cli-0.8.1/repository_cli/click_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 
 from collections.abc import Callable
 from typing import Any, TypeVar
 
 from click import BOOL, STRING, Choice, File, option
 
+from .click_param_types import JSON
+
 T = TypeVar("T")
 
 
 def optional_brackets(func: Callable) -> Callable:
     """With this decorator it is possible to write decorators without ()."""
 
     def wrapper(*args: dict, **kwargs: dict) -> Any:  # noqa: ANN401
@@ -78,14 +80,15 @@
 
     Sample use: --identifier '{ "identifier": "10.48436/fcze8-4vx33", "scheme": "doi"}'
     """
     return option(
         "--identifier",
         "-i",
         required=required,
+        type=JSON(validate=["identifier", "scheme"]),
         help="metadata identifier as JSON",
     )
 
 
 # TODO. rename to option_pid
 @optional_brackets
 def option_pid_identifier(
@@ -95,14 +98,15 @@
 
     Sample use: --pid-identifier '{"doi": {"identifier": "10.48436/fcze8-4vx33",
                                            "provider": "unmanaged"}}'
     """
     return option(
         "--pid-identifier",
         required=required,
+        type=JSON(),
         help="pid identifier as JSON",
     )
 
 
 # TODO: rename to option_id, refactore to true concept of the used id
 @optional_brackets
 def option_pid(
```

### Comparing `repository-cli-0.8.0/repository_cli/ext.py` & `repository-cli-0.8.1/repository_cli/ext.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/repository_cli/records.py` & `repository-cli-0.8.1/repository_cli/records.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from pathlib import Path
 from typing import TextIO
 
 import jq
 from click import STRING, Choice, File, group, option, secho
 from flask.cli import with_appcontext
 from invenio_db import db
-from invenio_pidstore.errors import PIDDoesNotExistError
 
 from .click_options import (
     option_data_model,
     option_identifier,
     option_input_file,
     option_jq_filter,
     option_output_file,
@@ -30,14 +29,15 @@
     option_record_type,
 )
 from .click_param_types import JSON
 from .types import Color
 from .utils import (
     add_metadata_to_marc21_record,
     exists_record,
+    get_data,
     get_draft,
     get_identity,
     get_metadata_model,
     get_record_or_draft,
     get_records_service,
     update_record,
 )
@@ -150,15 +150,15 @@
         pid = record["id"]
         secho(f"\n'{pid}', trying to update", fg=Color.warning)
 
         if not exists_record(service, pid, identity):
             secho(f"'{pid}', does not exist or is deleted", fg=Color.error)
             continue
 
-        old_data = service.read(id_=pid, identity=identity).data
+        old_data = get_data(service, pid, identity)
 
         try:
             update_record(service, pid, identity, record, old_data)
         except Exception as error:
             secho(f"'{pid}', problem during update, {error}", fg=Color.error)
             continue
 
@@ -191,15 +191,15 @@
 
     for record in records:
         pid = record["id"]
 
         secho(f"\n'{pid}', trying to update", fg=Color.warning)
 
         try:
-            old_data = get_record_or_draft(service, pid, identity)
+            old_data = get_data(service, pid, identity)
         except RuntimeError as error:
             secho(str(error), fg=Color.error)
             continue
 
         if data_model == "marc21":
             new_data = add_metadata_to_marc21_record(deepcopy(old_data), record)
         else:
@@ -299,41 +299,34 @@
 @option_pid_identifier
 @with_appcontext
 def replace_pid(pid: str, pid_identifier: str) -> None:
     """Update pid doi to unmanaged.
 
     example call:
         invenio repository records pids replace -p "fcze8-4vx33"
-        --pid-identifier ' { "doi": {
-        "identifier": "10.48436/fcze8-4vx33", "provider": "unmanaged" }}'
+        --pid-identifier '{"doi": {
+        "identifier": "10.48436/fcze8-4vx33", "provider": "unmanaged"}}'
     """
-    try:
-        pid_identifier_json = json.loads(pid_identifier)
-    except Exception as error:
-        secho(str(error), fg=Color.error)
-        secho("pid_identifier is not valid JSON", fg=Color.error)
-        return
-
     service = get_records_service()
     identity = get_identity(permission_name="system_process", role_name="admin")
 
     if not exists_record(service, pid, identity):
         secho(f"'{pid}', does not exist or is deleted", fg=Color.error)
         return
 
     old_data = service.read(id_=pid, identity=identity).data.copy()
     new_data = old_data.copy()
     pids = new_data.get("pids", {})
-    pid_key = list(pid_identifier_json.keys())[0]
+    pid_key = list(pid_identifier.keys())[0]
 
     if pids.get(pid_key, None) is None:
         secho(f"'{pid}' does not have pid identifier '{pid_key}'", fg=Color.warning)
         return
 
-    pids[pid_key] = pid_identifier_json.get(pid_key)
+    pids[pid_key] = pid_identifier.get(pid_key)
     new_data["pids"] = pids
 
     try:
         update_record(service, pid, identity, new_data, old_data)
     except Exception as error:
         secho(f"'{pid}', problem during update, {error}", fg=Color.error)
         return
@@ -379,39 +372,32 @@
 def add_identifier(identifier: str, pid: str) -> None:
     """Update the specified record's identifiers.
 
     example call:
         invenio repository records identifiers add -p "fcze8-4vx33"
         -i '{ "identifier": "10.48436/fcze8-4vx33", "scheme": "doi"}'
     """
-    try:
-        identifier_json = json.loads(identifier)
-    except Exception as error:
-        secho(str(error), fg=Color.error)
-        secho("identifier is not valid JSON", fg=Color.error)
-        return
-
     service = get_records_service()
     identity = get_identity("system_process", role_name="admin")
 
     if not exists_record(service, pid, identity):
         secho(f"'{pid}', does not exist or is deleted", fg=Color.error)
         return
 
     record_data = service.read(id_=pid, identity=identity).data.copy()
 
     current_identifiers = record_data["metadata"].get("identifiers", [])
-    current_schemes = [_["scheme"] for _ in current_identifiers]
-    scheme = identifier_json["scheme"]
+    current_schemes = [ci["scheme"] for ci in current_identifiers]
+    scheme = identifier["scheme"]
     if scheme in current_schemes:
         secho(f"scheme '{scheme}' already in identifiers", fg=Color.error)
         return
 
     old_data = record_data.copy()
-    current_identifiers.append(identifier_json)
+    current_identifiers.append(identifier)
     record_data["metadata"]["identifiers"] = current_identifiers
 
     try:
         update_record(service, pid, identity, record_data, old_data)
     except Exception as error:
         secho(f"'{pid}', Error during update, {error}", fg=Color.error)
         return
@@ -427,35 +413,28 @@
 def replace_identifier(identifier: str, pid: str) -> None:
     """Update the specified record's identifiers.
 
     example call:
         invenio repository records identifiers replace -p "fcze8-4vx33"
         -i '{ "identifier": "10.48436/fcze8-4vx33", "scheme": "doi"}'
     """
-    try:
-        identifier_json = json.loads(identifier)
-    except Exception as error:
-        secho(str(error), fg=Color.error)
-        secho("identifier is not valid JSON", fg=Color.error)
-        return
-
     service = get_records_service()
     identity = get_identity("system_process", role_name="admin")
 
     if not exists_record(service, pid, identity):
         secho(f"'{pid}', does not exist or is deleted", fg=Color.error)
         return
 
     record_data = service.read(id_=pid, identity=identity).data.copy()
     current_identifiers = record_data["metadata"].get("identifiers", [])
-    scheme = identifier_json["scheme"]
+    scheme = identifier["scheme"]
     replaced = False
     for index, current_identifier in enumerate(current_identifiers):
         if current_identifier["scheme"] == scheme:
-            current_identifiers[index] = identifier_json
+            current_identifiers[index] = identifier
             replaced = True
             break
 
     if not replaced:
         secho(f"scheme '{scheme}' not in identifiers", fg=Color.error)
         return
 
@@ -478,22 +457,18 @@
 @with_appcontext
 def delete_file(data_model: str, pid: str, filename: str) -> None:
     """Delete the file."""
     identity = get_identity("system_process", role_name="admin")
     service = get_records_service(data_model=data_model)
 
     try:
-        record = service.read(identity=identity, id_=pid)._record
-    except PIDDoesNotExistError:
-        try:
-            record = service.read_draft(identity=identity, id_=pid)._record
-        except PIDDoesNotExistError as error:
-            msg = f"Record id '{error.pid_value} ({data_model})' does not exist."
-            secho(msg, fg=Color.error)
-            return
+        record = get_record_or_draft(service, pid, identity)
+    except RuntimeError as error:
+        secho(error.msg, fg=Color.error)
+        return
 
     files = record.files
     obj = None
 
     try:
         obj = files[filename]
     except KeyError:
@@ -525,22 +500,18 @@
     override_name_match_check: bool,  # noqa: FBT001
 ) -> None:
     """Replace the file."""
     identity = get_identity("system_process", role_name="admin")
     service = get_records_service(data_model=data_model)
 
     try:
-        record = service.read(identity=identity, id_=pid)._record
-    except PIDDoesNotExistError:
-        try:
-            record = service.read_draft(identity=identity, id_=pid)._record
-        except PIDDoesNotExistError as error:
-            msg = f"Record id '{error.pid_value} ({data_model})' does not exist."
-            secho(msg, fg=Color.error)
-            return
+        record = get_record_or_draft(service, pid, identity)
+    except RuntimeError as error:
+        secho(error.msg, fg=Color.error)
+        return
 
     files = record.files
     filename = Path(input_file.name).name  # Path().name gets the filename only
     obj = None
 
     try:
         obj = files[filename]
@@ -583,22 +554,18 @@
     enable_files: bool,  # noqa: FBT001
 ) -> None:
     """Add a new file to a published record."""
     identity = get_identity("system_process", role_name="admin")
     service = get_records_service(data_model=data_model)
 
     try:
-        record = service.read(identity=identity, id_=pid)._record
-    except PIDDoesNotExistError:
-        try:
-            record = service.read_draft(identity=identity, id_=pid)._record
-        except PIDDoesNotExistError as error:
-            msg = f"Record id '{error.pid_value} ({data_model})' does not exist."
-            secho(msg, fg=Color.error)
-            return
+        record = get_record_or_draft(service, pid, identity)
+    except RuntimeError as error:
+        secho(error.msg, fg=Color.error)
+        return
 
     files = record.files
     filename = Path(input_file.name).name
 
     if files.enabled:
         obj = files.get(filename, None)
         if obj is not None:
```

### Comparing `repository-cli-0.8.0/repository_cli/types.py` & `repository-cli-0.8.1/repository_cli/types.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/repository_cli/users.py` & `repository-cli-0.8.1/repository_cli/users.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/repository_cli/utils.py` & `repository-cli-0.8.1/repository_cli/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 from invenio_access.permissions import any_user, system_process
 from invenio_accounts import current_accounts
 from invenio_rdm_records.proxies import current_rdm_records
 from invenio_rdm_records.records.models import RDMDraftMetadata, RDMRecordMetadata
 from invenio_records_marc21 import Marc21Metadata, current_records_marc21
 from invenio_records_marc21.records import DraftMetadata as Marc21DraftMetadata
 from invenio_records_marc21.records import RecordMetadata as Marc21RecordMetadata
+from sqlalchemy.orm.exc import NoResultFound
 
 if TYPE_CHECKING:
     from invenio_db import db
     from invenio_drafts_resources.records.api import Draft, Record
     from invenio_records_resources.services import RecordService
-
+    from invenio_records_resources.services.records.results import RecordItem
 
 BELOW_CONTROLFIELD = 10
 
 
 class IdentityNotFoundError(Exception):
     """Identity not found exception."""
 
@@ -70,29 +71,39 @@
     draft = None
     with suppress(Exception):
         draft = service.read_draft(id_=pid, identity=identity)
 
     return draft
 
 
+def get_record_item(service: RecordService, pid: str, identity: Identity) -> RecordItem:
+    """Get record item."""
+    try:
+        record_item = service.read(id_=pid, identity=identity)
+    except NoResultFound:
+        try:
+            record_item = service.read_draft(id_=pid, identity=identity)
+        except NoResultFound as exc:
+            msg = f"Record ({pid}) does not exists"
+            raise RuntimeError(msg) from exc
+    return record_item
+
+
+def get_data(service: RecordService, pid: str, identity: Identity) -> dict:
+    """Get data."""
+    return get_record_item(service, pid, identity).data
+
+
 def get_record_or_draft(
     service: RecordService,
     pid: str,
     identity: Identity,
 ) -> Draft | Record:
     """Get record or draft."""
-    try:
-        old_data = service.read(id_=pid, identity=identity).data
-    except Exception as exc:
-        try:
-            old_data = service.read_draft(id_=pid, identity=identity).data
-        except Exception:
-            msg = f"Record ({pid}) does not exists"
-            raise RuntimeError(msg) from exc
-    return old_data
+    return get_record_item(service, pid, identity)._record
 
 
 def get_records_service(data_model: str = "rdm") -> RecordService:
     """Get records service."""
     available_services = {
         "rdm": current_rdm_records.records_service,
         "marc21": current_records_marc21.records_service,
```

### Comparing `repository-cli-0.8.0/repository_cli.egg-info/PKG-INFO` & `repository-cli-0.8.1/repository_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-cli
-Version: 0.8.0
+Version: 0.8.1
 Summary: "CLI utilities for TU Graz Repository."
 Home-page: https://github.com/inveniosoftware/repository-cli
 Author: Graz University of Technology
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio repository cli
 Platform: any
@@ -52,14 +52,20 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.1 (release 2023-06-07)
+
+- refactor: move json validation into JSON
+- refactor: get_record_or_draft
+
+
 Version v0.8.0 (release 2023-06-01)
 
 - records: make arguments ready for drafts too
 - records: add argument delete-file
 
 
 Version v0.7.0 (release 2023-05-30)
```

### Comparing `repository-cli-0.8.0/repository_cli.egg-info/SOURCES.txt` & `repository-cli-0.8.1/repository_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/run-tests.sh` & `repository-cli-0.8.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/setup.cfg` & `repository-cli-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/tests/conftest.py` & `repository-cli-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/tests/test_rdmrecords.py` & `repository-cli-0.8.1/tests/test_rdmrecords.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.0/tests/test_rdmrecords_identifiers.py` & `repository-cli-0.8.1/tests/test_rdmrecords_identifiers.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,16 +83,21 @@
     """Test add identifier wrong identifier type."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     response = runner.invoke(
         add_identifier,
         ["--pid", r_id, "--identifier", "this is not a dict"],
     )
+
+    expected_error_msg = (
+        "ERROR - Invalid JSON provided. Check file path or json string."
+    )
+
     assert response.exit_code == 0
-    assert "identifier is not valid JSON" in response.output
+    assert expected_error_msg in response.output
 
 
 def test_add_identifiers_record_not_found(
     app_initialized: Flask,
     identifier: dict,
 ) -> None:
     """Test add identifiers record not found."""
@@ -131,27 +136,49 @@
         replace_identifier,
         ["--pid", r_id, "--identifier", json.dumps(identifier)],
     )
     assert response.exit_code == 0
     assert f"scheme '{identifier['scheme']}' not in identifiers" in response.output
 
 
+def test_replace_identifier_schema_missing(
+    app_initialized: Flask,
+    create_record: RecordItem,
+) -> None:
+    """Test replace identifier scheme missing."""
+    runner = app_initialized.test_cli_runner()
+    r_id = create_record.id
+    response = runner.invoke(
+        replace_identifier,
+        ["--pid", r_id, "--identifier", '{"identifier": "10.48436/fcze8-4vx33"}'],
+    )
+    expected_error_msg = (
+        "The given json does not validate, key: 'scheme' does not exists"
+    )
+    assert response.exit_code == 0
+    assert expected_error_msg in response.output
+
+
 def test_replace_identifier_wrong_identifier_type(
     app_initialized: Flask,
     create_record: RecordItem,
 ) -> None:
     """Test replace identifier wrong identifier type."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     response = runner.invoke(
         replace_identifier,
         ["--pid", r_id, "--identifier", "this is not a dict"],
     )
+    expected_error_msg = (
+        "ERROR - Invalid JSON provided. Check file path or json string."
+    )
+
     assert response.exit_code == 0
-    assert "identifier is not valid JSON" in response.output
+    assert expected_error_msg in response.output
 
 
 def test_replace_identifiers_record_not_found(
     app_initialized: Flask,
     identifier: dict,
 ) -> None:
     """Test replace identifiers record not found."""
```

### Comparing `repository-cli-0.8.0/tests/test_rdmrecords_pids.py` & `repository-cli-0.8.1/tests/test_rdmrecords_pids.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,16 +65,20 @@
     """Test replace pid wrong identifier type."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     response = runner.invoke(
         replace_pid,
         ["--pid", r_id, "--pid-identifier", "this is not a dict"],
     )
+
+    expected_error_msg = (
+        "ERROR - Invalid JSON provided. Check file path or json string."
+    )
     assert response.exit_code == 0
-    assert "pid_identifier is not valid JSON" in response.output
+    assert expected_error_msg in response.output
 
 
 def test_replace_pid_record_not_found(
     app_initialized: Flask,
     pid_identifier: dict,
 ) -> None:
     """Test replace pid record not found."""
```

### Comparing `repository-cli-0.8.0/tests/test_repository_cli.py` & `repository-cli-0.8.1/tests/test_repository_cli.py`

 * *Files identical despite different names*

