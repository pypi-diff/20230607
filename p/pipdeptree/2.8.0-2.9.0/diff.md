# Comparing `tmp/pipdeptree-2.8.0.tar.gz` & `tmp/pipdeptree-2.9.0.tar.gz`

## Comparing `pipdeptree-2.8.0.tar` & `pipdeptree-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.prettierrc.toml
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/CHANGES.md
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/tox.ini
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/whitelist.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.github/workflows/check.yml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.github/workflows/release.yml
--rw-r--r--   0        0        0    97568 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/docs/twine-pdt.png
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/docs/v2beta-opts.org
--rw-r--r--   0        0        0    37458 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/src/pipdeptree/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/src/pipdeptree/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/src/pipdeptree/version.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/tests/guess_version_setuptools.py
--rw-r--r--   0        0        0    30300 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/tests/test_pipdeptree.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/LICENSE
--rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/README.md
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/pyproject.toml
--rw-r--r--   0        0        0    15544 2020-02-02 00:00:00.000000 pipdeptree-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.prettierrc.toml
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/CHANGES.md
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/tox.ini
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/whitelist.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.github/workflows/check.yml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0    97568 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/docs/twine-pdt.png
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/docs/v2beta-opts.org
+-rw-r--r--   0        0        0    37997 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/src/pipdeptree/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/src/pipdeptree/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/src/pipdeptree/version.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/tests/guess_version_setuptools.py
+-rw-r--r--   0        0        0    34625 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/tests/test_pipdeptree.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/LICENSE
+-rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/README.md
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0    15544 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/PKG-INFO
```

### Comparing `pipdeptree-2.8.0/.pre-commit-config.yaml` & `pipdeptree-2.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.8.0/CHANGES.md` & `pipdeptree-2.9.0/CHANGES.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.8.0/tox.ini` & `pipdeptree-2.9.0/tox.ini`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.8.0/.github/workflows/check.yml` & `pipdeptree-2.9.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.8.0/.github/workflows/release.yml` & `pipdeptree-2.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.8.0/docs/twine-pdt.png` & `pipdeptree-2.9.0/docs/twine-pdt.png`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.8.0/docs/v2beta-opts.org` & `pipdeptree-2.9.0/docs/v2beta-opts.org`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.8.0/src/pipdeptree/__init__.py` & `pipdeptree-2.9.0/src/pipdeptree/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,15 +451,15 @@
                     node = v.as_parent_of(None)
                 m[node].append(k)
             if k.key not in child_keys:
                 m[k.dist] = []
         return PackageDAG(dict(m))
 
 
-def render_text(tree, list_all=True, frozen=False):
+def render_text(tree, max_depth, list_all=True, frozen=False):
     """Print tree as text on console
 
     :param dict tree: the package tree
     :param bool list_all: whether to list all the pgks at the root level or only those that are the sub-dependencies
     :param bool frozen: show the names of the pkgs in the output that's favourable to pip --freeze
     :returns: None
     """
@@ -467,20 +467,20 @@
     nodes = tree.keys()
     branch_keys = {r.key for r in chain.from_iterable(tree.values())}
 
     if not list_all:
         nodes = [p for p in nodes if p.key not in branch_keys]
 
     if sys.stdout.encoding.lower() in ("utf-8", "utf-16", "utf-32"):
-        _render_text_with_unicode(tree, nodes, frozen)
+        _render_text_with_unicode(tree, nodes, max_depth, frozen)
     else:
-        _render_text_without_unicode(tree, nodes, frozen)
+        _render_text_without_unicode(tree, nodes, max_depth, frozen)
 
 
-def _render_text_with_unicode(tree, nodes, frozen):
+def _render_text_with_unicode(tree, nodes, max_depth, frozen):
     use_bullets = not frozen
 
     def aux(
         node,
         parent=None,
         indent=0,
         cur_chain=None,
@@ -529,38 +529,38 @@
                 prefix=next_prefix,
                 depth=depth + 1,
                 has_grand_parent=parent is not None,
                 is_last_child=c is children[-1],
                 parent_is_last_child=is_last_child,
             )
             for c in children
-            if c.project_name not in cur_chain
+            if c.project_name not in cur_chain and depth + 1 <= max_depth
         ]
 
         result += list(chain.from_iterable(children_strings))
         return result
 
     lines = chain.from_iterable([aux(p) for p in nodes])
     print("\n".join(lines))
 
 
-def _render_text_without_unicode(tree, nodes, frozen):
+def _render_text_without_unicode(tree, nodes, max_depth, frozen):
     use_bullets = not frozen
 
-    def aux(node, parent=None, indent=0, cur_chain=None):
+    def aux(node, parent=None, indent=0, cur_chain=None, depth=0):
         cur_chain = cur_chain or []
         node_str = node.render(parent, frozen)
         if parent:
             prefix = " " * indent + ("- " if use_bullets else "")
             node_str = prefix + node_str
         result = [node_str]
         children = [
-            aux(c, node, indent=indent + 2, cur_chain=cur_chain + [c.project_name])
+            aux(c, node, indent=indent + 2, cur_chain=cur_chain + [c.project_name], depth=depth + 1)
             for c in tree.get_children(node.key)
-            if c.project_name not in cur_chain
+            if c.project_name not in cur_chain and depth + 1 <= max_depth
         ]
         result += list(chain.from_iterable(children))
         return result
 
     lines = chain.from_iterable([aux(p) for p in nodes])
     print("\n".join(lines))
 
@@ -967,14 +967,24 @@
         dest="output_format",
         help=(
             "Print a dependency graph in the specified output "
             "format. Available are all formats supported by "
             "GraphViz, e.g.: dot, jpeg, pdf, png, svg"
         ),
     )
+    parser.add_argument(
+        "-d",
+        "--depth",
+        type=lambda x: int(x) if x.isdigit() and (int(x) >= 0) else parser.error("Depth must be a number that is >= 0"),
+        default=float("inf"),
+        help=(
+            "Display dependency tree up to a depth >=0 using the default text display. All other display options"
+            " ignore this argument."
+        ),
+    )
     return parser
 
 
 def _get_args():
     parser = get_parser()
     return parser.parse_args()
 
@@ -1073,10 +1083,10 @@
         print(render_json_tree(tree, indent=4))
     elif args.mermaid:
         print(render_mermaid(tree))
     elif args.output_format:
         output = dump_graphviz(tree, output_format=args.output_format, is_reverse=args.reverse)
         print_graphviz(output)
     else:
-        render_text(tree, args.all, args.freeze)
+        render_text(tree, args.depth, args.all, args.freeze)
 
     return return_code
```

