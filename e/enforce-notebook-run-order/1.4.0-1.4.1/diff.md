# Comparing `tmp/enforce_notebook_run_order-1.4.0.tar.gz` & `tmp/enforce_notebook_run_order-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enforce_notebook_run_order-1.4.0.tar", max compression
+gzip compressed data, was "enforce_notebook_run_order-1.4.1.tar", max compression
```

## Comparing `enforce_notebook_run_order-1.4.0.tar` & `enforce_notebook_run_order-1.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4156 2023-06-06 20:51:56.061521 enforce_notebook_run_order-1.4.0/README.md
--rw-r--r--   0        0        0      930 2023-06-06 20:51:56.061521 enforce_notebook_run_order-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      131 2023-06-06 20:51:56.061521 enforce_notebook_run_order-1.4.0/src/enforce_notebook_run_order/__init__.py
--rw-r--r--   0        0        0     1562 2023-06-06 20:51:56.061521 enforce_notebook_run_order-1.4.0/src/enforce_notebook_run_order/cli.py
--rw-r--r--   0        0        0     4664 2023-06-06 20:51:56.061521 enforce_notebook_run_order-1.4.0/src/enforce_notebook_run_order/enforce_notebook_run_order.py
--rw-r--r--   0        0        0     4073 2023-06-06 20:51:56.061521 enforce_notebook_run_order-1.4.0/src/enforce_notebook_run_order/temp_notebook.py
--rw-r--r--   0        0        0     2045 2023-06-06 20:51:56.061521 enforce_notebook_run_order-1.4.0/src/enforce_notebook_run_order/utils.py
--rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 enforce_notebook_run_order-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4374 2023-06-07 17:39:05.651222 enforce_notebook_run_order-1.4.1/README.md
+-rw-r--r--   0        0        0      930 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/__init__.py
+-rw-r--r--   0        0        0     1562 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/cli.py
+-rw-r--r--   0        0        0     4664 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/enforce_notebook_run_order.py
+-rw-r--r--   0        0        0     4138 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/temp_notebook.py
+-rw-r--r--   0        0        0     2045 2023-06-07 17:39:05.655222 enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/utils.py
+-rw-r--r--   0        0        0     5092 1970-01-01 00:00:00.000000 enforce_notebook_run_order-1.4.1/PKG-INFO
```

### Comparing `enforce_notebook_run_order-1.4.0/README.md` & `enforce_notebook_run_order-1.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 <p align="left">
  <a href="https://badge.fury.io/py/enforce-notebook-run-order">
    <img src="https://badge.fury.io/py/enforce-notebook-run-order@2x.png" alt="PyPI version" height="20">
  </a>
+ <a href="https://codecov.io/gh/christopher-hacker/enforce-notebook-run-order" > 
+   <img src="https://codecov.io/gh/christopher-hacker/enforce-notebook-run-order/branch/main/graph/badge.svg?token=019MXVQYN5"/> 
+ </a>
   <a href="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/test.yaml">
     <img src="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/test.yaml/badge.svg" alt="Run tests">
   </a>
   <a href="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/auto-tag.yml">
     <img src="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/auto-tag.yml/badge.svg" alt="Create a tag if version changed">
   </a>
   <a href="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/publish-pypi.yaml">
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-[PyPI_version] [Run_tests] [Create_a_tag_if_version_changed] [Publish_to_PyPi]
-[Build_docs]
+[PyPI_version] [https://codecov.io/gh/christopher-hacker/enforce-notebook-run-
+order/branch/main/graph/badge.svg?token=019MXVQYN5] [Run_tests] [Create_a_tag
+if_version_changed] [Publish_to_PyPi] [Build_docs]
 enforce-notebook-run-order ========================== Enforce the run order of
 Jupyter notebooks. Jupyter notebooks are great for interactive data analysis.
 However, when they can encourage a bad habit: running cells out of order. This
 can lead to notebooks being committed to the repository in a state where they
 don\'t run from top to bottom, and other collaborators may receive different
 results when running the notebook from top to bottom. `enforce-notebook-run-
 order` enforces the run order of a notebook by raising an exception if any
