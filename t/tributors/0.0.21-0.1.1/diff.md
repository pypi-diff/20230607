# Comparing `tmp/tributors-0.0.21.tar.gz` & `tmp/tributors-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tributors-0.0.21.tar", last modified: Sun Mar 27 19:15:43 2022, max compression
+gzip compressed data, was "tributors-0.1.1.tar", last modified: Wed Jun  7 13:53:40 2023, max compression
```

## Comparing `tributors-0.0.21.tar` & `tributors-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-03-27 19:15:43.484567 tributors-0.0.21/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11357 2022-03-15 23:05:54.000000 tributors-0.0.21/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      140 2022-03-15 23:05:54.000000 tributors-0.0.21/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4494 2022-03-27 19:15:43.484567 tributors-0.0.21/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3042 2022-03-15 23:05:54.000000 tributors-0.0.21/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      112 2022-03-27 19:15:43.484567 tributors-0.0.21/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3862 2022-03-15 23:05:54.000000 tributors-0.0.21/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-03-27 19:15:43.480567 tributors-0.0.21/tributors/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-03-27 19:15:43.480567 tributors-0.0.21/tributors/client/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4853 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/client/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1630 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/client/init.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1490 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/client/lookup.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2003 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/client/update.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      910 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/client/utils.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      205 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/logger.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-03-27 19:15:43.480567 tributors-0.0.21/tributors/main/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5736 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/main/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8150 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/main/github.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7529 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/main/orcid.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-03-27 19:15:43.484567 tributors-0.0.21/tributors/main/parsers/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1694 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/main/parsers/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8209 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/main/parsers/allcontrib.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5097 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/main/parsers/base.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7401 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/main/parsers/codemeta.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2377 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/main/parsers/mailmap.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9360 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/main/parsers/zenodo.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-03-27 19:15:43.484567 tributors-0.0.21/tributors/utils/
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)     5178 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/utils/command.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2144 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/utils/file.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1670 2022-03-15 23:05:54.000000 tributors-0.0.21/tributors/utils/prompt.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      864 2022-03-27 19:15:40.000000 tributors-0.0.21/tributors/version.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-03-27 19:15:43.480567 tributors-0.0.21/tributors.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4494 2022-03-27 19:15:43.000000 tributors-0.0.21/tributors.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      835 2022-03-27 19:15:43.000000 tributors-0.0.21/tributors.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2022-03-27 19:15:43.000000 tributors-0.0.21/tributors.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2022-03-27 19:15:43.000000 tributors-0.0.21/tributors.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2022-03-27 19:15:43.000000 tributors-0.0.21/tributors.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       89 2022-03-27 19:15:43.000000 tributors-0.0.21/tributors.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2022-03-27 19:15:43.000000 tributors-0.0.21/tributors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:53:40.831447 tributors-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 13:53:13.000000 tributors-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-07 13:53:13.000000 tributors-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-07 13:53:40.831447 tributors-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-07 13:53:13.000000 tributors-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 13:53:40.831447 tributors-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-07 13:53:13.000000 tributors-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:53:40.827447 tributors-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-07 13:53:13.000000 tributors-0.1.1/tests/test_mailmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-07 13:53:13.000000 tributors-0.1.1/tests/test_orcid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-07 13:53:13.000000 tributors-0.1.1/tests/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:53:40.827447 tributors-0.1.1/tributors/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:53:40.827447 tributors-0.1.1/tributors/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/client/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/client/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/client/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:53:40.831447 tributors-0.1.1/tributors/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/main/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/main/orcid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:53:40.831447 tributors-0.1.1/tributors/main/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/main/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/main/parsers/allcontrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/main/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/main/parsers/codemeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/main/parsers/mailmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/main/parsers/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:53:40.831447 tributors-0.1.1/tributors/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5177 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-07 13:53:13.000000 tributors-0.1.1/tributors/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-07 13:53:29.000000 tributors-0.1.1/tributors/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:53:40.827447 tributors-0.1.1/tributors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-07 13:53:40.000000 tributors-0.1.1/tributors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-07 13:53:40.000000 tributors-0.1.1/tributors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:53:40.000000 tributors-0.1.1/tributors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 13:53:40.000000 tributors-0.1.1/tributors.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:53:40.000000 tributors-0.1.1/tributors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-07 13:53:40.000000 tributors-0.1.1/tributors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 13:53:40.000000 tributors-0.1.1/tributors.egg-info/top_level.txt
```

### Comparing `tributors-0.0.21/LICENSE` & `tributors-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tributors-0.0.21/PKG-INFO` & `tributors-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,18 @@
 Metadata-Version: 2.1
 Name: tributors
-Version: 0.0.21
+Version: 0.1.1
 Summary: give tribute to your repository contributors.
 Home-page: http://www.github.com/con/tributors
 Author: Vanessa Sochat
 Author-email: vsochat@stanford.edu
 Maintainer: Vanessa Sochat
 Maintainer-email: vsochat@stanford.edu
 License: LICENSE
