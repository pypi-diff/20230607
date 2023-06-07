# Comparing `tmp/dls-servbase-1.6.0.tar.gz` & `tmp/dls-servbase-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-servbase-1.6.0.tar", last modified: Tue Jun  6 10:15:12 2023, max compression
+gzip compressed data, was "dls-servbase-1.7.0.tar", last modified: Wed Jun  7 14:24:08 2023, max compression
```

## Comparing `dls-servbase-1.6.0.tar` & `dls-servbase-1.7.0.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.735133 dls-servbase-1.6.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.735133 dls-servbase-1.6.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.735133 dls-servbase-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/src/dls_servbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/src/dls_servbase_api/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/src/dls_servbase_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_api/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30611 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/cookie_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/dataface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/src/dls_servbase_lib/guis/html/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/src/dls_servbase_lib/guis/html/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/html/javascript/version.js
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/configurations/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/configurations/sqlite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_dataface_takeover.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_parse_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.635095 dls-servbase-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.603094 dls-servbase-1.7.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.603094 dls-servbase-1.7.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.603094 dls-servbase-1.7.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.603094 dls-servbase-1.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.599094 dls-servbase-1.7.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.603094 dls-servbase-1.7.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-07 14:24:08.631095 dls-servbase-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.599094 dls-servbase-1.7.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.611095 dls-servbase-1.7.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.611095 dls-servbase-1.7.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.611095 dls-servbase-1.7.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.611095 dls-servbase-1.7.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:24:08.635095 dls-servbase-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.599094 dls-servbase-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.611095 dls-servbase-1.7.0/src/dls_servbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_api/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.619095 dls-servbase-1.7.0/src/dls_servbase_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30611 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.619095 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/cookie_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/dataface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.623095 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.623095 dls-servbase-1.7.0/src/dls_servbase_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.623095 dls-servbase-1.7.0/src/dls_servbase_lib/guis/html/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.627095 dls-servbase-1.7.0/src/dls_servbase_lib/guis/html/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/html/javascript/version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.627095 dls-servbase-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.631095 dls-servbase-1.7.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/configurations/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/configurations/sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_dataface_takeover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_parse_cookie.py
```

### Comparing `dls-servbase-1.6.0/.dae-devops/Makefile` & `dls-servbase-1.7.0/.dae-devops/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint 2d453caef2662f6d4cfd06d459312f02
+# dae_devops_fingerprint 7a40fdc6afce4991715aeda7ae70c444
```

### Comparing `dls-servbase-1.6.0/.dae-devops/docs/conventions.rst` & `dls-servbase-1.7.0/.dae-devops/docs/conventions.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 Naming conventions
 =======================================================================
 
 Here are the naming conventions used within the source code.
 
@@ -27,8 +27,8 @@
 python packages
     lowercase, underscores
 
 repository
     lowercase, hyphens
 
 
-.. # dae_devops_fingerprint 377aec0d2a3859ddaaadcf7d54438742
+.. # dae_devops_fingerprint cbd0a78343b6577aa4ddb9d59a242b04
```

### Comparing `dls-servbase-1.6.0/.dae-devops/docs/developing.rst` & `dls-servbase-1.7.0/.dae-devops/docs/developing.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
@@ -24,8 +24,8 @@
 
     $ cd dls-servbase
     $ pip install -e .[dev,docs]
 
 Now you may begin modifying the code.
 
 
-.. # dae_devops_fingerprint 0fd7e3e20b23c566fad722262ab9f97a
+.. # dae_devops_fingerprint 382b21157de1abc87034e692cbcabaf2
```

### Comparing `dls-servbase-1.6.0/.dae-devops/docs/devops.rst` & `dls-servbase-1.7.0/.dae-devops/docs/devops.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 Devops
 =======================================================================
 
 In the top level of the repository there exists a configuration file called ``.dae-devops/project.yaml``.
 
@@ -40,8 +40,8 @@
 Publishing (for the Diamond intranet)::
 
     $ make -f .dae-devops/Makefile publish_pip
     $ make -f .dae-devops/Makefile publish_docs
     
 The Diamond intranet commands are not used for production. The production packaging and publishing are handled in the GitHub Actions workflows mechanism.
 
