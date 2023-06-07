# Comparing `tmp/env2ini-0.0.1.tar.gz` & `tmp/env2ini-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env2ini-0.0.1.tar", last modified: Sun Jun  4 20:31:03 2023, max compression
+gzip compressed data, was "env2ini-0.0.2.tar", last modified: Wed Jun  7 13:48:41 2023, max compression
```

## Comparing `env2ini-0.0.1.tar` & `env2ini-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-04 20:31:03.519518 env2ini-0.0.1/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 env2ini-0.0.1/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 env2ini-0.0.1/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3003 2023-06-04 20:31:03.519387 env2ini-0.0.1/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2235 2023-06-04 20:24:39.000000 env2ini-0.0.1/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-04 20:31:03.518326 env2ini-0.0.1/env2ini/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    17391 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     5081 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/commands.py
--rw-r--r--   0 solst      (501) staff       (20)      451 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/conda.py
--rw-r--r--   0 solst      (501) staff       (20)      508 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/constants.py
--rw-r--r--   0 solst      (501) staff       (20)    18193 2023-06-04 18:19:59.000000 env2ini-0.0.1/env2ini/core.py
--rw-r--r--   0 solst      (501) staff       (20)    25487 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/dataclasses.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/files.py
--rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/paths.py
--rw-r--r--   0 solst      (501) staff       (20)     1203 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/rich.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/typer.py
--rw-r--r--   0 solst      (501) staff       (20)      868 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/types.py
--rw-r--r--   0 solst      (501) staff       (20)     1922 2023-06-04 20:29:02.000000 env2ini-0.0.1/env2ini/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-04 20:31:03.519202 env2ini-0.0.1/env2ini.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3003 2023-06-04 20:31:03.000000 env2ini-0.0.1/env2ini.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      506 2023-06-04 20:31:03.000000 env2ini-0.0.1/env2ini.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-04 20:31:03.000000 env2ini-0.0.1/env2ini.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)      106 2023-06-04 20:31:03.000000 env2ini-0.0.1/env2ini.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-04 13:37:46.000000 env2ini-0.0.1/env2ini.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       25 2023-06-04 20:31:03.000000 env2ini-0.0.1/env2ini.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        8 2023-06-04 20:31:03.000000 env2ini-0.0.1/env2ini.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      752 2023-06-04 19:44:10.000000 env2ini-0.0.1/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-04 20:31:03.519553 env2ini-0.0.1/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 env2ini-0.0.1/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 13:48:41.765676 env2ini-0.0.2/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 env2ini-0.0.2/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 env2ini-0.0.2/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     6759 2023-06-07 13:48:41.765542 env2ini-0.0.2/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     5991 2023-06-07 13:48:25.000000 env2ini-0.0.2/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 13:48:41.764429 env2ini-0.0.2/env2ini/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    17387 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     5069 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)      462 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/conda.py
+-rw-r--r--   0 solst      (501) staff       (20)      508 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/constants.py
+-rw-r--r--   0 solst      (501) staff       (20)    18193 2023-06-04 18:19:59.000000 env2ini-0.0.2/env2ini/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    25487 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/dataclasses.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/files.py
+-rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/paths.py
+-rw-r--r--   0 solst      (501) staff       (20)     1203 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)      868 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/types.py
+-rw-r--r--   0 solst      (501) staff       (20)     1918 2023-06-07 13:48:24.000000 env2ini-0.0.2/env2ini/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 13:48:41.765385 env2ini-0.0.2/env2ini.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     6759 2023-06-07 13:48:41.000000 env2ini-0.0.2/env2ini.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      506 2023-06-07 13:48:41.000000 env2ini-0.0.2/env2ini.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-07 13:48:41.000000 env2ini-0.0.2/env2ini.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)      106 2023-06-07 13:48:41.000000 env2ini-0.0.2/env2ini.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-04 13:37:46.000000 env2ini-0.0.2/env2ini.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       25 2023-06-07 13:48:41.000000 env2ini-0.0.2/env2ini.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        8 2023-06-07 13:48:41.000000 env2ini-0.0.2/env2ini.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      891 2023-06-07 13:48:20.000000 env2ini-0.0.2/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-07 13:48:41.765717 env2ini-0.0.2/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 env2ini-0.0.2/setup.py
```

### Comparing `env2ini-0.0.1/LICENSE` & `env2ini-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `env2ini-0.0.1/env2ini/_modidx.py` & `env2ini-0.0.2/env2ini/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,8 +141,8 @@
             'env2ini.types': {},
             'env2ini.utils': { 'env2ini.utils.is_valid_conda_package_name_char': ( 'utils.html#is_valid_conda_package_name_char',
                                                                                    'env2ini/utils.py'),
                                'env2ini.utils.parse_aliases': ('utils.html#parse_aliases', 'env2ini/utils.py'),
                                'env2ini.utils.read_ini_file': ('utils.html#read_ini_file', 'env2ini/utils.py'),
                                'env2ini.utils.split_package_str_at_first_non_alpha': ( 'utils.html#split_package_str_at_first_non_alpha',
                                                                                        'env2ini/utils.py'),
-                               'env2ini.utils.to_macos_env_file': ('utils.html#to_macos_env_file', 'env2ini/utils.py')}}}
+                               'env2ini.utils.to_mps_env_file': ('utils.html#to_mps_env_file', 'env2ini/utils.py')}}}
```

