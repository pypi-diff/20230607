# Comparing `tmp/ohnlp-backbone-xlang-python-1.0.5.tar.gz` & `tmp/ohnlp-backbone-xlang-python-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.5.tar", last modified: Mon Jun  5 18:32:03 2023, max compression
+gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.6.tar", last modified: Wed Jun  7 18:20:16 2023, max compression
```

## Comparing `ohnlp-backbone-xlang-python-1.0.5.tar` & `ohnlp-backbone-xlang-python-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/ohnlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/backbone_module_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-05 18:32:03.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-05 18:32:03.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:32:03.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-05 18:32:03.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 18:32:03.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/ohnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/backbone_module_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 18:20:16.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-07 18:20:16.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:20:16.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-07 18:20:16.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 18:20:16.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/setup.py
```

### Comparing `ohnlp-backbone-xlang-python-1.0.5/LICENSE` & `ohnlp-backbone-xlang-python-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.5/README.md` & `ohnlp-backbone-xlang-python-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/api.py` & `ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,12 +211,12 @@
 
     def on_bundle_start(self) -> None:
         pass
 
     def on_bundle_end(self) -> None:
         pass
 
-    def apply(self, input_row: Row) -> Row:
+    def apply(self, input_row: Row) -> List[Row]:
         pass
 
     class Java:
         implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonOneToOneTransformDoFn"]
```

### Comparing `ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/backbone_module_launcher.py` & `ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/backbone_module_launcher.py`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.5/setup.py` & `ohnlp-backbone-xlang-python-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ohnlp-backbone-xlang-python",
-    version="1.0.5",
+    version="1.0.6",
     description="Python support for OHNLP Toolkit Backbone Components",
     author="Andrew Wen",
     author_email="contact@ohnlp.org",
     packages=find_packages(),
     python_requires='>3.7',
     install_requires=[
         'certifi==2023.5.7',
```

