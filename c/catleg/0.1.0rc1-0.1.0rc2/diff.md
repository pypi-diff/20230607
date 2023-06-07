# Comparing `tmp/catleg-0.1.0rc1.tar.gz` & `tmp/catleg-0.1.0rc2.tar.gz`

## Comparing `catleg-0.1.0rc1.tar` & `catleg-0.1.0rc2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/_version.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/tox.ini
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/.github/dependabot.yml
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/.github/workflows/check.yml
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/.github/workflows/publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/src/catleg/__init__.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/src/catleg/catleg.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/src/catleg/cli_util.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/src/catleg/config.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/src/catleg/find_changes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/src/catleg/git_diff.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/src/catleg/law_text_fr.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/src/catleg/parse_catala_markdown.py
--rw-r--r--   0        0        0     6402 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/src/catleg/query.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/src/catleg/skeleton.py
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/src/catleg/markdown_it/heading_extension.py
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/tests/test_catala_parsing.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/tests/test_legifrance_queries.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/README.md
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0    15391 2020-02-02 00:00:00.000000 catleg-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.catleg.toml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/_version.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/tox.ini
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.github/dependabot.yml
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.github/workflows/check.yml
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/catleg.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/cli_util.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/config.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/find_changes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/git_diff.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/law_text_fr.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/parse_catala_markdown.py
+-rw-r--r--   0        0        0     6402 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/query.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/skeleton.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/markdown_it/heading_extension.py
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/tests/test_catala_parsing.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/tests/test_legifrance_queries.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/LICENSE
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/README.md
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    14956 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/PKG-INFO
```

### Comparing `catleg-0.1.0rc1/tox.ini` & `catleg-0.1.0rc2/tox.ini`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/.github/dependabot.yml` & `catleg-0.1.0rc2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/.github/workflows/check.yml` & `catleg-0.1.0rc2/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/.github/workflows/publish.yml` & `catleg-0.1.0rc2/.github/workflows/publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         env:
           PYTEST_ADDOPTS: "-vv --durations=10"
 
   deploy:
     runs-on: ubuntu-latest
     needs: [test]
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.11'
     - name: Install dependencies
       run: |
         pip install hatch
```

### Comparing `catleg-0.1.0rc1/src/catleg/catleg.py` & `catleg-0.1.0rc2/src/catleg/catleg.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/src/catleg/find_changes.py` & `catleg-0.1.0rc2/src/catleg/find_changes.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/src/catleg/git_diff.py` & `catleg-0.1.0rc2/src/catleg/git_diff.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/src/catleg/law_text_fr.py` & `catleg-0.1.0rc2/src/catleg/law_text_fr.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/src/catleg/parse_catala_markdown.py` & `catleg-0.1.0rc2/src/catleg/parse_catala_markdown.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/src/catleg/query.py` & `catleg-0.1.0rc2/src/catleg/query.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/src/catleg/skeleton.py` & `catleg-0.1.0rc2/src/catleg/skeleton.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/src/catleg/markdown_it/heading_extension.py` & `catleg-0.1.0rc2/src/catleg/markdown_it/heading_extension.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/tests/test_catala_parsing.py` & `catleg-0.1.0rc2/tests/test_catala_parsing.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/tests/test_legifrance_queries.py` & `catleg-0.1.0rc2/tests/test_legifrance_queries.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/LICENSE` & `catleg-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc1/pyproject.toml` & `catleg-0.1.0rc2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "_version.py"
 
 [project]
 name = "catleg"
+description = "A library of helper tools for catala programming in the context of French legislative texts."
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
@@ -21,15 +22,15 @@
 dependencies = [
   "aiometer",
   "dynaconf",
   "httpx",
   "markdown-it-py[plugins]",
   "mdformat>=0.7.16",
   "more-itertools",
-  "typer",
+  "typer[all]",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "mypy",
   "pre-commit",
```

### Comparing `catleg-0.1.0rc1/PKG-INFO` & `catleg-0.1.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: catleg
-Version: 0.1.0rc1
+Version: 0.1.0rc2
+Summary: A library of helper tools for catala programming in the context of French legislative texts.
 Project-URL: Homepage, https://github.com/CatalaLang/catleg/
 Project-URL: Bug Tracker, https://github.com/CatalaLang/catleg/issues
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -211,15 +212,15 @@
 Requires-Python: >=3.10
 Requires-Dist: aiometer
 Requires-Dist: dynaconf
 Requires-Dist: httpx
 Requires-Dist: markdown-it-py[plugins]
 Requires-Dist: mdformat>=0.7.16
 Requires-Dist: more-itertools
-Requires-Dist: typer
+Requires-Dist: typer[all]
 Provides-Extra: dev
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: tox; extra == 'dev'
 Description-Content-Type: text/markdown
@@ -227,15 +228,29 @@
 # catleg
 
 A library of helper tools for [catala](https://catala-lang.org) programming in the context
 of French legislative texts.
 
 ## Installing
 
-`catleg` is not released on PyPI yet ; install it by running `pip install -e .` from a source clone.
+`catleg` requires python >= 3.10
+
+### from PyPI
+
+`pip install catleg`
+
+### from a source clone
+
+`pip install .`
+
+### from github
+
+`pip install 'catleg @ git+https://github.com/CatalaLang/catleg@main'`
+
+You may replace `main` with any ref (commit SHA, tag, branch...)
 
 ## Running `catleg`
 
 Run `catleg --help` for a list of commands.
 
 ### Legifrance credentials
 
@@ -248,29 +263,7 @@
 
 ```toml
 lf_client_id = "your_client_id"
 lf_client_secret = "your_client_secret"
 ```
 
 Alternatively, you may define the environment variables `CATLEG_LF_CLIENT_ID` and `CATLEG_LF_CLIENT_SECRET`.
-
-## Development install
-
-Run `pip install -e .[dev]` for a local, editable install that includes development dependencies.
-
-`catleg` uses [tox](https://tox.wiki/en/latest/) to run linters and unit tests in various environments.
-
-Run `tox` to execute tests and linters.
-
-Formatting and import ordering is done by [µFmt](https://ufmt.omnilib.dev/en/stable/index.html) which is basically black + µsort.
-
-### Pre-commit hook
-
-To ensure code is always formatted before a commit, you can use the supplied [pre-commit](https://pre-commit.com) hook.
-
-Run this once:
-
-`pre-commit install`
-
-Then, before every commit, the code will be reformatted automatically.
-
-The pre-commit hook will also run the `ruff` linter.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

