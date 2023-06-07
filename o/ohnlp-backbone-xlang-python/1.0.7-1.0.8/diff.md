# Comparing `tmp/ohnlp-backbone-xlang-python-1.0.7.tar.gz` & `tmp/ohnlp-backbone-xlang-python-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.7.tar", last modified: Wed Jun  7 20:56:17 2023, max compression
+gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.8.tar", last modified: Wed Jun  7 21:29:26 2023, max compression
```

## Comparing `ohnlp-backbone-xlang-python-1.0.7.tar` & `ohnlp-backbone-xlang-python-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:17.868150 ohnlp-backbone-xlang-python-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 20:56:17.864150 ohnlp-backbone-xlang-python-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:17.864150 ohnlp-backbone-xlang-python-1.0.7/ohnlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:17.864150 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:17.864150 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/backbone_module_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:17.864150 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 20:56:17.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-07 20:56:17.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:56:17.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-07 20:56:17.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 20:56:17.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:56:17.868150 ohnlp-backbone-xlang-python-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/ohnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/backbone_module_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 21:29:26.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-07 21:29:26.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:29:26.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-07 21:29:26.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 21:29:26.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/setup.py
```

### Comparing `ohnlp-backbone-xlang-python-1.0.7/LICENSE` & `ohnlp-backbone-xlang-python-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.7/README.md` & `ohnlp-backbone-xlang-python-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/api.py` & `ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         pass
 
     @abstractmethod
     def get_output_tags(self) -> List[str]:
         pass
 
     @abstractmethod
-    def calculate_output_schema(self, input_schema: Schema) -> Schema:
+    def calculate_output_schema(self, input_schema: Schema) -> dict[str, Schema]:
         pass
 
     class Java:
         implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonBackbonePipelineComponent"]
 
 
 class BackboneComponentOneToOneDoFn(ABC, BridgedInterfaceWithConvertableDataTypes):
```

### Comparing `ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/backbone_module_launcher.py` & `ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/backbone_module_launcher.py`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.7/setup.py` & `ohnlp-backbone-xlang-python-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ohnlp-backbone-xlang-python",
-    version="1.0.7",
+    version="1.0.8",
     description="Python support for OHNLP Toolkit Backbone Components",
     author="Andrew Wen",
     author_email="contact@ohnlp.org",
     packages=find_packages(),
     python_requires='>3.7',
     install_requires=[
         'certifi==2023.5.7',
```

