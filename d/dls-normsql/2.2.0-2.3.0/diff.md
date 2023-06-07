# Comparing `tmp/dls-normsql-2.2.0.tar.gz` & `tmp/dls-normsql-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-normsql-2.2.0.tar", last modified: Tue Jun  6 09:43:32 2023, max compression
+gzip compressed data, was "dls-normsql-2.3.0.tar", last modified: Wed Jun  7 14:07:38 2023, max compression
```

## Comparing `dls-normsql-2.2.0.tar` & `dls-normsql-2.3.0.tar`

### file list

```diff
@@ -1,85 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.739175 dls-normsql-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-06-06 09:43:32.739175 dls-normsql-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:43:32.739175 dls-normsql-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.727175 dls-normsql-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/src/dls_normsql/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/aiomysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    21939 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/src/dls_normsql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.731175 dls-normsql-2.2.0/src/dls_normsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 09:43:32.000000 dls-normsql-2.2.0/src/dls_normsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:32.739175 dls-normsql-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/my_database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/my_table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/test_aiomysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/test_backup_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-06 09:43:23.000000 dls-normsql-2.2.0/tests/test_revision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.694619 dls-normsql-2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.670619 dls-normsql-2.3.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.682618 dls-normsql-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.682618 dls-normsql-2.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-06-07 14:07:38.694619 dls-normsql-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.682618 dls-normsql-2.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.670619 dls-normsql-2.3.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.682618 dls-normsql-2.3.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.686619 dls-normsql-2.3.0/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.686619 dls-normsql-2.3.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.686619 dls-normsql-2.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.686619 dls-normsql-2.3.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.686619 dls-normsql-2.3.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:07:38.694619 dls-normsql-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.670619 dls-normsql-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.690619 dls-normsql-2.3.0/src/dls_normsql/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21932 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.690619 dls-normsql-2.3.0/src/dls_normsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.694619 dls-normsql-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/my_database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/my_table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/test_aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/test_backup_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/test_revision.py
```

### Comparing `dls-normsql-2.2.0/.dae-devops/Makefile` & `dls-normsql-2.3.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.dae-devops/docs/conventions.rst` & `dls-normsql-2.3.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.dae-devops/docs/developing.rst` & `dls-normsql-2.3.0/.dae-devops/docs/developing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -5,34 +5,27 @@
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
 Clone the repository::
 
+    $ cd <your development area>
     $ git clone https://gitlab.diamond.ac.uk/kbp43231/dls-normsql.git
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software.
-Make sure to have at least python version 3.9 then::
+Make sure to have at least python version 3.10 then::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd dls-normsql
-    $ pip install -e .[dev]
+    $ pip install -e .[dev,docs]
 
 Now you may begin modifying the code.
 
-|
 
-If you plan to modify the docs, you will need to::
-
-    $ pip install -e .[docs]
-
-    
-
-
-.. # dae_devops_fingerprint 7b83e003f8bbbf54c27b4bd8141fb0e5
+.. # dae_devops_fingerprint b23d73dd4de218c9524358cf343938e7
```

### Comparing `dls-normsql-2.2.0/.dae-devops/docs/devops.rst` & `dls-normsql-2.3.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.dae-devops/docs/docs_structure.rst` & `dls-normsql-2.3.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.dae-devops/docs/installing.rst` & `dls-normsql-2.3.0/.dae-devops/docs/installing.rst`

 * *Files 13% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 .. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-normsql
 
 Installing
 =======================================================================
 
 
-You will need python 3.9 or later. 
+You will need python 3.10 or later. 
 
-On a Diamond Light Source internal computer, you can achieve Python 3.9 by::
+On a Diamond Light Source internal computer, you can achieve Python 3.10 by::
 
-    $ module load python/3.9
+    $ module load python/3.10
 
 You can check your version of python by typing into a terminal::
 
     $ python3 --version
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 
-You can now use ``pip`` to install the library and its dependencies::
+You can now use ``pip`` to install the package and its dependencies::
 
     $ python3 -m pip install dls-normsql
 
-If you require a feature that is not currently released you can also install
+If you require a feature that is not currently released, you can also install
 from git::
 
     $ python3 -m pip install git+https://gitlab.diamond.ac.uk/kbp43231/dls-normsql.git
 
-The library should now be installed and the commandline should be available.
+The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ dls-normsql --version
     $ dls-normsql --version-json
 
-.. # dae_devops_fingerprint a2fe8dfbc79c151a5b899b244a529aa6
+.. # dae_devops_fingerprint d972d49fe32bcad19880f2817fed8fae
```

