# Comparing `tmp/repo_review-0.7.0b6.tar.gz` & `tmp/repo_review-0.7.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jun  7 16:55:51 2023, max compression
+gzip compressed data, last modified: Wed Jun  7 18:15:21 2023, max compression
```

## Comparing `repo_review-0.7.0b6.tar` & `repo_review-0.7.0b7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      125 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.gitattributes
--rw-r--r--   0        0        0     2061 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      187 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      399 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.readthedocs.yml
--rw-r--r--   0        0        0     1194 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/action.yml
--rw-r--r--   0        0        0     2291 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/noxfile.py
--rw-r--r--   0        0        0      359 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2544 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.github/matchers/pylint.json
--rw-r--r--   0        0        0      669 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1856 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/.nojekyll
--rw-r--r--   0        0        0     4777 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/checks.md
--rw-r--r--   0        0        0      978 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/cli.md
--rw-r--r--   0        0        0      277 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/conf.py
--rw-r--r--   0        0        0     1236 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/families.md
--rw-r--r--   0        0        0     2023 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/fixtures.md
--rw-r--r--   0        0        0     1917 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/index.html
--rw-r--r--   0        0        0      172 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/index.md
--rw-r--r--   0        0        0     2239 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/intro.md
--rw-r--r--   0        0        0     2293 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/plugins.md
--rw-r--r--   0        0        0    10238 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/webapp.js
--rw-r--r--   0        0        0     1769 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/docs/webapp.md
--rw-r--r--   0        0        0      243 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/__init__.py
--rw-r--r--   0        0        0     6279 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/__main__.py
--rw-r--r--   0        0        0      162 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/_version.pyi
--rw-r--r--   0        0        0     1311 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/checks.py
--rw-r--r--   0        0        0      494 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/families.py
--rw-r--r--   0        0        0     2004 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     3412 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     2176 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/html.py
--rw-r--r--   0        0        0     5156 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0      246 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/_compat/typing.py
--rw-r--r--   0        0        0        0 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     4393 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/tests/test_checks.py
--rw-r--r--   0        0        0      645 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/tests/test_cmd.py
--rw-r--r--   0        0        0     2460 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/tests/test_package.py
--rw-r--r--   0        0        0     2185 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/tests/test_self.py
--rw-r--r--   0        0        0     3981 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/tests/test_utilities/pyproject.py
--rw-r--r--   0        0        0      333 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/tests/test_utilities/pyproject.toml
--rw-r--r--   0        0        0     2086 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/.gitignore
--rw-r--r--   0        0        0     1525 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/LICENSE
--rw-r--r--   0        0        0     5461 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/README.md
--rw-r--r--   0        0        0     4890 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/pyproject.toml
--rw-r--r--   0        0        0     7324 2023-06-07 16:55:51.000000 repo_review-0.7.0b6/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.gitattributes
+-rw-r--r--   0        0        0     2061 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      187 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      399 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.readthedocs.yml
+-rw-r--r--   0        0        0     1194 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/action.yml
+-rw-r--r--   0        0        0     2291 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/noxfile.py
+-rw-r--r--   0        0        0      359 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2544 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      669 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1856 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/.nojekyll
+-rw-r--r--   0        0        0     4826 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/checks.md
+-rw-r--r--   0        0        0      978 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/cli.md
+-rw-r--r--   0        0        0      590 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/conf.py
+-rw-r--r--   0        0        0     1236 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/families.md
+-rw-r--r--   0        0        0     2023 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/fixtures.md
+-rw-r--r--   0        0        0     1917 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/index.html
+-rw-r--r--   0        0        0      172 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/index.md
+-rw-r--r--   0        0        0     2239 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/intro.md
+-rw-r--r--   0        0        0     2412 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/plugins.md
+-rw-r--r--   0        0        0    10238 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/webapp.js
+-rw-r--r--   0        0        0     1770 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/webapp.md
+-rw-r--r--   0        0        0      243 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     6279 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/__main__.py
+-rw-r--r--   0        0        0      162 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_version.pyi
+-rw-r--r--   0        0        0     1311 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/checks.py
+-rw-r--r--   0        0        0      494 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/families.py
+-rw-r--r--   0        0        0     2004 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     3412 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     2176 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/html.py
+-rw-r--r--   0        0        0     5156 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0      246 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/typing.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     4393 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_checks.py
+-rw-r--r--   0        0        0      645 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_cmd.py
+-rw-r--r--   0        0        0     2460 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_fixtures.py
+-rw-r--r--   0        0        0      598 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_package.py
+-rw-r--r--   0        0        0     2185 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_self.py
+-rw-r--r--   0        0        0     3981 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0      333 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2086 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.gitignore
+-rw-r--r--   0        0        0     1525 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/LICENSE
+-rw-r--r--   0        0        0     5552 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/README.md
+-rw-r--r--   0        0        0     5054 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/pyproject.toml
+-rw-r--r--   0        0        0     7653 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/PKG-INFO
```

### Comparing `repo_review-0.7.0b6/.pre-commit-config.yaml` & `repo_review-0.7.0b7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/action.yml` & `repo_review-0.7.0b7/action.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/noxfile.py` & `repo_review-0.7.0b7/noxfile.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/.github/CONTRIBUTING.md` & `repo_review-0.7.0b7/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/.github/matchers/pylint.json` & `repo_review-0.7.0b7/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/.github/workflows/cd.yml` & `repo_review-0.7.0b7/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/.github/workflows/ci.yml` & `repo_review-0.7.0b7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/docs/checks.md` & `repo_review-0.7.0b7/docs/checks.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,29 @@
     Short description.
     """
 
     family: str
     requires: Set[str] = frozenset()  # Optional
     url: str = ""  # Optional
 
-    def check(self) -> bool | str:
+    def check(self) -> bool | str | None:
         """
         Error message if returns False.
         """
         ...
 ```
 
 You need to implement `family`, which is a string indicating which family it is
 grouped under, and `check()`, which can take [](fixtures), and returns `True` if
 the check passes, or `False` if the check fails. If you want a dynamic error
 explanation instead of the `check()` docstring, you can return a non-empty
-string from the check instead of `False`. Docstrings/error messages can access
-their own object with `{self}` and check name with `{name}` (these are processed
-with `.format`, so escape `{}` as `{{}}`). The error message is in markdown
-format.
+string from the check instead of `False`. Returning `None` makes a check
+"skipped". Docstrings/error messages can access their own object with `{self}`
+and check name with `{name}` (these are processed with `.format`, so escape `{}`
+as `{{}}`). The error message is in markdown format.
 
 If the check named in `requires` does not pass, the check is skipped.
 
 A suggested convention for easily writing checks is as follows:
 
 ```python
 class General:
```

### Comparing `repo_review-0.7.0b6/docs/cli.md` & `repo_review-0.7.0b7/docs/cli.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/docs/families.md` & `repo_review-0.7.0b7/docs/families.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/docs/fixtures.md` & `repo_review-0.7.0b7/docs/fixtures.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/docs/index.html` & `repo_review-0.7.0b7/docs/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -59,13 +59,13 @@
   <body>
     <div id="root">Loading...</div>
     <script type="text/babel">
       const root = ReactDOM.createRoot(document.getElementById("root"));
       root.render(
         <App
           header={true}
-          deps={["sp_repo_review==2023.06.01", "repo-review==0.7.0b5"]}
+          deps={["sp_repo_review==2023.06.01", "repo-review==0.7.0b6"]}
         />,
       );
     </script>
   </body>
 </html>
```

### Comparing `repo_review-0.7.0b6/docs/intro.md` & `repo_review-0.7.0b7/docs/intro.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/docs/plugins.md` & `repo_review-0.7.0b7/docs/plugins.md`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,17 @@
       with:
         python-version: "3.11"
         update-environment: false
 
     - name: Run repo-review
       shell: bash
       run: >
+        pipx run
+        --python '${{ steps.python.outputs.python-path }}'
+        --spec '${{ github.action_path }}'
         repo-review .
         --stderr html
         --select "${{ inputs.select }}"
         --ignore "${{ inputs.ignore }}"
         --package-dir "${{ inputs.package-dir }}"
         2> $GITHUB_STEP_SUMMARY
 ```
```

### Comparing `repo_review-0.7.0b6/docs/webapp.js` & `repo_review-0.7.0b7/docs/webapp.js`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/docs/webapp.md` & `repo_review-0.7.0b7/docs/webapp.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 <https://scientific-python.github.io/repo-review/?repo=scikit-hep/hist&branch=main>.
 On the results screen, you can click on the check numbers to jump to the URLs
 provided by the checks.
 
 This webapp can be embedded into an existing webpage if you set
 `header={false}`. You can set your own deps with `deps = {["...", "..."]}`.
 
-## Custom App
+## Custom app
 
 You can also use the `html` output and write your own webapp. You need to provide Pyodide:
 
 ```html
 <script
   src="https://cdn.jsdelivr.net/pyodide/v0.23.2/full/pyodide.js"
   crossorigin
@@ -48,13 +48,13 @@
   from repo_review.processor import process
   from repo_review.ghpath import GHPath
   from repo_review.html import to_html
 
   GHPath.open_url = staticmethod(open_url)
 
   package = GHPath(repo="${state.repo}", branch="${state.branch}")
-  to_html(process(package))
+  to_html(*process(package))
 `);
 result_html = result_html_py.toString();
 ```
 
 This can throw an error with `KeyError: 'tree'` if the repo or branch is invalid.
```

#### html2text {}

```diff
@@ -4,20 +4,20 @@
 review` and can be seen at
 scientific-python.github.io/repo-review>. The webapp supports selecting org/
 repo and branch via URL, too, such as
 scientific-python.github.io/repo-review/?repo=scikit-hep/hist&branch=main>. On
 the results screen, you can click on the check numbers to jump to the URLs
 provided by the checks. This webapp can be embedded into an existing webpage if
 you set `header={false}`. You can set your own deps with `deps = {["...",
-"..."]}`. ## Custom App You can also use the `html` output and write your own
+"..."]}`. ## Custom app You can also use the `html` output and write your own
 webapp. You need to provide Pyodide: ```html
  ``` Then, you need to load your plugin & repo-review. ```js async function
 prepare_pyodide() { const pyodide = await loadPyodide(); await
 pyodide.loadPackage("micropip"); await pyodide.runPythonAsync(` import micropip
 await micropip.install(["my_plugin", "repo-review"]) `); return pyodide; } ```
 You can get the families and the checks: ```js result_html_py =
 pyodide.runPython(` from pyodide.http import open_url from
 repo_review.processor import process from repo_review.ghpath import GHPath from
 repo_review.html import to_html GHPath.open_url = staticmethod(open_url)
 package = GHPath(repo="${state.repo}", branch="${state.branch}") to_html
-(process(package)) `); result_html = result_html_py.toString(); ``` This can
+(*process(package)) `); result_html = result_html_py.toString(); ``` This can
 throw an error with `KeyError: 'tree'` if the repo or branch is invalid.
```

### Comparing `repo_review-0.7.0b6/src/repo_review/__main__.py` & `repo_review-0.7.0b7/src/repo_review/__main__.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/src/repo_review/checks.py` & `repo_review-0.7.0b7/src/repo_review/checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/src/repo_review/fixtures.py` & `repo_review-0.7.0b7/src/repo_review/fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/src/repo_review/ghpath.py` & `repo_review-0.7.0b7/src/repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/src/repo_review/html.py` & `repo_review-0.7.0b7/src/repo_review/html.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/src/repo_review/processor.py` & `repo_review-0.7.0b7/src/repo_review/processor.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/tests/test_checks.py` & `repo_review-0.7.0b7/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/tests/test_cmd.py` & `repo_review-0.7.0b7/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/tests/test_fixtures.py` & `repo_review-0.7.0b7/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/tests/test_package.py` & `repo_review-0.7.0b7/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/tests/test_self.py` & `repo_review-0.7.0b7/tests/test_self.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/tests/test_utilities/pyproject.py` & `repo_review-0.7.0b7/tests/test_utilities/pyproject.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/.gitignore` & `repo_review-0.7.0b7/.gitignore`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/LICENSE` & `repo_review-0.7.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b6/README.md` & `repo_review-0.7.0b7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # repo-review
 
 [![Actions Status][actions-badge]][actions-link]
-[![Code style: black][black-badge]][black-link]
+[![Documentation Status][docs-badge]][docs-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- SPHINX-START -->
 
 This is a framework for building checks designed to check to see if a
@@ -67,33 +67,33 @@
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
 
 Checks can request fixtures (like pytest) as arguments. Check files can add new
 fixtures as needed. Fixtures are are specified with entry points, and take any
-other fixture as arguments as well - the `package` fixture represents the root
-of the package you are checking, and is the basis for all other fixtures.
-Checks are specified via an entrypoint that returns a dict of checks; this also
-can accept fixtures, allowing dynamic check listings.
+other fixture as arguments as well - the `root` and `package` fixtures
+represents the root of the repository and of the package you are checking,
+respectively, and are the basis for all other fixtures. `pyproject` is provided
+as well. Checks are specified via an entrypoint that returns a dict of checks;
+this also can accept fixtures, allowing dynamic check listings.
 
 Check files do not depend on the main library, and can be extended (similar to
 Flake8). You register new check files via entry-points - so extending this is
 with custom checks or custom fixtures is easy and trivial. There's no need to
 subclass or do anything with the base library - no dependency required.
 
 Checks are as simple as possible so they are easy to write. A check is a class
 with the name (1-2 letters + number) and a docstring (the check message). It
 should define a set of `requires` with any checks it depends on (by name), and
 have a check classmethod. The docstring of this method is the failure message,
-and supports substitution. Arguments to this method are fixtures, and `package`
-is the built-in one providing the package directory as a Traversable. Any other
-fixtures are available by name. A new fixture is given the package Traversable,
-and can produce anything; fixtures are topologically sorted, pre-computed and
-cached.
+and supports substitution. Arguments to this method are fixtures, and `root` or
+`package` are built-in providing a Traversable. Any other fixtures are available
+by name. A new fixture can use any other fixtures, and can produce anything;
+fixtures are topologically sorted, pre-computed and cached.
 
 The runner will topologically sort the checks, and checks that do not run will
 get a `None` result and the check method will not run. The front-end (Rich
 powered CLI or Pyodide webapp) will render the markdown-formatted check
 docstring only if the result is `False`.
 
 ## Links
@@ -104,15 +104,15 @@
 This project inspired [abSENSE](https://princetonuniversity.github.io/abSENSE/), an
 web interface to abSENSE.
 
 This was developed for [Scikit-HEP][] before moving to Scientific-Python.
 
 [actions-badge]: https://github.com/scientific-python/repo-review/workflows/CI/badge.svg
 [actions-link]: https://github.com/scientific-python/repo-review/actions
-[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]: https://github.com/psf/black
 [pypi-link]: https://pypi.org/project/repo-review/
 [pypi-platforms]: https://img.shields.io/pypi/pyversions/repo-review
 [pypi-version]: https://badge.fury.io/py/repo-review.svg
+[docs-badge]: https://readthedocs.org/projects/repo-review/badge/?version=latest
+[docs-link]: https://repo-review.readthedocs.io/en/latest/?badge=latest
 [scientific-python development guide]: https://learn.scientific-python.org/development
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
 [scikit-hep]: https://scikit-hep.org
```

### Comparing `repo_review-0.7.0b6/pyproject.toml` & `repo_review-0.7.0b7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -46,24 +46,28 @@
   "pytest >=7",
   "sp-repo-review",
 ]
 dev = [
   "repo-review[test,cli]",
 ]
 docs = [
-  "repo-review[cli]",
   "furo",
   "myst_parser >=0.13",
+  "repo-review[cli]",
   "sphinx >=4.0",
+  "sphinx-copybutton",
   "sphinxcontrib-programoutput",
+  "sphinxext-opengraph",
 ]
 
 [project.urls]
-homepage = "https://github.com/scientific-python/repo-review"
-webpage = "https://scientific-python.github.io/repo-review"
+homepage = "https://repo-review.readthedocs.io/"
+source = "https://github.com/scientific-python/repo-review"
+demo = "https://scientific-python.github.io/repo-review"
+changelog = "https://github.com/scientific-python/repo-review/releases"
 
 [project.scripts]
 repo-review = "repo_review.__main__:main"
 
 [project.entry-points."repo_review.fixtures"]
 pyproject = "repo_review.fixtures:pyproject"
```

### Comparing `repo_review-0.7.0b6/PKG-INFO` & `repo_review-0.7.0b7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.7.0b6
+Version: 0.7.0b7
 Summary: Framework that can run checks on repos
-Project-URL: homepage, https://github.com/scientific-python/repo-review
-Project-URL: webpage, https://scientific-python.github.io/repo-review
+Project-URL: homepage, https://repo-review.readthedocs.io/
+Project-URL: source, https://github.com/scientific-python/repo-review
+Project-URL: demo, https://scientific-python.github.io/repo-review
+Project-URL: changelog, https://github.com/scientific-python/repo-review/releases
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -32,25 +34,27 @@
 Requires-Dist: rich>=12.2; extra == 'cli'
 Provides-Extra: dev
 Requires-Dist: repo-review[cli,test]; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: repo-review[cli]; extra == 'docs'
+Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx>=4.0; extra == 'docs'
 Requires-Dist: sphinxcontrib-programoutput; extra == 'docs'
+Requires-Dist: sphinxext-opengraph; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == 'test'
 Requires-Dist: sp-repo-review; extra == 'test'
 Description-Content-Type: text/markdown
 
 # repo-review
 
 [![Actions Status][actions-badge]][actions-link]
-[![Code style: black][black-badge]][black-link]
+[![Documentation Status][docs-badge]][docs-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- SPHINX-START -->
 
 This is a framework for building checks designed to check to see if a
@@ -112,33 +116,33 @@
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
 
 Checks can request fixtures (like pytest) as arguments. Check files can add new
 fixtures as needed. Fixtures are are specified with entry points, and take any
-other fixture as arguments as well - the `package` fixture represents the root
-of the package you are checking, and is the basis for all other fixtures.
-Checks are specified via an entrypoint that returns a dict of checks; this also
-can accept fixtures, allowing dynamic check listings.
+other fixture as arguments as well - the `root` and `package` fixtures
+represents the root of the repository and of the package you are checking,
+respectively, and are the basis for all other fixtures. `pyproject` is provided
+as well. Checks are specified via an entrypoint that returns a dict of checks;
+this also can accept fixtures, allowing dynamic check listings.
 
 Check files do not depend on the main library, and can be extended (similar to
 Flake8). You register new check files via entry-points - so extending this is
 with custom checks or custom fixtures is easy and trivial. There's no need to
 subclass or do anything with the base library - no dependency required.
 
 Checks are as simple as possible so they are easy to write. A check is a class
 with the name (1-2 letters + number) and a docstring (the check message). It
 should define a set of `requires` with any checks it depends on (by name), and
 have a check classmethod. The docstring of this method is the failure message,
-and supports substitution. Arguments to this method are fixtures, and `package`
-is the built-in one providing the package directory as a Traversable. Any other
-fixtures are available by name. A new fixture is given the package Traversable,
-and can produce anything; fixtures are topologically sorted, pre-computed and
-cached.
+and supports substitution. Arguments to this method are fixtures, and `root` or
+`package` are built-in providing a Traversable. Any other fixtures are available
+by name. A new fixture can use any other fixtures, and can produce anything;
+fixtures are topologically sorted, pre-computed and cached.
 
 The runner will topologically sort the checks, and checks that do not run will
 get a `None` result and the check method will not run. The front-end (Rich
 powered CLI or Pyodide webapp) will render the markdown-formatted check
 docstring only if the result is `False`.
 
 ## Links
@@ -149,15 +153,15 @@
 This project inspired [abSENSE](https://princetonuniversity.github.io/abSENSE/), an
 web interface to abSENSE.
 
 This was developed for [Scikit-HEP][] before moving to Scientific-Python.
 
 [actions-badge]: https://github.com/scientific-python/repo-review/workflows/CI/badge.svg
 [actions-link]: https://github.com/scientific-python/repo-review/actions
-[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]: https://github.com/psf/black
 [pypi-link]: https://pypi.org/project/repo-review/
 [pypi-platforms]: https://img.shields.io/pypi/pyversions/repo-review
 [pypi-version]: https://badge.fury.io/py/repo-review.svg
+[docs-badge]: https://readthedocs.org/projects/repo-review/badge/?version=latest
+[docs-link]: https://repo-review.readthedocs.io/en/latest/?badge=latest
 [scientific-python development guide]: https://learn.scientific-python.org/development
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
 [scikit-hep]: https://scikit-hep.org
```

