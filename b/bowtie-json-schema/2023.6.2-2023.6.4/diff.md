# Comparing `tmp/bowtie_json_schema-2023.6.2.tar.gz` & `tmp/bowtie_json_schema-2023.6.4.tar.gz`

## Comparing `bowtie_json_schema-2023.6.2.tar` & `bowtie_json_schema-2023.6.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.flake8
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.readthedocs.yml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/action.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/test-requirements.in
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/SECURITY.md
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/release.yml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/workflows/images.yml
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/__main__.py
--rw-r--r--   0        0        0    31383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/_cli.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/_core.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/cli.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/conf.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/requirements.in
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/requirements.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/docs/_static/dreamed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/conftest.py
--rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/LICENSE
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/README.rst
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/pyproject.toml
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.2/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.flake8
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.readthedocs.yml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/action.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/test-requirements.in
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/SECURITY.md
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/release.yml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/workflows/images.yml
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/__main__.py
+-rw-r--r--   0        0        0    31499 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/_cli.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/cli.rst
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/conf.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/contributing.rst
+-rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/requirements.in
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/requirements.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/docs/_static/dreamed.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/conftest.py
+-rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     2890 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/LICENSE
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/README.rst
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/pyproject.toml
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.6.4/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.6.2/.flake8` & `bowtie_json_schema-2023.6.4/.flake8`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/.pre-commit-config.yaml` & `bowtie_json_schema-2023.6.4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     hooks:
       - id: pyupgrade
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: "v0.0.270"
     hooks:
       - id: ruff
   - repo: https://github.com/Riverside-Healthcare/djLint
-    rev: v1.29.0
+    rev: v1.30.2
     hooks:
       - id: djlint-jinja
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - name: black (python implementations & bowtie internals)
         id: black
@@ -53,15 +53,15 @@
   - repo: https://github.com/doublify/pre-commit-rust
     rev: "v1.0"
     hooks:
       - name: cargo fmt rust-boon
         id: fmt
         args: ["--manifest-path", "implementations/rust-boon/Cargo.toml", "--"]
   - repo: https://github.com/syntaqx/git-hooks
-    rev: v0.0.17
+    rev: v0.0.18
     hooks:
       - name: go fmt (golang implementations)
         id: go-fmt
   - repo: https://github.com/jumanjihouse/pre-commit-hooks
     rev: "3.0.0"
     hooks:
       - name: rubocop (ruby implementations)
```

### Comparing `bowtie_json_schema-2023.6.2/noxfile.py` & `bowtie_json_schema-2023.6.4/noxfile.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from contextlib import ExitStack
 from pathlib import Path
+from tempfile import TemporaryDirectory
+import os
 import shlex
 
 import nox
 
 ROOT = Path(__file__).parent
 PYPROJECT = ROOT / "pyproject.toml"
 DOCS = ROOT / "docs"
@@ -19,61 +22,78 @@
         if default:
             nox.options.sessions.append(kwargs.get("name", fn.__name__))
         return nox.session(**kwargs)(fn)
 
     return _session
 
 
-@session(python=["3.8", "3.9", "3.10", "3.11"])
+@session(python=["3.10", "3.11"])
 def tests(session):
     session.install("-r", ROOT / "test-requirements.txt")
-    session.run("pytest", "--verbosity=3")
+
+    if session.posargs and session.posargs[0] == "coverage":
+        if len(session.posargs) > 1 and session.posargs[1] == "github":
+            github = os.environ["GITHUB_STEP_SUMMARY"]
+        else:
+            github = None
+
+        session.install("coverage[toml]")
+        session.run("coverage", "run", "-m", "pytest", TESTS)
+        if github is None:
+            session.run("coverage", "report")
+        else:
+            with open(github, "a") as summary:
+                summary.write("### Coverage\n\n")
+                summary.flush()  # without a flush, output seems out of order.
+                session.run(
+                    "coverage",
+                    "report",
+                    "--format=markdown",
+                    stdout=summary,
+                )
+    else:
+        session.run("pytest", *session.posargs, TESTS)
 
 
 @session(tags=["build"])
 def build(session):