-.. # dae_devops_fingerprint e8dff03fd491f40bda262817af6bf646
+.. # dae_devops_fingerprint 84e8a32100211cbba64804a3e5c5b337
```

### Comparing `dls-servbase-1.6.0/.dae-devops/docs/docs_structure.rst` & `dls-servbase-1.7.0/.dae-devops/docs/docs_structure.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 About the documentation
 -----------------------
 
   :material-regular:`format_quote;2em`
 
@@ -17,8 +17,8 @@
 They are: *tutorials*, *how-to guides*, *technical reference* and *explanation*.
 They represent four different purposes or functions, and require four different
 approaches to their creation. Understanding the implications of this will help
 improve most documentation - often immensely.
 
 `More information on this topic. <https://documentation.divio.com>`_
 
-.. # dae_devops_fingerprint 505d623863ca025fcddb20fe31db39d4
+.. # dae_devops_fingerprint 6ef08be920f12050c1c579cf6e9d4253
```

### Comparing `dls-servbase-1.6.0/.dae-devops/docs/documenting.rst` & `dls-servbase-1.7.0/.dae-devops/docs/documenting.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 Documenting
 =======================================================================
 
 If you plan to make update the documentation in this repository, you can use the steps below.
 
@@ -23,8 +23,8 @@
     file:///<your development area>/dls-servbase/build/html/index.html
 
 When you push either the main branch or a tag to GitHub, the documents are built and published automatically to this url::
 
     https://diamondlightsource.github.io/dls-servbase/main/index.html
 
 
-.. # dae_devops_fingerprint 850546fd7c3118fca1955e370bee4fc6
+.. # dae_devops_fingerprint d453f7183dae2edc0cf03aec47ef5c36
```

### Comparing `dls-servbase-1.6.0/.dae-devops/docs/installing.rst` & `dls-servbase-1.7.0/.dae-devops/docs/installing.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 Installing
 =======================================================================
 
 
 You will need python 3.10 or later. 
@@ -35,8 +35,8 @@
 
 The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ dls-servbase --version
     $ dls-servbase --version-json
 
-.. # dae_devops_fingerprint f5c12f1646c65db4968cb1f7cc1306d0
+.. # dae_devops_fingerprint b97a5d420f58e39a53c0a12e14d49e59
```

### Comparing `dls-servbase-1.6.0/.dae-devops/docs/testing.rst` & `dls-servbase-1.7.0/.dae-devops/docs/testing.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 Testing
 =======================================================================
 
 The package uses pytest for unit testing.
 
@@ -27,8 +27,8 @@
 
 The tests clear their directory when they start, but not when they finish.
 This allows you to examine what's been written by the test.
 
     
 
 
-.. # dae_devops_fingerprint 197b7a99ae5cd1520d710ad36ebd4236
+.. # dae_devops_fingerprint 139490d56d4a834f3de38d7da4db71bb
```

### Comparing `dls-servbase-1.6.0/.dae-devops/project.yaml` & `dls-servbase-1.7.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/.devcontainer/Dockerfile` & `dls-servbase-1.7.0/.devcontainer/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["dls-servbase"]
 CMD ["--version"]
 
-# dae_devops_fingerprint 0534faa0b5641c6bf5a6865dc868c633
+# dae_devops_fingerprint 80986671f8602f6e4666f78f98141826
```

### Comparing `dls-servbase-1.6.0/.devcontainer/devcontainer.json` & `dls-servbase-1.7.0/.devcontainer/devcontainer.json`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+// ********** It has been generated automatically by dae_devops version 0.5.3.
 // ********** For repository_name dls-servbase
 
 // For format details, see https://containers.dev/implementors/json_reference/
 {
     "name": "Python 3 Developer Container",
     "build": {
         "dockerfile": "Dockerfile",
@@ -53,8 +53,8 @@
     // make the workspace folder the same inside and outside of the container
     "workspaceMount": "source=${localWorkspaceFolder},target=${localWorkspaceFolder},type=bind",
     "workspaceFolder": "${localWorkspaceFolder}",
     // After the container is created, install the python project in editable form
     "postCreateCommand": "pip install -e .[dev]"
 }
 
-// dae_devops_fingerprint 41cc023010f4dbc2a199785da970798f
+// dae_devops_fingerprint 35358278c2556f05447815a0833301dc
```

