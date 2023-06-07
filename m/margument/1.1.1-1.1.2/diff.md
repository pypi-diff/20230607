# Comparing `tmp/margument-1.1.1.tar.gz` & `tmp/margument-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "margument-1.1.1.tar", last modified: Sun Apr  9 11:58:01 2023, max compression
+gzip compressed data, was "margument-1.1.2.tar", last modified: Wed Jun  7 21:31:42 2023, max compression
```

## Comparing `margument-1.1.1.tar` & `margument-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:58:01.110774 margument-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-09 11:57:46.000000 margument-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-09 11:58:01.110774 margument-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-09 11:57:46.000000 margument-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:58:01.110774 margument-1.1.1/margument/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:57:46.000000 margument-1.1.1/margument/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-09 11:57:46.000000 margument-1.1.1/margument/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-09 11:57:46.000000 margument-1.1.1/margument/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-09 11:57:46.000000 margument-1.1.1/margument/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-09 11:57:46.000000 margument-1.1.1/margument/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-09 11:57:46.000000 margument-1.1.1/margument/non_repeatable_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-09 11:57:46.000000 margument-1.1.1/margument/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-09 11:57:46.000000 margument-1.1.1/margument/reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-09 11:57:46.000000 margument-1.1.1/margument/repeatable_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-09 11:57:46.000000 margument-1.1.1/margument/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-09 11:57:46.000000 margument-1.1.1/margument/settings_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:58:01.110774 margument-1.1.1/margument/version/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:57:46.000000 margument-1.1.1/margument/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 11:57:46.000000 margument-1.1.1/margument/version/progsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-09 11:57:46.000000 margument-1.1.1/margument/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:58:01.110774 margument-1.1.1/margument.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-09 11:58:01.000000 margument-1.1.1/margument.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-09 11:58:01.000000 margument-1.1.1/margument.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:58:01.000000 margument-1.1.1/margument.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 11:58:01.000000 margument-1.1.1/margument.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 11:58:01.000000 margument-1.1.1/margument.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:58:01.114774 margument-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-09 11:57:46.000000 margument-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:42.863498 margument-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-07 21:31:30.000000 margument-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-06-07 21:31:42.859497 margument-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-06-07 21:31:30.000000 margument-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:42.859497 margument-1.1.2/margument/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:30.000000 margument-1.1.2/margument/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-07 21:31:30.000000 margument-1.1.2/margument/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-07 21:31:30.000000 margument-1.1.2/margument/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-07 21:31:30.000000 margument-1.1.2/margument/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-07 21:31:30.000000 margument-1.1.2/margument/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-07 21:31:30.000000 margument-1.1.2/margument/non_repeatable_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-07 21:31:30.000000 margument-1.1.2/margument/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-07 21:31:30.000000 margument-1.1.2/margument/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-07 21:31:30.000000 margument-1.1.2/margument/repeatable_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-07 21:31:30.000000 margument-1.1.2/margument/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-07 21:31:30.000000 margument-1.1.2/margument/settings_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:42.859497 margument-1.1.2/margument/version/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:30.000000 margument-1.1.2/margument/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-07 21:31:30.000000 margument-1.1.2/margument/version/progsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 21:31:30.000000 margument-1.1.2/margument/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:42.859497 margument-1.1.2/margument.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-06-07 21:31:42.000000 margument-1.1.2/margument.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-07 21:31:42.000000 margument-1.1.2/margument.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:31:42.000000 margument-1.1.2/margument.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 21:31:42.000000 margument-1.1.2/margument.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 21:31:42.000000 margument-1.1.2/margument.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:31:42.863498 margument-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-07 21:31:30.000000 margument-1.1.2/setup.py
```

### Comparing `margument-1.1.1/LICENSE` & `margument-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `margument-1.1.1/PKG-INFO` & `margument-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: margument
-Version: 1.1.1
+Version: 1.1.2
 Summary: python library to manage configurations from program arguments including doing commands and saving configurations in a yaml file.
 Home-page: https://github.com/zaytiri/settings-manager
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/settings-manager
 Project-URL: Changelog, https://github.com/zaytiri/settings-manager/blob/main/CHANGELOG.md
 Keywords: manager,configurations,settings,arguments,argparse,yaml,save
 Classifier: Environment :: Console
```

### Comparing `margument-1.1.1/README.md` & `margument-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `margument-1.1.1/margument/argument.py` & `margument-1.1.2/margument/argument.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.1/margument/arguments.py` & `margument-1.1.2/margument/arguments.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.1/margument/file.py` & `margument-1.1.2/margument/file.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.1/margument/non_repeatable_settings.py` & `margument-1.1.2/margument/non_repeatable_settings.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.1/margument/options.py` & `margument-1.1.2/margument/options.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.1/margument/repeatable_settings.py` & `margument-1.1.2/margument/repeatable_settings.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.1/margument/settings.py` & `margument-1.1.2/margument/settings.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.1/margument/settings_processor.py` & `margument-1.1.2/margument/settings_processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         """
         for setting in self.settings:
             setting.program_arguments.add_arguments(self.args_parser)
 
         user_arguments = None
         try:
             user_arguments = self.args_parser.parse_args()
-        except AssertionError:
-            throw("Required arguments were not specified.")
+        except AssertionError as ex:
+            throw(ex)
 
         parsed_settings = {}
         for setting in self.settings:
             setting.user_arguments = user_arguments
 
             setting.program_arguments.process_arguments(self.settings)
```

### Comparing `margument-1.1.1/margument.egg-info/PKG-INFO` & `margument-1.1.2/margument.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: margument
-Version: 1.1.1
+Version: 1.1.2
 Summary: python library to manage configurations from program arguments including doing commands and saving configurations in a yaml file.
 Home-page: https://github.com/zaytiri/settings-manager
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/settings-manager
 Project-URL: Changelog, https://github.com/zaytiri/settings-manager/blob/main/CHANGELOG.md
 Keywords: manager,configurations,settings,arguments,argparse,yaml,save
 Classifier: Environment :: Console
```

### Comparing `margument-1.1.1/margument.egg-info/SOURCES.txt` & `margument-1.1.2/margument.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `margument-1.1.1/setup.py` & `margument-1.1.2/setup.py`

 * *Files identical despite different names*

