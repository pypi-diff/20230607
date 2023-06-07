# Comparing `tmp/tree-ring-watermark-0.0.1.tar.gz` & `tmp/tree_ring_watermark-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-ring-watermark-0.0.1.tar", last modified: Wed Jun  7 14:40:20 2023, max compression
+gzip compressed data, was "tree_ring_watermark-0.0.2.tar", last modified: Wed Jun  7 14:59:12 2023, max compression
```

## Comparing `tree-ring-watermark-0.0.1.tar` & `tree_ring_watermark-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-07 14:40:20.532415 tree-ring-watermark-0.0.1/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1065 2023-06-07 14:16:59.000000 tree-ring-watermark-0.0.1/LICENSE.md
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3408 2023-06-07 14:40:20.532415 tree-ring-watermark-0.0.1/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2478 2023-06-07 14:16:59.000000 tree-ring-watermark-0.0.1/README.md
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-06-07 14:40:20.532415 tree-ring-watermark-0.0.1/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8207 2023-06-07 14:40:00.000000 tree-ring-watermark-0.0.1/setup.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-07 14:40:20.532415 tree-ring-watermark-0.0.1/src/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-07 14:40:20.532415 tree-ring-watermark-0.0.1/src/tree_ring_watermark/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      111 2023-06-07 14:40:00.000000 tree-ring-watermark-0.0.1/src/tree_ring_watermark/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      107 2023-06-07 14:40:00.000000 tree-ring-watermark-0.0.1/src/tree_ring_watermark/_check.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      164 2023-06-07 14:40:00.000000 tree-ring-watermark-0.0.1/src/tree_ring_watermark/_detect.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      149 2023-06-07 14:40:00.000000 tree-ring-watermark-0.0.1/src/tree_ring_watermark/_get_noise.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      274 2023-06-07 14:40:00.000000 tree-ring-watermark-0.0.1/src/tree_ring_watermark/dependency_versions_table.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-07 14:40:20.532415 tree-ring-watermark-0.0.1/src/tree_ring_watermark.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3408 2023-06-07 14:40:20.000000 tree-ring-watermark-0.0.1/src/tree_ring_watermark.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      459 2023-06-07 14:40:20.000000 tree-ring-watermark-0.0.1/src/tree_ring_watermark.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-06-07 14:40:20.000000 tree-ring-watermark-0.0.1/src/tree_ring_watermark.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       39 2023-06-07 14:40:20.000000 tree-ring-watermark-0.0.1/src/tree_ring_watermark.egg-info/requires.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       20 2023-06-07 14:40:20.000000 tree-ring-watermark-0.0.1/src/tree_ring_watermark.egg-info/top_level.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-07 14:59:12.449149 tree_ring_watermark-0.0.2/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1065 2023-06-07 14:16:59.000000 tree_ring_watermark-0.0.2/LICENSE.md
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3408 2023-06-07 14:59:12.449149 tree_ring_watermark-0.0.2/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2478 2023-06-07 14:16:59.000000 tree_ring_watermark-0.0.2/README.md
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-06-07 14:59:12.449149 tree_ring_watermark-0.0.2/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8190 2023-06-07 14:57:59.000000 tree_ring_watermark-0.0.2/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-07 14:59:12.449149 tree_ring_watermark-0.0.2/src/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-07 14:59:12.449149 tree_ring_watermark-0.0.2/src/tree_ring_watermark/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      111 2023-06-07 14:58:39.000000 tree_ring_watermark-0.0.2/src/tree_ring_watermark/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      107 2023-06-07 14:40:00.000000 tree_ring_watermark-0.0.2/src/tree_ring_watermark/_check.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      164 2023-06-07 14:40:00.000000 tree_ring_watermark-0.0.2/src/tree_ring_watermark/_detect.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      149 2023-06-07 14:40:00.000000 tree_ring_watermark-0.0.2/src/tree_ring_watermark/_get_noise.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      246 2023-06-07 14:56:48.000000 tree_ring_watermark-0.0.2/src/tree_ring_watermark/dependency_versions_table.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-07 14:59:12.449149 tree_ring_watermark-0.0.2/src/tree_ring_watermark.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3408 2023-06-07 14:59:12.000000 tree_ring_watermark-0.0.2/src/tree_ring_watermark.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      459 2023-06-07 14:59:12.000000 tree_ring_watermark-0.0.2/src/tree_ring_watermark.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-06-07 14:59:12.000000 tree_ring_watermark-0.0.2/src/tree_ring_watermark.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       53 2023-06-07 14:59:12.000000 tree_ring_watermark-0.0.2/src/tree_ring_watermark.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       20 2023-06-07 14:59:12.000000 tree_ring_watermark-0.0.2/src/tree_ring_watermark.egg-info/top_level.txt
```

### Comparing `tree-ring-watermark-0.0.1/LICENSE.md` & `tree_ring_watermark-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tree-ring-watermark-0.0.1/PKG-INFO` & `tree_ring_watermark-0.0.2/src/tree_ring_watermark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tree-ring-watermark
-Version: 0.0.1
-Summary: tree-ring-watermark
+Version: 0.0.2
+Summary: tree_ring_watermark
 Home-page: https://github.com/YuxinWenRick/tree-ring-watermark
 Author: Yuxin Wen
 Author-email: patrick@huggingface.co
 License: MIT
 Keywords: deep learning
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tree-ring-watermark-0.0.1/README.md` & `tree_ring_watermark-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tree-ring-watermark-0.0.1/setup.py` & `tree_ring_watermark-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -71,18 +71,17 @@
 from setuptools import find_packages, setup
 
 
 # IMPORTANT:
 # 1. all dependencies should be listed here with their version requirements if any
 # 2. once modified, run: `make deps_table_update` to update src/tree-ring-watermark/dependency_versions_table.py
 _deps = [
-    "tree-ring-watermark",
-    "accelerate",
-    "transformers",
-    "torch",
+   "torch==1.13.0",
+   "transformers==4.23.1",
+   "diffusers==0.11.1",
 ]
 
 # this is a lookup table with items like:
 #
 # tokenizers: "huggingface-hub==0.8.0"
 # packaging: "packaging"
 #
