# Comparing `tmp/litenv-0.0.2.tar.gz` & `tmp/litenv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litenv-0.0.2.tar", last modified: Wed Jun  7 13:24:19 2023, max compression
+gzip compressed data, was "litenv-0.0.3.tar", last modified: Wed Jun  7 18:37:41 2023, max compression
```

## Comparing `litenv-0.0.2.tar` & `litenv-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 13:24:19.136098 litenv-0.0.2/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 litenv-0.0.2/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 litenv-0.0.2/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     8078 2023-06-07 13:24:19.135953 litenv-0.0.2/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     7302 2023-06-07 13:13:47.000000 litenv-0.0.2/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 13:24:19.135729 litenv-0.0.2/data/
--rw-r--r--   0 solst      (501) staff       (20)     4773 2023-06-07 13:05:11.000000 litenv-0.0.2/data/litenv.yml
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 13:24:19.134656 litenv-0.0.2/litenv/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    25532 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     3947 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/commands.py
--rw-r--r--   0 solst      (501) staff       (20)     2408 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/constants.py
--rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-05 12:16:38.000000 litenv-0.0.2/litenv/core.py
--rw-r--r--   0 solst      (501) staff       (20)    24474 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/dataclasses.py
--rw-r--r--   0 solst      (501) staff       (20)    11704 2023-06-05 22:16:07.000000 litenv-0.0.2/litenv/defaults.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/files.py
--rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/paths.py
--rw-r--r--   0 solst      (501) staff       (20)      977 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/rich.py
--rw-r--r--   0 solst      (501) staff       (20)      216 2023-06-05 22:16:07.000000 litenv-0.0.2/litenv/tests.py
--rw-r--r--   0 solst      (501) staff       (20)     4104 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/themes.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/typer.py
--rw-r--r--   0 solst      (501) staff       (20)      269 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/types.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/utils.py
--rw-r--r--   0 solst      (501) staff       (20)     5788 2023-06-06 17:57:47.000000 litenv-0.0.2/litenv/yml.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 13:24:19.135603 litenv-0.0.2/litenv.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     8078 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      562 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       96 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-05 14:20:25.000000 litenv-0.0.2/litenv.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       37 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      933 2023-06-07 13:23:47.000000 litenv-0.0.2/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-07 13:24:19.136140 litenv-0.0.2/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2671 2023-06-05 19:37:38.000000 litenv-0.0.2/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 18:37:41.259639 litenv-0.0.3/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 litenv-0.0.3/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 litenv-0.0.3/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-07 18:37:41.259461 litenv-0.0.3/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     7305 2023-06-07 17:36:08.000000 litenv-0.0.3/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 18:37:41.259064 litenv-0.0.3/data/
+-rw-r--r--   0 solst      (501) staff       (20)     4773 2023-06-07 13:05:11.000000 litenv-0.0.3/data/litenv.yml
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 18:37:41.256857 litenv-0.0.3/litenv/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    25532 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     3947 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)     2408 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/constants.py
+-rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-05 12:16:38.000000 litenv-0.0.3/litenv/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    24475 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/dataclasses.py
+-rw-r--r--   0 solst      (501) staff       (20)    11704 2023-06-05 22:16:07.000000 litenv-0.0.3/litenv/defaults.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/files.py
+-rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/paths.py
+-rw-r--r--   0 solst      (501) staff       (20)      977 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)      216 2023-06-05 22:16:07.000000 litenv-0.0.3/litenv/tests.py
+-rw-r--r--   0 solst      (501) staff       (20)     4104 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/themes.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)      269 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/types.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-07 18:37:16.000000 litenv-0.0.3/litenv/utils.py
+-rw-r--r--   0 solst      (501) staff       (20)     5788 2023-06-06 17:57:47.000000 litenv-0.0.3/litenv/yml.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 18:37:41.258891 litenv-0.0.3/litenv.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      562 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       96 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-05 14:20:25.000000 litenv-0.0.3/litenv.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       37 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-07 18:37:41.000000 litenv-0.0.3/litenv.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      933 2023-06-07 18:37:11.000000 litenv-0.0.3/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-07 18:37:41.259690 litenv-0.0.3/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2671 2023-06-05 19:37:38.000000 litenv-0.0.3/setup.py
```

### Comparing `litenv-0.0.2/LICENSE` & `litenv-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `litenv-0.0.2/PKG-INFO` & `litenv-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litenv
-Version: 0.0.2
+Version: 0.0.3
 Summary: quickly make pytorch environments with mamba
 Home-page: https://github.com/dsm-72/litenv
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -58,15 +58,15 @@
 
 # make sure the litenv package is installed in development mode
 $ pip install -e .
 
 # make changes under nbs/ directory
 # ...
 
-# compile to have changes apply to the ivanova package
+# compile to have changes apply to the litenv package
 $ nbdev_prepare
 ```
 
 ### Publishing
 
 ``` sh
 # publish to pypi
@@ -141,28 +141,28 @@
 ### Structure of the Specification File
 
 #### `python`
 
 The `python` field specifies the required Python version for the
 application. For example:
 
-``` yml
+``` yaml
 python: '>=3.10'
 ```
 
 This entry implies that the application requires a Python version of
 3.10 or higher.
 
 #### `channels`
 
 This field specifies additional channels that might be needed for your
 application. Channels in Python are paths where packages are stored and
 can be accessed when needed. For example:
 