### Comparing `dls-servbase-1.6.0/.github/CONTRIBUTING.rst` & `dls-servbase-1.7.0/.github/CONTRIBUTING.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/dls-servbase/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint 5554a59e62e5009c44a967ba6a56e3ea
+.. # dae_devops_fingerprint 0f4cbc1f77b787f03a9a4d268ed08055
```

### Comparing `dls-servbase-1.6.0/.github/actions/install_requirements/action.yml` & `dls-servbase-1.7.0/.github/actions/install_requirements/action.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 name: Install requirements
 description: Run pip install with requirements and upload resulting requirements
 inputs:
   requirements_file:
     description: Name of requirements file to use and upload
@@ -57,8 +57,8 @@
             echo "Error: ${{ inputs.requirements_file }} need the above changes to be exhaustive"
             exit 1
           fi
         fi
       shell: bash
 
 
-# dae_devops_fingerprint 967212425bc2c65a1fcab3e8aaacd538
+# dae_devops_fingerprint 492458ca501cde9a298a80a102ff22a4
```

### Comparing `dls-servbase-1.6.0/.github/dependabot.yml` & `dls-servbase-1.7.0/.github/dependabot.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 # To get started with Dependabot version updates, you'll need to specify which
 # package ecosystems to update and where the package manifests are located.
 # Please see the documentation for all configuration options:
 # https://docs.github.com/github/administering-a-repository/configuration-options-for-dependency-updates
 
@@ -15,8 +15,8 @@
       interval: "weekly"
 
   - package-ecosystem: "pip"
     directory: "/"
     schedule:
       interval: "weekly"
 
-# dae_devops_fingerprint f3e273cc476ab516308a7a53ad8e30c6
+# dae_devops_fingerprint b5838c5e0d9b5041500c5cb701fb5e5b
```

### Comparing `dls-servbase-1.6.0/.github/pages/make_switcher.py` & `dls-servbase-1.7.0/.github/pages/make_switcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 import json
 import logging
 from argparse import ArgumentParser
 from pathlib import Path
 from subprocess import CalledProcessError, check_output
@@ -98,8 +98,8 @@
     versions = get_versions("origin/gh-pages", args.add, args.remove)
     write_json(args.output, args.repository, versions)
 
 
 if __name__ == "__main__":
     main()
 
-# dae_devops_fingerprint b0c90a9621cff9b99133ac54ac310ade
+# dae_devops_fingerprint 7a1b58b851c5198d7d380e4ab78d0b49
```

### Comparing `dls-servbase-1.6.0/.github/workflows/code.yml` & `dls-servbase-1.7.0/.github/workflows/code.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 name: Code CI
 
 on:
   push:
   pull_request:
@@ -207,8 +207,8 @@
 
       - name: Publish to PyPI
         if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
 
-# dae_devops_fingerprint 20cc3e951a4652adfe1bdb16f0746054
+# dae_devops_fingerprint 66f0e76ce29e7f64d1ef000bebeb3d8b
```

### Comparing `dls-servbase-1.6.0/.github/workflows/docs.yml` & `dls-servbase-1.7.0/.github/workflows/docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 name: Docs CI
 
 on:
   push:
   pull_request:
@@ -52,8 +52,8 @@
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
         uses: peaceiris/actions-gh-pages@bd8c6b06eba6b3d25d72b7a1767993c0aeee42e7 # v3.9.2
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
 
-# dae_devops_fingerprint e20397fc0e4761c7e1a235ec1ea95642
+# dae_devops_fingerprint fb2dde86086783119d0b0b805151bf09
```

### Comparing `dls-servbase-1.6.0/.github/workflows/docs_clean.yml` & `dls-servbase-1.7.0/.github/workflows/docs_clean.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 name: Docs Cleanup CI
 
 # delete branch documentation when a branch is deleted
 # also allow manually deleting a documentation version
 on:
@@ -42,8 +42,8 @@
           rm -r $DOCS_VERSION
           python make_switcher.py --remove $DOCS_VERSION ${{ github.repository }} switcher.json
           git config --global user.name 'GitHub Actions Docs Cleanup CI'
           git config --global user.email 'GithubActionsCleanup@noreply.github.com'
           git commit -am "Removing redundant docs version $DOCS_VERSION"
           git push
 
-# dae_devops_fingerprint 1f0958e89021d3ef04512fb059911cf4
+# dae_devops_fingerprint d46d59a6f5197bd11b1cece615feb4df
```

### Comparing `dls-servbase-1.6.0/.gitignore` & `dls-servbase-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/.gitlab-ci.yml` & `dls-servbase-1.7.0/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 variables:
   # I put the package_pip artifacts int his place just until I can use the corporate internal pipserver.
   # Maybe /dls_sw/work/python3/RHEL7-x86_64/distributions would be a better place?
   PIP_FIND_LINKS: "/dls_sw/apps/bxflow/artifacts"
 
