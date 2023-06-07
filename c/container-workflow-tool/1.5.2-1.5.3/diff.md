# Comparing `tmp/container-workflow-tool-1.5.2.tar.gz` & `tmp/container-workflow-tool-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "container-workflow-tool-1.5.2.tar", last modified: Mon Nov  7 11:16:30 2022, max compression
+gzip compressed data, was "container-workflow-tool-1.5.3.tar", last modified: Wed Jun  7 10:18:15 2023, max compression
```

## Comparing `container-workflow-tool-1.5.2.tar` & `container-workflow-tool-1.5.3.tar`

### file list

```diff
@@ -1,43 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:16:30.908326 container-workflow-tool-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2022-11-07 11:16:30.908326 container-workflow-tool-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:16:30.908326 container-workflow-tool-1.5.2/container_workflow_tool/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1447 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6712 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/cli_common.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:16:30.908326 container-workflow-tool-1.5.2/container_workflow_tool/config/
--rw-r--r--   0 runner    (1001) docker     (121)     4959 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/default.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5038 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/f27.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5005 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/f28.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5041 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/f29.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5037 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/f30.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/f31.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4889 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/f32.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4871 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/f33.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4872 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/f34.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4959 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/rawhide.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:16:30.908326 container-workflow-tool-1.5.2/container_workflow_tool/config/share/
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/share/cwt_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config/share/urls.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4592 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    26368 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/distgit.py
--rw-r--r--   0 runner    (1001) docker     (121)     4496 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/koji.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    23237 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2764 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/container_workflow_tool/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:16:30.908326 container-workflow-tool-1.5.2/container_workflow_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2022-11-07 11:16:30.000000 container-workflow-tool-1.5.2/container_workflow_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-11-07 11:16:30.000000 container-workflow-tool-1.5.2/container_workflow_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 11:16:30.000000 container-workflow-tool-1.5.2/container_workflow_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-07 11:16:30.000000 container-workflow-tool-1.5.2/container_workflow_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-07 11:16:30.000000 container-workflow-tool-1.5.2/container_workflow_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-07 11:16:30.000000 container-workflow-tool-1.5.2/container_workflow_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 11:16:30.000000 container-workflow-tool-1.5.2/container_workflow_tool.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:16:30.908326 container-workflow-tool-1.5.2/man/
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/man/cwt.1
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 11:16:30.908326 container-workflow-tool-1.5.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3138 2022-11-07 11:16:17.000000 container-workflow-tool-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.123876 container-workflow-tool-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-07 10:18:15.123876 container-workflow-tool-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.119876 container-workflow-tool-1.5.3/container_workflow_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1447 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/cli_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.119876 container-workflow-tool-1.5.3/container_workflow_tool/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f27.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f28.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f29.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f30.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f31.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f33.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/f34.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/rawhide.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.119876 container-workflow-tool-1.5.3/container_workflow_tool/config/share/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/share/cwt_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config/share/urls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/distgit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/git_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/koji.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23655 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/container_workflow_tool/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.119876 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 10:18:15.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:18:14.000000 container-workflow-tool-1.5.3/container_workflow_tool.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.119876 container-workflow-tool-1.5.3/man/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/man/cwt.1
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:18:15.123876 container-workflow-tool-1.5.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:18:15.123876 container-workflow-tool-1.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_brew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_distgit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_git_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-07 10:18:06.000000 container-workflow-tool-1.5.3/tests/test_utility.py
```

### Comparing `container-workflow-tool-1.5.2/LICENSE` & `container-workflow-tool-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/Makefile` & `container-workflow-tool-1.5.3/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.PHONY: test-in-container build-generator push-generator
+.PHONY: test-in-container build-generator push-generator build
 
 TEST_IMAGE=cwt-tests
 GENERATOR_IMAGE=quay.io/rhscl/cwt-generator
 UNAME=$(shell uname)
 ifeq ($(UNAME),Darwin)
 	PODMAN := /usr/local/bin/docker
 else
```

### Comparing `container-workflow-tool-1.5.2/PKG-INFO` & `container-workflow-tool-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: container-workflow-tool
-Version: 1.5.2
+Version: 1.5.3
 Summary: A python3 tool to make rebuilding images easier by automating several steps of the process.
 Home-page: https://github.com/sclorg/container-workflow-tool
 Author: Petr Kubat
 Author-email: pkubat@redhat.com
 License: MIT
 Keywords: tool,containers,images,automate,workflow
 Classifier: Development Status :: 4 - Beta
```

### Comparing `container-workflow-tool-1.5.2/README.md` & `container-workflow-tool-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/cli.py` & `container-workflow-tool-1.5.3/container_workflow_tool/cli.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/cli_common.py` & `container-workflow-tool-1.5.3/container_workflow_tool/cli_common.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config/default.yaml` & `container-workflow-tool-1.5.3/container_workflow_tool/config/default.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config/f27.yaml` & `container-workflow-tool-1.5.3/container_workflow_tool/config/f27.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config/f28.yaml` & `container-workflow-tool-1.5.3/container_workflow_tool/config/f28.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config/f29.yaml` & `container-workflow-tool-1.5.3/container_workflow_tool/config/f29.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config/f30.yaml` & `container-workflow-tool-1.5.3/container_workflow_tool/config/f30.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config/f31.yaml` & `container-workflow-tool-1.5.3/container_workflow_tool/config/f31.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config/f32.yaml` & `container-workflow-tool-1.5.3/container_workflow_tool/config/f32.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config/f33.yaml` & `container-workflow-tool-1.5.3/container_workflow_tool/config/f33.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config/f34.yaml` & `container-workflow-tool-1.5.3/container_workflow_tool/config/f34.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config/rawhide.yaml` & `container-workflow-tool-1.5.3/container_workflow_tool/config/rawhide.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config/share/urls.yaml` & `container-workflow-tool-1.5.3/container_workflow_tool/config/share/urls.yaml`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/config.py` & `container-workflow-tool-1.5.3/container_workflow_tool/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Loader class and construct_include function based on
 # code by Josh Bode, shared under the MIT license:
 # https://gist.github.com/joshbode/569627ced3076931b02f
 
 import os
 
 import yaml
-from typing import IO
 
 
 class Loader(yaml.SafeLoader):
     """YAML Loader with `!include` constructor."""
 
     def __init__(self, stream):
         """Initialise Loader."""
@@ -66,14 +65,17 @@
 
         urls = config["urls"]
         images = config["images"]
         self["layers"] = config["layer_ordering"]
         self["packager_util"] = config["packager_utils"]
         self["hostname_url"] = config.get("hostname_url", "")
         self["product"] = config.get("product", "")
+        self["jira_project"] = config.get("jira_project", "")
+        self["jira_label"] = config.get("jira_label", "")
+        self["jira_url"] = config.get("jira_url", "")
         self["image_names"] = config.get("image_names", "")
         self["rebuild_reason"] = config.get("rebuild_reason", "")
         self["ignore_files"] = config["ignore_files"]
         self["groups"] = config.get("groups", {})
         self["mails"] = config.get("mails", {})
         self["df_ext"] = config.get("df_ext", ".fedora")
         self["raw"] = config
```

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/constants.py` & `container-workflow-tool-1.5.3/container_workflow_tool/constants.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/distgit.py` & `container-workflow-tool-1.5.3/container_workflow_tool/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,590 +1,607 @@
+# description     : Script for helping with the rebuild of container images.
+# author          : pkubat@redhat.com
+# notes           : Rewritten from a shell script originally created by hhorak@redhat.com.
+# python_version  : 3.x
+
+import subprocess
 import os
 import shutil
 import re
