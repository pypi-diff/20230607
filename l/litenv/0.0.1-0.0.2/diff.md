# Comparing `tmp/litenv-0.0.1.tar.gz` & `tmp/litenv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litenv-0.0.1.tar", last modified: Tue Jun  6 20:52:37 2023, max compression
+gzip compressed data, was "litenv-0.0.2.tar", last modified: Wed Jun  7 13:24:19 2023, max compression
```

## Comparing `litenv-0.0.1.tar` & `litenv-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-06 20:52:37.220706 litenv-0.0.1/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 litenv-0.0.1/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 litenv-0.0.1/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1531 2023-06-06 20:52:37.220557 litenv-0.0.1/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      755 2023-06-05 15:03:37.000000 litenv-0.0.1/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-06 20:52:37.220329 litenv-0.0.1/data/
--rw-r--r--   0 solst      (501) staff       (20)     4467 2023-06-06 19:48:58.000000 litenv-0.0.1/data/litenv.yml
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-06 20:52:37.218746 litenv-0.0.1/litenv/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    25532 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     3947 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/commands.py
--rw-r--r--   0 solst      (501) staff       (20)     2408 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/constants.py
--rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-05 12:16:38.000000 litenv-0.0.1/litenv/core.py
--rw-r--r--   0 solst      (501) staff       (20)    24145 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/dataclasses.py
--rw-r--r--   0 solst      (501) staff       (20)    11704 2023-06-05 22:16:07.000000 litenv-0.0.1/litenv/defaults.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/files.py
--rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/paths.py
--rw-r--r--   0 solst      (501) staff       (20)      977 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/rich.py
--rw-r--r--   0 solst      (501) staff       (20)      216 2023-06-05 22:16:07.000000 litenv-0.0.1/litenv/tests.py
--rw-r--r--   0 solst      (501) staff       (20)     4104 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/themes.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/typer.py
--rw-r--r--   0 solst      (501) staff       (20)      269 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/types.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-06 20:21:17.000000 litenv-0.0.1/litenv/utils.py
--rw-r--r--   0 solst      (501) staff       (20)     5788 2023-06-06 17:57:47.000000 litenv-0.0.1/litenv/yml.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-06 20:52:37.220074 litenv-0.0.1/litenv.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1531 2023-06-06 20:52:37.000000 litenv-0.0.1/litenv.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      562 2023-06-06 20:52:37.000000 litenv-0.0.1/litenv.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-06 20:52:37.000000 litenv-0.0.1/litenv.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       96 2023-06-06 20:52:37.000000 litenv-0.0.1/litenv.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-05 14:20:25.000000 litenv-0.0.1/litenv.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       37 2023-06-06 20:52:37.000000 litenv-0.0.1/litenv.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-06 20:52:37.000000 litenv-0.0.1/litenv.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)     1065 2023-06-06 20:19:58.000000 litenv-0.0.1/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-06 20:52:37.220752 litenv-0.0.1/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2671 2023-06-05 19:37:38.000000 litenv-0.0.1/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 13:24:19.136098 litenv-0.0.2/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 litenv-0.0.2/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 litenv-0.0.2/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     8078 2023-06-07 13:24:19.135953 litenv-0.0.2/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     7302 2023-06-07 13:13:47.000000 litenv-0.0.2/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 13:24:19.135729 litenv-0.0.2/data/
+-rw-r--r--   0 solst      (501) staff       (20)     4773 2023-06-07 13:05:11.000000 litenv-0.0.2/data/litenv.yml
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 13:24:19.134656 litenv-0.0.2/litenv/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    25532 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     3947 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)     2408 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/constants.py
+-rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-05 12:16:38.000000 litenv-0.0.2/litenv/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    24474 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/dataclasses.py
+-rw-r--r--   0 solst      (501) staff       (20)    11704 2023-06-05 22:16:07.000000 litenv-0.0.2/litenv/defaults.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/files.py
+-rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/paths.py
+-rw-r--r--   0 solst      (501) staff       (20)      977 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)      216 2023-06-05 22:16:07.000000 litenv-0.0.2/litenv/tests.py
+-rw-r--r--   0 solst      (501) staff       (20)     4104 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/themes.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)      269 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/types.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-07 13:23:53.000000 litenv-0.0.2/litenv/utils.py
+-rw-r--r--   0 solst      (501) staff       (20)     5788 2023-06-06 17:57:47.000000 litenv-0.0.2/litenv/yml.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-07 13:24:19.135603 litenv-0.0.2/litenv.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     8078 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      562 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       96 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-05 14:20:25.000000 litenv-0.0.2/litenv.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       37 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-07 13:24:19.000000 litenv-0.0.2/litenv.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      933 2023-06-07 13:23:47.000000 litenv-0.0.2/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-07 13:24:19.136140 litenv-0.0.2/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2671 2023-06-05 19:37:38.000000 litenv-0.0.2/setup.py
```

### Comparing `litenv-0.0.1/LICENSE` & `litenv-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `litenv-0.0.1/data/litenv.yml` & `litenv-0.0.2/data/litenv.yml`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 channels:  
   - pytorch
   - conda-forge  
   - fastai
   - bioconda  
   - dglteam
   - nvidia