-    session.install("build")
-    tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
+    session.install("build", "twine")
+    with TemporaryDirectory() as tmpdir:
+        session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
+        session.run("twine", "check", "--strict", tmpdir + "/*")
 
 
 @session(tags=["build"])
 def shiv(session):
     session.install("shiv")
-    if session.posargs:
-        out = session.posargs[0]
-    else:
-        tmpdir = Path(session.create_tmp())
-        out = tmpdir / "bowtie"
-    session.run(
-        "python",
-        "-m",
-        "shiv",
-        "--reproducible",
-        "-c",
-        "bowtie",
-        ROOT,
-        "-o",
-        out,
-    )
-    print(f"Outputted a shiv to {out}.")
 
-
-@session(tags=["style"])
-def readme(session):
-    session.install("build", "twine")
-    tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-    session.run("python", "-m", "twine", "check", "--strict", tmpdir + "/*")
+    with ExitStack() as stack:
+        if session.posargs:
+            out = session.posargs[0]
+        else:
+            tmpdir = Path(stack.enter_context(TemporaryDirectory()))
+            out = tmpdir / "bowtie"
+        session.run(
+            "python",
+            "-m",
+            "shiv",
+            "--reproducible",
+            "-c",
+            "bowtie",
+            ROOT,
+            "-o",
+            out,
+        )
+        print(f"Outputted a shiv to {out}.")
 
 
 @session(tags=["style"])
 def style(session):
     session.install("ruff")
-    session.run("python", "-m", "ruff", "check", BOWTIE, TESTS, __file__)
+    session.run("ruff", "check", BOWTIE, TESTS, __file__)
 
 
 @session()
 def typing(session):
     session.install("pyright", ROOT)
     session.run("pyright", BOWTIE)
 
@@ -90,28 +110,29 @@
             "man",
             "spelling",
         ]
     ],
 )
 def docs(session, builder):
     session.install("-r", DOCS / "requirements.txt")
