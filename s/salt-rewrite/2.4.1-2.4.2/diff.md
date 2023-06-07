# Comparing `tmp/salt-rewrite-2.4.1.tar.gz` & `tmp/salt-rewrite-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salt-rewrite-2.4.1.tar", max compression
+gzip compressed data, was "salt-rewrite-2.4.2.tar", max compression
```

## Comparing `salt-rewrite-2.4.1.tar` & `salt-rewrite-2.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2020-02-05 15:05:21.219175 salt-rewrite-2.4.1/LICENSE
--rw-r--r--   0        0        0      652 2023-06-07 15:58:08.379179 salt-rewrite-2.4.1/pyproject.toml
--rw-r--r--   0        0        0       43 2022-06-23 07:32:30.489445 salt-rewrite-2.4.1/src/saltrewrite/__init__.py
--rw-r--r--   0        0        0     1537 2023-06-07 06:44:56.636972 salt-rewrite-2.4.1/src/saltrewrite/__main__.py
--rw-r--r--   0        0        0     1570 2023-06-07 06:44:53.926961 salt-rewrite-2.4.1/src/saltrewrite/__main__.py~
--rw-r--r--   0        0        0     1416 2022-06-23 07:32:30.506111 salt-rewrite-2.4.1/src/saltrewrite/fixes.py
--rw-r--r--   0        0        0      305 2022-06-23 07:32:30.499445 salt-rewrite-2.4.1/src/saltrewrite/imports/__init__.py
--rw-r--r--   0        0        0     2767 2022-06-23 07:33:00.272886 salt-rewrite-2.4.1/src/saltrewrite/imports/fix_tornado_imports.py
--rw-r--r--   0        0        0      343 2022-06-23 07:46:36.072615 salt-rewrite-2.4.1/src/saltrewrite/salt/__init__.py
--rw-r--r--   0        0        0    26710 2023-06-07 15:55:12.541351 salt-rewrite-2.4.1/src/saltrewrite/salt/fix_docstrings.py
--rw-r--r--   0        0        0    26702 2023-06-07 15:54:43.354479 salt-rewrite-2.4.1/src/saltrewrite/salt/fix_docstrings.py~
--rw-r--r--   0        0        0     5219 2023-06-07 15:43:48.044732 salt-rewrite-2.4.1/src/saltrewrite/salt/fix_dunder_utils.py
--rw-r--r--   0        0        0     5255 2023-06-07 15:31:58.591735 salt-rewrite-2.4.1/src/saltrewrite/salt/fix_dunder_utils.py~
--rw-r--r--   0        0        0      827 2022-06-23 07:32:30.536111 salt-rewrite-2.4.1/src/saltrewrite/testsuite/__init__.py
--rw-r--r--   0        0        0    20763 2022-06-23 07:34:49.989951 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_asserts.py
--rw-r--r--   0        0        0     1224 2022-06-23 07:32:30.486111 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_destructive_test_decorator.py
--rw-r--r--   0        0        0     1210 2022-06-23 07:32:30.502778 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_expensive_test_decorator.py
--rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_network_decorator.py
--rw-r--r--   0        0        0     1270 2022-06-23 07:32:30.499445 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py
--rw-r--r--   0        0        0     1263 2022-06-23 07:32:30.529445 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py
--rw-r--r--   0        0        0     1291 2022-06-23 07:32:30.479445 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py
--rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py
--rw-r--r--   0        0        0     1168 2022-06-23 07:32:30.492778 salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_slow_test_decorator.py
--rw-r--r--   0        0        0     6570 2022-06-23 07:32:30.532778 salt-rewrite-2.4.1/src/saltrewrite/utils.py
--rw-r--r--   0        0        0      903 2023-06-07 15:58:37.628346 salt-rewrite-2.4.1/setup.py
--rw-r--r--   0        0        0      543 2023-06-07 15:58:37.628598 salt-rewrite-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2020-02-05 15:05:21.219175 salt-rewrite-2.4.2/LICENSE
+-rw-r--r--   0        0        0      652 2023-06-07 16:31:25.236076 salt-rewrite-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0       43 2022-06-23 07:32:30.489445 salt-rewrite-2.4.2/src/saltrewrite/__init__.py
+-rw-r--r--   0        0        0     1537 2023-06-07 06:44:56.636972 salt-rewrite-2.4.2/src/saltrewrite/__main__.py
+-rw-r--r--   0        0        0     1570 2023-06-07 06:44:53.926961 salt-rewrite-2.4.2/src/saltrewrite/__main__.py~
+-rw-r--r--   0        0        0     1416 2022-06-23 07:32:30.506111 salt-rewrite-2.4.2/src/saltrewrite/fixes.py
+-rw-r--r--   0        0        0      305 2022-06-23 07:32:30.499445 salt-rewrite-2.4.2/src/saltrewrite/imports/__init__.py
+-rw-r--r--   0        0        0     2767 2022-06-23 07:33:00.272886 salt-rewrite-2.4.2/src/saltrewrite/imports/fix_tornado_imports.py
+-rw-r--r--   0        0        0      343 2022-06-23 07:46:36.072615 salt-rewrite-2.4.2/src/saltrewrite/salt/__init__.py
+-rw-r--r--   0        0        0    26730 2023-06-07 16:30:49.162571 salt-rewrite-2.4.2/src/saltrewrite/salt/fix_docstrings.py
+-rw-r--r--   0        0        0    27018 2023-06-07 16:29:54.122309 salt-rewrite-2.4.2/src/saltrewrite/salt/fix_docstrings.py~
+-rw-r--r--   0        0        0     5219 2023-06-07 15:43:48.044732 salt-rewrite-2.4.2/src/saltrewrite/salt/fix_dunder_utils.py
+-rw-r--r--   0        0        0     5255 2023-06-07 15:31:58.591735 salt-rewrite-2.4.2/src/saltrewrite/salt/fix_dunder_utils.py~
+-rw-r--r--   0        0        0      827 2022-06-23 07:32:30.536111 salt-rewrite-2.4.2/src/saltrewrite/testsuite/__init__.py
+-rw-r--r--   0        0        0    20763 2022-06-23 07:34:49.989951 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_asserts.py
+-rw-r--r--   0        0        0     1224 2022-06-23 07:32:30.486111 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_destructive_test_decorator.py
+-rw-r--r--   0        0        0     1210 2022-06-23 07:32:30.502778 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_expensive_test_decorator.py
+-rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_network_decorator.py
+-rw-r--r--   0        0        0     1270 2022-06-23 07:32:30.499445 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py
+-rw-r--r--   0        0        0     1263 2022-06-23 07:32:30.529445 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py
+-rw-r--r--   0        0        0     1291 2022-06-23 07:32:30.479445 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py
+-rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py
+-rw-r--r--   0        0        0     1168 2022-06-23 07:32:30.492778 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_slow_test_decorator.py
+-rw-r--r--   0        0        0     6570 2022-06-23 07:32:30.532778 salt-rewrite-2.4.2/src/saltrewrite/utils.py
+-rw-r--r--   0        0        0      903 2023-06-07 16:32:06.949920 salt-rewrite-2.4.2/setup.py
+-rw-r--r--   0        0        0      543 2023-06-07 16:32:06.950241 salt-rewrite-2.4.2/PKG-INFO
```

### Comparing `salt-rewrite-2.4.1/LICENSE` & `salt-rewrite-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/pyproject.toml` & `salt-rewrite-2.4.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "salt-rewrite"
-version = "2.4.1"
+version = "2.4.2"
 description = "A set of Bowler code to rewrite parts of Salt"
 authors = ["Pedro Algarvio <pedro@algarvio.me>"]
 license = "Apache-2.0"
 packages = [
   {include = "saltrewrite", from = "src" }
 ]