### Comparing `dls-normsql-2.2.0/.dae-devops/docs/testing.rst` & `dls-normsql-2.3.0/.dae-devops/docs/testing.rst`

 * *Files 19% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 If you want to see more output of the test while it's running you can do::
 
     $ pytest -sv -ra --tb=line tests/the_test_you_want.py
 
 Each test will write files into its own directory::
 
-    /tmp/dls-normsql/tests/....
+    /tmp/dls-normsql/tests/*
 
 The tests clear their directory when they start, but not when they finish.
-This allows peeking in there to see what's been written by the test.
+This allows you to examine what's been written by the test.
 
     
 
 
-.. # dae_devops_fingerprint 1801aaf6bd998d192c9fb4cdd6c3e79f
+.. # dae_devops_fingerprint 69544ab25d1fea250e99af1cf0c84506
```

### Comparing `dls-normsql-2.2.0/.devcontainer/Dockerfile` & `dls-normsql-2.3.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.devcontainer/devcontainer.json` & `dls-normsql-2.3.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.github/CONTRIBUTING.rst` & `dls-normsql-2.3.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.github/actions/install_requirements/action.yml` & `dls-normsql-2.3.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.github/dependabot.yml` & `dls-normsql-2.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.github/pages/make_switcher.py` & `dls-normsql-2.3.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.github/workflows/code.yml` & `dls-normsql-2.3.0/.github/workflows/code.yml`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,14 @@
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
         python: ["3.10"]
         install: ["-e .[dev,docs]"]
-        # Make one version be non-editable to test both paths of version code
-        include:
-          - os: "ubuntu-latest"
-            python: "3.9"
-            install: ".[dev,docs]"
 
     runs-on: ${{ matrix.os }}
     env:
       # https://github.com/pytest-dev/pytest/issues/2042
       PY_IGNORE_IMPORTMISMATCH: "1"
 
     steps:
@@ -212,8 +207,8 @@
 
       - name: Publish to PyPI
         if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
 
-# dae_devops_fingerprint d13e8289ca6252679ab7d9ae8db75617
+# dae_devops_fingerprint a23991a7d28e20d040902bf8d1aa4541
```

### Comparing `dls-normsql-2.2.0/.github/workflows/docs.yml` & `dls-normsql-2.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.github/workflows/docs_clean.yml` & `dls-normsql-2.3.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.github/workflows/linkcheck.yml` & `dls-normsql-2.3.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.gitignore` & `dls-normsql-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.gitlab-ci.yml` & `dls-normsql-2.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/.vscode/launch.json` & `dls-normsql-2.3.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/LICENSE` & `dls-normsql-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/PKG-INFO` & `dls-normsql-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 2.2.0
-Summary: Normalized API over various sql libraries.
+Version: 2.3.0
+Summary: Normalized API over various sql libraries for consistency across multiple projects.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -204,59 +204,19 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://gitlab.diamond.ac.uk/kbp43231/dls-normsql
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 dls-normsql
 =======================================================================
 
-Normalized API over various sql libraries.
-
-Intended advantages:
-
-- common connection and set of sql commands
-- reusable library for consistency across multiple projects
-
-Installation
------------------------------------------------------------------------
-::
-
-    pip install git+https://gitlab.diamond.ac.uk/kbp43231/dls-normsql.git 
-
-    dls-normsql --version
-
-Documentation
------------------------------------------------------------------------
-
-See https://www.cs.diamond.ac.uk/dls-normsql for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/kbp43231/dls-normsql.git 
-    cd dls-normsql
-    virtualenv /scratch/$USER/venv/dls-normsql
-    source /scratch/$USER/venv/dls-normsql/bin/activate 
-    pip install -e .[dev]
-    make -f .dls-normsql/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/dls-normsql/build/html/index.html
-
-Topics for further documentation:
-
-- TODO list of improvements
-- change log
-
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
+Normalized API over various sql libraries for consistency across multiple projects.
```

### Comparing `dls-normsql-2.2.0/docs/conf.py` & `dls-normsql-2.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     # Create pages from jupyter notebooks
     "nbsphinx",
     "IPython.sphinxext.ipython_console_highlighting",
 ]
 
 # If true, Sphinx will warn about all references where the target cannot
 # be found.
-nitpicky = True
+nitpicky = False
 
 # A list of (type, target) tuples (by default empty) that should be ignored when
 # generating warnings in "nitpicky mode". Note that type should include the
 # domain name if present. Example entries would be ('py:func', 'int') or
 # ('envvar', 'LD_LIBRARY_PATH').
 nitpick_ignore = [("py:class", "numpy.ma.core.MaskedArray")]
 
@@ -184,17 +184,17 @@
 
 # I got this from https://github.com/sphinx-doc/sphinx/issues/4054.
 # It will allow the ${token} replacement in the rst documents.
 ultimate_replacements = {
     "$" + "{repository_name}": "dls-normsql",
     "$" + "{package_name}": "dls_normsql",
     "$" + "{git_url}": "https://gitlab.diamond.ac.uk/kbp43231",
-    "$" + "{python_version_at_least}": "3.9",
+    "$" + "{python_version_at_least}": "3.10",
 }
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint cd8b8b6c6077d960c9ed6af1579909b3
+# dae_devops_fingerprint 0afc2bceebf806891327ed822e2760a9
```

### Comparing `dls-normsql-2.2.0/docs/images/dls-favicon.ico` & `dls-normsql-2.3.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/docs/images/dls-logo.svg` & `dls-normsql-2.3.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/pyproject.toml` & `dls-normsql-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dls-normsql"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
 ]
-description = "Normalized API over various sql libraries."
+description = "Normalized API over various sql libraries for consistency across multiple projects."
 dependencies = ["dls-utilpack", "aiosqlite", "aiomysql", "cryptography"]
 dynamic = ["version"]
 license.file = "LICENSE"
-readme = "README.rst"
-requires-python = ">=3.9"
+readme = "README.md"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = [
     "black==22.12.0",
     "mypy",
     "flake8-isort",
     "Flake8-pyproject",
@@ -98,8 +96,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint ecc6232348dbe2bd0e46bde0c1961e3b
+# dae_devops_fingerprint aec34b4646849a704b0974693e0148cc
```

### Comparing `dls-normsql-2.2.0/src/dls_normsql/__main__.py` & `dls-normsql-2.3.0/src/dls_normsql/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/src/dls_normsql/aiomysql.py` & `dls-normsql-2.3.0/src/dls_normsql/aiomysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,14 @@
 
         self.__connection = None
 
         self.__tables = {}
 
         self.__backup_restore_lock = asyncio.Lock()
 
-        # TODO: Remove cursor lock when adding connection pooling.
-        self.__cursor_lock = asyncio.Lock()
-
         # Last undo position.
         self.__last_restore = 0
 
     # ----------------------------------------------------------------------------------------
     def __parameterize(self, sql: str, subs: List[Any]):
         """
         Connect to database at filename given in constructor.
@@ -295,50 +292,49 @@
         if isinstance(table, str):
             table = require("table definitions", self.__tables, table)
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             await self.execute("DROP TABLE IF EXISTS %s" % (table.name))
 
-        async with self.__cursor_lock:
-            async with self.__connection.cursor() as cursor:
+        async with self.__connection.cursor() as cursor:
 
-                fields_sql = []
-                indices_sql = []
+            fields_sql = []
+            indices_sql = []
 
-                for field_name in table.fields:
-                    field = table.fields[field_name]
-                    field_type = field["type"].upper()
-                    if field_type == "TEXT PRIMARY KEY":
-                        field_type = "VARCHAR(64) PRIMARY KEY"
-                    fields_sql.append("`%s` %s" % (field_name, field_type))
-                    if field.get("index", False):
-                        if field_type == "TEXT":
-                            index_length = "(128)"
-                        else:
-                            index_length = ""
-                        indices_sql.append(
-                            "CREATE INDEX `%s_%s` ON `%s`(`%s`%s)"
-                            % (
-                                table.name,
-                                field_name,
-                                table.name,
-                                field_name,
-                                index_length,
-                            )
+            for field_name in table.fields:
+                field = table.fields[field_name]
+                field_type = field["type"].upper()
+                if field_type == "TEXT PRIMARY KEY":
+                    field_type = "VARCHAR(64) PRIMARY KEY"
+                fields_sql.append("`%s` %s" % (field_name, field_type))
+                if field.get("index", False):
+                    if field_type == "TEXT":
+                        index_length = "(128)"
+                    else:
+                        index_length = ""
+                    indices_sql.append(
+                        "CREATE INDEX `%s_%s` ON `%s`(`%s`%s)"
+                        % (
+                            table.name,
+                            field_name,
+                            table.name,
+                            field_name,
+                            index_length,
                         )
+                    )
 
-                sql = "CREATE TABLE `%s`\n(%s)" % (table.name, ",\n  ".join(fields_sql))
+            sql = "CREATE TABLE `%s`\n(%s)" % (table.name, ",\n  ".join(fields_sql))
 
-                logger.debug("\n%s\n%s" % (sql, "\n".join(indices_sql)))
+            logger.debug("\n%s\n%s" % (sql, "\n".join(indices_sql)))
 
-                await cursor.execute(sql)
+            await cursor.execute(sql)
 
-                for sql in indices_sql:
-                    await cursor.execute(sql)
+            for sql in indices_sql:
+                await cursor.execute(sql)
 
     # ----------------------------------------------------------------------------------------
     async def insert(
         self,
         table,
         rows,
         why=None,
@@ -394,18 +390,17 @@
 
         if why is None:
             message = "\n%s\n%s" % (sql, values_rows)
         else:
             message = "%s:\n%s\n%s" % (why, sql, values_rows)
 
         try:
-            async with self.__cursor_lock:
-                async with self.__connection.cursor() as cursor:
-                    await cursor.executemany(sql, values_rows)
-                    logger.debug(message)
+            async with self.__connection.cursor() as cursor:
+                await cursor.executemany(sql, values_rows)
+                logger.debug(message)
 
         except (TypeError, aiomysql.OperationalError) as exception:
             raise RuntimeError(f"{exception} doing {message}")
 
     # ----------------------------------------------------------------------------------------
     async def update(
         self,
@@ -444,35 +439,34 @@
         )
 
         if subs is not None:
             values_row.extend(subs)
 
         sql = self.__parameterize(sql, subs)
 
-        async with self.__cursor_lock:
-            async with self.__connection.cursor() as cursor:
-                try:
-                    await cursor.execute(sql, values_row)
-                    rowcount = cursor.rowcount
-
-                    if why is None:
-                        logger.debug(
-                            "%d rows from:\n%s\nvalues %s" % (rowcount, sql, values_row)
-                        )
-                    else:
-                        logger.debug(
-                            "%d rows from %s:\n%s\nvalues %s"
-                            % (rowcount, why, sql, values_row)
-                        )
+        async with self.__connection.cursor() as cursor:
+            try:
+                await cursor.execute(sql, values_row)
+                rowcount = cursor.rowcount
 
-                except (TypeError, aiomysql.OperationalError):
-                    if why is None:
-                        raise RuntimeError(f"failed to execute {sql}")
-                    else:
-                        raise RuntimeError(f"failed to execute {why}: {sql}")
+                if why is None:
+                    logger.debug(
+                        "%d rows from:\n%s\nvalues %s" % (rowcount, sql, values_row)
+                    )
+                else:
+                    logger.debug(
+                        "%d rows from %s:\n%s\nvalues %s"
+                        % (rowcount, why, sql, values_row)
+                    )
+
+            except (TypeError, aiomysql.OperationalError):
+                if why is None:
+                    raise RuntimeError(f"failed to execute {sql}")
+                else:
+                    raise RuntimeError(f"failed to execute {why}: {sql}")
 
         return rowcount
 
     # ----------------------------------------------------------------------------------------
     async def execute(
         self,
         sql,
@@ -480,86 +474,82 @@
         why=None,
     ):
         """
         Execute a sql statement.
         If subs is a list of lists, then these are presumed the values for executemany.
         """
 
-        async with self.__cursor_lock:
-            async with self.__connection.cursor() as cursor:
-                try:
-                    sql = self.__parameterize(sql, subs)
+        async with self.__connection.cursor() as cursor:
+            try:
+                sql = self.__parameterize(sql, subs)
 
-                    # Subs is a list of lists?
-                    if (
-                        isinstance(subs, list)
-                        and len(subs) > 0
-                        and isinstance(subs[0], list)
-                    ):
-                        logger.debug(f"inserting {len(subs)} of {len(subs[0])}")
-                        await cursor.executemany(sql, subs)
-                    else:
-                        await cursor.execute(sql, subs)
+                # Subs is a list of lists?
+                if (
+                    isinstance(subs, list)
+                    and len(subs) > 0
+                    and isinstance(subs[0], list)
+                ):
+                    logger.debug(f"inserting {len(subs)} of {len(subs[0])}")
+                    await cursor.executemany(sql, subs)
+                else:
+                    await cursor.execute(sql, subs)
 
-                    if why is None:
-                        if cursor.rowcount > 0:
-                            logger.debug(
-                                f"{cursor.rowcount} records affected by\n{sql}\nvalues {subs}"
-                            )
-                        else:
-                            logger.debug(f"{sql}\nvalues {subs}")
+                if why is None:
+                    if cursor.rowcount > 0:
+                        logger.debug(
+                            f"{cursor.rowcount} records affected by\n{sql}\nvalues {subs}"
+                        )
                     else:
-                        if cursor.rowcount > 0:
-                            logger.debug(
-                                f"{cursor.rowcount} records affected by {why}:\n{sql} values {subs}"
-                            )
-                        else:
-                            logger.debug(f"{why}: {sql}\nvalues {subs}")
-                except (TypeError, aiomysql.OperationalError):
-                    if why is None:
-                        raise RuntimeError(f"failed to execute {sql}")
+                        logger.debug(f"{sql}\nvalues {subs}")
+                else:
+                    if cursor.rowcount > 0:
+                        logger.debug(
+                            f"{cursor.rowcount} records affected by {why}:\n{sql} values {subs}"
+                        )
                     else:
-                        raise RuntimeError(f"failed to execute {why}: {sql}")
+                        logger.debug(f"{why}: {sql}\nvalues {subs}")
+            except (TypeError, aiomysql.OperationalError):
+                if why is None:
+                    raise RuntimeError(f"failed to execute {sql}")
+                else:
+                    raise RuntimeError(f"failed to execute {why}: {sql}")
 
     # ----------------------------------------------------------------------------------------
     async def query(self, sql, subs=None, why=None):
 
         if subs is None:
             subs = {}
 
         sql = self.__parameterize(sql, subs)
 
-        async with self.__cursor_lock:
-            async with self.__connection.cursor() as cursor:
-                try:
-                    cursor = await self.__connection.cursor()
-                    await cursor.execute(sql, subs)
-                    rows = await cursor.fetchall()
-                    cols = []
-                    for col in cursor.description:
-                        cols.append(col[0])
+        async with self.__connection.cursor() as cursor:
+            try:
+                cursor = await self.__connection.cursor()
+                await cursor.execute(sql, subs)
+                rows = await cursor.fetchall()
+                cols = []
+                for col in cursor.description:
+                    cols.append(col[0])
 
-                    if why is None:
-                        logger.debug("%d records from: %s" % (len(rows), sql))
-                    else:
-                        logger.debug("%d records from %s: %s" % (len(rows), why, sql))
-                    records = []
-                    for row in rows:
-                        record = OrderedDict()
-                        for index, col in enumerate(cols):
-                            record[col] = row[index]
-                        records.append(record)
-                    return records
-                except (TypeError, aiomysql.OperationalError) as exception:
-                    if why is None:
-                        raise RuntimeError(explain(exception, f"executing {sql}"))
-                    else:
-                        raise RuntimeError(
-                            explain(exception, f"executing {why}: {sql}")
-                        )
+                if why is None:
+                    logger.debug("%d records from: %s" % (len(rows), sql))
+                else:
+                    logger.debug("%d records from %s: %s" % (len(rows), why, sql))
+                records = []
+                for row in rows:
+                    record = OrderedDict()
+                    for index, col in enumerate(cols):
+                        record[col] = row[index]
+                    records.append(record)
+                return records
+            except (TypeError, aiomysql.OperationalError) as exception:
+                if why is None:
+                    raise RuntimeError(explain(exception, f"executing {sql}"))
+                else:
+                    raise RuntimeError(explain(exception, f"executing {why}: {sql}"))
 
     # ----------------------------------------------------------------------------------------
     async def backup(self):
         """
         Back up database to timestamped location.
         """
```

### Comparing `dls-normsql-2.2.0/src/dls_normsql/aiosqlite.py` & `dls-normsql-2.3.0/src/dls_normsql/aiosqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,14 @@
 
         self.__backup_restore_lock = asyncio.Lock()
 
         # Last undo position.
         self.__last_restore = 0
 
     # ----------------------------------------------------------------------------------------
-    # In aiosqlite, autocommit is enabled by default, which means changes made to the database are automatically committed
-    # after each SQL statement execution. This behavior aligns with the common usage patterns in asynchronous programming,
-    # where individual database operations are often executed within a coroutine or an asynchronous function.
 
     async def connect(self, should_drop_database=False):
         """
         Connect to database at filename given in constructor.
         """
 
         async with connect_lock:
```

### Comparing `dls-normsql-2.2.0/src/dls_normsql/constants.py` & `dls-normsql-2.3.0/src/dls_normsql/constants.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/src/dls_normsql/databases.py` & `dls-normsql-2.3.0/src/dls_normsql/databases.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/src/dls_normsql/version.py` & `dls-normsql-2.3.0/src/dls_normsql/version.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/src/dls_normsql.egg-info/PKG-INFO` & `dls-normsql-2.3.0/src/dls_normsql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 2.2.0
-Summary: Normalized API over various sql libraries.
+Version: 2.3.0
+Summary: Normalized API over various sql libraries for consistency across multiple projects.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -204,59 +204,19 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://gitlab.diamond.ac.uk/kbp43231/dls-normsql
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 dls-normsql
 =======================================================================
 
-Normalized API over various sql libraries.
-
-Intended advantages:
-
-- common connection and set of sql commands
-- reusable library for consistency across multiple projects
-
-Installation
------------------------------------------------------------------------
-::
-
-    pip install git+https://gitlab.diamond.ac.uk/kbp43231/dls-normsql.git 
-
-    dls-normsql --version
-
-Documentation
------------------------------------------------------------------------
-
-See https://www.cs.diamond.ac.uk/dls-normsql for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/kbp43231/dls-normsql.git 
-    cd dls-normsql
-    virtualenv /scratch/$USER/venv/dls-normsql
-    source /scratch/$USER/venv/dls-normsql/bin/activate 
-    pip install -e .[dev]
-    make -f .dls-normsql/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/dls-normsql/build/html/index.html
-
-Topics for further documentation:
-
-- TODO list of improvements
-- change log
-
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
+Normalized API over various sql libraries for consistency across multiple projects.
```

### Comparing `dls-normsql-2.2.0/src/dls_normsql.egg-info/SOURCES.txt` & `dls-normsql-2.3.0/src/dls_normsql.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
 LICENSE
-README.rst
+README.md
 pyproject.toml
 .dae-devops/Makefile
 .dae-devops/prepare_git_dependencies.sh
 .dae-devops/project.yaml
 .dae-devops/docs/conventions.rst
 .dae-devops/docs/developing.rst
 .dae-devops/docs/devops.rst
 .dae-devops/docs/docs_structure.rst
+.dae-devops/docs/documenting.rst
 .dae-devops/docs/installing.rst
 .dae-devops/docs/testing.rst
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .github/CONTRIBUTING.rst
 .github/dependabot.yml
 .github/actions/install_requirements/action.yml
@@ -27,20 +28,32 @@
 .vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 docs/conf.py
 docs/index.rst
 docs/_static/css/custom.css
-docs/api/classes.rst
-docs/api/command_line.rst
-docs/api/index.rst
-docs/api/modules.rst
+docs/explanations/conventions.rst
+docs/explanations/docs_structure.rst
+docs/explanations/index.rst
+docs/explanations/todo.rst
+docs/how-to/developing.rst
+docs/how-to/devops.rst
+docs/how-to/documenting.rst
+docs/how-to/index.rst
+docs/how-to/installing.rst
+docs/how-to/testing.rst
 docs/images/dls-favicon.ico
 docs/images/dls-logo.svg
+docs/reference/classes.rst
+docs/reference/command_line.rst
+docs/reference/index.rst
+docs/reference/modules.rst
+docs/tutorials/index.rst
+docs/tutorials/tbd.rst
 src/dls_normsql/__init__.py
 src/dls_normsql/__main__.py
 src/dls_normsql/_version.py
 src/dls_normsql/aiomysql.py
 src/dls_normsql/aiosqlite.py
 src/dls_normsql/constants.py
 src/dls_normsql/databases.py
```

### Comparing `dls-normsql-2.2.0/tests/base_tester.py` & `dls-normsql-2.3.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/tests/conftest.py` & `dls-normsql-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/tests/my_database_definition.py` & `dls-normsql-2.3.0/tests/my_database_definition.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/tests/my_table_definition.py` & `dls-normsql-2.3.0/tests/my_table_definition.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/tests/test_aiomysql.py` & `dls-normsql-2.3.0/tests/test_aiomysql.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/tests/test_backup_restore.py` & `dls-normsql-2.3.0/tests/test_backup_restore.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/tests/test_database.py` & `dls-normsql-2.3.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.2.0/tests/test_revision.py` & `dls-normsql-2.3.0/tests/test_revision.py`

 * *Files identical despite different names*