-import subprocess
-
-from git import Repo
-from git.exc import GitCommandError
+import tempfile
+import pprint
+import getpass
+import logging
+
+from git import Repo, GitError
+from typing import List, Any
+from pathlib import Path
 
 import container_workflow_tool.utility as u
+from container_workflow_tool.koji import KojiAPI
+from container_workflow_tool.distgit import DistgitAPI
+from container_workflow_tool.git_operations import GitOperations
 from container_workflow_tool.utility import RebuilderError
+from container_workflow_tool.config import Config
+
 
+class ImageRebuilder:
+    """Class for rebuilding Container images."""
 
-class DistgitAPI(object):
-    """Class for working with dist-git."""
+    def __init__(self,
+                 base_image: str,
+                 rebuild_reason: str = None,
+                 config: str = "default.yaml",
+                 release: str = "current"):
+        """ Init method of ImageRebuilder class
 
-    def __init__(self, base_image, conf, rebuild_reason, logger):
-        self.conf = conf
+        Args:
+            base_image (str): image id to be used as a base image
+            config (str, optional): configuration file to be used
+            rebuild_reason (str, optional): reason for the rebuild,
+                                            used in commit
+        """
         self.base_image = base_image
-        if not rebuild_reason:
-            rebuild_reason = self.conf.rebuild_reason
-        self.rebuild_reason = rebuild_reason.format(base_image=base_image)
-        self.logger = logger if logger else u.setup_logger("dist-git")
-        self.df_ext = self.conf.df_ext
 
+        self._brewapi: KojiAPI = None
+        self._distgit: DistgitAPI = None
+        self._git_ops: GitOperations = None
         self.commit_msg = None
+        self.args = None
+        self.tmp_workdir: str = None
+        self.repo_url = None
+        self.jira_header = None
+
+        self.conf_name = config
+        self.rebuild_reason = rebuild_reason
+        self.do_image = None
+        self.exclude_image = None
+        self.do_set = None
+        self.check_script = None
+        self.image_set = None
+        self.disable_klist = None
+        self.output_file = None
+        self.latest_release = None
+
+        self.logger = self._setup_logger()
+        self.set_config(self.conf_name, release=release)
+
+    @classmethod
+    def from_args(cls, args) -> Any:
+        """
+        Creates an ImageRebuilder instance from argparse arguments.
+        """
+        config = args.config if args.config else 'default.yaml'
+        config_path, image_set = u._split_config_path(config)
+        rebuilder = ImageRebuilder(base_image=args.base, config=config_path, release=image_set)
+        rebuilder._setup_args(args)
+        rebuilder.setup_log_to_file()
+        return rebuilder
+
+    def setup_log_to_file(self):
+        # File handler
+        if self.output_file:
+            out_file = Path(self.output_file)
+            # If file is not absolute lets create out_file from current directory
+            if not out_file.is_absolute():
+                out_file = Path.cwd() / self.output_file
+            file_handler = logging.FileHandler(out_file)
+            file_handler.setLevel(logging.INFO)
+            file_format_str = "%(message)s"
+            file_formatter = logging.Formatter(file_format_str)
+            file_handler.setFormatter(file_formatter)
+            self.logger.addHandler(file_handler)
+
+    def _setup_args(self, args):
+        self.args = args
+
+        if args.config:
+            config_path, image_set = u._split_config_path(args.config)
+            self.set_config(config_path, image_set)
+        if args.tmp:
+            self.set_tmp_workdir(args.tmp)
+        if args.clear_cache:
+            self.clear_cache()
+        if args.do_image:
+            self.set_do_images(args.do_image)
+        if args.exclude_image:
+            self.set_exclude_images(args.exclude_image)
+        if args.do_set:
+            self.set_do_set(args.do_set)
+        self.logger.setLevel(u._transform_verbosity(args.verbosity))
+
+        # Command specific
+        # TODO: generalize?
+        if getattr(args, 'repo_url', None) is not None and args.repo_url:
+            self.set_repo_url(args.repo_url)
+        if getattr(args, 'commit_msg', None) is not None:
+            self.set_commit_msg(args.commit_msg)
+        if getattr(args, 'rebuild_reason', None) is not None and args.rebuild_reason:
+            self.rebuild_reason = args.rebuild_reason
+        if getattr(args, 'check_script', None) is not None and args.check_script:
+            self.check_script = args.check_script
+        if getattr(args, 'disable_klist', None) is not None and args.disable_klist:
+            self.disable_klist = args.disable_klist
+        if getattr(args, 'latest_release', None) is not None and args.latest_release:
+            self.latest_release = args.latest_release
+        if getattr(args, 'output_file', None) is not None and args.output_file:
+            self.output_file = args.output_file
+
+        # Image set to build
+        if getattr(args, 'image_set', None) is not None and args.image_set:
+            self.image_set = args.image_set
+
+    def _get_set_from_config(self, layer: str) -> str:
+        i = getattr(self.conf, layer, [])
+        if i is None:
+            err_msg = "Image set '{}' not found in config.".format(layer)
+            raise RebuilderError(err_msg)
+        return i
+
+    @property
+    def distgit(self):
+        if not self._distgit:
+            self._distgit = DistgitAPI(self.base_image, self.conf,
+                                       self.rebuild_reason,
+                                       self.logger.getChild("dist-git"))
+        return self._distgit
+
+    @property
+    def git_ops(self):
+        if not self._git_ops:
+            self._git_ops = GitOperations(self.base_image, self.conf,
+                                          self.rebuild_reason,
+                                          self.logger.getChild("-git-ops"))
+        return self._git_ops
+
+    @property
+    def brewapi(self):
+        if not self._brewapi:
+            self._brewapi = KojiAPI(self.conf, self.logger.getChild("koji"),
+                                    self.latest_release)
+        return self._brewapi
+
+    def _setup_logger(self, level=logging.INFO, user_logger=None, name=__name__):
+        # If a logger is already set up, do not setup a new one
+        if hasattr(self, "logger") and self.logger:
+            return self.logger
+        # If a logger has been provided, do not setup own
+        if user_logger and isinstance(user_logger, logging.Logger):
+            logger = user_logger
+        else:
+            logger = u.setup_logger(name, level)
 