### Comparing `pipdeptree-2.8.0/tests/test_pipdeptree.py` & `pipdeptree-2.9.0/tests/test_pipdeptree.py`

 * *Files 18% similar despite different names*

```diff
@@ -464,15 +464,112 @@
         ),
     ],
 )
 def test_render_text(capsys, list_all, reverse, unicode, expected_output):
     tree = t.reverse() if reverse else t
     encoding = "utf-8" if unicode else "ascii"
     with mock.patch("sys.stdout", MockStdout(encoding)):
-        p.render_text(tree, list_all=list_all, frozen=False)
+        p.render_text(tree, float("inf"), list_all=list_all, frozen=False)
+        captured = capsys.readouterr()
+        assert "\n".join(expected_output).strip() == captured.out.strip()
+
+
+@pytest.mark.parametrize(
+    ("unicode", "level", "expected_output"),
+    [
+        (
+            True,
+            0,
+            [
+                "a==3.4.0",
+                "b==2.3.1",
+                "c==5.10.0",
+                "d==2.35",
+                "e==0.12.1",
+                "f==3.1",
+                "g==6.8.3rc1",
+            ],
+        ),
+        (
+            False,
+            0,
+            [
+                "a==3.4.0",
+                "b==2.3.1",
+                "c==5.10.0",
+                "d==2.35",
+                "e==0.12.1",
+                "f==3.1",
+                "g==6.8.3rc1",
+            ],
+        ),
+        (
+            True,
+            2,
+            [
+                "a==3.4.0",
+                "├── b [required: >=2.0.0, installed: 2.3.1]",
+                "│   └── d [required: >=2.30,<2.42, installed: 2.35]",
+                "└── c [required: >=5.7.1, installed: 5.10.0]",
+                "    ├── d [required: >=2.30, installed: 2.35]",
+                "    └── e [required: >=0.12.1, installed: 0.12.1]",
+                "b==2.3.1",
+                "└── d [required: >=2.30,<2.42, installed: 2.35]",
+                "    └── e [required: >=0.9.0, installed: 0.12.1]",
+                "c==5.10.0",
+                "├── d [required: >=2.30, installed: 2.35]",
+                "│   └── e [required: >=0.9.0, installed: 0.12.1]",
+                "└── e [required: >=0.12.1, installed: 0.12.1]",
+                "d==2.35",
+                "└── e [required: >=0.9.0, installed: 0.12.1]",
+                "e==0.12.1",
+                "f==3.1",
+                "└── b [required: >=2.1.0, installed: 2.3.1]",
+                "    └── d [required: >=2.30,<2.42, installed: 2.35]",
+                "g==6.8.3rc1",
+                "├── e [required: >=0.9.0, installed: 0.12.1]",
+                "└── f [required: >=3.0.0, installed: 3.1]",
+                "    └── b [required: >=2.1.0, installed: 2.3.1]",
+            ],
+        ),
+        (
+            False,
+            2,
+            [
+                "a==3.4.0",
+                "  - b [required: >=2.0.0, installed: 2.3.1]",
+                "    - d [required: >=2.30,<2.42, installed: 2.35]",
+                "  - c [required: >=5.7.1, installed: 5.10.0]",
+                "    - d [required: >=2.30, installed: 2.35]",
+                "    - e [required: >=0.12.1, installed: 0.12.1]",
+                "b==2.3.1",
+                "  - d [required: >=2.30,<2.42, installed: 2.35]",
+                "    - e [required: >=0.9.0, installed: 0.12.1]",
+                "c==5.10.0",
+                "  - d [required: >=2.30, installed: 2.35]",
+                "    - e [required: >=0.9.0, installed: 0.12.1]",
+                "  - e [required: >=0.12.1, installed: 0.12.1]",
+                "d==2.35",
+                "  - e [required: >=0.9.0, installed: 0.12.1]",
+                "e==0.12.1",
+                "f==3.1",
+                "  - b [required: >=2.1.0, installed: 2.3.1]",
+                "    - d [required: >=2.30,<2.42, installed: 2.35]",
+                "g==6.8.3rc1",
+                "  - e [required: >=0.9.0, installed: 0.12.1]",
+                "  - f [required: >=3.0.0, installed: 3.1]",
+                "    - b [required: >=2.1.0, installed: 2.3.1]",
+            ],
+        ),
+    ],
+)
+def test_render_text_given_depth(capsys, unicode, level, expected_output):
+    encoding = "utf-8" if unicode else "ascii"
+    with mock.patch("sys.stdout", MockStdout(encoding)):
+        p.render_text(t, level)
         captured = capsys.readouterr()
         assert "\n".join(expected_output).strip() == captured.out.strip()
 
 
 # Tests for graph outputs
 
 
@@ -772,14 +869,35 @@
 def test_parser_svg():
     parser = p.get_parser()
     args = parser.parse_args(["--graph-output", "svg"])
     assert args.output_format == "svg"
     assert not args.json
 
 
+@pytest.mark.parametrize(
+    ("should_be_error", "depth_arg", "expected_value"),
+    [
+        (True, ["-d", "-1"], None),
+        (True, ["--depth", "string"], None),
+        (False, ["-d", "0"], 0),
+        (False, ["--depth", "8"], 8),
+        (False, [], float("inf")),
+    ],
+)
+def test_parser_depth(should_be_error, depth_arg, expected_value):
+    parser = p.get_parser()
+
+    if should_be_error:
+        with pytest.raises(SystemExit):
+            parser.parse_args(depth_arg)
+    else:
+        args = parser.parse_args(depth_arg)
+        assert args.depth == expected_value
+
+
 @pytest.mark.parametrize("args_joined", [True, False])
 def test_custom_interpreter(tmp_path, monkeypatch, capfd, args_joined):
     result = virtualenv.cli_run([str(tmp_path), "--activators", ""])
     cmd = [sys.executable]
     cmd += [f"--python={result.creator.exe}"] if args_joined else ["--python", str(result.creator.exe)]
     monkeypatch.setattr(sys, "argv", cmd)
     p.main()
```

### Comparing `pipdeptree-2.8.0/LICENSE` & `pipdeptree-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.8.0/README.md` & `pipdeptree-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.8.0/pyproject.toml` & `pipdeptree-2.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.8.0/PKG-INFO` & `pipdeptree-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipdeptree
-Version: 2.8.0
+Version: 2.9.0
 Summary: Command line utility to show dependency tree of packages.
 Project-URL: Changelog, https://github.com/tox-dev/pipdeptree/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/tox-dev/pipdeptree/blob/main/README.md#pipdeptree
 Project-URL: Homepage, https://github.com/tox-dev/pipdeptree
 Project-URL: Source, https://github.com/tox-dev/pipdeptree
 Project-URL: Tracker, https://github.com/tox-dev/pipdeptree/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Vineet Naik <naikvin@gmail.com>
```