@@ -83,8 +83,8 @@
 
 # publish_docs:
 #   stage: publish
 #   script:
 #     # The validate_docs artifacts are in the build/html folder.
 #     - make -f .dae-devops/Makefile publish_docs
 
-# dae_devops_fingerprint 8c0d6830168b3a593396882beae5df6a
+# dae_devops_fingerprint 814043c19b1379f7f1d7b188546a7734
```

### Comparing `dls-servbase-1.6.0/.vscode/launch.json` & `dls-servbase-1.7.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/LICENSE` & `dls-servbase-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/PKG-INFO` & `dls-servbase-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.6.0
+Version: 1.7.0
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.6.0/docs/conf.py` & `dls-servbase-1.7.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
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
 
@@ -193,8 +193,8 @@
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint a8d7b8d65abc276648e440edf32e0454
+# dae_devops_fingerprint 6878b6b3f698c9be231083d88755956e
```

### Comparing `dls-servbase-1.6.0/docs/images/dls-favicon.ico` & `dls-servbase-1.7.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/docs/images/dls-logo.svg` & `dls-servbase-1.7.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/pyproject.toml` & `dls-servbase-1.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
@@ -96,8 +96,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint cde1577a97f0e28d7fd63100e14d53ab
+# dae_devops_fingerprint 25ba8f378cc5e02106bf918889322274
```

### Comparing `dls-servbase-1.6.0/src/dls_servbase.egg-info/PKG-INFO` & `dls-servbase-1.7.0/src/dls_servbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.6.0
+Version: 1.7.0
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.6.0/src/dls_servbase.egg-info/SOURCES.txt` & `dls-servbase-1.7.0/src/dls_servbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_api/aiohttp_client.py` & `dls-servbase-1.7.0/src/dls_servbase_api/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_api/databases/database_definition.py` & `dls-servbase-1.7.0/src/dls_servbase_api/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_api/databases/table_definitions.py` & `dls-servbase-1.7.0/src/dls_servbase_api/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_api/datafaces/aiohttp.py` & `dls-servbase-1.7.0/src/dls_servbase_api/datafaces/aiohttp.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,50 +26,91 @@
     # ----------------------------------------------------------------------------------------
     def specification(self):
         return self.__specification
 
     # ----------------------------------------------------------------------------------------
     async def query(self, sql, subs=None, why=None):
         """"""
-        return await self.__send_protocolj("query", sql, subs=subs, why=why)
+        return await self.__send_protocolj(
+            "query",
+            sql,
+            subs=subs,
+            why=why,
+        )
 
     # ----------------------------------------------------------------------------------------
     async def execute(self, sql, subs=None, why=None):
         """"""
-        return await self.__send_protocolj("execute", sql, subs=subs, why=why)
+        return await self.__send_protocolj(
+            "execute",
+            sql,
+            subs=subs,
+            why=why,
+            as_transaction=True,
+        )
 
     # ----------------------------------------------------------------------------------------
     async def insert(self, table_name, records, why=None):
         """"""
-        return await self.__send_protocolj("insert", table_name, records, why=why)
+        return await self.__send_protocolj(
+            "insert",
+            table_name,
+            records,
+            why=why,
+            as_transaction=True,
+        )
 
     # ----------------------------------------------------------------------------------------
-    async def update(self, table_name, record, where, subs=None, why=None):
+    async def update(
+        self,
+        table_name,
+        record,
+        where,
+        subs=None,
+        why=None,
+    ):
         """"""
         return await self.__send_protocolj(
-            "update", table_name, record, where, subs=subs, why=why
+            "update",
+            table_name,
+            record,
+            where,
+            subs=subs,
+            why=why,
+            as_transaction=True,
         )
 
     # ----------------------------------------------------------------------------------------
     async def set_cookie(self, cookie_dict):
         """ """
-        return await self.__send_protocolj("set_cookie", cookie_dict)
+        return await self.__send_protocolj(
+            "set_cookie",
+            cookie_dict,
+            as_transaction=True,
+        )
 
     # ----------------------------------------------------------------------------------------
     async def get_cookie(self, cookie_uuid):
         """
         Get single cookie from its uuid.
         Returns database record format.
         """
