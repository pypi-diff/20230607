# Comparing `tmp/salt-rewrite-2.4.0.tar.gz` & `tmp/salt-rewrite-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salt-rewrite-2.4.0.tar", max compression
+gzip compressed data, was "salt-rewrite-2.4.1.tar", max compression
```

## Comparing `salt-rewrite-2.4.0.tar` & `salt-rewrite-2.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2020-02-05 15:05:21.219175 salt-rewrite-2.4.0/LICENSE
--rw-r--r--   0        0        0      652 2023-06-07 15:50:21.039769 salt-rewrite-2.4.0/pyproject.toml
--rw-r--r--   0        0        0       43 2022-06-23 07:32:30.489445 salt-rewrite-2.4.0/src/saltrewrite/__init__.py
--rw-r--r--   0        0        0     1537 2023-06-07 06:44:56.636972 salt-rewrite-2.4.0/src/saltrewrite/__main__.py
--rw-r--r--   0        0        0     1570 2023-06-07 06:44:53.926961 salt-rewrite-2.4.0/src/saltrewrite/__main__.py~
--rw-r--r--   0        0        0     1416 2022-06-23 07:32:30.506111 salt-rewrite-2.4.0/src/saltrewrite/fixes.py
--rw-r--r--   0        0        0      305 2022-06-23 07:32:30.499445 salt-rewrite-2.4.0/src/saltrewrite/imports/__init__.py
--rw-r--r--   0        0        0     2767 2022-06-23 07:33:00.272886 salt-rewrite-2.4.0/src/saltrewrite/imports/fix_tornado_imports.py
--rw-r--r--   0        0        0      343 2022-06-23 07:46:36.072615 salt-rewrite-2.4.0/src/saltrewrite/salt/__init__.py
--rw-r--r--   0        0        0    26701 2023-06-07 15:44:54.911687 salt-rewrite-2.4.0/src/saltrewrite/salt/fix_docstrings.py
--rw-r--r--   0        0        0    26698 2023-06-07 15:44:21.388209 salt-rewrite-2.4.0/src/saltrewrite/salt/fix_docstrings.py~
--rw-r--r--   0        0        0     5219 2023-06-07 15:43:48.044732 salt-rewrite-2.4.0/src/saltrewrite/salt/fix_dunder_utils.py
--rw-r--r--   0        0        0     5255 2023-06-07 15:31:58.591735 salt-rewrite-2.4.0/src/saltrewrite/salt/fix_dunder_utils.py~
--rw-r--r--   0        0        0      827 2022-06-23 07:32:30.536111 salt-rewrite-2.4.0/src/saltrewrite/testsuite/__init__.py
--rw-r--r--   0        0        0    20763 2022-06-23 07:34:49.989951 salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_asserts.py
--rw-r--r--   0        0        0     1224 2022-06-23 07:32:30.486111 salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_destructive_test_decorator.py
--rw-r--r--   0        0        0     1210 2022-06-23 07:32:30.502778 salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_expensive_test_decorator.py
--rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_requires_network_decorator.py
--rw-r--r--   0        0        0     1270 2022-06-23 07:32:30.499445 salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py
--rw-r--r--   0        0        0     1263 2022-06-23 07:32:30.529445 salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py
--rw-r--r--   0        0        0     1291 2022-06-23 07:32:30.479445 salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py
--rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py
--rw-r--r--   0        0        0     1168 2022-06-23 07:32:30.492778 salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_slow_test_decorator.py
--rw-r--r--   0        0        0     6570 2022-06-23 07:32:30.532778 salt-rewrite-2.4.0/src/saltrewrite/utils.py
--rw-r--r--   0        0        0      903 2023-06-07 15:51:05.571774 salt-rewrite-2.4.0/setup.py
--rw-r--r--   0        0        0      543 2023-06-07 15:51:05.572028 salt-rewrite-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2020-02-05 15:05:21.219175 salt-rewrite-2.4.1/LICENSE
+-rw-r--r--   0        0        0      652 2023-06-07 15:58:08.379179 salt-rewrite-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0       43 2022-06-23 07:32:30.489445 salt-rewrite-2.4.1/src/saltrewrite/__init__.py
+-rw-r--r--   0        0        0     1537 2023-06-07 06:44:56.636972 salt-rewrite-2.4.1/src/saltrewrite/__main__.py
+-rw-r--r--   0        0        0     1570 2023-06-07 06:44:53.926961 salt-rewrite-2.4.1/src/saltrewrite/__main__.py~
+-rw-r--r--   0        0        0     1416 2022-06-23 07:32:30.506111 salt-rewrite-2.4.1/src/saltrewrite/fixes.py
+-rw-r--r--   0        0        0      305 2022-06-23 07:32:30.499445 salt-rewrite-2.4.1/src/saltrewrite/imports/__init__.py
+-rw-r--r--   0        0        0     2767 2022-06-23 07:33:00.272886 salt-rewrite-2.4.1/src/saltrewrite/imports/fix_tornado_imports.py
+-rw-r--r--   0        0        0      343 2022-06-23 07:46:36.072615 salt-rewrite-2.4.1/src/saltrewrite/salt/__init__.py
+-rw-r--r--   0        0        0    26710 2023-06-07 15:55:12.541351 salt-rewrite-2.4.1/src/saltrewrite/salt/fix_docstrings.py
+-rw-r--r--   0        0        0    26702 2023-06-07 15:54:43.354479 salt-rewrite-2.4.1/src/saltrewrite/salt/fix_docstrings.py~
+-rw-r--r--   0        0        0     5219 2023-06-07 15:43:48.044732 salt-rewrite-2.4.1/src/saltrewrite/salt/fix_dunder_utils.py
+-rw-r--r--   0        0        0     5255 2023-06-07 15:31:58.591735 salt-rewrite-2.4.1/src/saltrewrite/salt/fix_dunder_utils.py~
+-rw-r--r--   0        0        0      827 2022-06-23 07:32:30.536111 salt-rewrite-2.4.1/src/saltrewrite/testsuite/__init__.py
+-rw-r--r--   0        0        0    20763 2022-06-23 07:34:49.989951 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_asserts.py
+-rw-r--r--   0        0        0     1224 2022-06-23 07:32:30.486111 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_destructive_test_decorator.py
+-rw-r--r--   0        0        0     1210 2022-06-23 07:32:30.502778 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_expensive_test_decorator.py
+-rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_network_decorator.py
+-rw-r--r--   0        0        0     1270 2022-06-23 07:32:30.499445 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py
+-rw-r--r--   0        0        0     1263 2022-06-23 07:32:30.529445 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py
+-rw-r--r--   0        0        0     1291 2022-06-23 07:32:30.479445 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py
+-rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py
+-rw-r--r--   0        0        0     1168 2022-06-23 07:32:30.492778 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_slow_test_decorator.py
+-rw-r--r--   0        0        0     6570 2022-06-23 07:32:30.532778 salt-rewrite-2.4.1/src/saltrewrite/utils.py
+-rw-r--r--   0        0        0      903 2023-06-07 15:58:37.628346 salt-rewrite-2.4.1/setup.py
+-rw-r--r--   0        0        0      543 2023-06-07 15:58:37.628598 salt-rewrite-2.4.1/PKG-INFO
```

### Comparing `salt-rewrite-2.4.0/LICENSE` & `salt-rewrite-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/__main__.py` & `salt-rewrite-2.4.1/src/saltrewrite/__main__.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/__main__.py~` & `salt-rewrite-2.4.1/src/saltrewrite/__main__.py~`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/fixes.py` & `salt-rewrite-2.4.1/src/saltrewrite/fixes.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/imports/fix_tornado_imports.py` & `salt-rewrite-2.4.1/src/saltrewrite/imports/fix_tornado_imports.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/salt/fix_docstrings.py` & `salt-rewrite-2.4.1/src/saltrewrite/salt/fix_docstrings.py~`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # pylint: disable=consider-using-f-string
 import operator
 import re
 import sys
 from collections import namedtuple
 from functools import total_ordering
 