-    def set_commit_msg(self, msg):
-        """
-        Set the commit message to some other than the default one.
+        self.logger = logger
+        return logger
 
-        Args:
-            msg(str): Message to be written into the commit.
-        """
-        self.commit_msg = msg
+    def _check_kerb_ticket(self):
+        if not self.disable_klist:
+            ret = subprocess.run(["klist"], stdout=subprocess.DEVNULL)
+            if ret.returncode:
+                raise(RebuilderError("Kerberos token not found."))
+
+    def _change_workdir(self, path: str):
+        self.logger.info("Using working directory: " + path)
+        os.chdir(path)
+
+    def _get_tmp_workdir(self, setup_dir: bool = True) -> str:
+        self._check_base(self.base_image)
+        # Check if the workdir has been set by the user
+        if self.tmp_workdir:
+            return self.tmp_workdir
+        tmp = None
+        tmp_id = self.base_image.replace(":", "-")
+        # Check if there is an existing tempdir for the build
+        for f in os.scandir(tempfile.gettempdir()):
+            if os.path.isdir(f.path) and f.name.startswith(tmp_id):
+                tmp = f.path
+                break
+        else:
+            if setup_dir:
+                tmp = tempfile.mkdtemp(prefix=tmp_id)
+        return tmp
+
+    def set_do_images(self, val):
+        self.do_image = val
+
+    def set_exclude_images(self, val):
+        self.exclude_image = val
+
+    def set_do_set(self, val):
+        self.do_set = val
+
+    def _check_base(self, base_image):
+        if not base_image:
+            raise RebuilderError("Base image needs to be set.")
+
+    def _get_images(self) -> List:
+        images: List = []
+        if self.do_set:
+            # Use only the image sets the user asked for
+            for layer in self.do_set:
+                images += self._get_set_from_config(layer)
+        else:
+            # Go through all known layers and create a single image list
+            for (order, layer) in self.conf.layers.items():
+                i = getattr(self.conf, layer, [])
+                images += i
+        return self._filter_images(images)
+
+    def _filter_images(self, base: List) -> List:
+        if self.do_image:
+            return [i for i in base if i["component"] in self.do_image]
+        elif self.exclude_image:
+            return [i for i in base if i["component"] not in self.exclude_image]
+        else:
+            return base
+
+    def _prebuild_check(self, image_set: List, branches: List = None):
+        tmp = self._get_tmp_workdir(setup_dir=False)
+        if not tmp:
+            msg = "Temporary directory structure does not exist. Pull upstream first."
+            raise RebuilderError(msg)
+        self.logger.info("Checking for correct repository configuration ...")
+        releases = branches
+        for image in image_set:
+            component = image["component"]
+            cwd = os.path.join(tmp, component)
+            try:
+                repo = Repo(cwd)
+            except GitError as e:
+                self.logger.error("Failed to open repository for {}", component)
+                raise e
+            # This checks if any of the releases can be found in the name of the checked-out branch
+            if releases and not [i for i in releases if i in str(repo.active_branch)]:
+                msg = f"Unexpected active branch for {component}: {repo.active_branch}"
+                raise RebuilderError(msg)
+
+    def _build_images(self, image_set, custom_args: List = None, branches: List = None):
+        if not image_set:
+            # Nothing to build
+            self.logger.warn("No images to build, exiting.")
+            return
+        if not branches:
+            # Fill defaults from config if not provided
+            for release in self.conf.releases:
+                branches += [self.conf.releases[release]["current"]]
+        self._prebuild_check(image_set, branches)
+
+        procs = []
+        triggers = []
+        tmp = self._get_tmp_workdir(setup_dir=False)
+        for image in image_set:
+            component = image["component"]
+            cwd = os.path.join(tmp, component)
+            self.logger.info(f"Building image {component} ...")
+            args = [u._get_packager(self.conf), "container-build"]
+            if custom_args:
+                args.extend(custom_args)
+            proc = subprocess.Popen(args, cwd=cwd, stdout=subprocess.PIPE,
+                                    stderr=subprocess.PIPE,
+                                    universal_newlines=True)
+            # Append the process and component information for later use
+            procs.append((proc, image))
 
-    def _get_from_df(self, dockerfile_path):
-        res = None
-        if os.path.exists(dockerfile_path):
-            with open(dockerfile_path) as f:
-                fdata = f.read()
-            res = self._get_from(fdata)
-        return res
+        self.logger.info("Fetching tasks...")
+        for proc, image in procs:
+            component = image["component"]
+            self.logger.debug(f"Query component: {component}")
+            # Iterate until a taskID is found
+            for stdout in iter(proc.stdout.readline, ""):
+                if "taskID" in stdout:
+                    self.logger.info(f"{component} - {stdout.strip()}")
+                    break
+            else:
+                # If we get here the command must have failed
+                # The error will get printed out later when getting all builds
+                self.logger.warning(f"Could not find task for {component}!")
+
+        self.logger.info("Waiting for builds...")
+        timeout = 30
+        while procs:
+            self.logger.debug("Looping over all running builds")
+            for proc, image in procs:
+                out = err = None
+                component = image["component"]
+                try:
+                    self.logger.debug(f"Waiting {timeout} seconds for {component}")
+                    out, err = proc.communicate(timeout=timeout)
+                except subprocess.TimeoutExpired:
+                    msg = "{} not yet finished, checking next build"
+                    self.logger.debug(msg.format(component))
+                    self.logger.debug(f"{component} not yet finished, checking next build")
+                    continue
+                if proc.returncode != 0:
+                    self.logger.error(f"{component} build has failed")
+                else:
+                    self.logger.info(f"{component} build has finished")
+                    # If this image triggers a new layer, build it
+                    if "trigger" in image:
+                        triggers.append((component, image["trigger"]))
+
+                self.logger.info(f"{component} build has finished")
+                if err:
+                    # Write out stderr if we encounter an error
+                    err = u._4sp(err)
+                    self.logger.error(err)
+
+                procs.remove((proc, image))
+
+        for component, trigger in triggers:
+            msg = "Triggering layered builds on image %s..."
+            self.logger.info(msg, component)
+            self.build_images(trigger)
+
+    def _get_config_path(self, config: str) -> str:
+        if not os.path.isabs(config):
+            base_path = os.path.abspath(__file__)
+            dir_path = os.path.dirname(base_path)
+            path = os.path.join(dir_path, "config/", config)
+        else:
+            path = config
+        return path
 
-    def _get_from(self, fdata: str) -> str:
-        """Gets FROM field from a Dockerfile
+    def _not_yet_implemented(self):
+        print("Method not yet implemented.")
+
+    def get_brew_builds(self, print_time: bool = True) -> List[str]:
+        """Returns information about builds in brew
 
         Args:
-            fdata (str): String containing the Dockerfile
+            print_time (bool, optional): Print time finished for a build.
 
         Returns:
