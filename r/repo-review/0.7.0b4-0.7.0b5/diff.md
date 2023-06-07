# Comparing `tmp/repo_review-0.7.0b4.tar.gz` & `tmp/repo_review-0.7.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jun  5 21:02:57 2023, max compression
+gzip compressed data, last modified: Tue Jun  6 21:09:59 2023, max compression
```

## Comparing `repo_review-0.7.0b4.tar` & `repo_review-0.7.0b5.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0     2061 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      399 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.readthedocs.yml
--rw-r--r--   0        0        0     2293 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/noxfile.py
--rw-r--r--   0        0        0      359 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2544 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.github/matchers/pylint.json
--rw-r--r--   0        0        0      630 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1524 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/.nojekyll
--rw-r--r--   0        0        0     3355 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/checks.md
--rw-r--r--   0        0        0      694 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/cli.md
--rw-r--r--   0        0        0      277 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/conf.py
--rw-r--r--   0        0        0     1236 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/families.md
--rw-r--r--   0        0        0     2023 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/fixtures.md
--rw-r--r--   0        0        0     1778 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/index.html
--rw-r--r--   0        0        0      151 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/index.md
--rw-r--r--   0        0        0     9739 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/docs/webapp.js
--rw-r--r--   0        0        0      222 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/__init__.py
--rw-r--r--   0        0        0     6945 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/__main__.py
--rw-r--r--   0        0        0     1311 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/checks.py
--rw-r--r--   0        0        0      494 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/families.py
--rw-r--r--   0        0        0     2004 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     3412 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     4739 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     4393 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_checks.py
--rw-r--r--   0        0        0      450 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_cmd.py
--rw-r--r--   0        0        0     2460 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_package.py
--rw-r--r--   0        0        0     1921 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_self.py
--rw-r--r--   0        0        0     3981 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_utilities/pyproject.py
--rw-r--r--   0        0        0      333 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/tests/test_utilities/pyproject.toml
--rw-r--r--   0        0        0     2086 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/.gitignore
--rw-r--r--   0        0        0     1525 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/LICENSE
--rw-r--r--   0        0        0     4667 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/README.md
--rw-r--r--   0        0        0     4520 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/pyproject.toml
--rw-r--r--   0        0        0     7975 2023-06-05 21:02:57.000000 repo_review-0.7.0b4/PKG-INFO
+-rw-r--r--   0        0        0     2061 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      399 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/.readthedocs.yml
+-rw-r--r--   0        0        0     2291 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/noxfile.py
+-rw-r--r--   0        0        0      359 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2544 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      630 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1524 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/docs/.nojekyll
+-rw-r--r--   0        0        0     3355 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/docs/checks.md
+-rw-r--r--   0        0        0      694 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/docs/cli.md
+-rw-r--r--   0        0        0      277 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/docs/conf.py
+-rw-r--r--   0        0        0     1236 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/docs/families.md
+-rw-r--r--   0        0        0     2023 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/docs/fixtures.md
+-rw-r--r--   0        0        0     1917 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/docs/index.html
+-rw-r--r--   0        0        0      158 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/docs/index.md
+-rw-r--r--   0        0        0    10238 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/docs/webapp.js
+-rw-r--r--   0        0        0     1769 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/docs/webapp.md
+-rw-r--r--   0        0        0      222 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     5575 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/__main__.py
+-rw-r--r--   0        0        0     1311 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/checks.py
+-rw-r--r--   0        0        0      494 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/families.py
+-rw-r--r--   0        0        0     2004 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     3412 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     2176 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/html.py
+-rw-r--r--   0        0        0     5156 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     4393 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/tests/test_checks.py
+-rw-r--r--   0        0        0      450 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/tests/test_cmd.py
+-rw-r--r--   0        0        0     2460 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/tests/test_fixtures.py
+-rw-r--r--   0        0        0      598 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/tests/test_package.py
+-rw-r--r--   0        0        0     2185 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/tests/test_self.py
+-rw-r--r--   0        0        0     3981 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0      333 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2086 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/.gitignore
+-rw-r--r--   0        0        0     1525 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/LICENSE
+-rw-r--r--   0        0        0     4773 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/README.md
+-rw-r--r--   0        0        0     4540 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/pyproject.toml
+-rw-r--r--   0        0        0     8128 2023-06-06 21:09:59.000000 repo_review-0.7.0b5/PKG-INFO
```

### Comparing `repo_review-0.7.0b4/.pre-commit-config.yaml` & `repo_review-0.7.0b5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/noxfile.py` & `repo_review-0.7.0b5/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 @nox.session(venv_backend="none")
 def serve(session: nox.Session) -> None:
     """
     Serve the webapp.
     """
 
