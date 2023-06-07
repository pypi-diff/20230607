# Comparing `tmp/repo_review-0.7.0b7.tar.gz` & `tmp/repo_review-0.7.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jun  7 18:15:21 2023, max compression
+gzip compressed data, last modified: Wed Jun  7 21:09:14 2023, max compression
```

## Comparing `repo_review-0.7.0b7.tar` & `repo_review-0.7.0b8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      125 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.gitattributes
--rw-r--r--   0        0        0     2061 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      187 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      399 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.readthedocs.yml
--rw-r--r--   0        0        0     1194 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/action.yml
--rw-r--r--   0        0        0     2291 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/noxfile.py
--rw-r--r--   0        0        0      359 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2544 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.github/matchers/pylint.json
--rw-r--r--   0        0        0      669 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1856 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/.nojekyll
--rw-r--r--   0        0        0     4826 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/checks.md
--rw-r--r--   0        0        0      978 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/cli.md
--rw-r--r--   0        0        0      590 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/conf.py
--rw-r--r--   0        0        0     1236 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/families.md
--rw-r--r--   0        0        0     2023 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/fixtures.md
--rw-r--r--   0        0        0     1917 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/index.html
--rw-r--r--   0        0        0      172 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/index.md
--rw-r--r--   0        0        0     2239 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/intro.md
--rw-r--r--   0        0        0     2412 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/plugins.md
--rw-r--r--   0        0        0    10238 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/webapp.js
--rw-r--r--   0        0        0     1770 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/docs/webapp.md
--rw-r--r--   0        0        0      243 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/__init__.py
--rw-r--r--   0        0        0     6279 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/__main__.py
--rw-r--r--   0        0        0      162 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_version.pyi
--rw-r--r--   0        0        0     1311 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/checks.py
--rw-r--r--   0        0        0      494 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/families.py
--rw-r--r--   0        0        0     2004 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     3412 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     2176 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/html.py
--rw-r--r--   0        0        0     5156 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0      246 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/typing.py
--rw-r--r--   0        0        0        0 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     4393 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_checks.py
--rw-r--r--   0        0        0      645 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_cmd.py
--rw-r--r--   0        0        0     2460 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_package.py
--rw-r--r--   0        0        0     2185 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_self.py
--rw-r--r--   0        0        0     3981 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_utilities/pyproject.py
--rw-r--r--   0        0        0      333 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/tests/test_utilities/pyproject.toml
--rw-r--r--   0        0        0     2086 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/.gitignore
--rw-r--r--   0        0        0     1525 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/LICENSE
--rw-r--r--   0        0        0     5552 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/README.md
--rw-r--r--   0        0        0     5054 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/pyproject.toml
--rw-r--r--   0        0        0     7653 2023-06-07 18:15:21.000000 repo_review-0.7.0b7/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.gitattributes
+-rw-r--r--   0        0        0     2061 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      187 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      399 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.readthedocs.yml
+-rw-r--r--   0        0        0     1216 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/action.yml
+-rw-r--r--   0        0        0     2291 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/noxfile.py
+-rw-r--r--   0        0        0      359 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2544 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      669 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1856 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/.nojekyll
+-rw-r--r--   0        0        0     4826 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/checks.md
+-rw-r--r--   0        0        0      990 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/cli.md
+-rw-r--r--   0        0        0      590 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/conf.py
+-rw-r--r--   0        0        0     1236 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/families.md
+-rw-r--r--   0        0        0     2023 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/fixtures.md
+-rw-r--r--   0        0        0     1917 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/index.html
+-rw-r--r--   0        0        0      172 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/index.md
+-rw-r--r--   0        0        0     2239 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/intro.md
+-rw-r--r--   0        0        0     2731 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/plugins.md
+-rw-r--r--   0        0        0    10238 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/webapp.js
+-rw-r--r--   0        0        0     1770 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/docs/webapp.md
+-rw-r--r--   0        0        0      243 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     7283 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/__main__.py
+-rw-r--r--   0        0        0      162 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_version.pyi
+-rw-r--r--   0        0        0     1311 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/checks.py
+-rw-r--r--   0        0        0      494 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/families.py
+-rw-r--r--   0        0        0     2004 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     4767 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     2176 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/html.py
+-rw-r--r--   0        0        0     5156 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0      246 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/typing.py
+-rw-r--r--   0        0        0        0 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     4393 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_checks.py
+-rw-r--r--   0        0        0      904 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_cmd.py
+-rw-r--r--   0        0        0     2460 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_fixtures.py
+-rw-r--r--   0        0        0      598 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_package.py
+-rw-r--r--   0        0        0     2185 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_self.py
+-rw-r--r--   0        0        0     3981 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0      333 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2086 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/.gitignore
+-rw-r--r--   0        0        0     1525 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/LICENSE
+-rw-r--r--   0        0        0     5552 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/README.md
+-rw-r--r--   0        0        0     5108 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/pyproject.toml
+-rw-r--r--   0        0        0     7717 2023-06-07 21:09:14.000000 repo_review-0.7.0b8/PKG-INFO
```

### Comparing `repo_review-0.7.0b7/.pre-commit-config.yaml` & `repo_review-0.7.0b8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/action.yml` & `repo_review-0.7.0b8/action.yml`

 * *Files 14% similar despite different names*

```diff
@@ -35,12 +35,13 @@
         pipx install --python '${{ steps.python.outputs.python-path }}' '${{ github.action_path }}[cli]'
         pipx inject repo-review ${{ inputs.plugins }}
 
     - name: Run repo-review
       shell: bash
       run: >
         repo-review .
