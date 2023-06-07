# Comparing `tmp/pyright-1.1.311.tar.gz` & `tmp/pyright-1.1.312.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyright-1.1.311.tar", last modified: Wed May 31 08:23:19 2023, max compression
+gzip compressed data, was "pyright-1.1.312.tar", last modified: Wed Jun  7 13:00:23 2023, max compression
```

## Comparing `pyright-1.1.311.tar` & `pyright-1.1.312.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:23:19.010905 pyright-1.1.311/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 08:23:07.000000 pyright-1.1.311/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 08:23:07.000000 pyright-1.1.311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-31 08:23:19.010905 pyright-1.1.311/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-31 08:23:07.000000 pyright-1.1.311/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-31 08:23:07.000000 pyright-1.1.311/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:23:19.010905 pyright-1.1.311/pyright/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-31 08:23:07.000000 pyright-1.1.311/pyright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 08:23:07.000000 pyright-1.1.311/pyright/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-05-31 08:23:07.000000 pyright-1.1.311/pyright/_mureq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-31 08:23:07.000000 pyright-1.1.311/pyright/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 08:23:07.000000 pyright-1.1.311/pyright/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-31 08:23:07.000000 pyright-1.1.311/pyright/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-31 08:23:07.000000 pyright-1.1.311/pyright/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-31 08:23:07.000000 pyright-1.1.311/pyright/langserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-05-31 08:23:07.000000 pyright-1.1.311/pyright/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-31 08:23:07.000000 pyright-1.1.311/pyright/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-31 08:23:07.000000 pyright-1.1.311/pyright/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:23:19.010905 pyright-1.1.311/pyright.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-31 08:23:18.000000 pyright-1.1.311/pyright.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 08:23:18.000000 pyright-1.1.311/pyright.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:23:18.000000 pyright-1.1.311/pyright.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-31 08:23:18.000000 pyright-1.1.311/pyright.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:23:18.000000 pyright-1.1.311/pyright.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 08:23:18.000000 pyright-1.1.311/pyright.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 08:23:18.000000 pyright-1.1.311/pyright.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 08:23:07.000000 pyright-1.1.311/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 08:23:19.010905 pyright-1.1.311/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2149 2023-05-31 08:23:07.000000 pyright-1.1.311/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:23.826006 pyright-1.1.312/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 13:00:14.000000 pyright-1.1.312/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 13:00:14.000000 pyright-1.1.312/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-07 13:00:23.826006 pyright-1.1.312/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-07 13:00:14.000000 pyright-1.1.312/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-07 13:00:14.000000 pyright-1.1.312/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:23.826006 pyright-1.1.312/pyright/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-07 13:00:14.000000 pyright-1.1.312/pyright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-07 13:00:14.000000 pyright-1.1.312/pyright/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-06-07 13:00:14.000000 pyright-1.1.312/pyright/_mureq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-07 13:00:14.000000 pyright-1.1.312/pyright/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 13:00:14.000000 pyright-1.1.312/pyright/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-07 13:00:14.000000 pyright-1.1.312/pyright/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 13:00:14.000000 pyright-1.1.312/pyright/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-07 13:00:14.000000 pyright-1.1.312/pyright/langserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-07 13:00:14.000000 pyright-1.1.312/pyright/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-07 13:00:14.000000 pyright-1.1.312/pyright/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-07 13:00:14.000000 pyright-1.1.312/pyright/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:23.826006 pyright-1.1.312/pyright.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-07 13:00:23.000000 pyright-1.1.312/pyright.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-07 13:00:23.000000 pyright-1.1.312/pyright.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:00:23.000000 pyright-1.1.312/pyright.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 13:00:23.000000 pyright-1.1.312/pyright.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:00:23.000000 pyright-1.1.312/pyright.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 13:00:23.000000 pyright-1.1.312/pyright.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 13:00:23.000000 pyright-1.1.312/pyright.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 13:00:14.000000 pyright-1.1.312/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:00:23.826006 pyright-1.1.312/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2149 2023-06-07 13:00:14.000000 pyright-1.1.312/setup.py
```

### Comparing `pyright-1.1.311/LICENSE` & `pyright-1.1.312/LICENSE`

 * *Files identical despite different names*

### Comparing `pyright-1.1.311/PKG-INFO` & `pyright-1.1.312/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyright
-Version: 1.1.311
+Version: 1.1.312
 Summary: Command line wrapper for pyright
 Home-page: https://github.com/RobertCraigie/pyright-python
 Author: Robert Craigie
 Maintainer: Robert Craigie
 License: MIT
 Project-URL: Source, https://github.com/RobertCraigie/pyright-python
 Project-URL: Tracker, https://github.com/RobertCraigie/pyright-python/issues
@@ -61,15 +61,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.311
+    rev: v1.1.312
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
```

### Comparing `pyright-1.1.311/README.md` & `pyright-1.1.312/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.311
+    rev: v1.1.312
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
```

### Comparing `pyright-1.1.311/pyright/__init__.py` & `pyright-1.1.312/pyright/__init__.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.311/pyright/_mureq.py` & `pyright-1.1.312/pyright/_mureq.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.311/pyright/_utils.py` & `pyright-1.1.312/pyright/_utils.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.311/pyright/cli.py` & `pyright-1.1.312/pyright/cli.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.311/pyright/errors.py` & `pyright-1.1.312/pyright/errors.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.311/pyright/langserver.py` & `pyright-1.1.312/pyright/langserver.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.311/pyright/node.py` & `pyright-1.1.312/pyright/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import json
 import shutil
 import logging
 import platform
 import subprocess
 from functools import lru_cache
-from typing import Dict, Mapping, Tuple, Optional, Union, Any
+from typing import Dict, Mapping, Tuple, Optional, Union, Any, cast
 from pathlib import Path
 
 from . import errors
 from .types import Binary, Target, Strategy, check_target
 from .utils import get_env_dir, env_to_bool, get_bin_dir, maybe_decode
 
 
@@ -108,15 +108,18 @@
         node_args = [str(binary.path), *args]
     elif binary.strategy == Strategy.GLOBAL:
         node_args = [str(binary.path), *args]
     else:
         raise RuntimeError(f'Unknown strategy: {binary.strategy}')
 
     log.debug('Running node command with args: %s', node_args)
-    return subprocess.run(node_args, env=env, **kwargs)
+    return cast(
+        'subprocess.CompletedProcess[str] | subprocess.CompletedProcess[bytes]',
+        subprocess.run(node_args, env=env, **kwargs),
+    )
 
 
 def version(target: Target) -> Tuple[int, ...]:
     proc = run(target, '--version', stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     output = maybe_decode(proc.stdout)
     match = VERSION_RE.search(output)
     if not match:
```

### Comparing `pyright-1.1.311/pyright/types.py` & `pyright-1.1.312/pyright/types.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.311/pyright/utils.py` & `pyright-1.1.312/pyright/utils.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.311/pyright.egg-info/PKG-INFO` & `pyright-1.1.312/pyright.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyright
-Version: 1.1.311
+Version: 1.1.312
 Summary: Command line wrapper for pyright
 Home-page: https://github.com/RobertCraigie/pyright-python
 Author: Robert Craigie
 Maintainer: Robert Craigie
 License: MIT
 Project-URL: Source, https://github.com/RobertCraigie/pyright-python
 Project-URL: Tracker, https://github.com/RobertCraigie/pyright-python/issues
@@ -61,15 +61,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.311
+    rev: v1.1.312
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
```

### Comparing `pyright-1.1.311/setup.py` & `pyright-1.1.312/setup.py`

 * *Files identical despite different names*