```

### Comparing `enforce_notebook_run_order-1.4.0/pyproject.toml` & `enforce_notebook_run_order-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enforce-notebook-run-order"
-version = "1.4.0"
+version = "1.4.1"
 description = ""
 authors = ["Chris Hacker <49451910+christopher-hacker@users.noreply.github.com>"]
 license = "MIT"
 urls = { homepage = "https://github.com/christopher-hacker/enforce-notebook-run-order" }
 readme = "README.md"
 packages = [
     { include = "enforce_notebook_run_order", from = "src" },
```

### Comparing `enforce_notebook_run_order-1.4.0/src/enforce_notebook_run_order/cli.py` & `enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/cli.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-1.4.0/src/enforce_notebook_run_order/enforce_notebook_run_order.py` & `enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/enforce_notebook_run_order.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-1.4.0/src/enforce_notebook_run_order/temp_notebook.py` & `enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/temp_notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Creates and runs a temporary notebook to verify outputs"""
 
 import json
 from pathlib import Path
 import re
 import shutil
 import subprocess
+import sys
 import tempfile
 from . import utils
 
 
 class NotebookRunFailedError(Exception):
     """
     raised when a notebook fails to run because the provided json is not a valid notebook
@@ -40,14 +41,16 @@
 
         Raises:
             NotebookRunFailedError: if the notebook fails to run because
                 the provided json is not a valid notebook
         """
         resp = subprocess.run(
             [
+                sys.executable,
+                "-m",
                 "jupyter",
                 "nbconvert",
                 "--to",
                 "notebook",
                 "--execute",
                 "--output",
                 self.output_notebook_path,
```

### Comparing `enforce_notebook_run_order-1.4.0/src/enforce_notebook_run_order/utils.py` & `enforce_notebook_run_order-1.4.1/src/enforce_notebook_run_order/utils.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-1.4.0/PKG-INFO` & `enforce_notebook_run_order-1.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enforce-notebook-run-order
-Version: 1.4.0
+Version: 1.4.1
 Summary: 
 License: MIT
 Author: Chris Hacker
 Author-email: 49451910+christopher-hacker@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,17 @@
 Project-URL: homepage, https://github.com/christopher-hacker/enforce-notebook-run-order
 Description-Content-Type: text/markdown
 
 <p align="left">
  <a href="https://badge.fury.io/py/enforce-notebook-run-order">
    <img src="https://badge.fury.io/py/enforce-notebook-run-order@2x.png" alt="PyPI version" height="20">
  </a>
+ <a href="https://codecov.io/gh/christopher-hacker/enforce-notebook-run-order" > 
+   <img src="https://codecov.io/gh/christopher-hacker/enforce-notebook-run-order/branch/main/graph/badge.svg?token=019MXVQYN5"/> 
+ </a>
   <a href="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/test.yaml">
     <img src="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/test.yaml/badge.svg" alt="Run tests">
   </a>
   <a href="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/auto-tag.yml">
     <img src="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/auto-tag.yml/badge.svg" alt="Create a tag if version changed">
   </a>
   <a href="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/publish-pypi.yaml">
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 1.4.0 Summary:
+Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 1.4.1 Summary:
 License: MIT Author: Chris Hacker Author-email: 49451910+christopher-
 hacker@users.noreply.github.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
 (>=8.1.3,<9.0.0) Requires-Dist: jupyter (>=1.0.0,<2.0.0) Project-URL: homepage,
 https://github.com/christopher-hacker/enforce-notebook-run-order Description-
 Content-Type: text/markdown
-[PyPI_version] [Run_tests] [Create_a_tag_if_version_changed] [Publish_to_PyPi]
-[Build_docs]
+[PyPI_version] [https://codecov.io/gh/christopher-hacker/enforce-notebook-run-
+order/branch/main/graph/badge.svg?token=019MXVQYN5] [Run_tests] [Create_a_tag
+if_version_changed] [Publish_to_PyPi] [Build_docs]
 enforce-notebook-run-order ========================== Enforce the run order of
 Jupyter notebooks. Jupyter notebooks are great for interactive data analysis.
 However, when they can encourage a bad habit: running cells out of order. This
 can lead to notebooks being committed to the repository in a state where they
 don\'t run from top to bottom, and other collaborators may receive different
 results when running the notebook from top to bottom. `enforce-notebook-run-
 order` enforces the run order of a notebook by raising an exception if any
```