-        return await self.__send_protocolj("get_cookie", cookie_uuid)
+        return await self.__send_protocolj(
+            "get_cookie",
+            cookie_uuid,
+        )
 
     # ----------------------------------------------------------------------------------------
     async def update_cookie(self, row):
         """"""
-        return await self.__send_protocolj("update_cookie", row)
+        return await self.__send_protocolj(
+            "update_cookie",
+            row,
+            as_transaction=True,
+        )
 
     # ----------------------------------------------------------------------------------------
     async def __send_protocolj(self, function, *args, **kwargs):
         """"""
 
         return await self.client_protocolj(
             {
@@ -77,12 +118,7 @@
                 Keywords.PAYLOAD: {
                     "function": function,
                     "args": args,
                     "kwargs": kwargs,
                 },
             },
         )
-
-    # ----------------------------------------------------------------------------------------
-    async def report_health(self):
-        """"""
-        return await self.__send_protocolj("report_health")
```

### Comparing `dls-servbase-1.6.0/src/dls_servbase_api/datafaces/context.py` & `dls-servbase-1.7.0/src/dls_servbase_api/datafaces/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
         # If there is more than one dataface, the last one defined will be the default.
         dls_servbase_datafaces_set_default(self.interface)
 
         # Open client session to the service or direct connection.
         await self.interface.open_client_session()
 
+        # For convenience, return the object which is the client interface.
+        return self.interface
+
     # ----------------------------------------------------------------------------------------
     async def aexit(self):
         """ """
 
         if self.interface is not None:
             # Close client session to the service or direct connection.
             await self.interface.close_client_session()