-    session.cd("webapp")
+    session.cd("docs")
     session.log("Serving on http://localhost:8080")
     session.run("python3", "-m", "http.server", "8080")
 
 
 @nox.session(reuse_venv=True)
 def docs(session: nox.Session) -> None:
     """
```

### Comparing `repo_review-0.7.0b4/.github/CONTRIBUTING.md` & `repo_review-0.7.0b5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/.github/matchers/pylint.json` & `repo_review-0.7.0b5/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/.github/workflows/cd.yml` & `repo_review-0.7.0b5/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/.github/workflows/ci.yml` & `repo_review-0.7.0b5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/docs/checks.md` & `repo_review-0.7.0b5/docs/checks.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/docs/cli.md` & `repo_review-0.7.0b5/docs/cli.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/docs/families.md` & `repo_review-0.7.0b5/docs/families.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/docs/fixtures.md` & `repo_review-0.7.0b5/docs/fixtures.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/docs/index.html` & `repo_review-0.7.0b5/docs/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -19,20 +19,29 @@
       crossorigin
     ></script>
     <script
       src="https://unpkg.com/@mui/material@v5.13.3/umd/material-ui.production.min.js"
       crossorigin
     ></script>
     <!-- Development
-        <script src="https://unpkg.com/react@18/umd/react.development.js" crossorigin></script>
-        <script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js" crossorigin></script>
-        <script src="https://unpkg.com/@mui/material@v5.13.3/umd/material-ui.development.js" crossorigin></script>
-        ->
+    <script
+      src="https://unpkg.com/react@18/umd/react.development.js"
+      crossorigin
+    ></script>
+    <script
+      src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"
+      crossorigin
+    ></script>
+    <script
+      src="https://unpkg.com/@mui/material@v5.13.3/umd/material-ui.development.js"
+      crossorigin
+    ></script>
+    -->
 
-        <!-- Can remove this for a pre-processor -->
+    <!-- Can remove this for a pre-processor -->
     <script
       src="https://unpkg.com/babel-standalone/babel.min.js"
       crossorigin
     ></script>
     <!-- Fonts to support Material Design -->
     <link
       rel="stylesheet"
@@ -47,11 +56,16 @@
     <script type="text/babel" src="webapp.js" data-presets="react"></script>
   </head>
 
   <body>
     <div id="root">Loading...</div>
     <script type="text/babel">
       const root = ReactDOM.createRoot(document.getElementById("root"));
-      root.render(<App header={true} />);
+      root.render(
+        <App
+          header={true}
+          deps={["sp_repo_review==2023.06.01", "repo-review==0.7.0b4"]}
+        />,
+      );
     </script>
   </body>
 </html>
```

### Comparing `repo_review-0.7.0b4/docs/webapp.js` & `repo_review-0.7.0b5/docs/webapp.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -20,30 +20,72 @@
         MaterialUI.Typography variant = "h6"
         component = "div"
         sx = {
             {
                 flexGrow: 1
             }
         } >
-        Scikit - HEP - Repo - Review <
+        Repo - Review <
         /MaterialUI.Typography> <
-        MaterialUI.Button href = "https://scikit-hep.org/developer"
-        color = "inherit" >
-        Developer Guidelines <
-        /MaterialUI.Button> <
-        MaterialUI.Button href = "https://github.com/scikit-hep/repo-review"
+        MaterialUI.Button href = "https://github.com/scientific-python/repo-review"
         color = "inherit" >
         Source <
         /MaterialUI.Button> <
         /MaterialUI.Toolbar> <
         /MaterialUI.AppBar> <
         /MaterialUI.Box>
     );
 }
 
+function IfUrlLink({
+    name,
+    url,
+    color
+}) {
+    if (url) {
+        return ( <
+            MaterialUI.Typography sx = {
+                {
+                    display: "inline"
+                }
+            }
+            component = "span"
+            variant = "body2"
+            color = {
+                color
+            }
+            component = "a"
+            href = {
+                url
+            }
+            target = "_blank" >
+            {
+                name
+            } <
+            /MaterialUI.Typography>
+        );
+    }
+    return ( <
+        MaterialUI.Typography sx = {
+            {
+                display: "inline"
+            }
+        }
+        component = "span"
+        variant = "body2"
+        color = {
+            color
+        } >
+        {
+            name
+        } <
+        /MaterialUI.Typography>
+    );
+}
+
 function Results(props) {
     const output = [];
     for (const key in props.results) {
         const inner_results = props.results[key];
         const results_components = inner_results.map((result) => {
             const text_color =
                 result.state === false ?
@@ -92,28 +134,34 @@
                     " [skipped]"
                 } <
                 /MaterialUI.Typography>
             );
             const msg = ( <
                 React.Fragment >
                 <
-                MaterialUI.Typography sx = {
-                    {
-                        display: "inline"
-                    }
+                IfUrlLink name = {
+                    result.name
+                }
+                url = {
+                    result.url
                 }
-                component = "span"
-                variant = "body2"
                 color = {
                     text_color
-                } >
-                {
-                    result.name + ": "
-                } <
-                /MaterialUI.Typography> <
+                }
+                /> <
+                IfUrlLink name = {
+                    ": "
+                }
+                url = {
+                    ""
+                }
+                color = {
+                    text_color
+                }
+                /> <
                 React.Fragment >
                 <
                 MaterialUI.Typography sx = {
                     {
                         display: "inline"
                     }
                 }
@@ -140,14 +188,17 @@
                 } < /MaterialUI.ListItemIcon> <
                 MaterialUI.ListItemText primary = {
                     msg
                 }
                 secondary = {
                     details
                 }
+                href = {
+                    result.url
+                }
                 /> <
                 /MaterialUI.ListItem>
             );
         });
 
         output.push( <
             li key = {
@@ -181,27 +232,26 @@
             output
         } <
         /MaterialUI.List> <
         /MaterialUI.Box>
     );
 }
 
-async function prepare_pyodide() {
+async function prepare_pyodide(deps) {
+    const deps_str = deps.map((i) => `"${i}"`).join(", ");
     const pyodide = await loadPyodide();
 
     await pyodide.loadPackage("micropip");
     await pyodide.runPythonAsync(`
         import micropip
-        await micropip.install(["scikit_hep_repo_review==0.6.1"])
+        await micropip.install([${deps_str}])
     `);
     return pyodide;
 }
 
-const pyodide_promise = prepare_pyodide();
-
 function MyThemeProvider(props) {
     const prefersDarkMode = MaterialUI.useMediaQuery(
         "(prefers-color-scheme: dark)",
     );
 
     const theme = React.useMemo(
         () =>
@@ -222,22 +272,25 @@
         /MaterialUI.ThemeProvider>
     );
 }
 
 class App extends React.Component {
     constructor(props) {
         super(props);
+        const deps_str = props.deps.map((i) => `"${i}"`).join(", ");
         this.state = {
             results: [],
             repo: urlParams.get("repo") || "",
             branch: urlParams.get("branch") || "",
-            msg: DEFAULT_MSG,
+            msg: `${DEFAULT_MSG} Packages: ${deps_str}`,
             progress: false,
             err_msg: "",
+            url: "",
         };
+        this.pyodide_promise = prepare_pyodide(props.deps);
     }
 
     handleCompute() {
         if (!this.state.repo || !this.state.branch) {
             this.setState({
                 results: [],
                 msg: DEFAULT_MSG
@@ -255,21 +308,21 @@
         window.history.replaceState(null, "", `${baseurl}?${local_params}`);
         this.setState({
             results: [],
             msg: "Running Python via Pyodide",
             progress: true,
         });
         const state = this.state;
-        pyodide_promise.then((pyodide) => {
+        this.pyodide_promise.then((pyodide) => {
             var families_checks;
             try {
                 families_checks = pyodide.runPython(`
             from pyodide.http import open_url
-            from scikit_hep_repo_review.processor import process
-            from scikit_hep_repo_review.ghpath import GHPath
+            from repo_review.processor import process
+            from repo_review.ghpath import GHPath
 
             GHPath.open_url = staticmethod(open_url)
 
             package = GHPath(repo="${state.repo}", branch="${state.branch}")
             process(package)
         `);
             } catch (e) {
@@ -300,23 +353,25 @@
             console.log(families);
             for (const val of results_list) {
                 results[val.family].push({
                     name: val.name.toString(),
                     description: val.description.toString(),
                     state: val.result,
                     err_msg: val.err_markdown().toString(),
+                    url: val.url.toString(),
                 });
             }
 
             this.setState({
                 results: results,
                 families: families,
                 msg: `Results for ${state.repo}@${state.branch}`,
                 progress: false,
                 err_msg: "",
+                url: "",
             });
 
             results_list.destroy();
             families_dict.destroy();
         });
     }
```

### Comparing `repo_review-0.7.0b4/src/repo_review/__main__.py` & `repo_review-0.7.0b5/src/repo_review/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,435 +1,349 @@
 00000000: 6672 6f6d 205f 5f66 7574 7572 655f 5f20  from __future__ 
 00000010: 696d 706f 7274 2061 6e6e 6f74 6174 696f  import annotatio
-00000020: 6e73 0a0a 696d 706f 7274 2062 7569 6c74  ns..import built
-00000030: 696e 730a 696d 706f 7274 2066 756e 6374  ins.import funct
-00000040: 6f6f 6c73 0a69 6d70 6f72 7420 696f 0a69  ools.import io.i
-00000050: 6d70 6f72 7420 6974 6572 746f 6f6c 730a  mport itertools.
-00000060: 696d 706f 7274 206a 736f 6e0a 696d 706f  import json.impo
-00000070: 7274 2074 7970 696e 670a 6672 6f6d 2063  rt typing.from c
-00000080: 6f6c 6c65 6374 696f 6e73 2e61 6263 2069  ollections.abc i
-00000090: 6d70 6f72 7420 4d61 7070 696e 670a 6672  mport Mapping.fr
-000000a0: 6f6d 2070 6174 686c 6962 2069 6d70 6f72  om pathlib impor
-000000b0: 7420 5061 7468 0a66 726f 6d20 7479 7069  t Path.from typi
-000000c0: 6e67 2069 6d70 6f72 7420 4c69 7465 7261  ng import Litera
-000000d0: 6c0a 0a69 6620 7479 7069 6e67 2e54 5950  l..if typing.TYP
-000000e0: 455f 4348 4543 4b49 4e47 3a0a 2020 2020  E_CHECKING:.    
-000000f0: 696d 706f 7274 2063 6c69 636b 0a65 6c73  import click.els
-00000100: 653a 0a20 2020 2069 6d70 6f72 7420 7269  e:.    import ri
-00000110: 6368 5f63 6c69 636b 2061 7320 636c 6963  ch_click as clic
-00000120: 6b0a 0a69 6d70 6f72 7420 6d61 726b 646f  k..import markdo
-00000130: 776e 5f69 740a 696d 706f 7274 2072 6963  wn_it.import ric
-00000140: 682e 636f 6e73 6f6c 650a 696d 706f 7274  h.console.import
-00000150: 2072 6963 682e 6d61 726b 646f 776e 0a69   rich.markdown.i
-00000160: 6d70 6f72 7420 7269 6368 2e74 6572 6d69  mport rich.termi
-00000170: 6e61 6c5f 7468 656d 650a 696d 706f 7274  nal_theme.import
-00000180: 2072 6963 682e 7465 7874 0a69 6d70 6f72   rich.text.impor
-00000190: 7420 7269 6368 2e74 7261 6365 6261 636b  t rich.traceback
-000001a0: 0a69 6d70 6f72 7420 7269 6368 2e74 7265  .import rich.tre
-000001b0: 650a 0a66 726f 6d20 2e5f 636f 6d70 6174  e..from ._compat
-000001c0: 2e69 6d70 6f72 746c 6962 2e72 6573 6f75  .importlib.resou
-000001d0: 7263 6573 2e61 6263 2069 6d70 6f72 7420  rces.abc import 
-000001e0: 5472 6176 6572 7361 626c 650a 6672 6f6d  Traversable.from
-000001f0: 202e 6661 6d69 6c69 6573 2069 6d70 6f72   .families impor
-00000200: 7420 4661 6d69 6c79 0a66 726f 6d20 2e67  t Family.from .g
-00000210: 6870 6174 6820 696d 706f 7274 2047 4850  hpath import GHP
-00000220: 6174 680a 6672 6f6d 202e 7072 6f63 6573  ath.from .proces
-00000230: 736f 7220 696d 706f 7274 2052 6573 756c  sor import Resul
-00000240: 742c 205f 636f 6c6c 6563 745f 616c 6c2c  t, _collect_all,
-00000250: 2061 735f 7369 6d70 6c65 5f64 6963 742c   as_simple_dict,
-00000260: 2070 726f 6365 7373 0a0a 7269 6368 2e74   process..rich.t
-00000270: 7261 6365 6261 636b 2e69 6e73 7461 6c6c  raceback.install
-00000280: 2873 7570 7072 6573 733d 5b63 6c69 636b  (suppress=[click
-00000290: 2c20 7269 6368 5d2c 2073 686f 775f 6c6f  , rich], show_lo
-000002a0: 6361 6c73 3d54 7275 652c 2077 6964 7468  cals=True, width
-000002b0: 3d4e 6f6e 6529 0a0a 2320 5573 6520 6d6f  =None)..# Use mo
-000002c0: 6475 6c65 2d6c 6576 656c 2065 6e74 7279  dule-level entry
-000002d0: 206e 616d 6573 0a23 2072 6570 6f5f 7265   names.# repo_re
-000002e0: 7669 6577 5f66 6978 7475 7265 7320 3d20  view_fixtures = 
-000002f0: 7b22 7079 7072 6f6a 6563 7422 7d0a 2320  {"pyproject"}.# 
-00000300: 7265 706f 5f72 6576 6965 775f 6368 6563  repo_review_chec
-00000310: 6b73 203d 2073 6574 2870 2e5f 5f6e 616d  ks = set(p.__nam
-00000320: 655f 5f5f 2066 6f72 2070 2069 6e20 4765  e___ for p in Ge
-00000330: 6e65 7261 6c2e 5f5f 7375 6263 6c61 7373  neral.__subclass
-00000340: 6573 5f5f 2829 290a 0a0a 6465 6620 7269  es__())...def ri
-00000350: 6368 5f70 7269 6e74 6572 280a 2020 2020  ch_printer(.    
-00000360: 6661 6d69 6c69 6573 3a20 4d61 7070 696e  families: Mappin
-00000370: 675b 7374 722c 2046 616d 696c 795d 2c20  g[str, Family], 
-00000380: 7072 6f63 6573 7365 643a 206c 6973 745b  processed: list[
-00000390: 5265 7375 6c74 5d2c 202a 2c20 6f75 7470  Result], *, outp
-000003a0: 7574 3a20 5061 7468 207c 204e 6f6e 650a  ut: Path | None.
-000003b0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2063  ) -> None:.    c
-000003c0: 6f6e 736f 6c65 203d 2072 6963 682e 636f  onsole = rich.co
-000003d0: 6e73 6f6c 652e 436f 6e73 6f6c 6528 7265  nsole.Console(re
-000003e0: 636f 7264 3d54 7275 6529 0a0a 2020 2020  cord=True)..    
-000003f0: 666f 7220 6661 6d69 6c79 2c20 7265 7375  for family, resu
-00000400: 6c74 735f 6c69 7374 2069 6e20 6974 6572  lts_list in iter
-00000410: 746f 6f6c 732e 6772 6f75 7062 7928 7072  tools.groupby(pr
-00000420: 6f63 6573 7365 642c 206c 616d 6264 6120  ocessed, lambda 
-00000430: 723a 2072 2e66 616d 696c 7929 3a0a 2020  r: r.family):.  
-00000440: 2020 2020 2020 6661 6d69 6c79 5f6e 616d        family_nam
-00000450: 6520 3d20 6661 6d69 6c69 6573 5b66 616d  e = families[fam
-00000460: 696c 795d 2e67 6574 2822 6e61 6d65 222c  ily].get("name",
-00000470: 2066 616d 696c 7929 0a20 2020 2020 2020   family).       
-00000480: 2074 7265 6520 3d20 7269 6368 2e74 7265   tree = rich.tre
-00000490: 652e 5472 6565 2866 225b 626f 6c64 5d7b  e.Tree(f"[bold]{
-000004a0: 6661 6d69 6c79 5f6e 616d 657d 5b2f 626f  family_name}[/bo
-000004b0: 6c64 5d3a 2229 0a20 2020 2020 2020 2066  ld]:").        f
-000004c0: 6f72 2072 6573 756c 7420 696e 2072 6573  or result in res
-000004d0: 756c 7473 5f6c 6973 743a 0a20 2020 2020  ults_list:.     
-000004e0: 2020 2020 2020 2063 6f6c 6f72 203d 2028         color = (
-000004f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000500: 2022 7965 6c6c 6f77 220a 2020 2020 2020   "yellow".      
-00000510: 2020 2020 2020 2020 2020 6966 2072 6573            if res
-00000520: 756c 742e 7265 7375 6c74 2069 7320 4e6f  ult.result is No
-00000530: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-00000540: 2020 2065 6c73 6520 2267 7265 656e 220a     else "green".
-00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000560: 6966 2072 6573 756c 742e 7265 7375 6c74  if result.result
-00000570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000580: 2065 6c73 6520 2272 6564 220a 2020 2020   else "red".    
-00000590: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000005a0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-000005b0: 6e20 3d20 280a 2020 2020 2020 2020 2020  n = (.          
-000005c0: 2020 2020 2020 6622 5b6c 696e 6b3d 7b72        f"[link={r
-000005d0: 6573 756c 742e 7572 6c7d 5d7b 7265 7375  esult.url}]{resu
-000005e0: 6c74 2e64 6573 6372 6970 7469 6f6e 7d5b  lt.description}[
-000005f0: 2f6c 696e 6b5d 220a 2020 2020 2020 2020  /link]".        
-00000600: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
-00000610: 742e 7572 6c0a 2020 2020 2020 2020 2020  t.url.          
-00000620: 2020 2020 2020 656c 7365 2072 6573 756c        else resul
-00000630: 742e 6465 7363 7269 7074 696f 6e0a 2020  t.description.  
-00000640: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00000650: 2020 2020 2020 2020 6d73 6720 3d20 7269          msg = ri
-00000660: 6368 2e74 6578 742e 5465 7874 2829 0a20  ch.text.Text(). 
-00000670: 2020 2020 2020 2020 2020 206d 7367 2e61             msg.a
-00000680: 7070 656e 6428 7265 7375 6c74 2e6e 616d  ppend(result.nam
-00000690: 652c 2073 7479 6c65 3d22 626f 6c64 2229  e, style="bold")
-000006a0: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-000006b0: 2e61 7070 656e 6428 2220 2229 0a20 2020  .append(" ").   
-000006c0: 2020 2020 2020 2020 206d 7367 2e61 7070           msg.app
-000006d0: 656e 6428 7269 6368 2e74 6578 742e 5465  end(rich.text.Te
-000006e0: 7874 2e66 726f 6d5f 6d61 726b 7570 2864  xt.from_markup(d
-000006f0: 6573 6372 6970 7469 6f6e 2c20 7374 796c  escription, styl
-00000700: 653d 636f 6c6f 7229 290a 2020 2020 2020  e=color)).      
-00000710: 2020 2020 2020 6966 2072 6573 756c 742e        if result.
-00000720: 7265 7375 6c74 2069 7320 4e6f 6e65 3a0a  result is None:.
-00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 6d73 672e 6170 7065 6e64 2822 205b 736b  msg.append(" [sk
-00000750: 6970 7065 645d 222c 2073 7479 6c65 3d22  ipped]", style="
-00000760: 7965 6c6c 6f77 2062 6f6c 6422 290a 2020  yellow bold").  
-00000770: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00000780: 6565 2e61 6464 286d 7367 290a 2020 2020  ee.add(msg).    
-00000790: 2020 2020 2020 2020 656c 6966 2072 6573          elif res
-000007a0: 756c 742e 7265 7375 6c74 3a0a 2020 2020  ult.result:.    
-000007b0: 2020 2020 2020 2020 2020 2020 6d73 672e              msg.
-000007c0: 6170 7065 6e64 2872 6963 682e 7465 7874  append(rich.text
-000007d0: 2e54 6578 742e 6672 6f6d 5f6d 6172 6b75  .Text.from_marku
-000007e0: 7028 2220 3a77 6869 7465 5f63 6865 636b  p(" :white_check
-000007f0: 5f6d 6172 6b3a 2229 290a 2020 2020 2020  _mark:")).      
-00000800: 2020 2020 2020 2020 2020 7472 6565 2e61            tree.a
-00000810: 6464 286d 7367 290a 2020 2020 2020 2020  dd(msg).        
-00000820: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00000830: 2020 2020 2020 2020 2020 6d73 672e 6170            msg.ap
-00000840: 7065 6e64 2872 6963 682e 7465 7874 2e54  pend(rich.text.T
-00000850: 6578 742e 6672 6f6d 5f6d 6172 6b75 7028  ext.from_markup(
-00000860: 2220 3a78 3a22 2929 0a20 2020 2020 2020  " :x:")).       
-00000870: 2020 2020 2020 2020 2064 6574 6169 6c20           detail 
-00000880: 3d20 7269 6368 2e6d 6172 6b64 6f77 6e2e  = rich.markdown.
-00000890: 4d61 726b 646f 776e 2872 6573 756c 742e  Markdown(result.
-000008a0: 6572 725f 6d73 6729 0a20 2020 2020 2020  err_msg).       
-000008b0: 2020 2020 2020 2020 206d 7367 5f67 7270           msg_grp
-000008c0: 203d 2072 6963 682e 636f 6e73 6f6c 652e   = rich.console.
-000008d0: 4772 6f75 7028 6d73 672c 2064 6574 6169  Group(msg, detai
-000008e0: 6c29 0a20 2020 2020 2020 2020 2020 2020  l).             
-000008f0: 2020 2074 7265 652e 6164 6428 6d73 675f     tree.add(msg_
-00000900: 6772 7029 0a0a 2020 2020 2020 2020 636f  grp)..        co
-00000910: 6e73 6f6c 652e 7072 696e 7428 7472 6565  nsole.print(tree
-00000920: 290a 2020 2020 2020 2020 636f 6e73 6f6c  ).        consol
-00000930: 652e 7072 696e 7428 290a 0a20 2020 2069  e.print()..    i
-00000940: 6620 6f75 7470 7574 2069 7320 6e6f 7420  f output is not 
-00000950: 4e6f 6e65 3a0a 2020 2020 2020 2020 636f  None:.        co
-00000960: 6e73 6f6c 652e 7361 7665 5f73 7667 2873  nsole.save_svg(s
-00000970: 7472 286f 7574 7075 7429 2c20 7468 656d  tr(output), them
-00000980: 653d 7269 6368 2e74 6572 6d69 6e61 6c5f  e=rich.terminal_
-00000990: 7468 656d 652e 4445 4641 554c 545f 5445  theme.DEFAULT_TE
-000009a0: 524d 494e 414c 5f54 4845 4d45 290a 0a0a  RMINAL_THEME)...
-000009b0: 6465 6620 746f 5f68 746d 6c28 6661 6d69  def to_html(fami
-000009c0: 6c69 6573 3a20 4d61 7070 696e 675b 7374  lies: Mapping[st
-000009d0: 722c 2046 616d 696c 795d 2c20 7072 6f63  r, Family], proc
-000009e0: 6573 7365 643a 206c 6973 745b 5265 7375  essed: list[Resu
-000009f0: 6c74 5d29 202d 3e20 7374 723a 0a20 2020  lt]) -> str:.   
-00000a00: 206f 7574 203d 2069 6f2e 5374 7269 6e67   out = io.String
-00000a10: 494f 2829 0a20 2020 2070 7269 6e74 203d  IO().    print =
-00000a20: 2066 756e 6374 6f6f 6c73 2e70 6172 7469   functools.parti
-00000a30: 616c 2862 7569 6c74 696e 732e 7072 696e  al(builtins.prin
-00000a40: 742c 2066 696c 653d 6f75 7429 0a20 2020  t, file=out).   
-00000a50: 206d 6420 3d20 6d61 726b 646f 776e 5f69   md = markdown_i
-00000a60: 742e 4d61 726b 646f 776e 4974 2829 0a0a  t.MarkdownIt()..
-00000a70: 2020 2020 666f 7220 6661 6d69 6c79 2c20      for family, 
-00000a80: 7265 7375 6c74 735f 6c69 7374 2069 6e20  results_list in 
-00000a90: 6974 6572 746f 6f6c 732e 6772 6f75 7062  itertools.groupb
-00000aa0: 7928 7072 6f63 6573 7365 642c 206c 616d  y(processed, lam
-00000ab0: 6264 6120 723a 2072 2e66 616d 696c 7929  bda r: r.family)
-00000ac0: 3a0a 2020 2020 2020 2020 6661 6d69 6c79  :.        family
-00000ad0: 5f6e 616d 6520 3d20 6661 6d69 6c69 6573  _name = families
-00000ae0: 5b66 616d 696c 795d 2e67 6574 2822 6e61  [family].get("na
-00000af0: 6d65 222c 2066 616d 696c 7929 0a20 2020  me", family).   
-00000b00: 2020 2020 2070 7269 6e74 2866 223c 6832       print(f"<h2
-00000b10: 3e7b 6661 6d69 6c79 5f6e 616d 657d 3c2f  >{family_name}</
-00000b20: 6832 3e22 290a 2020 2020 2020 2020 7072  h2>").        pr
-00000b30: 696e 7428 223c 7461 626c 653e 2229 0a20  int("<table>"). 
-00000b40: 2020 2020 2020 2070 7269 6e74 2822 3c74         print("<t
-00000b50: 723e 3c74 683e 3f3c 2f74 683e 3c74 683e  r><th>?</th><th>
-00000b60: 4e61 6d65 3c2f 7468 3e3c 7468 3e44 6573  Name</th><th>Des
-00000b70: 6372 6970 7469 6f6e 3c2f 7468 3e3c 2f74  cription</th></t
-00000b80: 723e 2229 0a20 2020 2020 2020 2066 6f72  r>").        for
-00000b90: 2072 6573 756c 7420 696e 2072 6573 756c   result in resul
-00000ba0: 7473 5f6c 6973 743a 0a20 2020 2020 2020  ts_list:.       
-00000bb0: 2020 2020 2063 6f6c 6f72 203d 2028 0a20       color = (. 
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000bd0: 6f72 616e 6765 220a 2020 2020 2020 2020  orange".        
-00000be0: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
-00000bf0: 742e 7265 7375 6c74 2069 7320 4e6f 6e65  t.result is None
-00000c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c10: 2065 6c73 6520 2267 7265 656e 220a 2020   else "green".  
-00000c20: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00000c30: 2072 6573 756c 742e 7265 7375 6c74 0a20   result.result. 
-00000c40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00000c50: 6c73 6520 2272 6564 220a 2020 2020 2020  lse "red".      
-00000c60: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00000c70: 2020 2020 6963 6f6e 203d 2022 e29a a0ef      icon = "....
-00000c80: b88f 2220 6966 2072 6573 756c 742e 7265  .." if result.re
-00000c90: 7375 6c74 2069 7320 4e6f 6e65 2065 6c73  sult is None els
-00000ca0: 6520 22e2 9c85 2220 6966 2072 6573 756c  e "..." if resul
-00000cb0: 742e 7265 7375 6c74 2065 6c73 6520 22e2  t.result else ".
-00000cc0: 9d8c 220a 2020 2020 2020 2020 2020 2020  ..".            
-00000cd0: 7265 7375 6c74 5f74 7874 203d 2028 0a20  result_txt = (. 
-00000ce0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000cf0: 536b 6970 7065 6422 0a20 2020 2020 2020  Skipped".       
-00000d00: 2020 2020 2020 2020 2069 6620 7265 7375           if resu
-00000d10: 6c74 2e72 6573 756c 7420 6973 204e 6f6e  lt.result is Non
-00000d20: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00000d30: 2020 656c 7365 2022 5061 7373 6564 220a    else "Passed".
-00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d50: 6966 2072 6573 756c 742e 7265 7375 6c74  if result.result
-00000d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d70: 2065 6c73 6520 2246 6169 6c65 6422 0a20   else "Failed". 
-00000d80: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00000d90: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00000da0: 7469 6f6e 203d 2028 0a20 2020 2020 2020  tion = (.       
-00000db0: 2020 2020 2020 2020 2066 273c 6120 6872           f'<a hr
-00000dc0: 6566 3d22 7b72 6573 756c 742e 7572 6c7d  ef="{result.url}
-00000dd0: 223e 7b72 6573 756c 742e 6465 7363 7269  ">{result.descri
-00000de0: 7074 696f 6e7d 3c2f 613e 270a 2020 2020  ption}</a>'.    
-00000df0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00000e00: 6573 756c 742e 7572 6c0a 2020 2020 2020  esult.url.      
-00000e10: 2020 2020 2020 2020 2020 656c 7365 2072            else r
-00000e20: 6573 756c 742e 6465 7363 7269 7074 696f  esult.descriptio
-00000e30: 6e0a 2020 2020 2020 2020 2020 2020 290a  n.            ).
-00000e40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00000e50: 7428 6627 3c74 7220 7374 796c 653d 2263  t(f'<tr style="c
-00000e60: 6f6c 6f72 3a20 7b63 6f6c 6f72 7d3b 223e  olor: {color};">
-00000e70: 2729 0a20 2020 2020 2020 2020 2020 2070  ').            p
-00000e80: 7269 6e74 2866 273c 7464 3e3c 7370 616e  rint(f'<td><span
-00000e90: 2072 6f6c 653d 2269 6d67 2220 6172 6961   role="img" aria
-00000ea0: 2d6c 6162 656c 3d22 7b72 6573 756c 745f  -label="{result_
-00000eb0: 7478 747d 223e 7b69 636f 6e7d 3c2f 7370  txt}">{icon}</sp
-00000ec0: 616e 3e3c 2f74 643e 2729 0a20 2020 2020  an></td>').     
-00000ed0: 2020 2020 2020 2070 7269 6e74 2866 223c         print(f"<
-00000ee0: 7464 3e7b 7265 7375 6c74 2e6e 616d 657d  td>{result.name}
-00000ef0: 3c2f 7464 3e22 290a 2020 2020 2020 2020  </td>").        
-00000f00: 2020 2020 6966 2072 6573 756c 742e 7265      if result.re
-00000f10: 7375 6c74 2069 7320 4e6f 6e65 206f 7220  sult is None or 
-00000f20: 7265 7375 6c74 2e72 6573 756c 743a 0a20  result.result:. 
-00000f30: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00000f40: 7269 6e74 2866 223c 7464 3e7b 6465 7363  rint(f"<td>{desc
-00000f50: 7269 7074 696f 6e7d 3c2f 7464 3e22 290a  ription}</td>").
-00000f60: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00000f70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000f80: 2020 7072 696e 7428 223c 7464 3e22 290a    print("<td>").
-00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fa0: 7072 696e 7428 6465 7363 7269 7074 696f  print(descriptio
-00000fb0: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-00000fc0: 2020 2070 7269 6e74 2822 3c62 722f 3e22     print("<br/>"
-00000fd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00000fe0: 2020 7072 696e 7428 6d64 2e72 656e 6465    print(md.rende
-00000ff0: 7228 7265 7375 6c74 2e65 7272 5f6d 7367  r(result.err_msg
-00001000: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00001010: 2020 2070 7269 6e74 2822 3c2f 7464 3e22     print("</td>"
-00001020: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00001030: 696e 7428 223c 2f74 723e 2229 0a20 2020  int("</tr>").   
-00001040: 2020 2020 2070 7269 6e74 2822 3c2f 7461       print("</ta
-00001050: 626c 653e 2229 0a0a 2020 2020 6966 206c  ble>")..    if l
-00001060: 656e 2870 726f 6365 7373 6564 2920 3d3d  en(processed) ==
-00001070: 2030 3a0a 2020 2020 2020 2020 7072 696e   0:.        prin
-00001080: 7428 273c 7370 616e 2073 7479 6c65 3d22  t('<span style="
-00001090: 636f 6c6f 723a 2072 6564 3b22 3e4e 6f20  color: red;">No 
-000010a0: 6368 6563 6b73 2072 616e 2e3c 2f73 7061  checks ran.</spa
-000010b0: 6e3e 2729 0a0a 2020 2020 7265 7475 726e  n>')..    return
-000010c0: 206f 7574 2e67 6574 7661 6c75 6528 290a   out.getvalue().
-000010d0: 0a0a 4063 6c69 636b 2e63 6f6d 6d61 6e64  ..@click.command
-000010e0: 2863 6f6e 7465 7874 5f73 6574 7469 6e67  (context_setting
-000010f0: 733d 7b22 6865 6c70 5f6f 7074 696f 6e5f  s={"help_option_
-00001100: 6e61 6d65 7322 3a20 5b22 2d68 222c 2022  names": ["-h", "
-00001110: 2d2d 6865 6c70 225d 7d29 0a40 636c 6963  --help"]}).@clic
-00001120: 6b2e 6172 6775 6d65 6e74 2822 7061 636b  k.argument("pack
-00001130: 6167 6522 2c20 7479 7065 3d63 6c69 636b  age", type=click
-00001140: 2e50 6174 6828 6469 725f 6f6b 6179 3d54  .Path(dir_okay=T
-00001150: 7275 652c 2070 6174 685f 7479 7065 3d50  rue, path_type=P
-00001160: 6174 6829 290a 4063 6c69 636b 2e6f 7074  ath)).@click.opt
-00001170: 696f 6e28 0a20 2020 2022 2d2d 6f75 7470  ion(.    "--outp
-00001180: 7574 222c 0a20 2020 2074 7970 653d 636c  ut",.    type=cl
-00001190: 6963 6b2e 5061 7468 2866 696c 655f 6f6b  ick.Path(file_ok
-000011a0: 6179 3d54 7275 652c 2065 7869 7374 733d  ay=True, exists=
-000011b0: 4661 6c73 652c 2070 6174 685f 7479 7065  False, path_type
-000011c0: 3d50 6174 6829 2c0a 2020 2020 6465 6661  =Path),.    defa
-000011d0: 756c 743d 4e6f 6e65 2c0a 2020 2020 6865  ult=None,.    he
-000011e0: 6c70 3d22 5772 6974 6520 6f75 7420 6669  lp="Write out fi
-000011f0: 6c65 2e20 5772 6974 6573 2053 5647 2069  le. Writes SVG i
-00001200: 6620 666f 726d 6174 2069 7320 7269 6368  f format is rich
-00001210: 2e22 2c0a 290a 4063 6c69 636b 2e6f 7074  .",.).@click.opt
-00001220: 696f 6e28 0a20 2020 2022 2d2d 666f 726d  ion(.    "--form
-00001230: 6174 222c 0a20 2020 2074 7970 653d 636c  at",.    type=cl
-00001240: 6963 6b2e 4368 6f69 6365 285b 2272 6963  ick.Choice(["ric
-00001250: 6822 2c20 226a 736f 6e22 2c20 2268 746d  h", "json", "htm
-00001260: 6c22 5d29 2c0a 2020 2020 6465 6661 756c  l"]),.    defaul
-00001270: 743d 2272 6963 6822 2c0a 2020 2020 6865  t="rich",.    he
-00001280: 6c70 3d22 5365 6c65 6374 206f 7574 7075  lp="Select outpu
-00001290: 7420 666f 726d 6174 2e22 2c0a 290a 4063  t format.",.).@c
-000012a0: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
-000012b0: 2022 2d2d 7365 6c65 6374 222c 0a20 2020   "--select",.   
-000012c0: 2068 656c 703d 224f 6e6c 7920 7275 6e20   help="Only run 
-000012d0: 6365 7274 6169 6e20 6368 6563 6b73 2c20  certain checks, 
-000012e0: 636f 6d6d 6120 7365 7061 7261 7465 642e  comma separated.
-000012f0: 2041 6c6c 2063 6865 636b 7320 7275 6e20   All checks run 
-00001300: 6966 2065 6d70 7479 2e22 2c0a 2020 2020  if empty.",.    
-00001310: 6465 6661 756c 743d 2222 2c0a 290a 4063  default="",.).@c
-00001320: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
-00001330: 2022 2d2d 6967 6e6f 7265 222c 0a20 2020   "--ignore",.   
-00001340: 2068 656c 703d 2249 676e 6f72 6520 6120   help="Ignore a 
-00001350: 6368 6563 6b20 6f72 2063 6865 636b 732c  check or checks,
-00001360: 2063 6f6d 6d61 2073 6570 6172 6174 6564   comma separated
-00001370: 2e22 2c0a 2020 2020 6465 6661 756c 743d  .",.    default=
-00001380: 2222 2c0a 290a 4063 6c69 636b 2e6f 7074  "",.).@click.opt
-00001390: 696f 6e28 0a20 2020 2022 2d2d 7061 636b  ion(.    "--pack
-000013a0: 6167 652d 6469 7222 2c0a 2020 2020 222d  age-dir",.    "-
-000013b0: 7022 2c0a 2020 2020 6865 6c70 3d22 5061  p",.    help="Pa
-000013c0: 7468 2074 6f20 7079 7468 6f6e 2070 6163  th to python pac
-000013d0: 6b61 6765 2e22 2c0a 2020 2020 6465 6661  kage.",.    defa
-000013e0: 756c 743d 2222 2c0a 290a 6465 6620 6d61  ult="",.).def ma
-000013f0: 696e 280a 2020 2020 7061 636b 6167 653a  in(.    package:
-00001400: 2054 7261 7665 7273 6162 6c65 2c0a 2020   Traversable,.  
-00001410: 2020 6f75 7470 7574 3a20 5061 7468 207c    output: Path |
-00001420: 204e 6f6e 652c 0a20 2020 2066 6f72 6d61   None,.    forma
-00001430: 743a 204c 6974 6572 616c 5b22 7269 6368  t: Literal["rich
-00001440: 222c 2022 6a73 6f6e 222c 2022 6874 6d6c  ", "json", "html
-00001450: 225d 2c0a 2020 2020 7365 6c65 6374 3a20  "],.    select: 
-00001460: 7374 722c 0a20 2020 2069 676e 6f72 653a  str,.    ignore:
-00001470: 2073 7472 2c0a 2020 2020 7061 636b 6167   str,.    packag
-00001480: 655f 6469 723a 2073 7472 2c0a 2920 2d3e  e_dir: str,.) ->
-00001490: 204e 6f6e 653a 0a20 2020 2022 2222 0a20   None:.    """. 
-000014a0: 2020 2050 6173 7320 696e 2061 206c 6f63     Pass in a loc
-000014b0: 616c 2050 6174 6820 6f72 2067 683a 6f72  al Path or gh:or
-000014c0: 672f 7265 706f 4062 7261 6e63 682e 0a20  g/repo@branch.. 
-000014d0: 2020 2022 2222 0a20 2020 2069 676e 6f72     """.    ignor
-000014e0: 655f 6c69 7374 203d 207b 782e 7374 7269  e_list = {x.stri
-000014f0: 7028 2920 666f 7220 7820 696e 2069 676e  p() for x in ign
-00001500: 6f72 652e 7370 6c69 7428 222c 2229 2069  ore.split(",") i
-00001510: 6620 787d 0a20 2020 2073 656c 6563 745f  f x}.    select_
-00001520: 6c69 7374 203d 207b 782e 7374 7269 7028  list = {x.strip(
-00001530: 2920 666f 7220 7820 696e 2073 656c 6563  ) for x in selec
-00001540: 742e 7370 6c69 7428 222c 2229 2069 6620  t.split(",") if 
-00001550: 787d 0a0a 2020 2020 5f2c 2063 6865 636b  x}..    _, check
-00001560: 732c 205f 203d 205f 636f 6c6c 6563 745f  s, _ = _collect_
-00001570: 616c 6c28 7061 636b 6167 652c 2073 7562  all(package, sub
-00001580: 6469 723d 7061 636b 6167 655f 6469 7229  dir=package_dir)
-00001590: 0a20 2020 2069 6620 6c65 6e28 6368 6563  .    if len(chec
-000015a0: 6b73 2920 3d3d 2030 3a0a 2020 2020 2020  ks) == 0:.      
-000015b0: 2020 6d73 6720 3d20 224e 6f20 6368 6563    msg = "No chec
-000015c0: 6b73 2072 6567 6973 7465 7265 642e 2050  ks registered. P
-000015d0: 6c65 6173 6520 696e 7374 616c 6c20 6120  lease install a 
-000015e0: 7265 706f 2d72 6576 6965 7720 706c 7567  repo-review plug
-000015f0: 696e 2e22 0a20 2020 2020 2020 2072 6169  in.".        rai
-00001600: 7365 2063 6c69 636b 2e43 6c69 636b 4578  se click.ClickEx
-00001610: 6365 7074 696f 6e28 6d73 6729 0a0a 2020  ception(msg)..  
-00001620: 2020 6966 2073 7472 2870 6163 6b61 6765    if str(package
-00001630: 292e 7374 6172 7473 7769 7468 2822 6768  ).startswith("gh
-00001640: 3a22 293a 0a20 2020 2020 2020 205f 2c20  :"):.        _, 
-00001650: 6f72 675f 7265 706f 5f62 7261 6e63 682c  org_repo_branch,
-00001660: 202a 7020 3d20 7374 7228 7061 636b 6167   *p = str(packag
-00001670: 6529 2e73 706c 6974 2822 3a22 2c20 6d61  e).split(":", ma
-00001680: 7873 706c 6974 3d32 290a 2020 2020 2020  xsplit=2).      
-00001690: 2020 6f72 675f 7265 706f 2c20 6272 616e    org_repo, bran
-000016a0: 6368 203d 206f 7267 5f72 6570 6f5f 6272  ch = org_repo_br
-000016b0: 616e 6368 2e73 706c 6974 2822 4022 2c20  anch.split("@", 
-000016c0: 6d61 7873 706c 6974 3d31 290a 2020 2020  maxsplit=1).    
-000016d0: 2020 2020 7061 636b 6167 6520 3d20 4748      package = GH
-000016e0: 5061 7468 2872 6570 6f3d 6f72 675f 7265  Path(repo=org_re
-000016f0: 706f 2c20 6272 616e 6368 3d62 7261 6e63  po, branch=branc
-00001700: 682c 2070 6174 683d 705b 305d 2069 6620  h, path=p[0] if 
-00001710: 7020 656c 7365 2022 2229 0a20 2020 2020  p else "").     
-00001720: 2020 2069 6620 666f 726d 6174 203d 3d20     if format == 
-00001730: 2272 6963 6822 3a0a 2020 2020 2020 2020  "rich":.        
-00001740: 2020 2020 7269 6368 2e70 7269 6e74 2866      rich.print(f
-00001750: 225b 626f 6c64 5d50 726f 6365 7373 696e  "[bold]Processin
-00001760: 6720 5b62 6c75 655d 7b70 6163 6b61 6765  g [blue]{package
-00001770: 7d5b 2f62 6c75 655d 2066 726f 6d20 4769  }[/blue] from Gi
-00001780: 7448 7562 5c6e 2229 0a0a 2020 2020 6661  tHub\n")..    fa
-00001790: 6d69 6c69 6573 2c20 7072 6f63 6573 7365  milies, processe
-000017a0: 6420 3d20 7072 6f63 6573 7328 0a20 2020  d = process(.   
-000017b0: 2020 2020 2070 6163 6b61 6765 2c20 7365       package, se
-000017c0: 6c65 6374 3d73 656c 6563 745f 6c69 7374  lect=select_list
-000017d0: 2c20 6967 6e6f 7265 3d69 676e 6f72 655f  , ignore=ignore_
-000017e0: 6c69 7374 2c20 7375 6264 6972 3d70 6163  list, subdir=pac
-000017f0: 6b61 6765 5f64 6972 0a20 2020 2029 0a0a  kage_dir.    )..
-00001800: 2020 2020 6966 2066 6f72 6d61 7420 3d3d      if format ==
-00001810: 2022 7269 6368 223a 0a20 2020 2020 2020   "rich":.       
-00001820: 2072 6963 685f 7072 696e 7465 7228 6661   rich_printer(fa
-00001830: 6d69 6c69 6573 2c20 7072 6f63 6573 7365  milies, processe
-00001840: 642c 206f 7574 7075 743d 6f75 7470 7574  d, output=output
-00001850: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
-00001860: 2870 726f 6365 7373 6564 2920 3d3d 2030  (processed) == 0
-00001870: 3a0a 2020 2020 2020 2020 2020 2020 7269  :.            ri
-00001880: 6368 2e70 7269 6e74 2822 5b62 6f6c 6420  ch.print("[bold 
-00001890: 7265 645d 4e6f 2063 6865 636b 7320 7261  red]No checks ra
-000018a0: 6e5b 2f62 6f6c 6420 7265 645d 2229 0a20  n[/bold red]"). 
-000018b0: 2020 2065 6c69 6620 666f 726d 6174 203d     elif format =
-000018c0: 3d20 226a 736f 6e22 3a0a 2020 2020 2020  = "json":.      
-000018d0: 2020 6a20 3d20 6a73 6f6e 2e64 756d 7073    j = json.dumps
-000018e0: 280a 2020 2020 2020 2020 2020 2020 7b22  (.            {"
-000018f0: 6661 6d69 6c69 6573 223a 2066 616d 696c  families": famil
-00001900: 6965 732c 2022 6368 6563 6b73 223a 2061  ies, "checks": a
-00001910: 735f 7369 6d70 6c65 5f64 6963 7428 7072  s_simple_dict(pr
-00001920: 6f63 6573 7365 6429 7d2c 2069 6e64 656e  ocessed)}, inden
-00001930: 743d 320a 2020 2020 2020 2020 290a 2020  t=2.        ).  
-00001940: 2020 2020 2020 6966 206f 7574 7075 743a        if output:
-00001950: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-00001960: 7075 742e 7772 6974 655f 7465 7874 286a  put.write_text(j
-00001970: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00001980: 2020 2020 2020 2020 2020 2020 7269 6368              rich
-00001990: 2e70 7269 6e74 5f6a 736f 6e28 6a29 0a20  .print_json(j). 
-000019a0: 2020 2065 6c69 6620 666f 726d 6174 203d     elif format =
-000019b0: 3d20 2268 746d 6c22 3a0a 2020 2020 2020  = "html":.      
-000019c0: 2020 6874 6d6c 203d 2074 6f5f 6874 6d6c    html = to_html
-000019d0: 2866 616d 696c 6965 732c 2070 726f 6365  (families, proce
-000019e0: 7373 6564 290a 2020 2020 2020 2020 6966  ssed).        if
-000019f0: 206f 7574 7075 743a 0a20 2020 2020 2020   output:.       
-00001a00: 2020 2020 206f 7574 7075 742e 7772 6974       output.writ
-00001a10: 655f 7465 7874 2868 746d 6c29 0a20 2020  e_text(html).   
-00001a20: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00001a30: 2020 2020 2020 2072 6963 682e 7072 696e         rich.prin
-00001a40: 7428 6874 6d6c 290a 0a20 2020 2069 6620  t(html)..    if 
-00001a50: 616e 7928 702e 7265 7375 6c74 2069 7320  any(p.result is 
-00001a60: 4661 6c73 6520 666f 7220 7020 696e 2070  False for p in p
-00001a70: 726f 6365 7373 6564 293a 0a20 2020 2020  rocessed):.     
-00001a80: 2020 2072 6169 7365 2053 7973 7465 6d45     raise SystemE
-00001a90: 7869 7428 3229 0a20 2020 2069 6620 6c65  xit(2).    if le
-00001aa0: 6e28 7072 6f63 6573 7365 6429 203d 3d20  n(processed) == 
-00001ab0: 303a 0a20 2020 2020 2020 2072 6169 7365  0:.        raise
-00001ac0: 2053 7973 7465 6d45 7869 7428 3229 0a0a   SystemExit(2)..
-00001ad0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00001ae0: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-00001af0: 6d61 696e 2829 2020 2320 7079 6c69 6e74  main()  # pylint
-00001b00: 3a20 6469 7361 626c 653d 6e6f 2d76 616c  : disable=no-val
-00001b10: 7565 2d66 6f72 2d70 6172 616d 6574 6572  ue-for-parameter
-00001b20: 0a                                       .
+00000020: 6e73 0a0a 696d 706f 7274 2069 7465 7274  ns..import itert
+00000030: 6f6f 6c73 0a69 6d70 6f72 7420 6a73 6f6e  ools.import json
+00000040: 0a69 6d70 6f72 7420 7479 7069 6e67 0a66  .import typing.f
+00000050: 726f 6d20 636f 6c6c 6563 7469 6f6e 732e  rom collections.
+00000060: 6162 6320 696d 706f 7274 204d 6170 7069  abc import Mappi
+00000070: 6e67 0a66 726f 6d20 7061 7468 6c69 6220  ng.from pathlib 
+00000080: 696d 706f 7274 2050 6174 680a 6672 6f6d  import Path.from
+00000090: 2074 7970 696e 6720 696d 706f 7274 204c   typing import L
+000000a0: 6974 6572 616c 0a0a 6966 2074 7970 696e  iteral..if typin
+000000b0: 672e 5459 5045 5f43 4845 434b 494e 473a  g.TYPE_CHECKING:
+000000c0: 0a20 2020 2069 6d70 6f72 7420 636c 6963  .    import clic
+000000d0: 6b0a 656c 7365 3a0a 2020 2020 696d 706f  k.else:.    impo
+000000e0: 7274 2072 6963 685f 636c 6963 6b20 6173  rt rich_click as
+000000f0: 2063 6c69 636b 0a0a 696d 706f 7274 2072   click..import r
+00000100: 6963 682e 636f 6e73 6f6c 650a 696d 706f  ich.console.impo
+00000110: 7274 2072 6963 682e 6d61 726b 646f 776e  rt rich.markdown
+00000120: 0a69 6d70 6f72 7420 7269 6368 2e74 6572  .import rich.ter
+00000130: 6d69 6e61 6c5f 7468 656d 650a 696d 706f  minal_theme.impo
+00000140: 7274 2072 6963 682e 7465 7874 0a69 6d70  rt rich.text.imp
+00000150: 6f72 7420 7269 6368 2e74 7261 6365 6261  ort rich.traceba
+00000160: 636b 0a69 6d70 6f72 7420 7269 6368 2e74  ck.import rich.t
+00000170: 7265 650a 0a66 726f 6d20 2e5f 636f 6d70  ree..from ._comp
+00000180: 6174 2e69 6d70 6f72 746c 6962 2e72 6573  at.importlib.res
+00000190: 6f75 7263 6573 2e61 6263 2069 6d70 6f72  ources.abc impor
+000001a0: 7420 5472 6176 6572 7361 626c 650a 6672  t Traversable.fr
+000001b0: 6f6d 202e 6661 6d69 6c69 6573 2069 6d70  om .families imp
+000001c0: 6f72 7420 4661 6d69 6c79 0a66 726f 6d20  ort Family.from 
+000001d0: 2e67 6870 6174 6820 696d 706f 7274 2047  .ghpath import G
+000001e0: 4850 6174 680a 6672 6f6d 202e 6874 6d6c  HPath.from .html
+000001f0: 2069 6d70 6f72 7420 746f 5f68 746d 6c0a   import to_html.
+00000200: 6672 6f6d 202e 7072 6f63 6573 736f 7220  from .processor 
+00000210: 696d 706f 7274 2052 6573 756c 742c 205f  import Result, _
+00000220: 636f 6c6c 6563 745f 616c 6c2c 2061 735f  collect_all, as_
+00000230: 7369 6d70 6c65 5f64 6963 742c 2070 726f  simple_dict, pro
+00000240: 6365 7373 0a0a 7269 6368 2e74 7261 6365  cess..rich.trace
+00000250: 6261 636b 2e69 6e73 7461 6c6c 2873 7570  back.install(sup
+00000260: 7072 6573 733d 5b63 6c69 636b 2c20 7269  press=[click, ri
+00000270: 6368 5d2c 2073 686f 775f 6c6f 6361 6c73  ch], show_locals
+00000280: 3d54 7275 652c 2077 6964 7468 3d4e 6f6e  =True, width=Non
+00000290: 6529 0a0a 2320 5573 6520 6d6f 6475 6c65  e)..# Use module
+000002a0: 2d6c 6576 656c 2065 6e74 7279 206e 616d  -level entry nam
+000002b0: 6573 0a23 2072 6570 6f5f 7265 7669 6577  es.# repo_review
+000002c0: 5f66 6978 7475 7265 7320 3d20 7b22 7079  _fixtures = {"py
+000002d0: 7072 6f6a 6563 7422 7d0a 2320 7265 706f  project"}.# repo
+000002e0: 5f72 6576 6965 775f 6368 6563 6b73 203d  _review_checks =
+000002f0: 2073 6574 2870 2e5f 5f6e 616d 655f 5f5f   set(p.__name___
+00000300: 2066 6f72 2070 2069 6e20 4765 6e65 7261   for p in Genera
+00000310: 6c2e 5f5f 7375 6263 6c61 7373 6573 5f5f  l.__subclasses__
+00000320: 2829 290a 0a0a 6465 6620 7269 6368 5f70  ())...def rich_p
+00000330: 7269 6e74 6572 280a 2020 2020 6661 6d69  rinter(.    fami
+00000340: 6c69 6573 3a20 4d61 7070 696e 675b 7374  lies: Mapping[st
+00000350: 722c 2046 616d 696c 795d 2c20 7072 6f63  r, Family], proc
+00000360: 6573 7365 643a 206c 6973 745b 5265 7375  essed: list[Resu
+00000370: 6c74 5d2c 202a 2c20 6f75 7470 7574 3a20  lt], *, output: 
+00000380: 5061 7468 207c 204e 6f6e 650a 2920 2d3e  Path | None.) ->
+00000390: 204e 6f6e 653a 0a20 2020 2063 6f6e 736f   None:.    conso
+000003a0: 6c65 203d 2072 6963 682e 636f 6e73 6f6c  le = rich.consol
+000003b0: 652e 436f 6e73 6f6c 6528 7265 636f 7264  e.Console(record
+000003c0: 3d54 7275 6529 0a0a 2020 2020 666f 7220  =True)..    for 
+000003d0: 6661 6d69 6c79 2c20 7265 7375 6c74 735f  family, results_
+000003e0: 6c69 7374 2069 6e20 6974 6572 746f 6f6c  list in itertool
+000003f0: 732e 6772 6f75 7062 7928 7072 6f63 6573  s.groupby(proces
+00000400: 7365 642c 206c 616d 6264 6120 723a 2072  sed, lambda r: r
+00000410: 2e66 616d 696c 7929 3a0a 2020 2020 2020  .family):.      
+00000420: 2020 6661 6d69 6c79 5f6e 616d 6520 3d20    family_name = 
+00000430: 6661 6d69 6c69 6573 5b66 616d 696c 795d  families[family]
+00000440: 2e67 6574 2822 6e61 6d65 222c 2066 616d  .get("name", fam
+00000450: 696c 7929 0a20 2020 2020 2020 2074 7265  ily).        tre
+00000460: 6520 3d20 7269 6368 2e74 7265 652e 5472  e = rich.tree.Tr
+00000470: 6565 2866 225b 626f 6c64 5d7b 6661 6d69  ee(f"[bold]{fami
+00000480: 6c79 5f6e 616d 657d 5b2f 626f 6c64 5d3a  ly_name}[/bold]:
+00000490: 2229 0a20 2020 2020 2020 2066 6f72 2072  ").        for r
+000004a0: 6573 756c 7420 696e 2072 6573 756c 7473  esult in results
+000004b0: 5f6c 6973 743a 0a20 2020 2020 2020 2020  _list:.         
+000004c0: 2020 2063 6f6c 6f72 203d 2028 0a20 2020     color = (.   
+000004d0: 2020 2020 2020 2020 2020 2020 2022 7965               "ye
+000004e0: 6c6c 6f77 220a 2020 2020 2020 2020 2020  llow".          
+000004f0: 2020 2020 2020 6966 2072 6573 756c 742e        if result.
+00000500: 7265 7375 6c74 2069 7320 4e6f 6e65 0a20  result is None. 
+00000510: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00000520: 6c73 6520 2267 7265 656e 220a 2020 2020  lse "green".    
+00000530: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00000540: 6573 756c 742e 7265 7375 6c74 0a20 2020  esult.result.   
+00000550: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00000560: 6520 2272 6564 220a 2020 2020 2020 2020  e "red".        
+00000570: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00000580: 2020 6465 7363 7269 7074 696f 6e20 3d20    description = 
+00000590: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000005a0: 2020 6622 5b6c 696e 6b3d 7b72 6573 756c    f"[link={resul
+000005b0: 742e 7572 6c7d 5d7b 7265 7375 6c74 2e64  t.url}]{result.d
+000005c0: 6573 6372 6970 7469 6f6e 7d5b 2f6c 696e  escription}[/lin
+000005d0: 6b5d 220a 2020 2020 2020 2020 2020 2020  k]".            
+000005e0: 2020 2020 6966 2072 6573 756c 742e 7572      if result.ur
+000005f0: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
+00000600: 2020 656c 7365 2072 6573 756c 742e 6465    else result.de
+00000610: 7363 7269 7074 696f 6e0a 2020 2020 2020  scription.      
+00000620: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00000630: 2020 2020 6d73 6720 3d20 7269 6368 2e74      msg = rich.t
+00000640: 6578 742e 5465 7874 2829 0a20 2020 2020  ext.Text().     
+00000650: 2020 2020 2020 206d 7367 2e61 7070 656e         msg.appen
+00000660: 6428 7265 7375 6c74 2e6e 616d 652c 2073  d(result.name, s
+00000670: 7479 6c65 3d22 626f 6c64 2229 0a20 2020  tyle="bold").   
+00000680: 2020 2020 2020 2020 206d 7367 2e61 7070           msg.app
+00000690: 656e 6428 2220 2229 0a20 2020 2020 2020  end(" ").       
+000006a0: 2020 2020 206d 7367 2e61 7070 656e 6428       msg.append(
+000006b0: 7269 6368 2e74 6578 742e 5465 7874 2e66  rich.text.Text.f
+000006c0: 726f 6d5f 6d61 726b 7570 2864 6573 6372  rom_markup(descr
+000006d0: 6970 7469 6f6e 2c20 7374 796c 653d 636f  iption, style=co
+000006e0: 6c6f 7229 290a 2020 2020 2020 2020 2020  lor)).          
+000006f0: 2020 6966 2072 6573 756c 742e 7265 7375    if result.resu
+00000700: 6c74 2069 7320 4e6f 6e65 3a0a 2020 2020  lt is None:.    
+00000710: 2020 2020 2020 2020 2020 2020 6d73 672e              msg.
+00000720: 6170 7065 6e64 2822 205b 736b 6970 7065  append(" [skippe
+00000730: 645d 222c 2073 7479 6c65 3d22 7965 6c6c  d]", style="yell
+00000740: 6f77 2062 6f6c 6422 290a 2020 2020 2020  ow bold").      
+00000750: 2020 2020 2020 2020 2020 7472 6565 2e61            tree.a
+00000760: 6464 286d 7367 290a 2020 2020 2020 2020  dd(msg).        
+00000770: 2020 2020 656c 6966 2072 6573 756c 742e      elif result.
+00000780: 7265 7375 6c74 3a0a 2020 2020 2020 2020  result:.        
+00000790: 2020 2020 2020 2020 6d73 672e 6170 7065          msg.appe
+000007a0: 6e64 2872 6963 682e 7465 7874 2e54 6578  nd(rich.text.Tex
+000007b0: 742e 6672 6f6d 5f6d 6172 6b75 7028 2220  t.from_markup(" 
+000007c0: 3a77 6869 7465 5f63 6865 636b 5f6d 6172  :white_check_mar
+000007d0: 6b3a 2229 290a 2020 2020 2020 2020 2020  k:")).          
+000007e0: 2020 2020 2020 7472 6565 2e61 6464 286d        tree.add(m
+000007f0: 7367 290a 2020 2020 2020 2020 2020 2020  sg).            
+00000800: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00000810: 2020 2020 2020 6d73 672e 6170 7065 6e64        msg.append
+00000820: 2872 6963 682e 7465 7874 2e54 6578 742e  (rich.text.Text.
+00000830: 6672 6f6d 5f6d 6172 6b75 7028 2220 3a78  from_markup(" :x
+00000840: 3a22 2929 0a20 2020 2020 2020 2020 2020  :")).           
+00000850: 2020 2020 2064 6574 6169 6c20 3d20 7269       detail = ri
+00000860: 6368 2e6d 6172 6b64 6f77 6e2e 4d61 726b  ch.markdown.Mark
+00000870: 646f 776e 2872 6573 756c 742e 6572 725f  down(result.err_
+00000880: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
+00000890: 2020 2020 206d 7367 5f67 7270 203d 2072       msg_grp = r
+000008a0: 6963 682e 636f 6e73 6f6c 652e 4772 6f75  ich.console.Grou
+000008b0: 7028 6d73 672c 2064 6574 6169 6c29 0a20  p(msg, detail). 
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000008d0: 7265 652e 6164 6428 6d73 675f 6772 7029  ree.add(msg_grp)
+000008e0: 0a0a 2020 2020 2020 2020 636f 6e73 6f6c  ..        consol
+000008f0: 652e 7072 696e 7428 7472 6565 290a 2020  e.print(tree).  
+00000900: 2020 2020 2020 636f 6e73 6f6c 652e 7072        console.pr
+00000910: 696e 7428 290a 0a20 2020 2069 6620 6f75  int()..    if ou
+00000920: 7470 7574 2069 7320 6e6f 7420 4e6f 6e65  tput is not None
+00000930: 3a0a 2020 2020 2020 2020 636f 6e73 6f6c  :.        consol
+00000940: 652e 7361 7665 5f73 7667 2873 7472 286f  e.save_svg(str(o
+00000950: 7574 7075 7429 2c20 7468 656d 653d 7269  utput), theme=ri
+00000960: 6368 2e74 6572 6d69 6e61 6c5f 7468 656d  ch.terminal_them
+00000970: 652e 4445 4641 554c 545f 5445 524d 494e  e.DEFAULT_TERMIN
+00000980: 414c 5f54 4845 4d45 290a 0a0a 4063 6c69  AL_THEME)...@cli
+00000990: 636b 2e63 6f6d 6d61 6e64 2863 6f6e 7465  ck.command(conte
+000009a0: 7874 5f73 6574 7469 6e67 733d 7b22 6865  xt_settings={"he
+000009b0: 6c70 5f6f 7074 696f 6e5f 6e61 6d65 7322  lp_option_names"
+000009c0: 3a20 5b22 2d68 222c 2022 2d2d 6865 6c70  : ["-h", "--help
+000009d0: 225d 7d29 0a40 636c 6963 6b2e 6172 6775  "]}).@click.argu
+000009e0: 6d65 6e74 2822 7061 636b 6167 6522 2c20  ment("package", 
+000009f0: 7479 7065 3d63 6c69 636b 2e50 6174 6828  type=click.Path(
+00000a00: 6469 725f 6f6b 6179 3d54 7275 652c 2070  dir_okay=True, p
+00000a10: 6174 685f 7479 7065 3d50 6174 6829 290a  ath_type=Path)).
+00000a20: 4063 6c69 636b 2e6f 7074 696f 6e28 0a20  @click.option(. 
+00000a30: 2020 2022 2d2d 6f75 7470 7574 222c 0a20     "--output",. 
+00000a40: 2020 2074 7970 653d 636c 6963 6b2e 5061     type=click.Pa
+00000a50: 7468 2866 696c 655f 6f6b 6179 3d54 7275  th(file_okay=Tru
+00000a60: 652c 2065 7869 7374 733d 4661 6c73 652c  e, exists=False,
+00000a70: 2070 6174 685f 7479 7065 3d50 6174 6829   path_type=Path)
+00000a80: 2c0a 2020 2020 6465 6661 756c 743d 4e6f  ,.    default=No
+00000a90: 6e65 2c0a 2020 2020 6865 6c70 3d22 5772  ne,.    help="Wr
+00000aa0: 6974 6520 6f75 7420 6669 6c65 2e20 5772  ite out file. Wr
+00000ab0: 6974 6573 2053 5647 2069 6620 666f 726d  ites SVG if form
+00000ac0: 6174 2069 7320 7269 6368 2e22 2c0a 290a  at is rich.",.).
+00000ad0: 4063 6c69 636b 2e6f 7074 696f 6e28 0a20  @click.option(. 
+00000ae0: 2020 2022 2d2d 666f 726d 6174 222c 0a20     "--format",. 
+00000af0: 2020 2022 666f 726d 6174 5f6f 7074 222c     "format_opt",
+00000b00: 0a20 2020 2074 7970 653d 636c 6963 6b2e  .    type=click.
+00000b10: 4368 6f69 6365 285b 2272 6963 6822 2c20  Choice(["rich", 
+00000b20: 226a 736f 6e22 2c20 2268 746d 6c22 5d29  "json", "html"])
+00000b30: 2c0a 2020 2020 6465 6661 756c 743d 2272  ,.    default="r
+00000b40: 6963 6822 2c0a 2020 2020 6865 6c70 3d22  ich",.    help="
+00000b50: 5365 6c65 6374 206f 7574 7075 7420 666f  Select output fo
+00000b60: 726d 6174 2e22 2c0a 290a 4063 6c69 636b  rmat.",.).@click
+00000b70: 2e6f 7074 696f 6e28 0a20 2020 2022 2d2d  .option(.    "--
+00000b80: 7365 6c65 6374 222c 0a20 2020 2068 656c  select",.    hel
+00000b90: 703d 224f 6e6c 7920 7275 6e20 6365 7274  p="Only run cert
+00000ba0: 6169 6e20 6368 6563 6b73 2c20 636f 6d6d  ain checks, comm
+00000bb0: 6120 7365 7061 7261 7465 642e 2041 6c6c  a separated. All
+00000bc0: 2063 6865 636b 7320 7275 6e20 6966 2065   checks run if e
+00000bd0: 6d70 7479 2e22 2c0a 2020 2020 6465 6661  mpty.",.    defa
+00000be0: 756c 743d 2222 2c0a 290a 4063 6c69 636b  ult="",.).@click
+00000bf0: 2e6f 7074 696f 6e28 0a20 2020 2022 2d2d  .option(.    "--
+00000c00: 6967 6e6f 7265 222c 0a20 2020 2068 656c  ignore",.    hel
+00000c10: 703d 2249 676e 6f72 6520 6120 6368 6563  p="Ignore a chec
+00000c20: 6b20 6f72 2063 6865 636b 732c 2063 6f6d  k or checks, com
+00000c30: 6d61 2073 6570 6172 6174 6564 2e22 2c0a  ma separated.",.
+00000c40: 2020 2020 6465 6661 756c 743d 2222 2c0a      default="",.
+00000c50: 290a 4063 6c69 636b 2e6f 7074 696f 6e28  ).@click.option(
+00000c60: 0a20 2020 2022 2d2d 7061 636b 6167 652d  .    "--package-
+00000c70: 6469 7222 2c0a 2020 2020 222d 7022 2c0a  dir",.    "-p",.
+00000c80: 2020 2020 6865 6c70 3d22 5061 7468 2074      help="Path t
+00000c90: 6f20 7079 7468 6f6e 2070 6163 6b61 6765  o python package
+00000ca0: 2e22 2c0a 2020 2020 6465 6661 756c 743d  .",.    default=
+00000cb0: 2222 2c0a 290a 4063 6c69 636b 2e6f 7074  "",.).@click.opt
+00000cc0: 696f 6e28 0a20 2020 2022 2d2d 6c69 7374  ion(.    "--list
+00000cd0: 2f2d 2d6e 6f2d 6c69 7374 222c 0a20 2020  /--no-list",.   
+00000ce0: 2022 6c69 7374 5f6f 7074 222c 0a20 2020   "list_opt",.   
+00000cf0: 2068 656c 703d 224c 6973 7420 616c 6c20   help="List all 
+00000d00: 6368 6563 6b73 2061 6e64 2065 7869 7422  checks and exit"
+00000d10: 2c0a 2020 2020 6465 6661 756c 743d 4661  ,.    default=Fa
+00000d20: 6c73 652c 0a29 0a64 6566 206d 6169 6e28  lse,.).def main(
+00000d30: 0a20 2020 2070 6163 6b61 6765 3a20 5472  .    package: Tr
+00000d40: 6176 6572 7361 626c 652c 0a20 2020 206f  aversable,.    o
+00000d50: 7574 7075 743a 2050 6174 6820 7c20 4e6f  utput: Path | No
+00000d60: 6e65 2c0a 2020 2020 666f 726d 6174 5f6f  ne,.    format_o
+00000d70: 7074 3a20 4c69 7465 7261 6c5b 2272 6963  pt: Literal["ric
+00000d80: 6822 2c20 226a 736f 6e22 2c20 2268 746d  h", "json", "htm
+00000d90: 6c22 5d2c 0a20 2020 2073 656c 6563 743a  l"],.    select:
+00000da0: 2073 7472 2c0a 2020 2020 6967 6e6f 7265   str,.    ignore
+00000db0: 3a20 7374 722c 0a20 2020 2070 6163 6b61  : str,.    packa
+00000dc0: 6765 5f64 6972 3a20 7374 722c 0a20 2020  ge_dir: str,.   
+00000dd0: 206c 6973 745f 6f70 743a 2062 6f6f 6c2c   list_opt: bool,
+00000de0: 0a29 202d 3e20 4e6f 6e65 3a0a 2020 2020  .) -> None:.    
+00000df0: 2222 220a 2020 2020 5061 7373 2069 6e20  """.    Pass in 
+00000e00: 6120 6c6f 6361 6c20 5061 7468 206f 7220  a local Path or 
+00000e10: 6768 3a6f 7267 2f72 6570 6f40 6272 616e  gh:org/repo@bran
+00000e20: 6368 2e0a 2020 2020 2222 220a 2020 2020  ch..    """.    
+00000e30: 6967 6e6f 7265 5f6c 6973 7420 3d20 7b78  ignore_list = {x
+00000e40: 2e73 7472 6970 2829 2066 6f72 2078 2069  .strip() for x i
+00000e50: 6e20 6967 6e6f 7265 2e73 706c 6974 2822  n ignore.split("
+00000e60: 2c22 2920 6966 2078 7d0a 2020 2020 7365  ,") if x}.    se
+00000e70: 6c65 6374 5f6c 6973 7420 3d20 7b78 2e73  lect_list = {x.s
+00000e80: 7472 6970 2829 2066 6f72 2078 2069 6e20  trip() for x in 
+00000e90: 7365 6c65 6374 2e73 706c 6974 2822 2c22  select.split(","
+00000ea0: 2920 6966 2078 7d0a 0a20 2020 205f 2c20  ) if x}..    _, 
+00000eb0: 6368 6563 6b73 2c20 6661 6d69 6c69 6573  checks, families
+00000ec0: 203d 205f 636f 6c6c 6563 745f 616c 6c28   = _collect_all(
+00000ed0: 7061 636b 6167 652c 2073 7562 6469 723d  package, subdir=
+00000ee0: 7061 636b 6167 655f 6469 7229 0a20 2020  package_dir).   
+00000ef0: 2069 6620 6c65 6e28 6368 6563 6b73 2920   if len(checks) 
+00000f00: 3d3d 2030 3a0a 2020 2020 2020 2020 6d73  == 0:.        ms
+00000f10: 6720 3d20 224e 6f20 6368 6563 6b73 2072  g = "No checks r
+00000f20: 6567 6973 7465 7265 642e 2050 6c65 6173  egistered. Pleas
+00000f30: 6520 696e 7374 616c 6c20 6120 7265 706f  e install a repo
+00000f40: 2d72 6576 6965 7720 706c 7567 696e 2e22  -review plugin."
+00000f50: 0a20 2020 2020 2020 2072 6169 7365 2063  .        raise c
+00000f60: 6c69 636b 2e43 6c69 636b 4578 6365 7074  lick.ClickExcept
+00000f70: 696f 6e28 6d73 6729 0a0a 2020 2020 6966  ion(msg)..    if
+00000f80: 206c 6973 745f 6f70 743a 0a20 2020 2020   list_opt:.     
+00000f90: 2020 2066 6f72 2066 616d 696c 792c 2067     for family, g
+00000fa0: 7270 2069 6e20 6974 6572 746f 6f6c 732e  rp in itertools.
+00000fb0: 6772 6f75 7062 7928 6368 6563 6b73 2e69  groupby(checks.i
+00000fc0: 7465 6d73 2829 2c20 6b65 793d 6c61 6d62  tems(), key=lamb
+00000fd0: 6461 2078 3a20 785b 315d 2e66 616d 696c  da x: x[1].famil
+00000fe0: 7929 3a0a 2020 2020 2020 2020 2020 2020  y):.            
+00000ff0: 7269 6368 2e70 7269 6e74 2866 2720 205b  rich.print(f'  [
+00001000: 6469 6d5d 2320 7b66 616d 696c 6965 735b  dim]# {families[
+00001010: 6661 6d69 6c79 5d2e 6765 7428 226e 616d  family].get("nam
+00001020: 6522 2c20 6661 6d69 6c79 297d 2729 0a20  e", family)}'). 
+00001030: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+00001040: 6f64 652c 2063 6865 636b 2069 6e20 6772  ode, check in gr
+00001050: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+00001060: 2020 2072 6963 682e 7072 696e 7428 6627     rich.print(f'
+00001070: 2020 227b 636f 6465 7d22 2c20 205b 6469    "{code}",  [di
+00001080: 6d5d 2320 7b63 6865 636b 2e5f 5f64 6f63  m]# {check.__doc
+00001090: 5f5f 7d27 290a 0a20 2020 2020 2020 2072  __}')..        r
+000010a0: 6169 7365 2053 7973 7465 6d45 7869 7428  aise SystemExit(
+000010b0: 3029 0a0a 2020 2020 6966 2073 7472 2870  0)..    if str(p
+000010c0: 6163 6b61 6765 292e 7374 6172 7473 7769  ackage).startswi
+000010d0: 7468 2822 6768 3a22 293a 0a20 2020 2020  th("gh:"):.     
+000010e0: 2020 205f 2c20 6f72 675f 7265 706f 5f62     _, org_repo_b
+000010f0: 7261 6e63 682c 202a 7020 3d20 7374 7228  ranch, *p = str(
+00001100: 7061 636b 6167 6529 2e73 706c 6974 2822  package).split("
+00001110: 3a22 2c20 6d61 7873 706c 6974 3d32 290a  :", maxsplit=2).
+00001120: 2020 2020 2020 2020 6f72 675f 7265 706f          org_repo
+00001130: 2c20 6272 616e 6368 203d 206f 7267 5f72  , branch = org_r
+00001140: 6570 6f5f 6272 616e 6368 2e73 706c 6974  epo_branch.split
+00001150: 2822 4022 2c20 6d61 7873 706c 6974 3d31  ("@", maxsplit=1
+00001160: 290a 2020 2020 2020 2020 7061 636b 6167  ).        packag
+00001170: 6520 3d20 4748 5061 7468 2872 6570 6f3d  e = GHPath(repo=
+00001180: 6f72 675f 7265 706f 2c20 6272 616e 6368  org_repo, branch
+00001190: 3d62 7261 6e63 682c 2070 6174 683d 705b  =branch, path=p[
+000011a0: 305d 2069 6620 7020 656c 7365 2022 2229  0] if p else "")
+000011b0: 0a20 2020 2020 2020 2069 6620 666f 726d  .        if form
+000011c0: 6174 5f6f 7074 203d 3d20 2272 6963 6822  at_opt == "rich"
+000011d0: 3a0a 2020 2020 2020 2020 2020 2020 7269  :.            ri
+000011e0: 6368 2e70 7269 6e74 2866 225b 626f 6c64  ch.print(f"[bold
+000011f0: 5d50 726f 6365 7373 696e 6720 5b62 6c75  ]Processing [blu
+00001200: 655d 7b70 6163 6b61 6765 7d5b 2f62 6c75  e]{package}[/blu
+00001210: 655d 2066 726f 6d20 4769 7448 7562 5c6e  e] from GitHub\n
+00001220: 2229 0a0a 2020 2020 6661 6d69 6c69 6573  ")..    families
+00001230: 2c20 7072 6f63 6573 7365 6420 3d20 7072  , processed = pr
+00001240: 6f63 6573 7328 0a20 2020 2020 2020 2070  ocess(.        p
+00001250: 6163 6b61 6765 2c20 7365 6c65 6374 3d73  ackage, select=s
+00001260: 656c 6563 745f 6c69 7374 2c20 6967 6e6f  elect_list, igno
+00001270: 7265 3d69 676e 6f72 655f 6c69 7374 2c20  re=ignore_list, 
+00001280: 7375 6264 6972 3d70 6163 6b61 6765 5f64  subdir=package_d
+00001290: 6972 0a20 2020 2029 0a0a 2020 2020 6966  ir.    )..    if
+000012a0: 2066 6f72 6d61 745f 6f70 7420 3d3d 2022   format_opt == "
+000012b0: 7269 6368 223a 0a20 2020 2020 2020 2072  rich":.        r
+000012c0: 6963 685f 7072 696e 7465 7228 6661 6d69  ich_printer(fami
+000012d0: 6c69 6573 2c20 7072 6f63 6573 7365 642c  lies, processed,
+000012e0: 206f 7574 7075 743d 6f75 7470 7574 290a   output=output).
+000012f0: 2020 2020 2020 2020 6966 206c 656e 2870          if len(p
+00001300: 726f 6365 7373 6564 2920 3d3d 2030 3a0a  rocessed) == 0:.
+00001310: 2020 2020 2020 2020 2020 2020 7269 6368              rich
+00001320: 2e70 7269 6e74 2822 5b62 6f6c 6420 7265  .print("[bold re
+00001330: 645d 4e6f 2063 6865 636b 7320 7261 6e5b  d]No checks ran[
+00001340: 2f62 6f6c 6420 7265 645d 2229 0a20 2020  /bold red]").   
+00001350: 2065 6c69 6620 666f 726d 6174 5f6f 7074   elif format_opt
+00001360: 203d 3d20 226a 736f 6e22 3a0a 2020 2020   == "json":.    
+00001370: 2020 2020 6a20 3d20 6a73 6f6e 2e64 756d      j = json.dum
+00001380: 7073 280a 2020 2020 2020 2020 2020 2020  ps(.            
+00001390: 7b22 6661 6d69 6c69 6573 223a 2066 616d  {"families": fam
+000013a0: 696c 6965 732c 2022 6368 6563 6b73 223a  ilies, "checks":
+000013b0: 2061 735f 7369 6d70 6c65 5f64 6963 7428   as_simple_dict(
+000013c0: 7072 6f63 6573 7365 6429 7d2c 2069 6e64  processed)}, ind
+000013d0: 656e 743d 320a 2020 2020 2020 2020 290a  ent=2.        ).
+000013e0: 2020 2020 2020 2020 6966 206f 7574 7075          if outpu
+000013f0: 743a 0a20 2020 2020 2020 2020 2020 206f  t:.            o
+00001400: 7574 7075 742e 7772 6974 655f 7465 7874  utput.write_text
+00001410: 286a 290a 2020 2020 2020 2020 656c 7365  (j).        else
+00001420: 3a0a 2020 2020 2020 2020 2020 2020 7269  :.            ri
+00001430: 6368 2e70 7269 6e74 5f6a 736f 6e28 6a29  ch.print_json(j)
+00001440: 0a20 2020 2065 6c69 6620 666f 726d 6174  .    elif format
+00001450: 5f6f 7074 203d 3d20 2268 746d 6c22 3a0a  _opt == "html":.
+00001460: 2020 2020 2020 2020 6874 6d6c 203d 2074          html = t
+00001470: 6f5f 6874 6d6c 2866 616d 696c 6965 732c  o_html(families,
+00001480: 2070 726f 6365 7373 6564 290a 2020 2020   processed).    
+00001490: 2020 2020 6966 206f 7574 7075 743a 0a20      if output:. 
+000014a0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+000014b0: 742e 7772 6974 655f 7465 7874 2868 746d  t.write_text(htm
+000014c0: 6c29 0a20 2020 2020 2020 2065 6c73 653a  l).        else:
+000014d0: 0a20 2020 2020 2020 2020 2020 2072 6963  .            ric
+000014e0: 682e 7072 696e 7428 6874 6d6c 290a 0a20  h.print(html).. 
+000014f0: 2020 2069 6620 616e 7928 702e 7265 7375     if any(p.resu
+00001500: 6c74 2069 7320 4661 6c73 6520 666f 7220  lt is False for 
+00001510: 7020 696e 2070 726f 6365 7373 6564 293a  p in processed):
+00001520: 0a20 2020 2020 2020 2072 6169 7365 2053  .        raise S
+00001530: 7973 7465 6d45 7869 7428 3229 0a20 2020  ystemExit(2).   
+00001540: 2069 6620 6c65 6e28 7072 6f63 6573 7365   if len(processe
+00001550: 6429 203d 3d20 303a 0a20 2020 2020 2020  d) == 0:.       
+00001560: 2072 6169 7365 2053 7973 7465 6d45 7869   raise SystemExi
+00001570: 7428 3229 0a0a 0a69 6620 5f5f 6e61 6d65  t(2)...if __name
+00001580: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
+00001590: 3a0a 2020 2020 6d61 696e 2829 2020 2320  :.    main()  # 
+000015a0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+000015b0: 6e6f 2d76 616c 7565 2d66 6f72 2d70 6172  no-value-for-par
+000015c0: 616d 6574 6572 0a                        ameter.
```

### Comparing `repo_review-0.7.0b4/src/repo_review/checks.py` & `repo_review-0.7.0b5/src/repo_review/checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/src/repo_review/fixtures.py` & `repo_review-0.7.0b5/src/repo_review/fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/src/repo_review/ghpath.py` & `repo_review-0.7.0b5/src/repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/src/repo_review/processor.py` & `repo_review-0.7.0b5/src/repo_review/processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import dataclasses
 import graphlib
 import textwrap
 import typing
-from collections.abc import Set
-from typing import Any
+from collections.abc import Mapping, Set
+from typing import Any, TypeVar
 
 import markdown_it
 
 from ._compat.importlib.resources.abc import Traversable
 from .checks import Check, collect_checks, is_allowed
 from .families import Family, collect_families
 from .fixtures import apply_fixtures, collect_fixtures, compute_fixtures, pyproject
@@ -55,14 +55,34 @@
 
 
 class ProcessReturn(typing.NamedTuple):
     families: dict[str, Family]
     results: list[Result]
 
 
+class HasFamily(typing.Protocol):
+    @property
+    def family(self) -> str:
+        ...
+
+
+T = TypeVar("T", bound=HasFamily)
+
+
+def _sort_by_family(
+    families: Mapping[str, Family], dict_has_family: Mapping[str, T]
+) -> dict[str, T]:
+    return dict(
+        sorted(
+            dict_has_family.items(),
+            key=lambda x: (families[x[1].family].get("order", 0), x[1].family, x[0]),
+        )
+    )
+
+
 def _collect_all(
     root: Traversable, subdir: str = ""
 ) -> tuple[dict[str, Any], dict[str, Check], dict[str, Family]]:
     package = root.joinpath(subdir) if subdir else root
 
     # Collect the fixtures
     fixture_functions = collect_fixtures()
@@ -75,14 +95,17 @@
     families = collect_families()
 
     # These are optional, so fill in missing families.
     for name in {c.family for c in checks.values()}:
         if name not in families:
             families[name] = Family()
 
+    # Sort results
+    checks = _sort_by_family(families, checks)
+
     return fixtures, checks, families
 
 
 def process(
     root: Traversable,
     *,
     select: Set[str] = frozenset(),
@@ -129,18 +152,15 @@
             else:
                 completed[name] = result
         else:
             completed[name] = None
 
     # Collect the results
     result_list = []
-    for task_name, check in sorted(
-        tasks.items(),
-        key=lambda x: (families[x[1].family].get("order", 0), x[1].family, x[0]),
-    ):
+    for task_name, check in _sort_by_family(families, tasks).items():
         result = None if completed[task_name] is None else not completed[task_name]
         doc = check.__doc__ or ""
         err_msg = completed[task_name] or ""
 
         if not is_allowed(select_checks, skip_checks, task_name):
             continue
```

### Comparing `repo_review-0.7.0b4/tests/test_checks.py` & `repo_review-0.7.0b5/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/tests/test_fixtures.py` & `repo_review-0.7.0b5/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/tests/test_package.py` & `repo_review-0.7.0b5/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/tests/test_self.py` & `repo_review-0.7.0b5/tests/test_self.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,25 @@
 def patch_entry_points(monkeypatch: pytest.MonkeyPatch) -> None:
     orig_ep = importlib.metadata.entry_points
     ep = importlib.metadata.EntryPoint(
         name="pyproject",
         group="repo_review.checks",
         value="pyproject:repo_review_checks",
     )
-    monkeypatch.setattr(
-        importlib.metadata,
-        "entry_points",
-        lambda group: [ep] if group == "repo_review.checks" else orig_ep(group=group),
-    )
+
+    def new_ep(*, group: str) -> list[importlib.metadata.EntryPoint]:
+        if group == "repo_review.checks":
+            return [ep]
+        if group in {"repo_review.fixtures", "repo_review.families"}:
+            return [
+                e for e in orig_ep(group=group) if e.module.startswith("repo_review.")
+            ]
+        return orig_ep(group=group)
+
+    monkeypatch.setattr(importlib.metadata, "entry_points", new_ep)
 
 
 def test_pyproject() -> None:
     families, results = repo_review.processor.process(Path("."))
 
     assert families == {"general": {}, "pyproject": {}}
     assert len(results) == 9
```

### Comparing `repo_review-0.7.0b4/tests/test_utilities/pyproject.py` & `repo_review-0.7.0b5/tests/test_utilities/pyproject.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/.gitignore` & `repo_review-0.7.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/LICENSE` & `repo_review-0.7.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b4/README.md` & `repo_review-0.7.0b5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- SPHINX-START -->
 
 This is a framework for building checks designed to check to see if a
 repository follows guidelines. By itself, it does nothing - it requires at
-least one plugin to be installed..
+least one plugin to be installed.
 
 With one or more plugins, it will produce a list of results - green checkmarks
 mean this rule is followed, red x’s mean the rule is not. A yellow warning sign
 means that the check was skipped because a previous required check failed.
 
 `sp-repo-review` provides checks based on the
-[Scientific-Python Development Guide][] at [scientific-python/cookie][].
+[Scientific-Python Development Guide][] at [scientific-python/cookie][]. A live
+WebAssembly demo using `sp-repo-review` is
+[here](https://scientific-python.github.io/repo-review).
 
 ## Running repo-review
 
 Repo-review supports running multiple ways:
 
 - From the command line on a local folder
 - From the command line on a remote repository on GitHub (`gh:org/repo@branch`)
```

### Comparing `repo_review-0.7.0b4/pyproject.toml` & `repo_review-0.7.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 cli = [
   "click>=8",
   "rich>=12.2",
   "rich-click",
 ]
 test = [
   "pytest >=7",
+  "sp-repo-review",
 ]
 dev = [
   "repo-review[test,cli]",
 ]
 docs = [
   "repo-review[cli]",
   "furo",
```

### Comparing `repo_review-0.7.0b4/PKG-INFO` & `repo_review-0.7.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.7.0b4
+Version: 0.7.0b5
 Summary: Framework that can run checks on repos
 Project-URL: homepage, https://github.com/scientific-python/repo-review
 Project-URL: webpage, https://scientific-python.github.io/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Henry Schreiner.
@@ -60,36 +60,39 @@
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: repo-review[cli]; extra == 'docs'
 Requires-Dist: sphinx>=4.0; extra == 'docs'
 Requires-Dist: sphinxcontrib-programoutput; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == 'test'
+Requires-Dist: sp-repo-review; extra == 'test'
 Description-Content-Type: text/markdown
 
 # repo-review
 
 [![Actions Status][actions-badge]][actions-link]
 [![Code style: black][black-badge]][black-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- SPHINX-START -->
 
 This is a framework for building checks designed to check to see if a
 repository follows guidelines. By itself, it does nothing - it requires at
-least one plugin to be installed..
+least one plugin to be installed.
 
 With one or more plugins, it will produce a list of results - green checkmarks
 mean this rule is followed, red x’s mean the rule is not. A yellow warning sign
 means that the check was skipped because a previous required check failed.
 
 `sp-repo-review` provides checks based on the
-[Scientific-Python Development Guide][] at [scientific-python/cookie][].
+[Scientific-Python Development Guide][] at [scientific-python/cookie][]. A live
+WebAssembly demo using `sp-repo-review` is
+[here](https://scientific-python.github.io/repo-review).
 
 ## Running repo-review
 
 Repo-review supports running multiple ways:
 
 - From the command line on a local folder
 - From the command line on a remote repository on GitHub (`gh:org/repo@branch`)
```