-            str: FROM string
+            str: Resulting brew build text
         """
-        registry_base = None
-        image_base = re.search('FROM (.*)\n', fdata)
-        if image_base:
-            registry_base = image_base.group(1)
-        return registry_base
+        output = []
+        header = "||Component||Build||Image_name||"
+        if print_time:
+            header += "Build finished||"
+        header += "Archives||"
+        output.append(header)
+        nvrs = (self.brewapi.get_nvrs(self._get_images()))
+        for item in nvrs:
+            nvr, name, component, *rest = item
+            # No nvr found for the image, might not have been built
+            if nvr is None:
+                continue
+            else:
+                template = "|{0}|{1}|{2}|"
+            vr = re.search(".*-([^-]*-[^-]*)$", nvr).group(1)
+            build_id = self.brewapi.get_buildinfo(nvr)["build_id"]
+            archives = self.brewapi.get_listarchives(build_id)
+            archive = archives[0]["extra"]
+            name = archive["docker"]["config"]["config"]["Labels"]["name"]
+            image_name = f"{name}:{vr}"
+            result = template.format(component, nvr, image_name)
+            if print_time:
+                result += self.brewapi.get_time_built(nvr) + '|'
+            result += str(len(archives))
+            output.append(result)
+        return output
 
-    def _set_from(self, fdata, from_tag):
+    def set_config(self, conf_name: str, release: str = "current"):
         """
-        Updates FROM field from a Dockerfile with value defined in configuration file
+        Use a configuration file other than the current one.
+        The configuration file used must be located in the standard 'config' directory.
 
-        Returns:
-            str: Dockerfile content with updated tag field
+        Args:
+            config(str): Name of the configuration file (filename)
+            release(str, optional): ID of the release to be used inside the config
         """
-        self.logger.debug("Setting tag to: " + str(from_tag))
-        base_image = self._get_from(fdata=fdata)
-        self.logger.debug(f"Base image is: {base_image}")
-        imagename_without_tag = base_image.split(':')[0]
-        ret = re.sub("FROM (.*)\n",
-                     f"FROM {imagename_without_tag}:{from_tag}\n", fdata)
-        return ret
-
-    def _update_variable_in_string(self, fdata: str = "", tag: str = "", tag_str: str = "", variable: str = ""):
-        """
-        Updates variable in string. Mainly used for updating test-openshift.yaml file.
-        It replaces VERSION: VERSION_NUMBER -> VERSION: variable and
-        It replaces OS: OS_VERSION -> OS: <os_name>"
-        """
-        self.logger.debug(f"Replaces variable of tag {tag} from {tag_str} to {variable}")
-        ret = re.sub(rf"{tag}: {tag_str}", f"{tag}: \"{variable}\"", fdata)
-        return ret
+        path = self._get_config_path(conf_name)
+        self.logger.debug("Setting config to {}", path)
+        with open(path) as f:
+            newconf = Config(f, release)
+        self.conf = newconf
+        # Set config for every module that is set up
+        if self.brewapi:
+            self.brewapi.conf = newconf
+        if self.distgit:
+            self.distgit.conf = newconf
 
-    def _update_test_openshift_yaml(self, test_openshift_yaml, version: str = "", short_name: str = ""):
+    def set_tmp_workdir(self, tmp: str):
         """
-        Update test/test-openshift.yaml file with value VERSION_NUMBER and OS_NUMBER
-        The file is used for CVP pipeline
+        Sets the temporary working directory to the one provided.
+        The directory has to already exist.
 
         Args:
-            test_openshift_yaml (Path): Path to test/test-openshift.yaml file
-            version (str): version to be replaced with VERSION_NUMBER
-            short_name (str): short_name to be replaced with CONTAINER_NAME
-        """
-        with open(test_openshift_yaml) as f:
-            fdata = f.read()
-        fdata = self._update_variable_in_string(fdata, "VERSION", "VERSION_NUMBER", version)
-        os_name = "fedora"
-        if self.conf.image_names == "RHEL8":
-            os_name = "rhel8"
-        if self.conf.image_names == "RHEL9":
-            os_name = "rhel9"
-        if self.conf.image_names == "RHSCL":
-            os_name = "rhel7"
-        fdata = self._update_variable_in_string(fdata, tag="OS", tag_str="OS_NUMBER", variable=os_name)
-        fdata = self._update_variable_in_string(fdata, tag="SHORT_NAME", tag_str="CONTAINER_NAME", variable=short_name)
-        with open(test_openshift_yaml, 'w') as f:
-            f.write(fdata)
-
-    def _update_dockerfile_rebuild(
-            self, dockerfile_path, from_tag, downstream_from: str = "",
-    ):
-        with open(dockerfile_path) as f:
-            fdata = f.read()
-        res = self._set_from(fdata, from_tag)
-        with open(dockerfile_path, 'w') as f:
-            f.write(res)
+            tmp(str): location of the directory to be used
+        """
+        if os.path.isdir(tmp):
+            self.tmp_workdir = os.path.abspath(tmp)
+        else:
+            raise RebuilderError("Provided working directory does not exist.")
 
-    def update_dockerfile(self, df, from_tag, downstream_from: str = ""):
-        """Updates basic fields of a Dockerfile. Sets from field
+    def set_commit_msg(self, msg: str):
+        """
+        Set the commit message to some other than the default one.
 
         Args:
-            df (str): Path to the Dockerfile
-            from_tag (str): value to be inserted into the from field
-            downstream_from (str): value from downstream Dockerfile
-        """
-        self._update_dockerfile_rebuild(
-            df, from_tag, downstream_from=downstream_from
-        )
-
-    # FIXME: This should be provided by some external Dockerfile linters
-    def _check_labels(self, dockerfile_path):
-        old_labels = ['Release=', 'Name=', 'Version=']
-        with open(dockerfile_path) as f:
-            fdata = f.read()
-        for label in old_labels:
-            if label in fdata:
-                self.logger.warn("Wrong label '{}' found in {}".format(label, dockerfile_path))
+            msg(str): Message to be written into the commit.
+        """
+        self.distgit.set_commit_msg(msg)
 