```

### Comparing `dls-servbase-1.6.0/src/dls_servbase_api/datafaces/datafaces.py` & `dls-servbase-1.7.0/src/dls_servbase_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_api/guis/aiohttp.py` & `dls-servbase-1.7.0/src/dls_servbase_api/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_api/guis/context.py` & `dls-servbase-1.7.0/src/dls_servbase_api/guis/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_api/guis/guis.py` & `dls-servbase-1.7.0/src/dls_servbase_api/guis/guis.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_cli/main.py` & `dls-servbase-1.7.0/src/dls_servbase_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_cli/subcommands/base.py` & `dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_cli/subcommands/service.py` & `dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_cli/version.py` & `dls-servbase-1.7.0/src/dls_servbase_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/__main__.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/base_aiohttp.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/base_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/cookies/base.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/cookies/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/cookies/cookie_parser.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/cookies/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/cookies/cookies.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/cookies/cookies.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/cookies/dataface.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/cookies/dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/aiohttp.py` & `dls-servbase-1.7.0/tests/test_dataface_takeover.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,160 +1,112 @@
-import logging
-import multiprocessing
-import threading
-
-# Utilities.
-from dls_utilpack.callsign import callsign
-from dls_utilpack.explain import explain
-from dls_utilpack.require import require
-
-# Basic things.
-from dls_utilpack.thing import Thing
-
-# Class types.
-from dls_servbase_api.constants import ClassTypes
-
-# Dataface protocolj things.
-from dls_servbase_api.datafaces.constants import Commands, Keywords
-
-# Base class for an aiohttp server.
-from dls_servbase_lib.base_aiohttp import BaseAiohttp
-
-# Types of dls_servbase_dataface.
-# Global dls_servbase_dataface.
-from dls_servbase_lib.datafaces.datafaces import Datafaces
-
-logger = logging.getLogger(__name__)
-
-thing_type = ClassTypes.AIOHTTP
-
-
-# ------------------------------------------------------------------------------------------
-class Aiohttp(Thing, BaseAiohttp):
-    """
-    Object implementing remote procedure calls for dls_servbase_dataface methods.
-    """
-
-    # ----------------------------------------------------------------------------------------
-    def __init__(self, specification=None):
-        Thing.__init__(self, thing_type, specification)
-        BaseAiohttp.__init__(
-            self,
-            specification["type_specific_tbd"]["aiohttp_specification"],
-            calling_file=__file__,
-        )
-
-        self.__actual_dls_servbase_dataface = None
-
-    # ----------------------------------------------------------------------------------------
-    def callsign(self):
-        """"""
-        return "%s %s" % ("Servbase.Dataface", BaseAiohttp.callsign(self))
-
-    # ----------------------------------------------------------------------------------------
-    def activate_process(self):
-        """"""
-
-        try:
-            multiprocessing.current_process().name = "servbase-dataface"
-
-            self.activate_process_base()
-
-        except Exception as exception:
-            logger.exception(
-                f"unable to start {callsign(self)} process", exc_info=exception
-            )
-
-    # ----------------------------------------------------------------------------------------
-    def activate_thread(self, loop):
-        """
-        Called from inside a newly created thread.
-        """
-
-        try:
-            threading.current_thread().name = "servbase_dataface"
-
-            self.activate_thread_base(loop)
-
-        except Exception as exception:
-            logger.exception(
-                f"unable to start {callsign(self)} thread", exc_info=exception
-            )
-
-    # ----------------------------------------------------------------------------------------
-    async def activate_coro(self):
-        """"""
-        try:
-            # No special routes, we will use protocolj dispathcing only
-            route_tuples = []
-
-            # Build a local dls_servbase_dataface for our back-end.
-            self.__actual_dls_servbase_dataface = Datafaces().build_object(
-                self.specification()["type_specific_tbd"][
-                    "actual_dataface_specification"
-                ]
-            )
-
-            # Get the local implementation started.
-            await self.__actual_dls_servbase_dataface.start()
-
-            await self.activate_coro_base(route_tuples)
-
-        except Exception:
-            # We managed to get a dataface alive?
-            if self.__actual_dls_servbase_dataface is not None:
-                # Need to disconnect it so outer asyncio loop will quit.
-                logger.debug(
-                    f"[THRDIEP] {callsign(self)} disconnecting after failure to activate coro"
-                )
-
-                await self.__actual_dls_servbase_dataface.disconnect()
-
-            raise RuntimeError(f"{callsign(self)}  was unable to activate_coro")
-
-    # ----------------------------------------------------------------------------------------
-    async def direct_shutdown(self):
-        """"""
-        try:
-            # Disconnect our local dataface connection, i.e. the one which holds the database connection.
-            await self.__actual_dls_servbase_dataface.disconnect()
-
-        except Exception as exception:
-            raise RuntimeError(
-                callsign(
-                    self,
-                    explain(exception, "disconnecting local dls_servbase_dataface"),
-                )
-            )
-
-        # Let the base class stop the server listener.
-        await self.base_direct_shutdown()
-
-    # ----------------------------------------------------------------------------------------
-    async def __do_actually(self, function, args, kwargs):
-        """"""
-
-        # logger.info(describe("[CLIOPS] function", function))
-        # logger.info(describe("[CLIOPS] args", args))
-        # logger.info(describe("[CLIOPS] kwargs", kwargs))
-
-        function = getattr(self.__actual_dls_servbase_dataface, function)
-
-        response = await function(*args, **kwargs)
-
-        return response
-
-    # ----------------------------------------------------------------------------------------
-    async def dispatch(self, request_dict, opaque):
-        """"""
-
-        command = require("request json", request_dict, Keywords.COMMAND)
-
-        if command == Commands.EXECUTE:
-            payload = require("request json", request_dict, Keywords.PAYLOAD)
-            response = await self.__do_actually(
-                payload["function"], payload["args"], payload["kwargs"]
-            )
-        else:
-            raise RuntimeError("invalid command %s" % (command))
-
-        return response
+import logging
+
+from dls_servbase_api.databases.constants import CookieFieldnames, Tablenames
+from dls_servbase_api.datafaces.context import Context as ClientContext
+from dls_servbase_api.datafaces.datafaces import dls_servbase_datafaces_get_default
+from dls_servbase_lib.datafaces.context import Context as ServerContext
+
+# Base class for the tester.
+from tests.base_context_tester import BaseContextTester
+
+logger = logging.getLogger(__name__)
+
+
+# ----------------------------------------------------------------------------------------
+class TestDatafaceTakeoverSqlite:
+    def test(self, constants, logging_setup, output_directory):
+        """ """
+
+        configuration_file = "tests/configurations/sqlite.yaml"
+        DatafaceTakeoverTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestDatafaceTakeoverMysql:
+    """
+    Test that we can do a basic database operation through the service.
+    """
+
+    def test(self, constants, logging_setup, output_directory):
+        """ """
+
+        configuration_file = "tests/configurations/mysql.yaml"
+        DatafaceTakeoverTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class DatafaceTakeoverTester(BaseContextTester):
+    """
+    Class to test that a second instance of the dataface will cause the first one to shut down.
+    """
+
+    async def _main_coroutine(self, constants, output_directory):
+        """ """
+
+        dls_servbase_multiconf = self.get_multiconf()
+
+        context_configuration = await dls_servbase_multiconf.load()
+
+        servbase_specification = context_configuration[
+            "dls_servbase_dataface_specification"
+        ]
+
+        dls_servbase_client_context = ClientContext(servbase_specification)
+
+        dls_servbase_server_context = ServerContext(servbase_specification)
+
+        async with dls_servbase_client_context:
+            async with dls_servbase_server_context:
+                dataface = dls_servbase_datafaces_get_default()
+
+                # Write one record.
+                await dataface.insert(
+                    Tablenames.COOKIES,
+                    [
+                        {
+                            CookieFieldnames.UUID: "f0",
+                            CookieFieldnames.CONTENTS: "{'a': 'f000'}",
+                        }
+                    ],
+                )
+                all_sql = f"SELECT * FROM {Tablenames.COOKIES}"
+                records = await dataface.query(all_sql)
+
+                assert len(records) == 1
+                assert records[0][CookieFieldnames.UUID] == "f0"
+                assert records[0][CookieFieldnames.CONTENTS] == "{'a': 'f000'}"
+
+            # ----------------------------------------------------------------------------
+            # Make a new dataface context with the same specification, except don't drop.
+            servbase_specification["type_specific_tbd"][
+                "actual_dataface_specification"
+            ]["should_drop_database"] = False
+            dls_servbase_server_context = ServerContext(servbase_specification)
+            # Activate the new dataface which should send shutdown to the old process.
+            async with dls_servbase_server_context:
+                # Check the final insert made it to the database.
+                records = await dataface.query(all_sql)
+                assert len(records) == 1
+                assert records[0][CookieFieldnames.UUID] == "f0"
+                assert records[0][CookieFieldnames.CONTENTS] == "{'a': 'f000'}"
+
+                # Update the cookie record.
+                subs = []
+                subs.append("f0")
+                await dataface.update(
+                    Tablenames.COOKIES,
+                    {CookieFieldnames.CONTENTS: "{'a': 'f001'}"},
+                    f"{CookieFieldnames.UUID} = ?",
+                    subs=subs,
+                    why="update database revision",
+                )
+
+            # ----------------------------------------------------------------------------
+            # Make a new dataface context with the same specification, again without dropping.
+            dls_servbase_server_context = ServerContext(servbase_specification)
+            # Activate the new dataface which should send shutdown to the old process.
+            async with dls_servbase_server_context:
+                # Check the final update made it to the database.
+                records = await dataface.query(all_sql)
+                assert len(records) == 1
+                assert records[0][CookieFieldnames.UUID] == "f0"
+                assert records[0][CookieFieldnames.CONTENTS] == "{'a': 'f001'}"
```

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/context.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/datafaces.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/normsql.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/normsql.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,14 +151,35 @@
         return {
             "count": await self.__database.update(
                 table_name, record, where, subs=subs, why=why
             )
         }
 
     # ----------------------------------------------------------------------------------------
+    async def begin(self, why=None) -> None:
+        """"""
+        await self.establish_database_connection()
+
+        return await self.__database.begin()
+
+    # ----------------------------------------------------------------------------------------
+    async def commit(self, why=None) -> None:
+        """"""
+        await self.establish_database_connection()
+
+        return await self.__database.commit()
+
+    # ----------------------------------------------------------------------------------------
+    async def rollback(self, why=None) -> None:
+        """"""
+        await self.establish_database_connection()
+
+        return await self.__database.rollback()
+
+    # ----------------------------------------------------------------------------------------
     async def report_health(self):
         """"""
 
         report = {}
 
         report["alive"] = True
```

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/envvar.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/guis/aiohttp.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/guis/context.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/guis/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/guis/guis.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/guis/guis.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/src/dls_servbase_lib/version.py` & `dls-servbase-1.7.0/src/dls_servbase_lib/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/tests/base_context_tester.py` & `dls-servbase-1.7.0/tests/base_context_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/tests/base_tester.py` & `dls-servbase-1.7.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/tests/configurations/mysql.yaml` & `dls-servbase-1.7.0/tests/configurations/mysql.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/tests/configurations/sqlite.yaml` & `dls-servbase-1.7.0/tests/configurations/sqlite.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/tests/conftest.py` & `dls-servbase-1.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/tests/test_aiohttp.py` & `dls-servbase-1.7.0/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/tests/test_cli.py` & `dls-servbase-1.7.0/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import asyncio
 import logging
 import os
 import subprocess
 import time
 
