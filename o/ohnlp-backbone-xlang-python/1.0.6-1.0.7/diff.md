# Comparing `tmp/ohnlp-backbone-xlang-python-1.0.6.tar.gz` & `tmp/ohnlp-backbone-xlang-python-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.6.tar", last modified: Wed Jun  7 18:20:16 2023, max compression
+gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.7.tar", last modified: Wed Jun  7 20:56:17 2023, max compression
```

## Comparing `ohnlp-backbone-xlang-python-1.0.6.tar` & `ohnlp-backbone-xlang-python-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/ohnlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/backbone_module_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 18:20:16.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-07 18:20:16.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:20:16.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-07 18:20:16.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 18:20:16.000000 ohnlp-backbone-xlang-python-1.0.6/ohnlp_backbone_xlang_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:20:16.038522 ohnlp-backbone-xlang-python-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-07 18:20:10.000000 ohnlp-backbone-xlang-python-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:17.868150 ohnlp-backbone-xlang-python-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 20:56:17.864150 ohnlp-backbone-xlang-python-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:17.864150 ohnlp-backbone-xlang-python-1.0.7/ohnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:17.864150 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:17.864150 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/backbone_module_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:56:17.864150 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 20:56:17.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-07 20:56:17.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:56:17.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-07 20:56:17.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 20:56:17.000000 ohnlp-backbone-xlang-python-1.0.7/ohnlp_backbone_xlang_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:56:17.868150 ohnlp-backbone-xlang-python-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-07 20:56:15.000000 ohnlp-backbone-xlang-python-1.0.7/setup.py
```

### Comparing `ohnlp-backbone-xlang-python-1.0.6/LICENSE` & `ohnlp-backbone-xlang-python-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.6/README.md` & `ohnlp-backbone-xlang-python-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # OHNLP Toolkit Cross-Language Python Bridge
 This repository contains the python bridge and associated API to implement python-based components for the OHNLP Toolkit.
 For most users, direct usage of this git repository should not be necessary unless implementing your own
-python-based backbone component, in which case this module should be installed via `pip install ohnlp-backbone-xlang-pythont`
+python-based backbone component, in which case this module should be installed via `pip install ohnlp-backbone-xlang-python`
 and the relevant API functions correspondingly implemented.
 
 For example Backbone python module implementations of the relevant API functions, please refer to the 
 [Backbone-XLang-Python-Examples](https://github.com/OHNLP/backbone-xlang-python-examples) repository instead
```

### Comparing `ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/api.py` & `ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import json
+from abc import ABC, abstractmethod
 from enum import Enum
 from typing import List, Union
 
 
 class FieldType(object):
     def __init__(self, type_name: TypeName, array_content_type: Union[FieldType, None] = None,
                  row_content_type: Union[Schema, None] = None):
@@ -167,56 +168,67 @@
             for element in data:
                 ret.append(self.parse_row_field_value_to_json(field_type.array_content_type, element))
             return ret
         else:
             return data
 
 
-class BackboneComponentDefinition(object):
+class BackboneComponentDefinition(ABC):
+    @abstractmethod
     def get_component_def(self) -> BackboneComponent:
         pass
 
+    @abstractmethod
     def get_do_fn(self) -> BackboneComponentOneToOneDoFn:
         pass
 
 
-class BackboneComponent(BridgedInterfaceWithConvertableDataTypes):
+class BackboneComponent(ABC, BridgedInterfaceWithConvertableDataTypes):
     def __init__(self):
         pass
 
+    @abstractmethod
     def init(self, configstr: str) -> None:
         pass
 
+    @abstractmethod
     def to_do_fn_config(self) -> str:
         pass
 
+    @abstractmethod
     def get_input_tag(self) -> str:
         pass
 
+    @abstractmethod
     def get_output_tags(self) -> List[str]:
         pass
 
+    @abstractmethod
     def calculate_output_schema(self, input_schema: Schema) -> Schema:
         pass
 
     class Java:
         implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonBackbonePipelineComponent"]
 
 
-class BackboneComponentOneToOneDoFn(BridgedInterfaceWithConvertableDataTypes):
+class BackboneComponentOneToOneDoFn(ABC, BridgedInterfaceWithConvertableDataTypes):
     def __init__(self):
         pass
 
+    @abstractmethod
     def init_from_driver(self, config_json_str: str) -> None:
         pass
 
+    @abstractmethod
     def on_bundle_start(self) -> None:
         pass
 
+    @abstractmethod
     def on_bundle_end(self) -> None:
         pass
 
+    @abstractmethod
     def apply(self, input_row: Row) -> List[Row]:
         pass
 
     class Java:
         implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonOneToOneTransformDoFn"]
```

### Comparing `ohnlp-backbone-xlang-python-1.0.6/ohnlp/toolkit/backbone/backbone_module_launcher.py` & `ohnlp-backbone-xlang-python-1.0.7/ohnlp/toolkit/backbone/backbone_module_launcher.py`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.6/setup.py` & `ohnlp-backbone-xlang-python-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ohnlp-backbone-xlang-python",
-    version="1.0.6",
+    version="1.0.7",
     description="Python support for OHNLP Toolkit Backbone Components",
     author="Andrew Wen",
     author_email="contact@ohnlp.org",
     packages=find_packages(),
     python_requires='>3.7',
     install_requires=[
         'certifi==2023.5.7',
```

