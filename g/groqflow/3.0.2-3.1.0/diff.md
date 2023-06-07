# Comparing `tmp/groqflow-3.0.2.tar.gz` & `tmp/groqflow-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groqflow-3.0.2.tar", last modified: Thu May 11 15:26:06 2023, max compression
+gzip compressed data, was "groqflow-3.1.0.tar", last modified: Wed Jun  7 19:11:33 2023, max compression
```

## Comparing `groqflow-3.0.2.tar` & `groqflow-3.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.202463 groqflow-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-11 15:26:06.202463 groqflow-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-11 15:25:55.000000 groqflow-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.194463 groqflow-3.0.2/groqflow/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.198463 groqflow-3.0.2/groqflow/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19995 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/onnx_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/quantization_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/sdk_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/tensor_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/common/tf_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.198463 groqflow-3.0.2/groqflow/groqmodel/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/groqmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/groqmodel/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/groqmodel/groqmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/groqmodel/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.202463 groqflow-3.0.2/groqflow/justgroqit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/assemble_multichip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24108 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/export.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6101 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/groqit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/hummingbird.py
--rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/ignition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/justgroqit/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 15:25:56.000000 groqflow-3.0.2/groqflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:26:06.194463 groqflow-3.0.2/groqflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-11 15:26:06.000000 groqflow-3.0.2/groqflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-11 15:26:06.000000 groqflow-3.0.2/groqflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:26:06.000000 groqflow-3.0.2/groqflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-11 15:26:06.000000 groqflow-3.0.2/groqflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 15:26:06.000000 groqflow-3.0.2/groqflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-11 15:25:56.000000 groqflow-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:26:06.202463 groqflow-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-11 15:25:56.000000 groqflow-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:11:33.461943 groqflow-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-07 19:11:33.461943 groqflow-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-07 19:11:23.000000 groqflow-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:11:33.457943 groqflow-3.1.0/groqflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:11:33.461943 groqflow-3.1.0/groqflow/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/common/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/common/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/common/onnx_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/common/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/common/quantization_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/common/sdk_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/common/tensor_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/common/tf_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:11:33.461943 groqflow-3.1.0/groqflow/groqmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/groqmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/groqmodel/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/groqmodel/groqmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/groqmodel/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:11:33.461943 groqflow-3.1.0/groqflow/justgroqit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/justgroqit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/justgroqit/assemble_multichip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/justgroqit/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24108 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/justgroqit/export.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6101 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/justgroqit/groqit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/justgroqit/hummingbird.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/justgroqit/ignition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/justgroqit/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 19:11:23.000000 groqflow-3.1.0/groqflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:11:33.457943 groqflow-3.1.0/groqflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-07 19:11:33.000000 groqflow-3.1.0/groqflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-07 19:11:33.000000 groqflow-3.1.0/groqflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:11:33.000000 groqflow-3.1.0/groqflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-07 19:11:33.000000 groqflow-3.1.0/groqflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 19:11:33.000000 groqflow-3.1.0/groqflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-07 19:11:23.000000 groqflow-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:11:33.461943 groqflow-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 19:11:23.000000 groqflow-3.1.0/setup.py
```

### Comparing `groqflow-3.0.2/PKG-INFO` & `groqflow-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groqflow
-Version: 3.0.2
+Version: 3.1.0
 Summary: GroqFlow toolchain library
 Home-page: https://github.com/groq/groqflow
 Author: Groq
 Author-email: sales@groq.com
 License: MIT
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: groqflow Version: 3.0.2 Summary: GroqFlow toolchain
+Metadata-Version: 2.1 Name: groqflow Version: 3.1.0 Summary: GroqFlow toolchain
 library Home-page: https://github.com/groq/groqflow Author: Groq Author-email:
 sales@groq.com License: MIT Requires-Python: >=3.8, <3.11 Description-Content-
 Type: text/markdown Provides-Extra: tensorflow # GroqFlow ð GroqFlowâ¢ is
 the easiest way to get started with Groq's technology. GroqFlow provides an
 automated tool flow for compiling machine learning and linear algebra workloads
 into Groq programs and executing those programs on GroqChipâ¢ processors. We
 recommend that your system meets the following hardware requirements: - To
