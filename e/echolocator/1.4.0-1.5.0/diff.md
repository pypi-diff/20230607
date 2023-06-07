# Comparing `tmp/echolocator-1.4.0.tar.gz` & `tmp/echolocator-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echolocator-1.4.0.tar", last modified: Tue Jun  6 12:11:32 2023, max compression
+gzip compressed data, was "echolocator-1.5.0.tar", last modified: Wed Jun  7 04:53:07 2023, max compression
```

## Comparing `echolocator-1.4.0.tar` & `echolocator-1.5.0.tar`

### file list

```diff
@@ -1,218 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.724744 echolocator-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.704743 echolocator-1.4.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-06 12:11:24.000000 echolocator-1.4.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.704743 echolocator-1.4.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-06 12:11:24.000000 echolocator-1.4.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-06 12:11:24.000000 echolocator-1.4.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-06 12:11:24.000000 echolocator-1.4.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-06 12:11:24.000000 echolocator-1.4.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-06 12:11:24.000000 echolocator-1.4.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-06 12:11:24.000000 echolocator-1.4.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-06 12:11:24.000000 echolocator-1.4.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-06 12:11:24.000000 echolocator-1.4.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.704743 echolocator-1.4.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-06 12:11:24.000000 echolocator-1.4.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-06 12:11:24.000000 echolocator-1.4.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-06 12:11:24.000000 echolocator-1.4.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.700742 echolocator-1.4.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-06 12:11:24.000000 echolocator-1.4.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 12:11:24.000000 echolocator-1.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-06 12:11:24.000000 echolocator-1.4.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-06 12:11:24.000000 echolocator-1.4.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-06 12:11:24.000000 echolocator-1.4.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-06 12:11:24.000000 echolocator-1.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-06 12:11:24.000000 echolocator-1.4.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-06 12:11:24.000000 echolocator-1.4.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-06 12:11:24.000000 echolocator-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-06 12:11:24.000000 echolocator-1.4.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-06 12:11:24.000000 echolocator-1.4.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 12:11:24.000000 echolocator-1.4.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 12:11:24.000000 echolocator-1.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 12:11:24.000000 echolocator-1.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 12:11:24.000000 echolocator-1.4.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 12:11:24.000000 echolocator-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-06 12:11:24.000000 echolocator-1.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-06-06 12:11:32.724744 echolocator-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-06 12:11:24.000000 echolocator-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-06 12:11:24.000000 echolocator-1.4.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/docs/1_tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/1_tutorials/101_run_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/1_tutorials/102_update_image.rst
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/1_tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/docs/2_how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/2_how-to/201_add_fields.rst
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/2_how-to.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/docs/3_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/3_explanations/301_naming_conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/3_explanations/302_process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/3_explanations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/docs/4_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/4_reference/402_building_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/4_reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.708743 echolocator-1.4.0/docs/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/diagrams/3drop_texrank_coordinates.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.712743 echolocator-1.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/images/excalidraw-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/images/git_merge.png
--rw-r--r--   0 runner    (1001) docker     (123)   703604 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/images/image_details.png
--rw-r--r--   0 runner    (1001) docker     (123)   135258 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/images/image_list.png
--rw-r--r--   0 runner    (1001) docker     (123)   142461 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/images/swiss3.png
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-06 12:11:24.000000 echolocator-1.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.712743 echolocator-1.4.0/modulefiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-06 12:11:24.000000 echolocator-1.4.0/modulefiles/conda
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-06 12:11:24.000000 echolocator-1.4.0/modulefiles/paths
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-06 12:11:24.000000 echolocator-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:11:32.724744 echolocator-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.700742 echolocator-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.712743 echolocator-1.4.0/src/echolocator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-06-06 12:11:32.000000 echolocator-1.4.0/src/echolocator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-06-06 12:11:32.000000 echolocator-1.4.0/src/echolocator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:11:32.000000 echolocator-1.4.0/src/echolocator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 12:11:32.000000 echolocator-1.4.0/src/echolocator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-06 12:11:32.000000 echolocator-1.4.0/src/echolocator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 12:11:32.000000 echolocator-1.4.0/src/echolocator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.712743 echolocator-1.4.0/src/echolocator_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.712743 echolocator-1.4.0/src/echolocator_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.712743 echolocator-1.4.0/src/echolocator_api/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_api/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_api/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_api/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_api/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_api/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.712743 echolocator-1.4.0/src/echolocator_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.712743 echolocator-1.4.0/src/echolocator_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.716743 echolocator-1.4.0/src/echolocator_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 12:11:32.000000 echolocator-1.4.0/src/echolocator_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.716743 echolocator-1.4.0/src/echolocator_lib/composers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/composers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/composers/composers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/composers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/composers/prettyhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/composers/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.716743 echolocator-1.4.0/src/echolocator_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.716743 echolocator-1.4.0/src/echolocator_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28861 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.716743 echolocator-1.4.0/src/echolocator_lib/guis/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.716743 echolocator-1.4.0/src/echolocator_lib/guis/html/css/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/css/image_edit_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/css/image_list_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.716743 echolocator-1.4.0/src/echolocator_lib/guis/html/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/css/pixel_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/css/plate_list_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/css/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/css/system_health_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.716743 echolocator-1.4.0/src/echolocator_lib/guis/html/images/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/images/radial1.666.png
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.716743 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.716743 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/common/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.720744 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/events.js
--rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/page.js
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/plate_list_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.700742 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.720744 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.704743 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.720744 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.704743 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.720744 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.720744 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.704743 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/raphael/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.720744 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/runtime.js
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/version.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.720744 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.720744 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/hair/
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.720744 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-06 12:11:24.000000 echolocator-1.4.0/src/echolocator_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.724744 echolocator-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.724744 echolocator-1.4.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27821 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/configurations/store.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.724744 echolocator-1.4.0/tests/example_images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/example_images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/example_images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/example_images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/example_images/4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:11:32.724744 echolocator-1.4.0/tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/test_droplocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/test_export_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/test_export_to_soakdb3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/test_fetch_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/test_fetch_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-06 12:11:24.000000 echolocator-1.4.0/tests/test_report_plates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.566571 echolocator-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-07 04:52:58.000000 echolocator-1.5.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-07 04:52:58.000000 echolocator-1.5.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-07 04:52:58.000000 echolocator-1.5.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-07 04:52:58.000000 echolocator-1.5.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-07 04:52:58.000000 echolocator-1.5.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-07 04:52:58.000000 echolocator-1.5.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-07 04:52:58.000000 echolocator-1.5.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-07 04:52:58.000000 echolocator-1.5.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-07 04:52:58.000000 echolocator-1.5.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-07 04:52:58.000000 echolocator-1.5.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-07 04:52:58.000000 echolocator-1.5.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-07 04:52:58.000000 echolocator-1.5.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-07 04:52:58.000000 echolocator-1.5.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.538570 echolocator-1.5.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-07 04:52:58.000000 echolocator-1.5.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-07 04:52:58.000000 echolocator-1.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-07 04:52:58.000000 echolocator-1.5.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-07 04:52:58.000000 echolocator-1.5.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-07 04:52:58.000000 echolocator-1.5.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-07 04:52:58.000000 echolocator-1.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-07 04:52:58.000000 echolocator-1.5.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-07 04:52:58.000000 echolocator-1.5.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-07 04:52:58.000000 echolocator-1.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-07 04:52:58.000000 echolocator-1.5.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-07 04:52:58.000000 echolocator-1.5.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-07 04:52:58.000000 echolocator-1.5.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-07 04:52:58.000000 echolocator-1.5.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 04:52:58.000000 echolocator-1.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 04:52:58.000000 echolocator-1.5.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 04:52:58.000000 echolocator-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-07 04:52:58.000000 echolocator-1.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-07 04:53:07.566571 echolocator-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 04:52:58.000000 echolocator-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-07 04:52:58.000000 echolocator-1.5.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.538570 echolocator-1.5.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.546570 echolocator-1.5.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.550570 echolocator-1.5.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.550570 echolocator-1.5.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.550570 echolocator-1.5.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-07 04:52:58.000000 echolocator-1.5.0/docs/tutorials/tbd.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.550570 echolocator-1.5.0/modulefiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-07 04:52:58.000000 echolocator-1.5.0/modulefiles/conda
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-07 04:52:58.000000 echolocator-1.5.0/modulefiles/paths
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-07 04:52:58.000000 echolocator-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 04:53:07.566571 echolocator-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.542570 echolocator-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.550570 echolocator-1.5.0/src/echolocator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-07 04:53:07.000000 echolocator-1.5.0/src/echolocator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-07 04:53:07.000000 echolocator-1.5.0/src/echolocator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:53:07.000000 echolocator-1.5.0/src/echolocator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-07 04:53:07.000000 echolocator-1.5.0/src/echolocator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-07 04:53:07.000000 echolocator-1.5.0/src/echolocator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 04:53:07.000000 echolocator-1.5.0/src/echolocator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.550570 echolocator-1.5.0/src/echolocator_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.550570 echolocator-1.5.0/src/echolocator_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.550570 echolocator-1.5.0/src/echolocator_api/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_api/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_api/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_api/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_api/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_api/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.550570 echolocator-1.5.0/src/echolocator_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.554570 echolocator-1.5.0/src/echolocator_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.554570 echolocator-1.5.0/src/echolocator_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 04:53:07.000000 echolocator-1.5.0/src/echolocator_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.554570 echolocator-1.5.0/src/echolocator_lib/composers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/composers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/composers/composers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/composers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/composers/prettyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/composers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.554570 echolocator-1.5.0/src/echolocator_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28857 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.554570 echolocator-1.5.0/src/echolocator_lib/guis/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.554570 echolocator-1.5.0/src/echolocator_lib/guis/html/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/css/image_edit_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/css/image_list_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.554570 echolocator-1.5.0/src/echolocator_lib/guis/html/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/css/pixel_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/css/plate_list_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/css/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/css/system_health_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.554570 echolocator-1.5.0/src/echolocator_lib/guis/html/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/images/radial1.666.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.554570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.558570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/common/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.558570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/events.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/plate_list_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.542570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.558570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.542570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.558570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.542570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.558570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.562570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.542570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/raphael/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.562570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/runtime.js
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/version.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.562570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.562570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/hair/
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.562570 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-07 04:52:58.000000 echolocator-1.5.0/src/echolocator_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.562570 echolocator-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.562570 echolocator-1.5.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27821 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/configurations/store.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.562570 echolocator-1.5.0/tests/example_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/example_images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/example_images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/example_images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/example_images/4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:53:07.562570 echolocator-1.5.0/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/test_droplocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/test_export_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/test_export_to_soakdb3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/test_fetch_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/test_fetch_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-07 04:52:58.000000 echolocator-1.5.0/tests/test_report_plates.py
```

### Comparing `echolocator-1.4.0/.dae-devops/Makefile` & `echolocator-1.5.0/.dae-devops/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name echolocator
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint e508c365997a16fba9003f0e2c7345fc
+# dae_devops_fingerprint 95094fd1d3f3c345a482a1c91ca87334
```

### Comparing `echolocator-1.4.0/.dae-devops/docs/conventions.rst` & `echolocator-1.5.0/.dae-devops/docs/conventions.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name echolocator
 
 Naming conventions
 =======================================================================
 
 Here are the naming conventions used within the source code.
 