-    def check_script(self, component, script_path, component_path):
-        """Method that runs a given script against given directory
+    def clear_cache(self):
+        """Clears various caches used in the rebuilding process"""
 
-        Runs the script as provided by script_path and checks its exit value.
-        Prints the content of stderr when the sciprt fails (exit value != 0).
+        self.logger.info("Removing cached data and git storage.")
+        # Clear ondisk storage for git and the brew cache
+        tmp = self._get_tmp_workdir(setup_dir=False)
+        shutil.rmtree(tmp, ignore_errors=True)
+        # If the working directory has been set by the user, recreate it
+        if self.tmp_workdir:
+            os.makedirs(tmp)
+
+        # Clear koji object caches
+        self.nvrs = []
+        if self.brewapi:
+            self.brewapi.clear_cache()
 
-        Args:
-            component (string): name of the component being checked
-            script_path (string): script that should be run during the check
-            component_path (string): path to the directory being checked
-        """
-        template = "{name}: {status}"
-        ret = subprocess.run(script_path, shell=True, stderr=subprocess.PIPE,
-                             stdout=subprocess.DEVNULL, cwd=component_path)
-
-        if ret.returncode != 0:
-            self.logger.info(template.format(name=component, status="Affected"))
-            err = ret.stderr.decode('utf-8').strip()
-            if err:
-                self.logger.error(u._2sp(err))
-        else:
-            self.logger.info(template.format(name=component, status="OK"))
+    def set_repo_url(self, repo_url):
+        """Repofile url setter
 
-    def _do_git_reset(self, repo):
-        file_list = ['--', '.gitignore'] + self.conf.ignore_files
-        repo.git.reset(file_list)
-        # One file at a time to make sure all files get reset even on error
-        for f in file_list[1:]:
-            repo.git.checkout('--', f, with_exceptions=False)
-            self.logger.debug("Removing changes for: " + f)
-            # Remove all ignored files that are also untracked
-            untracked = repo.git.ls_files('-o').split('\n')
-            if f in untracked:
-                repo.git.clean('-xfd', f)
-                self.logger.debug("Removing untracked ignored file: " + f)
-
-    def get_commit_msg(self, rebase, image=None, ups_hash=None):
-        """Method to create a commit message to be used in git operations
-
-        Returns a general commit message depending on the value of the rebase
-        argument, or the user-specified commit message.
+        Sets the url of .repo file used for the build.
 
         Args:
-            rebase (bool): Specify if the rebase message is created
-            image (dict, optional): Metadata about the image being processed
-            ups_hash (str, optional): Upstream commit hash sources were synced from
-
-        Returns:
-            str: Resulting commit message text
+            repo_url: url of .repo file used for the build
         """
-        if self.commit_msg is not None:
-            return self.commit_msg
-        if rebase is True:
-            commit = "Rebuild for: {}".format(self.rebuild_reason)
-        elif rebase is False:
-            t = "Pull changes from upstream and rebase for: {}"
-            commit = t.format(self.rebuild_reason)
-        else:
-            t = "Unknown rebase argument provided: {}"
-            raise RebuilderError(t.format(str(rebase)))
-        if ups_hash:
-            commit += "\n created from upstream commit: " + ups_hash
-        return commit
+        self.repo_url = repo_url
 
-    def dist_git_changes(self, images, rebase=False):
-        """Method to merge changes from upstream into downstream
+    def list_images(self):
+        """Prints list of images that we work with"""
+        for i in self._get_images():
+            self.logger.info(i["component"])
+
+    def print_upstream(self):
+        """Prints the upstream name and url for images used in config"""
+        for i in self._get_images():
+            ups_name = re.search(r".*\/([a-zA-Z0-9-]+).git",
+                                 i["git_url"]).group(1)
+            msg = f"{i.get('component')} {i.get('name')} {ups_name} " \
+                  f"{i.get('git_url')} {i.get('git_path')} {i.get('git_branch')}"
+            self.logger.info(msg)
+
+    def show_config_contents(self):
+        """Prints the symbols and values of configuration used"""
+        for key in self.conf:
+            value = getattr(self.conf, key)
+            # Do not print clutter the output with unnecessary content
+            if key in ["raw"]:
+                continue
+            print(key + ":")
+            pprint.pprint(value, compact=True, width=256, indent=4)
+
+    def build_images(self, image_set=None):
+        """
+        Build images specified by image_set (or self.image_set)
+        """
+        if image_set is None and self.image_set is None:
+            raise RebuilderError("image_set is None, build cancelled.")
+        if image_set is None:
+            image_set = self.image_set
+        image_config = self._get_set_from_config(image_set)
+        images = self._filter_images(image_config)
+        self._build_images(images)
 
-        Pulls both downstream and upstream repositories into a temporary dir.
-        Merge is done by copying tracked files from upstream into downstream.
+    def print_brew_builds(self, print_time: bool = True):
+        """Prints information about builds in brew
 
         Args:
-            rebase (bool, optional): Specify if a rebase should be done instead
-        """
-        try:
-            for image in (images):
-                name = image["name"]
-                component = image["component"]
-                branch = image["git_branch"]
-                path = image["git_path"]
-                url = image["git_url"]
-                commands = image["commands"]
-                pull_upstr = image.get("pull_upstream", True)
-                repo = self._clone_downstream(component, branch)
-                df_path = os.path.join(component, "Dockerfile")
-                downstream_from = self._get_from_df(df_path)
-                self.logger.debug(f"Downstream_from: {downstream_from}\n")
-                from_tag = self.conf.get("from_tag", "latest")
-                if rebase or not pull_upstr:
-                    self.update_dockerfile(
-                        df_path, from_tag, downstream_from=downstream_from
-                    )
-                    # It is possible for the git repository to have no changes
-                    if repo.is_dirty():
-                        commit = self.get_commit_msg(rebase, image)
-                        if commit:
-                            repo.git.commit("-am", commit)
-                        else:
-                            msg = "Not creating new commit in: "
-                            self.logger.info(msg + component)
-                else:
-                    ups_name = name.split('-')[0]
-                    # Clone upstream repository
-                    ups_path = os.path.join('upstreams/', ups_name)
-                    self._clone_upstream(url, ups_path, commands=commands)
-                    # Save the upstream commit hash
-                    ups_hash = Repo(ups_path).commit().hexsha
-                    self._pull_upstream(component, path, url, repo, ups_name, commands)
-                    self.update_dockerfile(
-                        df_path, from_tag, downstream_from=downstream_from
-                    )
-                    repo.git.add("Dockerfile")
-                    # It is possible for the git repository to have no changes
-                    if repo.is_dirty():
-                        commit = self.get_commit_msg(rebase, image, ups_hash)
-                        if commit:
-                            repo.git.commit("-m", commit)
-                        else:
-                            msg = "Not creating new commit in: "
-                            self.logger.info(msg + component)
-
-                self._check_labels(df_path)
-        finally:
-            # Cleanup upstream repos
-            shutil.rmtree("upstreams", ignore_errors=True)
-
-    def _clone_upstream(self, url, ups_path, commands=None):
-        try:
-            repo = Repo.clone_from(url=url, to_path=ups_path)
-            self.logger.info("Cloned into: " + url)
-            for submodule in repo.submodules:
-                submodule.update(init=True)
-
-        except GitCommandError:
-            # Generally the directory already exists, try to open as a repo instead
-            # Throws InvalidGitRepositoryError if it is not a git repo
-            repo = Repo(ups_path)
-            self.logger.info("Using existing repository.")
-
-        # Run the commands either way
-        self.logger.debug("Running commands in upstream repo.")
-        # Need to be in the upstream git root, so change cwd
-        oldcwd = os.getcwd()
-        os.chdir(ups_path)
-        for order in sorted(commands):
-            cmd = commands[order]
-            self.logger.debug("Running '{o}' command '{c}'".format(o=order,
-                                                                   c=cmd))
-            ret = subprocess.run(cmd, stdout=subprocess.PIPE,
-                                 stderr=subprocess.PIPE, shell=True,
-                                 executable='/bin/bash')
-            if ret.returncode != 0:
-                msg = "'{c}' failed".format(c=cmd.split(" "))
-                self.logger.error(ret.stderr)
-                raise RebuilderError(msg)
-        os.chdir(oldcwd)
-        return repo
+            print_time (bool, optional): Print time finished for a build.
 