-    tmpdir = Path(session.create_tmp())
-    argv = ["-n", "-T", "-W"]
-    if builder != "spelling":
-        argv += ["-q"]
-    session.run(
-        "python",
-        "-m",
-        "sphinx",
-        "-b",
-        builder,
-        DOCS,
-        tmpdir / builder,
-        *argv,
-    )
+    with TemporaryDirectory() as tmpdir_str:
+        tmpdir = Path(tmpdir_str)
+        argv = ["-n", "-T", "-W"]
+        if builder != "spelling":
+            argv += ["-q"]
+        session.run(
+            "python",
+            "-m",
+            "sphinx",
+            "-b",
+            builder,
+            DOCS,
+            tmpdir / builder,
+            *argv,
+        )
 
 
 @session(tags=["docs", "style"], name="docs(style)")
 def docs_style(session):
     session.install(
         "doc8",
         "pygments",
```

### Comparing `bowtie_json_schema-2023.6.2/test-requirements.txt` & `bowtie_json_schema-2023.6.4/test-requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 markdown-it-py[linkify,plugins]==2.2.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
 markupsafe==2.1.3
     # via jinja2
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.0
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
```

### Comparing `bowtie_json_schema-2023.6.2/.github/SECURITY.md` & `bowtie_json_schema-2023.6.4/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/.github/dependabot.yml` & `bowtie_json_schema-2023.6.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/.github/workflows/ci.yml` & `bowtie_json_schema-2023.6.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.6.4/.github/workflows/dependabot-merge.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/.github/workflows/images.yml` & `bowtie_json_schema-2023.6.4/.github/workflows/images.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/.github/workflows/report.yml` & `bowtie_json_schema-2023.6.4/.github/workflows/report.yml`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,22 @@
           python-version: "3.x"
 
       - name: Install Bowtie
         run: python3 -m pip install bowtie-json-schema
 
       - name: Generate the Report
         run: |
-          bowtie suite $(find implementations/ -mindepth 1 -maxdepth 1 -type d | sed 's/implementations\//-i /') https://github.com/json-schema-org/JSON-Schema-Test-Suite/tree/main/tests/${{ matrix.version }} | tee >(gzip >${{ matrix.version }}.json.gz) | bowtie report --badges badges --generate-dialect-navigation --out ${{ matrix.version }}.html
+          bowtie suite $(find implementations/ -mindepth 1 -maxdepth 1 -type d | sed 's/implementations\//-i /') https://github.com/json-schema-org/JSON-Schema-Test-Suite/tree/main/tests/${{ matrix.version }} | tee ${{ matrix.version }}.jsonl | bowtie report --badges badges --generate-dialect-navigation --out ${{ matrix.version }}.html
 
       - uses: actions/upload-artifact@v3
         with:
           name: report
           path: |
             ${{ matrix.version }}.html
-            ${{ matrix.version }}.json.gz
+            ${{ matrix.version }}.jsonl
             badges/
 
   collect:
     runs-on: ubuntu-latest
     needs: test
 
     steps:
```

### Comparing `bowtie_json_schema-2023.6.2/bowtie/_cli.py` & `bowtie_json_schema-2023.6.4/bowtie/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from collections.abc import Awaitable, Callable, Iterable
 from contextlib import AsyncExitStack, asynccontextmanager
 from fnmatch import fnmatch
+from importlib.resources import files
 from io import BytesIO
 from pathlib import Path
-from typing import Any, AsyncIterator, TextIO, Union
+from typing import Any, AsyncIterator, Literal, TextIO, Union
 from urllib.parse import urljoin
 import asyncio
 import json
 import os
 import sys
 import zipfile
 
@@ -33,19 +34,14 @@
     NoSuchImage,
     StartupFailed,
 )
 from bowtie.exceptions import (
     _ProtocolError,  # type: ignore[reportPrivateUsage]
 )
 
-try:
-    from importlib.resources import files
-except ImportError:
-    from importlib_resources import files  # type: ignore
-
 IMAGE_REPOSITORY = "ghcr.io/bowtie-json-schema"
 TEST_SUITE_URL = "https://github.com/json-schema-org/json-schema-test-suite"
 
 DRAFT2020 = "https://json-schema.org/draft/2020-12/schema"
 DRAFT2019 = "https://json-schema.org/draft/2019-09/schema"
 DRAFT7 = "http://json-schema.org/draft-07/schema#"
 DRAFT6 = "http://json-schema.org/draft-06/schema#"
@@ -82,14 +78,15 @@
     "-f",
     "format",
     help="What format to use for the output",
     default=lambda: "pretty" if sys.stdout.isatty() else "json",
     show_default="pretty if stdout is a tty, otherwise JSON",
     type=click.Choice(["json", "pretty"]),
 )
