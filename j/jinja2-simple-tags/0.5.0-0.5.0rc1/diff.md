# Comparing `tmp/jinja2-simple-tags-0.5.0.tar.gz` & `tmp/jinja2-simple-tags-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2-simple-tags-0.5.0.tar", last modified: Wed Jun  7 10:52:01 2023, max compression
+gzip compressed data, was "jinja2-simple-tags-0.5.0rc1.tar", last modified: Fri Apr 28 11:43:20 2023, max compression
```

## Comparing `jinja2-simple-tags-0.5.0.tar` & `jinja2-simple-tags-0.5.0rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:52:01.679823 jinja2-simple-tags-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-07 10:52:01.679823 jinja2-simple-tags-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:52:01.679823 jinja2-simple-tags-0.5.0/jinja2_simple_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-07 10:52:01.000000 jinja2-simple-tags-0.5.0/jinja2_simple_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-07 10:52:01.000000 jinja2-simple-tags-0.5.0/jinja2_simple_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:52:01.000000 jinja2-simple-tags-0.5.0/jinja2_simple_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:52:01.000000 jinja2-simple-tags-0.5.0/jinja2_simple_tags.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 10:52:01.000000 jinja2-simple-tags-0.5.0/jinja2_simple_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 10:52:01.000000 jinja2-simple-tags-0.5.0/jinja2_simple_tags.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/jinja2_simple_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-07 10:52:01.679823 jinja2-simple-tags-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:52:01.679823 jinja2-simple-tags-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/tests/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/tests/test_escaping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-07 10:51:55.000000 jinja2-simple-tags-0.5.0/tests/test_standalone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:20.556799 jinja2-simple-tags-0.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-28 11:43:14.000000 jinja2-simple-tags-0.5.0rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-28 11:43:14.000000 jinja2-simple-tags-0.5.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-28 11:43:14.000000 jinja2-simple-tags-0.5.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 11:43:14.000000 jinja2-simple-tags-0.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-28 11:43:20.556799 jinja2-simple-tags-0.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-28 11:43:14.000000 jinja2-simple-tags-0.5.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:20.556799 jinja2-simple-tags-0.5.0rc1/jinja2_simple_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-28 11:43:20.000000 jinja2-simple-tags-0.5.0rc1/jinja2_simple_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-28 11:43:20.000000 jinja2-simple-tags-0.5.0rc1/jinja2_simple_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:43:20.000000 jinja2-simple-tags-0.5.0rc1/jinja2_simple_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:43:20.000000 jinja2-simple-tags-0.5.0rc1/jinja2_simple_tags.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 11:43:20.000000 jinja2-simple-tags-0.5.0rc1/jinja2_simple_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 11:43:20.000000 jinja2-simple-tags-0.5.0rc1/jinja2_simple_tags.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-28 11:43:14.000000 jinja2-simple-tags-0.5.0rc1/jinja2_simple_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-28 11:43:20.556799 jinja2-simple-tags-0.5.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 11:43:15.000000 jinja2-simple-tags-0.5.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:20.556799 jinja2-simple-tags-0.5.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-28 11:43:15.000000 jinja2-simple-tags-0.5.0rc1/tests/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-28 11:43:15.000000 jinja2-simple-tags-0.5.0rc1/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-28 11:43:15.000000 jinja2-simple-tags-0.5.0rc1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-28 11:43:15.000000 jinja2-simple-tags-0.5.0rc1/tests/test_escaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-28 11:43:15.000000 jinja2-simple-tags-0.5.0rc1/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-28 11:43:15.000000 jinja2-simple-tags-0.5.0rc1/tests/test_standalone.py
```

### Comparing `jinja2-simple-tags-0.5.0/CHANGELOG.md` & `jinja2-simple-tags-0.5.0rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `jinja2-simple-tags-0.5.0/CONTRIBUTING.md` & `jinja2-simple-tags-0.5.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jinja2-simple-tags-0.5.0/LICENSE` & `jinja2-simple-tags-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2-simple-tags-0.5.0/PKG-INFO` & `jinja2-simple-tags-0.5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinja2-simple-tags
-Version: 0.5.0
+Version: 0.5.0rc1
 Summary: Base classes for quick-and-easy template tag development
 Home-page: https://github.com/dldevinc/jinja2-simple-tags
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
```

### Comparing `jinja2-simple-tags-0.5.0/README.md` & `jinja2-simple-tags-0.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `jinja2-simple-tags-0.5.0/jinja2_simple_tags.egg-info/PKG-INFO` & `jinja2-simple-tags-0.5.0rc1/jinja2_simple_tags.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinja2-simple-tags
-Version: 0.5.0
+Version: 0.5.0rc1
 Summary: Base classes for quick-and-easy template tag development
 Home-page: https://github.com/dldevinc/jinja2-simple-tags
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
```

### Comparing `jinja2-simple-tags-0.5.0/jinja2_simple_tags.py` & `jinja2-simple-tags-0.5.0rc1/jinja2_simple_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from jinja2 import nodes
 from jinja2.ext import Extension
 from jinja2.lexer import describe_token
 from jinja2.parser import Parser
 from jinja2.runtime import Context
 
 __all__ = ["StandaloneTag", "ContainerTag"]
-__version__ = "0.5.0"
+__version__ = "0.5.0-rc.1"
 
 
 class BaseTemplateTag(Extension):
     def __init__(self, environment):
         super().__init__(environment)
         self.context = None
         self.template = None
```

### Comparing `jinja2-simple-tags-0.5.0/setup.cfg` & `jinja2-simple-tags-0.5.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jinja2-simple-tags-0.5.0/tests/test_args.py` & `jinja2-simple-tags-0.5.0rc1/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `jinja2-simple-tags-0.5.0/tests/test_container.py` & `jinja2-simple-tags-0.5.0rc1/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `jinja2-simple-tags-0.5.0/tests/test_context.py` & `jinja2-simple-tags-0.5.0rc1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `jinja2-simple-tags-0.5.0/tests/test_escaping.py` & `jinja2-simple-tags-0.5.0rc1/tests/test_escaping.py`

 * *Files identical despite different names*

### Comparing `jinja2-simple-tags-0.5.0/tests/test_properties.py` & `jinja2-simple-tags-0.5.0rc1/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `jinja2-simple-tags-0.5.0/tests/test_standalone.py` & `jinja2-simple-tags-0.5.0rc1/tests/test_standalone.py`

 * *Files identical despite different names*