@@ -27,8 +27,8 @@
 python packages
     lowercase, underscores
 
 repository
     lowercase, hyphens
 
 
-.. # dae_devops_fingerprint f1b13dc77352fa3d7806ebc008156e6f
+.. # dae_devops_fingerprint 3d3fc8778c1377ea19870bc6c53aae82
```

### Comparing `echolocator-1.4.0/.dae-devops/docs/developing.rst` & `echolocator-1.5.0/.dae-devops/docs/developing.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name echolocator
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
 Clone the repository::
 
+    $ cd <your development area>
     $ git clone https://gitlab.diamond.ac.uk/xchem/echolocator.git
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software.
-Make sure to have at least python version 3.9 then::
+Make sure to have at least python version 3.10 then::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd echolocator
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
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
-.. # dae_devops_fingerprint 8802592ab610cd9de3e657aeacb9c8c1
+.. # dae_devops_fingerprint 1787c6400e18669161c7a554629587de
```

### Comparing `echolocator-1.4.0/.dae-devops/docs/docs_structure.rst` & `echolocator-1.5.0/.dae-devops/docs/docs_structure.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name echolocator
 
 About the documentation
 -----------------------
 
   :material-regular:`format_quote;2em`
 
@@ -17,8 +17,8 @@
 They are: *tutorials*, *how-to guides*, *technical reference* and *explanation*.
 They represent four different purposes or functions, and require four different
 approaches to their creation. Understanding the implications of this will help
 improve most documentation - often immensely.
 
 `More information on this topic. <https://documentation.divio.com>`_
 