+  - dsm-72
 
 categories:
   utils:
     name: 'Utilities'
     checked: true
     dependencies:
       tqdm:
@@ -21,26 +22,23 @@
     name: 'Scripting'
     dependencies:
       rich:
       typer:
       questionary:
         channel: conda-forge
 
-  'conda-plugins':
-    name: 'Conda Plugins'
-    dependencies:
-      conda:
-
   packaging:
     name: 'Packaging'
     dependencies:
       twine:
         note: 'for uploading to PyPI'        
       anaconda-client:
         note: 'for uploading to Anaconda Cloud'
+      conda:
+        note: 'for building conda packages and conda-plugins'
     
     subcategories:
       versioning:
         packaging:
           note: 'for handling pypa versions'
 
   testing:
@@ -63,19 +61,33 @@
         always: true
       jupyterlab:
         channel: conda-forge
         always: true
 
   nbdev:
     name: 'nbdev'
+    checked: true
     dependencies:
       nbdev:
         version: '>=2.3.12'
         channel: fastai
 
+  dsm72:
+    name: 'Settings'
+    checked: true
+    dependencies:
+      env2ini:
+        channel: dsm-72
+        note: 'for converting environment.yml to requirements for settings.ini'
+
+      litenv:
+        channel: dsm-72
+        note: 'for quickly generating environments'
+        
+
   torch:
     name: 'PyTorch & Deep Learning'
     checked: true
     dependencies:
       pytorch:
         pypi_name: torch
 
@@ -173,15 +185,14 @@
     checked: true
     dependencies:
       phate:
         note: 'phate requires s_gd2 which is not built for ARM (e.g. Apple Silicon) on conda-forge. You can install it via pip.'
         no_arm_support: true
 
       
-      
     subcategories:
       graphtools:
         name: 'Graphtools'
         dependencies:
           graphtools:
             pip_only: true
             note: 'for graph diffusion'
```

### Comparing `litenv-0.0.1/litenv/_modidx.py` & `litenv-0.0.2/litenv/_modidx.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.1/litenv/commands.py` & `litenv-0.0.2/litenv/commands.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.1/litenv/constants.py` & `litenv-0.0.2/litenv/constants.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.1/litenv/dataclasses.py` & `litenv-0.0.2/litenv/dataclasses.py`

 * *Files 11% similar despite different names*

```diff
@@ -373,24 +373,27 @@
         return Header(self.name)
     
     @property
     def title(self) -> str:
         return self.name or self.key
 
     def place_in_dependency_list(
-        self, conda_deps: List[str], pip_deps: List[str], accel:Accelerator
+        self, conda_deps: List[str], pip_deps: List[str], accel:Accelerator, only_always:bool=False
     ) -> Tuple[List[str], List[str]]:
 
         n_conda, n_pip = self.dependencies.calc_n_conda_n_pip(accel)
         conda_deps, pip_deps = self.header.place_in_dependency_list(
             conda_deps, pip_deps, self.level, n_conda, n_pip
         )
         for dep in self.dependencies.values():
