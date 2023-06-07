# Comparing `tmp/cfg-argparser-1.1.5.tar.gz` & `tmp/cfg-argparser-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfg-argparser-1.1.5.tar", last modified: Tue May 23 20:56:34 2023, max compression
+gzip compressed data, was "cfg-argparser-1.2.0.tar", last modified: Wed Jun  7 05:59:14 2023, max compression
```

## Comparing `cfg-argparser-1.1.5.tar` & `cfg-argparser-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-23 20:56:34.949829 cfg-argparser-1.1.5/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.1.5/LICENSE
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-23 20:56:34.949829 cfg-argparser-1.1.5/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1285 2023-05-23 20:53:17.000000 cfg-argparser-1.1.5/README.md
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      874 2023-05-23 20:51:42.000000 cfg-argparser-1.1.5/pyproject.toml
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-05-23 20:56:34.949829 cfg-argparser-1.1.5/setup.cfg
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-23 20:56:34.946496 cfg-argparser-1.1.5/src/
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-23 20:56:34.949829 cfg-argparser-1.1.5/src/cfg_argparser/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      125 2023-05-18 23:35:00.000000 cfg-argparser-1.1.5/src/cfg_argparser/__init__.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2395 2023-05-18 23:40:33.000000 cfg-argparser-1.1.5/src/cfg_argparser/cfg_dict.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)    10048 2023-05-18 23:34:21.000000 cfg-argparser-1.1.5/src/cfg_argparser/config_arg_parser.py
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-23 20:56:34.949829 cfg-argparser-1.1.5/src/cfg_argparser.egg-info/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-23 20:56:34.000000 cfg-argparser-1.1.5/src/cfg_argparser.egg-info/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      295 2023-05-23 20:56:34.000000 cfg-argparser-1.1.5/src/cfg_argparser.egg-info/SOURCES.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-05-23 20:56:34.000000 cfg-argparser-1.1.5/src/cfg_argparser.egg-info/dependency_links.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-05-23 20:56:34.000000 cfg-argparser-1.1.5/src/cfg_argparser.egg-info/top_level.txt
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 05:59:14.646680 cfg-argparser-1.2.0/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.2.0/LICENSE
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1667 2023-06-07 05:59:14.646680 cfg-argparser-1.2.0/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      812 2023-06-07 05:54:45.000000 cfg-argparser-1.2.0/README.md
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      929 2023-06-07 04:30:47.000000 cfg-argparser-1.2.0/pyproject.toml
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-06-07 05:59:14.646680 cfg-argparser-1.2.0/setup.cfg
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 05:59:14.640013 cfg-argparser-1.2.0/src/
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 05:59:14.643346 cfg-argparser-1.2.0/src/cfg_argparser/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      316 2023-06-07 03:20:42.000000 cfg-argparser-1.2.0/src/cfg_argparser/__init__.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     9978 2023-06-07 01:13:05.000000 cfg-argparser-1.2.0/src/cfg_argparser/argparse_config.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2882 2023-06-07 05:11:51.000000 cfg-argparser-1.2.0/src/cfg_argparser/cfg_dict.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1486 2023-06-07 05:55:21.000000 cfg-argparser-1.2.0/src/cfg_argparser/function_config_wrapper.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1391 2023-06-07 04:44:11.000000 cfg-argparser-1.2.0/src/cfg_argparser/save_handlers.py
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 05:59:14.643346 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1667 2023-06-07 05:59:14.000000 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      413 2023-06-07 05:59:14.000000 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/SOURCES.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-06-07 05:59:14.000000 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/dependency_links.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       20 2023-06-07 05:59:14.000000 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/requires.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-06-07 05:59:14.000000 cfg-argparser-1.2.0/src/cfg_argparser.egg-info/top_level.txt
```

### Comparing `cfg-argparser-1.1.5/LICENSE` & `cfg-argparser-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.1.5/PKG-INFO` & `cfg-argparser-1.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.1.5
+Version: 1.2.0
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: typer
 License-File: LICENSE
 
 # cfg_argparser 1.1.5
 
 a config wrapper I made to be easily applied to argparse objects.
 
 ## Installation
@@ -33,49 +34,23 @@
 pip install -e .
 
 ```
 
 ## Example
 
 ```python