+from dls_utilpack.describe import describe
+
 from dls_servbase_api.databases.constants import CookieFieldnames, Tablenames
 from dls_servbase_api.datafaces.context import Context as ClientContext
-from dls_servbase_api.datafaces.datafaces import dls_servbase_datafaces_get_default
 
 # Base class for the tester.
 from tests.base_context_tester import BaseContextTester
 
 logger = logging.getLogger(__name__)
 
 
@@ -84,75 +85,83 @@
             multiconf_dict = await multiconf_object.load()
 
             # Get a client context to the server in the process we just started.
             servbase_specification = multiconf_dict[
                 "dls_servbase_dataface_specification"
             ]
             dls_servbase_client_context = ClientContext(servbase_specification)
-            async with dls_servbase_client_context:
-                dataface = dls_servbase_datafaces_get_default()
-
+            async with dls_servbase_client_context as dls_servbase_client:
                 # Some easy sql query.
                 all_sql = f"SELECT * FROM {Tablenames.COOKIES}"
 
                 # Wait for process to be up.
                 start_time = time.time()
                 max_seconds = 5.0
                 while True:
-                    try:
-                        records = await dataface.query(all_sql)
+                    # Try to check the health.
+                    health = await dls_servbase_client.client_report_health()
+
+                    # Check if health report contains an exception.
+                    exception = health.get("exception")
+                    if exception is None:
+                        logger.debug(describe("health", health))
+                        # Continue with test if no exception.
                         break
