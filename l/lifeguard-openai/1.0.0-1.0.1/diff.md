# Comparing `tmp/lifeguard-openai-1.0.0.tar.gz` & `tmp/lifeguard-openai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-openai-1.0.0.tar", last modified: Tue Jun  6 19:40:17 2023, max compression
+gzip compressed data, was "lifeguard-openai-1.0.1.tar", last modified: Wed Jun  7 13:58:01 2023, max compression
```

## Comparing `lifeguard-openai-1.0.0.tar` & `lifeguard-openai-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:40:17.225092 lifeguard-openai-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-06 19:40:17.225092 lifeguard-openai-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-06 19:39:56.000000 lifeguard-openai-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:40:17.225092 lifeguard-openai-1.0.0/lifeguard_openai/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-06 19:39:56.000000 lifeguard-openai-1.0.0/lifeguard_openai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:40:17.225092 lifeguard-openai-1.0.0/lifeguard_openai/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.000000 lifeguard-openai-1.0.0/lifeguard_openai/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-06 19:39:56.000000 lifeguard-openai-1.0.0/lifeguard_openai/actions/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-06 19:39:56.000000 lifeguard-openai-1.0.0/lifeguard_openai/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:40:17.225092 lifeguard-openai-1.0.0/lifeguard_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-06 19:40:17.000000 lifeguard-openai-1.0.0/lifeguard_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-06 19:40:17.000000 lifeguard-openai-1.0.0/lifeguard_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:40:17.000000 lifeguard-openai-1.0.0/lifeguard_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 19:40:17.000000 lifeguard-openai-1.0.0/lifeguard_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 19:40:17.000000 lifeguard-openai-1.0.0/lifeguard_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 19:40:17.225092 lifeguard-openai-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-06 19:39:56.000000 lifeguard-openai-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/lifeguard_openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/lifeguard_openai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/lifeguard_openai/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/lifeguard_openai/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/lifeguard_openai/actions/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/lifeguard_openai/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-07 13:58:01.000000 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-07 13:58:01.000000 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:58:01.000000 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 13:58:01.000000 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 13:58:01.000000 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/setup.py
```

### Comparing `lifeguard-openai-1.0.0/PKG-INFO` & `lifeguard-openai-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-openai
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lifeguard integration with OpenAI
 Home-page: https://github.com/LifeguardSystem/lifeguard-openai
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-openai-1.0.0/lifeguard_openai/settings.py` & `lifeguard-openai-1.0.1/lifeguard_openai/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-openai-1.0.0/lifeguard_openai.egg-info/PKG-INFO` & `lifeguard-openai-1.0.1/lifeguard_openai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-openai
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lifeguard integration with OpenAI
 Home-page: https://github.com/LifeguardSystem/lifeguard-openai
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-openai-1.0.0/setup.py` & `lifeguard-openai-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard-openai",
-    version="1.0.0",
+    version="1.0.1",
     url="https://github.com/LifeguardSystem/lifeguard-openai",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=[],
     include_package_data=True,
     description="Lifeguard integration with OpenAI",
```