@@ -115,15 +114,15 @@
     A custom distutils command that updates the dependency table.
     usage: python setup.py deps_table_update
     """
 
     description = "build runtime dependency table"
     user_options = [
         # format: (long option, short option, description).
-        ("dep-table-update", None, "updates src/tree-ring-watermark/dependency_versions_table.py"),
+        ("dep-table-update", None, "updates src/tree_ring_watermark/dependency_versions_table.py"),
     ]
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
@@ -135,33 +134,33 @@
             "# 1. modify the `_deps` dict in setup.py",
             "# 2. run `make deps_table_update``",
             "deps = {",
             entries,
             "}",
             "",
         ]
-        target = "src/tree-ring-watermark/dependency_versions_table.py"
+        target = "src/tree_ring_watermark/dependency_versions_table.py"
         print(f"updating {target}")
         with open(target, "w", encoding="utf-8", newline="\n") as f:
             f.write("\n".join(content))
 
 
 extras = {}
 
 
 install_requires = [
     deps["torch"],
-    deps["tree-ring-watermark"],
+    deps["diffusers"],
     deps["transformers"],
 ]
 
 setup(
-    name="tree-ring-watermark",
-    version="0.0.1",
-    description="tree-ring-watermark",
+    name="tree_ring_watermark",
+    version="0.0.2",
+    description="tree_ring_watermark",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="MIT",
     author="Yuxin Wen",
     author_email="patrick@huggingface.co",
     url="https://github.com/YuxinWenRick/tree-ring-watermark",
```

### Comparing `tree-ring-watermark-0.0.1/src/tree_ring_watermark.egg-info/PKG-INFO` & `tree_ring_watermark-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: tree-ring-watermark
-Version: 0.0.1
-Summary: tree-ring-watermark
+Name: tree_ring_watermark
+Version: 0.0.2
+Summary: tree_ring_watermark
 Home-page: https://github.com/YuxinWenRick/tree-ring-watermark
 Author: Yuxin Wen
 Author-email: patrick@huggingface.co
 License: MIT
 Keywords: deep learning
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

