# Comparing `tmp/autopub-0.2.2.tar.gz` & `tmp/autopub-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopub-0.2.2.tar", max compression
+gzip compressed data, was "autopub-0.3.0.tar", max compression
```

## Comparing `autopub-0.2.2.tar` & `autopub-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
--rw-r--r--   0        0        0    34523 2019-07-11 19:17:24.449879 autopub-0.2.2/LICENSE
--rw-r--r--   0        0        0     2130 2021-10-05 12:00:09.259692 autopub-0.2.2/README.md
--rw-r--r--   0        0        0        0 2019-07-11 19:29:37.040445 autopub-0.2.2/autopub/__init__.py
--rw-r--r--   0        0        0     1908 2019-07-25 14:52:50.309382 autopub-0.2.2/autopub/autopub.py
--rw-r--r--   0        0        0     4789 2021-10-12 09:45:58.106046 autopub-0.2.2/autopub/base.py
--rw-r--r--   0        0        0      302 2019-07-25 14:52:50.314506 autopub-0.2.2/autopub/build_release.py
--rw-r--r--   0        0        0      446 2020-02-27 14:02:17.101174 autopub-0.2.2/autopub/check_release.py
--rw-r--r--   0        0        0      680 2019-07-22 06:03:32.726529 autopub-0.2.2/autopub/commit_release.py
--rw-r--r--   0        0        0     1558 2022-05-26 12:08:00.514360 autopub-0.2.2/autopub/create_github_release.py
--rw-r--r--   0        0        0      447 2019-07-25 14:52:50.318367 autopub-0.2.2/autopub/deploy_release.py
--rw-r--r--   0        0        0     2466 2021-10-05 07:24:21.006191 autopub-0.2.2/autopub/github_contributor.py
--rw-r--r--   0        0        0     3322 2020-12-07 14:14:04.830613 autopub-0.2.2/autopub/prepare_release copy.py
--rw-r--r--   0        0        0     2372 2021-02-15 14:15:44.259717 autopub-0.2.2/autopub/prepare_release.py
--rw-r--r--   0        0        0      488 2019-08-23 16:06:42.335137 autopub-0.2.2/autopub/publish_release.py
--rw-r--r--   0        0        0     1594 2022-06-22 06:49:16.156548 autopub-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 autopub-0.2.2/setup.py
--rw-r--r--   0        0        0     3509 1970-01-01 00:00:00.000000 autopub-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-07 19:38:11.762968 autopub-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2128 2023-06-07 19:38:11.762968 autopub-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 19:38:11.762968 autopub-0.3.0/autopub/__init__.py
+-rw-r--r--   0        0        0     1908 2023-06-07 19:38:11.762968 autopub-0.3.0/autopub/autopub.py
+-rw-r--r--   0        0        0     4794 2023-06-07 19:38:11.762968 autopub-0.3.0/autopub/base.py
+-rw-r--r--   0        0        0      361 2023-06-07 19:38:11.762968 autopub-0.3.0/autopub/build_release.py
+-rw-r--r--   0        0        0      641 2023-06-07 19:38:11.762968 autopub-0.3.0/autopub/check_release.py
+-rw-r--r--   0        0        0      680 2023-06-07 19:38:11.762968 autopub-0.3.0/autopub/commit_release.py
+-rw-r--r--   0        0        0     1558 2023-06-07 19:38:11.762968 autopub-0.3.0/autopub/create_github_release.py
+-rw-r--r--   0        0        0      447 2023-06-07 19:38:11.762968 autopub-0.3.0/autopub/deploy_release.py
+-rw-r--r--   0        0        0     2466 2023-06-07 19:38:11.762968 autopub-0.3.0/autopub/github_contributor.py
+-rw-r--r--   0        0        0     2537 2023-06-07 19:38:11.762968 autopub-0.3.0/autopub/prepare_release.py
+-rw-r--r--   0        0        0      374 2023-06-07 19:38:11.762968 autopub-0.3.0/autopub/publish_release.py
+-rw-r--r--   0        0        0     1649 2023-06-07 19:38:30.659803 autopub-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3629 1970-01-01 00:00:00.000000 autopub-0.3.0/PKG-INFO
```

### Comparing `autopub-0.2.2/LICENSE` & `autopub-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autopub-0.2.2/README.md` & `autopub-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![Build Status](https://img.shields.io/circleci/build/github/autopub/autopub)](https://circleci.com/gh/autopub/autopub) [![PyPI Version](https://img.shields.io/pypi/v/autopub)](https://pypi.org/project/autopub/)
 
 AutoPub enables project maintainers to release new package versions to PyPI by merging pull requests.
 
 ## Environment
 
-AutoPub is intended for use with continuous integration (CI) systems such as [GitHub Actions][], [CircleCI][], or [Travis CI][]. Projects used with AutoPub can be published via [Poetry][] or [setuptools][]. Contributions that add support for other CI and build systems are welcome.
+AutoPub is intended for use with continuous integration (CI) systems such as [GitHub Actions][], [CircleCI][], or [Travis CI][]. Projects used with AutoPub are built via [build][] and published via [Twine][]. Contributions that add support for other CI and build systems are welcome.
 
 ## Configuration
 
 AutoPub settings can be configured via the `[tool.autopub]` table in the target project’s `pyproject.toml` file. Required settings include Git username and email address:
 
 ```toml
 [tool.autopub]
@@ -46,9 +46,9 @@
 
 * `autopub deploy`: Run `prepare`, `build`, `commit`, `githubrelease`, and `publish` in one invocation.
 
 
 [GitHub Actions]: https://github.com/features/actions
 [CircleCI]: https://circleci.com
 [Travis CI]: https://travis-ci.org
-[Poetry]: https://poetry.eustace.io
-[setuptools]: https://setuptools.readthedocs.io/
+[build]: https://pypa-build.readthedocs.io
+[Twine]: https://twine.readthedocs.io/
```

### Comparing `autopub-0.2.2/autopub/autopub.py` & `autopub-0.3.0/autopub/autopub.py`

 * *Files identical despite different names*

### Comparing `autopub-0.2.2/autopub/base.py` & `autopub-0.3.0/autopub/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import re
 import subprocess
-
+import sys
 from pathlib import Path
+
 from tomlkit import parse
 
 
 def dict_get(_dict, keys, default=None):
     """Query nested dictionary with list of keys, returning None if not found."""
     for key in keys:
         if isinstance(_dict, dict):
@@ -19,15 +20,15 @@
 # Determine CI/CD environment
 
 if os.environ.get("CIRCLECI"):
     CI_SYSTEM = "circleci"
     CIRCLE_PROJECT_USERNAME = os.environ.get("CIRCLE_PROJECT_USERNAME")
     CIRCLE_PROJECT_REPONAME = os.environ.get("CIRCLE_PROJECT_REPONAME")
     REPO_SLUG = f"{CIRCLE_PROJECT_USERNAME}/{CIRCLE_PROJECT_REPONAME}"
-elif os.environ.get("GITHUB_WORKFLOW"):
+elif os.environ.get("GITHUB_ACTIONS") == "true":
     CI_SYSTEM = "github"
     REPO_SLUG = os.environ.get("GITHUB_REPOSITORY")
 elif os.environ.get("TRAVIS"):
     CI_SYSTEM = "travis"
     REPO_SLUG = os.environ.get("TRAVIS_REPO_SLUG")
 else:
     CI_SYSTEM = os.environ.get("CI_SYSTEM", None)
@@ -50,24 +51,28 @@
 PYPROJECT_FILE = ROOT / PYPROJECT_FILE_NAME
 
 # Retrieve configuration from pyproject file
 
 if os.path.exists(PYPROJECT_FILE):
     config = parse(open(PYPROJECT_FILE).read())
 else:
-    raise SystemExit(f"Could not find pyproject file at: {PYPROJECT_FILE}")
+    print(f"Could not find pyproject file at: {PYPROJECT_FILE}")
+    sys.exit(1)
 
 PROJECT_NAME = dict_get(config, ["tool", "autopub", "project-name"])
 if not PROJECT_NAME:
     PROJECT_NAME = dict_get(config, ["tool", "poetry", "name"])
 if not PROJECT_NAME:
-    raise SystemExit(
+    PROJECT_NAME = dict_get(config, ["project", "name"])
+if not PROJECT_NAME:
+    print(
         "Could not determine project name. Under the pyproject file's "
         '[tool.autopub] header, add:\nproject-name = "YourProjectName"'
     )
+    sys.exit(1)
 
 RELEASE_FILE_NAME = dict_get(
     config, ["tool", "autopub", "release-file"], default="RELEASE.md"
 )
 RELEASE_FILE = ROOT / RELEASE_FILE_NAME
 
 CHANGELOG_FILE_NAME = dict_get(
@@ -82,78 +87,74 @@
 VERSION_HEADER = dict_get(config, ["tool", "autopub", "version-header"], default="-")
 VERSION_STRINGS = dict_get(config, ["tool", "autopub", "version-strings"], default=[])
 
 TAG_PREFIX = dict_get(config, ["tool", "autopub", "tag-prefix"], default="")
 
 PYPI_URL = dict_get(config, ["tool", "autopub", "pypi-url"])
 
-BUILD_SYSTEM = dict_get(config, ["tool", "autopub", "build-system"])
-if not BUILD_SYSTEM:
-    build_requires = dict_get(config, ["build-system", "requires"])
-    if "poetry" in build_requires:
-        BUILD_SYSTEM = "poetry"
-    elif "setuptools" in build_requires:
-        BUILD_SYSTEM = "setuptools"
-
 # Git configuration
 
 GIT_USERNAME = dict_get(config, ["tool", "autopub", "git-username"])
 GIT_EMAIL = dict_get(config, ["tool", "autopub", "git-email"])
 
 # GitHub
 
 GITHUB_TOKEN = os.environ.get("GITHUB_TOKEN", None)
 APPEND_GITHUB_CONTRIBUTOR = dict_get(
     config, ["tool", "autopub", "append-github-contributor"], False
 )
 
 
-def run_process(popenargs, encoding="utf-8"):
-    return subprocess.check_output(popenargs).decode(encoding).strip()
+def run_process(popenargs, encoding="utf-8", env=None):
+    if env is not None:
+        env = {**os.environ, **env}
+    try:
+        return subprocess.check_output(popenargs, encoding=encoding, env=env).strip()
+    except subprocess.CalledProcessError as e:
+        print(e.output, file=sys.stderr)
+        sys.exit(1)
 
 
 def git(popenargs):
     # Do not decode ASCII for commit messages so emoji are preserved
     return subprocess.check_output(["git", *popenargs])
 
 
 def check_exit_code(popenargs):
     return subprocess.call(popenargs, shell=True)
 
 
 def get_project_version():
-    VERSION_REGEX = re.compile(r"^version\s*=\s*\"(?P<version>\d+\.\d+\.\d+)\"$")
-
-    with open(PYPROJECT_FILE) as f:
-        for line in f:
-            match = VERSION_REGEX.match(line)
-
-            if match:
-                return match.group("version")
-
-    return None
+    # Backwards compat: Try poetry first and then fall "back" to standards
+    version = dict_get(config, ["tool", "poetry", "version"])
+    if version is None:
+        return dict_get(config, ["project", "version"])
+    else:
+        return version
 
 
 def get_release_info():
     RELEASE_TYPE_REGEX = re.compile(r"^[Rr]elease [Tt]ype: (major|minor|patch)$")
 
     with open(RELEASE_FILE, "r") as f:
         line = f.readline()
         match = RELEASE_TYPE_REGEX.match(line)
 
         if not match:
-            raise SystemExit(
+            print(
                 "The RELEASE file should start with 'Release type' and "
                 "specify one of the following values: major, minor, or patch."
             )
+            sys.exit(1)
 
         type_ = match.group(1)
         changelog = "".join([l for l in f.readlines()]).strip()
 
     return type_, changelog
 
 
 def configure_git():
     if not GIT_USERNAME or not GIT_EMAIL:
-        raise SystemExit("git-username and git-email must be defined in the pyproject file")
+        print("git-username and git-email must be defined in the pyproject file")
+        sys.exit(1)
     git(["config", "user.name", GIT_USERNAME])
     git(["config", "user.email", GIT_EMAIL])
```

### Comparing `autopub-0.2.2/autopub/commit_release.py` & `autopub-0.3.0/autopub/commit_release.py`

 * *Files identical despite different names*

### Comparing `autopub-0.2.2/autopub/create_github_release.py` & `autopub-0.3.0/autopub/create_github_release.py`

 * *Files identical despite different names*

### Comparing `autopub-0.2.2/autopub/github_contributor.py` & `autopub-0.3.0/autopub/github_contributor.py`

 * *Files identical despite different names*

### Comparing `autopub-0.2.2/autopub/prepare_release copy.py` & `autopub-0.3.0/autopub/prepare_release.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,52 +2,29 @@
 import re
 import sys
 
 sys.path.append(os.path.dirname(__file__))  # noqa
 
 from datetime import datetime
 
+import tomlkit
 from base import (
-    configure_git,
-    get_release_info,
-    run_process,
     CHANGELOG_FILE,
     CHANGELOG_HEADER,
+    PYPROJECT_FILE,
     ROOT,
     VERSION_HEADER,
     VERSION_STRINGS,
+    configure_git,
+    dict_get,
+    get_project_version,
+    get_release_info,
 )
-
-
-def find_existing_changelog_files():
-    changelogs = []
-    changelog_paths = [ROOT, ROOT / "docs"]
-    changelog_names = ["CHANGELOG", "CHANGES", "HISTORY"]
-    changelog_extensions = ["", ".md", ".markdown", ".mdown", ".mkd", ".rst", ".txt"]
-    for path in changelog_paths:
-        for name in changelog_names:
-            for ext in changelog_extensions:
-                changelog = path / f"{name}{ext}"
-                if changelog.is_file():
-                    changelogs.append(changelog)
-    if len(changelogs) > 0:
-        print(f"Specified changelog file not found: {CHANGELOG_FILE}")
-        print("Maybe set 'changelog-file' setting to discovered existing file:\n")
-        for changelog in changelogs:
-            print(f"{changelog}\n")
-        sys.exit(1)
-
-
-def validate_release():
-    if not CHANGELOG_FILE.is_file():
-        find_existing_changelog_files()
-
-    if not os.environ.get("PYPI_PASSWORD"):
-        print("PYPI_PASSWORD environment variable is not set.")
-        sys.exit(1)
+from dunamai import Version
+from github_contributor import append_github_contributor
 
 
 def update_version_strings(file_path, new_version):
     version_regex = re.compile(r"(^_*?version_*?\s*=\s*['\"])(\d+\.\d+\.\d+)", re.M)
     with open(file_path, "r+") as f:
         content = f.read()
         f.seek(0)
@@ -59,30 +36,31 @@
             )
         )
         f.truncate()
 
 
 def prepare_release():
     configure_git()
-    validate_release()
 
-    POETRY_DUMP_VERSION_OUTPUT = re.compile(
-        r"Bumping version from \d+\.\d+\.\d+ to (?P<version>\d+\.\d+\.\d+)"
-    )
+    type_, release_changelog = get_release_info()
 
-    release_type, release_changelog = get_release_info()
+    version = Version(get_project_version())
+    new_version = version.bump({"major": 0, "minor": 1, "patch": 2}[type_]).serialize()
 
-    output = run_process(["poetry", "version", release_type])
-    version_match = POETRY_DUMP_VERSION_OUTPUT.match(output)
+    with open(PYPROJECT_FILE, "r") as f:
+        config = tomlkit.load(f)
 
-    if not version_match:
-        print("Unable to bump the project version using Poetry")
-        sys.exit(1)
+    poetry = dict_get(config, ["tool", "poetry", "version"])
+    if poetry:
+        config["tool"]["poetry"]["version"] = new_version
+    else:
+        config["project"]["version"] = new_version
 
-    new_version = version_match.group("version")
+    with open(PYPROJECT_FILE, "w") as f:
+        config = tomlkit.dump(config, f)
 
     if VERSION_STRINGS:
         for version_file in VERSION_STRINGS:
             file_path = ROOT / version_file
             update_version_strings(file_path, new_version)
 
     current_date = datetime.utcnow().strftime("%Y-%m-%d")
@@ -110,10 +88,11 @@
 
         new_version_header = f"{new_version} - {current_date}"
 
         f.write(f"\n{new_version_header}\n")
         f.write(f"{VERSION_HEADER * len(new_version_header)}\n\n")
 
         f.write(release_changelog)
+        append_github_contributor(f)
         f.write("\n")
 
         f.write("".join(old_changelog_data))
```

### Comparing `autopub-0.2.2/pyproject.toml` & `autopub-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopub"
-version = "0.2.2"
+version = "0.3.0"
 description = "Automatic package release upon pull request merge"
 authors = ["Justin Mayer <entroP@gmail.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 keywords = ["automatic", "packaging", "publish", "release", "version"]
 repository = "https://github.com/autopub/autopub"
 
@@ -18,18 +18,21 @@
     "Topic :: System :: Systems Administration",
 ]
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/autopub/autopub/issues"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 tomlkit = ">= 0.5, < 2.0"
-githubrelease = {version = "^1.5.8", optional = true}
+githubrelease = {version = "^1.5.9", optional = true}
 httpx = {version = "=0.16.1", optional = true}
+build = "^0.10.0"
+twine = "^4.0.2"
+dunamai = "^1.17.0"
 
 [tool.poetry.dev-dependencies]
 githubrelease = "^1.5"
 
 # Tasks
 invoke = "^1.6"
```

### Comparing `autopub-0.2.2/PKG-INFO` & `autopub-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: autopub
-Version: 0.2.2
+Version: 0.3.0
 Summary: Automatic package release upon pull request merge
 Home-page: https://github.com/autopub/autopub
 License: AGPL-3.0
 Keywords: automatic,packaging,publish,release,version
 Author: Justin Mayer
 Author-email: entroP@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: System :: Systems Administration
 Provides-Extra: github
-Requires-Dist: githubrelease (>=1.5.8,<2.0.0); extra == "github"
-Requires-Dist: httpx (==0.16.1); extra == "github"
+Requires-Dist: build (>=0.10.0,<0.11.0)
+Requires-Dist: dunamai (>=1.17.0,<2.0.0)
+Requires-Dist: githubrelease (>=1.5.9,<2.0.0) ; extra == "github"
+Requires-Dist: httpx (==0.16.1) ; extra == "github"
 Requires-Dist: tomlkit (>=0.5,<2.0)
+Requires-Dist: twine (>=4.0.2,<5.0.0)
 Project-URL: Issue Tracker, https://github.com/autopub/autopub/issues
 Project-URL: Repository, https://github.com/autopub/autopub
 Description-Content-Type: text/markdown
 
 # AutoPub
 
 [![Build Status](https://img.shields.io/circleci/build/github/autopub/autopub)](https://circleci.com/gh/autopub/autopub) [![PyPI Version](https://img.shields.io/pypi/v/autopub)](https://pypi.org/project/autopub/)
 
 AutoPub enables project maintainers to release new package versions to PyPI by merging pull requests.
 
 ## Environment
 
-AutoPub is intended for use with continuous integration (CI) systems such as [GitHub Actions][], [CircleCI][], or [Travis CI][]. Projects used with AutoPub can be published via [Poetry][] or [setuptools][]. Contributions that add support for other CI and build systems are welcome.
+AutoPub is intended for use with continuous integration (CI) systems such as [GitHub Actions][], [CircleCI][], or [Travis CI][]. Projects used with AutoPub are built via [build][] and published via [Twine][]. Contributions that add support for other CI and build systems are welcome.
 
 ## Configuration
 
 AutoPub settings can be configured via the `[tool.autopub]` table in the target project’s `pyproject.toml` file. Required settings include Git username and email address:
 
 ```toml
 [tool.autopub]
@@ -78,10 +81,9 @@
 
 * `autopub deploy`: Run `prepare`, `build`, `commit`, `githubrelease`, and `publish` in one invocation.
 
 
 [GitHub Actions]: https://github.com/features/actions
 [CircleCI]: https://circleci.com
 [Travis CI]: https://travis-ci.org
-[Poetry]: https://poetry.eustace.io
-[setuptools]: https://setuptools.readthedocs.io/
-
+[build]: https://pypa-build.readthedocs.io
+[Twine]: https://twine.readthedocs.io/
```

