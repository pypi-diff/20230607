# Comparing `tmp/pyintelowl-4.4.3.tar.gz` & `tmp/pyintelowl-4.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintelowl-4.4.3.tar", last modified: Tue Apr 18 10:02:20 2023, max compression
+gzip compressed data, was "pyintelowl-4.4.4.tar", last modified: Wed Jun  7 14:42:26 2023, max compression
```

## Comparing `pyintelowl-4.4.3.tar` & `pyintelowl-4.4.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.610759 pyintelowl-4.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-18 10:02:20.610759 pyintelowl-4.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.606759 pyintelowl-4.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.606759 pyintelowl-4.4.3/pyintelowl/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.610759 pyintelowl-4.4.3/pyintelowl/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/_jobs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    52097 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/domain_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    38283 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/pyintelowl.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.606759 pyintelowl-4.4.3/pyintelowl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 10:02:20.610759 pyintelowl-4.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.610759 pyintelowl-4.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/mocked_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:42:26.487327 pyintelowl-4.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-06-07 14:42:26.487327 pyintelowl-4.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:42:26.487327 pyintelowl-4.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:42:26.487327 pyintelowl-4.4.4/pyintelowl/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:42:26.487327 pyintelowl-4.4.4/pyintelowl/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/cli/_jobs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/cli/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52097 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/cli/domain_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/cli/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/cli/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38320 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/pyintelowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyintelowl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:42:26.487327 pyintelowl-4.4.4/pyintelowl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-06-07 14:42:26.000000 pyintelowl-4.4.4/pyintelowl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-07 14:42:26.000000 pyintelowl-4.4.4/pyintelowl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:42:26.000000 pyintelowl-4.4.4/pyintelowl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-07 14:42:26.000000 pyintelowl-4.4.4/pyintelowl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-07 14:42:26.000000 pyintelowl-4.4.4/pyintelowl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 14:42:26.000000 pyintelowl-4.4.4/pyintelowl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:42:26.487327 pyintelowl-4.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:42:26.487327 pyintelowl-4.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/tests/mocked_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-07 14:42:16.000000 pyintelowl-4.4.4/tests/utils.py
```

### Comparing `pyintelowl-4.4.3/LICENSE` & `pyintelowl-4.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/PKG-INFO` & `pyintelowl-4.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelowl
-Version: 4.4.3
+Version: 4.4.4
 Summary: Robust Python SDK and CLI for IntelOwl's API
 Home-page: https://github.com/intelowlproject/pyintelowl
 Author: Matteo Lodi
 Project-URL: Documentation, https://github.com/intelowlproject/pyintelowl
 Project-URL: Funding, https://liberapay.com/IntelOwlProject/
 Project-URL: Source, https://github.com/intelowlproject/pyintelowl
 Project-URL: Tracker, https://github.com/intelowlproject/pyintelowl/issues
```

### Comparing `pyintelowl-4.4.3/README.md` & `pyintelowl-4.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/docs/conf.py` & `pyintelowl-4.4.4/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
-VERSION = "4.4.3"
+VERSION = "4.4.4"
 GITHUB_URL = "https://github.com/intelowlproject/pyintelowl"
 
 sys.path.append(os.path.abspath("../"))
 
 
 # -- Project information -----------------------------------------------------
```

### Comparing `pyintelowl-4.4.3/pyintelowl/cli/_jobs_utils.py` & `pyintelowl-4.4.4/pyintelowl/cli/_jobs_utils.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/pyintelowl/cli/_utils.py` & `pyintelowl-4.4.4/pyintelowl/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/pyintelowl/cli/analyse.py` & `pyintelowl-4.4.4/pyintelowl/cli/analyse.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/pyintelowl/cli/commands.py` & `pyintelowl-4.4.4/pyintelowl/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/pyintelowl/cli/config.py` & `pyintelowl-4.4.4/pyintelowl/cli/config.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/pyintelowl/cli/domain_checkers.py` & `pyintelowl-4.4.4/pyintelowl/cli/domain_checkers.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/pyintelowl/cli/jobs.py` & `pyintelowl-4.4.4/pyintelowl/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/pyintelowl/cli/tags.py` & `pyintelowl-4.4.4/pyintelowl/cli/tags.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/pyintelowl/exceptions.py` & `pyintelowl-4.4.4/pyintelowl/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/pyintelowl/main.py` & `pyintelowl-4.4.4/pyintelowl/main.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/pyintelowl/pyintelowl.py` & `pyintelowl-4.4.4/pyintelowl/pyintelowl.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,24 +503,25 @@
                 if answers:
                     answer = answers[0]
 
             warnings = answer.get("warnings", [])
             errors = answer.get("errors", {})
             if self.cli:
                 info_log = f"""New Job running..
-                    ID: {answer['job_id']} | Status: [u blue]{answer['status']}[/].
+                    ID: {answer.get('job_id')} | 
+                    Status: [u blue]{answer.get('status')}[/].
                     Got {len(warnings)} warnings:
                     [i yellow]{warnings if warnings else None}[/]
                     Got {len(errors)} errors:
                     [i red]{errors if errors else None}[/]
                 """
             else:
                 info_log = (
-                    f"New Job running.. ID: {answer['job_id']} "
-                    f"| Status: {answer['status']}."
+                    f"New Job running.. ID: {answer.get('job_id')} "
+                    f"| Status: {answer.get('status')}."
                     f" Got {len(warnings)} warnings:"
                     f" {warnings if warnings else None}"
                     f" Got {len(errors)} errors:"
                     f" {errors if errors else None}"
                 )
             self.logger.info(info_log)
             response.raise_for_status()
```

### Comparing `pyintelowl-4.4.3/pyintelowl.egg-info/PKG-INFO` & `pyintelowl-4.4.4/pyintelowl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelowl
-Version: 4.4.3
+Version: 4.4.4
 Summary: Robust Python SDK and CLI for IntelOwl's API
 Home-page: https://github.com/intelowlproject/pyintelowl
 Author: Matteo Lodi
 Project-URL: Documentation, https://github.com/intelowlproject/pyintelowl
 Project-URL: Funding, https://liberapay.com/IntelOwlProject/
 Project-URL: Source, https://github.com/intelowlproject/pyintelowl
 Project-URL: Tracker, https://github.com/intelowlproject/pyintelowl/issues
```

### Comparing `pyintelowl-4.4.3/pyintelowl.egg-info/SOURCES.txt` & `pyintelowl-4.4.4/pyintelowl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/pyintelowl.egg-info/requires.txt` & `pyintelowl-4.4.4/pyintelowl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/setup.py` & `pyintelowl-4.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/tests/mocked_requests.py` & `pyintelowl-4.4.4/tests/mocked_requests.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/tests/test_general.py` & `pyintelowl-4.4.4/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/tests/test_jobs.py` & `pyintelowl-4.4.4/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/tests/test_tags.py` & `pyintelowl-4.4.4/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.3/tests/utils.py` & `pyintelowl-4.4.4/tests/utils.py`

 * *Files identical despite different names*

