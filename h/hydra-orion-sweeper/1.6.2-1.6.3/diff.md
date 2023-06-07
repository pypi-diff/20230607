# Comparing `tmp/hydra-orion-sweeper-1.6.2.tar.gz` & `tmp/hydra-orion-sweeper-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra-orion-sweeper-1.6.2.tar", last modified: Tue Apr 11 15:23:53 2023, max compression
+gzip compressed data, was "hydra-orion-sweeper-1.6.3.tar", last modified: Wed Jun  7 15:07:38 2023, max compression
```

## Comparing `hydra-orion-sweeper-1.6.2.tar` & `hydra-orion-sweeper-1.6.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-11 15:23:53.000000 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 15:23:53.000000 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:23:53.000000 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 15:23:53.000000 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 15:23:53.000000 hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/hydra_plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20253 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/orion_sweeper.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:23:53.533922 hydra-orion-sweeper-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-11 15:23:01.000000 hydra-orion-sweeper-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:07:38.781648 hydra-orion-sweeper-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-07 15:06:44.000000 hydra-orion-sweeper-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-07 15:07:38.781648 hydra-orion-sweeper-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-07 15:06:44.000000 hydra-orion-sweeper-1.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:07:38.777648 hydra-orion-sweeper-1.6.3/hydra_orion_sweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-07 15:07:38.000000 hydra-orion-sweeper-1.6.3/hydra_orion_sweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-07 15:07:38.000000 hydra-orion-sweeper-1.6.3/hydra_orion_sweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:07:38.000000 hydra-orion-sweeper-1.6.3/hydra_orion_sweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 15:07:38.000000 hydra-orion-sweeper-1.6.3/hydra_orion_sweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 15:07:38.000000 hydra-orion-sweeper-1.6.3/hydra_orion_sweeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:07:38.777648 hydra-orion-sweeper-1.6.3/hydra_plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:07:38.781648 hydra-orion-sweeper-1.6.3/hydra_plugins/hydra_orion_sweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-07 15:06:44.000000 hydra-orion-sweeper-1.6.3/hydra_plugins/hydra_orion_sweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-07 15:06:44.000000 hydra-orion-sweeper-1.6.3/hydra_plugins/hydra_orion_sweeper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20580 2023-06-07 15:06:44.000000 hydra-orion-sweeper-1.6.3/hydra_plugins/hydra_orion_sweeper/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-07 15:06:44.000000 hydra-orion-sweeper-1.6.3/hydra_plugins/hydra_orion_sweeper/orion_sweeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:07:38.781648 hydra-orion-sweeper-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-07 15:06:44.000000 hydra-orion-sweeper-1.6.3/setup.py
```

### Comparing `hydra-orion-sweeper-1.6.2/PKG-INFO` & `hydra-orion-sweeper-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-orion-sweeper
-Version: 1.6.2
+Version: 1.6.3
 Summary: Hydra Orion Sweeper plugin
 Home-page: https://orion.readthedocs.io/
 Author: Pierre Delaunay
 Author-email: pierre.delaunay@mila.quebec
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hydra-orion-sweeper-1.6.2/README.rst` & `hydra-orion-sweeper-1.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `hydra-orion-sweeper-1.6.2/hydra_orion_sweeper.egg-info/PKG-INFO` & `hydra-orion-sweeper-1.6.3/hydra_orion_sweeper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-orion-sweeper
-Version: 1.6.2
+Version: 1.6.3
 Summary: Hydra Orion Sweeper plugin
 Home-page: https://orion.readthedocs.io/
 Author: Pierre Delaunay
 Author-email: pierre.delaunay@mila.quebec
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/config.py` & `hydra-orion-sweeper-1.6.3/hydra_plugins/hydra_orion_sweeper/config.py`

 * *Files identical despite different names*

### Comparing `hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/implementation.py` & `hydra-orion-sweeper-1.6.3/hydra_plugins/hydra_orion_sweeper/implementation.py`

 * *Files 5% similar despite different names*

```diff
@@ -262,37 +262,47 @@
         for arg in arguments:
             if NESTED_DIM_REGEX.match(arg):
                 name, rest = arg.split(".", 1)
                 nested_overrides[name].append(rest)
             else:
                 regular_args.append(arg)
 
-        parser = override_parser()
-        parsed = parser.parse_overrides(regular_args)
-
+        error = None
         for name, nestedargs in nested_overrides.items():
             suboverrides = dict()
             subargs = dict()
 
-            self._recursive_overrides(subargs, suboverrides, nestedargs)
+            error = self._recursive_overrides(subargs, suboverrides, nestedargs)
 
             if subargs:
                 args[name] = subargs
 
             if suboverrides:
                 overrides[name] = suboverrides
 
+            if error:
+                # Not a subdim
+                regular_args.append(f"{name}.{nestedargs[0]}")
+            else:
+                error = (name, nestedargs)
+
+        parser = override_parser()
+        parsed = parser.parse_overrides(regular_args)
+        parser = override_parser()
+        parsed = parser.parse_overrides(regular_args)
         for override in parsed:
             dim = self.process_overrides(override)
 
             if dim is None:
                 args[override.get_key_element()] = override.value()
             else:
                 overrides[dim.name] = dim.get_prior_string()
 
+        return error
+
     def process_overrides(self, override: Override) -> Dimension:
         """Identify the sweep overrides and build a matching dimension"""
         values = override.value()
         name = override.get_key_element()
 
         def build_dim(name):
             builder = DimensionBuilder()
```

### Comparing `hydra-orion-sweeper-1.6.2/hydra_plugins/hydra_orion_sweeper/orion_sweeper.py` & `hydra-orion-sweeper-1.6.3/hydra_plugins/hydra_orion_sweeper/orion_sweeper.py`

 * *Files identical despite different names*

### Comparing `hydra-orion-sweeper-1.6.2/setup.py` & `hydra-orion-sweeper-1.6.3/setup.py`

 * *Files identical despite different names*

