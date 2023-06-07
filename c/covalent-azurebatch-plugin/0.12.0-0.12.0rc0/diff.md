# Comparing `tmp/covalent-azurebatch-plugin-0.12.0.tar.gz` & `tmp/covalent-azurebatch-plugin-0.12.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-azurebatch-plugin-0.12.0.tar", last modified: Wed Jun  7 21:02:32 2023, max compression
+gzip compressed data, was "covalent-azurebatch-plugin-0.12.0rc0.tar", last modified: Wed Jun  7 20:47:12 2023, max compression
```

## Comparing `covalent-azurebatch-plugin-0.12.0.tar` & `covalent-azurebatch-plugin-0.12.0rc0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 willcunningham   (501) staff       (20)        0 2023-06-07 21:02:32.178620 covalent-azurebatch-plugin-0.12.0/
--rw-r--r--   0 willcunningham   (501) staff       (20)    34523 2023-05-29 17:44:19.000000 covalent-azurebatch-plugin-0.12.0/LICENSE
--rw-r--r--   0 willcunningham   (501) staff       (20)       91 2023-06-07 20:33:14.000000 covalent-azurebatch-plugin-0.12.0/MANIFEST.in
--rw-r--r--   0 willcunningham   (501) staff       (20)     6493 2023-06-07 21:02:32.178445 covalent-azurebatch-plugin-0.12.0/PKG-INFO
--rw-r--r--   0 willcunningham   (501) staff       (20)     5165 2023-06-07 20:34:11.000000 covalent-azurebatch-plugin-0.12.0/README.md
--rw-r--r--   0 willcunningham   (501) staff       (20)        7 2023-06-07 20:34:23.000000 covalent-azurebatch-plugin-0.12.0/VERSION
-drwxr-xr-x   0 willcunningham   (501) staff       (20)        0 2023-06-07 21:02:32.175588 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/
--rw-r--r--   0 willcunningham   (501) staff       (20)      835 2023-05-29 17:44:19.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/__init__.py
-drwxr-xr-x   0 willcunningham   (501) staff       (20)        0 2023-06-07 21:02:32.173875 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/
-drwxr-xr-x   0 willcunningham   (501) staff       (20)        0 2023-06-07 21:02:32.178190 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/
--rw-r--r--   0 willcunningham   (501) staff       (20)     1334 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/Dockerfile
--rw-r--r--   0 willcunningham   (501) staff       (20)     3849 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/exec.py
--rw-r--r--   0 willcunningham   (501) staff       (20)     3115 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/iam.tf
--rw-r--r--   0 willcunningham   (501) staff       (20)     2962 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/main.tf
--rw-r--r--   0 willcunningham   (501) staff       (20)     1706 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/outputs.tf
--rw-r--r--   0 willcunningham   (501) staff       (20)     1908 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/storage.tf
--rw-r--r--   0 willcunningham   (501) staff       (20)     1480 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/variables.tf
--rw-r--r--   0 willcunningham   (501) staff       (20)      993 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/versions.tf
--rw-r--r--   0 willcunningham   (501) staff       (20)    16633 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/azurebatch.py
--rw-r--r--   0 willcunningham   (501) staff       (20)     1279 2023-05-29 17:44:19.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/exceptions.py
--rw-r--r--   0 willcunningham   (501) staff       (20)     1287 2023-05-29 17:44:19.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/utils.py
-drwxr-xr-x   0 willcunningham   (501) staff       (20)        0 2023-06-07 21:02:32.176798 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin.egg-info/
--rw-r--r--   0 willcunningham   (501) staff       (20)     6493 2023-06-07 21:02:32.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin.egg-info/PKG-INFO
--rw-r--r--   0 willcunningham   (501) staff       (20)      938 2023-06-07 21:02:32.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 willcunningham   (501) staff       (20)        1 2023-06-07 21:02:32.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 willcunningham   (501) staff       (20)       88 2023-06-07 21:02:32.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin.egg-info/entry_points.txt
--rw-r--r--   0 willcunningham   (501) staff       (20)       92 2023-06-07 21:02:32.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin.egg-info/requires.txt
--rw-r--r--   0 willcunningham   (501) staff       (20)       27 2023-06-07 21:02:32.000000 covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin.egg-info/top_level.txt
--rw-r--r--   0 willcunningham   (501) staff       (20)     1238 2023-05-29 17:44:19.000000 covalent-azurebatch-plugin-0.12.0/pyproject.toml
--rw-r--r--   0 willcunningham   (501) staff       (20)      928 2023-06-07 20:34:48.000000 covalent-azurebatch-plugin-0.12.0/requirements.txt
--rw-r--r--   0 willcunningham   (501) staff       (20)       38 2023-06-07 21:02:32.178667 covalent-azurebatch-plugin-0.12.0/setup.cfg
--rw-r--r--   0 willcunningham   (501) staff       (20)     2874 2023-06-07 20:35:12.000000 covalent-azurebatch-plugin-0.12.0/setup.py
+drwxr-xr-x   0 willcunningham   (501) staff       (20)        0 2023-06-07 20:47:12.348393 covalent-azurebatch-plugin-0.12.0rc0/
+-rw-r--r--   0 willcunningham   (501) staff       (20)    34523 2023-05-29 17:44:19.000000 covalent-azurebatch-plugin-0.12.0rc0/LICENSE
+-rw-r--r--   0 willcunningham   (501) staff       (20)       91 2023-06-07 20:33:14.000000 covalent-azurebatch-plugin-0.12.0rc0/MANIFEST.in
+-rw-r--r--   0 willcunningham   (501) staff       (20)     6496 2023-06-07 20:47:12.348217 covalent-azurebatch-plugin-0.12.0rc0/PKG-INFO
+-rw-r--r--   0 willcunningham   (501) staff       (20)     5165 2023-06-07 20:34:11.000000 covalent-azurebatch-plugin-0.12.0rc0/README.md
+-rw-r--r--   0 willcunningham   (501) staff       (20)        7 2023-06-07 20:34:23.000000 covalent-azurebatch-plugin-0.12.0rc0/VERSION
+drwxr-xr-x   0 willcunningham   (501) staff       (20)        0 2023-06-07 20:47:12.345603 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/
+-rw-r--r--   0 willcunningham   (501) staff       (20)      835 2023-05-29 17:44:19.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/__init__.py
+drwxr-xr-x   0 willcunningham   (501) staff       (20)        0 2023-06-07 20:47:12.343493 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/
+drwxr-xr-x   0 willcunningham   (501) staff       (20)        0 2023-06-07 20:47:12.348002 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/
+-rw-r--r--   0 willcunningham   (501) staff       (20)     1334 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/Dockerfile
+-rw-r--r--   0 willcunningham   (501) staff       (20)     3849 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/exec.py
+-rw-r--r--   0 willcunningham   (501) staff       (20)     3115 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/iam.tf
+-rw-r--r--   0 willcunningham   (501) staff       (20)     2962 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/main.tf
+-rw-r--r--   0 willcunningham   (501) staff       (20)     1706 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/outputs.tf
+-rw-r--r--   0 willcunningham   (501) staff       (20)     1908 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/storage.tf
+-rw-r--r--   0 willcunningham   (501) staff       (20)     1480 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/variables.tf
+-rw-r--r--   0 willcunningham   (501) staff       (20)      993 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/versions.tf
+-rw-r--r--   0 willcunningham   (501) staff       (20)    16633 2023-06-07 20:31:17.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/azurebatch.py
+-rw-r--r--   0 willcunningham   (501) staff       (20)     1279 2023-05-29 17:44:19.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/exceptions.py
+-rw-r--r--   0 willcunningham   (501) staff       (20)     1287 2023-05-29 17:44:19.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/utils.py
+drwxr-xr-x   0 willcunningham   (501) staff       (20)        0 2023-06-07 20:47:12.346633 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin.egg-info/
+-rw-r--r--   0 willcunningham   (501) staff       (20)     6496 2023-06-07 20:47:12.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 willcunningham   (501) staff       (20)      938 2023-06-07 20:47:12.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 willcunningham   (501) staff       (20)        1 2023-06-07 20:47:12.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 willcunningham   (501) staff       (20)       88 2023-06-07 20:47:12.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 willcunningham   (501) staff       (20)       92 2023-06-07 20:47:12.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin.egg-info/requires.txt
+-rw-r--r--   0 willcunningham   (501) staff       (20)       27 2023-06-07 20:47:12.000000 covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin.egg-info/top_level.txt
+-rw-r--r--   0 willcunningham   (501) staff       (20)     1238 2023-05-29 17:44:19.000000 covalent-azurebatch-plugin-0.12.0rc0/pyproject.toml
+-rw-r--r--   0 willcunningham   (501) staff       (20)      928 2023-06-07 20:34:48.000000 covalent-azurebatch-plugin-0.12.0rc0/requirements.txt
+-rw-r--r--   0 willcunningham   (501) staff       (20)       41 2023-06-07 20:47:12.348437 covalent-azurebatch-plugin-0.12.0rc0/setup.cfg
+-rw-r--r--   0 willcunningham   (501) staff       (20)     2874 2023-06-07 20:35:12.000000 covalent-azurebatch-plugin-0.12.0rc0/setup.py
```

### Comparing `covalent-azurebatch-plugin-0.12.0/LICENSE` & `covalent-azurebatch-plugin-0.12.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/PKG-INFO` & `covalent-azurebatch-plugin-0.12.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-azurebatch-plugin
-Version: 0.12.0
+Version: 0.12.0rc0
 Summary: Covalent Azure Batch Plugin
 Home-page: https://github.com/AgnostiqHQ/covalent-azurebatch-plugin
 Download-URL: https://github.com/AgnostiqHQ/covalent-azurebatch-plugin/archive/v0.12.0.tar.gz
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
```

### Comparing `covalent-azurebatch-plugin-0.12.0/README.md` & `covalent-azurebatch-plugin-0.12.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/__init__.py` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/Dockerfile` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/Dockerfile`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/exec.py` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/exec.py`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/iam.tf` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/iam.tf`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/main.tf` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/main.tf`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/outputs.tf` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/outputs.tf`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/storage.tf` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/storage.tf`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/variables.tf` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/variables.tf`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/assets/infra/versions.tf` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/assets/infra/versions.tf`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/azurebatch.py` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/azurebatch.py`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/exceptions.py` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin/utils.py` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin.egg-info/PKG-INFO` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-azurebatch-plugin
-Version: 0.12.0
+Version: 0.12.0rc0
 Summary: Covalent Azure Batch Plugin
 Home-page: https://github.com/AgnostiqHQ/covalent-azurebatch-plugin
 Download-URL: https://github.com/AgnostiqHQ/covalent-azurebatch-plugin/archive/v0.12.0.tar.gz
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
```

### Comparing `covalent-azurebatch-plugin-0.12.0/covalent_azurebatch_plugin.egg-info/SOURCES.txt` & `covalent-azurebatch-plugin-0.12.0rc0/covalent_azurebatch_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/pyproject.toml` & `covalent-azurebatch-plugin-0.12.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/requirements.txt` & `covalent-azurebatch-plugin-0.12.0rc0/requirements.txt`

 * *Files identical despite different names*

### Comparing `covalent-azurebatch-plugin-0.12.0/setup.py` & `covalent-azurebatch-plugin-0.12.0rc0/setup.py`

 * *Files identical despite different names*