-import argparse
+from cfg_argparser import wrap_config, CfgDict
 
-from cfg_argparser import ConfigArgParser
-
-
-def parser() -> argparse.ArgumentParser:
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--file")
-    return parser
+cfg = CfgDict("test.json")
+@wrap_config(cfg)
+def test_function(s: str, is_real: bool = True): # I'd advise only wrapping functions all having default methods
+    return f"{s} is {'real' if is_real else 'fake'}"
 
 if __name__ == "__main__":
-    args = ConfigArgParser(parser(),
-                           "config.json",
-                           exit_on_change=True).parse_args()
-    print(args.file)
-```
-
-Wrapping the `ConfigArgParser` around `parser()` adds a few "magic" arguments.
-here's what it adds:
-
-```rich
-Config options:
-  --set KEY VAL        change a default argument's options
-  --reset [VALUE ...]  removes a changed option.
-  --reset_all          resets every option.
-```
-
-Here's what it looks like in practice:
-
-```null
-> python example.py
-None
-> python example.py --file foo.txt
-foo.txt
-> python example.py --set file foo.txt
-> python example.py
-foo.txt
+  print(test_function("We"))
+  cfg['s'] = "us"
+  print(test_function()) # Linters hate him!
 ```
 
 ## Compatibilty
 
 This was mainly tested on 3.9 and 3.10, but it should work from 3.6 onwards. i can't test earlier versions for some reason.
```

### Comparing `cfg-argparser-1.1.5/pyproject.toml` & `cfg-argparser-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools", "toml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfg-argparser"
-version = "1.1.5"
+version = "1.2.0"
 authors = [{ name = "Zeptofine", email = "zeptofine@gmail.com" }]
 description = "A package designed to simplify configurable defaults from argparse."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
@@ -20,7 +20,10 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zeptofine/cfg-argparser"
 "Bug Tracker" = "https://github.com/zeptofine/cfg-argparser/issues"
+
+[project.optional-dependencies]
+typer=['typer[all]']
```

### Comparing `cfg-argparser-1.1.5/src/cfg_argparser/config_arg_parser.py` & `cfg-argparser-1.2.0/src/cfg_argparser/argparse_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-
 from argparse import ArgumentParser, Namespace
 from sys import exit as sys_exit
 
 from .cfg_dict import CfgDict
 
 
 class ParserTree(dict):
     def __init__(self, argparser: ArgumentParser):
         super().__init__()
         self.parser = argparser
         self.update(ParserTree.parser_to_tree(argparser))
 
     @staticmethod
     def parser_to_tree(argparser: ArgumentParser):
-        new = {'parent': argparser}
+        new = {"parent": argparser}
 
         if argparser._actions:
             # make a new key dict that represents the parser's arguments