-    def _copy_upstream2downstream(self, src_parent, dest_parent):
-        """Copies content from upstream repo to downstream repo
-
-        Copies all files/dirs/symlinks from upstream source to dist-git one by one,
-        while removing previous if exists.
+        Returns:
+            str: Resulting brew build text
+        """
+        for builds in self.get_brew_builds(print_time=print_time):
+            self.logger.info(builds)
 
-        Args:
-            src_parent (string): path to source directory
-            dest_parent (string): path to destination directory
+    def pull_downstream(self):
         """
-        for f in os.listdir(src_parent):
-            dest = os.path.join(dest_parent, f)
-            src = os.path.join(src_parent, f)
-            # First remove the dest
-            if os.path.isdir(dest):
-                self.logger.debug("rmtree {}".format(dest))
-                shutil.rmtree(dest)
-            else:
-                u._remove_file(dest, self.logger)
+        Pulls downstream dist-git repositories and does not make any further changes to them
 
-            # Now copy the src to dest
-            if os.path.islink(src) or not os.path.isdir(src):
-                self.logger.debug("cp {} {}".format(src, dest))
-                shutil.copy2(src, dest, follow_symlinks=False)
-            else:
-                self.logger.debug("cp -r {} {}".format(src, dest))
-                shutil.copytree(src, dest, symlinks=True)
+        Additionally runs a script against each repository if check_script is set,
+        checking its exit value.
+        """
+        self._check_kerb_ticket()
+        tmp = self._get_tmp_workdir()
+        self._change_workdir(tmp)
+        images = self._get_images()
+        for i in images:
+            self.distgit._clone_downstream(i["component"], i["git_branch"])
+        # If check script is set, run the script provided for each config entry
+        if self.check_script:
+            for i in images:
+                self.distgit.check_script(i["component"], self.check_script,
+                                          i["git_branch"])
+
+    def pull_upstream(self):
+        """
+        Pulls upstream git repositories and does not make any further changes to them
+
+        Additionally runs a script against each repository if check_script is set,
+        checking its exit value.
+        """
+        tmp = self._get_tmp_workdir()
+        self._change_workdir(tmp)
+        images = self._get_images()
+        for i in images:
+            # Use unversioned name as a path for the repository
+            ups_name = i["name"].split('-')[0]
+            self.distgit._clone_upstream(i["git_url"],
+                                         ups_name,
+                                         commands=i["commands"])
+        # If check script is set, run the script provided for each config entry
+        if self.check_script:
+            for i in images:
+                ups_name = i["name"].split('-')[0]
+                self.distgit.check_script(i["component"], self.check_script,
+                                          os.path.join(ups_name, i["git_path"]))
 
-    def _handle_dangling_symlinks(self, src_parent, dest_parent):
-        """Replaces dangling symlinks in destination path with correct content
+    def push_changes(self):
+        """Pushes changes for all components into downstream dist-git repository"""
+        # Check for kerberos ticket
+        self._check_kerb_ticket()
+        tmp = self._get_tmp_workdir(setup_dir=False)
+        if not tmp:
+            msg = "Temporary directory structure does not exist. Pull upstream/rebase first."
+            raise RebuilderError(msg)
+        self._change_workdir(tmp)
+        images = self._get_images()
 
-        We need to remove downstream's (destination) dangling symlinks here,
-        because of files shared for more versions (s2i, root-common, test)
-        in upstream (source).
-        We do it by following first sources's symlink (not all symlinks) and
-        copying rest of the target to the destination.
+        self.distgit.push_changes(tmp, images)
 
-        Args:
-            src_parent (string): path to source directory
-            dest_parent (string): path to destination directory
+    def dist_git_rebase(self):
         """
