# Comparing `tmp/dcrx-0.0.4.tar.gz` & `tmp/dcrx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-0.0.4.tar", last modified: Wed Jun  7 16:00:47 2023, max compression
+gzip compressed data, was "dcrx-0.0.5.tar", last modified: Wed Jun  7 19:02:44 2023, max compression
```

## Comparing `dcrx-0.0.4.tar` & `dcrx-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.248116 dcrx-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 16:00:37.000000 dcrx-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-07 16:00:47.248116 dcrx-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-07 16:00:37.000000 dcrx-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.244115 dcrx-0.0.4/dcrx/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.248116 dcrx-0.0.4/dcrx/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/expose.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.248116 dcrx-0.0.4/dcrx/layers/mount_types/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/bind_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/cache_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/secret_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/ssh_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/mount_types/tmpfs_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/layers/workdir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.248116 dcrx-0.0.4/dcrx/memory_file/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/memory_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 16:00:37.000000 dcrx-0.0.4/dcrx/memory_file/memory_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:00:47.244115 dcrx-0.0.4/dcrx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-07 16:00:47.000000 dcrx-0.0.4/dcrx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-07 16:00:47.000000 dcrx-0.0.4/dcrx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:00:47.000000 dcrx-0.0.4/dcrx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 16:00:47.000000 dcrx-0.0.4/dcrx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 16:00:47.000000 dcrx-0.0.4/dcrx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:00:47.248116 dcrx-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-07 16:00:37.000000 dcrx-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.431843 dcrx-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 19:02:41.000000 dcrx-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-07 19:02:44.431843 dcrx-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-07 19:02:41.000000 dcrx-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.427842 dcrx-0.0.5/dcrx/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.427842 dcrx-0.0.5/dcrx/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/expose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.427842 dcrx-0.0.5/dcrx/layers/mount_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/bind_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/cache_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/secret_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/ssh_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/tmpfs_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/workdir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.431843 dcrx-0.0.5/dcrx/memory_file/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/memory_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/memory_file/memory_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.427842 dcrx-0.0.5/dcrx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-07 19:02:44.000000 dcrx-0.0.5/dcrx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-07 19:02:44.000000 dcrx-0.0.5/dcrx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:02:44.000000 dcrx-0.0.5/dcrx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 19:02:44.000000 dcrx-0.0.5/dcrx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 19:02:44.000000 dcrx-0.0.5/dcrx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:02:44.431843 dcrx-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-07 19:02:41.000000 dcrx-0.0.5/setup.py
```

### Comparing `dcrx-0.0.4/LICENSE` & `dcrx-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.4/PKG-INFO` & `dcrx-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dcrx
-Version: 0.0.4
-Summary: Easy project setup and migration.
+Version: 0.0.5
+Summary: A library for typesafe, programmatic generation of Docker images via SQL-builder like API.
 Home-page: https://github.com/scorbettUM/dcrx
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dcrx-0.0.4/README.md` & `dcrx-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.4/dcrx/image.py` & `dcrx-0.0.5/dcrx/image.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.4/dcrx/layers/add.py` & `dcrx-0.0.5/dcrx/layers/add.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.4/dcrx/layers/copy.py` & `dcrx-0.0.5/dcrx/layers/copy.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.4/dcrx/layers/mount_types/bind_mount.py` & `dcrx-0.0.5/dcrx/layers/mount_types/bind_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.4/dcrx/layers/mount_types/cache_mount.py` & `dcrx-0.0.5/dcrx/layers/mount_types/cache_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.4/dcrx/layers/mount_types/secret_mount.py` & `dcrx-0.0.5/dcrx/layers/mount_types/secret_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.4/dcrx/layers/mount_types/ssh_mount.py` & `dcrx-0.0.5/dcrx/layers/mount_types/ssh_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.4/dcrx/layers/run.py` & `dcrx-0.0.5/dcrx/layers/run.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.4/dcrx.egg-info/PKG-INFO` & `dcrx-0.0.5/dcrx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dcrx
-Version: 0.0.4
-Summary: Easy project setup and migration.
+Version: 0.0.5
+Summary: A library for typesafe, programmatic generation of Docker images via SQL-builder like API.
 Home-page: https://github.com/scorbettUM/dcrx
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dcrx-0.0.4/dcrx.egg-info/SOURCES.txt` & `dcrx-0.0.5/dcrx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.4/setup.py` & `dcrx-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 version_string = ""
 with open (os.path.join(current_directory, ".version"), 'r') as version_file:
     version_string = version_file.read()
 
 setup(
     name="dcrx",
     version=version_string,
-    description="Easy project setup and migration.",
+    description="A library for typesafe, programmatic generation of Docker images via SQL-builder like API.",
     long_description=package_description,
     long_description_content_type="text/markdown",
     author="Sean Corbett",
     author_email="sean.corbett@umontana.edu",
     url="https://github.com/scorbettUM/dcrx",
     packages=find_packages(),
     keywords=[
```

