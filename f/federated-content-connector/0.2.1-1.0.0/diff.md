# Comparing `tmp/federated-content-connector-0.2.1.tar.gz` & `tmp/federated-content-connector-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "federated-content-connector-0.2.1.tar", last modified: Mon Jun  5 16:00:23 2023, max compression
+gzip compressed data, was "federated-content-connector-1.0.0.tar", last modified: Wed Jun  7 11:20:26 2023, max compression
```

## Comparing `federated-content-connector-0.2.1.tar` & `federated-content-connector-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8226 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.068028 federated-content-connector-0.2.1/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/federated_content_connector/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/filters/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/federated_content_connector/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.068028 federated-content-connector-0.2.1/federated_content_connector/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/federated_content_connector/templates/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/templates/federated_content_connector/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/federated_content_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8226 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.788159 federated-content-connector-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8317 2023-06-07 11:20:26.788159 federated-content-connector-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.780159 federated-content-connector-1.0.0/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8965 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/course_metadata_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/filters/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/management/commands/import_course_runs_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.776158 federated-content-connector-1.0.0/federated_content_connector/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector/templates/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/templates/federated_content_connector/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/federated_content_connector/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.784159 federated-content-connector-1.0.0/federated_content_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8317 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-07 11:20:26.000000 federated-content-connector-1.0.0/federated_content_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.788159 federated-content-connector-1.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-07 11:20:26.788159 federated-content-connector-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:26.788159 federated-content-connector-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-07 11:20:18.000000 federated-content-connector-1.0.0/tests/test_signals.py
```

### Comparing `federated-content-connector-0.2.1/CHANGELOG.rst` & `federated-content-connector-1.0.0/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.0 – 2023-06-06
+------------------
+* Fetch course metadata from discovery and store.
+
 0.2.1 – 2023-06-5
 ------------------
 * Fixed issue with product source data type
 
 0.2.0 – 2023-05-31
 ------------------
 * Added support for stage and prod landing pages via settings
```

### Comparing `federated-content-connector-0.2.1/LICENSE.txt` & `federated-content-connector-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-0.2.1/PKG-INFO` & `federated-content-connector-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 0.2.1
+Version: 1.0.0
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.0 – 2023-06-06
+------------------
+* Fetch course metadata from discovery and store.
+
 0.2.1 – 2023-06-5
 ------------------
 * Fixed issue with product source data type
 
 0.2.0 – 2023-05-31
 ------------------
 * Added support for stage and prod landing pages via settings
```

### Comparing `federated-content-connector-0.2.1/README.rst` & `federated-content-connector-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `federated-content-connector-0.2.1/federated_content_connector/filters/pipeline.py` & `federated-content-connector-1.0.0/federated_content_connector/filters/pipeline.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-0.2.1/federated_content_connector/templates/federated_content_connector/base.html` & `federated-content-connector-1.0.0/federated_content_connector/templates/federated_content_connector/base.html`

 * *Files identical despite different names*

### Comparing `federated-content-connector-0.2.1/federated_content_connector.egg-info/PKG-INFO` & `federated-content-connector-1.0.0/federated_content_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 0.2.1
+Version: 1.0.0
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.0 – 2023-06-06
+------------------
+* Fetch course metadata from discovery and store.
+
 0.2.1 – 2023-06-5
 ------------------
 * Fixed issue with product source data type
 
 0.2.0 – 2023-05-31
 ------------------
 * Added support for stage and prod landing pages via settings
```

### Comparing `federated-content-connector-0.2.1/federated_content_connector.egg-info/SOURCES.txt` & `federated-content-connector-1.0.0/federated_content_connector.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,34 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 federated_content_connector/__init__.py
 federated_content_connector/apps.py
 federated_content_connector/constants.py
+federated_content_connector/course_metadata_importer.py
 federated_content_connector/models.py
+federated_content_connector/signals.py
+federated_content_connector/tasks.py
 federated_content_connector/urls.py
 federated_content_connector.egg-info/PKG-INFO
 federated_content_connector.egg-info/SOURCES.txt
 federated_content_connector.egg-info/dependency_links.txt
 federated_content_connector.egg-info/entry_points.txt
 federated_content_connector.egg-info/not-zip-safe
 federated_content_connector.egg-info/requires.txt
 federated_content_connector.egg-info/top_level.txt
 federated_content_connector/filters/__init__.py
 federated_content_connector/filters/pipeline.py
+federated_content_connector/management/__init__.py
+federated_content_connector/management/commands/__init__.py
+federated_content_connector/management/commands/import_course_runs_metadata.py
+federated_content_connector/migrations/0001_initial.py
+federated_content_connector/migrations/__init__.py
 federated_content_connector/settings/__init__.py
 federated_content_connector/settings/common.py
 federated_content_connector/settings/production.py
 federated_content_connector/templates/federated_content_connector/base.html
 requirements/base.in
 requirements/constraints.txt
-tests/test_models.py
+tests/test_models.py
+tests/test_signals.py
```

### Comparing `federated-content-connector-0.2.1/requirements/constraints.txt` & `federated-content-connector-1.0.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-0.2.1/setup.py` & `federated-content-connector-1.0.0/setup.py`

 * *Files identical despite different names*

