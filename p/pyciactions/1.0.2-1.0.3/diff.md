# Comparing `tmp/pyciactions-1.0.2.tar.gz` & `tmp/pyciactions-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyciactions-1.0.2.tar", last modified: Wed Jun  7 07:14:49 2023, max compression
+gzip compressed data, was "pyciactions-1.0.3.tar", last modified: Wed Jun  7 07:18:23 2023, max compression
```

## Comparing `pyciactions-1.0.2.tar` & `pyciactions-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:14:49.072847 pyciactions-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2784 2023-06-07 07:14:49.070847 pyciactions-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2587 2023-06-07 06:34:39.000000 pyciactions-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:14:48.974791 pyciactions-1.0.2/pyciactions/
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.2/pyciactions/IWorkflow.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-07 06:05:14.000000 pyciactions-1.0.2/pyciactions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.2/pyciactions/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:14:49.056102 pyciactions-1.0.2/pyciactions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2784 2023-06-07 07:14:48.000000 pyciactions-1.0.2/pyciactions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-07 07:14:48.000000 pyciactions-1.0.2/pyciactions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 07:14:48.000000 pyciactions-1.0.2/pyciactions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 07:14:48.000000 pyciactions-1.0.2/pyciactions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-07 07:14:48.000000 pyciactions-1.0.2/pyciactions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 07:14:49.073845 pyciactions-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      448 2023-06-07 06:58:02.000000 pyciactions-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:18:23.743419 pyciactions-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-06-07 07:18:23.741229 pyciactions-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2587 2023-06-07 06:34:39.000000 pyciactions-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:18:23.647424 pyciactions-1.0.3/pyciactions/
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.3/pyciactions/IWorkflow.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-07 06:05:14.000000 pyciactions-1.0.3/pyciactions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.3/pyciactions/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:18:23.725358 pyciactions-1.0.3/pyciactions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-06-07 07:18:23.000000 pyciactions-1.0.3/pyciactions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-07 07:18:23.000000 pyciactions-1.0.3/pyciactions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 07:18:23.000000 pyciactions-1.0.3/pyciactions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 07:18:23.000000 pyciactions-1.0.3/pyciactions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-07 07:18:23.000000 pyciactions-1.0.3/pyciactions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 07:18:23.744419 pyciactions-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-07 07:17:53.000000 pyciactions-1.0.3/setup.py
```

### Comparing `pyciactions-1.0.2/LICENSE` & `pyciactions-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.2/PKG-INFO` & `pyciactions-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: pyciactions
-Version: 1.0.2
-Summary: Declarative builder for Github Action Scripts
-Author: Julien Bongars
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Python CI Workflow Documentation
 
 This documentation provides an overview of the Python CI workflow implemented using GitHub Actions.
 
 ### Workflow Overview
 
 The Python CI workflow is triggered by two events: pushes to the `main` branch and pull requests targeting the `main` branch. It consists of a single job named `build`, which runs on an `ubuntu-latest` environment.
@@ -76,8 +68,8 @@
                     on=[on_push_main, on_pull_request_main],
                     jobs=[job])
 
 # Generate workflow file
 generate(workflow, ".github/workflows/python_ci.yml")
 ```
 
-The generated workflow file, python_ci.yml, can be found in the .github/workflows directory of the repository.
+The generated workflow file, python_ci.yml, can be found in the .github/workflows directory of the repository.
```

### Comparing `pyciactions-1.0.2/README.md` & `pyciactions-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: pyciactions
+Version: 1.0.3
+Summary: Declarative builder for Github Action Scripts
+Home-page: https://github.com/JBongars/pyciactions
+Author: Julien Bongars
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Python CI Workflow Documentation
 
 This documentation provides an overview of the Python CI workflow implemented using GitHub Actions.
 
 ### Workflow Overview
 
 The Python CI workflow is triggered by two events: pushes to the `main` branch and pull requests targeting the `main` branch. It consists of a single job named `build`, which runs on an `ubuntu-latest` environment.
@@ -68,8 +77,8 @@
                     on=[on_push_main, on_pull_request_main],
                     jobs=[job])
 
 # Generate workflow file
 generate(workflow, ".github/workflows/python_ci.yml")
 ```
 
-The generated workflow file, python_ci.yml, can be found in the .github/workflows directory of the repository.
+The generated workflow file, python_ci.yml, can be found in the .github/workflows directory of the repository.
```

### Comparing `pyciactions-1.0.2/pyciactions.egg-info/PKG-INFO` & `pyciactions-1.0.3/pyciactions.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.2
+Version: 1.0.3
 Summary: Declarative builder for Github Action Scripts
+Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
 
 This documentation provides an overview of the Python CI workflow implemented using GitHub Actions.
```

