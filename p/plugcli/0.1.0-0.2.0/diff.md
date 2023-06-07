# Comparing `tmp/plugcli-0.1.0.tar.gz` & `tmp/plugcli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugcli-0.1.0.tar", last modified: Wed Mar 15 17:57:40 2023, max compression
+gzip compressed data, was "plugcli-0.2.0.tar", last modified: Wed Jun  7 21:43:37 2023, max compression
```

## Comparing `plugcli-0.1.0.tar` & `plugcli-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:57:40.543175 plugcli-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-15 17:57:23.000000 plugcli-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-15 17:57:23.000000 plugcli-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-03-15 17:57:40.543175 plugcli-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-03-15 17:57:23.000000 plugcli-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:57:40.543175 plugcli-0.1.0/plugcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-15 17:57:40.000000 plugcli-0.1.0/plugcli/_installed_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/plugin_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:57:40.543175 plugcli-0.1.0/plugcli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:57:40.543175 plugcli-0.1.0/plugcli/tests/plugin_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/tests/plugin_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/tests/plugin_examples/exampleA.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/tests/plugin_examples/exampleB.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/tests/test_plugin_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-03-15 17:57:23.000000 plugcli-0.1.0/plugcli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:57:40.543175 plugcli-0.1.0/plugcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-03-15 17:57:40.000000 plugcli-0.1.0/plugcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-15 17:57:40.000000 plugcli-0.1.0/plugcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 17:57:40.000000 plugcli-0.1.0/plugcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-15 17:57:40.000000 plugcli-0.1.0/plugcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-15 17:57:40.000000 plugcli-0.1.0/plugcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-15 17:57:40.543175 plugcli-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-03-15 17:57:23.000000 plugcli-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:43:37.499706 plugcli-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-07 21:43:22.000000 plugcli-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 21:43:22.000000 plugcli-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-07 21:43:37.499706 plugcli-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-07 21:43:22.000000 plugcli-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:43:37.499706 plugcli-0.2.0/plugcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 21:43:37.000000 plugcli-0.2.0/plugcli/_installed_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/plugin_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:43:37.499706 plugcli-0.2.0/plugcli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:43:37.499706 plugcli-0.2.0/plugcli/tests/plugin_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/tests/plugin_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/tests/plugin_examples/exampleA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/tests/plugin_examples/exampleB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/tests/test_plugin_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-06-07 21:43:22.000000 plugcli-0.2.0/plugcli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:43:37.499706 plugcli-0.2.0/plugcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-07 21:43:37.000000 plugcli-0.2.0/plugcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 21:43:37.000000 plugcli-0.2.0/plugcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:43:37.000000 plugcli-0.2.0/plugcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 21:43:37.000000 plugcli-0.2.0/plugcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 21:43:37.000000 plugcli-0.2.0/plugcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-07 21:43:37.499706 plugcli-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-07 21:43:22.000000 plugcli-0.2.0/setup.py
```

### Comparing `plugcli-0.1.0/LICENSE` & `plugcli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plugcli-0.1.0/PKG-INFO` & `plugcli-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugcli
-Version: 0.1.0
+Version: 0.2.0
 Summary: Plugin based CLI framework built on click
 Home-page: https://github.com/dwhswenson/plugcli
 Author: David W.H. Swenson
 Author-email: dwhs@hyperblazer.net
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `plugcli-0.1.0/README.md` & `plugcli-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `plugcli-0.1.0/plugcli/cli.py` & `plugcli-0.2.0/plugcli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,17 @@
     def _command_sections(self):
         try:
             return self.COMMAND_SECTIONS
         except AttributeError:
             raise NotImplementedError("Subclasses must include class "
                                       "variable 'COMMAND_SECTIONS'")
 
+    def _section_label(self, section_name):
+        return section_name + " Commands"
+
     def _register_plugin(self, plugin):
         self.plugins.append(plugin)
         # normalize underscores to hyphens
         name = plugin.name.replace('_', '-')
         self._get_command[name] = plugin.command
         self._sections[plugin.section].append(name)
 
@@ -61,22 +64,31 @@
     def list_commands(self, ctx):
         return list(self._get_command.keys())
 
     def get_command(self, ctx, name):
         name = name.replace('_', '-')  # allow - or _ from user
         return self._get_command.get(name)
 
+    def _section_sort_commands(self, section, commands):
+        """
+        Parameters
+        ----------
+        section : str
+        commands : Iterable[str]
+        """
+        yield from commands
+
     def format_commands(self, ctx, formatter):
         for sec in self._command_sections:
             cmds = self._sections.get(sec, [])
             rows = []
-            for cmd in cmds:
+            for cmd in self._section_sort_commands(sec, cmds):
                 command = self.get_command(ctx, cmd)
                 if command is None:
                     # TODO: there is test code that claims to cover this,
                     # but it isn't getting covered; investigate why
                     continue
                 rows.append((cmd, command.short_help or ''))
 
             if rows:
-                with formatter.section(sec + " Commands"):
+                with formatter.section(self._section_label(sec)):
                     formatter.write_dl(rows)
```

### Comparing `plugcli-0.1.0/plugcli/params.py` & `plugcli-0.2.0/plugcli/params.py`

 * *Files identical despite different names*

### Comparing `plugcli-0.1.0/plugcli/plugin_management.py` & `plugcli-0.2.0/plugcli/plugin_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                       for f in os.listdir(self.search_path)
                       if is_plugin(f)]
         return candidates
 
     @staticmethod
     def _make_nsdict(candidate):
         ns = {}
