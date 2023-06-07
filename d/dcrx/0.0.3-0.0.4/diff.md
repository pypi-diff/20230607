# Comparing `tmp/dcrx-0.0.3.tar.gz` & `tmp/dcrx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-0.0.3.tar", last modified: Wed Jun  7 15:58:49 2023, max compression
+gzip compressed data, was "dcrx-0.0.4.tar", last modified: Wed Jun  7 16:00:47 2023, max compression
```

## Comparing `dcrx-0.0.3.tar` & `dcrx-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:58:49.172131 dcrx-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 15:58:46.000000 dcrx-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-07 15:58:49.172131 dcrx-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-07 15:58:46.000000 dcrx-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:58:49.172131 dcrx-0.0.3/dcrx/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:58:49.172131 dcrx-0.0.3/dcrx/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/expose.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:58:49.172131 dcrx-0.0.3/dcrx/layers/mount_types/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/mount_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/mount_types/bind_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/mount_types/cache_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/mount_types/secret_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/mount_types/ssh_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/mount_types/tmpfs_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/layers/workdir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:58:49.172131 dcrx-0.0.3/dcrx/memory_file/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/memory_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 15:58:46.000000 dcrx-0.0.3/dcrx/memory_file/memory_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:58:49.172131 dcrx-0.0.3/dcrx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-07 15:58:49.000000 dcrx-0.0.3/dcrx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-07 15:58:49.000000 dcrx-0.0.3/dcrx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:58:49.000000 dcrx-0.0.3/dcrx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 15:58:49.000000 dcrx-0.0.3/dcrx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 15:58:49.000000 dcrx-0.0.3/dcrx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:58:49.172131 dcrx-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-07 15:58:46.000000 dcrx-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.248116 dcrx-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 16:00:37.000000 dcrx-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-07 16:00:47.248116 dcrx-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-07 16:00:37.000000 dcrx-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.244115 dcrx-0.0.4/dcrx/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.248116 dcrx-0.0.4/dcrx/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/expose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.248116 dcrx-0.0.4/dcrx/layers/mount_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/bind_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/cache_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/secret_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/ssh_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/tmpfs_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/workdir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.248116 dcrx-0.0.4/dcrx/memory_file/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/memory_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/memory_file/memory_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.244115 dcrx-0.0.4/dcrx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-07 16:00:47.000000 dcrx-0.0.4/dcrx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-07 16:00:47.000000 dcrx-0.0.4/dcrx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:00:47.000000 dcrx-0.0.4/dcrx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 16:00:47.000000 dcrx-0.0.4/dcrx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 16:00:47.000000 dcrx-0.0.4/dcrx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:00:47.248116 dcrx-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-07 16:00:37.000000 dcrx-0.0.4/setup.py
```

### Comparing `dcrx-0.0.3/LICENSE` & `dcrx-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.3/PKG-INFO` & `dcrx-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,14 @@
-Metadata-Version: 2.1
-Name: dcrx
-Version: 0.0.3
-Summary: Easy project setup and migration.
-Home-page: https://github.com/scorbettUM/dcrx
-Author: Sean Corbett
-Author-email: sean.corbett@umontana.edu
-Keywords: pypi,cicd,python,setup,docker,infra,devops
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dcrx
+[![PyPI version](https://img.shields.io/pypi/v/dcrx?color=gre)](https://pypi.org/project/dcrx/)
+[![License](https://img.shields.io/github/license/scorbettUM/dcrx)](https://github.com/scorbettUM/dcrx/blob/main/LICENSE)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx/blob/main/CODE_OF_CONDUCT.md)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx)](https://pypi.org/project/dcrx/)
+
+
 DockerX (dcrx) is a library for creating Docker images via an SQL query-builder like API. It is designed to facilitate programmatic, typesafe, and in-memory image generation. dcrx is *not* a wrapper around the Docker CLI or API, nor is it an implementation of these things. Rather, it is designed a lightweight, single-dependency means of writing and creating images that can then be provided to the Docker CLI or SDK for consumption.
 
 
 # Setup and Install
 
 dcrx is available via PyPi as an installable package. We recommend using Python 3.10+ and a virtual environment. To install dcrx, run:
```

### Comparing `dcrx-0.0.3/dcrx/image.py` & `dcrx-0.0.4/dcrx/image.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.3/dcrx/layers/add.py` & `dcrx-0.0.4/dcrx/layers/add.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.3/dcrx/layers/copy.py` & `dcrx-0.0.4/dcrx/layers/copy.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.3/dcrx/layers/mount_types/bind_mount.py` & `dcrx-0.0.4/dcrx/layers/mount_types/bind_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.3/dcrx/layers/mount_types/cache_mount.py` & `dcrx-0.0.4/dcrx/layers/mount_types/cache_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.3/dcrx/layers/mount_types/secret_mount.py` & `dcrx-0.0.4/dcrx/layers/mount_types/secret_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.3/dcrx/layers/mount_types/ssh_mount.py` & `dcrx-0.0.4/dcrx/layers/mount_types/ssh_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.3/dcrx/layers/run.py` & `dcrx-0.0.4/dcrx/layers/run.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.3/dcrx.egg-info/PKG-INFO` & `dcrx-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx
-Version: 0.0.3
+Version: 0.0.4
 Summary: Easy project setup and migration.
 Home-page: https://github.com/scorbettUM/dcrx
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dcrx
+[![PyPI version](https://img.shields.io/pypi/v/dcrx?color=gre)](https://pypi.org/project/dcrx/)
+[![License](https://img.shields.io/github/license/scorbettUM/dcrx)](https://github.com/scorbettUM/dcrx/blob/main/LICENSE)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx/blob/main/CODE_OF_CONDUCT.md)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx)](https://pypi.org/project/dcrx/)
+
+
 DockerX (dcrx) is a library for creating Docker images via an SQL query-builder like API. It is designed to facilitate programmatic, typesafe, and in-memory image generation. dcrx is *not* a wrapper around the Docker CLI or API, nor is it an implementation of these things. Rather, it is designed a lightweight, single-dependency means of writing and creating images that can then be provided to the Docker CLI or SDK for consumption.
 
 
 # Setup and Install
 
 dcrx is available via PyPi as an installable package. We recommend using Python 3.10+ and a virtual environment. To install dcrx, run:
```

### Comparing `dcrx-0.0.3/dcrx.egg-info/SOURCES.txt` & `dcrx-0.0.4/dcrx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.3/setup.py` & `dcrx-0.0.4/setup.py`

 * *Files identical despite different names*