-        --stderr html
+        --format html
+        --stderr rich
         --select "${{ inputs.select }}"
         --ignore "${{ inputs.ignore }}"
         --package-dir "${{ inputs.package-dir }}"
-        2> $GITHUB_STEP_SUMMARY
+        >> $GITHUB_STEP_SUMMARY
```

### Comparing `repo_review-0.7.0b7/noxfile.py` & `repo_review-0.7.0b8/noxfile.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/.github/CONTRIBUTING.md` & `repo_review-0.7.0b8/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/.github/matchers/pylint.json` & `repo_review-0.7.0b8/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/.github/workflows/cd.yml` & `repo_review-0.7.0b8/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/.github/workflows/ci.yml` & `repo_review-0.7.0b8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/docs/checks.md` & `repo_review-0.7.0b8/docs/checks.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/docs/cli.md` & `repo_review-0.7.0b8/docs/cli.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 ```
 
 There are four output formats; `rich` produces great terminal output, `svg`
 produces an SVG based on the rich output, `html` produces a custom HTML report,
 and `json` produces a output that can be processed easily. To make it easier to
 support tools like GitHub Actions, there is also a `--stderr FORMAT` output
-option that produces the selected format on stderr as well, and avoids producing
-terminal escape codes, even if `FORCE_COLOR` is set.
+option that produces the selected format on stderr as well, and disables
+producing terminal escape codes on stdout, even if `FORCE_COLOR` is set.
 
 JSON output looks like this:
 
 ```json
 {
   "families": {
     "pyproject": {},
```

### Comparing `repo_review-0.7.0b7/docs/conf.py` & `repo_review-0.7.0b8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/docs/families.md` & `repo_review-0.7.0b8/docs/families.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/docs/fixtures.md` & `repo_review-0.7.0b8/docs/fixtures.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/docs/index.html` & `repo_review-0.7.0b8/docs/index.html`

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
-          deps={["sp_repo_review==2023.06.01", "repo-review==0.7.0b6"]}
+          deps={["sp_repo_review==2023.06.01", "repo-review==0.7.0b7"]}
         />,
       );
     </script>
   </body>
 </html>
```

### Comparing `repo_review-0.7.0b7/docs/intro.md` & `repo_review-0.7.0b8/docs/intro.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/docs/plugins.md` & `repo_review-0.7.0b8/docs/plugins.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 You can also add new [](fixtures), and customize [](families) with sorting and
 nicer display names. When writing a plugin, you should also do a few things
 when setting up the package. These suggestions assume you are using a
 standardized backend, such as `hatchling`, `flit-core`, `pdm-backend`, or
 `setuptools>=61`. If you are using some other build backend, please adjust
 accordingly.
 
+## Avoiding CLI requirements on WebAssembly usage
+
+Repo-review uses `repo-review[cli]` to keep CLI requirements from being
+included in the base package, and plugins can follow this if they want to be
+used directly:
+
+```toml
+[project.optional-dependencies]
+cli = [
+  "repo-review[cli]",
+]
+```
+
 ## Custom entry-point (optional)
 
 If you want to provide your own CLI name, you can
 add this to your `pyproject.toml`:
 
 ```toml
 [project.scripts]
@@ -48,15 +61,15 @@
 ```
 
 You can also narrow down the `files` / `types_or` if your plugin only supports
 a subset of files (which most should).
 
 ## GitHub Actions support
 
-You can add an `actions.yml` file similar to this to natively support GitHub
+You can add an `action.yml` file similar to this to natively support GitHub
 Actions & dependabot:
 
 ```yaml
 name: repo-review
 description: "Runs repo-review"
 inputs:
   package-dir:
@@ -74,15 +87,16 @@
         update-environment: false
 
     - name: Run repo-review
       shell: bash
       run: >
         pipx run
         --python '${{ steps.python.outputs.python-path }}'
-        --spec '${{ github.action_path }}'
+        --spec '${{ github.action_path }}[cli]'
         repo-review .
-        --stderr html
+        --format html
+        --stderr rich
         --select "${{ inputs.select }}"
         --ignore "${{ inputs.ignore }}"
         --package-dir "${{ inputs.package-dir }}"
-        2> $GITHUB_STEP_SUMMARY
+        >> $GITHUB_STEP_SUMMARY
 ```
```

### Comparing `repo_review-0.7.0b7/docs/webapp.js` & `repo_review-0.7.0b8/docs/webapp.js`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/docs/webapp.md` & `repo_review-0.7.0b8/docs/webapp.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/src/repo_review/__main__.py` & `repo_review-0.7.0b8/src/repo_review/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,55 +17,80 @@
 import rich.markdown
 import rich.syntax
 import rich.terminal_theme
 import rich.text
 import rich.traceback
 import rich.tree
 
+from . import __version__
 from ._compat.importlib.resources.abc import Traversable
 from ._compat.typing import assert_never
 from .families import Family
-from .ghpath import GHPath
+from .ghpath import EmptyTraversable, GHPath
 from .html import to_html
 from .processor import Result, _collect_all, as_simple_dict, process
 
+__all__ = ["main"]
+
+
+def __dir__() -> list[str]:
+    return __all__
+
+
 rich.traceback.install(suppress=[click, rich], show_locals=True, width=None)
 
 
+def list_all(ctx: click.Context, _param: click.Parameter, value: bool) -> None:
+    if not value or ctx.resilient_parsing:
+        return
+
+    _, checks, families = _collect_all(EmptyTraversable())
+    if len(checks) == 0:
+        msg = "No checks registered. Please install a repo-review plugin."
+        raise click.ClickException(msg)
+
+    for family, grp in itertools.groupby(checks.items(), key=lambda x: x[1].family):
+        rich.print(f'  [dim]# {families[family].get("name", family)}')
+        for code, check in grp:
+            rich.print(f'  "{code}",  [dim]# {check.__doc__}')
+    ctx.exit()
+
+
 def rich_printer(
     families: Mapping[str, Family],
     processed: list[Result],
     *,
     svg: bool = False,
     stderr: bool = False,
+    color: bool = True,
 ) -> None:
     console = rich.console.Console(
-        record=svg, quiet=svg, stderr=stderr, color_system=None if stderr else "auto"
+        record=svg, quiet=svg, stderr=stderr, color_system="auto" if color else None
     )
 
     for family, results_list in itertools.groupby(processed, lambda r: r.family):
         family_name = families[family].get("name", family)
         tree = rich.tree.Tree(f"[bold]{family_name}[/bold]:")
         for result in results_list:
-            color = (
+            style = (
                 "yellow"
                 if result.result is None
                 else "green"
                 if result.result
                 else "red"
             )
             description = (
                 f"[link={result.url}]{result.description}[/link]"
                 if result.url
                 else result.description
             )
             msg = rich.text.Text()
             msg.append(result.name, style="bold")
             msg.append(" ")
-            msg.append(rich.text.Text.from_markup(description, style=color))
+            msg.append(rich.text.Text.from_markup(description, style=style))
             if result.result is None:
                 msg.append(" [skipped]", style="yellow bold")
                 tree.add(msg)
             elif result.result:
                 msg.append(rich.text.Text.from_markup(" :white_check_mark:"))
                 tree.add(msg)
             else:
@@ -78,61 +103,72 @@
         console.print()
 
     if len(processed) == 0:
         console.print("[bold red]No checks ran")
 
     if svg:
         str = console.export_svg(theme=rich.terminal_theme.DEFAULT_TERMINAL_THEME)
-        if stderr:
-            print(str, file=sys.stderr)
+        if color:
+            rich.print(
+                rich.syntax.Syntax(str, lexer="xml"),
+                file=sys.stderr if stderr else sys.stdout,
+            )
         else:
-            rich.print(rich.syntax.Syntax(str, lexer="xml"))
+            print(str, file=sys.stderr if stderr else sys.stdout)
 
 
 def display_output(
     families: Mapping[str, Family],
     processed: list[Result],
     *,
     format_opt: Literal["rich", "json", "html", "svg"],
     stderr: bool,
+    color: bool,
 ) -> None:
     match format_opt:
         case "rich" | "svg":
-            rich_printer(families, processed, svg=format_opt == "svg", stderr=stderr)
+            rich_printer(
+                families, processed, svg=format_opt == "svg", stderr=stderr, color=color
+            )
         case "json":
             j = json.dumps(
                 {"families": families, "checks": as_simple_dict(processed)}, indent=2
             )
-            if stderr:
-                print(j, file=sys.stderr)
-            else:
-                rich.print_json(j)
+            console = rich.console.Console(
+                stderr=stderr, color_system="auto" if color else None
+            )
+            console.print_json(j)
         case "html":
             html = to_html(families, processed)
-            if stderr:
-                print(html, file=sys.stderr)
+            if color:
+                rich.print(
+                    rich.syntax.Syntax(html, lexer="html"),
+                    file=sys.stderr if stderr else sys.stdout,
+                )
             else:
-                rich.print(rich.syntax.Syntax(html, lexer="html"))
+                print(html, file=sys.stderr if stderr else sys.stdout)
         case _:
             assert_never(format_opt)
 
 
 @click.command(context_settings={"help_option_names": ["-h", "--help"]})
+@click.version_option(version=__version__)
 @click.argument("package", type=click.Path(dir_okay=True, path_type=Path))
 @click.option(
     "--format",
     "format_opt",
     type=click.Choice(["rich", "json", "html", "svg"]),
     default="rich",
     help="Select output format.",
 )
 @click.option(
     "--stderr",
+    "stderr_fmt",
     type=click.Choice(["rich", "json", "html", "svg"]),
-    help="Select additional output format for stderr. Will not use terminal escape codes.",
+    help="Select additional output format for stderr. Will disable terminal escape codes for stdout for easy redirection.",
 )
 @click.option(
     "--select",
     help="Only run certain checks, comma separated. All checks run if empty.",
     default="",
 )
 @click.option(
@@ -143,63 +179,64 @@
 @click.option(
     "--package-dir",
     "-p",
     help="Path to python package.",
     default="",
 )
 @click.option(
-    "--list/--no-list",
-    "list_opt",
+    "--list-all",
+    is_flag=True,
+    callback=list_all,
+    expose_value=False,
+    is_eager=True,
     help="List all checks and exit",
-    default=False,
 )
 def main(
     package: Traversable,
     format_opt: Literal["rich", "json", "html"],
-    stderr: Literal["rich", "json", "html"] | None,
+    stderr_fmt: Literal["rich", "json", "html"] | None,
     select: str,
     ignore: str,
     package_dir: str,
-    list_opt: bool,
 ) -> None:
     """
     Pass in a local Path or gh:org/repo@branch.
     """
     ignore_list = {x.strip() for x in ignore.split(",") if x}
     select_list = {x.strip() for x in select.split(",") if x}
 
-    _, checks, families = _collect_all(package, subdir=package_dir)
+    _, checks, _ = _collect_all(package, subdir=package_dir)
     if len(checks) == 0:
         msg = "No checks registered. Please install a repo-review plugin."
         raise click.ClickException(msg)
 
-    if list_opt:
-        for family, grp in itertools.groupby(checks.items(), key=lambda x: x[1].family):
-            rich.print(f'  [dim]# {families[family].get("name", family)}')
-            for code, check in grp:
-                rich.print(f'  "{code}",  [dim]# {check.__doc__}')
-
-        raise SystemExit(0)
-
     if str(package).startswith("gh:"):
         _, org_repo_branch, *p = str(package).split(":", maxsplit=2)
         org_repo, branch = org_repo_branch.split("@", maxsplit=1)
         package = GHPath(repo=org_repo, branch=branch, path=p[0] if p else "")
         if format_opt == "rich":
             rich.print(f"[bold]Processing [blue]{package}[/blue] from GitHub\n")
 
     families, processed = process(
         package, select=select_list, ignore=ignore_list, subdir=package_dir
     )
 
-    display_output(families, processed, format_opt=format_opt, stderr=False)
-    if stderr:
-        display_output(families, processed, format_opt=stderr, stderr=True)
+    display_output(
+        families,
+        processed,
+        format_opt=format_opt,
+        stderr=False,
+        color=stderr_fmt is None,
+    )
+    if stderr_fmt:
+        display_output(
+            families, processed, format_opt=stderr_fmt, stderr=True, color=True
+        )
 
     if any(p.result is False for p in processed):
         raise SystemExit(2)
     if len(processed) == 0:
-        raise SystemExit(2)
+        raise SystemExit(3)
 
 
 if __name__ == "__main__":
     main()  # pylint: disable=no-value-for-parameter
```

### Comparing `repo_review-0.7.0b7/src/repo_review/checks.py` & `repo_review-0.7.0b8/src/repo_review/checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/src/repo_review/fixtures.py` & `repo_review-0.7.0b8/src/repo_review/fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/src/repo_review/ghpath.py` & `repo_review-0.7.0b8/src/repo_review/ghpath.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # pylint: disable=arguments-differ
+# pylint: disable=unused-argument
+# ruff: noqa: ARG002
 
 from __future__ import annotations
 
 import dataclasses
 import io
 import json
 import typing
 from collections.abc import Iterator
 from typing import Literal
 
 from ._compat.importlib.resources.abc import Traversable
 
-__all__ = ["GHPath"]
+__all__ = ["GHPath", "EmptyTraversable"]
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
@@ -103,7 +105,54 @@
         return self.path in {d["path"] for d in self._info if d["type"] == "blob"}
 
     def read_text(self, encoding: str | None = "utf-8") -> str:
         return self.open("r", encoding=encoding).read()
 
     def read_bytes(self) -> bytes:
         return self.open("rb").read()
+
+
+@dataclasses.dataclass(frozen=True, kw_only=True)
+class EmptyTraversable(Traversable):
+    is_a_dir: bool = True
+    _fake_name: str = "not-a-real-path"
+
+    def __str__(self) -> str:
+        return self._fake_name
+
+    @property
+    def name(self) -> str:
+        return self._fake_name
+
+    @typing.overload  # type: ignore[override]
+    def open(self, mode: Literal["r"], encoding: str | None = ...) -> io.StringIO:
+        ...
+
+    @typing.overload
+    def open(self, mode: Literal["rb"]) -> io.BytesIO:
+        ...
+
+    def open(
+        self, mode: Literal["r", "rb"] = "r", encoding: str | None = "utf-8"
+    ) -> io.IOBase:
+        raise FileNotFoundError(self._fake_name)
+
+    def joinpath(self, child: str) -> EmptyTraversable:
+        return self.__class__(is_a_dir=False)
+
+    def __truediv__(self, child: str) -> EmptyTraversable:
+        return self.__class__(is_a_dir=False)
+
+    def iterdir(self) -> Iterator[EmptyTraversable]:
+        yield from ()
+
+    def is_dir(self) -> bool:
+        return self.is_a_dir
+
+    def is_file(self) -> bool:
+        return False
+
+    def read_text(self, encoding: str | None = "utf-8") -> str:
+        raise FileNotFoundError(self._fake_name)
+
+    def read_bytes(self) -> bytes:
+        raise FileNotFoundError(self._fake_name)
```

### Comparing `repo_review-0.7.0b7/src/repo_review/html.py` & `repo_review-0.7.0b8/src/repo_review/html.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/src/repo_review/processor.py` & `repo_review-0.7.0b8/src/repo_review/processor.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/tests/test_checks.py` & `repo_review-0.7.0b8/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/tests/test_cmd.py` & `repo_review-0.7.0b8/tests/test_cmd.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,26 @@
 pytest.importorskip("sp_repo_review")
 
 
 def test_cmd_help():
     subprocess.run(["repo-review", "--help"], check=True)
 
 
+def test_cmd_help_short():
+    subprocess.run(["repo-review", "-h"], check=True)
+
+
+def test_cmd_version():
+    subprocess.run(["repo-review", "--version"], check=True)
+
+
+def test_cmd_list_all():
+    subprocess.run(["repo-review", "--list-all"], check=True)
+
+
 def test_cmd_basic():
     subprocess.run(["repo-review", "."], check=True)
 
 
 def test_cmd_html():
     subprocess.run(
         ["repo-review", ".", "--format", "html", "--stderr", "html"], check=True
```

### Comparing `repo_review-0.7.0b7/tests/test_fixtures.py` & `repo_review-0.7.0b8/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/tests/test_package.py` & `repo_review-0.7.0b8/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/tests/test_self.py` & `repo_review-0.7.0b8/tests/test_self.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/tests/test_utilities/pyproject.py` & `repo_review-0.7.0b8/tests/test_utilities/pyproject.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/.gitignore` & `repo_review-0.7.0b8/.gitignore`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/LICENSE` & `repo_review-0.7.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/README.md` & `repo_review-0.7.0b8/README.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b7/pyproject.toml` & `repo_review-0.7.0b8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -56,18 +56,19 @@
   "sphinx >=4.0",
   "sphinx-copybutton",
   "sphinxcontrib-programoutput",
   "sphinxext-opengraph",
 ]
 
 [project.urls]
-homepage = "https://repo-review.readthedocs.io/"
-source = "https://github.com/scientific-python/repo-review"
-demo = "https://scientific-python.github.io/repo-review"
-changelog = "https://github.com/scientific-python/repo-review/releases"
+Changelog = "https://github.com/scientific-python/repo-review/releases"
+Demo = "https://scientific-python.github.io/repo-review"
+Documentation = "https://repo-review.readthedocs.io/"
+Homepage = "https://repo-review.readthedocs.io/"
+Source = "https://github.com/scientific-python/repo-review"
 
 [project.scripts]
 repo-review = "repo_review.__main__:main"
 
 [project.entry-points."repo_review.fixtures"]
 pyproject = "repo_review.fixtures:pyproject"
```

### Comparing `repo_review-0.7.0b7/PKG-INFO` & `repo_review-0.7.0b8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.7.0b7
+Version: 0.7.0b8
 Summary: Framework that can run checks on repos
-Project-URL: homepage, https://repo-review.readthedocs.io/
-Project-URL: source, https://github.com/scientific-python/repo-review
-Project-URL: demo, https://scientific-python.github.io/repo-review
-Project-URL: changelog, https://github.com/scientific-python/repo-review/releases
+Project-URL: Changelog, https://github.com/scientific-python/repo-review/releases
+Project-URL: Demo, https://scientific-python.github.io/repo-review
+Project-URL: Documentation, https://repo-review.readthedocs.io/
+Project-URL: Homepage, https://repo-review.readthedocs.io/
+Project-URL: Source, https://github.com/scientific-python/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