```

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/__main__.py` & `salt-rewrite-2.4.2/src/saltrewrite/__main__.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/__main__.py~` & `salt-rewrite-2.4.2/src/saltrewrite/__main__.py~`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/fixes.py` & `salt-rewrite-2.4.2/src/saltrewrite/fixes.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/imports/fix_tornado_imports.py` & `salt-rewrite-2.4.2/src/saltrewrite/imports/fix_tornado_imports.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/salt/fix_docstrings.py` & `salt-rewrite-2.4.2/src/saltrewrite/salt/fix_docstrings.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,24 +120,26 @@
         for _vs in version.split(splitter):
             for _splitter in splitters:
                 if _splitter in _vs:
                     break
             else:
                 versions.add(_vs)
     parsed_versions = []
-    for version in sorted(versions):
+    for version in versions:
         try:
-            version = SaltStackVersion.from_name(version).string
+            version = SaltStackVersion.from_name(version)
         except ValueError:
             try:
-                version = SaltStackVersion.parse(version).string
+                version = SaltStackVersion.parse(version)
             except ValueError:
                 pass
         parsed_versions.append(version)
-    replace_contents = ".. {}:: {}".format(vtype, ",".join(parsed_versions))
+    replace_contents = ".. {}:: {}".format(
+        vtype, ",".join([v.string for v in sorted(parsed_versions)])
+    )
     return replace_contents
 
 
 def _convert_version_names_to_numbers(docstring, filename):
     """
     Convert Salt version names to their version numbers counterpart
     """