-Description: # tributors
-        
-        ![docs/assets/img/logo.png](https://raw.githubusercontent.com/con/tributors/master/docs/assets/img/logo.png)
-        
-        <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-        [![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
-        <!-- ALL-CONTRIBUTORS-BADGE:END -->
-        
-        [Documentation](https://con.github.io/tributors/)
-        
-        ## What is tributors?
-        
-        Tributors is a Python library and GitHub action that helps you to pay tribute to your
-        contributors. Tribute interacts with several well-known repository metadata files:
-        
-         - [all-contributors](https://github.com/all-contributors)
-         - [Zenodo](https://zenodo.org)
-         - [CodeMeta](https://codemeta.github.io/)
-        
-        Each of the services above allows you to generate some kind of metadata file
-        that has one or more repository contributors. This file typically needs to be
-        generated and updated manually, and this is where tributors comes in to help!
-        Tributors will allow you to programatically create and update these files.
-        By way of using a shared cache, a `.tributors` file that can store common
-        identifiers, it becomes easy to update several of these metadata files at once.
-        You can set criteria such as a threshold for contributions to add a contributor,
-        export an Orcid ID token to ensure that you have Orcid Ids where needed,
-        or use an interactive mode to make decisions as you go.
-        
-        ## How does it work?
-        
-        Tributors uses the GitHub API, Zenodo API, and Orcid API to look up shared identifiers
-        for common metadata services like all contributors, Zenodo, and CodeMeta. The
-        tool is available for local or container usage, and as a GitHub Action (see the [examples](examples) folder).
-        See the full [documentation](https://con.github.io/tributors/) for getting started.
-        
-        
-        ## Contributors
-        
-        <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-        <!-- prettier-ignore-start -->
-        <!-- markdownlint-disable -->
-        <table>
-          <tr>
-            <td align="center"><a href="www.onerussian.com"><img src="https://avatars3.githubusercontent.com/u/39889?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Yaroslav Halchenko</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=yarikoptic" title="Code">💻</a> <a href="https://github.com/con/tributors/commits?author=yarikoptic" title="Documentation">📖</a></td>
-            <td align="center"><a href="https://vsoch.github.io"><img src="https://avatars0.githubusercontent.com/u/814322?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Vanessasaurus</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=vsoch" title="Code">💻</a></td>
-            <td align="center"><a href="https://github.com/pgrimaud"><img src="https://avatars1.githubusercontent.com/u/1866496?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pierre Grimaud</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=pgrimaud" title="Code">💻</a></td>
-          </tr>
-        </table>
-        
-        <!-- markdownlint-enable -->
-        <!-- prettier-ignore-end -->
-        <!-- ALL-CONTRIBUTORS-LIST:END -->
-        
 Keywords: contributions,tributes
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
@@ -75,7 +20,67 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: codemeta
+License-File: LICENSE
+
+# tributors
+
+![docs/assets/img/logo.png](https://raw.githubusercontent.com/con/tributors/master/docs/assets/img/logo.png)
+
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
+
+[Documentation](https://con.github.io/tributors/)
+
+## What is tributors?
+
+Tributors is a Python library and GitHub action that helps you to pay tribute to your
+contributors. Tribute interacts with several well-known repository metadata files:
+
+ - [all-contributors](https://github.com/all-contributors)
+ - [Zenodo](https://zenodo.org)
+ - [CodeMeta](https://codemeta.github.io/)
+
+Each of the services above allows you to generate some kind of metadata file
+that has one or more repository contributors. This file typically needs to be
+generated and updated manually, and this is where tributors comes in to help!
+Tributors will allow you to programmatically create and update these files.
+By way of using a shared cache, a `.tributors` file that can store common
+identifiers, it becomes easy to update several of these metadata files at once.
+You can set criteria such as a threshold for contributions to add a contributor,
+export an Orcid ID token to ensure that you have Orcid Ids where needed,
+or use an interactive mode to make decisions as you go.
+
+## How does it work?
+
+Tributors uses the GitHub API, Zenodo API, and Orcid API to look up shared identifiers
+for common metadata services like all contributors, Zenodo, and CodeMeta. The
+tool is available for local or container usage, and as a GitHub Action (see the [examples](examples) folder).
+See the full [documentation](https://con.github.io/tributors/) for getting started.
+
+
+## Contributors
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="www.onerussian.com"><img src="https://avatars3.githubusercontent.com/u/39889?v=4?s=100" width="100px;" alt="Yaroslav Halchenko"/><br /><sub><b>Yaroslav Halchenko</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=yarikoptic" title="Code">💻</a> <a href="https://github.com/con/tributors/commits?author=yarikoptic" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://vsoch.github.io"><img src="https://avatars0.githubusercontent.com/u/814322?v=4?s=100" width="100px;" alt="Vanessasaurus"/><br /><sub><b>Vanessasaurus</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=vsoch" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pgrimaud"><img src="https://avatars1.githubusercontent.com/u/1866496?v=4?s=100" width="100px;" alt="Pierre Grimaud"/><br /><sub><b>Pierre Grimaud</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=pgrimaud" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/vuillaut"><img src="https://avatars.githubusercontent.com/u/4263646?v=4?s=100" width="100px;" alt="vuillaut"/><br /><sub><b>vuillaut</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=vuillaut" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jwodder"><img src="https://avatars.githubusercontent.com/u/98207?v=4?s=100" width="100px;" alt="jwodder"/><br /><sub><b>jwodder</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=jwodder" title="Code">💻</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,41 +1,40 @@
-Metadata-Version: 2.1 Name: tributors Version: 0.0.21 Summary: give tribute to
+Metadata-Version: 2.1 Name: tributors Version: 0.1.1 Summary: give tribute to
 your repository contributors. Home-page: http://www.github.com/con/tributors
 Author: Vanessa Sochat Author-email: vsochat@stanford.edu Maintainer: Vanessa
-Sochat Maintainer-email: vsochat@stanford.edu License: LICENSE Description: #
-tributors ![docs/assets/img/logo.png](https://raw.githubusercontent.com/con/
-tributors/master/docs/assets/img/logo.png)  [![All Contributors](https://
-img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)]
-(#contributors-)  [Documentation](https://con.github.io/tributors/) ## What is
-tributors? Tributors is a Python library and GitHub action that helps you to
-pay tribute to your contributors. Tribute interacts with several well-known
-repository metadata files: - [all-contributors](https://github.com/all-
-contributors) - [Zenodo](https://zenodo.org) - [CodeMeta](https://
-codemeta.github.io/) Each of the services above allows you to generate some
-kind of metadata file that has one or more repository contributors. This file
-typically needs to be generated and updated manually, and this is where
-tributors comes in to help! Tributors will allow you to programatically create
-and update these files. By way of using a shared cache, a `.tributors` file
-that can store common identifiers, it becomes easy to update several of these
-metadata files at once. You can set criteria such as a threshold for
-contributions to add a contributor, export an Orcid ID token to ensure that you
-have Orcid Ids where needed, or use an interactive mode to make decisions as
-you go. ## How does it work? Tributors uses the GitHub API, Zenodo API, and
-Orcid API to look up shared identifiers for common metadata services like all
-contributors, Zenodo, and CodeMeta. The tool is available for local or
-container usage, and as a GitHub Action (see the [examples](examples) folder).
-See the full [documentation](https://con.github.io/tributors/) for getting
-started. ## Contributors
+Sochat Maintainer-email: vsochat@stanford.edu License: LICENSE Keywords:
+contributions,tributes Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: Mozilla Public License 2.0 (MPL 2.0) Classifier: Topic :: Software
+Development Classifier: Topic :: Scientific/Engineering Classifier: Natural
+Language :: English Classifier: Operating System :: Unix Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Description-Content-Type: text/markdown Provides-Extra: all
+Provides-Extra: codemeta License-File: LICENSE # tributors ![docs/assets/img/
+logo.png](https://raw.githubusercontent.com/con/tributors/master/docs/assets/
+img/logo.png)  [![All Contributors](https://img.shields.io/badge/
+all_contributors-5-orange.svg?style=flat-square)](#contributors-)
+[Documentation](https://con.github.io/tributors/) ## What is tributors?
+Tributors is a Python library and GitHub action that helps you to pay tribute
+to your contributors. Tribute interacts with several well-known repository
+metadata files: - [all-contributors](https://github.com/all-contributors) -
+[Zenodo](https://zenodo.org) - [CodeMeta](https://codemeta.github.io/) Each of
+the services above allows you to generate some kind of metadata file that has
+one or more repository contributors. This file typically needs to be generated
+and updated manually, and this is where tributors comes in to help! Tributors
+will allow you to programmatically create and update these files. By way of
+using a shared cache, a `.tributors` file that can store common identifiers, it
+becomes easy to update several of these metadata files at once. You can set
+criteria such as a threshold for contributions to add a contributor, export an
+Orcid ID token to ensure that you have Orcid Ids where needed, or use an
+interactive mode to make decisions as you go. ## How does it work? Tributors
+uses the GitHub API, Zenodo API, and Orcid API to look up shared identifiers
+for common metadata services like all contributors, Zenodo, and CodeMeta. The
+tool is available for local or container usage, and as a GitHub Action (see the
+[examples](examples) folder). See the full [documentation](https://
+con.github.io/tributors/) for getting started. ## Contributors
+[Yaroslav_Halchenko] [Vanessasaurus] [Pierre_Grimaud] [vuillaut] [jwodder]
+ Yaroslav_Halchenko   Vanessasaurus   Pierre_Grimaud   vuillaut   jwodder
+     ð» ð�     ð»         ð»      ð»  ð»
 
-Yaroslav_Halchenko Vanessasaurus Pierre_Grimaud
-
-    ð» ð    ð»       ð»
-   Keywords: contributions,tributes Platform: UNKNOWN Classifier: Intended
-Audience :: Science/Research Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Topic :: Software Development Classifier: Topic :: Scientific/
-Engineering Classifier: Natural Language :: English Classifier: Operating
-System :: Unix Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Description-Content-Type: text/markdown
-Provides-Extra: all Provides-Extra: codemeta
```

### Comparing `tributors-0.0.21/setup.py` & `tributors-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tributors-0.0.21/tributors/client/__init__.py` & `tributors-0.1.1/tributors/client/__init__.py`

 * *Files identical despite different names*

### Comparing `tributors-0.0.21/tributors/client/init.py` & `tributors-0.1.1/tributors/client/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import logging
 import sys
 
 bot = logging.getLogger("github")
 
 
 def main(args, extra):
-
     client = TributorsClient(skip_cache=args.skip_cache)
 
     # Parse extra arguments
     extra = parse_extra(extra)
     extra["--interactive"] = args.interactive
 
     # Skip users, if a space separated list is defined
```

### Comparing `tributors-0.0.21/tributors/client/lookup.py` & `tributors-0.1.1/tributors/client/lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from tributors.main import TributorsClient
 from .utils import parse_extra
 import os
 import sys
 
 
 def main(args, extra):
-
     client = TributorsClient(skip_cache=args.skip_cache)
 
     # Parse extra arguments
     extra = parse_extra(extra)
 
     # Start with user provided parsers
     resources = args.files
```

### Comparing `tributors-0.0.21/tributors/client/update.py` & `tributors-0.1.1/tributors/client/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from tributors.main import TributorsClient
 from .utils import parse_extra
 import os
 import sys
 
 
 def main(args, extra):
-
     client = TributorsClient(skip_cache=args.skip_cache)
 
     # Parse extra arguments
     extra = parse_extra(extra)
     extra["--interactive"] = args.interactive
 
     # Start with user provided parsers
```

### Comparing `tributors-0.0.21/tributors/client/utils.py` & `tributors-0.1.1/tributors/client/utils.py`

 * *Files identical despite different names*

### Comparing `tributors-0.0.21/tributors/main/__init__.py` & `tributors-0.1.1/tributors/main/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,14 @@
         as many lookups of unique ids (email, login, orcid) that
         the resource provides
         """
         from_resources = from_resources or ["github"]
         lookups = {"login": set(), "orcid": set(), "email": set(), "name": set()}
 
         for name in from_resources:
-
             # Special case, tributors is just the entire cache
             if name == "tributors":
                 lookups["login"].update(self.cache)
                 lookups["name"].update(
                     {x["name"]: x for _, x in self.cache.items() if "name" in x}
                 )
                 lookups["orcid"].update(
```

### Comparing `tributors-0.0.21/tributors/main/github.py` & `tributors-0.1.1/tributors/main/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     def update_lookup(self):
         """update the .tributors file using GitHub contributors"""
         if not self.skip_users:
             self.skip_users = self.params.get("--skip-users", "").split(" ")
 
         # Iterate through GitHub and update metadata
         for login, contributor in self.contributors.items():
-
             # Don't include bots, and others specified with --skip-user
             if not self.include_contributor(login):
                 continue
 
             # Look up a GitHub username, possibly email and site
             user = get_user(login)
```

### Comparing `tributors-0.0.21/tributors/main/orcid.py` & `tributors-0.1.1/tributors/main/orcid.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 from tributors.utils.file import write_file, get_tmpfile
 from tributors.utils.prompt import choice_prompt
 import logging
 import os
 import requests
+import urllib
 
 bot = logging.getLogger("github")
 
 
 class OrcidIdentifier:
     """A simple class to retrieve an orcid record, and expose needed fields"""
 
@@ -125,16 +126,23 @@
             f"Orcid token exports written to {tmp_file}. "
             "In the future export these variables for headless usage."
         )
 
     return orcid_token
 
 
-def record_search(url, email, interactive=False):
-    """Given a url (with a name or email) do a record search looking for an orcid id"""
+def record_search(url, email, interactive=False, search_type=""):
+    """Given a url (with a name or email) do a record search looking for an orcid id.
+
+    Arguments:
+      - url (str) : url to perform request
+      - email (str) : email, used just for logging
+      - interactive (bool) : if True, ask user if there is more than a single response
+      - search_type (str) : description on what search is based on, used just for logging
+    """
     response = requests.get(url, headers={"Accept": "application/json"})
     if response.status_code != 200:
         return
 
     results = response.json().get("expanded-result", []) or []
 
     if not results:
@@ -143,34 +151,35 @@
     # We found only one matching result
     if len(results) == 1:
         return results[0]["orcid-id"]
 
     # Only stream results to screen in interactive mode
     if not interactive:
         bot.info(
-            f"{email}: found more than 1 result, run with --interactive mode to select."
+            f"{email}: found more than 1 ({len(results)}) result for ORCID search {search_type}, "
+            "run with --interactive mode to select."
         )
         return
 
     # One or more results
     if len(results) > 10:
         bot.warning("Found more than 10 results, will only show top 10.")
 
     print("\n\n%s\n======================================================" % email)
     for idx, r in enumerate(results):
-
         # Limit is ten results, count starting at 0
         idx = idx + 1
         if idx > 10:
             break
 
-        record = "  Name: %s, %s\n  Orcid: %s" % (
+        record = "  Name: %s, %s\n  ORCID: %s (https://orcid.org/%s)" % (
             r["family-names"],
             r["given-names"],
             r["orcid-id"],
+            r["orcid-id"],
         )
         if r["institution-name"]:
             record = "%s\n  Institutions: %s" % (
                 record,
                 ", ".join(r["institution-name"]),
             )
         if r["other-name"]:
@@ -180,16 +189,16 @@
         if not interactive:
             print("%s\n" % record)
         else:
             print("[%s]\n%s\n" % (idx, record))
 
     # If interactive, ask for choice prompt
     if interactive:
-        choices = [str(i) for i, _ in enumerate(results)] + ["s", "S", "skip"]
-        prefix = "1:%s or s to skip" % ("10" if len(results) > 10 else len(results))
+        choices = [str(i) for i, _ in enumerate(results, 1)] + ["s", "S", "skip"]
+        prefix = "1:%s or s to skip" % min(10, len(results))
         choice = choice_prompt(
             "Please enter a choice, or s to skip.",
             choices=choices,
             choice_prefix=prefix,
             multiple=False,
         )
 
@@ -202,44 +211,51 @@
 
 def get_orcid(email, name=None, interactive=False):
     """Get an orcid identifier for a given email or name."""
     # We must have an email OR name
     if not email and not name:
         return
 
+    def extended_search_url(q, *args):
+        """Helper to properly quote args and avoid duplicating URL etc"""
+        url = f"https://pub.orcid.org/v3.0/expanded-search?q={q}"
+        if args:
+            url %= tuple(map(urllib.parse.quote, args))
+        return url
+
     # First look for records based on email
     orcid_id = None
     if email:
-        url = "https://pub.orcid.org/v3.0/expanded-search?q=email:%s" % email
-        orcid_id = record_search(url, email, interactive)
+        url = extended_search_url("email:%s", email)
+        orcid_id = record_search(url, email, interactive, "by email")
 
     # Attempt # 2 will use the first and last name
-    if name is not None and not orcid_id:
-
+    if not orcid_id and name is not None:
         delim = "," if "," in name else " "
         cleaner = "," if delim == " " else " "
 
         parts = name.split(delim)
 
         # No go if only a first or last name
         if len(parts) == 1:
             bot.debug(f"Skipping {name}, first and last are required for search.")
             return orcid_id
 
         last, first = parts[0].strip(cleaner), " ".join(parts[1:]).strip(cleaner)
-        url = "https://pub.orcid.org/v3.0/expanded-search?q=%s+AND+%s" % (first, last)
-        orcid_id = record_search(url, name, interactive)
+        url = extended_search_url("%s+AND+%s", first, last)
+        orcid_id = record_search(url, name, interactive, "by name")
 
         # Attempt # 3 will try removing the middle name
-        if " " in first:
-            url = "https://pub.orcid.org/v3.0/expanded-search?q=%s+AND+%s" % (
+        if not orcid_id and " " in first:
+            url = extended_search_url(
+                "%s+AND+%s",
                 first.split(" ")[0].strip(),
                 last,
             )
-            orcid_id = record_search(url, name, interactive)
+            orcid_id = record_search(url, name, interactive, "by name without middle")
 
-        # Last attempt tries full name
-        if orcid_id is None:
-            url = "https://pub.orcid.org/v3.0/expanded-search?q=%s" % name
-            orcid_id = record_search(url, name, interactive)
+        # Last attempt tries full name "as is"
+        if not orcid_id:
+            url = extended_search_url("%s", name)
+            orcid_id = record_search(url, name, interactive, "full name")
 
     return orcid_id
```

### Comparing `tributors-0.0.21/tributors/main/parsers/__init__.py` & `tributors-0.1.1/tributors/main/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `tributors-0.0.21/tributors/main/parsers/allcontrib.py` & `tributors-0.1.1/tributors/main/parsers/allcontrib.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from tributors.utils.file import write_json
 from .base import ParserBase
 
 bot = logging.getLogger("allcontrib")
 
 
 class AllContribParser(ParserBase):
-
     name = "allcontrib"
 
     # https://allcontributors.org/docs/en/emoji-key
     contribution_types = [
         "audio",
         "ally",
         "bug",
@@ -174,15 +173,14 @@
                     "contributions": [ctype],
                 }
                 self.extras.append(entry)
 
     def update_from_logins(self, logins, ctype):
         """Given a list of logins, update the loaded logins"""
         for login in logins:
-
             # Check against contribution threshold, and not bot
             if not self.include_contributor(login):
                 continue
 
             cache = self.cache.get(login) or {}
             if login in self.login_lookup:
                 entry = self.login_lookup[login]
```

### Comparing `tributors-0.0.21/tributors/main/parsers/base.py` & `tributors-0.1.1/tributors/main/parsers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,14 @@
 
         # If the parser can be used as a resource, use it to update .tributors
         if hasattr(self, "update_lookup") and update_lookup:
             self.update_lookup()
 
         # Then add an Orcid lookup
         for login, entry in self.cache.items():
-
             # If we have an email, and orcid isn't defined
             if "orcid" not in entry:
                 orcid = get_orcid(
                     entry.get("email"), entry.get("name"), interactive=interactive
                 )
                 if orcid:
                     entry["orcid"] = orcid
```

### Comparing `tributors-0.0.21/tributors/main/parsers/codemeta.py` & `tributors-0.1.1/tributors/main/parsers/codemeta.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from tributors.utils.file import write_json
 from .base import ParserBase
 
 bot = logging.getLogger("  codemeta")
 
 
 class CodeMetaParser(ParserBase):
-
     name = "codemeta"
 
     def __init__(self, filename=None, repo=None, params=None, **kwargs):
         filename = filename or "codemeta.json"
         self.data = {}
         super().__init__(filename, repo, params)
 
@@ -59,15 +58,15 @@
         self.data["contributor"] = self.lookup
         if save:
             write_json(self.data, self.filename)
         return self.data
 
     def update_metadata(self):
         """Update codemeta metadata from the repository, if we can."""
-        self.data["keywords"] = self.repo.topics(self.data["keywords"])
+        self.data["keywords"] = self.repo.topics(self.data.get("keywords", []))
         self.data["description"] = self.data.get("description") or self.repo.description
         self.data["codeRepository"] = (
             self.data.get("codeRepository") or self.repo.html_url
         )
         self.data["name"] = self.data.get("name") or self.repo.name
         self.data["issueTracker"] = (
             self.data.get("issueTracker") or self.repo.issues_url
@@ -83,15 +82,14 @@
                 entry = {"@type": "Person", "email": email}
                 self.lookup.append(entry)
 
     def update_from_logins(self, logins):
         """Update codemeta entries from GitHub logins"""
         # Now add contributors using cache (new GitHub contributors) with known email or orcid that isn't present
         for login in logins:
-
             # Check against contribution threshold, and not bot
             if not self.include_contributor(login):
                 continue
 
             cache = self.cache.get(login) or {}
             email = cache.get("email")
             orcid = cache.get("orcid")
@@ -148,15 +146,14 @@
         for login, cache in self.cache.items():
             orcid = cache.get("orcid")
             email = cache.get("email")
 
             # Case 1: double match (unlikely but possible)
             entry = None
             if email in self.email_lookup and orcid in self.orcid_lookup:
-
                 # If they don't point to the same entry, stop
                 if self.email_lookup[email] != self.orcid_lookup[orcid]:
                     bot.warning(
                         "Found email {email} and orcid {orcid} in cache from different entries, skipping."
                     )
                 else:
                     entry = self.email_lookup[email]
@@ -167,15 +164,14 @@
 
             # Case 2: We have a matching email
             elif email in self.email_lookup:
                 entry = self.email_lookup[email]
 
             # If we have a match (entry is defined) use it to update the record
             if entry is not None:
-
                 # Update the name
                 if (
                     "givenName" in entry
                     and "familyName" in entry
                     and "name" not in cache
                 ):
                     cache["name"] = "%s %s" % (entry["givenName"], entry["familyName"])
```

### Comparing `tributors-0.0.21/tributors/main/parsers/mailmap.py` & `tributors-0.1.1/tributors/main/parsers/mailmap.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Copyright (C) 2020 Vanessa Sochat.
+Copyright (C) 2020-2022 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
@@ -15,15 +15,14 @@
 from tributors.utils.file import read_file
 from .base import ParserBase
 
 bot = logging.getLogger("   mailmap")
 
 
 class MailmapParser(ParserBase):
-
     name = "mailmap"
 
     def __init__(self, filename=None, params=None, **kwargs):
         filename = filename or ".mailmap"
         super().__init__(filename=filename, params=params)
 
     def load_data(self):
@@ -34,17 +33,28 @@
             self.filename = self.params.get("--mailmap-file", self.filename)
 
             # Ensure codemeta file already exists
             if not os.path.exists(self.filename):
                 sys.exit("%s does not exist" % self.filename)
 
             for line in read_file(self.filename):
-                name, email = line.split("<")
-                email = email.strip().rstrip(">")
-                self.data[email] = {"name": name.strip()}
+                # keep track of the previous name, in case multiple per line
+                name = None
+
+                # mailmap line can have more than one entry, split by right >
+                for entry in line.strip().split(">"):
+                    if not entry:
+                        continue
+                    new_name, email = map(str.strip, entry.split("<"))
+                    # only the first name matters
+                    if not name and new_name:
+                        name = new_name
+                    if not name:
+                        raise ValueError(f"Could not figure out name in {line!r}")
+                    self.data[email] = {"name": name}
         return self.data
 
     @property
     def email_lookup(self):
         """Return loaded metadata as an email lookup. In this case, this
         is just the entire data.
         """
```

### Comparing `tributors-0.0.21/tributors/main/parsers/zenodo.py` & `tributors-0.1.1/tributors/main/parsers/zenodo.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from .base import ParserBase
 from tributors.main.orcid import get_orcid
 
 bot = logging.getLogger("    zenodo")
 
 
 class ZenodoParser(ParserBase):
-
     name = "zenodo"
 
     def __init__(self, filename=None, repo=None, params=None, **kwargs):
         filename = filename or ".zenodo.json"
         super().__init__(filename, repo, params)
 
     def load_data(self):
@@ -146,15 +145,14 @@
     def update_from_logins(self, logins):
         """Given a list of logins, update the zenodo.json from it. We only
         do this on init when we haven't added /updated logins with
         people's actual names.
         """
         # GitHub contributors are the source of truth
         for login in logins:
-
             # Check against contribution threshold, and not bot
             if not self.include_contributor(login):
                 continue
 
             cache = self.cache.get(login) or {}
             orcid = cache.get("orcid")
             email = cache.get("email")
@@ -205,28 +203,29 @@
         In the case of zenodo, we aren't necessarily aware of GitHub
         login (the current mapping mechanism) so we cannot update the
         cache yet. When orcid is added this might be an option.
         """
         self.load_data()
         bot.info(f"Updating .tributors cache from {self.filename}")
 
-        # We have to update based on orcid
-        lookup = {}
-        for entry in self.data.get("creators", []):
-            if "orcid" in entry:
-                lookup[entry["orcid"]] = entry
+        # We have to update based on (non-degenerate) orcid
+        lookup = {
+            entry["orcid"]: entry
+            for entry in self.data.get("creators", [])
+            if entry.get("orcid")
+        }
 
         # Now loop through cache
-        for login, cache in self.cache.items():
-            if "orcid" in cache and cache["orcid"] in lookup:
+        for login, cached in self.cache.items():
+            orcid = cached.get("orcid")
+            if orcid in lookup:
                 for field in ["name", "affiliation"]:
-                    if field in lookup[cache["orcid"]] and field not in cache:
-                        value = lookup[cache]["orcid"][field]
-                        bot.info(f"   Updating {login} with {field}: {value}")
-                        cache[field] = value
+                    if lookup[orcid].get(field) and not cached.get(field):
+                        cached[field] = lookup[orcid][field]
+                        bot.info(f"   Updating {login} with {field}: {cached[field]}")
 
 
 def get_zenodo_record(doi):
     """Given a doi, retrieve a record using the Zenodo API"""
     # Get the record number from the doi
     record = doi.split("/")[-1].replace("zenodo.", "")
     token = os.environ.get("ZENODO_TOKEN")
```

### Comparing `tributors-0.0.21/tributors/utils/command.py` & `tributors-0.1.1/tributors/utils/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 class Command:
     """Class method to invoke shell commands and retrieve output and error.
     This class is inspired and derived from utils functions in
     https://github.com/vsoch/scif
     """
 
     def __init__(self, cmd=None):
-
         cmd = cmd or []
         self.returncode = None
         self.out = []
         self.err = []
 
         # If a list isn't provided, split it
         if cmd:
```

### Comparing `tributors-0.0.21/tributors/utils/file.py` & `tributors-0.1.1/tributors/utils/file.py`

 * *Files identical despite different names*

### Comparing `tributors-0.0.21/tributors/utils/prompt.py` & `tributors-0.1.1/tributors/utils/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,14 @@
     if not choice_prefix:
         choice_prefix = "/".join(choices)
     message = "[%s] : " % (choice_prefix)
 
     while choice not in choices:
         choice = get_input(message).strip()
 
-        # If multiple allowed, add selection to choices if includes all vaid
+        # If multiple allowed, add selection to choices if includes all valid
         if multiple is True:
             contenders = choice.strip().split(" ")
             if all(x in choices for x in contenders):
                 choices.append(choice)
         message = "Please enter a valid option in [%s]" % choice_prefix
     return choice
```

### Comparing `tributors-0.0.21/tributors/version.py` & `tributors-0.1.1/tributors/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
-__version__ = "0.0.21"
+__version__ = "0.1.1"
 AUTHOR = "Vanessa Sochat"
 AUTHOR_EMAIL = "vsochat@stanford.edu"
 NAME = "tributors"
 PACKAGE_URL = "http://www.github.com/con/tributors"
 KEYWORDS = "contributions, tributes"
 DESCRIPTION = "give tribute to your repository contributors."
 LICENSE = "LICENSE"
```

### Comparing `tributors-0.0.21/tributors.egg-info/PKG-INFO` & `tributors-0.1.1/tributors.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,18 @@
 Metadata-Version: 2.1
 Name: tributors
-Version: 0.0.21
+Version: 0.1.1
 Summary: give tribute to your repository contributors.
 Home-page: http://www.github.com/con/tributors
 Author: Vanessa Sochat
 Author-email: vsochat@stanford.edu
 Maintainer: Vanessa Sochat
 Maintainer-email: vsochat@stanford.edu
 License: LICENSE
-Description: # tributors
-        
-        ![docs/assets/img/logo.png](https://raw.githubusercontent.com/con/tributors/master/docs/assets/img/logo.png)
-        
-        <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-        [![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
-        <!-- ALL-CONTRIBUTORS-BADGE:END -->
-        
-        [Documentation](https://con.github.io/tributors/)
-        
-        ## What is tributors?
-        
-        Tributors is a Python library and GitHub action that helps you to pay tribute to your
-        contributors. Tribute interacts with several well-known repository metadata files:
-        
-         - [all-contributors](https://github.com/all-contributors)
-         - [Zenodo](https://zenodo.org)
-         - [CodeMeta](https://codemeta.github.io/)
-        
-        Each of the services above allows you to generate some kind of metadata file
-        that has one or more repository contributors. This file typically needs to be
-        generated and updated manually, and this is where tributors comes in to help!
-        Tributors will allow you to programatically create and update these files.
-        By way of using a shared cache, a `.tributors` file that can store common
-        identifiers, it becomes easy to update several of these metadata files at once.
-        You can set criteria such as a threshold for contributions to add a contributor,
-        export an Orcid ID token to ensure that you have Orcid Ids where needed,
-        or use an interactive mode to make decisions as you go.
-        
-        ## How does it work?
-        
-        Tributors uses the GitHub API, Zenodo API, and Orcid API to look up shared identifiers
-        for common metadata services like all contributors, Zenodo, and CodeMeta. The
-        tool is available for local or container usage, and as a GitHub Action (see the [examples](examples) folder).
-        See the full [documentation](https://con.github.io/tributors/) for getting started.
-        
-        
-        ## Contributors
-        
-        <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-        <!-- prettier-ignore-start -->
-        <!-- markdownlint-disable -->
-        <table>
-          <tr>
-            <td align="center"><a href="www.onerussian.com"><img src="https://avatars3.githubusercontent.com/u/39889?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Yaroslav Halchenko</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=yarikoptic" title="Code">💻</a> <a href="https://github.com/con/tributors/commits?author=yarikoptic" title="Documentation">📖</a></td>
-            <td align="center"><a href="https://vsoch.github.io"><img src="https://avatars0.githubusercontent.com/u/814322?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Vanessasaurus</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=vsoch" title="Code">💻</a></td>
-            <td align="center"><a href="https://github.com/pgrimaud"><img src="https://avatars1.githubusercontent.com/u/1866496?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pierre Grimaud</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=pgrimaud" title="Code">💻</a></td>
-          </tr>
-        </table>
-        
-        <!-- markdownlint-enable -->
-        <!-- prettier-ignore-end -->
-        <!-- ALL-CONTRIBUTORS-LIST:END -->
-        
 Keywords: contributions,tributes
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
@@ -75,7 +20,67 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: codemeta
+License-File: LICENSE
+
+# tributors
+
+![docs/assets/img/logo.png](https://raw.githubusercontent.com/con/tributors/master/docs/assets/img/logo.png)
+
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
+
+[Documentation](https://con.github.io/tributors/)
+
+## What is tributors?
+
+Tributors is a Python library and GitHub action that helps you to pay tribute to your
+contributors. Tribute interacts with several well-known repository metadata files:
+
+ - [all-contributors](https://github.com/all-contributors)
+ - [Zenodo](https://zenodo.org)
+ - [CodeMeta](https://codemeta.github.io/)
+
+Each of the services above allows you to generate some kind of metadata file
+that has one or more repository contributors. This file typically needs to be
+generated and updated manually, and this is where tributors comes in to help!
+Tributors will allow you to programmatically create and update these files.
+By way of using a shared cache, a `.tributors` file that can store common
+identifiers, it becomes easy to update several of these metadata files at once.
+You can set criteria such as a threshold for contributions to add a contributor,
+export an Orcid ID token to ensure that you have Orcid Ids where needed,
+or use an interactive mode to make decisions as you go.
+
+## How does it work?
+
+Tributors uses the GitHub API, Zenodo API, and Orcid API to look up shared identifiers
+for common metadata services like all contributors, Zenodo, and CodeMeta. The
+tool is available for local or container usage, and as a GitHub Action (see the [examples](examples) folder).
+See the full [documentation](https://con.github.io/tributors/) for getting started.
+
+
+## Contributors
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="www.onerussian.com"><img src="https://avatars3.githubusercontent.com/u/39889?v=4?s=100" width="100px;" alt="Yaroslav Halchenko"/><br /><sub><b>Yaroslav Halchenko</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=yarikoptic" title="Code">💻</a> <a href="https://github.com/con/tributors/commits?author=yarikoptic" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://vsoch.github.io"><img src="https://avatars0.githubusercontent.com/u/814322?v=4?s=100" width="100px;" alt="Vanessasaurus"/><br /><sub><b>Vanessasaurus</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=vsoch" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pgrimaud"><img src="https://avatars1.githubusercontent.com/u/1866496?v=4?s=100" width="100px;" alt="Pierre Grimaud"/><br /><sub><b>Pierre Grimaud</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=pgrimaud" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/vuillaut"><img src="https://avatars.githubusercontent.com/u/4263646?v=4?s=100" width="100px;" alt="vuillaut"/><br /><sub><b>vuillaut</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=vuillaut" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jwodder"><img src="https://avatars.githubusercontent.com/u/98207?v=4?s=100" width="100px;" alt="jwodder"/><br /><sub><b>jwodder</b></sub></a><br /><a href="https://github.com/con/tributors/commits?author=jwodder" title="Code">💻</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,41 +1,40 @@
-Metadata-Version: 2.1 Name: tributors Version: 0.0.21 Summary: give tribute to
+Metadata-Version: 2.1 Name: tributors Version: 0.1.1 Summary: give tribute to
 your repository contributors. Home-page: http://www.github.com/con/tributors
 Author: Vanessa Sochat Author-email: vsochat@stanford.edu Maintainer: Vanessa
-Sochat Maintainer-email: vsochat@stanford.edu License: LICENSE Description: #
-tributors ![docs/assets/img/logo.png](https://raw.githubusercontent.com/con/
-tributors/master/docs/assets/img/logo.png)  [![All Contributors](https://
-img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)]
-(#contributors-)  [Documentation](https://con.github.io/tributors/) ## What is
-tributors? Tributors is a Python library and GitHub action that helps you to
-pay tribute to your contributors. Tribute interacts with several well-known
-repository metadata files: - [all-contributors](https://github.com/all-
-contributors) - [Zenodo](https://zenodo.org) - [CodeMeta](https://
-codemeta.github.io/) Each of the services above allows you to generate some
-kind of metadata file that has one or more repository contributors. This file
-typically needs to be generated and updated manually, and this is where
-tributors comes in to help! Tributors will allow you to programatically create
-and update these files. By way of using a shared cache, a `.tributors` file
-that can store common identifiers, it becomes easy to update several of these
-metadata files at once. You can set criteria such as a threshold for
-contributions to add a contributor, export an Orcid ID token to ensure that you
-have Orcid Ids where needed, or use an interactive mode to make decisions as
-you go. ## How does it work? Tributors uses the GitHub API, Zenodo API, and
-Orcid API to look up shared identifiers for common metadata services like all
-contributors, Zenodo, and CodeMeta. The tool is available for local or
-container usage, and as a GitHub Action (see the [examples](examples) folder).
-See the full [documentation](https://con.github.io/tributors/) for getting
-started. ## Contributors
+Sochat Maintainer-email: vsochat@stanford.edu License: LICENSE Keywords:
+contributions,tributes Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: Mozilla Public License 2.0 (MPL 2.0) Classifier: Topic :: Software
+Development Classifier: Topic :: Scientific/Engineering Classifier: Natural
+Language :: English Classifier: Operating System :: Unix Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Description-Content-Type: text/markdown Provides-Extra: all
+Provides-Extra: codemeta License-File: LICENSE # tributors ![docs/assets/img/
+logo.png](https://raw.githubusercontent.com/con/tributors/master/docs/assets/
+img/logo.png)  [![All Contributors](https://img.shields.io/badge/
+all_contributors-5-orange.svg?style=flat-square)](#contributors-)
+[Documentation](https://con.github.io/tributors/) ## What is tributors?
+Tributors is a Python library and GitHub action that helps you to pay tribute
+to your contributors. Tribute interacts with several well-known repository
+metadata files: - [all-contributors](https://github.com/all-contributors) -
+[Zenodo](https://zenodo.org) - [CodeMeta](https://codemeta.github.io/) Each of
+the services above allows you to generate some kind of metadata file that has
+one or more repository contributors. This file typically needs to be generated
+and updated manually, and this is where tributors comes in to help! Tributors
+will allow you to programmatically create and update these files. By way of
+using a shared cache, a `.tributors` file that can store common identifiers, it
+becomes easy to update several of these metadata files at once. You can set
+criteria such as a threshold for contributions to add a contributor, export an
+Orcid ID token to ensure that you have Orcid Ids where needed, or use an
+interactive mode to make decisions as you go. ## How does it work? Tributors
+uses the GitHub API, Zenodo API, and Orcid API to look up shared identifiers
+for common metadata services like all contributors, Zenodo, and CodeMeta. The
+tool is available for local or container usage, and as a GitHub Action (see the
+[examples](examples) folder). See the full [documentation](https://
+con.github.io/tributors/) for getting started. ## Contributors
+[Yaroslav_Halchenko] [Vanessasaurus] [Pierre_Grimaud] [vuillaut] [jwodder]
+ Yaroslav_Halchenko   Vanessasaurus   Pierre_Grimaud   vuillaut   jwodder
+     ð» ð�     ð»         ð»      ð»  ð»
 
-Yaroslav_Halchenko Vanessasaurus Pierre_Grimaud
-
-    ð» ð    ð»       ð»
-   Keywords: contributions,tributes Platform: UNKNOWN Classifier: Intended
-Audience :: Science/Research Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Topic :: Software Development Classifier: Topic :: Scientific/
-Engineering Classifier: Natural Language :: English Classifier: Operating
-System :: Unix Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Description-Content-Type: text/markdown
-Provides-Extra: all Provides-Extra: codemeta
```

### Comparing `tributors-0.0.21/tributors.egg-info/SOURCES.txt` & `tributors-0.1.1/tributors.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+tests/test_mailmap.py
+tests/test_orcid.py
+tests/test_parsers.py
 tributors/__init__.py
 tributors/logger.py
 tributors/version.py
 tributors.egg-info/PKG-INFO
 tributors.egg-info/SOURCES.txt
 tributors.egg-info/dependency_links.txt
 tributors.egg-info/entry_points.txt
```