-``` yml
+``` yaml
 channels:  
   - pytorch
   - conda-forge  
 ```
 
 This implies that packages for the application may be sourced from the
 `pytorch` or `conda-forge` channels.
@@ -179,15 +179,15 @@
 
 Each dependency could optionally include attributes such as `channel`,
 `note`, `always`, `pypi_name`, `cuda_only`, `version`, `pip_only` and
 `no_arm_support`.
 
 For example:
 
-``` yml
+``` yaml
 categories:
   utils:
     name: 'Utilities'
     checked: true
     dependencies:
       tqdm:
         always: true
@@ -201,15 +201,15 @@
 
 #### `accelerators`
 
 The `accelerators` field specifies the type of hardware accelerator that
 your application supports. This includes options like ‘mps’, ‘cpu’, or
 ‘cuda’.
 
-``` yml
+``` yaml
 accelerators:
   - mps
   - cpu
   - cuda
 ```
 
 This entry implies that the application can use either MPS, CPU, or CUDA
```

### Comparing `litenv-0.0.2/README.md` & `litenv-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 # make sure the litenv package is installed in development mode
 $ pip install -e .
 
 # make changes under nbs/ directory
 # ...
 
-# compile to have changes apply to the ivanova package
+# compile to have changes apply to the litenv package
 $ nbdev_prepare
 ```
 
 ### Publishing
 
 ``` sh
 # publish to pypi
@@ -119,28 +119,28 @@
 ### Structure of the Specification File
 
 #### `python`
 
 The `python` field specifies the required Python version for the
 application. For example:
 
-``` yml
+``` yaml
 python: '>=3.10'
 ```
 
 This entry implies that the application requires a Python version of
 3.10 or higher.
 
 #### `channels`
 
 This field specifies additional channels that might be needed for your
 application. Channels in Python are paths where packages are stored and
 can be accessed when needed. For example:
 
-``` yml
+``` yaml
 channels:  
   - pytorch
   - conda-forge  
 ```
 
 This implies that packages for the application may be sourced from the
 `pytorch` or `conda-forge` channels.
@@ -157,15 +157,15 @@
 
 Each dependency could optionally include attributes such as `channel`,
 `note`, `always`, `pypi_name`, `cuda_only`, `version`, `pip_only` and
 `no_arm_support`.
 
 For example:
 
-``` yml
+``` yaml
 categories:
   utils:
     name: 'Utilities'
     checked: true
     dependencies:
       tqdm:
         always: true
@@ -179,15 +179,15 @@
 
 #### `accelerators`
 
 The `accelerators` field specifies the type of hardware accelerator that
 your application supports. This includes options like ‘mps’, ‘cpu’, or
 ‘cuda’.
 
-``` yml
+``` yaml
 accelerators:
   - mps
   - cpu
   - cuda
 ```
 
 This entry implies that the application can use either MPS, CPU, or CUDA
```