-            conda_deps, pip_deps = dep.place_in_dependency_list(conda_deps, pip_deps, accel)
-        
+            if only_always:
+                if dep.always:
+                    conda_deps, pip_deps = dep.place_in_dependency_list(conda_deps, pip_deps, accel)
+            else:
+                conda_deps, pip_deps = dep.place_in_dependency_list(conda_deps, pip_deps, accel)        
         return conda_deps, pip_deps
 
     def to_choice(self) -> Choice:    
         deps = self.dependencies.get_names()
         title = self.title
         deps = str(tuple(deps)).replace("'", "").replace(",)", ")").replace(", )", ")")
         title = f'{self.title} {deps}'
@@ -440,19 +443,26 @@
     def values(self) -> Iterable[T]:
         return self.categories.values()
 
     def items(self) -> Iterable[Tuple[str, T]]:
         return self.categories.items()
 
     def place_in_dependency_list(
-        self, conda_deps: List[str], pip_deps: List[str], accel:Accelerator, include: List[str] = []
+        self, conda_deps: List[str], pip_deps: List[str], accel:Accelerator, 
+        include: List[str] = [], include_always: Optional[bool] = False
     ) -> Tuple[List[str], List[str]]:
         keys = list(filter(lambda k: k in include, self.categories.keys()))
         for key in keys:
-            conda_deps, pip_deps = self.categories[key].place_in_dependency_list(conda_deps, pip_deps, accel)            
+            conda_deps, pip_deps = self.categories[key].place_in_dependency_list(conda_deps, pip_deps, accel)
+        if not include_always:
+            return conda_deps, pip_deps
+        
+        for key in self.categories.keys():
+            if key not in keys:
+                conda_deps, pip_deps = self.categories[key].place_in_dependency_list(conda_deps, pip_deps, accel, only_always=True)                         
         return conda_deps, pip_deps
 
 
     def make_choices(self) -> List[Choice]:
         return [cat.to_choice() for cat in self.categories.values()]
 
     def get_all_dependencies(self) -> Iterable[Tuple[str, EnvDep]]:
@@ -493,23 +503,23 @@
 
     def __init__(self, key, **kwargs):
         super().__init__(key, **kwargs)
         self.subcategories = SubCategories(**kwargs.pop(SUBCATEGORIES, {}))
         
     def add_to_dependency_lists(
         self, conda_deps: List[str], pip_deps: List[str], accel:Accelerator,
-        subcategories_to_include: Optional[List[str]] = [],
+        subcategories_to_include: Optional[List[str]] = [], include_always: Optional[bool] = False
     ) -> Tuple[List[str], List[str]]:
-        self.place_in_dependency_list(conda_deps, pip_deps, accel)
+        self.place_in_dependency_list(conda_deps, pip_deps, accel, include_always)
         self.subcategories.place_in_dependency_list(
-            conda_deps, pip_deps, accel, subcategories_to_include
+            conda_deps, pip_deps, accel, subcategories_to_include, include_always
         )
         return conda_deps, pip_deps
     
-    def get_subcategory(self, catkey:str) -> dict:
+    def get_subcategory(self, subkey:str) -> dict:
         return self.subcategories.get_subcategory(subkey, {})  
 
     def get_selected_dependencies(self, selected: List[str] = []) -> Dict[str, EnvDep]:
         deps = {**self.dependencies.dependencies}
         selected = selected or []
         subdeps = self.subcategories.get_selected_dependencies(selected)
         deps.update(subdeps)        
@@ -521,21 +531,21 @@
 @rich_auto(angular=True)
 class Categories(BaseCategories):
     def __init__(self, *args, **kwargs):
         super().__init__(Category, **kwargs)
 
     def add_to_dependency_lists(
         self, conda_deps: List[str], pip_deps: List[str], accel:Accelerator,
-        include_specification: Dict[str, List[str]] = {},
+        include_specification: Dict[str, List[str]] = {}, include_always: Optional[bool] = False
     ) -> Tuple[List[str], List[str]]:        
         for key, category in self.categories.items():
             if key in include_specification:        
                 subcategories_to_include = include_specification[key] or []      
                 conda_deps, pip_deps = category.add_to_dependency_lists(
-                    conda_deps, pip_deps, accel, subcategories_to_include
+                    conda_deps, pip_deps, accel, subcategories_to_include, include_always
                 )
         return conda_deps, pip_deps
 
     def get_category(self, catkey:str) -> dict:
         return self.categories[catkey]
 
     def get_subcategories(self, catkey:str) -> dict:
@@ -605,33 +615,23 @@
             'Select categories:',
             choices=choices, style=style,
             use_jk_keys=False, use_arrow_keys=True,
         ).ask()
         if selected_catkeys is None:
             return 
 
-        titles = [choice.title for choice in choices if choice.value in selected_catkeys]
-        # tree = Tree('Selected Categories')
-        # for cat in selected_catkeys:
-        #     tcat = tree.add(self.categories[cat].title)
-        #     for dep in self.categories[cat].dependencies.values():
-        #         tcat.add(dep.name)
-        # print(tree)
-        # print(Panel(Pretty(titles), title='Selected Categories'))
         return selected_catkeys
 
     def select_subcategories(self, catkey:str) -> List[str]:
         style = self.get_style()
 
         subchoices = self.categories.get_subcategories(catkey).make_choices()
         if len(subchoices) == 0:
             return []
         
-        # console.print(f'Selecting subcategories for {catkey}')
-        # cprint('italic purple', f'\tSelecting subcategories for {catkey}')
         selected_subkeys = checkbox(
             f'Select additional subcategories for {catkey} (use space to select multiple):',
             choices=subchoices, style=style,
             use_jk_keys=False, use_arrow_keys=True,
         ).ask()
         return selected_subkeys
 
@@ -665,33 +665,37 @@
         env_str = yaml.dump(env_dict, width=float('inf'), sort_keys=False)
 
         env_lines = []
         added_space = False
         for line in env_str.split('\n'):
             prev = env_lines[-1] if len(env_lines) > 0 else ''
             
-            if '#' in line:
-                
+            if '#' in line:                
                 prev_not_dep = '::' not in prev and ':' in prev 
-                if not added_space and env_lines[-1] != ' ' and (not prev_not_dep and '#' not in env_lines[-1]):
-                    env_lines.append(' ')
+                if not added_space and env_lines[-1] != '' and (not prev_not_dep and '#' not in env_lines[-1]):
+                    env_lines.append('')
                     added_space = True
-                
+                                    
                 line = re.sub(r"'", '', line, flags=re.IGNORECASE)
                 line = line.replace('- ', '')
             else:                
                 added_space = False         
                                    
             # space before top level keys
-            if '::' not in line and ':' in line and len(env_lines) > 0 and env_lines[-1] != ' ':
+            if '::' not in line and ':' in line and len(env_lines) > 0 and env_lines[-1] != '':
                 if not ('- pip' in env_lines[-1]):
-                    env_lines.append(' ')
+                    env_lines.append('')
+
+            if line == '- pip' and ':' not in line and not added_space:
+                env_lines.append('')
 
-            if line == '- pip' and ':' not in line:
-                env_lines.append(' ')
+            if 'NOTE' in line:
+                prev = env_lines[-1] if len(env_lines) > 0 else ''
+                if prev == '' and len(env_lines):
+                    env_lines.pop()
             env_lines.append(line)
             
 
         env_str = '\n'.join(env_lines)
         return env_str
```

### Comparing `litenv-0.0.1/litenv/defaults.py` & `litenv-0.0.2/litenv/defaults.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.1/litenv/paths.py` & `litenv-0.0.2/litenv/paths.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.1/litenv/rich.py` & `litenv-0.0.2/litenv/rich.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.1/litenv/themes.py` & `litenv-0.0.2/litenv/themes.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.1/litenv/yml.py` & `litenv-0.0.2/litenv/yml.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.1/litenv.egg-info/SOURCES.txt` & `litenv-0.0.2/litenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litenv-0.0.1/setup.py` & `litenv-0.0.2/setup.py`

 * *Files identical despite different names*