```

### Comparing `groqflow-3.0.2/README.md` & `groqflow-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/common/build.py` & `groqflow-3.1.0/groqflow/common/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,14 +274,15 @@
     build_name: str
     compiler_flags: List[str]
     assembler_flags: List[str]
     groqview: bool
     groqcard: Groqcard
     sequence: List[str]
     num_chips: Optional[int] = None
+    onnx_opset: int = DEFAULT_ONNX_OPSET
 
 
 @dataclasses.dataclass
 class Info:
     """
     Information about a build that may be useful for analysis
     or debugging purposes.
```

### Comparing `groqflow-3.0.2/groqflow/common/cache.py` & `groqflow-3.1.0/groqflow/common/cache.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/common/exceptions.py` & `groqflow-3.1.0/groqflow/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/common/onnx_helpers.py` & `groqflow-3.1.0/groqflow/common/onnx_helpers.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/common/printing.py` & `groqflow-3.1.0/groqflow/common/printing.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/common/quantization_helpers.py` & `groqflow-3.1.0/groqflow/common/quantization_helpers.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/common/sdk_helpers.py` & `groqflow-3.1.0/groqflow/common/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/common/tensor_helpers.py` & `groqflow-3.1.0/groqflow/common/tensor_helpers.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/common/tf_helpers.py` & `groqflow-3.1.0/groqflow/common/tf_helpers.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/groqmodel/execute.py` & `groqflow-3.1.0/groqflow/groqmodel/execute.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/groqmodel/groqmodel.py` & `groqflow-3.1.0/groqflow/groqmodel/groqmodel.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/groqmodel/remote.py` & `groqflow-3.1.0/groqflow/groqmodel/remote.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/justgroqit/assemble_multichip.py` & `groqflow-3.1.0/groqflow/justgroqit/assemble_multichip.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/justgroqit/compile.py` & `groqflow-3.1.0/groqflow/justgroqit/compile.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/justgroqit/export.py` & `groqflow-3.1.0/groqflow/justgroqit/export.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/justgroqit/groqit.py` & `groqflow-3.1.0/groqflow/justgroqit/groqit.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/justgroqit/hummingbird.py` & `groqflow-3.1.0/groqflow/justgroqit/hummingbird.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/justgroqit/ignition.py` & `groqflow-3.1.0/groqflow/justgroqit/ignition.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow/justgroqit/stage.py` & `groqflow-3.1.0/groqflow/justgroqit/stage.py`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/groqflow.egg-info/PKG-INFO` & `groqflow-3.1.0/groqflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groqflow
-Version: 3.0.2
+Version: 3.1.0
 Summary: GroqFlow toolchain library
 Home-page: https://github.com/groq/groqflow
 Author: Groq
 Author-email: sales@groq.com
 License: MIT
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: groqflow Version: 3.0.2 Summary: GroqFlow toolchain
+Metadata-Version: 2.1 Name: groqflow Version: 3.1.0 Summary: GroqFlow toolchain
 library Home-page: https://github.com/groq/groqflow Author: Groq Author-email:
 sales@groq.com License: MIT Requires-Python: >=3.8, <3.11 Description-Content-
 Type: text/markdown Provides-Extra: tensorflow # GroqFlow ð GroqFlowâ¢ is
 the easiest way to get started with Groq's technology. GroqFlow provides an
 automated tool flow for compiling machine learning and linear algebra workloads
 into Groq programs and executing those programs on GroqChipâ¢ processors. We
 recommend that your system meets the following hardware requirements: - To
```

### Comparing `groqflow-3.0.2/groqflow.egg-info/SOURCES.txt` & `groqflow-3.1.0/groqflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `groqflow-3.0.2/setup.py` & `groqflow-3.1.0/setup.py`

 * *Files identical despite different names*