```

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/salt/fix_docstrings.py~` & `salt-rewrite-2.4.2/src/saltrewrite/salt/fix_docstrings.py~`

 * *Files 1% similar despite different names*

```diff
@@ -122,22 +122,26 @@
                 if _splitter in _vs:
                     break
             else:
                 versions.add(_vs)
     parsed_versions = []
     for version in versions:
         try:
-            version = SaltStackVersion.from_name(version).string
+            version = SaltStackVersion.from_name(version)
         except ValueError:
             try:
-                version = SaltStackVersion.parse(version).string
+                version = SaltStackVersion.parse(version)
             except ValueError:
                 pass
         parsed_versions.append(version)
-    replace_contents = ".. {}:: {}".format(vtype, ",".join(parsed_versions))
+    import click
+    click.echo(f"V1: {parsed_versions}")
+    click.echo(f"V2: {sorted(parsed_versions)}")
+    click.echo(f"V2.1: {sorted(parsed_versions, key=lambda v: v.full_info_all_versions)}")
+    replace_contents = ".. {}:: {}".format(vtype, ",".join([v.string for v in sorted(parsed_versions)]))
     return replace_contents
 
 
 def _convert_version_names_to_numbers(docstring, filename):
     """
     Convert Salt version names to their version numbers counterpart
     """
@@ -693,14 +697,17 @@
             # We have pre-release information, the other side doesn't
             other_noc_info[other_pre_type] = "zzzzz"
 
         if not self.pre_type and other.pre_type:
             # The other side has pre-release information, we don't
             noc_info[pre_type] = "zzzzz"
 
+        import click
+        click.echo(f"V3: {method} - {tuple(noc_info)} , {tuple(other_noc_info)}")
+
         return method(tuple(noc_info), tuple(other_noc_info))
 
     def __lt__(self, other):
         return self.__compare__(other, lambda _self, _other: _self < _other)
 
     def __le__(self, other):
         return self.__compare__(other, lambda _self, _other: _self <= _other)
```

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/salt/fix_dunder_utils.py` & `salt-rewrite-2.4.2/src/saltrewrite/salt/fix_dunder_utils.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/salt/fix_dunder_utils.py~` & `salt-rewrite-2.4.2/src/saltrewrite/salt/fix_dunder_utils.py~`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/testsuite/__init__.py` & `salt-rewrite-2.4.2/src/saltrewrite/testsuite/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_asserts.py` & `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_asserts.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_destructive_test_decorator.py` & `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_destructive_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_expensive_test_decorator.py` & `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_expensive_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_network_decorator.py` & `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_network_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py` & `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py` & `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py` & `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py` & `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/testsuite/fix_slow_test_decorator.py` & `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_slow_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/src/saltrewrite/utils.py` & `salt-rewrite-2.4.2/src/saltrewrite/utils.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.1/setup.py` & `salt-rewrite-2.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ['bowler>=0.9.0', 'fissix>=21.6,<22.0']
 
 entry_points = \
 {'console_scripts': ['salt-rewrite = saltrewrite.__main__:rewrite']}
 
 setup_kwargs = {
     'name': 'salt-rewrite',
-    'version': '2.4.1',
+    'version': '2.4.2',
     'description': 'A set of Bowler code to rewrite parts of Salt',
     'long_description': None,
     'author': 'Pedro Algarvio',
     'author_email': 'pedro@algarvio.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `salt-rewrite-2.4.1/PKG-INFO` & `salt-rewrite-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-rewrite
-Version: 2.4.1
+Version: 2.4.2
 Summary: A set of Bowler code to rewrite parts of Salt
 License: Apache-2.0
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