-        for dest_root, dest_dirs, dest_files in os.walk(dest_parent):
-            for dest_file_name in dest_files:
-                dest_file = os.path.join(dest_root, dest_file_name)
-                # Look for danging symlinks to relative path, then copy the content
-                # from source, following the first symlink
-                if os.path.islink(dest_file) and not os.path.isabs(os.readlink(dest_file)):
-                    dest_target = os.path.join(os.path.dirname(dest_file), os.readlink(dest_file))
-                    msg = f"looking for dangling symlink {dest_file} (that points to {dest_target})"
-                    self.logger.debug(msg)
-                    if os.path.exists(dest_target):
-                        continue
-                    # We found a dangling symlink to relative path,
-                    # so we need to use the matching path in source,
-                    # which means removing destination name
-                    # from destination and adding it to source root
-                    dest_path_rel = re.sub(
-                        r"^{comp}{sep}".format(comp=dest_parent, sep=os.path.sep),
-                        "",
-                        dest_file
-                    )
-                    src_path_content = os.path.join(src_parent, dest_path_rel)
-                    self.logger.debug("unlink {dest}".format(dest=dest_file))
-                    os.unlink(dest_file)
-                    src_full = os.path.join(os.path.dirname(src_path_content),
-                                            os.readlink(src_path_content))
-                    if os.path.isdir(src_full):
-                        # In this case, when the source directory includes another symlinks outside
-                        # of this directory, those wouldn't be fixed, so let's run the same function
-                        # to fix dangling symlinks recursively.
-                        self.logger.debug("cp -r {src} {dest}".format(src=src_full, dest=dest_file))
-                        shutil.copytree(src_full, dest_file, symlinks=True)
-                        self._handle_dangling_symlinks(src_parent, dest_parent)
-                    else:
-                        self.logger.debug("cp {src} {dest}".format(src=src_full, dest=dest_file))
-                        shutil.copy2(src_full, dest_file, follow_symlinks=False)
-
-    def _pull_upstream(self, component, path, url, repo, ups_name, commands):
-        """Pulls an upstream repo and copies it into downstream"""
-        ups_path = os.path.join('upstreams/', ups_name)
-        cp_path = os.path.join(ups_path, path)
-
-        # First check if there is a version upstream
-        # If not we just skip the whole copy action
-        if not os.path.exists(cp_path):
-            msg = "Source {} does not exist, skipping copy upstream."
-            self.logger.warning(msg.format(cp_path))
-            return
-
-        for f in repo.git.ls_files().split('\n'):
-            file = os.path.join(component, f)
-            if os.path.isdir(file) and not os.path.islink(file):
-                shutil.rmtree(file)
-            else:
-                os.remove(file)
+        Do a rebase against a new base/s2i image.
+        Does not pull in upstream changes of layered images.
+        """
+        self.dist_git_changes(rebase=True)
 
-        # No need for upstream .git files so we remove them
-        shutil.rmtree(os.path.join(ups_path, path, '.git'), ignore_errors=True)
-        self._copy_upstream2downstream(cp_path, component)
-        self._handle_dangling_symlinks(cp_path, component)
-        # If README.md exists but help.md does not, create a symlink
-        help_md = os.path.join(component, "help.md")
-        readme_md = os.path.join(component, "README.md")
-        if not os.path.isfile(help_md):
-            if os.path.isfile(readme_md):
-                os.symlink('README.md', help_md)
-                repo.git.add('help.md')
-            else:
-                # Report warning if help.md does not exists
-                self.logger.warn("help.md file missing")
-        # Add all the changes and remove those we do not want
-        test_openshift_yaml_file = os.path.join(component, "test", "test-openshift.yaml")
-        if os.path.exists(test_openshift_yaml_file):
-            self._update_test_openshift_yaml(test_openshift_yaml_file, path, short_name=ups_name)
-
-        repo.git.add("*")
-        self._do_git_reset(repo)
-        # TODO: Configurable?
-        df_ext = self.df_ext
-        df_path = os.path.join(component, "Dockerfile")
-        if os.path.isfile(df_path + df_ext) and not os.path.islink(df_path + df_ext):
-            try:
-                os.remove(df_path)
-            except FileNotFoundError:
-                # We don't care whether CentOS dockerfile exists or not. Just don't fail here.
-                pass
-            repo.git.mv("Dockerfile" + df_ext, "Dockerfile")
-            os.symlink("Dockerfile", df_path + df_ext)
-            repo.git.add("Dockerfile", "Dockerfile" + df_ext)
-
-        # Make sure a $VERSION symlink exists
-        repo = Repo(component)
-        version = os.path.basename(cp_path)
-        link_name = os.path.join(component, version)
-        if not os.path.islink(link_name):
-            try:
-                os.symlink(".", link_name)
-                repo.git.add(version)
-            except FileExistsError:  # noqa: F821 - Doesnt see built-ins?
-                t = "Failed creating symlink '{}' -> '.', file already exists."
-                raise u.RebuilderError(t.format(link_name))
-
-        # Run post upstream pull hook
-        self._post_upstream_pull(cp_path, component)
-
-    def _post_upstream_pull(sefl, upstream_path, downstream_path):
-        """Post upstream pull hook"""
-        pass
-
-    def _clone_downstream(self, component, branch):
-        """Clones downstream dist-git repo"""
-        # Do not set up downstream repo if it already exists
-        if os.path.isdir(component):
-            self.logger.info("Using existing downstream repo: " + component)
-            repo = Repo(component)
-        else:
-            hostname_url = u._get_hostname_url(self.conf)
-            packager = u._get_packager(self.conf)
-            # if packager is fedpkg then namespace is `container` else `containers`
-            namespace = "container" if packager == "fedpkg" else "containers"
-            component_path = f"{namespace}/{component}"
-            # If hostname_url is specified use `git` otherwise `packager` command.
-            if hostname_url:
-                cmd = "git"
-                ccomponent = f"{hostname_url}/{component_path}.git"
-            else:
-                cmd = packager
-                ccomponent = component_path
+    def dist_git_changes(self, rebase: bool = False):
+        """Method to merge changes from upstream into downstream
 
-            self.logger.info("Cloning into: " + ccomponent)
-            ret = subprocess.run([cmd, "clone", ccomponent],
-                                 stdout=subprocess.DEVNULL,
-                                 stderr=subprocess.DEVNULL)
-            # If the clone failed, try once again with the containers prefix
-            if ret.returncode != 0:
-                template = "{} failed to clone {} with return value {}."
-                raise RebuilderError(template.format(cmd, component,
-                                                     ret.returncode))
-
-            repo = Repo(component)
-            repo.git.checkout(branch)
-        return repo
-
-    def _get_unpushed_commits(self, repo):
-        """
-        Get unpushed commits
-        :param repo: repo name to check for unpushed commits
-        :return: List of commits or empty array
-        """
-        branch = repo.active_branch.name
-        # Get a list of commits that have not been pushed to remote
-        select = "origin/" + branch + ".." + branch
-        commits = [i for i in repo.iter_commits(select)]
-        return commits
+        Pulls both downstream and upstream repositories into a temporary directory.
+        Merge is done by copying tracked files from upstream into downstream.
 
-    def push_changes(self, tmp, images):
-        """Pushes changes for components into downstream dist-git repository"""
+        Args:
+            rebase (bool, optional): Specifies whether a rebase should be done instead.
+        """
         # Check for kerberos ticket
-        failed = []
-        for image in images:
-            component = image["component"]
-            try:
-                repo = Repo(component)
-                # If a commit message is provided do a commit first
-                if self.commit_msg and repo.is_dirty():
-                    # commit_msg is set so it is always returned
-                    commit = self.get_commit_msg(None, image)
-                    repo.git.commit("-am", commit)
-                if self._get_unpushed_commits(repo):
-                    self.logger.info("Pushing: " + component)
-
-                    repo.git.push()
-                else:
-                    self.logger.info(f"There are no unpushed commits."
-                                     f" Push skipped for {component}.")
-            except GitCommandError as e:
-                failed.append(image)
-                self.logger.error(e)
-
-        if failed:
-            self.logger.error("Failed pushing images:")
-            for image in failed:
-                self.logger.error(u._2sp(image["component"]))
-            self.logger.error("Please check the failures and push the changes manually.")
+        self._check_kerb_ticket()
+        tmp = self._get_tmp_workdir()
+        self._change_workdir(tmp)
+        images = self._get_images()
+        self.distgit.dist_git_changes(images, rebase)
+        self.logger.info("\nGit location: " + tmp)
+        if self.args:
+            tmp_str = ' --tmp ' + self.tmp_workdir if self.tmp_workdir else '"'
+            self.logger.info("You can view changes made by running:")
+            self.logger.info(f"cwt --base {self.base_image} {tmp_str} git show")
+        if self.args:
+            self.logger.info(
+                "To push and build run:"
+                "cwt git push && cwt build"
+                "[base/core/s2i] --repo-url link-to-repo-file")
 
-    # TODO: Multiple future branches?
-    def merge_future_branches(self, images):
+    def merge_future_branches(self):
         """Merges current branch with future branches"""
         # Check for kerberos ticket
-        failed = []
-        for image in images:
-            component = image["component"]
-            branch = image["git_branch"]
-            # TODO: config only has one future branch
-            fb_list = [image["git_future"]]
-            repo = self._clone_downstream(component, branch)
-            for fb in fb_list:
-                try:
-                    repo.git.checkout(fb)
-                    repo.git.merge(branch)
-                    # print("Pushing into: {}".format(res))
-                    self.logger.info("NOT Pushing into: {}".format(fb))
-                    # repo.git.push()
-                except GitCommandError as e:
-                    failed.append(image)
-                    self.logger.error(e)
-                    continue
-        if failed:
-            self.logger.error("Failed merging images:")
-            for image in failed:
-                self.logger.error(u._2sp(image["component"]))
-            self.logger.error("Please check the failures and push the changes manually.")
+        self._check_kerb_ticket()
+        tmp = self._get_tmp_workdir()
+        self._change_workdir(tmp)
+        images = self._get_images()
+        self.distgit.merge_future_branches(images)
 
-    def show_git_changes(self, tmp, components=None, diff=False):
+    def show_git_changes(self, components: List = None):
         """Shows changes made to tracked files in local downstream repositories
 
