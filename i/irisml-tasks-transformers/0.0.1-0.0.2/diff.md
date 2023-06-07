# Comparing `tmp/irisml-tasks-transformers-0.0.1.tar.gz` & `tmp/irisml-tasks-transformers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/shono/repos/irisml-tasks-transformers/dist/tmpja47r3ho/irisml-tasks-transformers-0.0.1.tar", last modified: Thu Aug  4 02:07:04 2022, max compression
+gzip compressed data, was "irisml-tasks-transformers-0.0.2.tar", last modified: Wed Jun  7 06:18:36 2023, max compression
```

## Comparing `irisml-tasks-transformers-0.0.1.tar` & `irisml-tasks-transformers-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2022-08-04 02:07:04.757967 irisml-tasks-transformers-0.0.1/
--rw-r--r--   0 shono     (1000) shono     (1000)     1141 2022-08-04 01:59:30.000000 irisml-tasks-transformers-0.0.1/LICENSE
--rw-r--r--   0 shono     (1000) shono     (1000)      900 2022-08-04 02:07:04.757967 irisml-tasks-transformers-0.0.1/PKG-INFO
--rw-r--r--   0 shono     (1000) shono     (1000)      603 2022-08-04 02:03:40.000000 irisml-tasks-transformers-0.0.1/README.md
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2022-08-04 02:07:04.747967 irisml-tasks-transformers-0.0.1/irisml/
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2022-08-04 02:07:04.747967 irisml-tasks-transformers-0.0.1/irisml/tasks/
--rw-r--r--   0 shono     (1000) shono     (1000)     2078 2022-08-04 02:02:30.000000 irisml-tasks-transformers-0.0.1/irisml/tasks/create_transformers_model.py
--rw-r--r--   0 shono     (1000) shono     (1000)      750 2022-08-04 01:59:40.000000 irisml-tasks-transformers-0.0.1/irisml/tasks/create_transformers_tokenizer.py
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2022-08-04 02:07:04.757967 irisml-tasks-transformers-0.0.1/irisml_tasks_transformers.egg-info/
--rw-r--r--   0 shono     (1000) shono     (1000)      900 2022-08-04 02:07:04.000000 irisml-tasks-transformers-0.0.1/irisml_tasks_transformers.egg-info/PKG-INFO
--rw-r--r--   0 shono     (1000) shono     (1000)      456 2022-08-04 02:07:04.000000 irisml-tasks-transformers-0.0.1/irisml_tasks_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 shono     (1000) shono     (1000)        1 2022-08-04 02:07:04.000000 irisml-tasks-transformers-0.0.1/irisml_tasks_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 shono     (1000) shono     (1000)       50 2022-08-04 02:07:04.000000 irisml-tasks-transformers-0.0.1/irisml_tasks_transformers.egg-info/requires.txt
--rw-r--r--   0 shono     (1000) shono     (1000)        7 2022-08-04 02:07:04.000000 irisml-tasks-transformers-0.0.1/irisml_tasks_transformers.egg-info/top_level.txt
--rw-r--r--   0 shono     (1000) shono     (1000)       81 2022-08-04 01:59:40.000000 irisml-tasks-transformers-0.0.1/pyproject.toml
--rw-r--r--   0 shono     (1000) shono     (1000)      542 2022-08-04 02:07:04.757967 irisml-tasks-transformers-0.0.1/setup.cfg
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2022-08-04 02:07:04.757967 irisml-tasks-transformers-0.0.1/test/
--rw-r--r--   0 shono     (1000) shono     (1000)      525 2022-08-04 01:59:40.000000 irisml-tasks-transformers-0.0.1/test/test_create_transformers_model.py
--rw-r--r--   0 shono     (1000) shono     (1000)      516 2022-08-04 01:59:40.000000 irisml-tasks-transformers-0.0.1/test/test_create_transformers_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/irisml/tasks/cache_transformers_model_on_azure_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/irisml/tasks/create_transformers_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/irisml/tasks/create_transformers_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/irisml/tasks/create_transformers_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-07 06:18:36.000000 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-07 06:18:36.000000 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:18:36.000000 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-07 06:18:36.000000 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 06:18:36.000000 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/test/test_cache_transformers_model_on_azure_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/test/test_create_transformers_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/test/test_create_transformers_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/test/test_create_transformers_tokenizer.py
```

### Comparing `irisml-tasks-transformers-0.0.1/LICENSE` & `irisml-tasks-transformers-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.1/PKG-INFO` & `irisml-tasks-transformers-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-transformers
-Version: 0.0.1
+Version: 0.0.2
 Summary: IrisML tasks for transformers library
 Home-page: https://github.com/microsoft/irisml-tasks-transformers
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-transformers-0.0.1/README.md` & `irisml-tasks-transformers-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.1/irisml/tasks/create_transformers_tokenizer.py` & `irisml-tasks-transformers-0.0.2/irisml/tasks/create_transformers_tokenizer.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.1/irisml_tasks_transformers.egg-info/PKG-INFO` & `irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-transformers
-Version: 0.0.1
+Version: 0.0.2
 Summary: IrisML tasks for transformers library
 Home-page: https://github.com/microsoft/irisml-tasks-transformers
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-transformers-0.0.1/setup.cfg` & `irisml-tasks-transformers-0.0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [metadata]
 name = irisml-tasks-transformers
-version = 0.0.1
+version = 0.0.2
 url = https://github.com/microsoft/irisml-tasks-transformers
 description = IrisML tasks for transformers library
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
 
 [options]
 packages = find_namespace:
 python_requires = >= 3.8
 install_requires = 
 	irisml
 	irisml-tasks-training
-	transformers~=4.21.0
+	transformers~=4.29.2
 
 [options.packages.find]
 include = 
 	irisml.tasks
 
 [flake8]
 max-line-length = 200
```

### Comparing `irisml-tasks-transformers-0.0.1/test/test_create_transformers_model.py` & `irisml-tasks-transformers-0.0.2/test/test_create_transformers_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.1/test/test_create_transformers_tokenizer.py` & `irisml-tasks-transformers-0.0.2/test/test_create_transformers_tokenizer.py`

 * *Files identical despite different names*

