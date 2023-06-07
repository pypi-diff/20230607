# Comparing `tmp/dtorch-0.0.1.tar.gz` & `tmp/dtorch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtorch-0.0.1.tar", last modified: Tue Jun  6 09:48:42 2023, max compression
+gzip compressed data, was "dtorch-0.0.2.tar", last modified: Wed Jun  7 08:36:02 2023, max compression
```

## Comparing `dtorch-0.0.1.tar` & `dtorch-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-06 09:48:42.397788 dtorch-0.0.1/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1067 2023-06-06 07:48:12.000000 dtorch-0.0.1/LICENSE
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      537 2023-06-06 09:48:42.397788 dtorch-0.0.1/PKG-INFO
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       28 2023-06-06 09:03:30.000000 dtorch-0.0.1/README.md
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-06 09:48:42.394455 dtorch-0.0.1/dtorch/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      176 2023-06-06 07:59:44.000000 dtorch-0.0.1/dtorch/__init__.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1146 2023-06-06 09:01:03.000000 dtorch-0.0.1/dtorch/dataset.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    13723 2023-06-06 09:01:03.000000 dtorch-0.0.1/dtorch/derivatives.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1979 2023-06-06 09:01:03.000000 dtorch-0.0.1/dtorch/einops.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     8970 2023-06-06 09:01:03.000000 dtorch-0.0.1/dtorch/functionnal.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    10586 2023-06-06 09:01:03.000000 dtorch-0.0.1/dtorch/jtensors.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2691 2023-06-06 09:01:03.000000 dtorch-0.0.1/dtorch/loss.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    11642 2023-06-06 09:01:03.000000 dtorch-0.0.1/dtorch/nn.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      218 2023-06-06 07:48:45.000000 dtorch-0.0.1/dtorch/operation_class.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      940 2023-06-06 09:01:03.000000 dtorch-0.0.1/dtorch/operations.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2698 2023-06-06 09:01:03.000000 dtorch-0.0.1/dtorch/optim.py
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-06 09:48:42.397788 dtorch-0.0.1/dtorch.egg-info/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      537 2023-06-06 09:48:42.000000 dtorch-0.0.1/dtorch.egg-info/PKG-INFO
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      360 2023-06-06 09:48:42.000000 dtorch-0.0.1/dtorch.egg-info/SOURCES.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        1 2023-06-06 09:48:42.000000 dtorch-0.0.1/dtorch.egg-info/dependency_links.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        7 2023-06-06 09:48:42.000000 dtorch-0.0.1/dtorch.egg-info/top_level.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      616 2023-06-06 09:48:17.000000 dtorch-0.0.1/pyproject.toml
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       38 2023-06-06 09:48:42.397788 dtorch-0.0.1/setup.cfg
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-07 08:36:02.822552 dtorch-0.0.2/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1067 2023-06-06 07:48:12.000000 dtorch-0.0.2/LICENSE
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      529 2023-06-07 08:36:02.822552 dtorch-0.0.2/PKG-INFO
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       21 2023-06-06 10:00:34.000000 dtorch-0.0.2/README.md
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-07 08:36:02.822552 dtorch-0.0.2/dtorch/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      176 2023-06-06 10:00:04.000000 dtorch-0.0.2/dtorch/__init__.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1146 2023-06-06 10:00:04.000000 dtorch-0.0.2/dtorch/dataset.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    13723 2023-06-06 10:00:04.000000 dtorch-0.0.2/dtorch/derivatives.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1979 2023-06-06 10:00:04.000000 dtorch-0.0.2/dtorch/einops.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     8970 2023-06-06 10:00:04.000000 dtorch-0.0.2/dtorch/functionnal.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    10586 2023-06-06 10:00:04.000000 dtorch-0.0.2/dtorch/jtensors.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2691 2023-06-06 10:00:04.000000 dtorch-0.0.2/dtorch/loss.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    11642 2023-06-06 10:00:04.000000 dtorch-0.0.2/dtorch/nn.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      218 2023-06-06 10:00:04.000000 dtorch-0.0.2/dtorch/operation_class.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      940 2023-06-06 10:00:04.000000 dtorch-0.0.2/dtorch/operations.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2698 2023-06-06 10:00:04.000000 dtorch-0.0.2/dtorch/optim.py
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-07 08:36:02.822552 dtorch-0.0.2/dtorch.egg-info/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      529 2023-06-07 08:36:02.000000 dtorch-0.0.2/dtorch.egg-info/PKG-INFO
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      360 2023-06-07 08:36:02.000000 dtorch-0.0.2/dtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        1 2023-06-07 08:36:02.000000 dtorch-0.0.2/dtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        7 2023-06-07 08:36:02.000000 dtorch-0.0.2/dtorch.egg-info/top_level.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      616 2023-06-07 08:35:55.000000 dtorch-0.0.2/pyproject.toml
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       38 2023-06-07 08:36:02.822552 dtorch-0.0.2/setup.cfg
```

### Comparing `dtorch-0.0.1/LICENSE` & `dtorch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.1/PKG-INFO` & `dtorch-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dtorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A scientific package made a fellow student
 Author-email: Just1truc <hyppoduc@gmail.com>
 Project-URL: Homepage, https://github.com/Just1truc/dtorch
 Project-URL: Bug Tracker, https://github.com/Just1truc/dtorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# JTorch
-The package is here
+# DTorch
+The package
```

### Comparing `dtorch-0.0.1/dtorch/dataset.py` & `dtorch-0.0.2/dtorch/dataset.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.1/dtorch/derivatives.py` & `dtorch-0.0.2/dtorch/derivatives.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.1/dtorch/einops.py` & `dtorch-0.0.2/dtorch/einops.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.1/dtorch/functionnal.py` & `dtorch-0.0.2/dtorch/functionnal.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.1/dtorch/jtensors.py` & `dtorch-0.0.2/dtorch/jtensors.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.1/dtorch/loss.py` & `dtorch-0.0.2/dtorch/loss.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.1/dtorch/nn.py` & `dtorch-0.0.2/dtorch/nn.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.1/dtorch/operations.py` & `dtorch-0.0.2/dtorch/operations.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.1/dtorch/optim.py` & `dtorch-0.0.2/dtorch/optim.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.1/dtorch.egg-info/PKG-INFO` & `dtorch-0.0.2/dtorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dtorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A scientific package made a fellow student
 Author-email: Just1truc <hyppoduc@gmail.com>
 Project-URL: Homepage, https://github.com/Just1truc/dtorch
 Project-URL: Bug Tracker, https://github.com/Just1truc/dtorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# JTorch
-The package is here
+# DTorch
+The package
```

### Comparing `dtorch-0.0.1/pyproject.toml` & `dtorch-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["dtorch"]
 
 [project]
 name = "dtorch"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Just1truc", email="hyppoduc@gmail.com" },
 ]
 description = "A scientific package made a fellow student"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