### Comparing `litenv-0.0.2/data/litenv.yml` & `litenv-0.0.3/data/litenv.yml`

 * *Files identical despite different names*

### Comparing `litenv-0.0.2/litenv/_modidx.py` & `litenv-0.0.3/litenv/_modidx.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.2/litenv/commands.py` & `litenv-0.0.3/litenv/commands.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.2/litenv/constants.py` & `litenv-0.0.3/litenv/constants.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.2/litenv/dataclasses.py` & `litenv-0.0.3/litenv/dataclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -653,15 +653,15 @@
             cnd_deps.append(dict(pip=pip_deps))
 
     
         all_deps = self.categories.get_selected_dependencies(selected)
         all_deps = EnvDeps(dependencies=all_deps)
         channels = all_deps.determine_needed_channels(accel, possible_channels=self.channels)
 
-        res = dict(name=name, channels=channels, dependecies=cnd_deps)
+        res = dict(name=name, channels=channels, dependencies=cnd_deps)
         return res
 
 
     def dict_to_str(self, env_dict:dict) -> str:        
         env_str = yaml.dump(env_dict, width=float('inf'), sort_keys=False)
 
         env_lines = []
```

### Comparing `litenv-0.0.2/litenv/defaults.py` & `litenv-0.0.3/litenv/defaults.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.2/litenv/paths.py` & `litenv-0.0.3/litenv/paths.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.2/litenv/rich.py` & `litenv-0.0.3/litenv/rich.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.2/litenv/themes.py` & `litenv-0.0.3/litenv/themes.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.2/litenv/yml.py` & `litenv-0.0.3/litenv/yml.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.2/litenv.egg-info/PKG-INFO` & `litenv-0.0.3/litenv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litenv
-Version: 0.0.2
+Version: 0.0.3
 Summary: quickly make pytorch environments with mamba
 Home-page: https://github.com/dsm-72/litenv
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -58,15 +58,15 @@
 
 # make sure the litenv package is installed in development mode
 $ pip install -e .
 
 # make changes under nbs/ directory
 # ...
 
-# compile to have changes apply to the ivanova package
+# compile to have changes apply to the litenv package
 $ nbdev_prepare
 ```
 
 ### Publishing
 
 ``` sh
 # publish to pypi
@@ -141,28 +141,28 @@
 ### Structure of the Specification File
 
 #### `python`
 
 The `python` field specifies the required Python version for the
 application. For example:
 
-``` yml
+``` yaml
 python: '>=3.10'
 ```
 
 This entry implies that the application requires a Python version of
 3.10 or higher.
 
 #### `channels`
 
 This field specifies additional channels that might be needed for your
 application. Channels in Python are paths where packages are stored and
 can be accessed when needed. For example:
 
-``` yml
+``` yaml
 channels:  
   - pytorch
   - conda-forge  
 ```
 
 This implies that packages for the application may be sourced from the
 `pytorch` or `conda-forge` channels.
@@ -179,15 +179,15 @@
 
 Each dependency could optionally include attributes such as `channel`,
 `note`, `always`, `pypi_name`, `cuda_only`, `version`, `pip_only` and
 `no_arm_support`.
 
 For example:
 
-``` yml
+``` yaml
 categories:
   utils:
     name: 'Utilities'
     checked: true
     dependencies:
       tqdm:
         always: true
@@ -201,15 +201,15 @@
 
 #### `accelerators`
 
 The `accelerators` field specifies the type of hardware accelerator that
 your application supports. This includes options like ‘mps’, ‘cpu’, or
 ‘cuda’.
 
-``` yml
+``` yaml
 accelerators:
   - mps
   - cpu
   - cuda
 ```
 
 This entry implies that the application can use either MPS, CPU, or CUDA
```

### Comparing `litenv-0.0.2/litenv.egg-info/SOURCES.txt` & `litenv-0.0.3/litenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litenv-0.0.2/settings.ini` & `litenv-0.0.3/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = litenv
 lib_name = litenv
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = litenv
 nbs_path = nbs
 recursive = True
```

### Comparing `litenv-0.0.2/setup.py` & `litenv-0.0.3/setup.py`

 * *Files identical despite different names*