-.. # dae_devops_fingerprint 58611b915d52f7b59bbed09020e30356
+.. # dae_devops_fingerprint 694da572ea0f17cfcb8cc0957fc89d42
```

### Comparing `echolocator-1.4.0/.dae-devops/docs/installing.rst` & `echolocator-1.5.0/.dae-devops/docs/installing.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name echolocator
 
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
 
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
     $ python3 -m pip install echolocator
 
-If you require a feature that is not currently released you can also install
+If you require a feature that is not currently released, you can also install
 from git::
 
     $ python3 -m pip install git+https://gitlab.diamond.ac.uk/xchem/echolocator.git
 
-The library should now be installed and the commandline interface on your path.
+The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ echolocator --version
     $ echolocator --version-json
 
-.. # dae_devops_fingerprint c6472f1053e4ee44f3e70cc67c9fbddd
+.. # dae_devops_fingerprint 63057ec638dd81e8434ea6f4b7c44ef9
```

### Comparing `echolocator-1.4.0/.dae-devops/docs/testing.rst` & `echolocator-1.5.0/.dae-devops/docs/testing.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name echolocator
 
 Testing
 =======================================================================
 
 The package uses pytest for unit testing.
 
 If you want to run the tests, first get a copy of the code per the instructions in the Developing section.
 
 Then you can run all tests by::
 
-    $ pytest
-
-Or this, which is the command used by the CI runner.
-
-    $ make -f .dae-devops/Makefile validate_pytest
+    $ tox -q -e pytest
 
 To run a single test you can do::
 
     $ pytest tests/the_test_you_want.py
 
-If you want to see more output of the test while it's running you can do:
+If you want to see more output of the test while it's running you can do::
 
     $ pytest -sv -ra --tb=line tests/the_test_you_want.py
 
 Each test will write files into its own directory::
 