+_F = Literal["json", "pretty"]
 
 
 @tui()
 @click.group(context_settings=dict(help_option_names=["--help", "-h"]))
 @click.version_option(prog_name="bowtie", package_name="bowtie-json-schema")
 def main():
     """
@@ -160,15 +157,15 @@
     type=click.Choice(["failures", "validation"]),
 )
 @click.argument(
     "input",
     default="-",
     type=click.File(mode="r"),
 )
-def summary(input: Iterable[str], format: str, show: str):
+def summary(input: Iterable[str], format: _F, show: str):
     """
     Generate an (in-terminal) summary of a Bowtie run.
     """
     summary = _report.from_input(input)["summary"]
     if show == "failures":
         results = _ordered_failures(summary)
         to_table = _failure_table
@@ -179,19 +176,20 @@
             return [(metadata, asdict(counts)) for metadata, counts in value]
 
     else:
         results = _validation_results(summary)
         to_table = _validation_results_table
         to_serializable = list  # type: ignore[reportGeneralTypeIssues]
 
-    if format == "json":
-        click.echo(json.dumps(to_serializable(results), indent=2))  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
-    else:
-        table = to_table(summary, results)  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
-        console.Console().print(table)
+    match format:
+        case "json":
+            click.echo(json.dumps(to_serializable(results), indent=2))  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
+        case "pretty":
+            table = to_table(summary, results)  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
+            console.Console().print(table)
 
 
 def _ordered_failures(
     summary: _report._Summary,  # type: ignore[reportPrivateUsage]
 ) -> Iterable[tuple[tuple[str, str], _report.Count]]:
     counts = (
         (
@@ -464,15 +462,15 @@
     """
     Retrieve a particular implementation (harness)'s metadata.
     """
     exit_code = asyncio.run(_info(**kwargs))
     context.exit(exit_code)
 
 
-async def _info(image_names: list[str], format: str):
+async def _info(image_names: list[str], format: _F):
     exit_code = 0
     async with _start(
         image_names=image_names,
         make_validator=validator_for_dialect,
         reporter=_report.Reporter(),
     ) as starting:
         for each in asyncio.as_completed(starting):
@@ -499,23 +497,25 @@
                         kv[0] != "language",
                         kv[0] != "version",
                         kv[0] == "dialects",
                         kv[0],
                     ),
                 )
             }
-            if format == "json":
-                click.echo(json.dumps(metadata, indent=2))
-            else:
-                click.echo(
-                    "\n".join(
-                        f"{k}: {json.dumps(v, indent=2)}"
-                        for k, v in metadata.items()
-                    ),
-                )
+
+            match format:
+                case "json":
+                    click.echo(json.dumps(metadata, indent=2))
+                case "pretty":
+                    click.echo(
+                        "\n".join(
+                            f"{k}: {json.dumps(v, indent=2)}"
+                            for k, v in metadata.items()
+                        ),
+                    )
     return exit_code
 
 
 @main.command()
 @click.pass_context
 @FORMAT
 @IMPLEMENTATION
@@ -523,15 +523,15 @@
     """
     Smoke test one or more implementations for basic correctness.
     """
     exit_code = asyncio.run(_smoke(**kwargs))
     context.exit(exit_code)
 
 
-async def _smoke(image_names: list[str], format: str):
+async def _smoke(image_names: list[str], format: _F):
     exit_code = 0
     async with _start(
         image_names=image_names,
         make_validator=validator_for_dialect,
         reporter=_report.Reporter(),
     ) as starting:
         for each in asyncio.as_completed(starting):
@@ -568,42 +568,43 @@
                     description="allow-nothing schema",
                     schema={"$schema": dialect, "not": {}},
                     tests=[
                         Test(description="First", instance=12, valid=False),
                     ],
                 ),
             ]
-            responses: AsyncIterator[tuple[TestCase, ReportableResult]] = (  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
+            responses: AsyncIterator[tuple[TestCase, ReportableResult]] = (
                 (case, await runner.run_case(seq=seq, case=case))
                 for seq, case in enumerate(cases)
             )
 
-            if format == "json":
-                serializable = [
-                    {
-                        "case": case.without_expected_results(),
-                        "response": dict(
-                            errored=response.errored,
-                            failed=response.failed,
-                        ),
-                    }
-                    async for case, response in responses
-                ]
-                click.echo(json.dumps(serializable, indent=2))
-            else:
-                async for case, response in responses:
-                    if response.errored:  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
-                        exit_code |= os.EX_DATAERR
-                        message = "❗ (error)"
-                    elif response.failed:  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
-                        exit_code |= os.EX_DATAERR
-                        message = "✗ (failed)"
-                    else:
-                        message = "✓"
-                    click.echo(f"  {message}: {case.description}")
+            match format:
+                case "json":
+                    serializable = [
+                        {
+                            "case": case.without_expected_results(),
+                            "response": dict(
+                                errored=response.errored,
+                                failed=response.failed,
+                            ),
+                        }
+                        async for case, response in responses
+                    ]
+                    click.echo(json.dumps(serializable, indent=2))
+                case "pretty":
+                    async for case, response in responses:
+                        if response.errored:  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
+                            exit_code |= os.EX_DATAERR
+                            message = "❗ (error)"
+                        elif response.failed:  # type: ignore[reportGeneralTypeIssues]  # noqa: E501
+                            exit_code |= os.EX_DATAERR
+                            message = "✗ (failed)"
+                        else:
+                            message = "✓"
+                        click.echo(f"  {message}: {case.description}")
 
     if exit_code:
         click.echo("\n❌ some failures", file=sys.stderr)
     else:
         click.echo("\n✅ all passed", file=sys.stderr)
 
     return exit_code
```

### Comparing `bowtie_json_schema-2023.6.2/bowtie/_commands.py` & `bowtie_json_schema-2023.6.4/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/bowtie/_core.py` & `bowtie_json_schema-2023.6.4/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/bowtie/_report.py` & `bowtie_json_schema-2023.6.4/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/bowtie/exceptions.py` & `bowtie_json_schema-2023.6.4/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/docs/Makefile` & `bowtie_json_schema-2023.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/docs/cli.rst` & `bowtie_json_schema-2023.6.4/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/docs/conf.py` & `bowtie_json_schema-2023.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/docs/contributing.rst` & `bowtie_json_schema-2023.6.4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/docs/implementers.rst` & `bowtie_json_schema-2023.6.4/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/docs/index.rst` & `bowtie_json_schema-2023.6.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/docs/requirements.txt` & `bowtie_json_schema-2023.6.4/docs/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     #   mdit-py-plugins
     #   rich
     #   textual
 markupsafe==2.1.3
     # via jinja2
 matplotlib==3.7.1
     # via sphinxext-opengraph
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.0
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
```

### Comparing `bowtie_json_schema-2023.6.2/docs/_static/dreamed.png` & `bowtie_json_schema-2023.6.4/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/tests/test_integration.py` & `bowtie_json_schema-2023.6.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.6.4/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.6.4/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.6.4/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2023.6.4/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.6.4/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.6.4/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/.gitignore` & `bowtie_json_schema-2023.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/LICENSE` & `bowtie_json_schema-2023.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/README.rst` & `bowtie_json_schema-2023.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.6.2/pyproject.toml` & `bowtie_json_schema-2023.6.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [tool.hatch.build.force-include]
 "bowtie/schemas/io-schema.json" = "bowtie/schemas/io-schema.json"
 "bowtie/templates/" = "bowtie/templates/"
 
 [project]
 name = "bowtie-json-schema"
 description = "A meta-validator for the JSON Schema specification."
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 readme = "README.rst"
 license = {text = "MIT"}
 keywords = [
     "validation",
     "data validation",
     "jsonschema",
     "json",
@@ -33,16 +33,14 @@
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: File Formats :: JSON :: JSON Schema",
 ]
 dynamic = ["version"]
@@ -53,15 +51,14 @@
   "click",
   "github3.py",
   "jinja2",
   "jsonschema",
   "rich",
   "structlog",
   "trogon>=0.4.0",
-  "importlib-resources; python_version<'3.9'",
   "typing-extensions; python_version<'3.11'",
 ]
 
 [project.scripts]
 bowtie = "bowtie._cli:main"
 
 [project.urls]
```

### Comparing `bowtie_json_schema-2023.6.2/PKG-INFO` & `bowtie_json_schema-2023.6.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.6.2
+Version: 2023.6.4
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
@@ -13,26 +13,23 @@
 Keywords: data validation,json,json schema,jsonschema,validation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: File Formats :: JSON :: JSON Schema
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Requires-Dist: aiodocker
 Requires-Dist: attrs>=22.2.0
 Requires-Dist: click
 Requires-Dist: github3-py
-Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: jinja2
 Requires-Dist: jsonschema
 Requires-Dist: rich
 Requires-Dist: structlog
 Requires-Dist: trogon>=0.4.0
 Requires-Dist: typing-extensions; python_version < '3.11'
 Description-Content-Type: text/x-rst
```