-        Walks through all repositories and calls 'git-show' or 'git-diff' on each of them.
-
         Args:
-            tmp (str): Path to the directory that is used to store git repositories
             components (list of str, optional): List of components to show changes for
-            diff (boolean, optional): Controls whether the method calls git-show or git-diff
+        Walks through all downstream repositories and calls 'git-show' on each of them.
         """
-        # Function to check if a path contains a git repository
-        def is_git(x): return os.path.isdir(os.path.join(x, '.git'))
-        files = None
-        command = 'diff' if diff else 'show'
-        # Create a list of repository paths
         if not components:
-            # Get the whole subdirectory
-            files = [f.path for f in os.scandir(tmp) if is_git(f.path)]
-        elif isinstance(components, list):
-            files = [path for path in [os.path.join(tmp, c) for c in components] if is_git(path)]
-        elif isinstance(components, str) and is_git(os.path.join(tmp, components)):
-            files = [os.path.join(tmp, components)]
-        else:
-            raise u.RebuilderError("Unknown component: {}".format(str(components)))
-        if not files:
-            self.logger.warn("No git repositories found in directory " + tmp)
-        # Walk through the repositories and show changes made in the last commit
-        for path in files:
-            repo = Repo(path)
-            # Only show changes if there are unpushed commits to show
-            # or we only want the diff of unstaged changes
-            if self._get_unpushed_commits(repo) or diff:
-                # Clears the screen
-                print(chr(27) + "[2J")
-                # Force pager for short git diffs
-                subprocess.run(
-                    "git config core.pager 'less -+F' --replace-all",
-                    cwd=path,
-                    shell=True
-                )
-                # Not using GitPython as its git.show seems to have some problems with encoding
-                subprocess.run(['git', command], cwd=path)
+            images = self._get_images()
+            components = [i["component"] for i in images]
+        tmp = self._get_tmp_workdir()
+        self._change_workdir(tmp)
+        self.distgit.show_git_changes(tmp, components)
```

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/koji.py` & `container-workflow-tool-1.5.3/container_workflow_tool/koji.py`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool/utility.py` & `container-workflow-tool-1.5.3/container_workflow_tool/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 def _get_hostname_url(config) -> str:
     # Try to read which packager to use from the config file
     # default to "https://src.fedoraproject.org"
     git_url = getattr(config, "hostname_url", None)
     return git_url
 
 
-def _split_config_path(config: str) -> (str, str):
+def _split_config_path(config: str):
     conf = config.split(':')
     if len(conf) > 2:
         raise RebuilderError("You can only use one image_set argument with the --config option.")
     config_path = conf[0]
     image_set = conf[1] if len(conf) > 1 else 'current'
     return config_path, image_set
```

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool.egg-info/PKG-INFO` & `container-workflow-tool-1.5.3/container_workflow_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: container-workflow-tool
-Version: 1.5.2
+Version: 1.5.3
 Summary: A python3 tool to make rebuilding images easier by automating several steps of the process.
 Home-page: https://github.com/sclorg/container-workflow-tool
 Author: Petr Kubat
 Author-email: pkubat@redhat.com
 License: MIT
 Keywords: tool,containers,images,automate,workflow
 Classifier: Development Status :: 4 - Beta
```

### Comparing `container-workflow-tool-1.5.2/container_workflow_tool.egg-info/SOURCES.txt` & `container-workflow-tool-1.5.3/container_workflow_tool.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 setup.py
 container_workflow_tool/__init__.py
 container_workflow_tool/cli.py
 container_workflow_tool/cli_common.py
 container_workflow_tool/config.py
 container_workflow_tool/constants.py
 container_workflow_tool/distgit.py
+container_workflow_tool/dockerfile.py
+container_workflow_tool/git_operations.py
 container_workflow_tool/koji.py
 container_workflow_tool/main.py
+container_workflow_tool/sync.py
 container_workflow_tool/utility.py
 container_workflow_tool.egg-info/PKG-INFO
 container_workflow_tool.egg-info/SOURCES.txt
 container_workflow_tool.egg-info/dependency_links.txt
 container_workflow_tool.egg-info/entry_points.txt
 container_workflow_tool.egg-info/requires.txt
 container_workflow_tool.egg-info/top_level.txt
@@ -28,8 +31,16 @@
 container_workflow_tool/config/f31.yaml
 container_workflow_tool/config/f32.yaml
 container_workflow_tool/config/f33.yaml
 container_workflow_tool/config/f34.yaml
 container_workflow_tool/config/rawhide.yaml
 container_workflow_tool/config/share/cwt_config.yaml
 container_workflow_tool/config/share/urls.yaml
-man/cwt.1
+man/cwt.1
+tests/test_brew.py
+tests/test_cli.py
+tests/test_distgit.py
+tests/test_dockerfile.py
+tests/test_git_operations.py
+tests/test_print.py
+tests/test_rebuilder.py
+tests/test_utility.py
```

### Comparing `container-workflow-tool-1.5.2/man/cwt.1` & `container-workflow-tool-1.5.3/man/cwt.1`

 * *Files identical despite different names*

### Comparing `container-workflow-tool-1.5.2/setup.py` & `container-workflow-tool-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
 # The MIT License (MIT)
 #
-# Copyright (c) 2016-2021 CWT Authors
+# Copyright (c) 2016-2023 CWT Authors
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -54,15 +54,15 @@
         if system_path is None:
             system_path = []
     return os.path.join(*(['/'] + system_path))
 
 
 setup(
     name='container-workflow-tool',
-    version="1.5.2",
+    version="1.5.3",
     description='A python3 tool to make rebuilding images easier by automating several steps of the process.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='tool,containers,images,automate, workflow',
     author='Petr Kubat',
     author_email='pkubat@redhat.com',
     url='https://github.com/sclorg/container-workflow-tool',
```