-    /tmp/echolocator/tests/....
+    /tmp/echolocator/tests/*
 
 The tests clear their directory when they start, but not when they finish.
-This allows peeking in there to see what's been written by the test.
+This allows you to examine what's been written by the test.
 
     
 
 
-.. # dae_devops_fingerprint 7daed3c9e65a523a0fbf7d347dfa6ebe
+.. # dae_devops_fingerprint d3dc8494ee0c6b7dfc924ee704e64c79
```

### Comparing `echolocator-1.4.0/.dae-devops/project.yaml` & `echolocator-1.5.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/.devcontainer/Dockerfile` & `echolocator-1.5.0/.devcontainer/Dockerfile`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name echolocator
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["echolocator"]
 CMD ["--version"]
 
-# dae_devops_fingerprint 9302e007f97570a60d29bb25449a92bb
+# dae_devops_fingerprint 366b50795b8545b74defed75fb1ba9e9
```

### Comparing `echolocator-1.4.0/.devcontainer/devcontainer.json` & `echolocator-1.5.0/.devcontainer/devcontainer.json`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.2.
+// ********** It has been generated automatically by dae_devops version 0.5.3.
 // ********** For repository_name echolocator
 
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
 
-// dae_devops_fingerprint 529b4c792a9fdad91835e1a4b32e0138
+// dae_devops_fingerprint ab68bbbf41d5a201de3278cef1da11ac
```

### Comparing `echolocator-1.4.0/.github/CONTRIBUTING.rst` & `echolocator-1.5.0/.github/CONTRIBUTING.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name echolocator
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/echolocator/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint d17faed109d26c120150d4cad9b012bd
+.. # dae_devops_fingerprint b624a2401d1f7c71d1b7a645d80c81c4
```

### Comparing `echolocator-1.4.0/.github/actions/install_requirements/action.yml` & `echolocator-1.5.0/.github/actions/install_requirements/action.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name echolocator
 
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
 
 
-# dae_devops_fingerprint 1fae1b6e8b391bfca7aad4310624e6c4
+# dae_devops_fingerprint 94559b5e936b574b2379a365653896bc
```

### Comparing `echolocator-1.4.0/.github/pages/make_switcher.py` & `echolocator-1.5.0/.github/pages/make_switcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name echolocator
 
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
 
-# dae_devops_fingerprint e707603d7cbd385a51462ce91214bed6
+# dae_devops_fingerprint b1cf83c6a3f4e6e3b0b8179dc6117147
```

### Comparing `echolocator-1.4.0/.github/workflows/code.yml` & `echolocator-1.5.0/.github/workflows/code.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name echolocator
 
 name: Code CI
 
 on:
   push:
   pull_request:
@@ -35,21 +35,16 @@
 
   test:
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
-        python: ["3.10", "3.11"]
+        python: ["3.10"]
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
@@ -65,14 +60,18 @@
           python_version: ${{ matrix.python }}
           requirements_file: requirements-test-${{ matrix.os }}-${{ matrix.python }}.txt
           install_options: ${{ matrix.install }}
 
       - name: List dependency tree
         run: pipdeptree
 
+      # TODO: Make startup of MySQL able to be configured.
+      - name: Start up the MySQL that comes with Unbuntu
+        run: sudo /etc/init.d/mysql start
+
       - name: Run tests
         run: |
           sudo apt install environment-modules
           export MODULESHOME=/usr/share/modules
           source $MODULESHOME/init/bash
           pytest
 
@@ -208,8 +207,8 @@
 
       - name: Publish to PyPI
         if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
 
-# dae_devops_fingerprint febe27315441a7232f0895dff16de450
+# dae_devops_fingerprint 5da612bfb00d4d9148e19ade99749411
```

### Comparing `echolocator-1.4.0/.github/workflows/docs.yml` & `echolocator-1.5.0/.github/workflows/docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name echolocator
 
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
 
-# dae_devops_fingerprint 248b6927066389c57cb985f999015228
+# dae_devops_fingerprint d9f015515d78bcb8b6c8f4142e280eab
```

### Comparing `echolocator-1.4.0/.github/workflows/docs_clean.yml` & `echolocator-1.5.0/.github/workflows/docs_clean.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name echolocator
 
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
 
-# dae_devops_fingerprint 13b4db6f5b6317157d8d36b632434d2d
+# dae_devops_fingerprint b7ffd3d8dcdf6b3d3cb583a1753ece53
```

### Comparing `echolocator-1.4.0/.gitignore` & `echolocator-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/.gitlab-ci.yml` & `echolocator-1.5.0/.gitlab-ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name echolocator
 
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
 
-# dae_devops_fingerprint 14d3e80d54ae3da9497b0ce79d6fa611
+# dae_devops_fingerprint 8aaa3a95f94e1c0ec255f133dea1c40a
```

### Comparing `echolocator-1.4.0/.vscode/launch.json` & `echolocator-1.5.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/LICENSE` & `echolocator-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/Makefile` & `echolocator-1.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/PKG-INFO` & `echolocator-1.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.4.0
+Version: 1.5.0
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,42 +204,24 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://gitlab.diamond.ac.uk/xchem/echolocator
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
 
-===========================
 echolocator
-===========================
+=======================================================================
 
 XChem GUI for manually targeting drop points for the Echo dispenser.
 
-.. image:: images/image_details.png
-    :width: 400
-    :alt: Image edit tab.
+Contains both backend server and front end html/javascript.
 
+Uses xchembku for database interaction.
 
----------------------------
-Table of contents
----------------------------
-
-..
-    Anything below this line is used only when viewing README.rst on Gitlab.
-    It will be ingored when included in index.rst
-
----------------------------
-Viewing the docs
----------------------------
-
-You can view the docs from Diamond's internal server
-
-    https://diamondlightsource.github.io/echolocator
+For documentation see: https://diamondlightsource.github.io/echolocator
```

### Comparing `echolocator-1.4.0/configurations/development.yaml` & `echolocator-1.5.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/docs/conf.py` & `echolocator-1.5.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name echolocator
 
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
 
@@ -184,17 +184,17 @@
 
 # I got this from https://github.com/sphinx-doc/sphinx/issues/4054.
 # It will allow the ${token} replacement in the rst documents.
 ultimate_replacements = {
     "$" + "{repository_name}": "echolocator",
     "$" + "{package_name}": "echolocator_lib",
     "$" + "{git_url}": "https://gitlab.diamond.ac.uk/xchem",
-    "$" + "{python_version_at_least}": "3.9",
+    "$" + "{python_version_at_least}": "3.10",
 }
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 522695c29baed7676543987e99fc61dd
+# dae_devops_fingerprint 03014300546e31a10942329f91438b95
```

### Comparing `echolocator-1.4.0/docs/images/dls-favicon.ico` & `echolocator-1.5.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/docs/images/dls-logo.svg` & `echolocator-1.5.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/modulefiles/conda` & `echolocator-1.5.0/modulefiles/conda`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/pyproject.toml` & `echolocator-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name echolocator
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "echolocator"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
 ]
 description = "XChem GUI for manually targeting drop points for the Echo dispenser."
 dependencies = ["xchembku", "dls_servbase", "dls_mainiac", "dls_utilpack", "beautifulsoup4"]
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
@@ -99,8 +97,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint 8d6ec2f437b47d4156e639a67957fdc1
+# dae_devops_fingerprint f039ca194f8add3d50810a4e9d62fab2
```

### Comparing `echolocator-1.4.0/src/echolocator.egg-info/PKG-INFO` & `echolocator-1.5.0/src/echolocator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.4.0
+Version: 1.5.0
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,42 +204,24 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://gitlab.diamond.ac.uk/xchem/echolocator
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
 
-===========================
 echolocator
-===========================
+=======================================================================
 
 XChem GUI for manually targeting drop points for the Echo dispenser.
 
-.. image:: images/image_details.png
-    :width: 400
-    :alt: Image edit tab.
+Contains both backend server and front end html/javascript.
 
+Uses xchembku for database interaction.
 
----------------------------
-Table of contents
----------------------------
-
-..
-    Anything below this line is used only when viewing README.rst on Gitlab.
-    It will be ingored when included in index.rst
-
----------------------------
-Viewing the docs
----------------------------
-
-You can view the docs from Diamond's internal server
-
-    https://diamondlightsource.github.io/echolocator
+For documentation see: https://diamondlightsource.github.io/echolocator
```

### Comparing `echolocator-1.4.0/src/echolocator.egg-info/SOURCES.txt` & `echolocator-1.5.0/src/echolocator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
 LICENSE
 Makefile
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
@@ -26,47 +27,45 @@
 .github/workflows/docs_clean.yml
 .github/workflows/linkcheck.yml
 .vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 configurations/development.yaml
-docs/1_tutorials.rst
-docs/2_how-to.rst
-docs/3_explanations.rst
-docs/4_reference.rst
 docs/conf.py
 docs/index.rst
-docs/1_tutorials/101_run_conda.rst
-docs/1_tutorials/102_update_image.rst
-docs/2_how-to/201_add_fields.rst
-docs/3_explanations/301_naming_conventions.rst
-docs/3_explanations/302_process.rst
-docs/4_reference/402_building_conda.rst
-docs/_static/theme_overrides.css
 docs/_static/css/custom.css
-docs/diagrams/3drop_texrank_coordinates.drawio
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
-docs/images/excalidraw-example.svg
-docs/images/git_merge.png
-docs/images/image_details.png
-docs/images/image_list.png
-docs/images/swiss3.png
+docs/reference/classes.rst
+docs/reference/command_line.rst
+docs/reference/index.rst
+docs/reference/modules.rst
+docs/tutorials/index.rst
+docs/tutorials/tbd.rst
 modulefiles/conda
 modulefiles/paths
 src/echolocator.egg-info/PKG-INFO
 src/echolocator.egg-info/SOURCES.txt
 src/echolocator.egg-info/dependency_links.txt
 src/echolocator.egg-info/entry_points.txt
 src/echolocator.egg-info/requires.txt
 src/echolocator.egg-info/top_level.txt
 src/echolocator_api/__init__.py
 src/echolocator_api/aiohttp_client.py
-src/echolocator_api/context_base.py
 src/echolocator_api/exceptions.py
 src/echolocator_api/databases/constants.py
 src/echolocator_api/guis/__init__.py
 src/echolocator_api/guis/aiohttp.py
 src/echolocator_api/guis/constants.py
 src/echolocator_api/guis/context.py
 src/echolocator_api/guis/guis.py
@@ -83,16 +82,14 @@
 src/echolocator_lib/envvar.py
 src/echolocator_lib/version.py
 src/echolocator_lib/composers/__init__.py
 src/echolocator_lib/composers/composers.py
 src/echolocator_lib/composers/html.py
 src/echolocator_lib/composers/prettyhelper.py
 src/echolocator_lib/composers/text.py
-src/echolocator_lib/contexts/__init__.py
-src/echolocator_lib/contexts/base.py
 src/echolocator_lib/guis/__init__.py
 src/echolocator_lib/guis/aiohttp.py
 src/echolocator_lib/guis/base.py
 src/echolocator_lib/guis/constants.py
 src/echolocator_lib/guis/context.py
 src/echolocator_lib/guis/guis.py
 src/echolocator_lib/guis/html/index.html
```

### Comparing `echolocator-1.4.0/src/echolocator_api/databases/constants.py` & `echolocator-1.5.0/src/echolocator_api/databases/constants.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_api/exceptions.py` & `echolocator-1.5.0/src/echolocator_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_api/guis/aiohttp.py` & `echolocator-1.5.0/src/echolocator_api/guis/context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,43 @@
 import logging
 
-# Class for an aiohttp client.
-from echolocator_api.aiohttp_client import AiohttpClient
+# Base class.
+from dls_utilpack.client_context_base import ClientContextBase
 
-# Dataface protocolj things.
-from echolocator_api.guis.constants import Commands, Keywords
+# Things created in the context.
+from echolocator_api.guis.guis import Guis, echolocator_guis_set_default
 
 logger = logging.getLogger(__name__)
 
 
-# ------------------------------------------------------------------------------------------
-class Aiohttp:
+class Context(ClientContextBase):
     """
-    Object implementing client side API for talking to the echolocator_gui server.
-    Please see doctopic [A01].
+    Client context for a echolocator_gui object.
+    On entering, it creates the object according to the specification (a dict).
+    On exiting, it closes client connection.
+
+    The aenter and aexit methods are exposed for use by an enclosing context and the base class.
     """
 
     # ----------------------------------------------------------------------------------------
-    def __init__(self, specification=None):
-        self.__specification = specification
-
-        self.__aiohttp_client = AiohttpClient(
-            specification["type_specific_tbd"]["aiohttp_specification"],
-        )
+    def __init__(self, specification):
+        ClientContextBase.__init__(self, specification)
 
     # ----------------------------------------------------------------------------------------
-    def specification(self):
-        return self.__specification
+    async def aenter(self):
+        """ """
 
-    # ----------------------------------------------------------------------------------------
-    async def report_health(self):
-        """"""
-        return await self.__send_protocolj("report_health")
+        # Build the object according to the specification.
+        self.interface = Guis().build_object(self.specification)
 
-    # ----------------------------------------------------------------------------------------
-    async def __send_protocolj(self, function, *args, **kwargs):
-        """"""
-
-        return await self.__aiohttp_client.client_protocolj(
-            {
-                Keywords.COMMAND: Commands.EXECUTE,
-                Keywords.PAYLOAD: {
-                    "function": function,
-                    "args": args,
-                    "kwargs": kwargs,
-                },
-            },
-        )
+        # If there is more than one gui, the last one defined will be the default.
+        echolocator_guis_set_default(self.interface)
 
     # ----------------------------------------------------------------------------------------
-    async def close_client_session(self):
-        """"""
-
-        if self.__aiohttp_client is not None:
-            await self.__aiohttp_client.close_client_session()
+    async def aexit(self):
+        """ """
 
-    # ----------------------------------------------------------------------------------------
-    async def client_report_health(self):
-        """"""
+        if self.interface is not None:
+            await self.interface.close_client_session()
 
-        return await self.__aiohttp_client.client_report_health()
+            # Clear the global variable.  Important between pytests.
+            echolocator_guis_set_default(None)
```

### Comparing `echolocator-1.4.0/src/echolocator_api/guis/guis.py` & `echolocator-1.5.0/src/echolocator_api/guis/guis.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 def echolocator_guis_get_default():
     global __default_echolocator_gui
     if __default_echolocator_gui is None:
         raise RuntimeError("echolocator_guis_get_default instance is None")
     return __default_echolocator_gui
 
 
+def echolocator_guis_has_default():
+    global __default_echolocator_gui
+    return __default_echolocator_gui is not None
+
+
 # -----------------------------------------------------------------------------------------
 
 
 class Guis(Things):
     """
     List of available echolocator_guis.
     """
```

### Comparing `echolocator-1.4.0/src/echolocator_cli/main.py` & `echolocator-1.5.0/src/echolocator_cli/main.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_cli/subcommands/base.py` & `echolocator-1.5.0/src/echolocator_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_cli/subcommands/service.py` & `echolocator-1.5.0/src/echolocator_cli/subcommands/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 # Servbase context creator.
 from dls_servbase_lib.datafaces.context import Context as DlsServbaseDatafaceContext
 
 # Xchembku client context.
 from xchembku_api.datafaces.context import Context as XchembkuDatafacesContext
 
+# Things created in the context.
+from echolocator_api.guis.guis import echolocator_guis_get_default
+
 # Base class for cli subcommands.
 from echolocator_cli.subcommands.base import ArgKeywords, Base
 
 # Rockingest context creator.
 from echolocator_lib.guis.context import Context as GuiContext
 
-# Things created in the context.
-from echolocator_lib.guis.guis import echolocator_guis_get_default
-
 logger = logging.getLogger()
 
 
 # --------------------------------------------------------------
 class Service(Base):
     """
     Start single service and keep running until ^C or remotely requested shutdown.
```

### Comparing `echolocator-1.4.0/src/echolocator_cli/version.py` & `echolocator-1.5.0/src/echolocator_cli/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/__main__.py` & `echolocator-1.5.0/src/echolocator_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/composers/composers.py` & `echolocator-1.5.0/src/echolocator_lib/composers/composers.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/composers/html.py` & `echolocator-1.5.0/src/echolocator_lib/composers/html.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/composers/prettyhelper.py` & `echolocator-1.5.0/src/echolocator_lib/composers/prettyhelper.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/composers/text.py` & `echolocator-1.5.0/src/echolocator_lib/composers/text.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/envvar.py` & `echolocator-1.5.0/src/echolocator_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/aiohttp.py` & `echolocator-1.5.0/src/echolocator_lib/guis/aiohttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 thing_type = "echolocator_lib.echolocator_guis.aiohttp"
 
 
 # ------------------------------------------------------------------------------------------
 class Aiohttp(Thing, BaseAiohttp):
     """
-    Object implementing remote procedure calls for echolocator_gui methods.
+    Object implementing remote procedure calls for the echolocator API.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification=None):
         Thing.__init__(self, thing_type, specification)
         BaseAiohttp.__init__(
             self,
```

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/constants.py` & `echolocator-1.5.0/src/echolocator_lib/guis/constants.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/context.py` & `echolocator-1.5.0/src/echolocator_lib/guis/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 import logging
 
-# Base class which maps flask requests to methods.
-from echolocator_lib.contexts.base import Base as ContextBase
+# Base class for an asyncio server context.
+from dls_utilpack.server_context_base import ServerContextBase
 
 # Things created in the context.
-from echolocator_lib.guis.guis import Guis, echolocator_guis_set_default
+from echolocator_lib.guis.guis import Guis
 
 logger = logging.getLogger(__name__)
 
 
 thing_type = "echolocator_lib.echolocator_guis.context"
 
 
-class Context(ContextBase):
+class Context(ServerContextBase):
     """
     Object representing an event echolocator_dataface connection.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification):
-        ContextBase.__init__(self, thing_type, specification)
+        ServerContextBase.__init__(self, thing_type, specification)
 
     # ----------------------------------------------------------------------------------------
     async def aenter(self):
         """ """
 
         self.server = Guis().build_object(self.specification())
 
-        # If there is more than one gui, the last one defined will be the default.
-        echolocator_guis_set_default(self.server)
-
         if self.context_specification.get("start_as") == "coro":
             await self.server.activate_coro()
 
         elif self.context_specification.get("start_as") == "thread":
             await self.server.start_thread()
 
         elif self.context_specification.get("start_as") == "process":
             logger.debug("starting gui context")
             await self.server.start_process()
 
     # ----------------------------------------------------------------------------------------
-    async def aexit(self):
+    async def aexit(self, type, value, traceback):
         """ """
         logger.debug(f"[DISSHU] {thing_type} aexit")
 
         if self.server is not None:
             if self.context_specification.get("start_as") == "process":
                 logger.debug(f"[DISSHU] {thing_type} calling client_shutdown")
                 # Put in request to shutdown the server.
```

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/css/image_list_ux.css` & `echolocator-1.5.0/src/echolocator_lib/guis/html/css/image_list_ux.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png` & `echolocator-1.5.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/css/plate_list_ux.css` & `echolocator-1.5.0/src/echolocator_lib/guis/html/css/plate_list_ux.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/css/styles.css` & `echolocator-1.5.0/src/echolocator_lib/guis/html/css/styles.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png` & `echolocator-1.5.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/images/radial1.666.png` & `echolocator-1.5.0/src/echolocator_lib/guis/html/images/radial1.666.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/index.html` & `echolocator-1.5.0/src/echolocator_lib/guis/html/index.html`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/index.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/index.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/common/base.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/common/base.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/plate_list_ux.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/plate_list_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/ring.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js` & `echolocator-1.5.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/src/echolocator_lib/version.py` & `echolocator-1.5.0/src/echolocator_lib/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/base.py` & `echolocator-1.5.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/configurations/service.yaml` & `echolocator-1.5.0/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/configurations/store.csv` & `echolocator-1.5.0/tests/configurations/store.csv`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/conftest.py` & `echolocator-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/example_images/1.jpg` & `echolocator-1.5.0/tests/example_images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/example_images/2.jpg` & `echolocator-1.5.0/tests/example_images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/example_images/3.jpg` & `echolocator-1.5.0/tests/example_images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/example_images/4.png` & `echolocator-1.5.0/tests/example_images/4.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/images/1.jpg` & `echolocator-1.5.0/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/images/2.jpg` & `echolocator-1.5.0/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/images/3.jpg` & `echolocator-1.5.0/tests/images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.4.0/tests/test_droplocation.py` & `echolocator-1.5.0/tests/test_droplocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 # Client context creator.
 from echolocator_api.guis.context import Context as GuiClientContext
 
+# Object managing gui
+from echolocator_api.guis.guis import echolocator_guis_get_default
+
 # GUI constants.
 from echolocator_lib.guis.constants import Commands, Cookies, Keywords
 
 # Server context creator.
 from echolocator_lib.guis.context import Context as GuiServerContext
 
-# Object managing gui
-from echolocator_lib.guis.guis import echolocator_guis_get_default
-
 # Base class for the tester.
 from tests.base import Base
 
 # Things xchembku provides.
 
 
 logger = logging.getLogger(__name__)
@@ -87,14 +87,15 @@
         # Make the client context.
         gui_client_context = GuiClientContext(gui_specification)
 
         # Start the client context for the remote access to the xchembku.
         async with xchembku_client_context:
             # Start the server context xchembku which starts the process.
             async with xchembku_server_context:
+                # Start the servbase (cookies) server.
                 async with servbase_dataface_context:
                     # Start the gui client context.
                     async with gui_client_context:
                         # And the gui server context which starts the coro.
                         async with gui_server_context:
                             await self.__run_the_test(constants, output_directory)
```

### Comparing `echolocator-1.4.0/tests/test_export_to_csv.py` & `echolocator-1.5.0/tests/test_export_to_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 # Client context creator.
 from echolocator_api.guis.context import Context as GuiClientContext
 
+# Object managing gui
+from echolocator_api.guis.guis import echolocator_guis_get_default
+
 # GUI constants.
 from echolocator_lib.guis.constants import Commands, Keywords
 
 # Server context creator.
 from echolocator_lib.guis.context import Context as GuiServerContext
 
-# Object managing gui
-from echolocator_lib.guis.guis import echolocator_guis_get_default
-
 # Base class for the tester.
 from tests.base import Base
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
```

### Comparing `echolocator-1.4.0/tests/test_export_to_soakdb3.py` & `echolocator-1.5.0/tests/test_export_to_soakdb3.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 # Client context creator.
 from echolocator_api.guis.context import Context as GuiClientContext
 
+# Object managing gui
+from echolocator_api.guis.guis import echolocator_guis_get_default
+
 # GUI constants.
 from echolocator_lib.guis.constants import Commands, Keywords
 
 # Server context creator.
 from echolocator_lib.guis.context import Context as GuiServerContext
 
-# Object managing gui
-from echolocator_lib.guis.guis import echolocator_guis_get_default
-
 # Base class for the tester.
 from tests.base import Base
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
```

### Comparing `echolocator-1.4.0/tests/test_fetch_image.py` & `echolocator-1.5.0/tests/test_fetch_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 # Client context creator.
 from echolocator_api.guis.context import Context as GuiClientContext
 
+# Object managing gui
+from echolocator_api.guis.guis import echolocator_guis_get_default
+
 # GUI constants.
 from echolocator_lib.guis.constants import Commands, Cookies, Keywords
 
 # Server context creator.
 from echolocator_lib.guis.context import Context as GuiServerContext
 
-# Object managing gui
-from echolocator_lib.guis.guis import echolocator_guis_get_default
-
 # Base class for the tester.
 from tests.base import Base
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
```

### Comparing `echolocator-1.4.0/tests/test_fetch_images.py` & `echolocator-1.5.0/tests/test_fetch_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 # Client context creator.
 from echolocator_api.guis.context import Context as GuiClientContext
 
+# Object managing gui
+from echolocator_api.guis.guis import echolocator_guis_get_default
+
 # GUI constants.
 from echolocator_lib.guis.constants import Commands, Cookies, Keywords
 
 # Server context creator.
 from echolocator_lib.guis.context import Context as GuiServerContext
 
-# Object managing gui
-from echolocator_lib.guis.guis import echolocator_guis_get_default
-
 # Base class for the tester.
 from tests.base import Base
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
```

### Comparing `echolocator-1.4.0/tests/test_report_plates.py` & `echolocator-1.5.0/tests/test_report_plates.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 # Client context creator.
 from echolocator_api.guis.context import Context as GuiClientContext
 
+# Object managing gui
+from echolocator_api.guis.guis import echolocator_guis_get_default
+
 # GUI constants.
 from echolocator_lib.guis.constants import Commands, Cookies, Keywords
 
 # Server context creator.
 from echolocator_lib.guis.context import Context as GuiServerContext
 
-# Object managing gui
-from echolocator_lib.guis.guis import echolocator_guis_get_default
-
 # Base class for the tester.
 from tests.base import Base
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
```

