# Comparing `tmp/weave-py-api-1.1.0.tar.gz` & `tmp/weave-py-api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weave-py-api-1.1.0.tar", last modified: Wed Jun  7 06:52:56 2023, max compression
+gzip compressed data, was "weave-py-api-1.2.0.tar", last modified: Wed Jun  7 09:23:48 2023, max compression
```

## Comparing `weave-py-api-1.1.0.tar` & `weave-py-api-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 06:52:56.108037 weave-py-api-1.1.0/
--rw-rw-rw-   0        0        0     1086 2023-06-07 05:54:07.000000 weave-py-api-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       15 2023-06-07 06:24:55.000000 weave-py-api-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1972 2023-06-07 06:52:56.108037 weave-py-api-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      169 2023-06-07 06:32:45.000000 weave-py-api-1.1.0/README.md
--rw-rw-rw-   0        0        0     1436 2023-06-07 06:48:40.000000 weave-py-api-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 06:52:56.108037 weave-py-api-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-07 06:52:56.072039 weave-py-api-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 06:52:56.083036 weave-py-api-1.1.0/src/weave_py_api.egg-info/
--rw-rw-rw-   0        0        0     1972 2023-06-07 06:52:56.000000 weave-py-api-1.1.0/src/weave_py_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-06-07 06:52:56.000000 weave-py-api-1.1.0/src/weave_py_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 06:52:56.000000 weave-py-api-1.1.0/src/weave_py_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      178 2023-06-07 06:52:56.000000 weave-py-api-1.1.0/src/weave_py_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 06:52:56.000000 weave-py-api-1.1.0/src/weave_py_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 06:52:56.107038 weave-py-api-1.1.0/src/weaveapi/
--rw-rw-rw-   0        0        0        0 2022-03-20 14:22:30.000000 weave-py-api-1.1.0/src/weaveapi/__init__.py
--rw-rw-rw-   0        0        0     3817 2023-01-27 18:40:16.000000 weave-py-api-1.1.0/src/weaveapi/apicontext.py
--rw-rw-rw-   0        0        0    34203 2023-05-09 11:29:57.000000 weave-py-api-1.1.0/src/weaveapi/clienthttp.py
--rw-rw-rw-   0        0        0    40963 2023-05-09 11:29:57.000000 weave-py-api-1.1.0/src/weaveapi/clientws.py
--rw-rw-rw-   0        0        0     3968 2023-02-28 07:27:53.000000 weave-py-api-1.1.0/src/weaveapi/filter.py
--rw-rw-rw-   0        0        0      363 2022-03-20 14:22:30.000000 weave-py-api-1.1.0/src/weaveapi/futures.py
--rw-rw-rw-   0        0        0     5015 2022-12-30 12:27:54.000000 weave-py-api-1.1.0/src/weaveapi/javarandom.py
--rw-rw-rw-   0        0        0     3455 2022-12-12 12:20:08.000000 weave-py-api-1.1.0/src/weaveapi/keys.py
--rw-rw-rw-   0        0        0    14919 2023-05-09 11:29:57.000000 weave-py-api-1.1.0/src/weaveapi/nodeapi.py
--rw-rw-rw-   0        0        0    14300 2023-04-05 10:54:57.000000 weave-py-api-1.1.0/src/weaveapi/options.py
--rw-rw-rw-   0        0        0      984 2022-12-30 12:27:54.000000 weave-py-api-1.1.0/src/weaveapi/records.py
--rw-rw-rw-   0        0        0      884 2023-01-23 13:53:04.000000 weave-py-api-1.1.0/src/weaveapi/session.py
--rw-rw-rw-   0        0        0      894 2022-03-28 18:45:18.000000 weave-py-api-1.1.0/src/weaveapi/setup.py
--rw-rw-rw-   0        0        0     4282 2023-01-25 16:39:28.000000 weave-py-api-1.1.0/src/weaveapi/utils.py
--rw-rw-rw-   0        0        0       81 2022-03-20 14:22:30.000000 weave-py-api-1.1.0/src/weaveapi/weaveapi.py
--rw-rw-rw-   0        0        0     4980 2023-03-15 09:17:36.000000 weave-py-api-1.1.0/src/weaveapi/weaveh.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:23:48.694781 weave-py-api-1.2.0/
+-rw-rw-rw-   0        0        0     1086 2023-06-07 05:54:07.000000 weave-py-api-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       15 2023-06-07 06:24:55.000000 weave-py-api-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2648 2023-06-07 09:23:48.693780 weave-py-api-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      845 2023-06-07 09:20:21.000000 weave-py-api-1.2.0/README.md
+-rw-rw-rw-   0        0        0     1436 2023-06-07 09:23:13.000000 weave-py-api-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 09:23:48.694781 weave-py-api-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 09:23:48.662789 weave-py-api-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 09:23:48.680781 weave-py-api-1.2.0/src/weave_py_api.egg-info/
+-rw-rw-rw-   0        0        0     2648 2023-06-07 09:23:48.000000 weave-py-api-1.2.0/src/weave_py_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-06-07 09:23:48.000000 weave-py-api-1.2.0/src/weave_py_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 09:23:48.000000 weave-py-api-1.2.0/src/weave_py_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      178 2023-06-07 09:23:48.000000 weave-py-api-1.2.0/src/weave_py_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 09:23:48.000000 weave-py-api-1.2.0/src/weave_py_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 09:23:48.693780 weave-py-api-1.2.0/src/weaveapi/
+-rw-rw-rw-   0        0        0        0 2022-03-20 14:22:30.000000 weave-py-api-1.2.0/src/weaveapi/__init__.py
+-rw-rw-rw-   0        0        0     3817 2023-01-27 18:40:16.000000 weave-py-api-1.2.0/src/weaveapi/apicontext.py
+-rw-rw-rw-   0        0        0    34203 2023-05-09 11:29:57.000000 weave-py-api-1.2.0/src/weaveapi/clienthttp.py
+-rw-rw-rw-   0        0        0    40963 2023-05-09 11:29:57.000000 weave-py-api-1.2.0/src/weaveapi/clientws.py
+-rw-rw-rw-   0        0        0     3968 2023-02-28 07:27:53.000000 weave-py-api-1.2.0/src/weaveapi/filter.py
+-rw-rw-rw-   0        0        0      363 2022-03-20 14:22:30.000000 weave-py-api-1.2.0/src/weaveapi/futures.py
+-rw-rw-rw-   0        0        0     5015 2022-12-30 12:27:54.000000 weave-py-api-1.2.0/src/weaveapi/javarandom.py
+-rw-rw-rw-   0        0        0     3455 2022-12-12 12:20:08.000000 weave-py-api-1.2.0/src/weaveapi/keys.py
+-rw-rw-rw-   0        0        0    14919 2023-05-09 11:29:57.000000 weave-py-api-1.2.0/src/weaveapi/nodeapi.py
+-rw-rw-rw-   0        0        0    14300 2023-04-05 10:54:57.000000 weave-py-api-1.2.0/src/weaveapi/options.py
+-rw-rw-rw-   0        0        0      984 2022-12-30 12:27:54.000000 weave-py-api-1.2.0/src/weaveapi/records.py
+-rw-rw-rw-   0        0        0      884 2023-01-23 13:53:04.000000 weave-py-api-1.2.0/src/weaveapi/session.py
+-rw-rw-rw-   0        0        0      894 2022-03-28 18:45:18.000000 weave-py-api-1.2.0/src/weaveapi/setup.py
+-rw-rw-rw-   0        0        0     4282 2023-01-25 16:39:28.000000 weave-py-api-1.2.0/src/weaveapi/utils.py
+-rw-rw-rw-   0        0        0       81 2022-03-20 14:22:30.000000 weave-py-api-1.2.0/src/weaveapi/weaveapi.py
+-rw-rw-rw-   0        0        0     4980 2023-03-15 09:17:36.000000 weave-py-api-1.2.0/src/weaveapi/weaveh.py
```

### Comparing `weave-py-api-1.1.0/LICENSE` & `weave-py-api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/pyproject.toml` & `weave-py-api-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "weave-py-api"
-version = "1.1.0"
+version = "1.2.0"
 description = "Weavechain Python API"
 readme = "README.md"
 authors = [{ name = "Weavechain", email = "support@weavechain.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -37,15 +37,15 @@
 
 [project.urls]
 Homepage = "https://github.com/weavechain/weave-py-api"
 
 [project.scripts]
 
 [tool.bumpver]
-current_version = "1.1.0"
+current_version = "1.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `weave-py-api-1.1.0/src/weave_py_api.egg-info/SOURCES.txt` & `weave-py-api-1.2.0/src/weave_py_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/apicontext.py` & `weave-py-api-1.2.0/src/weaveapi/apicontext.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/clienthttp.py` & `weave-py-api-1.2.0/src/weaveapi/clienthttp.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/clientws.py` & `weave-py-api-1.2.0/src/weaveapi/clientws.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/filter.py` & `weave-py-api-1.2.0/src/weaveapi/filter.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/javarandom.py` & `weave-py-api-1.2.0/src/weaveapi/javarandom.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/keys.py` & `weave-py-api-1.2.0/src/weaveapi/keys.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/nodeapi.py` & `weave-py-api-1.2.0/src/weaveapi/nodeapi.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/options.py` & `weave-py-api-1.2.0/src/weaveapi/options.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/records.py` & `weave-py-api-1.2.0/src/weaveapi/records.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/session.py` & `weave-py-api-1.2.0/src/weaveapi/session.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/setup.py` & `weave-py-api-1.2.0/src/weaveapi/setup.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/utils.py` & `weave-py-api-1.2.0/src/weaveapi/utils.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.1.0/src/weaveapi/weaveh.py` & `weave-py-api-1.2.0/src/weaveapi/weaveh.py`

 * *Files identical despite different names*

