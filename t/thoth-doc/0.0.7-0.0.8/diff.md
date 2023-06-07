# Comparing `tmp/thoth_doc-0.0.7.tar.gz` & `tmp/thoth_doc-0.0.8.tar.gz`

## Comparing `thoth_doc-0.0.7.tar` & `thoth_doc-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0    28955 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/Thoth.svg.png
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/vscode.env
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/README.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.vscode/settings.json
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/src/thoth_doc/__init__.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/src/thoth_doc/main.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/src/thoth_doc/parsers.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/src/thoth_doc/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/tests/test_parsers.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/LICENSE
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.env
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/Makefile
+-rw-r--r--   0        0        0    28955 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/Thoth.svg.png
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/vscode.env
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/README.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/src/thoth_doc/__init__.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/src/thoth_doc/main.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/src/thoth_doc/parsers.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/src/thoth_doc/utils.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/src/thoth_doc/compiled_docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/tests/test_generator.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/tests/test_parsers.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/LICENSE
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 thoth_doc-0.0.8/PKG-INFO
```

### Comparing `thoth_doc-0.0.7/Thoth.svg.png` & `thoth_doc-0.0.8/Thoth.svg.png`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.7/src/thoth_doc/main.py` & `thoth_doc-0.0.8/src/thoth_doc/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 
-from .parsers import code_reference_parser
+from thoth_doc.parsers import code_reference_parser
+
 
 
 class DocGenerator:
     parsers = []
+    image_host = None
     _default_parsers = [code_reference_parser]
 
     def __init__(self, docs_folder, compiled_docs_folder):
         self.docs_folder = docs_folder
         self.compiled_docs_folder = compiled_docs_folder
 
     def _get_compiled_docs_path(self, path=None):
@@ -28,21 +30,19 @@
             elif line.startswith('[endignore]'):
                 skip = False
                 continue
             elif skip:
                 compiled_markdown += line
                 continue
 
+            parsed = line
             for parser in self.parsers + self._default_parsers:
-                parsed = parser(line)
-                if parsed is not None:
-                    compiled_markdown += parsed
-                    break
-            if parsed is None:
-                compiled_markdown += line
+                parsed = parser(self, parsed)
+
+            compiled_markdown += parsed
         return compiled_markdown
 
     def _create_folder_structure(self, cwd):
         os.makedirs(cwd, exist_ok=True)
 
         for root, dirs, files in os.walk(self.docs_folder):
             for dir in dirs:
@@ -107,8 +107,9 @@
                             f.write(self._compile_lines(compiled_lines))
                     else:
                         os.system(f'cp {path} {compiled_docs_path}/{root.replace(self.docs_folder, "")}')
 
 
 if __name__ == '__main__':
     generator = DocGenerator('docs', 'docs_compiled')
+    generator.image_folder = 'images'
     generator.generate()
```

### Comparing `thoth_doc-0.0.7/src/thoth_doc/parsers.py` & `thoth_doc-0.0.8/src/thoth_doc/parsers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,59 @@
 import os
 import re
 
-from .utils import get_docstring, remove_whitespaces
+from thoth_doc.utils import get_docstring, remove_whitespaces
 
 
-def code_reference_parser(line):
+def add_image_host_to_image_links(generator, line):
+    ''' Adds image host to image links. you need to set image_host attribute on generator instance. '''
+
+    host = getattr(generator, 'image_host', None)
+    matches = re.findall(r'(!\[.*?\]\((.*?)\))', line)
+    if matches and host:
+        for match in matches:
+            line = line.replace(match[1], f'{host}/{match[1]}')
+        return line
+    return line
+
+
+def code_reference_parser(_, line):
     ''' Parses [@code/main.py#Class.method] syntax. Extacts docstring. '''
 
     matches = re.findall(r'(\[@(.+?)\])', line)
     if matches:
         for match in matches:
             mod, name = match[1].split('#')
             docstring = get_docstring(mod, name)
             docstring = remove_whitespaces(docstring)
             docstring = docstring.replace('\n', '\n\n')
             line = line.replace(match[0], docstring)
         return line
-    return None
+    return line
 
 
-def env_var_parser(line):
+def env_var_parser(_, line):
     ''' Parses [$env.ENV_VAR_NAME] syntax '''
 
     matches = re.findall(r'(\[\$env\.(\w+)\])', line)
     if matches:
         for match, var_name in matches:
             value = os.environ.get(var_name)
             line = line.replace(match, str(value))
         return line
-    return None
+    return line
 
 
-def django_settings_parser(line):
+def django_settings_parser(_, line):
     ''' Parses [$settings.SETTINGS_VAR_NAME] syntax '''
 
     matches = re.findall(r'(\[\$settings\.(\w+)\])', line)
     if matches:
         try:
             from django.conf import settings
         except ImportError:
             raise ImportError('Django is not installed')
         for match, setting_name in matches:
             value = getattr(settings, setting_name)
             line = line.replace(match, str(value))
         return line
-    return None
+    return line
```

### Comparing `thoth_doc-0.0.7/src/thoth_doc/utils.py` & `thoth_doc-0.0.8/src/thoth_doc/utils.py`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.7/LICENSE` & `thoth_doc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.7/README.md` & `thoth_doc-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.7/pyproject.toml` & `thoth_doc-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thoth_doc"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Lev", email="smj510black@gmail.com" },
 ]
 description = "Dependency-free, lightweight docstring parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thoth_doc-0.0.7/PKG-INFO` & `thoth_doc-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoth_doc
-Version: 0.0.7
+Version: 0.0.8
 Summary: Dependency-free, lightweight docstring parser
 Project-URL: Homepage, https://github.com/mariownyou/thoth-doc
 Project-URL: Bug Tracker, https://github.com/mariownyou/thoth-doc/issues
 Author-email: Lev <smj510black@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