### Comparing `env2ini-0.0.1/env2ini/commands.py` & `env2ini-0.0.2/env2ini/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     PIP, DEP_SEP, PYPI_NAME, CONDA_NAME, 
     DEFAULT_DEPENDENCIES_TO_IGNORE, SETTINGS_INI,
     ENV_DEPENDENCIES, INI_REQUIREMENTS
 )
 
 from env2ini.utils import (
     split_package_str_at_first_non_alpha,
-    to_macos_env_file, parse_aliases
+    to_mps_env_file, parse_aliases
 )
 
 from env2ini.types import (
     YamlDependencyStr, IniRequirementStr, YamlFileItem, 
     YamlDependencies, Dependencies, CondaDependencies, IniRequirements
 )
 
@@ -51,17 +51,17 @@
     ),
 
     ini_file: Optional[str] = typer.Option(
         SETTINGS_INI, '--ini-file', '-i',
         help='The settings.ini file to update.',
     ),
 
-    macos: Optional[bool] = typer.Option(
-        False,'--macos', '-m',
-        help='Whether or not to use the macos env file. `{os.path.basename(file)}.mac.yml`.',
+    mps: Optional[bool] = typer.Option(
+        False,'--mps', '-m',
+        help='Whether or not to use the mps env file. `{os.path.basename(file)}.mps.yml`.',
     ),
 
     dryrun: Optional[bool] = typer.Option(
         False, '--dryrun', '-d',
         help='Whether to actually update the settings.ini file or just print the changes.',
     ),
 
@@ -82,19 +82,19 @@
 
     confirm: Optional[bool] = typer.Option(
         True, '--confirm', '-c',
         help='Ask for confirmation before writing to the ini file.',
     ),
     
 ):      
-    # NOTE: notice that file is `env.mac.yml` and not `env.yml`. Now with Apple Silicon I have 
+    # NOTE: notice that file is `env.mps.yml` and not `env.yml`. Now with Apple Silicon I have 
     #       one env file for more common CUDA versions and one for Apple Silicon.
     cprint('bold cyan', f'Loading environment yaml file {file}...')
-    if macos:
-        file = to_macos_env_file(file)
+    if mps:
+        file = to_mps_env_file(file)
         
     with open(file, 'r') as f:
         yml_env = yaml.safe_load(f)
     
     yml_ignore = yml_env.get('env2ini', {}).get('ignore', [])
     ignore = DEFAULT_DEPENDENCIES_TO_IGNORE + (dependencies_to_ignore or []) + yml_ignore
```

### Comparing `env2ini-0.0.1/env2ini/core.py` & `env2ini-0.0.2/env2ini/core.py`

 * *Files identical despite different names*

### Comparing `env2ini-0.0.1/env2ini/dataclasses.py` & `env2ini-0.0.2/env2ini/dataclasses.py`

 * *Files identical despite different names*

### Comparing `env2ini-0.0.1/env2ini/paths.py` & `env2ini-0.0.2/env2ini/paths.py`

 * *Files identical despite different names*

### Comparing `env2ini-0.0.1/env2ini/rich.py` & `env2ini-0.0.2/env2ini/rich.py`

 * *Files identical despite different names*

### Comparing `env2ini-0.0.1/env2ini/types.py` & `env2ini-0.0.2/env2ini/types.py`

 * *Files identical despite different names*

### Comparing `env2ini-0.0.1/env2ini/utils.py` & `env2ini-0.0.2/env2ini/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/04_utils.ipynb.
 
 # %% auto 0
-__all__ = ['read_ini_file', 'to_macos_env_file', 'is_valid_conda_package_name_char', 'split_package_str_at_first_non_alpha',
+__all__ = ['read_ini_file', 'to_mps_env_file', 'is_valid_conda_package_name_char', 'split_package_str_at_first_non_alpha',
            'parse_aliases']
 
 # %% ../nbs/04_utils.ipynb 3
 import os
 import configparser
 from typing import (Tuple, Optional)
 
@@ -14,15 +14,15 @@
 
 # %% ../nbs/04_utils.ipynb 5
 def read_ini_file(file: str = SETTINGS_INI) -> configparser.ConfigParser:    
     ini_cfg = configparser.ConfigParser()
     ini_cfg.read_file(file)    
     return ini_cfg
 
-def to_macos_env_file(file: str) -> str:
+def to_mps_env_file(file: str) -> str:
     base_dir = os.path.dirname(file)
     yml_file = os.path.basename(file)
     mac_file = yml_file.replace('.yml', '.mac.yml')
     
 
     if os.path.exists(os.path.join(base_dir, mac_file)):
         return os.path.join(base_dir, mac_file)
```

### Comparing `env2ini-0.0.1/setup.py` & `env2ini-0.0.2/setup.py`

 * *Files identical despite different names*