-            new.update({
-                'actions': {
-                    action.dest: action
-                    for action in
-                    argparser._actions
-                    if not action.default == '==SUPPRESS=='
+            new.update(
+                {
+                    "actions": {
+                        action.dest: action for action in argparser._actions if not action.default == "==SUPPRESS=="
+                    }
                 }
-            })
+            )
 
         subparser = ParserTree.get_subparsers(argparser)
         if subparser:
             # make a new key dict that represents the parser's subparser and choices in a sub-ParserTree
-            new['subparsers'] = {
-                'group': subparser,
-                'choices': {dest: ParserTree(parser) for dest, parser in subparser.choices.items()},
+            new["subparsers"] = {
+                "group": subparser,
+                "choices": {dest: ParserTree(parser) for dest, parser in subparser.choices.items()},
             }
 
         return new
 
     def get_defaults(self):
         return ParserTree.defaults_from_tree(self)
 
@@ -44,20 +42,20 @@
 
     def disable_required(self):
         # returns a partial tree representing all of the actions that don't have a default
         return ParserTree._disable_required_with_defaults(self)
 
     def parse(self):
         # Main issue is that it doesn't take in account bad arguments
-        known, _ = self['parent'].parse_known_args()
+        known, _ = self["parent"].parse_known_args()
 
-        if 'subparsers' in self:
-            subparser = self['subparsers']['group']
-            if subparser.default and subparser.default in self['subparsers']['choices']:
-                return self.combine_namespaces(known, self['subparsers']['choices'][subparser.default].parse())
+        if "subparsers" in self:
+            subparser = self["subparsers"]["group"]
+            if subparser.default and subparser.default in self["subparsers"]["choices"]:
+                return self.combine_namespaces(known, self["subparsers"]["choices"][subparser.default].parse())
         return known
 
     @staticmethod
     def combine_namespaces(*namespaces: Namespace):
         dct = {}
         for namespace in namespaces:
             dct.update(namespace.__dict__)
@@ -66,198 +64,209 @@
     @staticmethod
     def get_subparsers(argparser: ArgumentParser):
         subparser = argparser._subparsers
         if subparser:
             return subparser._group_actions[0]
 
     @staticmethod
-    def flatten(argdict: dict, sep='.'):
+    def flatten(argdict: dict, sep="."):
         out_dict = {}
         for key, value in argdict.items():
             if isinstance(value, dict):
                 for subkey, subvalue in ParserTree.flatten(value, sep).items():
                     out_dict[f"{key}{sep}{subkey}"] = subvalue
             else:
                 out_dict[key] = value
         return out_dict
 
     @staticmethod
     def defaults_from_tree(parser_tree):
         out = {}
-        if 'actions' in parser_tree:
-            out.update({
-                dest: action.default
-                for dest, action in parser_tree['actions'].items()
-                if action.default != '==SUPPRESS=='
-            })
-        if 'subparsers' in parser_tree:
-            out.update({
-                dest: subparser.get_defaults()
-                for dest, subparser in parser_tree['subparsers']['choices'].items()
-            })
+        if "actions" in parser_tree:
+            out.update(
+                {
+                    dest: action.default
+                    for dest, action in parser_tree["actions"].items()
+                    if action.default != "==SUPPRESS=="
+                }
+            )
+        if "subparsers" in parser_tree:
+            out.update(
+                {dest: subparser.get_defaults() for dest, subparser in parser_tree["subparsers"]["choices"].items()}
+            )
         return out
 
     @staticmethod
     def update_from_flattened_recurs(original, flattened):
         for key, item in flattened.items():
-            if '.' in key:
+            if "." in key:
                 key, future = key.split(".", 1)
-                if 'subparsers' in original and key in original['subparsers']['choices']:
-                    ParserTree.update_from_flattened_recurs(original['subparsers']['choices'][key], {future: item})
+                if "subparsers" in original and key in original["subparsers"]["choices"]:
+                    ParserTree.update_from_flattened_recurs(original["subparsers"]["choices"][key], {future: item})
             else:
-                if 'actions' in original and key in original['actions']:
-                    original['actions'][key].default = item
+                if "actions" in original and key in original["actions"]:
+                    original["actions"][key].default = item
 
     @staticmethod
     def _disable_required_with_defaults(subtree):
         still_required = {}
-        if 'actions' in subtree:
-            for dest, action in subtree['actions'].items():
+        if "actions" in subtree:
+            for dest, action in subtree["actions"].items():
                 if action.required:
                     if action.default:
                         action.required = False
                     else:
-                        if 'actions' not in still_required:
-                            still_required['actions'] = {}
-                        still_required['actions'][dest] = action
+                        if "actions" not in still_required:
+                            still_required["actions"] = {}
+                        still_required["actions"][dest] = action
                         action.required = False
-        if 'subparsers' in subtree:
-            still_required['subparsers'] = {'choices': {}}
-            for dest, subtree in subtree['subparsers']['choices'].items():
+        if "subparsers" in subtree:
+            still_required["subparsers"] = {"choices": {}}
+            for dest, subtree in subtree["subparsers"]["choices"].items():
                 out = subtree.disable_required()
                 if out:
-                    still_required['subparsers']['choices'].update({dest: out})
+                    still_required["subparsers"]["choices"].update({dest: out})
 
         return still_required
 
     @staticmethod
     def reenable_required(required):
-        if 'actions' in required:
-            for dest, action in required['actions'].items():
+        if "actions" in required:
+            for dest, action in required["actions"].items():
                 if not action.default:
                     action.required = True
-        if 'subparsers' in required:
-            for dest, subparser in required['subparsers']['choices'].items():
+        if "subparsers" in required:
+            for dest, subparser in required["subparsers"]["choices"].items():
                 ParserTree.reenable_required(subparser)
 
     # def __getitem__(self, key):
     #     if not isinstance(key, tuple):
     #         return super().__getitem__(key)
     #     else:
     #         return self.subparsers[key[0]][key[1:]]
 
 
 def update_from_flattened(original, flattened):
     for key, value in flattened.items():
-        if '.' in key:
-            key, future = key.split('.', 1)
+        if "." in key:
+            key, future = key.split(".", 1)
             if key not in original:
                 original[key] = {}
             update_from_flattened(original[key], {future: value})
         else:
             original[key] = value
 
 
-class ConfigArgParser:
-    '''an easy argparse config utility. It saves given args to a json, and returns them when args are parsed again.'''
+class ArgparseConfig:
+    """an easy argparse config utility. It saves given args to a json, and returns them when args are parsed again."""
 
-    def __init__(self,
-                 parser: ArgumentParser,
-                 config_path: str,
-                 cfgObject: CfgDict = None,
-                 exit_on_change: bool = False,
-                 argument_group_name: str = "Config options"):
+    def __init__(
+        self,
+        parser: ArgumentParser,
+        config_path: str,
+        cfg_object: CfgDict | None = None,
+        exit_on_change: bool = False,
+        argument_group_name: str = "Config options",
+    ):
         """Constructs a parser wrapper.
 
         Parameters
         ----------
         parser : ArgumentParser
             parser to wrap.
         config_path : str
             the path to the json file.
-        cfgObject : CfgDict, optional
+        cfg_object : CfgDict, optional
             if desired, update an existing CfgDict object, by default None
         exit_on_change : bool, optional
             exits when set, reset, or reset_all is called, by default False
         argument_group_name : str, optional
             name of the argument group, by default "Config options"
 
         """
 
         # parent parser
         self.parser = parser
         self.default_prefix = self.parser.prefix_chars[0]
         self.exit_on_change = exit_on_change
-        self.file = cfgObject or CfgDict(config_path)
+        self.file = cfg_object or CfgDict(config_path)
 
         # Add config options
         self.config_option_group = self.parser.add_argument_group(argument_group_name)
         self.config_options = self.config_option_group.add_mutually_exclusive_group()
-        self.config_options.add_argument(self.default_prefix * 2 + "set", nargs=2, metavar=('KEY', 'VAL'),
-                                         help="change a default argument's options")
-        self.config_options.add_argument(self.default_prefix * 2 + "reset", metavar='VALUE', nargs="*",
-                                         help="removes a changed option.")
-        self.config_options.add_argument(self.default_prefix * 2 + "reset_all", action="store_true",
-                                         help="resets every option.")
+        self.config_options.add_argument(
+            self.default_prefix * 2 + "set",
+            nargs=2,
+            metavar=("KEY", "VAL"),
+            help="change a default argument's options",
+        )
+        self.config_options.add_argument(
+            self.default_prefix * 2 + "reset",
+            metavar="VALUE",
+            nargs="*",
+            help="removes a changed option.",
+        )
+        self.config_options.add_argument(
+            self.default_prefix * 2 + "reset_all",
+            action="store_true",
+            help="resets every option.",
+        )
 
         # get defaults from the actions
-        # self.parser_tree = get_parser_tree(self._parent)
         self.parser_tree = ParserTree(self.parser)
 
-    def parse_args(self, **kwargs) -> Namespace:
-        '''args.set, reset, reset_all logic. Also a passthrough for parser.parse_args.'''
+    def parse_args(self, *args, **kwargs) -> Namespace:
+        """args.set, reset, reset_all logic. Also a passthrough for parser.parse_args."""
 
         self.file.load()
 
         # Add subparsers to the dict so it can be configured
         self.parser_tree.update_from_flattened(ParserTree.flatten(self.file))
 
-        self.kwargs = ParserTree.flatten(self.parser_tree.get_defaults())
-
         # disable every required item that wasn in the file
         still_required = self.parser_tree.disable_required()
 
-        self.parsed_args, _ = self.parser.parse_known_args(**kwargs)
+        parsed_args, _ = self.parser.parse_known_args(*args, **kwargs)
+
+        flattened_kwargs = ParserTree.flatten(self.parser_tree.get_defaults())
 
         # TODO: make set, reset, and reset_all work for subparsers
         # set defaults
-        if self.parsed_args.set or self.parsed_args.reset or self.parsed_args.reset_all:
-            if self.parsed_args.set:
-                potential_args = self.parsed_args.set
+        if parsed_args.set or parsed_args.reset or parsed_args.reset_all:
+            if parsed_args.set:
+                potential_args = parsed_args.set
                 # convert potential_args to respective types
                 potential_args = self._convert_type(potential_args)
-                if not potential_args[0] in self.kwargs:
+                if not potential_args[0] in flattened_kwargs:
                     sys_exit("Given key not found")
 
                 update_from_flattened(self.file, {potential_args[0]: potential_args[1]})
 
-            elif self.parsed_args.reset:
-                for arg in self.parsed_args.reset:
+            elif parsed_args.reset:
+                for arg in parsed_args.reset:
                     self._pop_from_flattened(self.file, arg)
 
-            elif self.parsed_args.reset_all:
+            elif parsed_args.reset_all:
                 self.file.clear()
             self.file.save().load()
 
             if self.exit_on_change:
                 sys_exit()
 
         # edit defaults
         self.parser_tree.update_from_flattened(ParserTree.flatten(self.file))
 
         # reenable every required item except for the ones with defaults
         ParserTree.reenable_required(still_required)
 
         # sys_exit()
-        self.parser.parse_args()
+        self.parser.parse_args(*args, **kwargs)
 
         return self.parser_tree.parse()
 
     @staticmethod
     def _convert_type(potential_args: list) -> list:
-        arg_replacements = {"true": True, "false": False,
-                            "none": None, "null": None}
-        potential_args[1] = arg_replacements.get(
-            potential_args[1].lower(), potential_args[1])
+        arg_replacements = {"true": True, "false": False, "none": None, "null": None}
+        potential_args[1] = arg_replacements.get(potential_args[1].lower(), potential_args[1])
         if str(potential_args[1]).isdigit():
             potential_args[1] = int(potential_args[1])
         return potential_args
```

### Comparing `cfg-argparser-1.1.5/src/cfg_argparser.egg-info/PKG-INFO` & `cfg-argparser-1.2.0/src/cfg_argparser.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.1.5
+Version: 1.2.0
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: typer
 License-File: LICENSE
 
 # cfg_argparser 1.1.5
 
 a config wrapper I made to be easily applied to argparse objects.
 
 ## Installation
@@ -33,49 +34,23 @@
 pip install -e .
 
 ```
 
 ## Example
 
 ```python
-import argparse
+from cfg_argparser import wrap_config, CfgDict
 
-from cfg_argparser import ConfigArgParser
-
-
-def parser() -> argparse.ArgumentParser:
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--file")
-    return parser
+cfg = CfgDict("test.json")
+@wrap_config(cfg)
+def test_function(s: str, is_real: bool = True): # I'd advise only wrapping functions all having default methods
+    return f"{s} is {'real' if is_real else 'fake'}"
 
 if __name__ == "__main__":
-    args = ConfigArgParser(parser(),
-                           "config.json",
-                           exit_on_change=True).parse_args()
-    print(args.file)
-```
-
-Wrapping the `ConfigArgParser` around `parser()` adds a few "magic" arguments.
-here's what it adds:
-
-```rich
-Config options:
-  --set KEY VAL        change a default argument's options
-  --reset [VALUE ...]  removes a changed option.
-  --reset_all          resets every option.
-```
-
-Here's what it looks like in practice:
-
-```null
-> python example.py
-None
-> python example.py --file foo.txt
-foo.txt
-> python example.py --set file foo.txt
-> python example.py
-foo.txt
+  print(test_function("We"))
+  cfg['s'] = "us"
+  print(test_function()) # Linters hate him!
 ```
 
 ## Compatibilty
 
 This was mainly tested on 3.9 and 3.10, but it should work from 3.6 onwards. i can't test earlier versions for some reason.
```

