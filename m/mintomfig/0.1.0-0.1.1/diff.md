# Comparing `tmp/mintomfig-0.1.0.tar.gz` & `tmp/mintomfig-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mintomfig-0.1.0.tar", max compression
+gzip compressed data, was "mintomfig-0.1.1.tar", max compression
```

## Comparing `mintomfig-0.1.0.tar` & `mintomfig-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       30 2023-06-07 19:02:13.667768 mintomfig-0.1.0/README.md
--rw-r--r--   0        0        0     1866 2023-06-07 19:10:52.117861 mintomfig-0.1.0/mintomfig/__init__.py
--rw-r--r--   0        0        0      295 2023-06-07 19:11:22.787125 mintomfig-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 mintomfig-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-07 19:02:13.667768 mintomfig-0.1.1/README.md
+-rw-r--r--   0        0        0     1770 2023-06-07 19:17:57.853322 mintomfig-0.1.1/mintomfig/__init__.py
+-rw-r--r--   0        0        0      295 2023-06-07 19:18:16.276402 mintomfig-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 mintomfig-0.1.1/PKG-INFO
```

### Comparing `mintomfig-0.1.0/mintomfig/__init__.py` & `mintomfig-0.1.1/mintomfig/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,17 +48,14 @@
         return table[key]
 
     def load_from(self, config_path, wizard_callback=None) -> bool:
         # ensure the config file exists
         if not os.path.exists(config_path):
             # show a wizard to create the config file
             if wizard_callback:
-                wizard_callback(config_path)
-
-            # if the config file still doesn't exist, fail
-            if not os.path.exists(config_path):
-                return False
+                if not wizard_callback(config_path):
+                    return False
 
         with open(config_path, "r") as conf_file:
             self.config = toml.load(conf_file)
 
         return True
```

### Comparing `mintomfig-0.1.0/PKG-INFO` & `mintomfig-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mintomfig
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: redthing1
 Author-email: redthing1@alt.icu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