-        with open(candidate) as f:
+        with open(candidate, encoding='utf-8') as f:
             code = compile(f.read(), candidate, 'exec')
             eval(code, ns, ns)
         return ns
 
 
 class NamespacePluginLoader(CLIPluginLoader):
     """Load namespace plugins (plugins for wide distribution)
```

### Comparing `plugcli-0.1.0/plugcli/tests/test_cli.py` & `plugcli-0.2.0/plugcli/tests/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,17 +48,35 @@
         self.plugin_dict = {
             'foo': foo_plugin,
             'foo-bar': foobar_plugin,
             'baz-qux': underscored_plugin,
         }
         return [foo_plugin, foobar_plugin]
 
+class MockFormatter(object):
+    def __init__(self):
+        self.title = None
+        self.contents = {}
+
+    def section(self, title):
+        self.title = title
+        return MagicMock()
+
+    def write_dl(self, rows):
+        self.contents[self.title] = rows
+
+
+class FakeCLIResorted(FakeCLI):
+    def _section_sort_commands(self, section, commands):
+        # default is foo-bar then baz-qux, this should flip the order
+        yield from sorted(commands)
+
 
 class TestCLI(object):
-    def setup(self):
+    def setup_method(self):
         self.cli = FakeCLI()
         self.plugin_dict = self.cli.plugin_dict
         self.plugins = list(self.cli.plugin_dict.values())
         # need to copy the plugins since we're changing the list
         for plugin in self.cli.plugins[:]:
             self.cli._deregister_plugin(plugin)
 
@@ -86,38 +104,48 @@
     ])
     def test_get_command(self, command, output):
         # this tests that renamings work
         cmd = self.cli.get_command(ctx=None, name=command)
         assert cmd() == output
 
     def test_format_commands(self):
-        class MockFormatter(object):
-            def __init__(self):
-                self.title = None
-                self.contents = {}
-
-            def section(self, title):
-                self.title = title
-                return MagicMock()
-
-            def write_dl(self, rows):
-                self.contents[self.title] = rows
-
         formatter = MockFormatter()
         # add a non-existent command; tests when get_command is None
         self.cli._sections['Workflow'] = ['baz']
         self.cli.format_commands(ctx=None, formatter=formatter)
         foo_row = ('foo', 'foo help')
         foobar_row = ('foo-bar', '')
         bazqux_row = ('baz-qux', '')
         assert formatter.contents['Simulation Commands'] == [foo_row]
         assert formatter.contents['Miscellaneous Commands'] == [foobar_row,
-                                                               bazqux_row]
+                                                                bazqux_row]
         assert len(formatter.contents) == 2
 
+    def test_section_sort_commands(self):
+        cli = FakeCLIResorted()
+        # deal with the fact that baz-qux isn't registered
+        plugins = list(cli.plugin_dict.values())
+        assert len(plugins) == 3
+        for plugin in cli.plugins[:]:
+            cli._deregister_plugin(plugin)
+
+        for plugin in plugins:
+            cli._register_plugin(plugin)
+
+        assert len(cli.plugins) == 3
+
+        formatter = MockFormatter()
+        cli.format_commands(ctx=None, formatter=formatter)
+        foo_row = ('foo', 'foo help')
+        foobar_row = ('foo-bar', '')
+        bazqux_row = ('baz-qux', '')
+        assert formatter.contents['Simulation Commands'] == [foo_row]
+        assert formatter.contents['Miscellaneous Commands'] == [bazqux_row,
+                                                                foobar_row]
+
 
 def test_abstract_no_command_section():
     # If COMMAND_SECTIONS is not defined, format_commands raises
     # NotImplementedError
     class MyCLI(CLI):
         def get_installed_plugins(self):
             return []
```

### Comparing `plugcli-0.1.0/plugcli/tests/test_params.py` & `plugcli-0.2.0/plugcli/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `plugcli-0.1.0/plugcli/tests/test_plugin_management.py` & `plugcli-0.2.0/plugcli/tests/test_plugin_management.py`

 * *Files identical despite different names*

### Comparing `plugcli-0.1.0/plugcli/version.py` & `plugcli-0.2.0/plugcli/version.py`

 * *Files identical despite different names*

### Comparing `plugcli-0.1.0/plugcli.egg-info/PKG-INFO` & `plugcli-0.2.0/plugcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugcli
-Version: 0.1.0
+Version: 0.2.0
 Summary: Plugin based CLI framework built on click
 Home-page: https://github.com/dwhswenson/plugcli
 Author: David W.H. Swenson
 Author-email: dwhs@hyperblazer.net
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `plugcli-0.1.0/plugcli.egg-info/SOURCES.txt` & `plugcli-0.2.0/plugcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plugcli-0.1.0/setup.cfg` & `plugcli-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plugcli
-version = 0.1.0
+version = 0.2.0
 short_description = Plugin based CLI framework built on click
 description = Plugin based CLI framework built on click
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = David W.H. Swenson
 license = MIT
 license_file = LICENSE
```

### Comparing `plugcli-0.1.0/setup.py` & `plugcli-0.2.0/setup.py`

 * *Files identical despite different names*

