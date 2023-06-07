# Comparing `tmp/godoo_cli-0.4.3.tar.gz` & `tmp/godoo_cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godoo_cli-0.4.3.tar", max compression
+gzip compressed data, was "godoo_cli-0.5.0.tar", max compression
```

## Comparing `godoo_cli-0.4.3.tar` & `godoo_cli-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0     7633 2023-02-18 22:20:55.968164 godoo_cli-0.4.3/LICENSE
--rw-r--r--   0        0        0     7074 2023-02-18 22:20:55.968164 godoo_cli-0.4.3/README.md
--rw-r--r--   0        0        0     5004 2023-02-18 22:20:55.968164 godoo_cli-0.4.3/pyproject.toml
--rw-r--r--   0        0        0       61 2023-02-18 22:20:55.968164 godoo_cli-0.4.3/src/godoo_cli/__init__.py
--rw-r--r--   0        0        0       88 2023-02-18 22:20:55.968164 godoo_cli-0.4.3/src/godoo_cli/__main__.py
--rw-r--r--   0        0        0     1963 2023-02-18 22:20:55.968164 godoo_cli-0.4.3/src/godoo_cli/cli.py
--rw-r--r--   0        0        0     5596 2023-02-18 22:20:55.968164 godoo_cli-0.4.3/src/godoo_cli/cli_common.py
--rw-r--r--   0        0        0      293 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/__init__.py
--rw-r--r--   0        0        0     5929 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/bootstrap.py
--rw-r--r--   0        0        0     1173 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/config.py
--rw-r--r--   0        0        0       28 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/db/__init__.py
--rw-r--r--   0        0        0      243 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/db/cli.py
--rw-r--r--   0        0        0     1300 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/db/connection.py
--rw-r--r--   0        0        0     1325 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/db/passwords.py
--rw-r--r--   0        0        0    10763 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/launch.py
--rw-r--r--   0        0        0      177 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/rpc/__init__.py
--rw-r--r--   0        0        0      710 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/rpc/cli.py
--rw-r--r--   0        0        0     2301 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/rpc/importer.py
--rw-r--r--   0        0        0     3623 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/rpc/modules.py
--rw-r--r--   0        0        0     4000 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/rpc/translations.py
--rw-r--r--   0        0        0     1619 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/shell.py
--rw-r--r--   0        0        0     8544 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/source_get.py
--rw-r--r--   0        0        0     4562 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/commands/test.py
--rw-r--r--   0        0        0      161 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/git/__init__.py
--rw-r--r--   0        0        0     1299 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/git/git_odoo.py
--rw-r--r--   0        0        0     3296 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/git/git_odoo_addons.py
--rw-r--r--   0        0        0     6460 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/git/git_repo.py
--rw-r--r--   0        0        0     4585 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/git/git_url.py
--rw-r--r--   0        0        0     1575 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/git/zip_download.py
--rw-r--r--   0        0        0       49 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/helpers/__init__.py
--rw-r--r--   0        0        0     2225 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/helpers/bootstrap.py
--rw-r--r--   0        0        0      386 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/helpers/cli.py
--rw-r--r--   0        0        0     8895 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/helpers/odoo_files.py
--rw-r--r--   0        0        0     3277 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/helpers/odoo_manifest.py
--rw-r--r--   0        0        0     2766 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/helpers/system.py
--rw-r--r--   0        0        0       22 2023-02-18 22:20:55.972164 godoo_cli-0.4.3/src/godoo_cli/version.py
--rw-r--r--   0        0        0     9110 1970-01-01 00:00:00.000000 godoo_cli-0.4.3/setup.py
--rw-r--r--   0        0        0     9094 1970-01-01 00:00:00.000000 godoo_cli-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-06-07 09:56:53.914171 godoo_cli-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7304 2023-06-07 09:56:53.914171 godoo_cli-0.5.0/README.md
+-rw-r--r--   0        0        0     5004 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/__init__.py
+-rw-r--r--   0        0        0       88 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/__main__.py
+-rw-r--r--   0        0        0     1963 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/cli.py
+-rw-r--r--   0        0        0     5596 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/cli_common.py
+-rw-r--r--   0        0        0      293 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/__init__.py
+-rw-r--r--   0        0        0     5929 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/bootstrap.py
+-rw-r--r--   0        0        0     1173 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/config.py
+-rw-r--r--   0        0        0       28 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/db/__init__.py
+-rw-r--r--   0        0        0      311 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/db/cli.py
+-rw-r--r--   0        0        0     1801 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/db/connection.py
+-rw-r--r--   0        0        0     1325 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/db/passwords.py
+-rw-r--r--   0        0        0    10763 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/launch.py
+-rw-r--r--   0        0        0      177 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/rpc/__init__.py
+-rw-r--r--   0        0        0      710 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/rpc/cli.py
+-rw-r--r--   0        0        0     2301 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/rpc/importer.py
+-rw-r--r--   0        0        0     3623 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/rpc/modules.py
+-rw-r--r--   0        0        0     4000 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/rpc/translations.py
+-rw-r--r--   0        0        0     1619 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/shell.py
+-rw-r--r--   0        0        0     8544 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/source_get.py
+-rw-r--r--   0        0        0     4562 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/test.py
+-rw-r--r--   0        0        0      161 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/git_odoo.py
+-rw-r--r--   0        0        0     3296 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/git_odoo_addons.py
+-rw-r--r--   0        0        0     6460 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/git_repo.py
+-rw-r--r--   0        0        0     4585 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/git_url.py
+-rw-r--r--   0        0        0     1575 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/zip_download.py
+-rw-r--r--   0        0        0       49 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/__init__.py
+-rw-r--r--   0        0        0     2225 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/bootstrap.py
+-rw-r--r--   0        0        0      386 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/cli.py
+-rw-r--r--   0        0        0     8895 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/odoo_files.py
+-rw-r--r--   0        0        0     3277 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/odoo_manifest.py
+-rw-r--r--   0        0        0     2766 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/system.py
+-rw-r--r--   0        0        0       22 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/version.py
+-rw-r--r--   0        0        0     9324 1970-01-01 00:00:00.000000 godoo_cli-0.5.0/PKG-INFO
```

### Comparing `godoo_cli-0.4.3/LICENSE` & `godoo_cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/README.md` & `godoo_cli-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 **gOdoo** is short for **go Odoo**. \
 It is a [Vscode Devcontainer](https://code.visualstudio.com/docs/remote/containers) Environment for [Odoo](https://odoo.com/)
 with Python CLI `godoo` convenience wrapper around `odoo-bin`.
 
 This repository is the base source for the Python package [godoo-cli](https://pypi.org/project/godoo-cli/) and serves as
 an all batteries included development environment.
 
+This is the source repository for `gOdoo`. If you want to use `gOdoo` please refer to [./docker/Dockerfile](./docker/Dockerfile) and modify it to install godoo using Pip.
+
 Made Possible by: [WEMPE Elektronic GmbH](https://wetech.de)
 
 # gOdoo-cli
 
 Python package that provides `godoo` command line interface around `odoo-bin`.
 
 It's build with [Typer](https://github.com/tiangolo/typer) to provide some convenience Wrappers for Odoo development and
@@ -25,23 +27,23 @@
 Use `godoo --help` to find out more. HINT: Install tab-completion with `godoo --install-completion`
 
 # Docker
 
 This workspace also contains Docker and Docker-Compose files. \
 
 They are used to provide either easy Odoo instances where the source is pulled according to
-[ODOO_MANIFEST.yml](./ODOO_MANIFEST.yml), or as a all batteries included devcontainer for VScode.
+[ODOO_MANIFEST.yml](odoo_manifest.yml), or as a all batteries included devcontainer for VScode.
 
 ## Requirements
 
 - [Docker Compose](https://github.com/docker/compose)
 - [Traefik](https://doc.traefik.io/traefik/) container running with docker provider and "traefik" named docker network.
   Example: [Traefik Devproxy](https://github.com/joshkreud/traefik_devproxy)
 - SSH Agent running. (check `echo $SSH_AUTH_SOCK`)\
-  This gets passed trough in the Buildprocess to clone Thirdparty repos.
+  This gets passed trough in the Buildprocess to clone Thirdparty repos (Optional).
 
 ## Just wanna have a quick and easy Odoo Instance?
 
 ```bash
 git clone https://github.com/OpenJKSoftware/gOdoo
 cd godoo
 . scripts/container_requirements.sh # Check Requirements
@@ -59,14 +61,15 @@
 ## Features
 
 - All batteries included [Devcontainer](https://code.visualstudio.com/docs/remote/containers) with postgres service
   Container and local DNS resolvig managed by [Traefik](https://doc.traefik.io/traefik/).
 - Easy fully working Odoo instance by `docker-compose up` with https access.
 - `godoo` CLI wrapper around Odoo. (Most flags can be configured by Environment Variables and are already preconfigured
   in the Containers. See [.env.sample](./.env.sample))
+- Cups Container, that provides a CUPS Printserver
 - `odoo-bin` is added to PATH and can thus be invoked from every folder.
 - Odoo will run in Proxy_Mode behind a Traefik reverse proxy for easy access on
   `https://$COMPOSE_PROJECT_NAME.docker.localhost`
 - [Odoo Pylint plugin](https://github.com/OCA/pylint-odoo) preconfigured in vscode
 - Preinstalled vscode Extensions Highlights:
   - [SQL Tools](https://marketplace.visualstudio.com/items?itemName=mtxr.sqltools) with preconfigured connection for
     easy Database access in the Sidebar.
@@ -140,11 +143,11 @@
 Use `godoo shell` to enter an interactive shell on the Database.
 
 # Odoo Modules
 
 ## Third Party Modules (manifest.yml)
 
 The `godoo` bootstrap function, will download some modules using git. \
-Which Repos to download is specified in `ODOO_MANIFEST.yml` ([Default](./ODOO_MANIFEST.yml)) \
+Which Repos to download is specified in `ODOO_MANIFEST.yml` ([Default](odoo_manifest.yml)) \
 Not all of the cloned addons are automatically installed. \
 Install them via the Apps Page in Odoo using `godoo rpc modules install` or using `odoo-bin`.\
 Modules downloaded on the Odoo Marketplace can be dropped as a `.zip` archive in [./thirdparty](./thirdparty)
```

### Comparing `godoo_cli-0.4.3/pyproject.toml` & `godoo_cli-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gOdoo-cli"
-version = "0.4.3"
+version = "0.5.0"
 description = "Wrapper around Odoo-Bin with some convinience RPC functions."
 authors = ["Joshua Kreuder <Joshua_Kreuder@outlook.com>"]
 license = "LGPL-3"
 readme = "README.md"
 packages = [{include = "godoo_cli",  from = "src"}]
 repository = "https://github.com/OpenJKSoftware/gOdoo"
 keywords = ["odoo", "godoo","devcontainer"]
```

### Comparing `godoo_cli-0.4.3/src/godoo_cli/cli.py` & `godoo_cli-0.5.0/src/godoo_cli/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/cli_common.py` & `godoo_cli-0.5.0/src/godoo_cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/commands/bootstrap.py` & `godoo_cli-0.5.0/src/godoo_cli/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/commands/config.py` & `godoo_cli-0.5.0/src/godoo_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/commands/db/passwords.py` & `godoo_cli-0.5.0/src/godoo_cli/commands/db/passwords.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/commands/launch.py` & `godoo_cli-0.5.0/src/godoo_cli/commands/launch.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/commands/rpc/cli.py` & `godoo_cli-0.5.0/src/godoo_cli/commands/rpc/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/commands/rpc/importer.py` & `godoo_cli-0.5.0/src/godoo_cli/commands/rpc/importer.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/commands/rpc/modules.py` & `godoo_cli-0.5.0/src/godoo_cli/commands/rpc/modules.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/commands/rpc/translations.py` & `godoo_cli-0.5.0/src/godoo_cli/commands/rpc/translations.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/commands/shell.py` & `godoo_cli-0.5.0/src/godoo_cli/commands/shell.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/commands/source_get.py` & `godoo_cli-0.5.0/src/godoo_cli/commands/source_get.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/commands/test.py` & `godoo_cli-0.5.0/src/godoo_cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/git/git_odoo.py` & `godoo_cli-0.5.0/src/godoo_cli/git/git_odoo.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/git/git_odoo_addons.py` & `godoo_cli-0.5.0/src/godoo_cli/git/git_odoo_addons.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/git/git_repo.py` & `godoo_cli-0.5.0/src/godoo_cli/git/git_repo.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/git/git_url.py` & `godoo_cli-0.5.0/src/godoo_cli/git/git_url.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/git/zip_download.py` & `godoo_cli-0.5.0/src/godoo_cli/git/zip_download.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/helpers/bootstrap.py` & `godoo_cli-0.5.0/src/godoo_cli/helpers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/helpers/odoo_files.py` & `godoo_cli-0.5.0/src/godoo_cli/helpers/odoo_files.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/helpers/odoo_manifest.py` & `godoo_cli-0.5.0/src/godoo_cli/helpers/odoo_manifest.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/src/godoo_cli/helpers/system.py` & `godoo_cli-0.5.0/src/godoo_cli/helpers/system.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.4.3/setup.py` & `godoo_cli-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,196 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: godoo-cli
+Version: 0.5.0
+Summary: Wrapper around Odoo-Bin with some convinience RPC functions.
+Home-page: https://github.com/OpenJKSoftware/gOdoo
+License: LGPL-3
+Keywords: odoo,godoo,devcontainer
+Author: Joshua Kreuder
+Author-email: Joshua_Kreuder@outlook.com
+Requires-Python: >=3.8.1,<3.12
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: codequality
+Provides-Extra: devcontainer
+Requires-Dist: black (>=22.10.0,<23.0.0) ; extra == "codequality"
+Requires-Dist: debugpy (>=1.6.0,<2.0.0) ; extra == "devcontainer"
+Requires-Dist: flake8 (>=5.0.4,<6.0.0) ; extra == "codequality"
+Requires-Dist: gitpython (>=3.1.27,<4.0.0)
+Requires-Dist: godoo-rpc (>=0.1.1,<0.2.0)
+Requires-Dist: inotify (>=0.2.10,<0.3.0) ; extra == "devcontainer"
+Requires-Dist: ipdb (>=0.13.9,<0.14.0) ; extra == "devcontainer"
+Requires-Dist: isort (>=5.10.1,<6.0.0) ; extra == "codequality"
+Requires-Dist: mock (>=4.0.3,<5.0.0) ; extra == "devcontainer"
+Requires-Dist: openupgradelib (>=3.3.4,<4.0.0)
+Requires-Dist: passlib (>=1.7.3,<2.0.0)
+Requires-Dist: pre-commit (>=2.20.0,<3.0.0) ; extra == "devcontainer"
+Requires-Dist: psycopg2 (>=2.8.6,<3.0.0)
+Requires-Dist: py-spy (>=0.3.11,<0.4.0) ; extra == "devcontainer"
+Requires-Dist: pylint-odoo (>=8.0.16,<9.0.0) ; extra == "codequality"
+Requires-Dist: pytest (>=7.2.1,<8.0.0) ; extra == "codequality"
+Requires-Dist: pytest-cov (>=4.0.0,<5.0.0) ; extra == "codequality"
+Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
+Requires-Dist: rope (>=0.23.0,<0.24.0) ; extra == "devcontainer"
+Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
+Requires-Dist: typer-common-functions (>=0.0.3,<0.0.4)
+Requires-Dist: watchdog (>=2.1.7,<3.0.0) ; extra == "devcontainer"
+Project-URL: Repository, https://github.com/OpenJKSoftware/gOdoo
+Description-Content-Type: text/markdown
+
+# gOdoo Dev Environment
+
+![OdooLogo](https://raw.githubusercontent.com/OpenJKSoftware/gOdoo/main/assets/odoo_logo.png)
+![ComposeLogo](https://raw.githubusercontent.com/docker/compose/v2/logo.png)
+
+[<img src="https://raw.githubusercontent.com/OpenJKSoftware/gOdoo/main/assets/godoo-main-cli.png" width="1000"/>](image.png)
+
+**gOdoo** is short for **go Odoo**. \
+It is a [Vscode Devcontainer](https://code.visualstudio.com/docs/remote/containers) Environment for [Odoo](https://odoo.com/)
+with Python CLI `godoo` convenience wrapper around `odoo-bin`.
+
+This repository is the base source for the Python package [godoo-cli](https://pypi.org/project/godoo-cli/) and serves as
+an all batteries included development environment.
+
+This is the source repository for `gOdoo`. If you want to use `gOdoo` please refer to [./docker/Dockerfile](./docker/Dockerfile) and modify it to install godoo using Pip.
+
+Made Possible by: [WEMPE Elektronic GmbH](https://wetech.de)
+
+# gOdoo-cli
+
+Python package that provides `godoo` command line interface around `odoo-bin`.
+
+It's build with [Typer](https://github.com/tiangolo/typer) to provide some convenience Wrappers for Odoo development and
+Deployment.
+
+Most flags can be configured by Env variables. \
+Use `godoo --help` to find out more. HINT: Install tab-completion with `godoo --install-completion`
+
+# Docker
+
+This workspace also contains Docker and Docker-Compose files. \
+
+They are used to provide either easy Odoo instances where the source is pulled according to
+[ODOO_MANIFEST.yml](odoo_manifest.yml), or as a all batteries included devcontainer for VScode.
+
+## Requirements
+
+- [Docker Compose](https://github.com/docker/compose)
+- [Traefik](https://doc.traefik.io/traefik/) container running with docker provider and "traefik" named docker network.
+  Example: [Traefik Devproxy](https://github.com/joshkreud/traefik_devproxy)
+- SSH Agent running. (check `echo $SSH_AUTH_SOCK`)\
+  This gets passed trough in the Buildprocess to clone Thirdparty repos (Optional).
+
+## Just wanna have a quick and easy Odoo Instance?
+
+```bash
+git clone https://github.com/OpenJKSoftware/gOdoo
+cd godoo
+. scripts/container_requirements.sh # Check Requirements
+docker-compose build
+docker-compose up
+# wait......
+# wait a bit mode ...
+# just a little bit longer ..
+# There we go.
+# Odoo should be reachable on 'https://godoo.docker.localhost' assuming you didn't change .env TRAEFIK_HOST_RULE or COMPOSE_PROJECT_NAME
+```
+
+# Devcontainer
+
+## Features
+
+- All batteries included [Devcontainer](https://code.visualstudio.com/docs/remote/containers) with postgres service
+  Container and local DNS resolvig managed by [Traefik](https://doc.traefik.io/traefik/).
+- Easy fully working Odoo instance by `docker-compose up` with https access.
+- `godoo` CLI wrapper around Odoo. (Most flags can be configured by Environment Variables and are already preconfigured
+  in the Containers. See [.env.sample](./.env.sample))
+- Cups Container, that provides a CUPS Printserver
+- `odoo-bin` is added to PATH and can thus be invoked from every folder.
+- Odoo will run in Proxy_Mode behind a Traefik reverse proxy for easy access on
+  `https://$COMPOSE_PROJECT_NAME.docker.localhost`
+- [Odoo Pylint plugin](https://github.com/OCA/pylint-odoo) preconfigured in vscode
+- Preinstalled vscode Extensions Highlights:
+  - [SQL Tools](https://marketplace.visualstudio.com/items?itemName=mtxr.sqltools) with preconfigured connection for
+    easy Database access in the Sidebar.
+  - [Docker Extension](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker) controls
+    container host.
+  - [Odoo Snippets](https://marketplace.visualstudio.com/items?itemName=mstuttgart.odoo-snippets)
+  - [Odoo Developments](https://marketplace.visualstudio.com/items?itemName=scapigliato.vsc-odoo-development) can Grab
+    Odoo Model information from a running Server
+  - [Todo Tree](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree)
+
+## Usage
+
+1. For Docker on windows: Clone the repo into the WSL2 Filesystem for better IO performance
+2. Have [Traefik](https://github.com/traefik/traefik) Running on `docker.localhost`
+   [Example](https://github.com/joshkreud/traefik_devproxy) \
+   There must be a Docker network called `traefik` that can reach traefik.
+3. Open Devcontianer:
+   - If you have the Devcontainer CLI: `devcontainer open .`
+   - If not open the workspace in Local Vscode. In the Command pallete search for `Reopen in container`
+4. From **within the container** start Odoo using one of the following commands:
+   - You can enable godoo tab-completion by `godoo --install-completion`
+   - `make` -> Loads Odoo + Workspace Addons
+   - `make bare` -> Loads Odoo with ony `web` installed.
+   - `make kill` -> Search for `odoo-bin` processes and kill them
+   - `make reset` -> Drops DB, deletes config file and datafolder
+   - The full init script is available via "`godoo`". (See --help for Options)
+5. Open Odoo `https://$COMPOSE_PROJECT_NAME.docker.localhost`\
+   For example `COMPOSE_PROJECT_NAME=godoo` --> [https://godoo.docker.localhost](https://godoo.docker.localhost)
+6. Login with `admin:admin`
+7. Profit!
+
+### Access to Odoo and Thirdparty addon Source
+
+You can access the Odoo source by opening the VsCode workspace [full.code-workspace](full.code-workspace) from within
+the Container. This will open a [Multi-Root Workspace](https://code.visualstudio.com/docs/editor/multi-root-workspaces).
+Really waiting for https://github.com/microsoft/vscode-remote-release/issues/3665 here.
+
+## Reset Devcontainer Data
+
+When you screwed up so bad its time to just start Over godoo has you covered:
+
+### Automatic Reset
+
+There are 3 Options to reset the Dev Env.
+
+1. From **Outside** the Container run `make reset` in the project root to delete docker volumes and restart the
+   container. (Vscode will prompt to reconnect if still open)
+2. From **Outside** the Container run `make reset-hard` in the project root to force rebuild the main Odoo container and
+   then do the same as `make reset`
+3. From **Inside** the Container run `make reset` to drop the DB and delete varlib and the bootstrap flag, which is way
+   quicker than the other options.
+
+### Manual Reset
+
+1. Close vscode
+2. Remove `app` and `db` container from docker.
+3. Remove volumes: `db, odoo_thirdparty, odoo_web, vscode_extensions`
+4. Restart Devcontainer
+
+## Python Debugging
+
+### VsCode Debugging
+
+Debugging doesn't reliably work with
+[Odoo Multiprocess](https://www.odoo.com/documentation/14.0/developer/misc/other/cmdline.html#multiprocessing) mode
+enabled. \
+The container ships with a Vscode Debug profile, that sets `--workers 0` to allow for Debugging Breakpoints. See [.vscode/launch.json](./.vscode/launch.json)
+
+### Interactive Shell
+
+Use `godoo shell` to enter an interactive shell on the Database.
+
+# Odoo Modules
+
+## Third Party Modules (manifest.yml)
+
+The `godoo` bootstrap function, will download some modules using git. \
+Which Repos to download is specified in `ODOO_MANIFEST.yml` ([Default](odoo_manifest.yml)) \
+Not all of the cloned addons are automatically installed. \
+Install them via the Apps Page in Odoo using `godoo rpc modules install` or using `odoo-bin`.\
+Modules downloaded on the Odoo Marketplace can be dropped as a `.zip` archive in [./thirdparty](./thirdparty)
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['godoo_cli',
- 'godoo_cli.commands',
- 'godoo_cli.commands.db',
- 'godoo_cli.commands.rpc',
- 'godoo_cli.git',
- 'godoo_cli.helpers']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['gitpython>=3.1.27,<4.0.0',
- 'godoo-rpc>=0.1.1,<0.2.0',
- 'openupgradelib>=3.3.4,<4.0.0',
- 'passlib>=1.7.3,<2.0.0',
- 'psycopg2>=2.8.6,<3.0.0',
- 'python-dotenv>=0.20.0,<0.21.0',
- 'ruamel-yaml>=0.17.21,<0.18.0',
- 'typer-common-functions>=0.0.3,<0.0.4']
-
-extras_require = \
-{'codequality': ['pylint-odoo>=8.0.16,<9.0.0',
-                 'black>=22.10.0,<23.0.0',
-                 'isort>=5.10.1,<6.0.0',
-                 'flake8>=5.0.4,<6.0.0',
-                 'pytest>=7.2.1,<8.0.0',
-                 'pytest-cov>=4.0.0,<5.0.0'],
- 'devcontainer': ['ipdb>=0.13.9,<0.14.0',
-                  'debugpy>=1.6.0,<2.0.0',
-                  'pre-commit>=2.20.0,<3.0.0',
-                  'watchdog>=2.1.7,<3.0.0',
-                  'py-spy>=0.3.11,<0.4.0',
-                  'rope>=0.23.0,<0.24.0',
-                  'inotify>=0.2.10,<0.3.0',
-                  'mock>=4.0.3,<5.0.0']}
-
-entry_points = \
-{'console_scripts': ['godoo = godoo_cli:launch_cli']}
-
-setup_kwargs = {
-    'name': 'godoo-cli',
-    'version': '0.4.3',
-    'description': 'Wrapper around Odoo-Bin with some convinience RPC functions.',
-    'long_description': '# gOdoo Dev Environment\n\n![OdooLogo](https://raw.githubusercontent.com/OpenJKSoftware/gOdoo/main/assets/odoo_logo.png)\n![ComposeLogo](https://raw.githubusercontent.com/docker/compose/v2/logo.png)\n\n[<img src="https://raw.githubusercontent.com/OpenJKSoftware/gOdoo/main/assets/godoo-main-cli.png" width="1000"/>](image.png)\n\n**gOdoo** is short for **go Odoo**. \\\nIt is a [Vscode Devcontainer](https://code.visualstudio.com/docs/remote/containers) Environment for [Odoo](https://odoo.com/)\nwith Python CLI `godoo` convenience wrapper around `odoo-bin`.\n\nThis repository is the base source for the Python package [godoo-cli](https://pypi.org/project/godoo-cli/) and serves as\nan all batteries included development environment.\n\nMade Possible by: [WEMPE Elektronic GmbH](https://wetech.de)\n\n# gOdoo-cli\n\nPython package that provides `godoo` command line interface around `odoo-bin`.\n\nIt\'s build with [Typer](https://github.com/tiangolo/typer) to provide some convenience Wrappers for Odoo development and\nDeployment.\n\nMost flags can be configured by Env variables. \\\nUse `godoo --help` to find out more. HINT: Install tab-completion with `godoo --install-completion`\n\n# Docker\n\nThis workspace also contains Docker and Docker-Compose files. \\\n\nThey are used to provide either easy Odoo instances where the source is pulled according to\n[ODOO_MANIFEST.yml](./ODOO_MANIFEST.yml), or as a all batteries included devcontainer for VScode.\n\n## Requirements\n\n- [Docker Compose](https://github.com/docker/compose)\n- [Traefik](https://doc.traefik.io/traefik/) container running with docker provider and "traefik" named docker network.\n  Example: [Traefik Devproxy](https://github.com/joshkreud/traefik_devproxy)\n- SSH Agent running. (check `echo $SSH_AUTH_SOCK`)\\\n  This gets passed trough in the Buildprocess to clone Thirdparty repos.\n\n## Just wanna have a quick and easy Odoo Instance?\n\n```bash\ngit clone https://github.com/OpenJKSoftware/gOdoo\ncd godoo\n. scripts/container_requirements.sh # Check Requirements\ndocker-compose build\ndocker-compose up\n# wait......\n# wait a bit mode ...\n# just a little bit longer ..\n# There we go.\n# Odoo should be reachable on \'https://godoo.docker.localhost\' assuming you didn\'t change .env TRAEFIK_HOST_RULE or COMPOSE_PROJECT_NAME\n```\n\n# Devcontainer\n\n## Features\n\n- All batteries included [Devcontainer](https://code.visualstudio.com/docs/remote/containers) with postgres service\n  Container and local DNS resolvig managed by [Traefik](https://doc.traefik.io/traefik/).\n- Easy fully working Odoo instance by `docker-compose up` with https access.\n- `godoo` CLI wrapper around Odoo. (Most flags can be configured by Environment Variables and are already preconfigured\n  in the Containers. See [.env.sample](./.env.sample))\n- `odoo-bin` is added to PATH and can thus be invoked from every folder.\n- Odoo will run in Proxy_Mode behind a Traefik reverse proxy for easy access on\n  `https://$COMPOSE_PROJECT_NAME.docker.localhost`\n- [Odoo Pylint plugin](https://github.com/OCA/pylint-odoo) preconfigured in vscode\n- Preinstalled vscode Extensions Highlights:\n  - [SQL Tools](https://marketplace.visualstudio.com/items?itemName=mtxr.sqltools) with preconfigured connection for\n    easy Database access in the Sidebar.\n  - [Docker Extension](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker) controls\n    container host.\n  - [Odoo Snippets](https://marketplace.visualstudio.com/items?itemName=mstuttgart.odoo-snippets)\n  - [Odoo Developments](https://marketplace.visualstudio.com/items?itemName=scapigliato.vsc-odoo-development) can Grab\n    Odoo Model information from a running Server\n  - [Todo Tree](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree)\n\n## Usage\n\n1. For Docker on windows: Clone the repo into the WSL2 Filesystem for better IO performance\n2. Have [Traefik](https://github.com/traefik/traefik) Running on `docker.localhost`\n   [Example](https://github.com/joshkreud/traefik_devproxy) \\\n   There must be a Docker network called `traefik` that can reach traefik.\n3. Open Devcontianer:\n   - If you have the Devcontainer CLI: `devcontainer open .`\n   - If not open the workspace in Local Vscode. In the Command pallete search for `Reopen in container`\n4. From **within the container** start Odoo using one of the following commands:\n   - You can enable godoo tab-completion by `godoo --install-completion`\n   - `make` -> Loads Odoo + Workspace Addons\n   - `make bare` -> Loads Odoo with ony `web` installed.\n   - `make kill` -> Search for `odoo-bin` processes and kill them\n   - `make reset` -> Drops DB, deletes config file and datafolder\n   - The full init script is available via "`godoo`". (See --help for Options)\n5. Open Odoo `https://$COMPOSE_PROJECT_NAME.docker.localhost`\\\n   For example `COMPOSE_PROJECT_NAME=godoo` --> [https://godoo.docker.localhost](https://godoo.docker.localhost)\n6. Login with `admin:admin`\n7. Profit!\n\n### Access to Odoo and Thirdparty addon Source\n\nYou can access the Odoo source by opening the VsCode workspace [full.code-workspace](full.code-workspace) from within\nthe Container. This will open a [Multi-Root Workspace](https://code.visualstudio.com/docs/editor/multi-root-workspaces).\nReally waiting for https://github.com/microsoft/vscode-remote-release/issues/3665 here.\n\n## Reset Devcontainer Data\n\nWhen you screwed up so bad its time to just start Over godoo has you covered:\n\n### Automatic Reset\n\nThere are 3 Options to reset the Dev Env.\n\n1. From **Outside** the Container run `make reset` in the project root to delete docker volumes and restart the\n   container. (Vscode will prompt to reconnect if still open)\n2. From **Outside** the Container run `make reset-hard` in the project root to force rebuild the main Odoo container and\n   then do the same as `make reset`\n3. From **Inside** the Container run `make reset` to drop the DB and delete varlib and the bootstrap flag, which is way\n   quicker than the other options.\n\n### Manual Reset\n\n1. Close vscode\n2. Remove `app` and `db` container from docker.\n3. Remove volumes: `db, odoo_thirdparty, odoo_web, vscode_extensions`\n4. Restart Devcontainer\n\n## Python Debugging\n\n### VsCode Debugging\n\nDebugging doesn\'t reliably work with\n[Odoo Multiprocess](https://www.odoo.com/documentation/14.0/developer/misc/other/cmdline.html#multiprocessing) mode\nenabled. \\\nThe container ships with a Vscode Debug profile, that sets `--workers 0` to allow for Debugging Breakpoints. See [.vscode/launch.json](./.vscode/launch.json)\n\n### Interactive Shell\n\nUse `godoo shell` to enter an interactive shell on the Database.\n\n# Odoo Modules\n\n## Third Party Modules (manifest.yml)\n\nThe `godoo` bootstrap function, will download some modules using git. \\\nWhich Repos to download is specified in `ODOO_MANIFEST.yml` ([Default](./ODOO_MANIFEST.yml)) \\\nNot all of the cloned addons are automatically installed. \\\nInstall them via the Apps Page in Odoo using `godoo rpc modules install` or using `odoo-bin`.\\\nModules downloaded on the Odoo Marketplace can be dropped as a `.zip` archive in [./thirdparty](./thirdparty)\n',
-    'author': 'Joshua Kreuder',
-    'author_email': 'Joshua_Kreuder@outlook.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/OpenJKSoftware/gOdoo',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