-import click
 from bowler import Query
 from bowler import TOKEN
 
 
 def rewrite(paths, interactive=False, silent=False):
     """
     Rewrite the passed in paths
@@ -120,15 +119,14 @@
     for splitter in splitters:
         for _vs in version.split(splitter):
             for _splitter in splitters:
                 if _splitter in _vs:
                     break
             else:
                 versions.add(_vs)
-    click.echo(f"Versions: {versions}")
     parsed_versions = []
     for version in versions:
         try:
             version = SaltStackVersion.from_name(version).string
         except ValueError:
             try:
                 version = SaltStackVersion.parse(version).string
@@ -529,14 +527,16 @@
         """
         return bool(int(major) >= 3000 and int(major) < VERSION_LIMIT)
 
     def can_have_dot_zero(self, major):
         """
         determine if using new versioning scheme
         """
+        if int(major) < 3000:
+            return True
         return bool(int(major) >= 3006 and int(major) < VERSION_LIMIT)
 
     @classmethod
     def parse(cls, version_string):
         if version_string.lower() in cls.LNAMES:
             return cls.from_name(version_string)
         vstr = version_string.decode() if isinstance(version_string, bytes) else version_string
```

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/salt/fix_docstrings.py~` & `salt-rewrite-2.4.1/src/saltrewrite/salt/fix_docstrings.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # pylint: disable=consider-using-f-string
 import operator
 import re
 import sys
 from collections import namedtuple
 from functools import total_ordering
 
-import click
 from bowler import Query
 from bowler import TOKEN
 
 
 def rewrite(paths, interactive=False, silent=False):
     """
     Rewrite the passed in paths
@@ -114,23 +113,22 @@
     Convert every match with a properly formatted version.
     """
     vtype = match.group("vtype")
     version = match.group("version")
     versions = set()
     splitters = (",", "/", " ")
     for splitter in splitters:
-        for vs in version.split(splitter):
+        for _vs in version.split(splitter):
             for _splitter in splitters:
-                if _splitter in vs:
+                if _splitter in _vs:
                     break
             else:
-                versions.add(vs)
-    click.echo(f"Versions: {versions}")
+                versions.add(_vs)
     parsed_versions = []
-    for version in versions:
+    for version in sorted(versions):
         try:
             version = SaltStackVersion.from_name(version).string
         except ValueError:
             try:
                 version = SaltStackVersion.parse(version).string
             except ValueError:
                 pass
@@ -529,14 +527,16 @@
         """
         return bool(int(major) >= 3000 and int(major) < VERSION_LIMIT)
 
     def can_have_dot_zero(self, major):
         """
         determine if using new versioning scheme
         """
+        if int(major) < 3000:
+            return True
         return bool(int(major) >= 3006 and int(major) < VERSION_LIMIT)
 
     @classmethod
     def parse(cls, version_string):
         if version_string.lower() in cls.LNAMES:
             return cls.from_name(version_string)
         vstr = version_string.decode() if isinstance(version_string, bytes) else version_string
```

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/salt/fix_dunder_utils.py` & `salt-rewrite-2.4.1/src/saltrewrite/salt/fix_dunder_utils.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/salt/fix_dunder_utils.py~` & `salt-rewrite-2.4.1/src/saltrewrite/salt/fix_dunder_utils.py~`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/testsuite/__init__.py` & `salt-rewrite-2.4.1/src/saltrewrite/testsuite/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_asserts.py` & `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_asserts.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_destructive_test_decorator.py` & `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_destructive_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_expensive_test_decorator.py` & `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_expensive_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_requires_network_decorator.py` & `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_network_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py` & `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py` & `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py` & `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py` & `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/testsuite/fix_slow_test_decorator.py` & `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_slow_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/src/saltrewrite/utils.py` & `salt-rewrite-2.4.1/src/saltrewrite/utils.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.0/setup.py` & `salt-rewrite-2.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ['bowler>=0.9.0', 'fissix>=21.6,<22.0']
 
 entry_points = \
 {'console_scripts': ['salt-rewrite = saltrewrite.__main__:rewrite']}
 
 setup_kwargs = {
     'name': 'salt-rewrite',
-    'version': '2.4.0',
+    'version': '2.4.1',
     'description': 'A set of Bowler code to rewrite parts of Salt',
     'long_description': None,
     'author': 'Pedro Algarvio',
     'author_email': 'pedro@algarvio.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `salt-rewrite-2.4.0/PKG-INFO` & `salt-rewrite-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-rewrite
-Version: 2.4.0
+Version: 2.4.1
 Summary: A set of Bowler code to rewrite parts of Salt
 License: Apache-2.0
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