-                    except Exception as exception:
-                        logger.debug(f"retrying after failure {exception}")
+
+                    logger.debug(f"[CONNRETRY] retrying after {exception}")
 
                     if process.poll() is not None:
                         raise RuntimeError(
-                            "server apprently died before first command worked"
+                            "server apprently died without being able to give a health check"
                         )
 
+                    # Too much time has elapsed?
                     if time.time() - start_time > max_seconds:
                         raise RuntimeError(
                             f"server not answering within {max_seconds} seconds"
                         )
 
                     await asyncio.sleep(1.0)
 
                 # Interact with it.
-                await dataface.insert(
+                await dls_servbase_client.insert(
                     Tablenames.COOKIES,
                     [
                         {
                             CookieFieldnames.UUID: "f0",
                             CookieFieldnames.CONTENTS: "{'a': 'f000'}",
                         }
                     ],
                 )
 
-                records = await dataface.query(all_sql)
+                records = await dls_servbase_client.query(all_sql)
 
                 assert len(records) == 1
                 assert records[0][CookieFieldnames.UUID] == "f0"
                 assert records[0][CookieFieldnames.CONTENTS] == "{'a': 'f000'}"
 
-                await dataface.client_shutdown()
+                await dls_servbase_client.client_shutdown()
         finally:
             try:
                 # Wait for the process to finish and get the output.
                 stdout_bytes, stderr_bytes = process.communicate(timeout=5)
             except subprocess.TimeoutExpired:
                 # Timeout happens when client dies but server hasn't been told to shutdown.
                 process.kill()
                 stdout_bytes, stderr_bytes = process.communicate()
 
             # Get the return code of the process
             return_code = process.returncode
             logger.debug(f"server return_code is {return_code}")
 
-            logger.debug(
-                f"================================== server stderr is:\n{stderr_bytes.decode()}"
-            )
-            logger.debug(
-                f"================================== server stdout is:\n{stdout_bytes.decode()}"
-            )
-            logger.debug("==================================")
+            if len(stderr_bytes) > 0:
+                logger.debug(
+                    f"================================== server stderr is:\n{stderr_bytes.decode()}"
+                )
+            if len(stdout_bytes) > 0:
+                logger.debug(
+                    f"================================== server stdout is:\n{stdout_bytes.decode()}"
+                )
+            if len(stderr_bytes) > 0 or len(stdout_bytes) > 0:
+                logger.debug("================================== end of server output")
 
         assert return_code == 0
```

### Comparing `dls-servbase-1.6.0/tests/test_database.py` & `dls-servbase-1.7.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/tests/test_dataface.py` & `dls-servbase-1.7.0/tests/test_dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/tests/test_gui.py` & `dls-servbase-1.7.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.6.0/tests/test_parse_cookie.py` & `dls-servbase-1.7.0/tests/test_parse_cookie.py`

 * *Files identical despite different names*

