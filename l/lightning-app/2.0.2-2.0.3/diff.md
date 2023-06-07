# Comparing `tmp/lightning-app-2.0.2.tar.gz` & `tmp/lightning-app-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-app-2.0.2.tar", last modified: Mon Apr 24 13:57:18 2023, max compression
+gzip compressed data, was "lightning-app-2.0.3.tar", last modified: Wed Jun  7 17:10:57 2023, max compression
```

## Comparing `lightning-app-2.0.2.tar` & `lightning-app-2.0.3.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.955029 lightning-app-2.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.883029 lightning-app-2.0.2/.actions/
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-04-24 13:57:07.000000 lightning-app-2.0.2/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-24 13:57:07.000000 lightning-app-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-04-24 13:57:18.955029 lightning-app-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-04-24 13:57:07.000000 lightning-app-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-24 13:57:07.000000 lightning-app-2.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.875028 lightning-app-2.0.2/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.887029 lightning-app-2.0.2/requirements/app/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/cloud.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/components.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/devel.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/ui.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:57:18.955029 lightning-app-2.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7917 2023-04-24 13:57:07.000000 lightning-app-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.887029 lightning-app-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.887029 lightning-app-2.0.2/src/lightning_app/
--rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.891029 lightning-app-2.0.2/src/lightning_app/api/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/api/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/api/request_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.895029 lightning-app-2.0.2/src/lightning_app/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.895029 lightning-app-2.0.2/src/lightning_app/cli/app-template/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.895029 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.875028 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.895029 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_a/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.895029 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_b/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.899029 lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    21746 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_pl_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_react_ui_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.899029 lightning-app-2.0.2/src/lightning_app/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/cd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/pwd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/rm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.899029 lightning-app-2.0.2/src/lightning_app/cli/component-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.875028 lightning-app-2.0.2/src/lightning_app/cli/component-template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.899029 lightning-app-2.0.2/src/lightning_app/cli/component-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.903029 lightning-app-2.0.2/src/lightning_app/cli/component-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/placeholdername/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/placeholdername/component.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.903029 lightning-app-2.0.2/src/lightning_app/cli/component-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.903029 lightning-app-2.0.2/src/lightning_app/cli/connect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/connect/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/connect/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/connect/maverick.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20545 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/lightning_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.903029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/.lightningignore
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.903029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/script_runner/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/test_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/craco.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.911029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.911029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.915029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.915029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.915029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.915029 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/example_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.915029 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/App.css
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)    55270 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/components/database/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/database/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/database/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/database/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/components/multi_node/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/multi_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/multi_node/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/multi_node/fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/multi_node/pytorch_spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/multi_node/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.923029 lightning-app-2.0.2/src/lightning_app/components/python/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/python/popen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/python/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.923029 lightning-app-2.0.2/src/lightning_app/components/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-04-24 13:57:16.000000 lightning-app-2.0.2/src/lightning_app/components/serve/catimage.png
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/cold_start_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/gradio_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/python_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.923029 lightning-app-2.0.2/src/lightning_app/components/serve/types/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/types/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/types/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.927029 lightning-app-2.0.2/src/lightning_app/core/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29740 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32847 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)    30754 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/work.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.927029 lightning-app-2.0.2/src/lightning_app/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.927029 lightning-app-2.0.2/src/lightning_app/frontend/just_py/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/just_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/just_py/just_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/just_py/just_py_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.927029 lightning-app-2.0.2/src/lightning_app/frontend/panel/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/panel/app_state_comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/panel/app_state_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/panel/panel_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/panel/panel_serve_render_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/stream_lit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/streamlit_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.931029 lightning-app-2.0.2/src/lightning_app/perf/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/perf/pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.931029 lightning-app-2.0.2/src/lightning_app/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/plugin/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.931029 lightning-app-2.0.2/src/lightning_app/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.931029 lightning-app-2.0.2/src/lightning_app/runners/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/backends/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/backends/mp_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    45581 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/runtime_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.935029 lightning-app-2.0.2/src/lightning_app/source_code/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/copytree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.935029 lightning-app-2.0.2/src/lightning_app/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/copier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18312 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.935029 lightning-app-2.0.2/src/lightning_app/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/structures/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/structures/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.939029 lightning-app-2.0.2/src/lightning_app/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.939029 lightning-app-2.0.2/src/lightning_app/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.939029 lightning-app-2.0.2/src/lightning_app/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.939029 lightning-app-2.0.2/src/lightning_app/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/css/main.bb0f092c.css
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/css/main.bb0f092c.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.2/src/lightning_app/ui/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.939029 lightning-app-2.0.2/src/lightning_app/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/js/787.418637a8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.2/src/lightning_app/ui/static/lightningState.js
--rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.2/src/lightning_app/ui/static/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.943029 lightning-app-2.0.2/src/lightning_app/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
--rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.2/src/lightning_app/ui/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.955029 lightning-app-2.0.2/src/lightning_app/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/app_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/app_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/app_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/cluster_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.955029 lightning-app-2.0.2/src/lightning_app/utilities/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/dependency_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/load_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/logs_socket_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60241 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.955029 lightning-app-2.0.2/src/lightning_app/utilities/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/cloud_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/tarfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    30463 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/safe_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/version.info
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.891029 lightning-app-2.0.2/src/lightning_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.924584 lightning-app-2.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/.actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    17470 2023-06-07 17:10:40.000000 lightning-app-2.0.3/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-07 17:10:40.000000 lightning-app-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-07 17:10:57.920584 lightning-app-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-06-07 17:10:40.000000 lightning-app-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-07 17:10:40.000000 lightning-app-2.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.888584 lightning-app-2.0.3/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/requirements/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/cloud.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/components.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/ui.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 17:10:57.924584 lightning-app-2.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-06-07 17:10:40.000000 lightning-app-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/src/lightning_app/
+-rw-r--r--   0 runner    (1001) docker     (123)    33897 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/src/lightning_app/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/api/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/api/request_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/app-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.888584 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_a/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_b/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_pl_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_react_ui_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/rm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/component-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.888584 lightning-app-2.0.3/src/lightning_app/cli/component-template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/component-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/component-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/placeholdername/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/placeholdername/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/component-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/connect/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/connect/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/connect/maverick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/lightning_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/.lightningignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/craco.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/example_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    55270 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/components/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/database/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/database/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/database/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/components/multi_node/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/multi_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/multi_node/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/multi_node/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/multi_node/pytorch_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/multi_node/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/components/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/python/popen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/python/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/components/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30215 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-06-07 17:10:55.000000 lightning-app-2.0.3/src/lightning_app/components/serve/catimage.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/cold_start_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/gradio_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/python_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/components/serve/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19322 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32847 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/core/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31224 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/core/work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/frontend/just_py/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/just_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/just_py/just_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/just_py/just_py_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/frontend/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/panel/app_state_comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/panel/app_state_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/panel/panel_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/panel/panel_serve_render_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/stream_lit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/streamlit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/perf/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/perf/pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/plugin/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/runners/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/backends/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/backends/mp_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45732 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/runtime_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/source_code/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/copier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/structures/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/structures/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/css/main.bb0f092c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/css/main.bb0f092c.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.3/src/lightning_app/ui/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.916584 lightning-app-2.0.3/src/lightning_app/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.3/src/lightning_app/ui/static/lightningState.js
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.3/src/lightning_app/ui/static/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.916584 lightning-app-2.0.3/src/lightning_app/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.3/src/lightning_app/ui/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.920584 lightning-app-2.0.3/src/lightning_app/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/app_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/app_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/app_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/cluster_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.920584 lightning-app-2.0.3/src/lightning_app/utilities/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/dependency_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/load_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/logs_socket_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60255 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.920584 lightning-app-2.0.3/src/lightning_app/utilities/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/cloud_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30277 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/safe_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/src/lightning_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/version.info
```

### Comparing `lightning-app-2.0.2/.actions/assistant.py` & `lightning-app-2.0.3/.actions/assistant.py`

 * *Files 5% similar despite different names*

```diff
@@ -154,15 +154,16 @@
 def load_readme_description(path_dir: str, homepage: str, version: str) -> str:
     """Load readme as decribtion.
 
     >>> load_readme_description(_PROJECT_ROOT, "", "")  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
     '...PyTorch Lightning is just organized PyTorch...'
     """
     path_readme = os.path.join(path_dir, "README.md")
-    text = open(path_readme, encoding="utf-8").read()
+    with open(path_readme, encoding="utf-8") as fo:
+        text = fo.read()
 
     # drop images from readme
     text = text.replace(
         "![PT to PL](docs/source-pytorch/_static/images/general/pl_quick_start_full_compressed.gif)", ""
     )
 
     # https://github.com/Lightning-AI/lightning/raw/master/docs/source/_static/images/lightning_module/pt_to_pl.png
@@ -327,15 +328,15 @@
         fp_new = fp.replace(source_dir, target_dir)
         _, ext = os.path.splitext(fp)
         if ext in (".png", ".jpg", ".ico"):
             os.makedirs(dirname(fp_new), exist_ok=True)
             if not isfile(fp_new):
                 shutil.copy(fp, fp_new)
             continue
-        elif ext in (".pyc",):
+        if ext in (".pyc",):
             continue
         # Try to parse everything else
         with open(fp, encoding="utf-8") as fo:
             try:
                 lines = fo.readlines()
             except UnicodeDecodeError:
                 # a binary file, skip
@@ -390,16 +391,18 @@
             if req.name not in packages:
                 final.append(line)
         print(final)
         path.write_text("\n".join(final) + "\n")
 
     @staticmethod
     def _replace_min(fname: str) -> None:
-        req = open(fname, encoding="utf-8").read().replace(">=", "==")
-        open(fname, "w", encoding="utf-8").write(req)
+        with open(fname, encoding="utf-8") as fo:
+            req = fo.read().replace(">=", "==")
+        with open(fname, "w", encoding="utf-8") as fw:
+            fw.write(req)
 
     @staticmethod
     def replace_oldest_ver(requirement_fnames: Sequence[str] = REQUIREMENT_FILES_ALL) -> None:
         """Replace the min package version by fixed one."""
         for fname in requirement_fnames:
             AssistantCLI._replace_min(fname)
```

### Comparing `lightning-app-2.0.2/LICENSE` & `lightning-app-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/PKG-INFO` & `lightning-app-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.2
+Version: 2.0.3
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,18 +21,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: components
-Provides-Extra: test
 Provides-Extra: ui
+Provides-Extra: components
 Provides-Extra: cloud
+Provides-Extra: test
 Provides-Extra: extra
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.2 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.3 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
 Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
 Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
@@ -10,17 +10,17 @@
 Language :: English Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: components Provides-Extra: test
-Provides-Extra: ui Provides-Extra: cloud Provides-Extra: extra Provides-Extra:
-all Provides-Extra: dev License-File: LICENSE
+Content-Type: text/markdown Provides-Extra: ui Provides-Extra: components
+Provides-Extra: cloud Provides-Extra: test Provides-Extra: extra Provides-
+Extra: all Provides-Extra: dev License-File: LICENSE
  [https://pl-flash-data.s3.amazonaws.com/brandmark.png] **With Lightning Apps,
 you build exactly what you need: from production-ready, multi-cloud ML systems
                           to simple research demos.**
     ______________________________________________________________________
             Website â¢ Docs â¢ Getting_started â¢ Help â¢ Slack
        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 lightning_app)](https://pypi.org/project/lightning_app/) [![PyPI Status](https:
```

### Comparing `lightning-app-2.0.2/README.md` & `lightning-app-2.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 </p>
 
 <!-- DO NOT ADD CONDA DOWNLOADS... README CHANGES MUST BE APPROVED BY EDEN OR WILL -->
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)](https://pypi.org/project/pytorch-lightning/)
 [![PyPI Status](https://badge.fury.io/py/pytorch-lightning.svg)](https://badge.fury.io/py/pytorch-lightning)
 [![PyPI Status](https://pepy.tech/badge/pytorch-lightning)](https://pepy.tech/project/pytorch-lightning)
-[![Conda](https://img.shields.io/conda/v/conda-forge/pytorch-lightning?label=conda&color=success)](https://anaconda.org/conda-forge/pytorch-lightning)
+[![Conda](https://img.shields.io/conda/v/conda-forge/lightning?label=conda&color=success)](https://anaconda.org/conda-forge/lightning)
 [![DockerHub](https://img.shields.io/docker/pulls/pytorchlightning/pytorch_lightning.svg)](https://hub.docker.com/r/pytorchlightning/pytorch_lightning)
 [![codecov](https://codecov.io/gh/Lightning-AI/lightning/branch/master/graph/badge.svg?token=SmzX8mnKlA)](https://codecov.io/gh/Lightning-AI/lightning)
 
-[![ReadTheDocs](https://readthedocs.org/projects/pytorch-lightning/badge/?version=stable)](https://lightning.ai/docs/pytorch/stable/)
 [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/lightning-ai/lightning)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lightning/blob/master/LICENSE)
 
 <!--
 [![CodeFactor](https://www.codefactor.io/repository/github/Lightning-AI/lightning/badge)](https://www.codefactor.io/repository/github/Lightning-AI/lightning)
 -->
 
 </div>
@@ -486,15 +486,15 @@
 ______________________________________________________________________
 
 ## Community
 
 The lightning community is maintained by
 
 - [10+ core contributors](https://lightning.ai/docs/pytorch/latest/community/governance.html) who are all a mix of professional engineers, Research Scientists, and Ph.D. students from top AI labs.
-- 590+ active community contributors.
+- 800+ community contributors.
 
 Want to help us build Lightning and reduce boilerplate for thousands of researchers? [Learn how to make your first contribution here](https://lightning.ai/docs/pytorch/stable/generated/CONTRIBUTING.html)
 
 Lightning is also part of the [PyTorch ecosystem](https://pytorch.org/ecosystem/) which requires projects to have solid testing, documentation and support.
 
 ### Asking for help
```

### Comparing `lightning-app-2.0.2/requirements/app/base.txt` & `lightning-app-2.0.3/requirements/app/base.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 lightning-cloud >=0.5.34
 packaging
 typing-extensions >=4.0.0, <=4.4.0
-deepdiff >=5.7.0, <6.2.4
+deepdiff >=5.7.0, <6.3.1
 starsessions >=1.2.1, <2.0 # strict
 fsspec >=2022.5.0, <=2022.7.1
 croniter >=1.3.0, <1.4.0  # strict; TODO: for now until we find something more robust.
-traitlets >=5.3.0, <5.9.0
+traitlets >=5.3.0, <5.10.0
 arrow >=1.2.0, <1.2.4
 lightning-utilities >=0.7.0, <0.9.0
 beautifulsoup4 >=4.8.0, <4.11.2
-inquirer >=2.10.0, <=3.1.2
+inquirer >=2.10.0, <=3.1.3
 psutil <5.9.5
 click <=8.1.3
+python-multipart>=0.0.5, <=0.0.6
 
 fastapi >=0.69.0, <0.89.0  # strict; TODO: broken serializations
 starlette  # https://fastapi.tiangolo.com/deployment/versions/#about-starlette
 pydantic >=1.7.4, <2.0.0  # https://fastapi.tiangolo.com/deployment/versions/#about-pydantic
 
 dateutils <=0.6.12
 Jinja2 <=3.1.2
 PyYAML <=6.0
 requests <2.28.3
 rich >=12.3.0, <=13.0.1
 urllib3 <=1.26.13
-uvicorn <=0.17.6
+uvicorn <=0.22.0
 websocket-client <1.5.2
 websockets <=10.4
```

### Comparing `lightning-app-2.0.2/setup.py` & `lightning-app-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,19 @@
 
 
 @contextlib.contextmanager
 def _set_manifest_path(manifest_dir: str, aggregate: bool = False, mapping: Mapping = _PACKAGE_MAPPING) -> Generator:
     if aggregate:
         # aggregate all MANIFEST.in contents into a single temporary file
         manifest_path = _named_temporary_file(manifest_dir)
-        lines = ["include src/lightning/version.info\n", "include requirements/base.txt\n"]
+        lines = [
+            "include src/lightning/version.info\n",
+            "include src/lightning/py.typed\n",
+            "include requirements/base.txt\n",
+        ]
         # load manifest and aggregated all manifests
         for pkg in mapping.values():
             pkg_manifest = os.path.join(_PATH_SRC, pkg, "MANIFEST.in")
             if os.path.isfile(pkg_manifest):
                 with open(pkg_manifest) as fh:
                     lines.extend(fh.readlines())
         # convert lightning_foo to lightning/foo
```

### Comparing `lightning-app-2.0.2/src/lightning_app/CHANGELOG.md` & `lightning-app-2.0.3/src/lightning_app/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
+## [2.0.3] - 2023-06-07
+
+- Added the property `LightningWork.public_ip` that exposes the public IP of the `LightningWork` instance ([#17742](https://github.com/Lightning-AI/lightning/pull/17742))
+- Add missing python-multipart dependency ([#17244](https://github.com/Lightning-AI/lightning/pull/17244))
+
+### Changed
+
+- Made type hints public ([#17100](https://github.com/Lightning-AI/lightning/pull/17100))
+
+### Fixed
+
+- Fixed `LightningWork.internal_ip` that was mistakenly exposing the public IP instead; now exposes the private/internal IP address ([#17742](https://github.com/Lightning-AI/lightning/pull/17742))
+- Fixed resolution of latest version in CLI ([#17351](https://github.com/Lightning-AI/lightning/pull/17351))
+- Fixed property raised instead of returned ([#17595](https://github.com/Lightning-AI/lightning/pull/17595))
+- Fixed get project ([#17617](https://github.com/Lightning-AI/lightning/pull/17617), [#17666](https://github.com/Lightning-AI/lightning/pull/17666))
+
+
 ## [2.0.2] - 2023-04-24
 
 ### Fixed
 
 - Resolved Lightning App with remote storage ([#17426](https://github.com/Lightning-AI/lightning/pull/17426))
 - Fixed `AppState`, streamlit example ([#17452](https://github.com/Lightning-AI/lightning/pull/17452))
```

### Comparing `lightning-app-2.0.2/src/lightning_app/README.md` & `lightning-app-2.0.3/src/lightning_app/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/__about__.py` & `lightning-app-2.0.3/src/lightning_app/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/__init__.py` & `lightning-app-2.0.3/src/lightning_app/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/__setup__.py` & `lightning-app-2.0.3/src/lightning_app/__setup__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,22 +28,22 @@
     return _load_py_module("assistant", location)
 
 
 def _prepare_extras() -> Dict[str, Any]:
     assistant = _load_assistant()
     # https://setuptools.readthedocs.io/en/latest/setuptools.html#declaring-extras
     # Define package extras. These are only installed if you specify them.
-    # From remote, use like `pip install pytorch-lightning[dev, docs]`
-    # From local copy of repo, use like `pip install ".[dev, docs]"`
+    # From remote, use like `pip install "pytorch-lightning[dev, docs]"`
+    # From local copy of repo, use like `PACKAGE_NAME=app pip install ".[dev, docs]"`
     req_files = [Path(p) for p in glob.glob(os.path.join(_PATH_REQUIREMENTS, "*.txt"))]
     common_args = {"path_dir": _PATH_REQUIREMENTS, "unfreeze": "none" if _FREEZE_REQUIREMENTS else "major"}
     extras = {
         p.stem: assistant.load_requirements(file_name=p.name, **common_args)
         for p in req_files
-        if p.name not in ("docs.txt", "devel.txt", "base.txt")
+        if p.name not in ("docs.txt", "base.txt")
     }
     extras["extra"] = extras["cloud"] + extras["ui"] + extras["components"]
     extras["all"] = extras["extra"]
     extras["dev"] = extras["all"] + extras["test"]  # + extras['docs']
     return extras
```

### Comparing `lightning-app-2.0.2/src/lightning_app/api/http_methods.py` & `lightning-app-2.0.3/src/lightning_app/api/http_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     @property
     def receive(self):
         raise NotImplementedError
 
     @property
     def method(self):
-        raise self._method
+        return self._method
 
     @property
     def headers(self):
         return self._headers
 
     def body(self):
         return self._body
```

### Comparing `lightning-app-2.0.2/src/lightning_app/api/request_types.py` & `lightning-app-2.0.3/src/lightning_app/api/request_types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/app-template/.gitignore` & `lightning-app-2.0.3/src/lightning_app/cli/app-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/app-template/LICENSE` & `lightning-app-2.0.3/src/lightning_app/cli/app-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/app-template/README.md` & `lightning-app-2.0.3/src/lightning_app/cli/app-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py` & `lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/cmd_apps.py` & `lightning-app-2.0.3/src/lightning_app/cli/cmd_apps.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/cmd_clusters.py` & `lightning-app-2.0.3/src/lightning_app/cli/cmd_clusters.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,16 +321,16 @@
         try:
             resp: V1GetClusterResponse = api_client.cluster_service_get_cluster(id=cluster_id)
             click.echo(_cluster_status_long(cluster=resp, desired_state=target_state, elapsed=elapsed))
             if resp.status.phase == target_state:
                 break
             time.sleep(poll_duration_seconds)
             elapsed = int(time.time() - start)
-        except lightning_cloud.openapi.rest.ApiException as e:
-            if e.status == 404 and target_state == V1ClusterState.DELETED:
+        except lightning_cloud.openapi.rest.ApiException as ex:
+            if ex.status == 404 and target_state == V1ClusterState.DELETED:
                 return
             raise
     else:
         state_str = ClusterState.from_api(target_state)
         raise click.ClickException(
             dedent(
                 f"""\
@@ -362,41 +362,39 @@
 def _cluster_status_long(cluster: V1GetClusterResponse, desired_state: V1ClusterState, elapsed: float) -> str:
     """Echos a long-form status message to the user about the cluster state.
 
     Args:
         cluster: The cluster object
         elapsed: Seconds since we've started polling
     """
-
     cluster_id = cluster.id
     current_state = cluster.status.phase
     current_reason = cluster.status.reason
     bucket_name = cluster.spec.driver.kubernetes.aws.bucket_name
 
     duration = _format_elapsed_seconds(elapsed)
 
-    if current_state == V1ClusterState.FAILED:
-        if not _is_retryable_error(current_reason):
-            return dedent(
-                f"""\
+    if current_state == V1ClusterState.FAILED and not _is_retryable_error(current_reason):
+        return dedent(
+            f"""\
                 The requested cluster operation for cluster {cluster_id} has errors:
 
                 {current_reason}
 
                 --------------------------------------------------------------
 
                 We are automatically retrying, and an automated alert has been created
 
                 WARNING: Any non-deleted cluster may be using resources.
                 To avoid incuring cost on your cloud provider, delete the cluster using the following command:
                     lightning delete cluster {cluster_id}
 
                 Contact support@lightning.ai for additional help
                 """
-            )
+        )
 
     if desired_state == current_state == V1ClusterState.RUNNING:
         return dedent(
             f"""\
                 Cluster {cluster_id} is now running and ready to use.
                 To launch an app on this cluster use: lightning run app app.py --cloud --cluster-id {cluster_id}
                 """
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/cmd_init.py` & `lightning-app-2.0.3/src/lightning_app/cli/cmd_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,18 @@
     # for each file, rename the word
     trouble_names = {".DS_Store"}
     files = _ls_recursively(new_resource_name)
     for bad_file in files:
         if bad_file.split("/")[-1] in trouble_names:
             continue
         # find the words and replace
-        content = open(bad_file).read().replace("placeholdername", name_for_files)
-        with open(bad_file, "w") as file:
-            file.write(content)
+        with open(bad_file) as fo:
+            content = fo.read().replace("placeholdername", name_for_files)
+        with open(bad_file, "w") as fw:
+            fw.write(content)
 
     # rename files
     for file_name in files:
         new_file = re.sub("placeholdername", name_for_files, file_name)
         os.rename(file_name, new_file)
 
     return new_resource_name, name_for_files
@@ -108,18 +109,19 @@
 
             valid example:
             lightning-{resource_type}
             """
             raise SystemExit(m)
 
     except KeyboardInterrupt:
-        m = f"""
+        raise SystemExit(
+            f"""
         ⚡ {resource_type} init aborted! ⚡
         """
-        raise SystemExit(m)
+        )
 
     return value
 
 
 def component(component_name: str) -> None:
     if component_name is None:
         component_name = _capture_valid_app_component_name(resource_type="component")
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/cmd_install.py` & `lightning-app-2.0.3/src/lightning_app/cli/cmd_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,34 +86,33 @@
     if "github.com" in name:
         if version != "latest":
             logger.warn(
                 "When installing from GitHub, only the 'latest' version is supported. "
                 f"The provided version ({version}) will be ignored."
             )
         return non_gallery_app(name, yes, overwrite=overwrite)
-    else:
-        return gallery_app(name, yes, version, overwrite=overwrite)
+
+    return gallery_app(name, yes, version, overwrite=overwrite)
 
 
 def _install_component_command(name: str, yes: bool, version: str, overwrite: bool = False) -> None:
     if "github.com" in name:
         if version != "latest":
             logger.warn(
                 "When installing from GitHub, only the 'latest' version is supported. "
                 f"The provided version ({version}) will be ignored."
             )
         return non_gallery_component(name, yes)
-    else:
-        return gallery_component(name, yes, version)
+
+    return gallery_component(name, yes, version)
 
 
 def gallery_apps_and_components(
     name: str, yes_arg: bool, version_arg: str, cwd: Optional[str] = None, overwrite: bool = False
 ) -> Optional[str]:
-
     try:
         org, app_or_component = name.split("/")
     except Exception:
         return None
 
     entry, kind = _resolve_entry(name, version_arg)
 
@@ -123,15 +122,15 @@
             entry, app_or_component, org, yes_arg, resource_type="app"
         )
         # run installation if requested
         _install_app_from_source(source_url, git_url, folder_name, cwd=cwd, overwrite=overwrite, git_sha=git_sha)
 
         return os.path.join(os.getcwd(), *entry["appEntrypointFile"].split("/"))
 
-    elif kind == "component":
+    if kind == "component":
         # give the user the chance to do a manual install
         source_url, git_url, folder_name, git_sha = _show_install_app_prompt(
             entry, app_or_component, org, yes_arg, resource_type="component"
         )
         if "@" in git_url:
             git_url = git_url.split("git+")[1].split("@")[0]
         # run installation if requested
@@ -224,21 +223,22 @@
         should_install = len(value) == 0 or value in {"y", "yes", 1}
         if not should_install:
             raise KeyboardInterrupt()
 
         return git_url
     except KeyboardInterrupt:
         repo = entry["sourceUrl"]
-        m = f"""
+        raise SystemExit(
+            f"""
         ⚡ Installation aborted! ⚡
 
         Install the component yourself by visiting:
         {repo}
         """
-        raise SystemExit(m)
+        )
 
 
 def _show_non_gallery_install_component_prompt(gh_url: str, yes_arg: bool) -> str:
     if ".git@" not in gh_url:
         m = """
         Error, your github url must be in the following format:
         git+https://github.com/OrgName/repo-name.git@ALongCommitSHAString
@@ -279,21 +279,22 @@
         value = value.strip().lower()
         should_install = len(value) == 0 or value in {"y", "yes", 1}
         if not should_install:
             raise KeyboardInterrupt()
 
         return gh_url
     except KeyboardInterrupt:
-        m = f"""
+        raise SystemExit(
+            f"""
         ⚡ Installation aborted! ⚡
 
         Install the component yourself by visiting:
         {repo_url}
         """
-        raise SystemExit(m)
+        )
 
 
 def _show_install_app_prompt(
     entry: Dict[str, str], app: str, org: str, yes_arg: bool, resource_type: str
 ) -> Tuple[str, str, str, Optional[str]]:
     source_url = entry["sourceUrl"]  # This URL is used only to display the repo and extract folder name
     full_git_url = entry["gitUrl"]  # Used to clone the repo (can include tokens for private repos)
@@ -329,43 +330,45 @@
         should_install = len(value) == 0 or value in {"y", "yes", 1}
         if not should_install:
             raise KeyboardInterrupt()
 
         return source_url, git_url, folder_name, git_sha
     except KeyboardInterrupt:
         repo = entry["sourceUrl"]
-        m = f"""
+        raise SystemExit(
+            f"""
         ⚡ Installation aborted! ⚡
 
         Install the {resource_type} yourself by visiting:
         {repo}
         """
-        raise SystemExit(m)
+        )
 
 
 def _show_non_gallery_install_app_prompt(gh_url: str, yes_arg: bool) -> Tuple[str, str]:
     try:
         if gh_url.endswith(".git"):
             # folder_name when it's a GH url with .git
             folder_name = gh_url.split("/")[-1]
             folder_name = folder_name[:-4]
         else:
             # the last part of the url is the folder name otherwise
             folder_name = gh_url.split("/")[-1]
 
         org = re.search(r"github.com\/(.*)\/", gh_url).group(1)  # type: ignore
-    except Exception as e:  # noqa
-        m = """
+    except Exception:
+        raise SystemExit(
+            """
         Your github url is not supported. Here's the supported format:
         https://github.com/YourOrgName/your-repo-name
 
         Example:
         https://github.com/Lightning-AI/lightning
         """
-        raise SystemExit("")
+        )
 
     # yes arg does not prompt the user for permission to install anything
     # automatically creates env and sets up the project
     if yes_arg:
         return gh_url, folder_name
 
     prompt = f"""
@@ -393,57 +396,53 @@
         value = value.strip().lower()
         should_install = len(value) == 0 or value in {"y", "yes", 1}
         if not should_install:
             raise KeyboardInterrupt()
 
         return gh_url, folder_name
     except KeyboardInterrupt:
-        m = f"""
+        raise SystemExit(
+            f"""
         ⚡ Installation aborted! ⚡
 
         Install the app yourself by visiting {gh_url}
         """
-        raise SystemExit(m)
+        )
 
 
 def _validate_name(name: str, resource_type: str, example: str) -> Tuple[str, str]:
     # ensure resource identifier is properly formatted
     try:
         org, resource = name.split("/")
-    except Exception as e:  # noqa
-        m = f"""
+    except Exception:
+        raise SystemExit(
+            f"""
         {resource_type} name format must have organization/{resource_type}-name
 
         Examples:
         {example}
         user/{resource_type}-name
 
         You passed in: {name}
         """
-        raise SystemExit(m)
-    m = f"""
-    ⚡ Installing Lightning {resource_type} ⚡
-    {resource_type} name: {resource}
-    developer: {org}
-    """
+        )
     return org, resource
 
 
 def _resolve_entry(name, version_arg) -> Tuple[Optional[Dict], Optional[str]]:
     entry = None
     kind = None
 
     # resolve registry (orgs can have a private registry through their environment variables)
     registry_url = _resolve_app_registry()
 
     # load the app resource
     entry = _resolve_resource(registry_url, name=name, version_arg=version_arg, resource_type="app", raise_error=False)
 
     if not entry:
-
         registry_url = _resolve_component_registry()
 
         # load the component resource
         entry = _resolve_resource(
             registry_url, name=name, version_arg=version_arg, resource_type="component", raise_error=False
         )
         kind = "component" if entry else None
@@ -464,34 +463,35 @@
 
         if resource_type == "app":
             gallery_entries = [a for a in data["apps"] if a["canDownloadSourceCode"]]
 
         elif resource_type == "component":
             gallery_entries = data["components"]
     except requests.ConnectionError:
-        m = f"""
+        sys.tracebacklimit = 0
+        raise SystemError(
+            f"""
         Network connection error, could not load list of available Lightning {resource_type}s.
 
         Try again when you have a network connection!
         """
-        sys.tracebacklimit = 0
-        raise SystemError(m)
+        )
 
     entries = []
     all_versions = []
     for x in gallery_entries:
         if name == x["name"]:
             entries.append(x)
             all_versions.append(x["version"])
 
     if len(entries) == 0:
         if raise_error:
             raise SystemExit(f"{resource_type}: '{name}' is not available on ⚡ Lightning AI ⚡")
-        else:
-            return None
+
+        return None
 
     entry = None
     if version_arg == "latest":
         entry = max(entries, key=lambda app: Version(app["version"]))
     else:
         for e in entries:
             if e["version"] == version_arg:
@@ -499,16 +499,15 @@
                 break
     if entry is None and raise_error:
         if raise_error:
             raise Exception(
                 f"{resource_type}: 'Version {version_arg} for {name}' is not available on ⚡ Lightning AI ⚡. "
                 f"Here is the list of all availables versions:{os.linesep}{os.linesep.join(all_versions)}"
             )
-        else:
-            return None
+        return None
 
     return entry
 
 
 def _install_with_env(repo_url: str, folder_name: str, cwd: Optional[str] = None) -> None:
     if not cwd:
         cwd = os.getcwd()
@@ -580,36 +579,35 @@
                 f"or force to overwrite the existing folder by passing `--overwrite`.",
             )
         shutil.rmtree(destination)
     # clone repo
     logger.info(f"⚡ RUN: git clone {source_url}")
     try:
         subprocess.check_output(["git", "clone", git_url], stderr=subprocess.STDOUT)
-    except subprocess.CalledProcessError as e:
-        if "Repository not found" in str(e.output):
-            m = f"""
+    except subprocess.CalledProcessError as ex:
+        if "Repository not found" in str(ex.output):
+            raise SystemExit(
+                f"""
             Looks like the github url was not found or doesn't exist. Do you have a typo?
             {source_url}
             """
-            raise SystemExit(m)
-        else:
-            raise Exception(e)
+            )
+        raise Exception(ex)
 
     # step into the repo folder
     os.chdir(f"{folder_name}")
     cwd = os.getcwd()
 
     try:
         if git_sha:
             subprocess.check_output(["git", "checkout", git_sha], stderr=subprocess.STDOUT)
-    except subprocess.CalledProcessError as e:
-        if "did not match any" in str(e.output):
+    except subprocess.CalledProcessError as ex:
+        if "did not match any" in str(ex.output):
             raise SystemExit("Looks like the git SHA is not valid or doesn't exist in app repo.")
-        else:
-            raise Exception(e)
+        raise Exception(ex)
 
     # activate and install reqs
     # TODO: remove shell=True... but need to run command in venv
     logger.info("⚡ RUN: install requirements (pip install -r requirements.txt)")
     subprocess.call("pip install -r requirements.txt", shell=True)
 
     # install project
@@ -647,14 +645,12 @@
         if you want to uninstall, run this command:
         pip uninstall {uninstall_step}
         """
         logger.info(m)
 
 
 def _resolve_app_registry() -> str:
-    registry = os.environ.get("LIGHTNING_APP_REGISTRY", LIGHTNING_APPS_PUBLIC_REGISTRY)
-    return registry
+    return os.environ.get("LIGHTNING_APP_REGISTRY", LIGHTNING_APPS_PUBLIC_REGISTRY)
 
 
 def _resolve_component_registry() -> str:
-    registry = os.environ.get("LIGHTNING_COMPONENT_REGISTRY", LIGHTNING_COMPONENT_PUBLIC_REGISTRY)
-    return registry
+    return os.environ.get("LIGHTNING_COMPONENT_REGISTRY", LIGHTNING_COMPONENT_PUBLIC_REGISTRY)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/cmd_pl_init.py` & `lightning-app-2.0.3/src/lightning_app/cli/cmd_pl_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,16 +82,16 @@
         if not overwrite:
             click.echo(
                 f"There is already an app with the name {name} in the current working directory. Choose a different"
                 f" name with `--name` or force to overwrite the existing folder by passing `--overwrite`.",
                 err=True,
             )
             raise SystemExit(1)
-        else:
-            shutil.rmtree(destination)
+
+        shutil.rmtree(destination)
 
     template_dir = Path(lightning_app.cli.__file__).parent / "pl-app-template"
 
     with Status("[bold green]Copying app files"):
         shutil.copytree(template_dir, destination, ignore=shutil.ignore_patterns("node_modules", "build"))
         if (template_dir / "ui" / "build").exists():
             shutil.copytree(template_dir / "ui" / "build", destination / "ui" / "build")
@@ -115,22 +115,22 @@
 
 
 def download_frontend(destination: Path) -> None:
     # TODO: Update the URL to the release in GitHub once the PL app repo is public
     url = "https://storage.googleapis.com/grid-packages/pytorch-lightning-app/v0.0.0/build.tar.gz"
     build_dir_name = "build"
     with TemporaryDirectory() as download_dir:
-        response = urllib.request.urlopen(url)
+        response = urllib.request.urlopen(url)  # noqa: S310
         file = tarfile.open(fileobj=response, mode="r|gz")
         file.extractall(path=download_dir)
         shutil.move(str(Path(download_dir, build_dir_name)), destination)
 
 
 def project_file_from_template(template_dir: Path, destination_dir: Path, template_name: str, **kwargs: Any) -> None:
-    env = Environment(loader=FileSystemLoader(template_dir))
+    env = Environment(loader=FileSystemLoader(template_dir))  # noqa: S701
     template = env.get_template(template_name)
     rendered_template = template.render(**kwargs)
     with open(destination_dir / template_name, "w") as file:
         file.write(rendered_template)
 
 
 def print_pretty_report(
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/cmd_react_ui_init.py` & `lightning-app-2.0.3/src/lightning_app/cli/cmd_react_ui_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,16 +116,16 @@
         """
         missing_msgs.append(m)
 
     # exit or show success message
     if len(missing_msgs) > 0:
         missing_msg = "\n".join(missing_msgs)
         raise SystemExit(missing_msg)
-    else:
-        m = f"""
-        found npm  version: {npm_version}
-        found node version: {node_version}
-        found yarn version: {yarn_version}
+    logger.info(
+        f"""
+    found npm  version: {npm_version}
+    found node version: {node_version}
+    found yarn version: {yarn_version}
 
-        Pre-requisites met!
-        """
-        logger.info(m)
+    Pre-requisites met!
+    """
+    )
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/cmd_ssh_keys.py` & `lightning-app-2.0.3/src/lightning_app/cli/cmd_ssh_keys.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,15 +55,16 @@
 
     def list(self) -> None:
         ssh_keys = self.get_ssh_keys()
         console = Console()
         console.print(ssh_keys.as_table())
 
     def add_key(self, public_key: str, name: Optional[str], comment: Optional[str]) -> None:
-        key_name = name if name is not None else "-".join(random.choice(string.ascii_lowercase) for _ in range(5))
+        rnd = "-".join(random.choice(string.ascii_lowercase) for _ in range(5))  # noqa: S311
+        key_name = name if name is not None else rnd
         self.api_client.s_sh_public_key_service_create_ssh_public_key(
             V1CreateSSHPublicKeyRequest(
                 name=key_name,
                 public_key=public_key,
                 comment=comment if comment is not None else key_name,
             )
         )
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/commands/app_commands.py` & `lightning-app-2.0.3/src/lightning_app/cli/commands/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/commands/cd.py` & `lightning-app-2.0.3/src/lightning_app/cli/commands/cd.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,17 +30,15 @@
 _HOME = os.path.expanduser("~")
 _CD_FILE = os.path.join(_LIGHTNING_CONNECTION_FOLDER, "cd.txt")
 
 
 @click.argument("path", nargs=-1)
 def cd(path: Optional[Union[Tuple[str], str]], verify: bool = True) -> None:
     """Change the current directory within the Lightning Cloud filesystem."""
-
     with Live(Spinner("point", text=Text("pending...", style="white")), transient=True) as live:
-
         root = "/"
 
         if isinstance(path, Tuple) and len(path) > 0:
             path = " ".join(path)
 
         # handle ~/
         if isinstance(path, str) and path.startswith(_HOME):
@@ -62,61 +60,58 @@
                 f.write(root + "\n")
 
             live.stop()
 
             print(f"cd {root}")
 
             return root
+
+        # read from saved cd
+        with open(_CD_FILE) as f:
+            lines = f.readlines()
+            root = lines[0].replace("\n", "")
+
+        if verify:
+            if path.startswith("/"):
+                paths = [os.path.join(path, p) for p in ls.ls(path, print=False, use_live=False)]
+            else:
+                paths = [os.path.join(root, p) for p in ls.ls(root, print=False, use_live=False)]
+
+        # generate new root
+        if root == "/":
+            if path == "/":
+                root = "/"
+            elif not path.startswith(".."):
+                if not path.startswith("/"):
+                    path = "/" + path
+                root = path
+            else:
+                root = _apply_double_dots(root, path)
         else:
-            # read from saved cd
-            with open(_CD_FILE) as f:
-                lines = f.readlines()
-                root = lines[0].replace("\n", "")
-
-            if verify:
-                if path.startswith("/"):
-                    paths = [os.path.join(path, p) for p in ls.ls(path, print=False, use_live=False)]
-                else:
-                    paths = [os.path.join(root, p) for p in ls.ls(root, print=False, use_live=False)]
-
-            # generate new root
-            if root == "/":
-                if path == "/":
-                    root = "/"
-                elif not path.startswith(".."):
-                    if not path.startswith("/"):
-                        path = "/" + path
-                    root = path
-                else:
-                    root = _apply_double_dots(root, path)
+            if path.startswith(".."):
+                root = _apply_double_dots(root, path)
+            elif path.startswith("~"):
+                root = path[2:]
             else:
-                if path.startswith(".."):
-                    root = _apply_double_dots(root, path)
-                elif path.startswith("~"):
-                    root = path[2:]
-                else:
-                    root = os.path.join(root, path)
+                root = os.path.join(root, path)
 
-            if verify and root != "/" and not any(p.startswith(root) or root.startswith(p) for p in paths):
-                _error_and_exit(f"no such file or directory: {path}")
+        if verify and root != "/" and not any(p.startswith(root) or root.startswith(p) for p in paths):
+            _error_and_exit(f"no such file or directory: {path}")
 
-            os.remove(_CD_FILE)
+        os.remove(_CD_FILE)
 
-            # store new root
-            with open(_CD_FILE, "w") as f:
-                f.write(root + "\n")
+        # store new root
+        with open(_CD_FILE, "w") as f:
+            f.write(root + "\n")
 
         live.stop()
 
         print(f"cd {root}")
 
     return root
 
 
 def _apply_double_dots(root: str, path: str) -> str:
     splits = [split for split in path.split("/") if split != ""]
     for split in splits:
-        if split == "..":
-            root = "/" + os.path.join(*root.split("/")[:-1])
-        else:
-            root = os.path.join(root, split)
+        root = "/" + os.path.join(*root.split("/")[:-1]) if split == ".." else os.path.join(root, split)
     return root
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/commands/cp.py` & `lightning-app-2.0.3/src/lightning_app/cli/commands/cp.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import concurrent
+import contextlib
 import os
 import sys
 from functools import partial
 from multiprocessing.pool import ApplyResult
 from pathlib import Path
 from textwrap import dedent
 from typing import Any, Optional, Tuple, Union
@@ -50,21 +51,19 @@
 @click.argument("src_path", required=True)
 @click.argument("dst_path", required=True)
 @click.option("-r", required=False, hidden=True)
 @click.option("--recursive", required=False, hidden=True)
 @click.option("--zip", required=False, is_flag=True, default=False)
 def cp(src_path: str, dst_path: str, r: bool = False, recursive: bool = False, zip: bool = False) -> None:
     """Copy files between your local filesystem and the Lightning Cloud filesystem."""
-
     if sys.platform == "win32":
         print("`cp` isn't supported on windows. Open an issue on Github.")
         sys.exit(0)
 
     with Live(Spinner("point", text=Text("pending...", style="white")), transient=True) as live:
-
         pwd = _pwd()
 
         client = LightningClient(retry=False)
 
         src_path, src_remote = _sanitize_path(src_path, pwd)
         dst_path, dst_remote = _sanitize_path(dst_path, pwd)
 
@@ -73,20 +72,22 @@
 
         if not src_remote and dst_remote:
             if dst_path == "/" or len(dst_path.split("/")) == 1:
                 return _error_and_exit("Uploading files at the project level isn't allowed yet.")
             if zip:
                 return _error_and_exit("Zipping uploads isn't supported yet. Please, open a Github issue.")
             _upload_files(live, client, src_path, dst_path, pwd)
-        elif src_remote and not dst_remote:
+            return None
+        if src_remote and not dst_remote:
             if zip:
                 return _zip_files(live, src_path, dst_path)
             _download_files(live, client, src_path, dst_path, pwd)
-        else:
-            return _error_and_exit("Moving files locally isn't supported yet. Please, open a Github issue.")
+            return None
+
+        return _error_and_exit("Moving files locally isn't supported yet. Please, open a Github issue.")
 
 
 def _upload_files(live, client: LightningClient, local_src: str, remote_dst: str, pwd: str) -> str:
     remote_splits = [split for split in remote_dst.split("/") if split != ""]
     remote_dst = os.path.join(*remote_splits)
 
     if not os.path.exists(local_src):
@@ -117,33 +118,30 @@
     clusters = client.projects_service_list_project_cluster_bindings(project_id)
 
     live.stop()
 
     for upload_path in upload_paths:
         for cluster in clusters.clusters:
             filename = str(upload_path).replace(str(os.getcwd()), "")[1:]
-            if lit_resource:
-                filename = _get_prefix(os.path.join(remote_dst, filename), lit_resource)
-            else:
-                filename = "/" + filename
+            filename = _get_prefix(os.path.join(remote_dst, filename), lit_resource) if lit_resource else "/" + filename
 
             response = client.lightningapp_instance_service_upload_project_artifact(
                 project_id=project_id,
                 body=ProjectIdStorageBody(cluster_id=cluster.cluster_id, filename=filename),
                 async_req=True,
             )
             upload_urls.append(response)
 
     upload_urls = [upload_url.get().upload_url for upload_url in upload_urls]
 
     live.stop()
 
     if not upload_paths:
         print("There were no files to upload.")
-        return
+        return None
 
     progress = _get_progress_bar()
 
     total_size = sum([Path(path).stat().st_size for path in upload_paths]) // max(len(clusters.clusters), 1)
     task_id = progress.add_task("upload", filename="", total=total_size)
 
     progress.start()
@@ -155,14 +153,16 @@
 
     progress.stop()
 
     # Raise the first exception found
     exception = next((e for e in results if isinstance(e, Exception)), None)
     if exception:
         _error_and_exit("We detected errors in uploading your files.")
+        return None
+    return None
 
 
 def _upload(source_file: str, presigned_url: ApplyResult, progress: Progress, task_id: TaskID) -> Optional[Exception]:
     source_file = Path(source_file)
     file_uploader = FileUploader(
         presigned_url,
         source_file,
@@ -206,14 +206,15 @@
     progress.start()
     task_id = progress.add_task("download zip", total=None)
 
     _download_file(local_dst, url, progress, task_id)
     progress.stop()
 
     click.echo(f"Downloaded to {local_dst}")
+    return None
 
 
 def _download_files(live, client, remote_src: str, local_dst: str, pwd: str):
     project_id, lit_resource = _get_project_id_and_resource(pwd)
 
     download_paths = []
     download_urls = []
@@ -254,35 +255,30 @@
         _error_and_exit("There was an error downloading your files.")
 
 
 def _download_file(path: str, url: str, progress: Progress, task_id: TaskID) -> None:
     # Disable warning about making an insecure request
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-    try:
-        request = requests.get(url, stream=True, verify=False)
+    with contextlib.suppress(ConnectionError):
+        request = requests.get(url, stream=True, verify=False)  # noqa: S501
 
         chunk_size = 1024
 
         with open(path, "wb") as fp:
             for chunk in request.iter_content(chunk_size=chunk_size):
                 fp.write(chunk)  # type: ignore
                 progress.update(task_id, advance=len(chunk))
-    except ConnectionError:
-        pass
 
 
 def _sanitize_path(path: str, pwd: str) -> Tuple[str, bool]:
     is_remote = _is_remote(path)
     if is_remote:
         path = _remove_remote(path)
-        if path == ".":
-            path = pwd
-        else:
-            path = os.path.join(pwd, path)
+        path = pwd if path == "." else os.path.join(pwd, path)
     return path, is_remote
 
 
 def _is_remote(path: str) -> bool:
     return path.startswith("r:") or path.startswith("remote:")
 
 
@@ -304,19 +300,17 @@
     lit_apps = client.lightningapp_instance_service_list_lightningapp_instances(project_id=project_id).lightningapps
 
     lit_cloud_spaces = client.cloud_space_service_list_cloud_spaces(project_id=project_id).cloudspaces
 
     lit_ressources = [lit_resource for lit_resource in lit_cloud_spaces if lit_resource.name == resource_name]
 
     if len(lit_ressources) == 0:
-
         lit_ressources = [lit_resource for lit_resource in lit_apps if lit_resource.name == resource_name]
 
         if len(lit_ressources) == 0:
-
             print(f"ERROR: There isn't any Lightning Ressource matching the name {resource_name}.")
             sys.exit(0)
 
     return project_id, lit_ressources[0]
 
 
 def _get_project_id_from_name(project_name: str) -> str:
@@ -350,7 +344,8 @@
     if isinstance(lit_resource, Externalv1LightningappInstance):
         return client.cluster_service_get_cluster(lit_resource.spec.cluster_id)
 
     clusters = client.cluster_service_list_clusters()
     for cluster in clusters.clusters:
         if cluster.id == clusters.default_cluster:
             return cluster
+    return None
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/commands/logs.py` & `lightning-app-2.0.3/src/lightning_app/cli/commands/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,27 +31,25 @@
 @click.argument("components", nargs=-1, required=False)
 @click.option("-f", "--follow", required=False, is_flag=True, help="Wait for new logs, to exit use CTRL+C.")
 def logs(app_name: str, components: List[str], follow: bool) -> None:
     """Show cloud application logs. By default, prints logs for all currently available components.
 
     Example uses:
 
-        Print all application logs:
+    Print all application logs:
 
-            $ lightning show logs my-application
+    $ lightning show logs my-application
 
+    Print logs only from the flow (no work):
 
-        Print logs only from the flow (no work):
+    $ lightning show logs my-application flow
 
-            $ lightning show logs my-application flow
+    Print logs only from selected works:
 
-
-        Print logs only from selected works:
-
-            $ lightning show logs my-application root.work_a root.work_b
+    $ lightning show logs my-application root.work_a root.work_b
     """
     _show_logs(app_name, components, follow)
 
 
 def _show_logs(app_name: str, components: List[str], follow: bool) -> None:
     client = LightningClient(retry=False)
     project = _get_project(client)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/commands/ls.py` & `lightning-app-2.0.3/src/lightning_app/cli/commands/ls.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import contextlib
 import os
 import sys
 from contextlib import nullcontext
 from typing import Generator, List, Optional
 
 import click
 import lightning_cloud
@@ -36,28 +36,26 @@
 
 logger = Logger(__name__)
 
 
 @click.argument("path", required=False)
 def ls(path: Optional[str] = None, print: bool = True, use_live: bool = True) -> List[str]:
     """List the contents of a folder in the Lightning Cloud Filesystem."""
-
     from lightning_app.cli.commands.cd import _CD_FILE
 
     if sys.platform == "win32":
         _error_and_exit("`ls` isn't supported on windows. Open an issue on Github.")
 
     root = "/"
 
     context = (
         Live(Spinner("point", text=Text("pending...", style="white")), transient=True) if use_live else nullcontext()
     )
 
     with context:
-
         if not os.path.exists(_LIGHTNING_CONNECTION_FOLDER):
             os.makedirs(_LIGHTNING_CONNECTION_FOLDER)
 
         if not os.path.exists(_CD_FILE):
             with open(_CD_FILE, "w") as f:
                 f.write(root + "\n")
         else:
@@ -104,15 +102,14 @@
             if print:
                 _print_names_with_colors(ressource_names, [_FOLDER_COLOR] * len(ressource_names))
             return ressource_names
 
         lit_ressources = [lit_resource for lit_resource in lit_cloud_spaces if lit_resource.name == splits[1]]
 
         if len(lit_ressources) == 0:
-
             lit_ressources = [lit_resource for lit_resource in lit_apps if lit_resource.name == splits[1]]
 
             if len(lit_ressources) == 0:
                 _error_and_exit(f"There isn't any Lightning Ressource matching the name {splits[1]}.")
 
         lit_resource = lit_ressources[0]
 
@@ -124,15 +121,14 @@
 
         depth = len(splits)
 
         prefix = "/".join(splits[2:])
         prefix = _get_prefix(prefix, lit_resource)
 
         for artifact in _collect_artifacts(client=client, project_id=project_id, prefix=prefix):
-
             if str(artifact.filename).startswith("/"):
                 artifact.filename = artifact.filename[1:]
 
             path = os.path.join(project_id, prefix[1:], artifact.filename)
 
             artifact_splits = path.split("/")
 
@@ -187,19 +183,16 @@
         row = index // num_cols
         if row not in columns:
             columns[row] = []
         columns[row].append((name, color))
 
     for row_index in sorted(columns):
         row = ""
-        for (name, color) in columns[row_index]:
-            if use_spacing:
-                spacing = padding
-            else:
-                spacing = max_L - len(name)
+        for name, color in columns[row_index]:
+            spacing = padding if use_spacing else max_L - len(name)
             spaces = " " * spacing
             row += _add_colors(name, color) + spaces
         rich.print(row)
 
 
 def _collect_artifacts(
     client: LightningClient,
@@ -224,19 +217,20 @@
                 cluster_id=cluster.cluster_id,
                 page_token=page_token,
                 tokens=tokens,
                 page_size=page_size,
                 include_download_url=include_download_url,
             )
     else:
-
         if page_token in tokens:
             return
 
-        try:
+        # Note: This is triggered when the request is wrong.
+        # This is currently happening due to looping through the user clusters.
+        with contextlib.suppress(lightning_cloud.openapi.rest.ApiException):
             response = client.lightningapp_instance_service_list_project_artifacts(
                 project_id,
                 prefix=prefix,
                 cluster_id=cluster_id,
                 page_token=page_token,
                 include_download_url=include_download_url,
                 page_size=str(page_size),
@@ -252,18 +246,14 @@
                     client,
                     project_id,
                     prefix=prefix,
                     cluster_id=cluster_id,
                     page_token=response.next_page_token,
                     tokens=tokens,
                 )
-        except lightning_cloud.openapi.rest.ApiException:
-            # Note: This is triggered when the request is wrong.
-            # This is currently happening due to looping through the user clusters.
-            pass
 
 
 def _add_resource_prefix(prefix: str, resource_path: str):
     if resource_path in prefix:
         return prefix
     prefix = os.path.join(resource_path, prefix)
     if not prefix.startswith("/"):
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/commands/pwd.py` & `lightning-app-2.0.3/src/lightning_app/cli/commands/pwd.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,19 @@
 from lightning_app.utilities.app_helpers import Logger
 
 logger = Logger(__name__)
 
 
 def pwd() -> str:
     """Print your current working directory in the Lightning Cloud filesystem."""
-
     if sys.platform == "win32":
         print("`pwd` isn't supported on windows. Open an issue on Github.")
         sys.exit(0)
 
     with Live(Spinner("point", text=Text("pending...", style="white")), transient=True):
-
         root = _pwd()
 
     print(root)
 
     return root
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/commands/rm.py` & `lightning-app-2.0.3/src/lightning_app/cli/commands/rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import contextlib
 import os
 
 import click
 import lightning_cloud
 import rich
 
 from lightning_app.cli.commands.ls import _add_colors, _get_prefix
@@ -28,15 +28,14 @@
 
 
 @click.argument("rm_path", required=True)
 @click.option("-r", required=False, hidden=True)
 @click.option("--recursive", required=False, hidden=True)
 def rm(rm_path: str, r: bool = False, recursive: bool = False) -> None:
     """Delete files on the Lightning Cloud filesystem."""
-
     root = _pwd()
 
     if rm_path in (".", ".."):
         return _error_and_exit('rm "." and ".." may not be removed')
 
     if ".." in rm_path:
         return _error_and_exit('rm ".." or higher may not be removed')
@@ -66,39 +65,37 @@
 
     lit_apps = lit_apps.get().lightningapps
     lit_cloud_spaces = lit_cloud_spaces.get().cloudspaces
 
     lit_ressources = [lit_resource for lit_resource in lit_cloud_spaces if lit_resource.name == splits[1]]
 
     if len(lit_ressources) == 0:
-
         lit_ressources = [lit_resource for lit_resource in lit_apps if lit_resource.name == splits[1]]
 
         if len(lit_ressources) == 0:
             _error_and_exit(f"There isn't any Lightning Ressource matching the name {splits[1]}.")
 
     lit_resource = lit_ressources[0]
 
     prefix = "/".join(splits[2:])
     prefix = _get_prefix(prefix, lit_resource)
 
     clusters = client.projects_service_list_project_cluster_bindings(project_id)
     succeeded = False
 
     for cluster in clusters.clusters:
-        try:
+        with contextlib.suppress(lightning_cloud.openapi.rest.ApiException):
             client.lightningapp_instance_service_delete_project_artifact(
                 project_id=project_id,
                 cluster_id=cluster.cluster_id,
                 filename=prefix,
             )
             succeeded = True
             break
-        except lightning_cloud.openapi.rest.ApiException:
-            pass
 
     prefix = os.path.join(*splits)
 
     if succeeded:
         rich.print(_add_colors(f"Successfuly deleted `{prefix}`.", color="green"))
-    else:
-        return _error_and_exit(f"No file or folder named `{prefix}` was found.")
+        return None
+
+    return _error_and_exit(f"No file or folder named `{prefix}` was found.")
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml` & `lightning-app-2.0.3/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/component-template/.gitignore` & `lightning-app-2.0.3/src/lightning_app/cli/component-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/component-template/LICENSE` & `lightning-app-2.0.3/src/lightning_app/cli/component-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/component-template/README.md` & `lightning-app-2.0.3/src/lightning_app/cli/component-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/connect/app.py` & `lightning-app-2.0.3/src/lightning_app/cli/connect/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,14 @@
             else:
                 click.echo(f"You are already connected to the cloud Lightning App: {app_name_or_id}.")
         else:
             disconnect_app()
             connect_app(app_name_or_id)
 
     elif app_name_or_id.startswith("localhost"):
-
         with Progress() as progress_bar:
             connecting = progress_bar.add_task("[magenta]Setting things up for you...", total=1.0)
 
             if app_name_or_id != "localhost":
                 raise Exception("You need to pass localhost to connect to the local Lightning App.")
 
             retriever = _LightningAppOpenAPIRetriever(None)
@@ -136,15 +135,14 @@
             f"LIGHTNING_CONNECT_PPID={_PPID} {sys.executable} -m lightning --help",
             shell=True,
             stdout=sys.stdout,
             stderr=sys.stderr,
         ).wait()
 
     elif matched_connection_path:
-
         matched_connected_file = os.path.join(matched_connection_path, "connect.txt")
         matched_commands = os.path.join(matched_connection_path, "commands")
         if os.path.isdir(matched_commands):
             commands = os.path.join(_LIGHTNING_CONNECTION_FOLDER, "commands")
             shutil.copytree(matched_commands, commands)
             shutil.copy(matched_connected_file, connected_file)
 
@@ -362,15 +360,15 @@
             connection = os.path.join(_LIGHTNING_CONNECTION, str(ppid))
             if os.path.exists(connection):
                 shutil.rmtree(connection)
 
 
 def _scan_lightning_connections(app_name_or_id):
     if not os.path.exists(_LIGHTNING_CONNECTION):
-        return
+        return None
 
     for ppid in os.listdir(_LIGHTNING_CONNECTION):
         try:
             psutil.Process(int(ppid))
         except (psutil.NoSuchProcess, ValueError):
             continue
 
@@ -378,11 +376,11 @@
 
         connected_file = os.path.join(connection_path, "connect.txt")
         curr_app_name, curr_app_id = _read_connected_file(connected_file)
 
         if not curr_app_name:
             continue
 
-        if app_name_or_id == curr_app_name or app_name_or_id == curr_app_id:
+        if app_name_or_id in (curr_app_name, curr_app_id):
             return connection_path
 
     return None
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/connect/data.py` & `lightning-app-2.0.3/src/lightning_app/cli/connect/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,24 +58,22 @@
 
     from lightning_cloud.openapi import Create, V1AwsDataConnection
 
     if sys.platform == "win32":
         _error_and_exit("Data connection isn't supported on windows. Open an issue on Github.")
 
     with Live(Spinner("point", text=Text("pending...", style="white")), transient=True) as live:
-
         live.stop()
 
         client = LightningClient(retry=False)
         projects = client.projects_service_list_memberships()
 
         project_id = None
 
         for project in projects.memberships:
-
             if project.name == project_name:
                 project_id = project.project_id
                 break
 
         if project_id is None:
             project_id = _get_project(client).project_id
 
@@ -104,7 +102,8 @@
             #     id=response.id,
             # )
         except lightning_cloud.openapi.rest.ApiException as e:
             message = ast.literal_eval(e.body.decode("utf-8"))["message"]
             _error_and_exit(f"The data connection creation failed. Message: {message}")
 
     rich.print(f"[green]Succeeded[/green]: You have created a new data connection {name}.")
+    return None
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/connect/maverick.py` & `lightning-app-2.0.3/src/lightning_app/cli/connect/maverick.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,29 +98,28 @@
 
     if "lightning.ai" in CLOUD_PROXY_HOST:
         _error_and_exit("Maverick connection isn't publicly available. Open an issue on Github.")
 
     with Live(Spinner("point", text=Text("Registering maverick...", style="white")), transient=True) as live:
         try:
             register_to_cloud(name, project_name)
-        except Exception as e:
+        except Exception as ex:
             live.stop()
-            rich.print(f"[red]Failed[/red]: Registering maverick failed with error {e}")
+            rich.print(f"[red]Failed[/red]: Registering maverick failed with error {ex}")
             return
 
         live.update(Spinner("point", text=Text("Setting up ...", style="white")))
 
         # run network creation in the background
         out = subprocess.run(CMD_CREATE_NETWORK, shell=True, capture_output=True)
         error = out.stderr
-        if error:
-            if "already exists" not in str(error):
-                live.stop()
-                rich.print(f"[red]Failed[/red]: network creation failed with error: {str(error)}")
-                return
+        if error and "already exists" not in str(error):
+            live.stop()
+            rich.print(f"[red]Failed[/red]: network creation failed with error: {str(error)}")
+            return
 
         # if code server is already running, ignore.
         # If not, but container exists, remove it and run. Otherwise, run.
         out = subprocess.run(
             f"docker ps -q -f name={CODE_SERVER_CONTAINER}", shell=True, check=True, capture_output=True
         )
         if out.stdout:
@@ -206,16 +205,16 @@
 
 @click.argument("name", required=True)
 def disconnect_maverick(name: str) -> None:
     # disconnect stop and remove the docker containers
     with Live(Spinner("point", text=Text("disconnecting maverick...", style="white")), transient=True):
         try:
             deregister_from_cloud(name)
-        except Exception as e:
-            rich.print(f"[red]Failed[/red]: Disconnecting machine failed with error: {e}")
+        except Exception as ex:
+            rich.print(f"[red]Failed[/red]: Disconnecting machine failed with error: {ex}")
             return
         subprocess.run(f"docker stop {CODE_SERVER_CONTAINER}", shell=True, capture_output=True)
         subprocess.run(f"docker stop {LIGHTNING_DAEMON_CONTAINER}", shell=True, capture_output=True)
     rich.print(f"[green]Succeeded[/green]: maverick {name} has been disconnected from lightning.")
 
 
 def register_to_cloud(name: str, project_name: str) -> None:
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/core.py` & `lightning-app-2.0.3/src/lightning_app/cli/core.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/lightning_cli.py` & `lightning-app-2.0.3/src/lightning_app/cli/lightning_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,34 +186,30 @@
 @click.option("--limit", default=10000, help="The max number of log lines returned.")
 @click.option("-f", "--follow", required=False, is_flag=True, help="Wait for new logs, to exit use CTRL+C.")
 def cluster_logs(cluster_id: str, to_time: arrow.Arrow, from_time: arrow.Arrow, limit: int, follow: bool) -> None:
     """Show cluster logs.
 
     Example uses:
 
-        Print cluster logs:
+    Print cluster logs:
 
-            $ lightning show cluster logs my-cluster
+    $ lightning show cluster logs my-cluster
 
+    Print cluster logs and wait for new logs:
 
-        Print cluster logs and wait for new logs:
+    $ lightning show cluster logs my-cluster --follow
 
-            $ lightning show cluster logs my-cluster --follow
+    Print cluster logs, from 48 hours ago to now:
 
+    $ lightning show cluster logs my-cluster --from "48 hours ago"
 
-        Print cluster logs, from 48 hours ago to now:
+    Print cluster logs, 10 most recent lines:
 
-            $ lightning show cluster logs my-cluster --from "48 hours ago"
-
-
-        Print cluster logs, 10 most recent lines:
-
-            $ lightning show cluster logs my-cluster --limit 10
+    $ lightning show cluster logs my-cluster --limit 10
     """
-
     client = LightningClient(retry=False)
     cluster_manager = AWSClusterManager()
     existing_cluster_list = cluster_manager.get_clusters()
 
     clusters = {cluster.id: cluster.id for cluster in existing_cluster_list.clusters}
 
     if not clusters:
@@ -244,16 +240,16 @@
 
         for log_event in log_reader:
             date = log_event.timestamp.strftime("%m/%d/%Y %H:%M:%S")
             color = colors.get(log_event.labels.level, "green")
             rich.print(f"[{color}]{log_event.labels.level:5}[/{color}] {date} {log_event.message.rstrip()}")
     except LogLinesLimitExceeded:
         raise click.ClickException(f"Read {limit} log lines, but there may be more. Use --limit param to read more")
-    except Exception as error:
-        logger.error(f"⚡ Error while reading logs ({type(error)}), {error}", exc_info=DEBUG)
+    except Exception as ex:
+        logger.error(f"⚡ Error while reading logs ({type(ex)}), {ex}", exc_info=DEBUG)
 
 
 @_main.command()
 def login() -> None:
     """Log in to your lightning.ai account."""
     auth = Auth()
     auth.clear()
@@ -282,15 +278,14 @@
     blocking: bool,
     open_ui: bool,
     env: tuple,
     secret: tuple,
     run_app_comment_commands: bool,
     enable_basic_auth: str,
 ) -> None:
-
     if not os.path.exists(file):
         original_file = file
         file = cmd_install.gallery_apps_and_components(file, True, "latest", overwrite=True)  # type: ignore[assignment]  # noqa E501
         if file is None:
             click.echo(f"The provided entrypoint `{original_file}` doesn't exist.")
             sys.exit(1)
         run_app_comment_commands = True
@@ -308,17 +303,16 @@
                 "Using the flag --no-cache in local execution is not supported."
             )
         if secret:
             raise click.ClickException(
                 "Secrets can only be used for apps running in cloud. "
                 "Using the option --secret in local execution is not supported."
             )
-        if ENABLE_APP_COMMENT_COMMAND_EXECUTION or run_app_comment_commands:
-            if file is not None:
-                run_app_commands(str(file))
+        if (ENABLE_APP_COMMENT_COMMAND_EXECUTION or run_app_comment_commands) and file is not None:
+            run_app_commands(str(file))
 
     env_vars = _format_input_env_variables(env)
     os.environ.update(env_vars)
 
     secrets = _format_input_env_variables(secret)
 
     port = _find_lit_app_port(constants.APP_SERVER_PORT)
@@ -440,15 +434,14 @@
     type=str,
     default=None,
     help="Open on a specific Lightning AI BYOC compute cluster",
 )
 @click.option("--name", help="The name to use for the CloudSpace", default="", type=str)
 def open(path: str, cluster_id: str, name: str) -> None:
     """Open files or folders from your machine in a Lightning CloudSpace."""
-
     if not os.path.exists(path):
         click.echo(f"The provided path `{path}` doesn't exist.")
         sys.exit(1)
 
     runtime = CloudRuntime(entrypoint=Path(path))
     runtime.open(name, cluster_id)
 
@@ -472,15 +465,14 @@
     "component_name",
     type=str,
     default=None,
     help="Specify which component to SSH into",
 )
 def ssh(app_name: Optional[str] = None, component_name: Optional[str] = None) -> None:
     """SSH into a Lightning App."""
-
     app_manager = _AppManager()
     apps = app_manager.list_apps(phase_in=[V1LightningappInstanceState.RUNNING])
     if len(apps) == 0:
         raise click.ClickException("No running apps available. Start a Lightning App in the cloud to use this feature.")
 
     available_app_names = [app.name for app in apps]
     if app_name is None:
@@ -533,15 +525,15 @@
     ssh_endpoint = app_cluster.status.ssh_gateway_endpoint
 
     ssh_path = shutil.which("ssh")
     if ssh_path is None:
         raise click.ClickException(
             "Unable to find the ssh binary. You must install ssh first to use this functionality."
         )
-    os.execv(ssh_path, ["-tt", f"{component_id}@{ssh_endpoint}"])
+    os.execv(ssh_path, ["-tt", f"{component_id}@{ssh_endpoint}"])  # noqa: S606
 
 
 @_main.group()
 def init() -> None:
     """Init a Lightning App and/or component."""
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_create.py` & `lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,13 +113,13 @@
 ) -> None:
     """Add a new Lightning AI ssh-key to your account."""
     ssh_key_manager = _SSHKeyManager()
 
     new_public_key = Path(str(public_key)).read_text() if os.path.isfile(str(public_key)) else public_key
     try:
         ssh_key_manager.add_key(name=key_name, comment=comment, public_key=str(new_public_key))
-    except ApiException as e:
+    except ApiException as ex:
         # if we got an exception it might be the user passed the private key file
         if os.path.isfile(str(public_key)) and os.path.isfile(f"{public_key}.pub"):
             ssh_key_manager.add_key(name=key_name, comment=comment, public_key=Path(f"{public_key}.pub").read_text())
         else:
-            raise e
+            raise ex
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_delete.py` & `lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,20 +207,20 @@
     except InterruptedError:
         return
 
     try:
         # Delete the app!
         app_manager = _AppManager()
         app_manager.delete(app_id=selected_app_instance_id)
-    except Exception as e:
+    except Exception as ex:
         console.print(
             f'[b][red]An issue occurred while deleting app "{app_name}. If the issue persists, please '
             "reach out to us at [link=mailto:support@lightning.ai]support@lightning.ai[/link][/b][/red]."
         )
-        raise click.ClickException(str(e))
+        raise click.ClickException(str(ex))
 
     console.print(f'[b][green]App "{app_name}" has been successfully deleted from cluster "{cluster_id}"![/green][/b]')
     return
 
 
 @delete.command("ssh-key")
 @click.argument("key_id")
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_list.py` & `lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/app.py` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,20 +86,21 @@
         if hasattr(self, "logger_component"):
             tabs.extend(self.logger_component.configure_layout())
         return tabs
 
     def _choose_logger_component(self) -> Optional[Union[TensorBoard, WeightsAndBiases]]:
         logger_metadatas = self.script_orchestrator.script_runner.logger_metadatas
         if not logger_metadatas:
-            return
+            return None
         if logger_metadatas[0].get("class_name") == "TensorBoardLogger":
             return TensorBoard(log_dir=self.script_orchestrator.script_runner.log_dir)
         if logger_metadatas[0].get("class_name") == "WandbLogger":
             return WeightsAndBiases(
                 username=logger_metadatas[0]["username"],
                 project_name=logger_metadatas[0]["project_name"],
                 run_id=logger_metadatas[0]["run_id"],
                 api_key=self.script_orchestrator.environment_variables.get("WANDB_API_KEY"),
             )
+        return None
 
 
 app = LightningApp(Main())
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/callbacks.py` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,21 +154,17 @@
         if self.is_enabled:
             self._send_state()
 
     def _train_batch_idx(self, trainer: "pl.Trainer") -> int:
         return trainer.fit_loop.epoch_loop.batch_progress.current.processed
 
     def _val_batch_idx(self, trainer: "pl.Trainer") -> int:
-        if trainer.state.fn == "fit":
-            loop = trainer.fit_loop.epoch_loop.val_loop
-        else:
-            loop = trainer.validate_loop
+        loop = trainer.fit_loop.epoch_loop.val_loop if trainer.state.fn == "fit" else trainer.validate_loop
 
-        current_batch_idx = loop.epoch_loop.batch_progress.current.processed
-        return current_batch_idx
+        return loop.epoch_loop.batch_progress.current.processed
 
     def _test_batch_idx(self, trainer: "pl.Trainer") -> int:
         return trainer.test_loop.epoch_loop.batch_progress.current.processed
 
     def _predict_batch_idx(self, trainer: "pl.Trainer") -> int:
         return trainer.predict_loop.epoch_loop.batch_progress.current.processed
 
@@ -265,16 +261,15 @@
         stage: str,
     ) -> None:
         self.work.model_hparams = self._sanitize_model_init_args(dict(**pl_module.hparams))
 
     def _sanitize_trainer_init_args(self, init_args: Dict[str, Any]) -> Dict[str, str]:
         if init_args["callbacks"]:
             init_args["callbacks"] = [c.__class__.__name__ for c in init_args["callbacks"]]
-        init_args = {k: str(v) for k, v in init_args.items()}
-        return init_args
+        return {k: str(v) for k, v in init_args.items()}
 
     def _sanitize_model_init_args(self, init_args: Dict[str, Any]) -> Dict[str, str]:
         return {k: str(v) for k, v in init_args.items()}
 
 
 class PLAppArtifactsTracker(Callback):
     def __init__(self, work: "ScriptRunner") -> None:
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/state.py` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/setup.py` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from core.components.script_runner import ScriptRunner
 
 from lightning_app.storage import Path
 from pytorch_lightning import LightningModule, Trainer
 from pytorch_lightning.loggers import TensorBoardLogger
 
 
-@pytest.mark.parametrize("rank", (0, 1))
+@pytest.mark.parametrize("rank", [0, 1])
 def test_progress_tracker_enabled(rank):
     trainer = Mock()
     trainer.global_rank = rank
     trainer.is_global_zero = rank == 0
     work = Mock()
     tracker = PLAppProgressTracker(work)
     assert not tracker.is_enabled
```

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/.prettierrc` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/.prettierrc`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/craco.config.js` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/craco.config.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/package.json` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/index.html` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/App.tsx` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/index.tsx` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/tsconfig.json` & `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/README.md` & `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/example_app.py` & `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/example_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/package.json` & `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/App.tsx` & `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg` & `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts` & `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/tsconfig.json` & `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/yarn.lock` & `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/yarn.lock`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/__init__.py` & `lightning-app-2.0.3/src/lightning_app/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/database/client.py` & `lightning-app-2.0.3/src/lightning_app/components/database/client.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/database/server.py` & `lightning-app-2.0.3/src/lightning_app/components/database/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,16 @@
         return self.db_url != ""
 
     @property
     def db_url(self) -> Optional[str]:
         use_localhost = "LIGHTNING_APP_STATE_URL" not in os.environ
         if use_localhost:
             return self.url
-        if self.internal_ip != "":
-            return f"http://{self.internal_ip}:{self.port}"
-        return self.internal_ip
+        ip_addr = self.public_ip or self.internal_ip
+        if ip_addr != "":
+            return f"http://{ip_addr}:{self.port}"
+        return ip_addr
 
     def on_exit(self):
         self._exit_event.set()
         with _lock:
             self.store_database()
```

### Comparing `lightning-app-2.0.2/src/lightning_app/components/database/utilities.py` & `lightning-app-2.0.3/src/lightning_app/components/database/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,42 +84,39 @@
                         # This allows to assign non-InDB models and if they're
                         # compatible, they're directly parsed into the InDB
                         # representation, thus hiding the implementation in the
                         # background. However, the InDB model will still be returned
                         value_to_dump = pydantic_type.from_orm(value)
                     else:
                         value_to_dump = value
-                    value = dumps(jsonable_encoder(value_to_dump))
-                    return value
+                    return dumps(jsonable_encoder(value_to_dump))
 
             return process
 
         def result_processor(self, dialect, coltype) -> T:
             impl_processor = self.impl.result_processor(dialect, coltype)
             if impl_processor:
 
                 def process(value):
                     value = impl_processor(value)
                     if value is None:
                         return None
 
                     data = value
                     # Explicitly use the generic directly, not type(T)
-                    full_obj = parse_obj_as(pydantic_type, data)
-                    return full_obj
+                    return parse_obj_as(pydantic_type, data)
 
             else:
 
                 def process(value):
                     if value is None:
                         return None
 
                     # Explicitly use the generic directly, not type(T)
-                    full_obj = parse_obj_as(pydantic_type, value)
-                    return full_obj
+                    return parse_obj_as(pydantic_type, value)
 
             return process
 
         def compare_values(self, x, y):
             return x == y
 
     return PydanticJSONType
@@ -221,14 +218,15 @@
                 if k in ("id", "_sa_instance_state"):
                     continue
                 if getattr(result, k) != v:
                     setattr(result, k, v)
             session.add(result)
             session.commit()
             session.refresh(result)
+            return None
 
 
 class _Delete:
     def __init__(self, models, token):
         self.models = models
         self.token = token
 
@@ -242,21 +240,22 @@
             primary_key = _get_primary_key(update_data.__class__)
             identifier = getattr(update_data.__class__, primary_key, None)
             statement = select(update_data.__class__).where(identifier == getattr(update_data, primary_key))
             results = session.exec(statement)
             result = results.one()
             session.delete(result)
             session.commit()
+            return None
 
 
 def _create_database(db_filename: str, models: List[Type["SQLModel"]], echo: bool = False):
     global engine
 
     from sqlmodel import create_engine
 
     engine = create_engine(f"sqlite:///{pathlib.Path(db_filename).resolve()}", echo=echo)
 
     logger.debug(f"Creating the following tables {models}")
     try:
         SQLModel.metadata.create_all(engine)
-    except Exception as e:
-        logger.debug(e)
+    except Exception as ex:
+        logger.debug(ex)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/components/multi_node/base.py` & `lightning-app-2.0.3/src/lightning_app/components/multi_node/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,14 @@
     def run(self) -> None:
         # 1. Wait for all works to be started !
         if not all(w.internal_ip for w in self.ws):
             return
 
         # 2. Loop over all node machines
         for node_rank in range(len(self.ws)):
-
             # 3. Run the user code in a distributed way !
             self.ws[node_rank].run(
                 main_address=self.ws[0].internal_ip,
                 main_port=self.ws[0].port,
                 num_nodes=len(self.ws),
                 node_rank=node_rank,
             )
```

### Comparing `lightning-app-2.0.2/src/lightning_app/components/multi_node/fabric.py` & `lightning-app-2.0.3/src/lightning_app/components/multi_node/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/multi_node/pytorch_spawn.py` & `lightning-app-2.0.3/src/lightning_app/components/multi_node/pytorch_spawn.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         work_run: Callable,
         main_address: str,
         main_port: int,
         num_nodes: int,
         node_rank: int,
         nprocs: int,
     ):
-
         import torch
 
         # 1. Setting distributed environment
         global_rank = local_rank + node_rank * nprocs
         world_size = num_nodes * nprocs
 
         if torch.distributed.is_available():
```

### Comparing `lightning-app-2.0.2/src/lightning_app/components/multi_node/trainer.py` & `lightning-app-2.0.3/src/lightning_app/components/multi_node/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/python/popen.py` & `lightning-app-2.0.3/src/lightning_app/components/python/popen.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/python/tracer.py` & `lightning-app-2.0.3/src/lightning_app/components/python/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/serve/__init__.py` & `lightning-app-2.0.3/src/lightning_app/components/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/serve/auto_scaler.py` & `lightning-app-2.0.3/src/lightning_app/components/serve/auto_scaler.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,17 +68,16 @@
     if isinstance(exception, aiohttp.client_exceptions.ClientError):
         logging.exception(exception)
         raise HTTPException(500, "Worker Server error") from exception
 
     if isinstance(exception, asyncio.TimeoutError):
         raise HTTPException(408, "Request timed out") from exception
 
-    if isinstance(exception, Exception):
-        if exception.args[0] == "Server disconnected":
-            raise HTTPException(500, "Worker Server disconnected") from exception
+    if isinstance(exception, Exception) and exception.args[0] == "Server disconnected":
+        raise HTTPException(500, "Worker Server disconnected") from exception
 
     logging.exception(exception)
     raise HTTPException(500, exception.args[0]) from exception
 
 
 class _SysInfo(BaseModel):
     num_workers: int
@@ -177,17 +176,17 @@
                 self._cold_start_proxy = ColdStartProxy(proxy_url=cold_start_proxy)
             elif isinstance(cold_start_proxy, ColdStartProxy):
                 self._cold_start_proxy = cold_start_proxy
             else:
                 raise ValueError("cold_start_proxy must be of type ColdStartProxy or str")
 
     def get_internal_url(self) -> str:
-        if not self._internal_ip:
-            raise ValueError("Internal IP not set")
-        return f"http://{self._internal_ip}:{self._port}"
+        if not self._public_ip:
+            raise ValueError("Public IP not set")
+        return f"http://{self._public_ip}:{self._port}"
 
     async def send_batch(self, batch: List[Tuple[str, _BatchRequestModel]], server_url: str):
         request_data: List[_LoadBalancer._input_type] = [b[1] for b in batch]
         batch_request_data = _BatchRequestModel(inputs=request_data)
 
         try:
             self._server_status[server_url] = False
@@ -226,14 +225,15 @@
         existing = set(self._server_status.keys())
         for server in existing:
             status = self._server_status.get(server, None)
             if status is None:
                 logger.error("Server is not found in the status list. This should not happen.")
             if status:
                 return server
+        return None
 
     async def consumer(self):
         """The consumer process that continuously checks for new requests and sends them to the API.
 
         Two instances of this function should not be running with shared `_state_server` as that would create race
         conditions
         """
@@ -308,15 +308,15 @@
         fastapi_app.SEND_TASK = None
         self._fastapi_app = fastapi_app
 
         input_type = self._input_type
 
         @fastapi_app.middleware("http")
         async def current_request_counter(request: Request, call_next):
-            if not request.scope["path"] == self.endpoint:
+            if request.scope["path"] != self.endpoint:
                 return await call_next(request)
             fastapi_app.global_request_count += 1
             fastapi_app.num_current_requests += 1
             start_time = time.time()
             response = await call_next(request)
             processing_time = time.time() - start_time
             fastapi_app.last_processing_time = processing_time
@@ -382,15 +382,15 @@
     def update_servers(self, server_works: List[LightningWork]):
         """Updates works that load balancer distributes requests to.
 
         AutoScaler uses this method to increase/decrease the number of works.
         """
         old_server_urls = set(self.servers)
         current_server_urls = {
-            f"http://{server._internal_ip}:{server.port}" for server in server_works if server._internal_ip
+            f"http://{server._public_ip}:{server.port}" for server in server_works if server._internal_ip
         }
 
         # doing nothing if no server work has been added/removed
         if old_server_urls == current_server_urls:
             return
 
         # checking if the url is ready or not
@@ -452,15 +452,15 @@
     def _get_endpoint_info_page(self) -> Optional["APIAccessFrontend"]:  # noqa: F821
         try:
             from lightning_api_access import APIAccessFrontend
         except ModuleNotFoundError:
             logger.warn(
                 "Some dependencies to run the UI are missing. To resolve, run `pip install lightning-api-access`"
             )
-            return
+            return None
 
         if is_running_in_cloud():
             url = f"{self._future_url}{self.endpoint}"
         else:
             url = f"http://localhost:{self.port}{self.endpoint}"
 
         frontend_objects = {"name": self._api_name, "url": url, "method": "POST", "request": None, "response": None}
@@ -637,16 +637,15 @@
         work.stop()
         self.num_replicas -= 1
         return work_attribute
 
     def get_work(self, index: int) -> LightningWork:
         """Returns the ``LightningWork`` instance with the given index."""
         work_attribute = self._work_registry[index]
-        work = getattr(self, work_attribute)
-        return work
+        return getattr(self, work_attribute)
 
     def run(self):
         if not self.load_balancer.is_running:
             self.load_balancer.run()
         for work in self.workers:
             work.run()
         if self.load_balancer.url:
@@ -738,12 +737,11 @@
                 logger.info(f"Work removed: '{removed_work_id}'")
             if num_workers_to_remove > 0:
                 self._last_autoscale = time.time()
 
         self.load_balancer.update_servers(self.workers)
 
     def configure_layout(self):
-        tabs = [
+        return [
             {"name": "Endpoint Info", "content": f"{self.load_balancer.url}/endpoint-info"},
             {"name": "Swagger", "content": self.load_balancer.url},
         ]
-        return tabs
```

### Comparing `lightning-app-2.0.2/src/lightning_app/components/serve/catimage.png` & `lightning-app-2.0.3/src/lightning_app/components/serve/catimage.png`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/serve/cold_start_proxy.py` & `lightning-app-2.0.3/src/lightning_app/components/serve/cold_start_proxy.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/serve/gradio_server.py` & `lightning-app-2.0.3/src/lightning_app/components/serve/gradio_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/serve/python_server.py` & `lightning-app-2.0.3/src/lightning_app/components/serve/python_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 
     _TORCH_GREATER_EQUAL_1_12 = compare_version("torch", operator.ge, "1.12.0")
 
     local_rank = int(os.getenv("LOCAL_RANK", "0"))
 
     if _TORCH_GREATER_EQUAL_1_12 and torch.backends.mps.is_available() and platform.processor() in ("arm", "arm64"):
         return torch.device("mps", local_rank)
-    else:
-        return torch.device(f"cuda:{local_rank}" if torch.cuda.is_available() else "cpu")
+
+    return torch.device(f"cuda:{local_rank}" if torch.cuda.is_available() else "cpu")
 
 
 class _DefaultInputData(BaseModel):
     payload: str
 
 
 class _DefaultOutputData(BaseModel):
@@ -292,15 +292,15 @@
     def configure_layout(self) -> Optional["Frontend"]:
         try:
             from lightning_api_access import APIAccessFrontend
         except ModuleNotFoundError:
             logger.warn(
                 "Some dependencies to run the UI are missing. To resolve, run `pip install lightning-api-access`"
             )
-            return
+            return None
 
         class_name = self.__class__.__name__
         url = f"{self.url}/predict"
 
         try:
             request = self._get_sample_dict_from_datatype(self.configure_input_type())
             response = self._get_sample_dict_from_datatype(self.configure_output_type())
```

### Comparing `lightning-app-2.0.2/src/lightning_app/components/serve/serve.py` & `lightning-app-2.0.3/src/lightning_app/components/serve/serve.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/serve/streamlit.py` & `lightning-app-2.0.3/src/lightning_app/components/serve/streamlit.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             return getattr(self._state, name)
         except AttributeError:
             # The name isn't in the state, so check if it's a callable or a property
             attribute = inspect.getattr_static(self._work_class, name)
             if callable(attribute):
                 attribute = attribute.__get__(self, self._work_class)
                 return attribute
-            elif isinstance(attribute, (staticmethod, property)):
+            if isinstance(attribute, (staticmethod, property)):
                 return attribute.__get__(self, self._work_class)
 
             # Look for the name in the instance (e.g. for private variables)
             return object.__getattribute__(self, name)
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name in ["_state", "_work_class"]:
```

### Comparing `lightning-app-2.0.2/src/lightning_app/components/serve/types/image.py` & `lightning-app-2.0.3/src/lightning_app/components/serve/types/image.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/serve/types/type.py` & `lightning-app-2.0.3/src/lightning_app/components/serve/types/type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/components/training.py` & `lightning-app-2.0.3/src/lightning_app/components/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         from pytorch_lightning import Trainer
         from pytorch_lightning.cli import LightningCLI
 
         for v in script_globals.values():
             if isinstance(v, LightningCLI):
                 trainer = v.trainer
                 break
-            elif isinstance(v, Trainer):
+            if isinstance(v, Trainer):
                 trainer = v
                 break
         else:
             raise RuntimeError("No trainer instance found.")
 
         self.monitor = trainer.checkpoint_callback.monitor
```

### Comparing `lightning-app-2.0.2/src/lightning_app/core/api.py` & `lightning-app-2.0.3/src/lightning_app/core/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import asyncio
+import contextlib
 import json
 import os
 import queue
+import socket
 import sys
 import traceback
 from copy import deepcopy
 from multiprocessing import Queue
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from threading import Event, Lock, Thread
@@ -43,41 +45,43 @@
     ENABLE_PULLING_STATE_ENDPOINT,
     ENABLE_PUSHING_STATE_ENDPOINT,
     ENABLE_STATE_WEBSOCKET,
     ENABLE_UPLOAD_ENDPOINT,
     FRONTEND_DIR,
     get_cloud_queue_type,
 )
+from lightning_app.core.flow import LightningFlow
 from lightning_app.core.queues import QueuingSystem
+from lightning_app.core.work import LightningWork
 from lightning_app.storage import Drive
 from lightning_app.utilities.app_helpers import InMemoryStateStore, Logger, StateStore
 from lightning_app.utilities.app_status import AppStatus
 from lightning_app.utilities.cloud import is_running_in_cloud
 from lightning_app.utilities.component import _context
 from lightning_app.utilities.enum import ComponentContext, OpenAPITags
 from lightning_app.utilities.imports import _is_starsessions_available
 
 if _is_starsessions_available():
     from starsessions import SessionMiddleware
 else:
 
-    class SessionMiddleware:
+    class SessionMiddleware:  # type: ignore[no-redef]
         pass
 
 
 # TODO: fixed uuid for now, it will come from the FastAPI session
 TEST_SESSION_UUID = "1234"
 
 STATE_EVENT = "State changed"
 
 frontend_static_dir = os.path.join(FRONTEND_DIR, "static")
 
-api_app_delta_queue: Queue = None
+api_app_delta_queue: Optional[Queue] = None
 
-template = {"ui": {}, "app": {}}
+template: dict = {"ui": {}, "app": {}}
 templates = Jinja2Templates(directory=FRONTEND_DIR)
 
 # TODO: try to avoid using global var for state store
 global_app_state_store = InMemoryStateStore()
 global_app_state_store.add(TEST_SESSION_UUID)
 
 lock = Lock()
@@ -94,54 +98,50 @@
 # This can be replaced with a consumer that publishes states in a kv-store
 # in a serverless architecture
 
 
 class UIRefresher(Thread):
     def __init__(
         self,
-        api_publish_state_queue,
-        api_response_queue,
+        api_publish_state_queue: Queue,
+        api_response_queue: Queue,
         refresh_interval: float = 0.1,
     ) -> None:
         super().__init__(daemon=True)
         self.api_publish_state_queue = api_publish_state_queue
         self.api_response_queue = api_response_queue
         self._exit_event = Event()
         self.refresh_interval = refresh_interval
 
-    def run(self):
+    def run(self) -> None:
         # TODO: Create multiple threads to handle the background logic
         # TODO: Investigate the use of `parallel=True`
         try:
             while not self._exit_event.is_set():
                 self.run_once()
                 # Note: Sleep to reduce queue calls.
                 sleep(self.refresh_interval)
-        except Exception as e:
-            logger.error(traceback.print_exc())
-            raise e
+        except Exception as ex:
+            traceback.print_exc()
+            raise ex
 
-    def run_once(self):
-        try:
+    def run_once(self) -> None:
+        with contextlib.suppress(queue.Empty):
             global app_status
             state, app_status = self.api_publish_state_queue.get(timeout=0)
             with lock:
                 global_app_state_store.set_app_state(TEST_SESSION_UUID, state)
-        except queue.Empty:
-            pass
 
-        try:
+        with contextlib.suppress(queue.Empty):
             responses = self.api_response_queue.get(timeout=0)
             with lock:
                 # TODO: Abstract the responses store to support horizontal scaling.
                 global responses_store
                 for response in responses:
                     responses_store[response["id"]] = response["response"]
-        except queue.Empty:
-            pass
 
     def join(self, timeout: Optional[float] = None) -> None:
         self._exit_event.set()
         super().join(timeout)
 
 
 class StateUpdate(BaseModel):
@@ -172,15 +172,15 @@
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
 if _is_starsessions_available():
-    fastapi_service.add_middleware(SessionMiddleware, secret_key="secret", autoload=True)
+    fastapi_service.add_middleware(SessionMiddleware, secret_key="secret", autoload=True)  # noqa: S106
 
 
 # General sequence is:
 # * an update is generated in the UI
 # * the value and the location in the state (or the whole state, easier)
 #   is sent to the REST API along with the session UID
 # * the previous state is loaded from the cache, the delta is generated
@@ -192,17 +192,17 @@
 # * the UI is updated with the new value of the state
 # Before the above happens, we need to refactor App so that it doesn't
 # rely on timeouts, but on sequences of updates (and alignments between
 # ranks)
 @fastapi_service.get("/api/v1/state", response_class=JSONResponse)
 async def get_state(
     response: Response,
-    x_lightning_type: Optional[str] = Header(None),
-    x_lightning_session_uuid: Optional[str] = Header(None),
-    x_lightning_session_id: Optional[str] = Header(None),
+    x_lightning_type: Optional[str] = Header(None),  # type: ignore[assignment]
+    x_lightning_session_uuid: Optional[str] = Header(None),  # type: ignore[assignment]
+    x_lightning_session_id: Optional[str] = Header(None),  # type: ignore[assignment]
 ) -> Mapping:
     if x_lightning_session_uuid is None:
         raise Exception("Missing X-Lightning-Session-UUID header")
     if x_lightning_session_id is None:
         raise Exception("Missing X-Lightning-Session-ID header")
 
     if not ENABLE_PULLING_STATE_ENDPOINT:
@@ -212,15 +212,15 @@
     with lock:
         x_lightning_session_uuid = TEST_SESSION_UUID
         state = global_app_state_store.get_app_state(x_lightning_session_uuid)
         global_app_state_store.set_served_state(x_lightning_session_uuid, state)
         return state
 
 
-def _get_component_by_name(component_name: str, state):
+def _get_component_by_name(component_name: str, state: dict) -> Union[LightningFlow, LightningWork]:
     child = state
     for child_name in component_name.split(".")[1:]:
         try:
             child = child["flows"][child_name]
         except KeyError:
             child = child["structures"][child_name]
 
@@ -242,16 +242,16 @@
                 la["content"] = _get_component_by_name(la["content"], state)
         return layout
 
 
 @fastapi_service.get("/api/v1/spec", response_class=JSONResponse)
 async def get_spec(
     response: Response,
-    x_lightning_session_uuid: Optional[str] = Header(None),
-    x_lightning_session_id: Optional[str] = Header(None),
+    x_lightning_session_uuid: Optional[str] = Header(None),  # type: ignore[assignment]
+    x_lightning_session_id: Optional[str] = Header(None),  # type: ignore[assignment]
 ) -> Union[List, Dict]:
     if x_lightning_session_uuid is None:
         raise Exception("Missing X-Lightning-Session-UUID header")
     if x_lightning_session_id is None:
         raise Exception("Missing X-Lightning-Session-ID header")
 
     if not ENABLE_PULLING_STATE_ENDPOINT:
@@ -262,41 +262,43 @@
     return app_spec or []
 
 
 @fastapi_service.post("/api/v1/delta")
 async def post_delta(
     request: Request,
     response: Response,
-    x_lightning_type: Optional[str] = Header(None),
-    x_lightning_session_uuid: Optional[str] = Header(None),
-    x_lightning_session_id: Optional[str] = Header(None),
+    x_lightning_type: Optional[str] = Header(None),  # type: ignore[assignment]
+    x_lightning_session_uuid: Optional[str] = Header(None),  # type: ignore[assignment]
+    x_lightning_session_id: Optional[str] = Header(None),  # type: ignore[assignment]
 ) -> Optional[Dict]:
     """This endpoint is used to make an update to the app state using delta diff, mainly used by streamlit to
     update the state."""
 
     if x_lightning_session_uuid is None:
         raise Exception("Missing X-Lightning-Session-UUID header")
     if x_lightning_session_id is None:
         raise Exception("Missing X-Lightning-Session-ID header")
 
     if not ENABLE_PUSHING_STATE_ENDPOINT:
         response.status_code = status.HTTP_405_METHOD_NOT_ALLOWED
         return {"status": "failure", "reason": "This endpoint is disabled."}
 
     body: Dict = await request.json()
+    assert api_app_delta_queue is not None
     api_app_delta_queue.put(_DeltaRequest(delta=Delta(body["delta"])))
+    return None
 
 
 @fastapi_service.post("/api/v1/state")
 async def post_state(
     request: Request,
     response: Response,
-    x_lightning_type: Optional[str] = Header(None),
-    x_lightning_session_uuid: Optional[str] = Header(None),
-    x_lightning_session_id: Optional[str] = Header(None),
+    x_lightning_type: Optional[str] = Header(None),  # type: ignore[assignment]
+    x_lightning_session_uuid: Optional[str] = Header(None),  # type: ignore[assignment]
+    x_lightning_session_id: Optional[str] = Header(None),  # type: ignore[assignment]
 ) -> Optional[Dict]:
     if x_lightning_session_uuid is None:
         raise Exception("Missing X-Lightning-Session-UUID header")
     if x_lightning_session_id is None:
         raise Exception("Missing X-Lightning-Session-ID header")
     # This needs to be sent so that it can be set as last state
     # in app (see sequencing above)
@@ -316,19 +318,21 @@
         state = deepcopy(last_state)
         state["app_state"]["stage"] = body["stage"]
         deep_diff = DeepDiff(last_state, state, verbose_level=2)
     else:
         state = body["state"]
         last_state = global_app_state_store.get_served_state(x_lightning_session_uuid)
         deep_diff = DeepDiff(last_state, state, verbose_level=2)
+    assert api_app_delta_queue is not None
     api_app_delta_queue.put(_DeltaRequest(delta=Delta(deep_diff)))
+    return None
 
 
 @fastapi_service.put("/api/v1/upload_file/{filename}")
-async def upload_file(response: Response, filename: str, uploaded_file: UploadFile = File(...)):
+async def upload_file(response: Response, filename: str, uploaded_file: UploadFile = File(...)) -> Union[str, dict]:
     if not ENABLE_UPLOAD_ENDPOINT:
         response.status_code = status.HTTP_405_METHOD_NOT_ALLOWED
         return {"status": "failure", "reason": "This endpoint is disabled."}
 
     with TemporaryDirectory() as tmp:
         drive = Drive(
             "lit://uploaded_files",
@@ -342,15 +346,15 @@
             done = False
             while not done:
                 # Note: The 8192 number doesn't have a strong reason.
                 content = await uploaded_file.read(8192)
                 f.write(content)
                 done = content == b""
 
-        with _context(ComponentContext.WORK):
+        with _context(str(ComponentContext.WORK)):
             drive.put(filename)
     return f"Successfully uploaded '{filename}' to the Drive"
 
 
 @fastapi_service.get("/api/v1/status", response_model=AppStatus)
 async def get_status() -> AppStatus:
     """Get the current status of the app and works."""
@@ -366,15 +370,15 @@
 async def get_annotations() -> Union[List, Dict]:
     """Get the annotations associated with this app."""
     global app_annotations
     return app_annotations or []
 
 
 @fastapi_service.get("/healthz", status_code=200)
-async def healthz(response: Response):
+async def healthz(response: Response) -> dict:
     """Health check endpoint used in the cloud FastAPI servers to check the status periodically."""
     # check the queue status only if running in cloud
     if is_running_in_cloud():
         queue_obj = QueuingSystem(get_cloud_queue_type()).get_queue(queue_name="healthz")
         # this is only being implemented on Redis Queue. For HTTP Queue, it doesn't make sense to have every single
         # app checking the status of the Queue server
         if not queue_obj.is_running:
@@ -388,15 +392,15 @@
         return {"status": "failure", "reason": f"State is empty {state}"}
     return {"status": "ok"}
 
 
 # Creates session websocket connection to notify client about any state changes
 # The websocket instance needs to be stored based on session id so it is accessible in the api layer
 @fastapi_service.websocket("/api/v1/ws")
-async def websocket_endpoint(websocket: WebSocket):
+async def websocket_endpoint(websocket: WebSocket) -> None:
     await websocket.accept()
     if not ENABLE_STATE_WEBSOCKET:
         await websocket.close()
         return
     try:
         counter = global_app_state_store.counter
         while True:
@@ -406,74 +410,74 @@
                 logger.debug("Updated websocket.")
             await asyncio.sleep(0.01)
     except ConnectionClosed:
         logger.debug("Websocket connection closed")
     await websocket.close()
 
 
-async def api_catch_all(request: Request, full_path: str):
+async def api_catch_all(request: Request, full_path: str) -> None:
     raise HTTPException(status_code=404, detail="Not found")
 
 
 # Serve frontend from a static directory using FastAPI
 fastapi_service.mount("/static", StaticFiles(directory=frontend_static_dir, check_dir=False), name="static")
 
 
-async def frontend_route(request: Request, full_path: str):
+async def frontend_route(request: Request, full_path: str):  # type: ignore[no-untyped-def]
     if "pytest" in sys.modules:
         return ""
     return templates.TemplateResponse("index.html", {"request": request})
 
 
-def register_global_routes():
+def register_global_routes() -> None:
     # Catch-all for nonexistent API routes (since we define a catch-all for client-side routing)
     fastapi_service.get("/api{full_path:path}", response_class=JSONResponse)(api_catch_all)
     fastapi_service.get("/{full_path:path}", response_class=HTMLResponse)(frontend_route)
 
 
 class LightningUvicornServer(uvicorn.Server):
-    has_started_queue = None
+    has_started_queue: Optional[Queue] = None
 
-    def run(self, sockets=None):
+    def run(self, sockets: Optional[List[socket.socket]] = None) -> None:
         self.config.setup_event_loop()
         loop = asyncio.get_event_loop()
         asyncio.ensure_future(self.serve(sockets=sockets))
         if self.has_started_queue:
             asyncio.ensure_future(self.check_is_started(self.has_started_queue))
         loop.run_forever()
 
-    async def check_is_started(self, queue):
+    async def check_is_started(self, queue: Queue) -> None:
         while not self.started:
             await asyncio.sleep(0.1)
         queue.put("SERVER_HAS_STARTED")
 
 
 def start_server(
-    api_publish_state_queue,
-    api_delta_queue,
-    api_response_queue,
+    api_publish_state_queue: Queue,
+    api_delta_queue: Queue,
+    api_response_queue: Queue,
     has_started_queue: Optional[Queue] = None,
-    host="127.0.0.1",
-    port=8000,
+    host: str = "127.0.0.1",
+    port: int = 8000,
     root_path: str = "",
     uvicorn_run: bool = True,
     spec: Optional[List] = None,
     apis: Optional[List[_HttpMethod]] = None,
     app_state_store: Optional[StateStore] = None,
-):
+) -> UIRefresher:
     global api_app_delta_queue
     global global_app_state_store
     global app_spec
     global app_annotations
 
     app_spec = spec
     api_app_delta_queue = api_delta_queue
 
     if app_state_store is not None:
-        global_app_state_store = app_state_store
+        global_app_state_store = app_state_store  # type: ignore[assignment]
 
     global_app_state_store.add(TEST_SESSION_UUID)
 
     # Load annotations
     annotations_path = Path("lightning-annotations.json").resolve()
     if annotations_path.exists():
         with open(annotations_path) as f:
@@ -481,15 +485,15 @@
 
     refresher = UIRefresher(api_publish_state_queue, api_response_queue)
     refresher.setDaemon(True)
     refresher.start()
 
     if uvicorn_run:
         host = host.split("//")[-1] if "//" in host else host
-        if host == "0.0.0.0":
+        if host == "0.0.0.0":  # noqa: S104
             logger.info("Your app has started.")
         else:
             logger.info(f"Your app has started. View it in your browser: http://{host}:{port}/view")
         if has_started_queue:
             LightningUvicornServer.has_started_queue = has_started_queue
             # uvicorn is doing some uglyness by replacing uvicorn.main by click command.
             sys.modules["uvicorn.main"].Server = LightningUvicornServer
```

### Comparing `lightning-app-2.0.2/src/lightning_app/core/app.py` & `lightning-app-2.0.3/src/lightning_app/core/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,31 +337,30 @@
         # The while loop can exit sooner if both queues are empty.
 
         deltas = []
         api_or_command_request_deltas = []
         t0 = time()
 
         while (time() - t0) < self.state_accumulate_wait:
-
             # TODO: Fetch all available deltas at once to reduce queue calls.
             delta: Optional[
                 Union[_DeltaRequest, _APIRequest, _CommandRequest, ComponentDelta]
             ] = self.get_state_changed_from_queue(
                 self.delta_queue  # type: ignore[assignment,arg-type]
             )
             if delta:
                 if isinstance(delta, _DeltaRequest):
                     deltas.append(delta.delta)
                 elif isinstance(delta, ComponentDelta):
                     logger.debug(f"Received from {delta.id} : {delta.delta.to_dict()}")
                     work = None
                     try:
                         work = self.get_component_by_name(delta.id)
-                    except (KeyError, AttributeError) as e:
-                        logger.error(f"The component {delta.id} couldn't be accessed. Exception: {e}")
+                    except (KeyError, AttributeError) as ex:
+                        logger.error(f"The component {delta.id} couldn't be accessed. Exception: {ex}")
 
                     if work:
                         delta = _delta_to_app_state_delta(
                             self.root, work, deepcopy(delta.delta)  # type: ignore[arg-type]
                         )
                         deltas.append(delta)
                 else:
@@ -418,20 +417,21 @@
         # 2: Collect the state
         state = self.state
 
         # 3: Apply the state delta
         for delta in deltas:
             try:
                 state += delta
-            except Exception as e:
-                raise Exception(f"Current State {state}, {delta.to_dict()}") from e
+            except Exception as ex:
+                raise Exception(f"Current State {state}, {delta.to_dict()}") from ex
 
         # new_state = self.populate_changes(self.last_state, state)
         self.set_state(state)
         self._has_updated = True
+        return None
 
     def run_once(self) -> bool:
         """Method used to collect changes and run the root Flow once."""
         done = False
         self._last_run_time = 0.0
 
         if self.backend is not None:
@@ -447,15 +447,15 @@
 
         if self.stage == AppStage.BLOCKING:
             return done
 
         if self.stage in (AppStage.STOPPING, AppStage.FAILED):
             return True
 
-        elif self.stage == AppStage.RESTARTING:
+        if self.stage == AppStage.RESTARTING:
             return self._apply_restarting()
 
         t0 = time()
 
         try:
             self.check_error_queue()
             # Execute the flow only if:
@@ -527,15 +527,14 @@
             self._has_updated = False
 
         self._on_run_end()
 
         return True
 
     def _update_layout(self) -> None:
-
         if self.backend:
             self.backend.resolve_url(self, base_url=None)
 
         for component in breadth_first(self.root, types=(lightning_app.LightningFlow,)):  # type: ignore[arg-type]
             layout = _collect_layout(self, component)
             component._layout = layout
 
@@ -580,20 +579,19 @@
         work_finished_status = {work.name: self._has_work_finished(work) for work in self.works}
         assert len(work_finished_status) == len(self.works)
         return work_finished_status
 
     def _should_snapshot(self) -> bool:
         if len(self.works) == 0:
             return True
-        elif self._has_updated:
+        if self._has_updated:
             work_finished_status = self._collect_work_finish_status()
             if work_finished_status:
                 return all(work_finished_status.values())
-            else:
-                return True
+            return True
         return False
 
     def state_dict(self) -> Dict:
         return self.state
 
     def load_state_dict(self, state: Dict) -> None:
         self.set_state(state)
@@ -612,37 +610,34 @@
         if version is None:
             # take the latest checkpoint.
             version = sorted(int(c.split("_")[1]) for c in checkpoints)[-1]
 
         available_checkpoints = [c for c in checkpoints if c.startswith(f"v_{version}_")]
         if not available_checkpoints:
             raise FileNotFoundError(f"The version `{version}` wasn't found in {checkpoints}.")
-        elif len(available_checkpoints) > 1:
+        if len(available_checkpoints) > 1:
             raise Exception(f"Found 2 checkpoints `{available_checkpoints}`with the same version.")
         checkpoint_path = os.path.join(checkpoints_dir, available_checkpoints[0])
-        state = pickle.load(open(checkpoint_path, "rb"))
+        with open(checkpoint_path, "rb") as fo:
+            state = pickle.load(fo)
         self.load_state_dict(state)
 
     def _dump_checkpoint(self) -> Optional[str]:
         checkpoints_dir = self.checkpoint_dir
         # TODO: Add supports to remotely saving checkpoints.
         if checkpoints_dir.startswith("s3:"):
             return None
         os.makedirs(checkpoints_dir, exist_ok=True)
 
         # Get all current version within the provided folder and sort them
         checkpoint_versions = sorted(
             int(f.split("_")[1]) for f in os.listdir(checkpoints_dir) if f.startswith("v_") and f.endswith(".json")
         )
 
-        if checkpoint_versions:
-            previous_version = checkpoint_versions[-1]
-        else:
-            # initialization
-            previous_version = -1
+        previous_version = checkpoint_versions[-1] if checkpoint_versions else -1
 
         checkpoint_path = os.path.join(checkpoints_dir, f"v_{previous_version + 1}_{time()}.json")
 
         with open(checkpoint_path, "wb") as f:
             pickle.dump(self.state_dict(), f)
         return checkpoint_path
```

### Comparing `lightning-app-2.0.2/src/lightning_app/core/constants.py` & `lightning-app-2.0.3/src/lightning_app/core/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 ENABLE_PUSHING_STATE_ENDPOINT = ENABLE_PULLING_STATE_ENDPOINT and bool(
     int(os.getenv("ENABLE_PUSHING_STATE_ENDPOINT", "1"))
 )
 ENABLE_STATE_WEBSOCKET = bool(int(os.getenv("ENABLE_STATE_WEBSOCKET", "1")))
 ENABLE_UPLOAD_ENDPOINT = bool(int(os.getenv("ENABLE_UPLOAD_ENDPOINT", "1")))
 
 # directory where system customization sync files stored
-SYS_CUSTOMIZATIONS_SYNC_ROOT = "/tmp/sys-customizations-sync"
+SYS_CUSTOMIZATIONS_SYNC_ROOT = "/tmp/sys-customizations-sync"  # noqa: S108 # todo
 # directory where system customization sync files will be copied to be packed into app tarball
 SYS_CUSTOMIZATIONS_SYNC_PATH = ".sys-customizations-sync"
 
 
 def enable_multiple_works_in_default_container() -> bool:
     return bool(int(os.getenv("ENABLE_MULTIPLE_WORKS_IN_DEFAULT_CONTAINER", "0")))
```

### Comparing `lightning-app-2.0.2/src/lightning_app/core/flow.py` & `lightning-app-2.0.3/src/lightning_app/core/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from lightning_app.utilities.packaging.cloud_compute import _maybe_create_cloud_compute, CloudCompute
 
 if TYPE_CHECKING:
     from lightning_app.runners.backends.backend import Backend
 
 
 class LightningFlow:
-
     _INTERNAL_STATE_VARS = {
         # Internal protected variables that are still part of the state (even though they are prefixed with "_")
         "_paths",
         "_layout",
     }
 
     def __init__(self) -> None:
@@ -106,15 +105,14 @@
             ...         self.counter += 1
             ...
             >>> flow = RootFlow()
             >>> flow.run()
             >>> assert flow.counter == 1
             >>> assert flow.state["vars"]["counter"] == 1
         """
-
         self._state: set = set()
         self._name: str = ""
         self._flows: set = set()
         self._works: set = set()
         self._structures: set = set()
         self._calls: dict = {}
         self._changes: dict = {}
@@ -150,15 +148,14 @@
         ):
             raise AttributeError(f"Cannot set attributes that were not defined in __init__: {name}")
 
         if isinstance(value, str) and value.startswith("lit://"):
             value = Path(value)
 
         if self._is_state_attribute(name):
-
             if hasattr(self, name):
                 if name in self._flows and value != getattr(self, name):
                     raise AttributeError(f"Cannot set attributes as the flow can't be changed once defined: {name}")
 
                 if name in self._works and value != getattr(self, name):
                     raise AttributeError(f"Cannot set attributes as the work can't be changed once defined: {name}")
 
@@ -236,14 +233,15 @@
                     f" (str, int, float, bool, tuple, list, dict etc.) to be part of {self} state. "
                     f"Found the attribute {name} with {value} instead. \n"
                     "HINT: Private attributes defined as follows `self._x = y` won't be shared between components "
                     "and therefore don't need to be JSON-serializable."
                 )
 
         super().__setattr__(name, value)
+        return None
 
     @staticmethod
     def _attach_backend(flow: "LightningFlow", backend: "Backend") -> None:
         """Attach the backend to all flows and its children."""
         flow._backend = backend
 
         for name in flow._structures:
@@ -529,16 +527,16 @@
             }
 
             self._calls["scheduling"][call_hash] = schedule_metadata
             app = _LightningAppRef().get_current()
             if app:
                 app._register_schedule(call_hash, schedule_metadata)
             return True
-        else:
-            return self._calls["scheduling"][call_hash]["running"]
+
+        return self._calls["scheduling"][call_hash]["running"]
 
     def _enable_schedule(self, call_hash: str) -> None:
         self._calls["scheduling"][call_hash]["running"] = True
 
     def _disable_running_schedules(self) -> None:
         if "scheduling" not in self._calls:
             return
```

### Comparing `lightning-app-2.0.2/src/lightning_app/core/queues.py` & `lightning-app-2.0.3/src/lightning_app/core/queues.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,18 +70,17 @@
     MULTIPROCESS = "multiprocess"
     REDIS = "redis"
     HTTP = "http"
 
     def get_queue(self, queue_name: str) -> "BaseQueue":
         if self == QueuingSystem.MULTIPROCESS:
             return MultiProcessQueue(queue_name, default_timeout=STATE_UPDATE_TIMEOUT)
-        elif self == QueuingSystem.REDIS:
+        if self == QueuingSystem.REDIS:
             return RedisQueue(queue_name, default_timeout=REDIS_QUEUES_READ_DEFAULT_TIMEOUT)
-        else:
-            return HTTPQueue(queue_name, default_timeout=STATE_UPDATE_TIMEOUT)
+        return HTTPQueue(queue_name, default_timeout=STATE_UPDATE_TIMEOUT)
 
     def get_api_response_queue(self, queue_id: Optional[str] = None) -> "BaseQueue":
         queue_name = f"{queue_id}_{API_RESPONSE_QUEUE_CONSTANT}" if queue_id else API_RESPONSE_QUEUE_CONSTANT
         return self.get_queue(queue_name)
 
     def get_readiness_queue(self, queue_id: Optional[str] = None) -> "BaseQueue":
         queue_name = f"{queue_id}_{READINESS_QUEUE_CONSTANT}" if queue_id else READINESS_QUEUE_CONSTANT
@@ -283,15 +282,14 @@
 
         Parameters
         ----------
         timeout:
             Read timeout in seconds, in case of input timeout is 0, the `self.default_timeout` is used.
             A timeout of None can be used to block indefinitely.
         """
-
         if timeout is None:
             # this means it's blocking in redis
             timeout = 0
         elif timeout == 0:
             timeout = self.default_timeout
 
         try:
@@ -416,15 +414,15 @@
                 # Note: In theory, there isn't a need for a sleep as the queue shouldn't
                 # block the flow if the queue is empty.
                 # However, as the Http Server can saturate,
                 # let's add a sleep here if a higher timeout is provided
                 # than the default timeout
                 if timeout > self.default_timeout:
                     time.sleep(0.05)
-                pass
+        return None
 
     def _get(self) -> Any:
         try:
             resp = self.client.post(f"v1/{self.app_id}/{self._name_suffix}", query_params={"action": "pop"})
             if resp.status_code == 204:
                 raise queue.Empty
             return pickle.loads(resp.content)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/core/work.py` & `lightning-app-2.0.3/src/lightning_app/core/work.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         # Internal protected variables that are still part of the state (even though they are prefixed with "_")
         "_paths",
         "_host",
         "_port",
         "_url",
         "_restarting",
         "_internal_ip",
+        "_public_ip",
     )
 
     _run_executor_cls: Type[WorkRunExecutor] = WorkRunExecutor
     # TODO: Move to spawn for all Operating System.
     _start_method = "spawn" if sys.platform in ("darwin", "win32") else "fork"
 
     def __init__(
@@ -134,24 +135,26 @@
         self._cache_calls = run_once if run_once is not None else cache_calls
         self._state = {
             "_host",
             "_port",
             "_url",
             "_future_url",
             "_internal_ip",
+            "_public_ip",
             "_restarting",
             "_cloud_compute",
             "_display_name",
         }
         self._parallel: bool = parallel
         self._host: str = host
         self._port: Optional[int] = port
         self._url: str = ""
         self._future_url: str = ""  # The cache URL is meant to defer resolving the url values.
         self._internal_ip: str = ""
+        self._public_ip: str = ""
         # setattr_replacement is used by the multiprocessing runtime to send the latest changes to the main coordinator
         self._setattr_replacement: Optional[Callable[[str, Any], None]] = None
         self._name: str = ""
         self._display_name: str = ""
         # The ``self._calls`` is used to track whether the run
         # method with a given set of input arguments has already been called.
         # Example of its usage:
@@ -208,14 +211,23 @@
         """The internal ip address of this LightningWork, reachable by other Work locally and in the cloud.
 
         By default, this attribute returns the empty string and the ip address will only be returned once the work runs.
         Locally, the address is 127.0.0.1 and in the cloud it will be determined by the cluster.
         """
         return self._internal_ip
 
+    @property
+    def public_ip(self) -> str:
+        """The public ip address of this LightningWork, reachable from the internet.
+
+        By default, this attribute returns the empty string and the ip address will only be returned once the work runs.
+        Locally, this address is undefined (empty string) and in the cloud it will be determined by the cluster.
+        """
+        return self._public_ip
+
     def _on_init_end(self) -> None:
         self._local_build_config.on_work_init(self)
         self._cloud_build_config.on_work_init(self, self._cloud_compute)
 
     @staticmethod
     def _is_state_attribute(name: str) -> bool:
         """Every public attribute is part of the state by default and all protected (prefixed by '_') or private
@@ -379,15 +391,15 @@
             return status.count
         return 0
 
     @property
     def num_successes(self) -> int:
         """Returns the number of successful runs."""
         # FIXME: Resolve this within  single process runtime.
-        run_keys = [key for key in self._calls.keys() if key.startswith("run:")]
+        run_keys = [key for key in self._calls if key.startswith("run:")]
         if not run_keys:
             return 0
 
         has_succeeded_counter = 0
         for run_key in run_keys:
             c = len([s for s in self._calls[run_key]["statuses"] if s["stage"] == WorkStageStatus.SUCCEEDED])
             has_succeeded_counter += c
@@ -434,15 +446,15 @@
         if self._is_state_attribute(name):
             if isinstance(value, (LightningFlow, LightningWork)):
                 raise LightningWorkException(
                     "A ``LightningWork`` isn't allowed to take any children "
                     f"such as ``LightningWork`` or ``LightningFlow``. Found {value}."
                 )
 
-            elif isinstance(value, Path):
+            if isinstance(value, Path):
                 value._attach_work(work=self)
                 value._attach_queues(self._request_queue, self._response_queue)  # type: ignore[arg-type]
                 value._name = name
                 # In the init context, the full name of the Flow and Work is not known, i.e., we can't serialize
                 # the path without losing the information of origin and consumer. Hence, we delay the serialization
                 # of the path object until the app is instantiated.
                 if not is_init_context:
@@ -479,26 +491,25 @@
                 )
 
         super().__setattr__(name, value)
 
     def __getattribute__(self, name: str) -> Any:
         try:
             attr = object.__getattribute__(self, name)
-        except AttributeError as e:
-            if str(e).endswith("'_state'"):
+        except AttributeError as ex:
+            if str(ex).endswith("'_state'"):
                 raise AttributeError(f"Did you forget to call super().__init__() in {self}")
-            raise e
+            raise ex
 
         if isinstance(attr, ProxyWorkRun):
             return attr
 
-        if callable(attr) and getattr(attr, "__name__", "") == "run":
+        if callable(attr) and getattr(attr, "__name__", "") == "run" and getattr(self, "_cache_calls", False):
             # disable while building the class.
-            if getattr(self, "_cache_calls", False):
-                return self._wrap_run_for_caching(attr)
+            return self._wrap_run_for_caching(attr)
         return attr
 
     def __getattr__(self, item: str) -> Any:
         if item in self.__dict__.get("_paths", {}) and not _is_init_context(self):
             path = Path.from_dict(self._paths[item])
             path._attach_work(work=self)
             path._attach_queues(self._request_queue, self._response_queue)  # type: ignore[arg-type]
```

### Comparing `lightning-app-2.0.2/src/lightning_app/frontend/frontend.py` & `lightning-app-2.0.3/src/lightning_app/frontend/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/frontend/just_py/just_py.py` & `lightning-app-2.0.3/src/lightning_app/frontend/just_py/just_py.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/frontend/just_py/just_py_base.py` & `lightning-app-2.0.3/src/lightning_app/frontend/just_py/just_py_base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     render_fn_name = os.environ["LIGHTNING_RENDER_FUNCTION"]
     render_fn_module_file = os.environ["LIGHTNING_RENDER_MODULE_FILE"]
     module = pydoc.importfile(render_fn_module_file)
     return getattr(module, render_fn_name)
 
 
 def _main() -> None:
+    """Run the render_fn with the current flow_state."""
     import justpy as jp
 
-    """Run the render_fn with the current flow_state."""
     # Fetch the information of which flow attaches to this justpy instance
     flow_name = os.environ["LIGHTNING_FLOW_NAME"]
 
     # Call the provided render function.
     # Pass it the state, scoped to the current flow.
     render_fn = _get_render_fn_from_environment()
     host = os.environ["LIGHTNING_HOST"]
```

### Comparing `lightning-app-2.0.2/src/lightning_app/frontend/panel/app_state_comm.py` & `lightning-app-2.0.3/src/lightning_app/frontend/panel/app_state_comm.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """The watch_app_state function enables us to trigger a callback function when ever the app state changes."""
 # Todo: Refactor with Streamlit
 # Note: It would be nice one day to just watch changes within the Flow scope instead of whole app
 from __future__ import annotations
 
 import asyncio
 import os
```

### Comparing `lightning-app-2.0.2/src/lightning_app/frontend/panel/app_state_watcher.py` & `lightning-app-2.0.3/src/lightning_app/frontend/panel/app_state_watcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """The ``AppStateWatcher`` enables a Frontend to:
 
 - subscribe to App state changes
 - to access and change the App state.
 
 This is particularly useful for the ``PanelFrontend`` but can be used by other frontends too.
 """
```

### Comparing `lightning-app-2.0.2/src/lightning_app/frontend/panel/panel_frontend.py` & `lightning-app-2.0.3/src/lightning_app/frontend/panel/panel_frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """The PanelFrontend wraps your Panel code in your LightningFlow."""
 from __future__ import annotations
 
 import inspect
 import os
 import pathlib
 import subprocess
```

### Comparing `lightning-app-2.0.2/src/lightning_app/frontend/panel/panel_serve_render_fn.py` & `lightning-app-2.0.3/src/lightning_app/frontend/panel/panel_serve_render_fn.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """This file gets run by Python to launch a Panel Server with Lightning.
 
 We will call the ``render_fn`` that the user provided to the PanelFrontend.
 
 It requires the following environment variables to be set
```

### Comparing `lightning-app-2.0.2/src/lightning_app/frontend/stream_lit.py` & `lightning-app-2.0.3/src/lightning_app/frontend/stream_lit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/frontend/streamlit_base.py` & `lightning-app-2.0.3/src/lightning_app/frontend/streamlit_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """This file gets run by streamlit, which we launch within Lightning.
 
 From here, we will call the render function that the user provided in ``configure_layout``.
 """
 import os
 import pydoc
 from typing import Callable
```

### Comparing `lightning-app-2.0.2/src/lightning_app/frontend/utils.py` & `lightning-app-2.0.3/src/lightning_app/frontend/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """Utility functions for lightning Frontends."""
 from __future__ import annotations
 
 import inspect
 import os
 from typing import Callable
 
@@ -37,16 +36,15 @@
     """Returns an AppState scoped to the current Flow.
 
     Returns:
         AppState: An AppState scoped to the current Flow.
     """
     app_state = AppState()
     app_state._request_state()  # pylint: disable=protected-access
-    flow_state = _reduce_to_flow_scope(app_state, flow)
-    return flow_state
+    return _reduce_to_flow_scope(app_state, flow)
 
 
 def _get_frontend_environment(flow: str, render_fn_or_file: Callable | str, port: int, host: str) -> os._Environ:
     """Returns an _Environ with the environment variables for serving a Frontend app set.
 
     Args:
         flow: The name of the flow, for example root.lit_frontend
```

### Comparing `lightning-app-2.0.2/src/lightning_app/frontend/web.py` & `lightning-app-2.0.3/src/lightning_app/frontend/web.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/perf/pdb.py` & `lightning-app-2.0.3/src/lightning_app/perf/pdb.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/plugin/actions.py` & `lightning-app-2.0.3/src/lightning_app/plugin/actions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/plugin/plugin.py` & `lightning-app-2.0.3/src/lightning_app/plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,36 +124,36 @@
             response = requests.get(source_code_url)
 
             # TODO: Backoff retry a few times in case the URL is flaky
             response.raise_for_status()
 
             with open(download_path, "wb") as f:
                 f.write(response.content)
-        except Exception as e:
+        except Exception as ex:
             raise HTTPException(
                 status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
-                detail=f"Error downloading plugin source: {str(e)}.",
+                detail=f"Error downloading plugin source: {str(ex)}.",
             )
 
         # Extract
         try:
             with tarfile.open(download_path, "r:gz") as tf:
                 tf.extractall(source_path)
-        except Exception as e:
+        except Exception as ex:
             raise HTTPException(
                 status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
-                detail=f"Error extracting plugin source: {str(e)}.",
+                detail=f"Error extracting plugin source: {str(ex)}.",
             )
 
         # Import the plugin
         try:
             plugin = _load_plugin_from_file(os.path.join(source_path, run.plugin_entrypoint))
-        except Exception as e:
+        except Exception as ex:
             raise HTTPException(
-                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=f"Error loading plugin: {str(e)}."
+                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=f"Error loading plugin: {str(ex)}."
             )
 
         # Ensure that apps are dispatched from the temp directory
         cwd = os.getcwd()
         os.chdir(source_path)
 
         # Setup and run the plugin
@@ -161,17 +161,17 @@
             plugin._setup(
                 project_id=run.project_id,
                 cloudspace_id=run.cloudspace_id,
                 cluster_id=run.cluster_id,
             )
             actions = plugin.run(**run.plugin_arguments) or []
             return {"actions": [action.to_spec().to_dict() for action in actions]}
-        except Exception as e:
+        except Exception as ex:
             raise HTTPException(
-                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=f"Error running plugin: {str(e)}."
+                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=f"Error running plugin: {str(ex)}."
             )
         finally:
             os.chdir(cwd)
 
 
 async def _healthz() -> Dict[str, str]:
     """Health check endpoint."""
```

### Comparing `lightning-app-2.0.2/src/lightning_app/runners/backends/__init__.py` & `lightning-app-2.0.3/src/lightning_app/runners/backends/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,13 +13,12 @@
     CLOUD = "cloud"
 
     def get_backend(self, entrypoint_file: str) -> "Backend":
         if self == BackendType.MULTIPROCESSING:
             if APP_SERVER_IN_CLOUD:
                 return CloudMultiProcessingBackend(entrypoint_file)
             return MultiProcessingBackend(entrypoint_file)
-        elif self == BackendType.DOCKER:
+        if self == BackendType.DOCKER:
             return DockerBackend(entrypoint_file)
-        elif self == BackendType.CLOUD:
+        if self == BackendType.CLOUD:
             return CloudBackend(entrypoint_file)
-        else:
-            raise ValueError("Unknown client type")
+        raise ValueError("Unknown client type")
```

### Comparing `lightning-app-2.0.2/src/lightning_app/runners/backends/backend.py` & `lightning-app-2.0.3/src/lightning_app/runners/backends/backend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/runners/backends/cloud.py` & `lightning-app-2.0.3/src/lightning_app/runners/backends/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/runners/backends/docker.py` & `lightning-app-2.0.3/src/lightning_app/runners/backends/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/runners/backends/mp_process.py` & `lightning-app-2.0.3/src/lightning_app/runners/backends/mp_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     def __init__(self, entrypoint_file: str):
         super().__init__(entrypoint_file=entrypoint_file, queues=QueuingSystem.MULTIPROCESS, queue_id="0")
 
     def create_work(self, app, work) -> None:
         if constants.LIGHTNING_CLOUDSPACE_HOST is not None:
             # Override the port if set by the user
             work._port = find_free_network_port()
-            work._host = "0.0.0.0"
+            work._host = "0.0.0.0"  # noqa: S104
             work._future_url = f"https://{work.port}-{constants.LIGHTNING_CLOUDSPACE_HOST}"
 
         app.processes[work.name] = MultiProcessWorkManager(app, work)
         app.processes[work.name].start()
         self.resolve_url(app)
         app._update_layout()
 
@@ -117,15 +117,15 @@
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
 
         # Note: Track the open ports to close them on termination.
         self.ports = []
 
     def create_work(self, app, work) -> None:
-        work._host = "0.0.0.0"
+        work._host = "0.0.0.0"  # noqa: S104
         nc = enable_port()
         self.ports.append(nc.port)
         work._port = nc.port
         work._future_url = f"https://{nc.host}"
         return super().create_work(app, work)
 
     def stop_work(self, app, work: "lightning_app.LightningWork") -> None:
```

### Comparing `lightning-app-2.0.2/src/lightning_app/runners/cloud.py` & `lightning-app-2.0.3/src/lightning_app/runners/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,28 +99,27 @@
 from lightning_app.utilities.secrets import _names_to_ids
 
 logger = Logger(__name__)
 
 
 def _to_clean_dict(swagger_object, map_attributes):
     """Returns the swagger object properties as a dict with correct object names."""
-
     if hasattr(swagger_object, "to_dict"):
         attribute_map = swagger_object.attribute_map
         result = {}
-        for key in attribute_map.keys():
+        for key in attribute_map:
             value = getattr(swagger_object, key)
             value = _to_clean_dict(value, map_attributes)
             if value is not None and value != {}:
                 key = attribute_map[key] if map_attributes else key
                 result[key] = value
         return result
-    elif isinstance(swagger_object, list):
+    if isinstance(swagger_object, list):
         return [_to_clean_dict(x, map_attributes) for x in swagger_object]
-    elif isinstance(swagger_object, dict):
+    if isinstance(swagger_object, dict):
         return {key: _to_clean_dict(value, map_attributes) for key, value in swagger_object.items()}
     return swagger_object
 
 
 @dataclass
 class CloudRuntime(Runtime):
     backend: Union[str, CloudBackend] = "cloud"
@@ -183,16 +182,16 @@
 
             if getattr(run, "cluster_id", None):
                 print(f"Running on {run.cluster_id}")
 
             if "PYTEST_CURRENT_TEST" not in os.environ:
                 click.launch(self._get_cloudspace_url(project, cloudspace_name, "code", needs_credits))
 
-        except ApiException as e:
-            logger.error(e.body)
+        except ApiException as ex:
+            logger.error(ex.body)
             sys.exit(1)
 
     def cloudspace_dispatch(
         self,
         project_id: str,
         cloudspace_id: str,
         name: str,
@@ -381,32 +380,31 @@
                 click.launch(
                     self._get_app_url(project, run_instance, "logs" if run.is_headless else "web-ui", needs_credits)
                 )
 
             if bool(int(os.getenv("LIGHTING_TESTING", "0"))):
                 print(f"APP_LOGS_URL: {self._get_app_url(project, run_instance, 'logs')}")
 
-        except ApiException as e:
-            logger.error(e.body)
+        except ApiException as ex:
+            logger.error(ex.body)
             sys.exit(1)
         finally:
             if cleanup_handle:
                 cleanup_handle()
 
     @classmethod
     def load_app_from_file(cls, filepath: str, env_vars: Dict[str, str] = {}) -> "LightningApp":
         """Load a LightningApp from a file, mocking the imports."""
-
         # Pretend we are running in the cloud when loading the app locally
         os.environ["LAI_RUNNING_IN_CLOUD"] = "1"
 
         try:
             app = load_app_from_file(filepath, raise_exception=True, mock_imports=True, env_vars=env_vars)
-        except FileNotFoundError as e:
-            raise e
+        except FileNotFoundError as ex:
+            raise ex
         except Exception:
             from lightning_app.testing.helpers import EmptyFlow
 
             # Create a generic app.
             logger.info("Could not load the app locally. Starting the app directly on the cloud.")
             app = LightningApp(EmptyFlow())
         finally:
@@ -491,14 +489,17 @@
             if cloudspace.name == cloudspace_name or (re.fullmatch(pattern, cloudspace.name) is not None)
         ]
 
     def _resolve_cluster_id(
         self, cluster_id: Optional[str], project_id: str, existing_cloudspaces: List[V1CloudSpace]
     ) -> Optional[str]:
         """If cloudspaces exist and cluster is None, mimic cluster selection logic to choose a default."""
+        if cluster_id is None:
+            cluster_id = os.getenv("CLUSTER_ID", None)
+
         if cluster_id is None and len(existing_cloudspaces) > 0:
             # Determine the cluster ID
             cluster_id = _get_default_cluster(self.backend.client, project_id)
         return cluster_id
 
     def _resolve_existing_run_instance(
         self, cluster_id: Optional[str], project_id: str, existing_cloudspaces: List[V1CloudSpace]
@@ -534,43 +535,41 @@
         existing_cloudspaces: List[V1CloudSpace],
     ) -> str:
         """If there are existing cloudspaces but not on the cluster - choose a randomised name."""
         if len(existing_cloudspaces) > 0 and existing_cloudspace is None:
             name_exists = True
             while name_exists:
                 random_name = cloudspace_name + "-" + "".join(random.sample(string.ascii_letters, 4))
-                name_exists = any([app.name == random_name for app in existing_cloudspaces])
+                name_exists = any(app.name == random_name for app in existing_cloudspaces)
 
             cloudspace_name = random_name
         return cloudspace_name
 
     def _resolve_run_name(
         self,
         name: str,
         existing_instances: List[Externalv1LightningappInstance],
     ) -> str:
         """If there are existing instances with the same name - choose a randomised name."""
         if len(existing_instances) > 0:
             name_exists = True
             while name_exists:
                 random_name = name + "-" + "".join(random.sample(string.ascii_letters, 4))
-                name_exists = any([app.name == random_name for app in existing_instances])
+                name_exists = any(app.name == random_name for app in existing_instances)
 
             name = random_name
         return name
 
     def _resolve_cloudspace(self, project_id: str, cloudspace_id: str) -> Optional[V1CloudSpace]:
         """Returns a cloudspace by project_id and cloudspace_id, if exists."""
-        existing_cloudspace = self.backend.client.cloud_space_service_get_cloud_space(
+        return self.backend.client.cloud_space_service_get_cloud_space(
             project_id=project_id,
             id=cloudspace_id,
         )
 
-        return existing_cloudspace
-
     def _resolve_queue_server_type(self) -> V1QueueServerType:
         """Resolve the cloud queue type from the environment."""
         queue_server_type = V1QueueServerType.UNSPECIFIED
         # Note: Enable app to select their own queue type.
         queue_type = get_cloud_queue_type()
         if queue_type == "http":
             queue_server_type = V1QueueServerType.HTTP
@@ -628,15 +627,18 @@
     def _validate_cluster_id(self, cluster_id: Optional[str], project_id: str):
         """Check that the provided cluster exists and ensure that it is bound to the given project."""
         if cluster_id is not None:
             # Verify that the cluster exists
             list_clusters_resp = self.backend.client.cluster_service_list_clusters()
             cluster_ids = [cluster.id for cluster in list_clusters_resp.clusters]
             if cluster_id not in cluster_ids:
-                raise ValueError(f"You requested to run on cluster {cluster_id}, but that cluster doesn't exist.")
+                raise ValueError(
+                    f"You requested to run on cluster {cluster_id}, but that cluster doesn't exist."
+                    f" Found {list_clusters_resp} with project_id: {project_id}"
+                )
 
             _ensure_cluster_project_binding(self.backend.client, project_id, cluster_id)
 
     def _validate_work_build_specs_and_compute(self) -> None:
         """Check that the cloud compute and build configs are valid for all works in the app."""
         for work in self.app.works:
             if work.cloud_build_config.image is not None and work.cloud_compute.name == "default":
@@ -666,15 +668,15 @@
                     if mount.protocol != "s3://":
                         raise RuntimeError(f"Unknown mount protocol `{mount.protocol}` for work `{work.name}`.")
 
     def _get_flow_servers(self) -> List[V1Flowserver]:
         """Collect a spec for each flow that contains a frontend so that the backend knows for which flows it needs
         to start servers."""
         flow_servers: List[V1Flowserver] = []
-        for flow_name in self.app.frontends.keys():
+        for flow_name in self.app.frontends:
             flow_server = V1Flowserver(name=flow_name)
             flow_servers.append(flow_server)
         return flow_servers
 
     @staticmethod
     def _get_network_configs(flow_servers: List[V1Flowserver]) -> Optional[List[V1NetworkConfig]]:
         """Get the list of network configs for the run if multiple works in default container is enabled."""
@@ -768,15 +770,15 @@
             drives = self._get_drives(work)
             mounts = self._get_mounts(work)
 
             data_connection_mounts: list[V1DataConnectionMount] = []
             if cloudspace is not None and cloudspace.code_config is not None:
                 data_connection_mounts = cloudspace.code_config.data_connection_mounts
 
-            random_name = "".join(random.choice(string.ascii_lowercase) for _ in range(5))
+            random_name = "".join(random.choice(string.ascii_lowercase) for _ in range(5))  # noqa: S311
             work_spec = V1LightningworkSpec(
                 build_spec=build_spec,
                 drives=drives + mounts,
                 user_requested_compute_config=user_compute_config,
                 network_config=[V1NetworkConfig(name=random_name, port=work.port)],
                 data_connection_mounts=data_connection_mounts,
             )
```

### Comparing `lightning-app-2.0.2/src/lightning_app/runners/multiprocess.py` & `lightning-app-2.0.3/src/lightning_app/runners/multiprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def dispatch(self, *args: Any, open_ui: bool = True, **kwargs: Any):
         """Method to dispatch and run the LightningApp."""
         try:
             _set_flow_context()
 
             # Note: In case the runtime is used in the cloud.
             in_cloudspace = constants.LIGHTNING_CLOUDSPACE_HOST is not None
-            self.host = "0.0.0.0" if constants.APP_SERVER_IN_CLOUD or in_cloudspace else self.host
+            self.host = "0.0.0.0" if constants.APP_SERVER_IN_CLOUD or in_cloudspace else self.host  # noqa: S104
 
             self.app.backend = self.backend
             self.backend._prepare_queues(self.app)
             self.backend.resolve_url(self.app, "http://127.0.0.1")
             self.app._update_index_file()
 
             # set env variables
@@ -64,15 +64,15 @@
             # refresh the layout with the populated urls.
             self.app._update_layout()
 
             _set_frontend_context()
             for frontend in self.app.frontends.values():
                 port = find_free_network_port()
 
-                server_host = "0.0.0.0" if in_cloudspace else "localhost"
+                server_host = "0.0.0.0" if in_cloudspace else "localhost"  # noqa: S104
                 server_target = (
                     f"https://{port}-{constants.LIGHTNING_CLOUDSPACE_HOST}"
                     if in_cloudspace
                     else f"http://localhost:{port}"
                 )
 
                 frontend.start_server(host=server_host, port=port)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/runners/runtime.py` & `lightning-app-2.0.3/src/lightning_app/runners/runtime.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/runners/runtime_type.py` & `lightning-app-2.0.3/src/lightning_app/runners/runtime_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,11 +24,10 @@
 class RuntimeType(Enum):
     MULTIPROCESS = "multiprocess"
     CLOUD = "cloud"
 
     def get_runtime(self) -> Type["Runtime"]:
         if self == RuntimeType.MULTIPROCESS:
             return MultiProcessRuntime
-        elif self == RuntimeType.CLOUD:
+        if self == RuntimeType.CLOUD:
             return CloudRuntime
-        else:
-            raise ValueError("Unknown runtime type")
+        raise ValueError("Unknown runtime type")
```

### Comparing `lightning-app-2.0.2/src/lightning_app/source_code/copytree.py` & `lightning-app-2.0.3/src/lightning_app/source_code/copytree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/source_code/hashing.py` & `lightning-app-2.0.3/src/lightning_app/source_code/hashing.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     [1] https://crypto.stackexchange.com/questions/70101/blake2-vs-md5-for-checksum-file-integrity
     [2] https://stackoverflow.com/questions/1131220/get-md5-hash-of-big-files-in-python
     """
     # validate input
     if algorithm == "blake2":
         h = hashlib.blake2b(digest_size=20)
     elif algorithm == "md5":
-        h = hashlib.md5()
+        h = hashlib.md5()  # noqa: S324
     else:
         raise ValueError(f"Algorithm {algorithm} not supported")
 
     # calculate hash for all files
     for file in files:
         with open(file, "rb") as f:
             for chunk in iter(lambda: f.read(chunk_num_blocks * h.block_size), b""):
```

### Comparing `lightning-app-2.0.2/src/lightning_app/source_code/local.py` & `lightning-app-2.0.3/src/lightning_app/source_code/local.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/source_code/tar.py` & `lightning-app-2.0.3/src/lightning_app/source_code/tar.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,16 @@
     file_mode = "w:gz" if compression else "w:"
 
     with tarfile.open(target_file, file_mode) as tar:
         if os.path.isdir(source_path):
             tar.add(str(source_path), arcname=".")
         elif os.path.isfile(source_path):
             file_info = tarfile.TarInfo(os.path.basename(str(source_path)))
-            tar.addfile(file_info, open(source_path))
+            with open(source_path) as fo:
+                tar.addfile(file_info, fo)
 
 
 def _tar_path_subprocess(source_path: str, target_file: str, compression: bool = False) -> None:
     """Create tar from directory using `tar`
 
     Parameters
     ----------
```

### Comparing `lightning-app-2.0.2/src/lightning_app/source_code/uploader.py` & `lightning-app-2.0.3/src/lightning_app/source_code/uploader.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/storage/copier.py` & `lightning-app-2.0.3/src/lightning_app/storage/copier.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 
 
 def _find_matching_path(work, request: _GetRequest) -> Optional["lightning_app.storage.Path"]:
     for name in work._paths:
         candidate: lightning_app.storage.Path = getattr(work, name)
         if candidate.hash == request.hash:
             return candidate
+    return None
 
 
 def _copy_files(
     source_path: pathlib.Path,
     destination_path: pathlib.Path,
     fs: Optional[AbstractFileSystem] = None,
 ) -> None:
@@ -124,17 +125,17 @@
 
         try:
             # NOTE: S3 does not have a concept of directories, so we do not need to create one.
             if isinstance(fs, LocalFileSystem):
                 fs.makedirs(str(to_path.parent), exist_ok=True)
 
             fs.put(str(from_path), str(to_path), recursive=False)
-        except Exception as e:
+        except Exception as ex:
             # Return the exception so that it can be handled in the main thread
-            return e
+            return ex
 
     # NOTE: Cannot use `S3FileSystem.put(recursive=True)` because it tries to access parent directories
     #       which it does not have access to.
     if source_path.is_dir():
         src = [file for file in source_path.rglob("*") if file.is_file()]
         dst = [destination_path / file.relative_to(source_path) for file in src]
```

### Comparing `lightning-app-2.0.2/src/lightning_app/storage/drive.py` & `lightning-app-2.0.3/src/lightning_app/storage/drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,15 @@
         root_path = self.drive_root / self.component_name
         if isinstance(self.fs, LocalFileSystem):
             self.fs.makedirs(root_path, exist_ok=True)
         return root_path
 
     @property
     def drive_root(self) -> pathlib.Path:
-        drive_root = _shared_storage_path() / "artifacts" / "drive" / self.id
-        return drive_root
+        return _shared_storage_path() / "artifacts" / "drive" / self.id
 
     def put(self, path: str) -> None:
         """This method enables to put a file to the Drive in a blocking fashion.
 
         Arguments:
             path: The relative path to your files to be added to the Drive.
         """
@@ -326,12 +325,12 @@
 
     def __str__(self) -> str:
         assert self.id
         return self.id
 
 
 def _maybe_create_drive(component_name: str, state: Dict) -> Union[Dict, Drive]:
-    if Drive.__IDENTIFIER__ == state.get("type", None):
+    if state.get("type", None) == Drive.__IDENTIFIER__:
         drive = Drive.from_dict(state)
         drive.component_name = component_name
         return drive
     return state
```

### Comparing `lightning-app-2.0.2/src/lightning_app/storage/filesystem.py` & `lightning-app-2.0.3/src/lightning_app/storage/filesystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
             glob = f"{str(src)}/**"
             fs.get(glob, str(dst), recursive=False)
     else:
         fs.get(str(src), str(dst), recursive=False)
 
 
 class FileSystem:
-
     """This filesystem enables to easily move files from and to the shared storage."""
 
     def __init__(self) -> None:
         self._fs = _filesystem()
         self._root = str(_shared_storage_path())
 
     def put(self, src_path: str, dst_path: str, put_fn: Callable = _copy_files) -> None:
```

### Comparing `lightning-app-2.0.2/src/lightning_app/storage/mount.py` & `lightning-app-2.0.3/src/lightning_app/storage/mount.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/storage/orchestrator.py` & `lightning-app-2.0.3/src/lightning_app/storage/orchestrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,14 @@
                     response_queue = self.response_queues[response.destination]
                     response_queue.put(response)
 
         # Check the current work is within the sources.
         # It is possible to have multiple destination targeting
         # the same source concurrently.
         if work_name in self.waiting_for_response.values():
-
             # check if the current work has responses for file transfers to other works.
             copy_response_queue = self.copy_response_queues[work_name]
             try:
                 # check if the share-point file manager has confirmed a copy request
                 response: _PathResponse = copy_response_queue.get(timeout=0)  # this should not block
             except Empty:
                 pass
```

### Comparing `lightning-app-2.0.2/src/lightning_app/storage/path.py` & `lightning-app-2.0.3/src/lightning_app/storage/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         """The hash of this Path uniquely identifies the file path and the associated origin Work.
 
         Returns ``None`` if the origin is not defined, i.e., this Path did not yet get attached to a LightningWork.
         """
         if self._origin is None:
             return None
         contents = f"{self.origin_name}/{self}"
-        return hashlib.sha1(contents.encode("utf-8")).hexdigest()
+        return hashlib.sha1(contents.encode("utf-8")).hexdigest()  # noqa: S324
 
     @property
     def parents(self) -> Sequence["Path"]:
         parents: List["Path"] = list(super().parents)
         for parent in parents:
             parent._copy_properties_from(self)
         return parents
@@ -359,16 +359,16 @@
             size=source_path.stat().st_size,
             destination=request.destination,
         )
 
         try:
             _copy_files(source_path, destination_path)
             _logger.debug(f"All files copied from {request.path} to {response.path}.")
-        except Exception as e:
-            response.exception = e
+        except Exception as ex:
+            response.exception = ex
         return response
 
 
 def _is_lit_path(path: Union[str, Path]) -> bool:
     path = Path(path)
     return path == _storage_root_dir() or _storage_root_dir() in path.parents
```

### Comparing `lightning-app-2.0.2/src/lightning_app/storage/payload.py` & `lightning-app-2.0.3/src/lightning_app/storage/payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         """The hash of this Payload uniquely identifies the payload and the associated origin Work.
 
         Returns ``None`` if the origin is not defined, i.e., this Path did not yet get attached to a LightningWork.
         """
         if self._origin is None:
             return None
         contents = f"{self.origin_name}/{self.consumer_name}/{self.name}"
-        return hashlib.sha1(contents.encode("utf-8")).hexdigest()
+        return hashlib.sha1(contents.encode("utf-8")).hexdigest()  # noqa: S324
 
     @property
     def origin_name(self) -> str:
         """The name of the LightningWork where this payload was first created.
 
         Attaching a Payload to a LightningWork will automatically make it the `origin`.
         """
@@ -87,15 +87,15 @@
 
         return self._consumer.name if isinstance(self._consumer, LightningWork) else self._consumer
 
     @property
     def _path(self) -> Optional[Path]:
         """Path to the file that the payload value gets serialized to."""
         if not self._name:
-            return
+            return None
         return Path("lit://", self._name)
 
     @abstractmethod
     def save(self, obj: Any, path: str) -> None:
         """Override this method with your own saving logic."""
 
     @abstractmethod
@@ -247,24 +247,23 @@
 
         try:
             payload = getattr(work, request.name)
             payload.save(payload.value, source_path)
             response.size = source_path.stat().st_size
             _copy_files(source_path, destination_path)
             _logger.debug(f"All files copied from {request.path} to {response.path}.")
-        except Exception as e:
-            response.exception = e
+        except Exception as ex:
+            response.exception = ex
         return response
 
 
 class Payload(_BasePayload):
     """The Payload object enables to transfer python objects from one work to another in a similar fashion as
     :class:`~lightning_app.storage.path.Path`."""
 
     def save(self, obj: Any, path: str) -> None:
         with open(path, "wb") as f:
             pickle.dump(obj, f)
 
     def load(self, path: str) -> Any:
         with open(path, "rb") as f:
-            obj = pickle.load(f)
-        return obj
+            return pickle.load(f)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/storage/requests.py` & `lightning-app-2.0.3/src/lightning_app/storage/requests.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/structures/dict.py` & `lightning-app-2.0.3/src/lightning_app/structures/dict.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/structures/list.py` & `lightning-app-2.0.3/src/lightning_app/structures/list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/testing/config.py` & `lightning-app-2.0.3/src/lightning_app/testing/config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/testing/helpers.py` & `lightning-app-2.0.3/src/lightning_app/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/testing/testing.py` & `lightning-app-2.0.3/src/lightning_app/testing/testing.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,16 +229,15 @@
     lit_apps = [
         app
         for app in client.lightningapp_instance_service_list_lightningapp_instances(project_id=project_id).lightningapps
         if app.name == name or getattr(app, "display_name", None) == name
     ]
     if not len(lit_apps) == 1:
         raise ValueError(f"Expected to find just one app, found {len(lit_apps)}")
-    app = lit_apps[0]
-    return app
+    return lit_apps[0]
 
 
 @requires("playwright")
 @contextmanager
 def run_app_in_cloud(
     app_folder: str, app_name: str = "app.py", extra_args: List[str] = [], debug: bool = True
 ) -> Generator:
@@ -290,28 +289,36 @@
         env_copy["LIGHTING_TESTING"] = "1"
         if debug:
             print("Debug mode is enabled")
             env_copy["LIGHTNING_DEBUG"] = "1"
         shutil.copytree(app_folder, tmpdir, dirs_exist_ok=True)
         # TODO - add -no-cache to the command line.
         stdout_path = get_logfile(f"run_app_in_cloud_{name}")
+
+        cmd_extra_args = []
+
+        if "staging.gridai.dev" in os.getenv("LIGHTNING_CLOUD_URL", ""):
+            cmd_extra_args = ["--cluster-id", "staging"]
+
         with open(stdout_path, "w") as stdout:
             cmd = [
                 sys.executable,
                 "-m",
                 "lightning",
                 "run",
                 "app",
                 app_name,
                 "--cloud",
                 "--name",
                 name,
                 "--open-ui",
                 "false",
+                *cmd_extra_args,
             ]
+            print(f"Command: {cmd}")
             process = Popen((cmd + extra_args), cwd=tmpdir, env=env_copy, stdout=stdout, stderr=sys.stderr)
             process.wait()
 
         # Fallback URL to prevent failures in case we don't get the admin URL
         admin_url = _Config.url
         with open(stdout_path) as fo:
             for line in fo.readlines():
@@ -444,14 +451,16 @@
             if debug:
                 process.kill()
 
             context.close()
             browser.close()
             Popen("lightning disconnect", shell=True).wait()
 
+            delete_cloud_lightning_apps(name=name)
+
 
 def wait_for(page, callback: Callable, *args: Any, **kwargs: Any) -> Any:
     import playwright
 
     while True:
         try:
             res = callback(*args, **kwargs)
@@ -489,44 +498,44 @@
             id=cloud_space_id,
         )
         assert res == {}
     except ApiException as ex:
         print(f"Failed to delete {app_name}. Exception {ex}")
 
 
-def delete_cloud_lightning_apps():
+def delete_cloud_lightning_apps(name=None):
     """Cleanup cloud apps that start with the name test-{PR_NUMBER}-{TEST_APP_NAME}.
 
     PR_NUMBER and TEST_APP_NAME are environment variables.
     """
 
     client = LightningClient()
 
     try:
         pr_number = int(os.getenv("PR_NUMBER", None))
     except (TypeError, ValueError):
         # Failed when the PR is running master or 'PR_NUMBER' isn't defined.
         pr_number = ""
 
-    app_name = os.getenv("TEST_APP_NAME", "")
+    app_name = os.getenv("TEST_APP_NAME", "").replace("_", "-")
 
     print(f"deleting apps for pr_number: {pr_number}, app_name: {app_name}")
     project_id = _get_project(client).project_id
     list_apps = client.lightningapp_instance_service_list_lightningapp_instances(project_id=project_id)
 
-    for lit_app in list_apps.lightningapps:
-        if pr_number and app_name and not lit_app.name.startswith(f"test-{pr_number}-{app_name}-"):
-            continue
-        _delete_lightning_app(client, project_id=project_id, app_id=lit_app.id, app_name=lit_app.name)
-        _delete_cloud_space(
-            client, project_id=project_id, cloud_space_id=lit_app.spec.cloud_space_id, app_name=lit_app.name
-        )
+    if pr_number and app_name:
+        for lit_app in list_apps.lightningapps:
+            if name == lit_app.name or (str(pr_number) in lit_app.name and app_name in lit_app.name):
+                _delete_lightning_app(client, project_id=project_id, app_id=lit_app.id, app_name=lit_app.name)
+                _delete_cloud_space(
+                    client, project_id=project_id, cloud_space_id=lit_app.spec.cloud_space_id, app_name=lit_app.name
+                )
 
-    print("deleting apps that were created more than 1 hour ago.")
+    print("deleting apps that were created more than 20 minutes ago.")
 
     for lit_app in list_apps.lightningapps:
-
-        if lit_app.created_at < datetime.datetime.now(lit_app.created_at.tzinfo) - datetime.timedelta(hours=1):
+        time_diff = datetime.datetime.now(lit_app.created_at.tzinfo) - lit_app.created_at
+        if time_diff > datetime.timedelta(minutes=20):
             _delete_lightning_app(client, project_id=project_id, app_id=lit_app.id, app_name=lit_app.name)
             _delete_cloud_space(
                 client, project_id=project_id, cloud_space_id=lit_app.spec.cloud_space_id, app_name=lit_app.name
             )
```

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/asset-manifest.json` & `lightning-app-2.0.3/src/lightning_app/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/index.html` & `lightning-app-2.0.3/src/lightning_app/ui/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/css/main.bb0f092c.css` & `lightning-app-2.0.3/src/lightning_app/ui/static/css/main.bb0f092c.css`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/css/main.bb0f092c.css.map` & `lightning-app-2.0.3/src/lightning_app/ui/static/css/main.bb0f092c.css.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/favicon.ico` & `lightning-app-2.0.3/src/lightning_app/ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/js/787.418637a8.chunk.js` & `lightning-app-2.0.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map` & `lightning-app-2.0.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js` & `lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt` & `lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js.map` & `lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/lightningState.js` & `lightning-app-2.0.3/src/lightning_app/ui/static/lightningState.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2` & `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff` & `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff` & `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2` & `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2` & `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff` & `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg` & `lightning-app-2.0.3/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg` & `lightning-app-2.0.3/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/app_commands.py` & `lightning-app-2.0.3/src/lightning_app/utilities/app_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,28 +102,23 @@
             logger.error(err_txt)
             raise MisconfigurationException(err_txt) from None
 
 
 def run_app_commands(file: str) -> None:
     """Extract all lines at the top of the file which contain commands & execute them.
 
-    Commands to execute are comment lines whose first non-whitespace character
-    begins with the "bang" symbol (`!`).  After the first non comment line we
-    stop parsing the rest of the file. Running environment is preserved in the
+    Commands to execute are comment lines whose first non-whitespace character begins with the "bang" symbol (`!`).
+    After the first non comment line we stop parsing the rest of the file. Running environment is preserved in the
     subprocess shell.
 
     For example:
 
-        # some file           <--- not a command
-        # !echo "hello world" <--- a command
-        # ! pip install foo   <--- a command
-        # foo! bar            <--- not a command
-        import lightning_app      <--- not a command, end parsing.
+    # some file           <--- not a command # !echo "hello world" <--- a command # ! pip install foo   <--- a command #
+    foo! bar            <--- not a command import lightning_app      <--- not a command, end parsing.
 
-        where `echo "hello world" && pip install foo` would be executed in the current
-        running environment.
+    where `echo "hello world" && pip install foo` would be executed in the current running environment.
     """
     cl = _extract_commands_from_file(file_name=file)
     if len(cl.commands) == 0:
         logger.debug("No in app commands to install.")
         return
     _execute_app_commands(cl=cl)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/app_helpers.py` & `lightning-app-2.0.3/src/lightning_app/utilities/app_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
     def connect(cls, app_instance: "LightningApp") -> None:
         cls._app_instance = app_instance
 
     @classmethod
     def get_current(cls) -> Optional["LightningApp"]:
         if cls._app_instance:
             return cls._app_instance
+        return None
 
 
 def affiliation(component: "Component") -> Tuple[str, ...]:
     """Returns the affiliation of a component."""
     if component.name in ("root", ""):
         return ()
     return tuple(component.name.split(".")[1:])
@@ -314,20 +315,19 @@
 
     return child_name
 
 
 def _delta_to_app_state_delta(root: "LightningFlow", component: "Component", delta: Delta) -> Delta:
     delta_dict = delta.to_dict()
     for changed in delta_dict.values():
-        for delta_key in changed.copy().keys():
+        for delta_key in changed.copy():
             val = changed[delta_key]
 
             new_prefix = "root"
             for p, c in _walk_to_component(root, component):
-
                 if isinstance(c, lightning_app.core.LightningWork):
                     new_prefix += "['works']"
 
                 if isinstance(c, lightning_app.core.LightningFlow):
                     new_prefix += "['flows']"
 
                 if isinstance(c, (lightning_app.structures.Dict, lightning_app.structures.List)):
@@ -364,15 +364,15 @@
             child = getattr(parent, n)
         yield parent, child
         parent = child
 
 
 def _collect_child_process_pids(pid: int) -> List[int]:
     """Function to return the list of child process pid's of a process."""
-    processes = os.popen("ps -ej | grep -i 'python' | grep -v 'grep' | awk '{ print $2,$3 }'").read()
+    processes = os.popen("ps -ej | grep -i 'python' | grep -v 'grep' | awk '{ print $2,$3 }'").read()  # noqa: S605
     processes = [p.split(" ") for p in processes.split("\n")[:-1]]
     return [int(child) for child, parent in processes if parent == str(pid) and child != str(pid)]
 
 
 def _print_to_logger_info(*args: Any, **kwargs: Any):
     # TODO Find a better way to re-direct print to loggers.
     lightning_app._logger.info(" ".join([str(v) for v in args]))
@@ -546,15 +546,15 @@
 
 def _using_debugger() -> bool:
     """This method is used to detect whether the app is run with a debugger attached."""
     if "LIGHTNING_DETECTED_DEBUGGER" in os.environ:
         return True
 
     # Collect the information about the process.
-    parent_process = os.popen(f"ps -ax | grep -i {os.getpid()} | grep -v grep").read()
+    parent_process = os.popen(f"ps -ax | grep -i {os.getpid()} | grep -v grep").read()  # noqa: S605
 
     # Detect whether VSCode or PyCharm debugger are used
     use_debugger = "debugpy" in parent_process or "pydev" in parent_process
 
     # Store the result to avoid multiple popen calls.
     if use_debugger:
         os.environ["LIGHTNING_DETECTED_DEBUGGER"] = "1"
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/app_logs.py` & `lightning-app-2.0.3/src/lightning_app/utilities/app_logs.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     Returns callback function used with `on_message_callback` of websocket.WebSocketApp.
     """
 
     def callback(ws_app: WebSocketApp, msg: str):
         # We strongly trust that the contract on API will hold atm :D
         event_dict = json.loads(msg)
-        labels = _LogEventLabels(**event_dict["labels"])
+        labels = _LogEventLabels(**event_dict.get("labels", {}))
 
         if "message" in event_dict:
             message = event_dict["message"]
             timestamp = dateutil.parser.isoparse(event_dict["timestamp"])
             event = _LogEvent(
                 message=message,
                 timestamp=timestamp,
@@ -75,15 +75,14 @@
     logs_api_client: _LightningLogsSocketAPI,
     project_id: str,
     app_id: str,
     component_names: List[str],
     follow: bool,
     on_error_callback: Optional[Callable] = None,
 ) -> Iterator[_LogEvent]:
-
     read_queue = queue.PriorityQueue()
 
     # We will use a socket per component
     log_sockets = [
         logs_api_client.create_lightning_logs_socket(
             project_id=project_id,
             app_id=app_id,
@@ -113,17 +112,16 @@
             log_event: _LogEvent = read_queue.get(timeout=None if follow else 1.0)
 
             token = flow if log_event.component_name == "flow" else work
             if token in log_event.message:
                 start_timestamps[log_event.component_name] = log_event.timestamp
 
             timestamp = start_timestamps.get(log_event.component_name, None)
-            if timestamp and log_event.timestamp >= timestamp:
-                if "launcher" not in log_event.message:
-                    yield log_event
+            if timestamp and log_event.timestamp >= timestamp and "launcher" not in log_event.message:
+                yield log_event
 
     except queue.Empty:
         # Empty is raised by queue.get if timeout is reached. Follow = False case.
         pass
 
     except KeyboardInterrupt:
         # User pressed CTRL+C to exit, we should respect that
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/app_status.py` & `lightning-app-2.0.3/src/lightning_app/utilities/app_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     reason: Optional[str] = None
     message: Optional[str] = None
     count: int = 1
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
-        assert self.timestamp > 0 and self.timestamp < (int(datetime.now().timestamp()) + 10)
+        assert self.timestamp > 0
+        assert self.timestamp < (int(datetime.now().timestamp()) + 10)
 
 
 class AppStatus(BaseModel):
     """The ``AppStatus`` captures the current status of the app and its components."""
 
     # ``True`` when the app UI is ready to be viewed
     is_ui_ready: bool
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/auth.py` & `lightning-app-2.0.3/src/lightning_app/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/cli_helpers.py` & `lightning-app-2.0.3/src/lightning_app/utilities/cli_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import contextlib
 import functools
 import json
 import os
 import re
 import subprocess
 import sys
 from typing import Dict, Optional
@@ -43,15 +43,14 @@
            List of str for the env variables, e.g. ['foo=bar', 'bla=bloz']
 
     Returns:
         Dict of the env variables with the following format
             key: env variable name
             value: env variable value
     """
-
     env_vars_dict = {}
     for env_str in env_list:
         var_parts = env_str.split("=")
         if len(var_parts) != 2 or not var_parts[0]:
             raise Exception(
                 f"Invalid format of environment variable {env_str}, "
                 f"please ensure that the variable is in the format e.g. foo=bar."
@@ -191,38 +190,36 @@
 
         for app in list_apps.lightningapps:
             if app.id == self.app_id_or_name_or_url or _get_app_display_name(app) == self.app_id_or_name_or_url:
                 if app.status.url == "":
                     print("The application is starting. Try in a few moments.")
                     sys.exit(0)
                 return app
+        return None
 
     def _collect_open_api_json(self):
         """This function is used to retrieve the current url associated with an id."""
-
         if _is_url(self.app_id_or_name_or_url):
             self.url = self.app_id_or_name_or_url
             assert self.url
             resp = requests.get(self.url + "/openapi.json")
             if resp.status_code != 200:
                 print(f"ERROR: The server didn't process the request properly. Found {resp.json()}")
                 sys.exit(0)
             self.openapi = resp.json()
             return
 
         # 2: If no identifier has been provided, evaluate the local application
         if self.app_id_or_name_or_url is None:
-            try:
+            with contextlib.suppress(requests.exceptions.ConnectionError):
                 self.url = f"http://localhost:{APP_SERVER_PORT}"
                 resp = requests.get(f"{self.url}/openapi.json")
                 if resp.status_code != 200:
                     raise Exception(f"The server didn't process the request properly. Found {resp.json()}")
                 self.openapi = resp.json()
-            except requests.exceptions.ConnectionError:
-                pass
 
         # 3: If an identified was provided or the local evaluation has failed, evaluate the cloud.
         else:
             app = self._maybe_find_matching_cloud_app()
             if app:
                 if app.status.url == "":
                     raise Exception("The application is starting. Try in a few moments.")
@@ -245,40 +242,31 @@
     except ValueError:
         try:
             return arrow.get(value)
         except (ValueError, TypeError):
             raise click.ClickException(f"cannot parse time {value}")
 
 
-def _is_valid_release(release):
-    version, release = release
-    version = packaging.version.parse(version)
-    if any(r["yanked"] for r in release) or version.is_devrelease or version.is_prerelease:
-        return False
-    return True
-
-
 @functools.lru_cache(maxsize=1)
 def _get_newer_version() -> Optional[str]:
     """Check PyPI for newer versions of ``lightning``, returning the newest version if different from the current
     or ``None`` otherwise."""
     if packaging.version.parse(__version__).is_prerelease:
         return None
     try:
         response = requests.get(f"https://pypi.org/pypi/{__package_name__}/json")
-        releases = response.json()["releases"]
+        response_json = response.json()
+        releases = response_json["releases"]
         if __version__ not in releases:
             # Always return None if not installed from PyPI (e.g. dev versions)
             return None
-        releases = dict(filter(_is_valid_release, releases.items()))
-        sorted_releases = sorted(
-            releases.items(), key=lambda release: release[1][0]["upload_time_iso_8601"], reverse=True
-        )
-        latest_version = sorted_releases[0][0]
-        return None if __version__ == latest_version else latest_version
+        latest_version = response_json["info"]["version"]
+        parsed_version = packaging.version.parse(latest_version)
+        is_invalid = response_json["info"]["yanked"] or parsed_version.is_devrelease or parsed_version.is_prerelease
+        return None if __version__ == latest_version or is_invalid else latest_version
     except Exception:
         # Return None if any exception occurs
         return None
 
 
 def _redirect_command(executable: str):
     """Redirect the current lightning CLI call to the given executable."""
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/cloud.py` & `lightning-app-2.0.3/src/lightning_app/utilities/cloud.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,30 +24,37 @@
 
 
 def _get_project(client: LightningClient, project_id: Optional[str] = None, verbose: bool = True) -> V1Membership:
     """Get a project membership for the user from the backend."""
     if project_id is None:
         project_id = LIGHTNING_CLOUD_PROJECT_ID
 
-    projects = client.projects_service_list_memberships()
     if project_id is not None:
-        for membership in projects.memberships:
-            if membership.project_id == project_id:
-                break
-        else:
+        project = client.projects_service_get_project(project_id)
+        if not project:
             raise ValueError(
                 "Environment variable `LIGHTNING_CLOUD_PROJECT_ID` is set but could not find an associated project."
             )
-        return membership
+        return V1Membership(
+            name=project.name,
+            display_name=project.display_name,
+            description=project.description,
+            created_at=project.created_at,
+            project_id=project.id,
+            owner_id=project.owner_id,
+            owner_type=project.owner_type,
+            quotas=project.quotas,
+            updated_at=project.updated_at,
+        )
 
+    projects = client.projects_service_list_memberships()
     if len(projects.memberships) == 0:
         raise ValueError("No valid projects found. Please reach out to lightning.ai team to create a project")
-    if len(projects.memberships) > 1:
-        if verbose:
-            print(f"Defaulting to the project: {projects.memberships[0].name}")
+    if len(projects.memberships) > 1 and verbose:
+        print(f"Defaulting to the project: {projects.memberships[0].name}")
     return projects.memberships[0]
 
 
 def _sigterm_flow_handler(*_, app: "lightning_app.LightningApp"):
     app.stage = AppStage.STOPPING
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/cluster_logs.py` & `lightning-app-2.0.3/src/lightning_app/utilities/cluster_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/clusters.py` & `lightning-app-2.0.3/src/lightning_app/utilities/clusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 
     # Filter global clusters
     clusters = [cluster for cluster in clusters if cluster.spec.cluster_type == V1ClusterType.GLOBAL]
 
     if len(clusters) == 0:
         raise RuntimeError(f"No clusters found on `{client.api_client.configuration.host}`.")
 
-    return random.choice(clusters).id
+    return random.choice(clusters).id  # noqa: S311
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/commands/base.py` & `lightning-app-2.0.3/src/lightning_app/utilities/commands/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 logger = Logger(__name__)
 
 
 def makedirs(path: str):
     r"""Recursive directory creation function."""
     try:
         os.makedirs(osp.expanduser(osp.normpath(path)))
-    except OSError as e:
-        if e.errno != errno.EEXIST and osp.isdir(path):
-            raise e
+    except OSError as ex:
+        if ex.errno != errno.EEXIST and osp.isdir(path):
+            raise ex
 
 
 class ClientCommand:
     description: str = ""
     requirements: List[str] = []
 
     def __init__(self, method: Callable):
@@ -193,20 +193,21 @@
     filepath = f"{prefix}/{name}.py"
     fs = _filesystem()
 
     if _is_s3fs_available():
         from s3fs import S3FileSystem
 
         if not isinstance(fs, S3FileSystem):
-            return
+            return None
 
         source_file = str(inspect.getfile(obj.__class__))
         remote_url = str(_shared_storage_path() / "artifacts" / filepath)
         fs.put(source_file, remote_url)
         return filepath
+    return None
 
 
 def _prepare_commands(app) -> List:
     if not is_overridden("configure_commands", app.root):
         return []
 
     # 1: Upload the command to s3.
@@ -222,17 +223,17 @@
 
 
 def _process_api_request(app, request: _APIRequest):
     flow = app.get_component_by_name(request.name)
     method = getattr(flow, request.method_name)
     try:
         response = _RequestResponse(content=method(*request.args, **request.kwargs), status_code=200)
-    except HTTPException as e:
-        logger.error(repr(e))
-        response = _RequestResponse(status_code=e.status_code, content=e.detail)
+    except HTTPException as ex:
+        logger.error(repr(ex))
+        response = _RequestResponse(status_code=ex.status_code, content=ex.detail)
     except Exception:
         logger.error(traceback.print_exc())
         response = _RequestResponse(status_code=500)
     return {"response": response, "id": request.id}
 
 
 def _process_command_requests(app, request: _CommandRequest):
@@ -240,21 +241,22 @@
         for command_name, method in command.items():
             command_name = command_name.replace(" ", "_")
             if request.method_name == command_name:
                 # 2.1: Evaluate the method associated to a specific command.
                 # Validation is done on the CLI side.
                 try:
                     response = _RequestResponse(content=method(*request.args, **request.kwargs), status_code=200)
-                except HTTPException as e:
-                    logger.error(repr(e))
-                    response = _RequestResponse(status_code=e.status_code, content=e.detail)
+                except HTTPException as ex:
+                    logger.error(repr(ex))
+                    response = _RequestResponse(status_code=ex.status_code, content=ex.detail)
                 except Exception:
                     logger.error(traceback.print_exc())
                     response = _RequestResponse(status_code=500)
                 return {"response": response, "id": request.id}
+    return None
 
 
 def _process_requests(app, requests: List[Union[_APIRequest, _CommandRequest]]) -> None:
     """Convert user commands to API endpoint."""
     responses = []
     for request in requests:
         if isinstance(request, _APIRequest):
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/component.py` & `lightning-app-2.0.3/src/lightning_app/utilities/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,15 @@
 
 def _state_to_json(state: Dict[str, Any]) -> Dict[str, Any]:
     """Utility function to make sure that state dict is json serializable."""
     from lightning_app.storage import Path
     from lightning_app.storage.payload import _BasePayload
 
     state_paths_cleaned = apply_to_collection(state, dtype=(Path, _BasePayload), function=lambda x: x.to_dict())
-    state_diff_cleaned = apply_to_collection(state_paths_cleaned, dtype=type(NotPresent), function=lambda x: None)
-    return state_diff_cleaned
+    return apply_to_collection(state_paths_cleaned, dtype=type(NotPresent), function=lambda x: None)
 
 
 def _set_context(name: Optional[str]) -> None:
     global COMPONENT_CONTEXT
     COMPONENT_CONTEXT = os.getenv("COMPONENT_CONTEXT") if name is None else ComponentContext(name)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/data_structures.py` & `lightning-app-2.0.3/src/lightning_app/utilities/data_structures.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,9 +42,8 @@
 
     def __repr__(self) -> str:
         if not len(self):
             return ""
         max_key_length = max(len(str(k)) for k in self)
         tmp_name = "{:" + str(max_key_length + 3) + "s} {}"
         rows = [tmp_name.format(f'"{n}":', self[n]) for n in sorted(self.keys())]
-        out = "\n".join(rows)
-        return out
+        return "\n".join(rows)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/dependency_caching.py` & `lightning-app-2.0.3/src/lightning_app/utilities/dependency_caching.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/enum.py` & `lightning-app-2.0.3/src/lightning_app/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/exceptions.py` & `lightning-app-2.0.3/src/lightning_app/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/frontend.py` & `lightning-app-2.0.3/src/lightning_app/utilities/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/git.py` & `lightning-app-2.0.3/src/lightning_app/utilities/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 
     Returns
     -------
     output: str
         String combining stdout and stderr.
     """
     process = subprocess.run(["git"] + args, capture_output=True, text=True, cwd=cwd, check=False)
-    output = process.stdout.strip() + process.stderr.strip()
-    return output
+    return process.stdout.strip() + process.stderr.strip()
 
 
 def get_dir_name(cwd=None) -> str:
     github_repository = execute_git_command(["config", "--get", "remote.origin.url"], cwd=cwd)
     if github_repository and "github.com" in github_repository:
         return github_repository.split("/")[-1].split(".")[0]
     raise RuntimeError("Only work with github repositories.")
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/imports.py` & `lightning-app-2.0.3/src/lightning_app/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/introspection.py` & `lightning-app-2.0.3/src/lightning_app/utilities/introspection.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,17 @@
 from typing import Any, Dict, List, Optional, Set, Type, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from lightning_app import LightningFlow, LightningWork
 
 
 class LightningVisitor(ast.NodeVisitor):
-    """
-    Base class for visitor that finds class definitions based on
-    class inheritance.
-    Derived classes are expected to define class_name and implement
-    the analyze_class_def method.
+    """Base class for visitor that finds class definitions based on class inheritance. Derived classes are expected
+    to define class_name and implement the analyze_class_def method.
+
     Attributes
     ----------
     class_name: str
         Name of class to identify, to be defined in subclasses.
     """
 
     class_name: Optional[str] = None
@@ -51,16 +49,16 @@
         if self.class_name in bases:
             entry = {"name": node.name, "type": self.class_name}
             entry.update(self.analyze_class_def(node))
             self.found.append(entry)
 
 
 class LightningModuleVisitor(LightningVisitor):
-    """
-    Finds Lightning modules based on class inheritance.
+    """Finds Lightning modules based on class inheritance.
+
     Attributes
     ----------
     class_name: Optional[str]
         Name of class to identify.
     methods: Set[str]
         Names of methods that are part of the LightningModule API.
     hooks: Set[str]
@@ -122,16 +120,16 @@
         "val_dataloader",
         "test_dataloader",
         "transfer_batch_to_device",
     }
 
 
 class LightningDataModuleVisitor(LightningVisitor):
-    """
-    Finds Lightning data modules based on class inheritance.
+    """Finds Lightning data modules based on class inheritance.
+
     Attributes
     ----------
     class_name: Optional[str]
         Name of class to identify.
     methods: Set[str]
         Names of methods that are part of the LightningDataModule API.
     """
@@ -145,32 +143,32 @@
         "val_dataloader",
         "test_dataloader",
         "transfer_batch_to_device",
     }
 
 
 class LightningLoggerVisitor(LightningVisitor):
-    """
-    Finds Lightning loggers based on class inheritance.
+    """Finds Lightning loggers based on class inheritance.
+
     Attributes
     ----------
     class_name: Optional[str]
         Name of class to identify.
     methods: Set[str]
         Names of methods that are part of the Logger API.
     """
 
     class_name = "Logger"
 
     methods: Set[str] = {"log_hyperparams", "log_metrics"}
 
 
 class LightningCallbackVisitor(LightningVisitor):
-    """
-    Finds Lightning callbacks based on class inheritance.
+    """Finds Lightning callbacks based on class inheritance.
+
     Attributes
     ----------
     class_name: Optional[str]
         Name of class to identify.
     methods: Set[str]
         Names of methods that are part of the Logger API.
     """
@@ -213,16 +211,16 @@
         "on_keyboard_interrupt",
         "on_save_checkpoint",
         "on_load_checkpoint",
     }
 
 
 class LightningStrategyVisitor(LightningVisitor):
-    """
-    Finds Lightning callbacks based on class inheritance.
+    """Finds Lightning callbacks based on class inheritance.
+
     Attributes
     ----------
     class_name: Optional[str]
         Name of class to identify.
     methods: Set[str]
         Names of methods that are part of the Logger API.
     """
@@ -267,16 +265,16 @@
 
 
 class LightningProfilerVisitor(LightningVisitor):
     class_name = "Profiler"
 
 
 class Scanner:
-    """
-    Finds relevant Lightning objects in files in the file system.
+    """Finds relevant Lightning objects in files in the file system.
+
     Attributes
     ----------
     visitor_classes: List[Type]
         List of visitor classes to use when traversing files.
     Parameters
     ----------
     path: str
@@ -320,30 +318,28 @@
             try:
                 module = ast.parse(path.open().read())
             except SyntaxError:
                 print(f"Error while parsing {path}: SKIPPING")
                 continue
 
             for node in ast.walk(module):
-
                 if isinstance(node, ast.ImportFrom):
                     for import_from_cls in node.names:
                         classes.append(import_from_cls.name)
 
                 if isinstance(node, ast.Call):
                     cls_name = getattr(node.func, "attr", None)
                     if cls_name:
                         classes.append(cls_name)
 
         return cls.__name__ in classes
 
     def scan(self) -> List[Dict[str, str]]:
-        """
-        Finds Lightning modules in files, returning importable
-        objects.
+        """Finds Lightning modules in files, returning importable objects.
+
         Returns
         -------
         List[Dict[str, Any]]
             List of dicts containing all metadata required
             to import modules found.
         """
         modules_found: Dict[str, List[Dict[str, Any]]] = {}
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/layout.py` & `lightning-app-2.0.3/src/lightning_app/utilities/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         for i in idx_list:
             line = lines[i]
             line += comment
             lines[i] = line
 
         return "\n".join(lines)
 
-    except Exception as e:  # noqa
+    except Exception:
         return ""
 
 
 def _collect_layout(app: "lightning_app.LightningApp", flow: "lightning_app.LightningFlow") -> Union[Dict, List[Dict]]:
     """Process the layout returned by the ``configure_layout()`` method in each flow."""
     layout = flow.configure_layout()
 
@@ -50,25 +50,26 @@
         frontend = layout
         frontend.flow = flow
         app.frontends.setdefault(flow.name, frontend)
 
         # When running locally, the target will get overwritten by the dispatcher when launching the frontend servers
         # When running in the cloud, the frontend code will construct the URL based on the flow name
         return flow._layout
-    elif isinstance(layout, _MagicMockJsonSerializable):
+    if isinstance(layout, _MagicMockJsonSerializable):
         # The import was mocked, we set a dummy `Frontend` so that `is_headless` knows there is a UI
         app.frontends.setdefault(flow.name, "mock")
         return flow._layout
-    elif isinstance(layout, dict):
+    if isinstance(layout, dict):
         layout = _collect_content_layout([layout], app, flow)
     elif isinstance(layout, (list, tuple)) and all(isinstance(item, dict) for item in layout):
         layout = _collect_content_layout(layout, app, flow)
     else:
         lines = _add_comment_to_literal_code(flow.configure_layout, contains="return", comment="  <------- this guy")
-        m = f"""
+        raise TypeError(
+            f"""
         The return value of configure_layout() in `{flow.__class__.__name__}`  is an unsupported layout format:
         \n{lines}
 
         Return either an object of type {Frontend} (e.g., StreamlitFrontend, StaticWebFrontend):
             def configure_layout(self):
                 return la.frontend.Frontend(...)
 
@@ -81,15 +82,15 @@
             def configure_layout(self):
                 tab1 = {{'name': 'tab name 1', 'content': self.component_a}}
                 tab2 = {{'name': 'tab name 2', 'content': self.component_b}}
                 return [tab1, tab2]
 
         (see the docs for `LightningFlow.configure_layout`).
         """
-        raise TypeError(m)
+        )
 
     return layout
 
 
 def _collect_content_layout(
     layout: List[Dict], app: "lightning_app.LightningApp", flow: "lightning_app.LightningFlow"
 ) -> Union[List[Dict], Dict]:
@@ -181,35 +182,32 @@
 
     Args:
         work: The work to collect the layout for.
 
     Raises:
         TypeError: If the value returned by ``configure_layout`` is not of a supported format.
     """
-    if is_overridden("configure_layout", work):
-        work_layout = work.configure_layout()
-    else:
-        work_layout = work.url
+    work_layout = work.configure_layout() if is_overridden("configure_layout", work) else work.url
 
     if work_layout is None:
         return None
-    elif isinstance(work_layout, str):
+    if isinstance(work_layout, str):
         url = work_layout
         # The URL isn't fully defined yet. Looks something like ``self.work.url + /something``.
         if url and not url.startswith("/"):
             return url
         return ""
-    elif isinstance(work_layout, (Frontend, _MagicMockJsonSerializable)):
+    if isinstance(work_layout, (Frontend, _MagicMockJsonSerializable)):
         return work_layout
-    else:
-        m = f"""
-        The value returned by `{work.__class__.__name__}.configure_layout()` is of an unsupported type.
+    raise TypeError(
+        f"""
+    The value returned by `{work.__class__.__name__}.configure_layout()` is of an unsupported type.
 
-        {repr(work_layout)}
+    {repr(work_layout)}
 
-        Return a `Frontend` or a URL string, for example:
+    Return a `Frontend` or a URL string, for example:
 
-        class {work.__class__.__name__}(LightningWork):
-            def configure_layout(self):
-                return MyFrontend() OR 'http://some/url'
-        """
-        raise TypeError(m)
+    class {work.__class__.__name__}(LightningWork):
+        def configure_layout(self):
+            return MyFrontend() OR 'http://some/url'
+    """
+    )
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/load_app.py` & `lightning-app-2.0.3/src/lightning_app/utilities/load_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,24 +67,23 @@
 
     # In order for imports to work in a non-package, Python normally adds the current working directory to the
     # system path, not however when running from an entry point like the `lightning` CLI command. So we do it manually:
     with _patch_sys_path(os.path.dirname(os.path.abspath(filepath))):
         code = _create_code(filepath)
         with _create_fake_main_module(filepath) as module:
             try:
-                with _add_to_env(env_vars):
-                    with _patch_sys_argv():
-                        if mock_imports:
-                            with _mock_missing_imports():
-                                exec(code, module.__dict__)
-                        else:
-                            exec(code, module.__dict__)
-            except Exception as e:
+                with _add_to_env(env_vars), _patch_sys_argv():
+                    if mock_imports:
+                        with _mock_missing_imports():
+                            exec(code, module.__dict__)  # noqa: S102
+                    else:
+                        exec(code, module.__dict__)  # noqa: S102
+            except Exception as ex:
                 if raise_exception:
-                    raise e
+                    raise ex
                 _prettifiy_exception(filepath)
 
     return [v for v in module.__dict__.values() if isinstance(v, target_type)], module
 
 
 def _load_plugin_from_file(filepath: str) -> "LightningPlugin":
     from lightning_app.plugin.plugin import LightningPlugin
@@ -131,15 +130,14 @@
         f"The provided file {filepath} does not contain a LightningApp. Instantiate your app at the module level"
         " like so: `app = LightningApp(flow, ...)`"
     )
 
 
 def _new_module(name):
     """Create a new module with the given name."""
-
     return types.ModuleType(name)
 
 
 def open_python_file(filename):
     """Open a read-only Python file taking proper care of its encoding.
 
     In Python 3, we would like all files to be opened with utf-8 encoding. However, some author like to specify PEP263
@@ -147,16 +145,15 @@
     """
     import tokenize
 
     if hasattr(tokenize, "open"):  # Added in Python 3.2
         # Open file respecting PEP263 encoding. If no encoding header is
         # found, opens as utf-8.
         return tokenize.open(filename)
-    else:
-        return open(filename, encoding="utf-8")
+    return open(filename, encoding="utf-8")  # noqa: SIM115
 
 
 def _create_code(script_path: str):
     with open_python_file(script_path) as f:
         filebody = f.read()
 
     return compile(
@@ -257,18 +254,15 @@
         argv_slice = sys.argv
         # 4: Find the index of `app_args`
         first_index = argv_slice.index("--app_args") + 1
         # 5: Find the next argument from the CLI if any.
         matches = [
             argv_slice.index(opt) for opt in options if opt in argv_slice and argv_slice.index(opt) >= first_index
         ]
-        if not matches:
-            last_index = len(argv_slice)
-        else:
-            last_index = min(matches)
+        last_index = len(argv_slice) if not matches else min(matches)
         # 6: last_index is either the fully command or the latest match from the CLI options.
         new_argv = [argv_slice[0]] + argv_slice[first_index:last_index]
 
     # 7: Patch the command
     sys.argv = new_argv
 
     try:
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/log.py` & `lightning-app-2.0.3/src/lightning_app/utilities/types.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,17 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from pathlib import Path
+import typing as t
+from typing import Protocol, runtime_checkable
 
-from lightning_app.storage.path import _storage_root_dir
+from lightning_app import LightningFlow, LightningWork
+from lightning_app.structures import Dict, List
 
+Component = t.Union[LightningFlow, LightningWork, Dict, List]
+ComponentTuple = (LightningFlow, LightningWork, Dict, List)
 
-def get_logfile(filename: str = "logs.log") -> Path:
-    log_dir = Path(_storage_root_dir(), "frontend")
-    log_dir.mkdir(parents=True, exist_ok=True)
-    log_file = log_dir / filename
-    return log_file
+
+@runtime_checkable
+class Hashable(Protocol):
+    def to_dict(self) -> t.Dict[str, t.Any]:
+        ...
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/log_helpers.py` & `lightning-app-2.0.3/src/lightning_app/utilities/log_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/login.py` & `lightning-app-2.0.3/src/lightning_app/utilities/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,25 +123,25 @@
             for key in Keys:
                 setattr(self, key.suffix, os.environ.get(key.value, None))
 
             if self.user_id and self.api_key:
                 self.save("", self.user_id, self.api_key, self.user_id)
                 logger.info("Credentials loaded from environment variables")
                 return self.auth_header
-            elif self.api_key or self.user_id:
+            if self.api_key or self.user_id:
                 raise ValueError(
                     "To use env vars for authentication both "
                     f"{Keys.USER_ID.value} and {Keys.API_KEY.value} should be set."
                 )
 
             logger.debug("failed to load credentials, opening browser to get new.")
             self._run_server()
             return self.auth_header
 
-        elif self.user_id and self.api_key:
+        if self.user_id and self.api_key:
             return self.auth_header
 
         raise ValueError(
             "We couldn't find any credentials linked to your account. "
             "Please try logging in using the CLI command `lightning login`"
         )
 
@@ -157,21 +157,21 @@
         app = FastAPI()
         port = find_free_network_port()
         url = self.get_auth_url(port)
 
         try:
             # check if server is reachable or catch any network errors
             requests.head(url)
-        except requests.ConnectionError as e:
+        except requests.ConnectionError as ex:
             raise requests.ConnectionError(
-                f"No internet connection available. Please connect to a stable internet connection \n{e}"  # E501
+                f"No internet connection available. Please connect to a stable internet connection \n{ex}"  # E501
             )
-        except requests.RequestException as e:
+        except requests.RequestException as ex:
             raise requests.RequestException(
-                f"An error occurred with the request. Please report this issue to Lightning Team \n{e}"  # E501
+                f"An error occurred with the request. Please report this issue to Lightning Team \n{ex}"  # E501
             )
 
         logger.info(
             "\nAttempting to automatically open the login page in your default browser.\n"
             'If the browser does not open, navigate to the "Keys" tab on your Lightning AI profile page:\n\n'
             f"{get_lightning_cloud_url()}/me/keys\n\n"
             'Copy the "Headless CLI Login" command, and execute it in your terminal.\n'
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/logs_socket_api.py` & `lightning-app-2.0.3/src/lightning_app/utilities/logs_socket_api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/name_generator.py` & `lightning-app-2.0.3/src/lightning_app/utilities/name_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1350,9 +1350,9 @@
 
     >>> import random ; random.seed(42)
     >>> get_unique_name()
     'meek-ardinghelli-4506'
     >>> get_unique_name()
     'truthful-dijkstra-2286'
     """
-    adjective, surname, i = choice(_adjectives), choice(_surnames), randint(0, 9999)
+    adjective, surname, i = choice(_adjectives), choice(_surnames), randint(0, 9999)  # noqa: S311
     return f"{adjective}-{surname}-{i}"
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/network.py` & `lightning-app-2.0.3/src/lightning_app/utilities/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,31 +132,31 @@
 
     @wraps(func)
     def wrapped(*args: Any, **kwargs: Any) -> Any:
         consecutive_errors = 0
         while _get_next_backoff_time(consecutive_errors) != _DEFAULT_BACKOFF_MAX:
             try:
                 return func(self, *args, **kwargs)
-            except lightning_cloud.openapi.rest.ApiException as e:
+            except lightning_cloud.openapi.rest.ApiException as ex:
                 # retry if the control plane fails with all errors except 4xx but not 408 - (Request Timeout)
-                if e.status == 408 or e.status == 409 or not str(e.status).startswith("4"):
+                if ex.status == 408 or ex.status == 409 or not str(ex.status).startswith("4"):
                     consecutive_errors += 1
                     backoff_time = _get_next_backoff_time(consecutive_errors)
                     logger.debug(
-                        f"The {func.__name__} request failed to reach the server, got a response {e.status}."
+                        f"The {func.__name__} request failed to reach the server, got a response {ex.status}."
                         f" Retrying after {backoff_time} seconds."
                     )
                     time.sleep(backoff_time)
                 else:
-                    raise e
-            except urllib3.exceptions.HTTPError as e:
+                    raise ex
+            except urllib3.exceptions.HTTPError as ex:
                 consecutive_errors += 1
                 backoff_time = _get_next_backoff_time(consecutive_errors)
                 logger.debug(
-                    f"The {func.__name__} request failed to reach the server, got a an error {str(e)}."
+                    f"The {func.__name__} request failed to reach the server, got a an error {str(ex)}."
                     f" Retrying after {backoff_time} seconds."
                 )
                 time.sleep(backoff_time)
 
         raise Exception(f"The default maximum backoff {_DEFAULT_BACKOFF_MAX} seconds has been reached.")
 
     return wrapped
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/openapi.py` & `lightning-app-2.0.3/src/lightning_app/utilities/openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 def string2dict(text):
     """string2dict parses a JSON string into a dictionary, ensuring no keys are duplicated by accident."""
     if not isinstance(text, str):
         text = text.decode("utf-8")
     try:
         js = json.loads(text, object_pairs_hook=_duplicate_checker)
         return js
-    except ValueError as e:
-        raise ValueError(f"Unable to load JSON: {str(e)}.")
+    except ValueError as ex:
+        raise ValueError(f"Unable to load JSON: {str(ex)}.")
 
 
 def is_openapi(obj):
     """is_openopi checks if an object was generated by OpenAPI."""
     return hasattr(obj, "swagger_types")
 
 
@@ -67,9 +67,8 @@
             target_attribs[key] = create_openapi_object(value, sub_target)
         else:
             target_attribs[key] = value
 
         # TODO(sherin) - specifically process list and dict and do the validation. Also do the
         #  verification for enum types
 
-    new_target = target.__class__(**target_attribs)
-    return new_target
+    return target.__class__(**target_attribs)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/packaging/app_config.py` & `lightning-app-2.0.3/src/lightning_app/utilities/packaging/app_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/packaging/build_config.py` & `lightning-app-2.0.3/src/lightning_app/utilities/packaging/build_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,21 +27,15 @@
 
 logger = Logger(__name__)
 
 
 def load_requirements(
     path_dir: str, file_name: str = "base.txt", comment_char: str = "#", unfreeze: bool = True
 ) -> List[str]:
-    """Load requirements from a file.
-
-    >>> from lightning_app import _PROJECT_ROOT
-    >>> path_req = os.path.join(_PROJECT_ROOT, "requirements")
-    >>> load_requirements(path_req, "docs.txt")  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE +SKIP
-    ['sphinx>=4.0', ...]
-    """
+    """Load requirements from a file."""
     path = os.path.join(path_dir, file_name)
     if not os.path.isfile(path):
         return []
 
     with open(path) as file:
         lines = [ln.strip() for ln in file.readlines()]
     reqs = []
@@ -165,14 +159,15 @@
         if file is None:
             return None
         # 2. Check for Dockerfile.
         dirname = os.path.dirname(file)
         dockerfile = os.path.join(dirname, filename)
         if os.path.isfile(dockerfile):
             return dockerfile
+        return None
 
     def _prepare_requirements(self) -> None:
         requirements = []
         for req in self.requirements:
             # 1. Check for relative path
             path = os.path.join(self._call_dir, req)
             if os.path.isfile(path):
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/packaging/cloud_compute.py` & `lightning-app-2.0.3/src/lightning_app/utilities/packaging/cloud_compute.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,11 +167,10 @@
     if isinstance(mounts, (list, tuple, set)):
         mount_paths = [mount.mount_path for mount in mounts]
         if len(set(mount_paths)) != len(mount_paths):
             raise ValueError("Every Mount attached to a work must have a unique 'mount_path' argument.")
 
 
 def _maybe_create_cloud_compute(state: Dict) -> Union[CloudCompute, Dict]:
-    if state and __CLOUD_COMPUTE_IDENTIFIER__ == state.get("type", None):
-        cloud_compute = CloudCompute.from_dict(state)
-        return cloud_compute
+    if state and state.get("type", None) == __CLOUD_COMPUTE_IDENTIFIER__:
+        return CloudCompute.from_dict(state)
     return state
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/packaging/docker.py` & `lightning-app-2.0.3/src/lightning_app/utilities/packaging/docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         container_base = f"{_PROJECT_ROOT}/dockers/Dockerfile.base.cpu"
         destination_path = os.path.join(_PROJECT_ROOT, "Dockerfile")
 
         # 2. Copy the base Dockerfile within the Lightning project
         shutil.copy(container_base, destination_path)
 
         # 3. Build the docker image.
-        os.system("docker build . --tag thomaschaton/base")
+        os.system("docker build . --tag thomaschaton/base")  # noqa: S605
 
         # 4. Clean the copied base Dockerfile.
         os.remove(destination_path)
 
     def _create_work_container(self) -> None:
         # 1. Get work container.
         source_path = os.path.join(_PROJECT_ROOT, "dockers/Dockerfile.jinja")
@@ -80,15 +80,15 @@
         )
 
         with open(destination_path, "w") as f:
             f.write(dockerfile_str)
 
         # 4. Build the container.
         self.image = f"work-{self.work.__class__.__qualname__.lower()}"
-        os.system(f"docker build . --tag {self.image}")
+        os.system(f"docker build . --tag {self.image}")  # noqa: S605
 
         # 5. Clean the leftover files.
         os.remove(destination_path)
         os.remove(work_destination_path)
 
     def run(self) -> None:
         assert self.image
@@ -111,15 +111,15 @@
 
         # 2. Check the log and exit when ``Starting WorkRunner`` is found.
         for line in self.container.logs(stream=True):
             line = str(line.strip())
             print(line)
             if "command not found" in line:
                 raise RuntimeError("The container wasn't properly executed.")
-            elif "Starting WorkRunner" in line:
+            if "Starting WorkRunner" in line:
                 break
 
     def get_container_logs(self) -> str:
         """Returns the logs of the container produced until now."""
         return "".join([chr(c) for c in self.container.logs(until=datetime.now())])
 
     def kill(self) -> None:
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/packaging/lightning_utils.py` & `lightning-app-2.0.3/src/lightning_app/utilities/packaging/lightning_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     directory."""
     build_dir = "build"
     frontend_dir = pathlib.Path(FRONTEND_DIR)
     download_dir = tempfile.mkdtemp()
 
     shutil.rmtree(frontend_dir, ignore_errors=True)
 
-    response = urllib.request.urlopen(LIGHTNING_FRONTEND_RELEASE_URL)
+    response = urllib.request.urlopen(LIGHTNING_FRONTEND_RELEASE_URL)  # noqa: S310
 
     file = tarfile.open(fileobj=response, mode="r|gz")
     file.extractall(path=download_dir)
 
     shutil.move(os.path.join(download_dir, build_dir), frontend_dir)
     print("The Lightning UI has successfully been downloaded!")
 
@@ -110,25 +110,25 @@
 def _prepare_lightning_wheels_and_requirements(root: Path, package_name: str = "lightning") -> Optional[Callable]:
     """This function determines if lightning is installed in editable mode (for developers) and packages the
     current lightning source along with the app.
 
     For normal users who install via PyPi or Conda, then this function does not do anything.
     """
     if not get_dist_path_if_editable_install(package_name):
-        return
+        return None
 
     os.environ["PACKAGE_NAME"] = "app" if package_name == "lightning" + "_app" else "lightning"
 
     # Packaging the Lightning codebase happens only inside the `lightning` repo.
     git_dir_name = get_dir_name() if check_github_repository() else None
 
     is_lightning = git_dir_name and git_dir_name == package_name
 
     if (PACKAGE_LIGHTNING is None and not is_lightning) or PACKAGE_LIGHTNING == "0":
-        return
+        return None
 
     download_frontend(_PROJECT_ROOT)
     _prepare_wheel(_PROJECT_ROOT)
 
     # todo: check why logging.info is missing in outputs
     print(f"Packaged Lightning with your application. Version: {version}")
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/packaging/tarfile.py` & `lightning-app-2.0.3/src/lightning_app/utilities/packaging/tarfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 import os
 import shutil
 import tarfile
 
 
 def clean_tarfile(file_path: str, mode: str) -> None:
     """This utility removes all files extracted from a tarfile."""
-
     if not os.path.exists(file_path):
-        return None
+        return
 
     with tarfile.open(file_path, mode=mode) as tar_ref:
         for member in tar_ref.getmembers():
             p = member.path
             if p == "." or not os.path.exists(p):
                 continue
             try:
@@ -39,15 +38,15 @@
     if os.path.exists(file_path):
         os.remove(file_path)
 
 
 def extract_tarfile(file_path: str, extract_path: str, mode: str) -> None:
     """This utility extracts all files from a tarfile."""
     if not os.path.exists(file_path):
-        return None
+        return
 
     with tarfile.open(file_path, mode=mode) as tar_ref:
         for member in tar_ref.getmembers():
             try:
                 tar_ref.extract(member, path=extract_path, set_attrs=False)
             except PermissionError:
                 raise PermissionError(f"Could not extract tar file {file_path}")
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/port.py` & `lightning-app-2.0.3/src/lightning_app/utilities/port.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
         )
 
     return found_nc
 
 
 def disable_port(port: int, ignore_disabled: bool = True) -> None:
     """Make a request to the cloud controlplane to close a port of the flow."""
-
     app_id = os.getenv("LIGHTNING_CLOUD_APP_ID", None)
     project_id = os.getenv("LIGHTNING_CLOUD_PROJECT_ID", None)
 
     if not app_id or not project_id:
         raise Exception("The app_id and project_id should be defined.")
 
     client = LightningClient()
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/proxies.py` & `lightning-app-2.0.3/src/lightning_app/utilities/proxies.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         fn = fn.__wrapped__
     return fn
 
 
 def _send_data_to_caller_queue(
     proxy, work: "LightningWork", caller_queue: "BaseQueue", data: Dict, call_hash: str
 ) -> Dict:
-
     proxy.has_sent = True
 
     if work._calls[CacheCallsKeys.LATEST_CALL_HASH] is None:
         work._calls[CacheCallsKeys.LATEST_CALL_HASH] = call_hash
 
     if call_hash not in work._calls:
         work._calls[call_hash] = {"statuses": []}
@@ -131,30 +130,24 @@
         entered = call_hash in self.work._calls
         returned = entered and "ret" in self.work._calls[call_hash]
         # TODO (tchaton): Handle spot instance retrieval differently from stopped work.
         stopped_on_sigterm = self.work._restarting and self.work.status.reason == WorkStopReasons.SIGTERM_SIGNAL_HANDLER
 
         data = {"args": args, "kwargs": kwargs, "call_hash": call_hash}
 
-        # The if/else conditions are left un-compressed to simplify readability
-        # for the readers.
-        if self.work.cache_calls:
-            if not entered or stopped_on_sigterm:
-                _send_data_to_caller_queue(self, self.work, self.caller_queue, data, call_hash)
-            else:
-                if returned:
-                    return
+        # The if/else conditions are left un-compressed to simplify readability for the readers.
+        if not entered or stopped_on_sigterm:
+            _send_data_to_caller_queue(self, self.work, self.caller_queue, data, call_hash)
         else:
-            if not entered or stopped_on_sigterm:
+            if self.work.cache_calls and returned:
+                return
+            elif returned or stopped_on_sigterm:
+                # the previous task has completed and we can re-queue the next one.
+                # overriding the return value for next loop iteration.
                 _send_data_to_caller_queue(self, self.work, self.caller_queue, data, call_hash)
-            else:
-                if returned or stopped_on_sigterm:
-                    # the previous task has completed and we can re-queue the next one.
-                    # overriding the return value for next loop iteration.
-                    _send_data_to_caller_queue(self, self.work, self.caller_queue, data, call_hash)
         if not self.work.parallel:
             raise CacheMissException("Task never called before. Triggered now")
 
     def _validate_call_args(self, args: Tuple[Any, ...], kwargs: Dict[str, Any]) -> None:
         """Validate the call args before they get passed to the run method of the Work.
 
         Currently, this performs a check against strings that look like filesystem paths and may need to be wrapped with
@@ -300,18 +293,18 @@
             while True:
                 deep_diff = self.get_state_changed_from_queue(self._flow_to_work_delta_queue)
                 if not isinstance(deep_diff, dict):
                     break
                 try:
                     with _state_observer_lock:
                         self._work.apply_flow_delta(Delta(deep_diff, raise_errors=True))
-                except Exception as e:
+                except Exception as ex:
                     print(traceback.print_exc())
-                    self._error_queue.put(e)
-                    raise e
+                    self._error_queue.put(ex)
+                    raise ex
 
     def join(self, timeout: Optional[float] = None) -> None:
         self._exit_event.set()
         super().join(timeout)
 
 
 @dataclass
@@ -382,16 +375,15 @@
     def process_queue(queue):
         from lightning_app.core.queues import HTTPQueue, RedisQueue
 
         if isinstance(queue, dict):
             queue_type = queue.pop("type")
             if queue_type == "redis":
                 return RedisQueue.from_dict(queue)
-            else:
-                return HTTPQueue.from_dict(queue)
+            return HTTPQueue.from_dict(queue)
         return queue
 
 
 @dataclass
 class WorkRunner:
     work: "LightningWork"
     work_name: str
@@ -418,27 +410,27 @@
                 self.run_once()
             except KeyboardInterrupt:
                 if self.state_observer:
                     if self.state_observer.started:
                         self.state_observer.join(0)
                     self.state_observer = None
                 self.copier.join(0)
-            except LightningSigtermStateException as e:
+            except LightningSigtermStateException as ex:
                 logger.debug("Exiting")
-                os._exit(e.exit_code)
-            except Exception as e:
+                os._exit(ex.exit_code)
+            except Exception as ex:
                 # Inform the flow the work failed. This would fail the entire application.
-                self.error_queue.put(e)
+                self.error_queue.put(ex)
                 # Terminate the threads
                 if self.state_observer:
                     if self.state_observer.started:
                         self.state_observer.join(0)
                     self.state_observer = None
                 self.copier.join(0)
-                raise e
+                raise ex
 
     def setup(self):
         from lightning_app.utilities.state import AppState
 
         _set_work_context()
 
         # 1. Make the AppState aware of the affiliation of the work.
@@ -497,16 +489,17 @@
 
         # 7. Deepcopy the work state and send the first `RUNNING` status delta to the flow.
         reference_state = deepcopy(self.work.state)
 
         # Set the internal IP address.
         # Set this here after the state observer is initialized, since it needs to record it as a change and send
         # it back to the flow
-        default_internal_ip = "127.0.0.1" if constants.LIGHTNING_CLOUDSPACE_HOST is None else "0.0.0.0"
-        self.work._internal_ip = os.environ.get("LIGHTNING_NODE_IP", default_internal_ip)
+        default_internal_ip = "127.0.0.1" if constants.LIGHTNING_CLOUDSPACE_HOST is None else "0.0.0.0"  # noqa: S104
+        self.work._internal_ip = os.environ.get("LIGHTNING_NODE_PRIVATE_IP", default_internal_ip)
+        self.work._public_ip = os.environ.get("LIGHTNING_NODE_IP", "")
 
         # 8. Patch the setattr method of the work. This needs to be done after step 4, so we don't
         # send delta while calling `set_state`.
         self._proxy_setattr()
 
         if self._is_starting(called, reference_state, call_hash):
             return
@@ -528,17 +521,17 @@
         if self.run_executor_cls.enable_start_observer:
             self.state_observer.start()
 
         # 12. Run the `work_run` method.
         # If an exception is raised, send a `FAILED` status delta to the flow and call the `on_exception` hook.
         try:
             ret = self.run_executor_cls(self.work, work_run, self.delta_queue)(*args, **kwargs)
-        except LightningSigtermStateException as e:
-            raise e
-        except BaseException as e:
+        except LightningSigtermStateException as ex:
+            raise ex
+        except BaseException as ex:
             # 10.2 Send failed delta to the flow.
             reference_state = deepcopy(self.work.state)
             exp, val, tb = sys.exc_info()
             listing = traceback.format_exception(exp, val, tb)
             user_exception = False
             used_runpy = False
             trace = []
@@ -562,24 +555,23 @@
                 )
             )
             self.delta_queue.put(
                 ComponentDelta(
                     id=self.work_name, delta=Delta(DeepDiff(reference_state, self.work.state, verbose_level=2))
                 )
             )
-            self.work.on_exception(e)
+            self.work.on_exception(ex)
             print("########## CAPTURED EXCEPTION ###########")
             print(traceback.print_exc())
             print("########## CAPTURED EXCEPTION ###########")
             return
 
         # 13. Destroy the state observer.
-        if self.run_executor_cls.enable_start_observer:
-            if self.state_observer.started:
-                self.state_observer.join(0)
+        if self.run_executor_cls.enable_start_observer and self.state_observer.started:
+            self.state_observer.join(0)
         self.state_observer = None
 
         # 14. Copy all artifacts to the shared storage so other Works can access them while this Work gets scaled down
         persist_artifacts(work=self.work)
 
         # 15. An asynchronous work shouldn't return a return value.
         if ret is not None:
@@ -685,16 +677,15 @@
                 # 9. Inform the flow the work is running and add the delta to the deepcopy.
                 self.work._calls[CacheCallsKeys.LATEST_CALL_HASH] = call_hash
                 self.work._calls[call_hash]["statuses"].append(make_status(WorkStageStatus.STARTED))
                 delta = Delta(DeepDiff(reference_state, self.work.state))
                 self.delta_queue.put(ComponentDelta(id=self.work_name, delta=delta))
                 self._proxy_setattr(cleanup=True)
                 return True
-            else:
-                raise Exception("Only the `start` action is supported right now !")
+            raise Exception("Only the `start` action is supported right now !")
         return False
 
 
 def persist_artifacts(work: "LightningWork") -> None:
     """Copies all :class:`~lightning_app.storage.path.Path` referenced by the given LightningWork to the shared
     storage.
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/redis.py` & `lightning-app-2.0.3/src/lightning_app/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/safe_pickle.py` & `lightning-app-2.0.3/src/lightning_app/utilities/safe_pickle.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         __module__ attribute
 
         └── foo
             ├── __init__.py
             └── bar
                 └── app.py
     """
-
     # If the work object not taken from the app ref, there is a thread lock reference
     # somewhere thats preventing it from being pickled. Investigate it later. We
     # shouldn't be fetching the work object from the app ref. TODO @sherin
     app_ref = _LightningAppRef.get_current()
     if app_ref is None:
         raise RuntimeError("Cannot pickle LightningWork outside of a LightningApp")
     for w in app_ref.works:
@@ -86,17 +85,16 @@
         expected_module_name = relative_path.as_posix().replace(".py", "").replace("/", ".")
         # TODO @sherin: also check if the module is importable from the CWD
         fake_module = types.ModuleType(expected_module_name)
         fake_module.__dict__.update(work_class_module.__dict__)
         fake_module.__dict__["__name__"] = expected_module_name
         sys.modules[expected_module_name] = fake_module
         for k, v in fake_module.__dict__.items():
-            if not k.startswith("__") and hasattr(v, "__module__"):
-                if "_main__" in v.__module__:
-                    v.__module__ = expected_module_name
+            if not k.startswith("__") and hasattr(v, "__module__") and "_main__" in v.__module__:
+                v.__module__ = expected_module_name
     return copied_work
 
 
 def dump(work: LightningWork, f: typing.BinaryIO) -> None:
     picklable_work = get_picklable_work(work)
     pickle.dump(picklable_work, f)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/scheduler.py` & `lightning-app-2.0.3/src/lightning_app/utilities/scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,20 +28,17 @@
     def __init__(self, app) -> None:
         super().__init__(daemon=True)
         self._exit_event = threading.Event()
         self._sleep_time = 1.0
         self._app = app
 
     def run(self) -> None:
-        try:
-            while not self._exit_event.is_set():
-                self._exit_event.wait(self._sleep_time)
-                self.run_once()
-        except Exception as e:
-            raise e
+        while not self._exit_event.is_set():
+            self._exit_event.wait(self._sleep_time)
+            self.run_once()
 
     def run_once(self):
         for call_hash in list(self._app._schedules.keys()):
             metadata = self._app._schedules[call_hash]
             start_time = datetime.fromisoformat(metadata["start_time"])
             current_date = datetime.now()
             next_event = croniter(metadata["cron_pattern"], start_time).get_next(datetime)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/secrets.py` & `lightning-app-2.0.3/src/lightning_app/utilities/secrets.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/state.py` & `lightning-app-2.0.3/src/lightning_app/utilities/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,18 +119,15 @@
                 app_ip = app_instance.status.ip_address
 
             # TODO: Don't hard code port 8080 here
             self._host = f"http://{app_ip}:8080" if app_ip else APP_SERVER_HOST
         return f"{self._host}:{self._port}" if self._use_localhost else self._host
 
     def _attach_plugin(self, plugin: Optional[BaseStatePlugin]) -> None:
-        if plugin is not None:
-            plugin = plugin
-        else:
-            plugin = AppStatePlugin()
+        plugin = plugin if plugin is not None else AppStatePlugin()
         self._plugin = plugin
 
     @staticmethod
     def _find_state_under_affiliation(state, my_affiliation: Tuple[str, ...]) -> Dict[str, Any]:
         """This method is used to extract the subset of the app state associated with the given affiliation.
 
         For example, if the affiliation is ``("root", "subflow")``, then the returned state will be
@@ -165,16 +162,16 @@
         # TODO: Find how to prevent the infinite loop on refresh without storing the DeepDiff
         if self._plugin.should_update_app(deep_diff):
             data = {"delta": json.loads(deep_diff.to_json())}
             headers = headers_for(self._plugin.get_context())
             try:
                 # TODO: Send the delta directly to the REST API.
                 response = self._session.post(app_url, json=data, headers=headers)
-            except ConnectionError as e:
-                raise AttributeError("Failed to connect and send the app state. Is the app running?") from e
+            except ConnectionError as ex:
+                raise AttributeError("Failed to connect and send the app state. Is the app running?") from ex
 
             if response and response.status_code != 200:
                 raise Exception(f"The response from the server was {response.status_code}. Your inputs were rejected.")
 
     def _request_state(self) -> None:
         if self._state is not None:
             return
@@ -185,16 +182,16 @@
 
         # Sometimes the state URL can return an empty JSON when things are being set-up,
         # so we wait for it to be ready here.
         while response_json == {}:
             sleep(0.5)
             try:
                 response = self._session.get(app_url, headers=headers, timeout=1)
-            except ConnectionError as e:
-                raise AttributeError("Failed to connect and fetch the app state. Is the app running?") from e
+            except ConnectionError as ex:
+                raise AttributeError("Failed to connect and fetch the app state. Is the app running?") from ex
 
             self._authorized = response.status_code
             if self._authorized != 200:
                 return
 
             response_json = response.json()
 
@@ -210,28 +207,28 @@
 
         if name in self._state.get("vars", {}):
             value = self._state["vars"][name]
             if isinstance(value, dict):
                 return _maybe_create_drive("root." + ".".join(self._my_affiliation), value)
             return value
 
-        elif name in self._state.get("works", {}):
+        if name in self._state.get("works", {}):
             return AppState(
                 self._host, self._port, last_state=self._last_state["works"][name], state=self._state["works"][name]
             )
 
-        elif name in self._state.get("flows", {}):
+        if name in self._state.get("flows", {}):
             return AppState(
                 self._host,
                 self._port,
                 last_state=self._last_state["flows"][name],
                 state=self._state["flows"][name],
             )
 
-        elif name in self._state.get("structures", {}):
+        if name in self._state.get("structures", {}):
             return AppState(
                 self._host,
                 self._port,
                 last_state=self._last_state["structures"][name],
                 state=self._state["structures"][name],
             )
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/tracer.py` & `lightning-app-2.0.3/src/lightning_app/utilities/tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,18 +71,15 @@
         trace_entry["default_args"] = get_default_args(fn)
 
         # we cache also the parameters used during the function call
         trace_entry["call_args"] = kwargs
 
         trace_entry["call"] = {"start": time.time_ns()}
 
-        if not is_class_method:
-            ret = fn(self, *args, **kwargs)
-        else:
-            ret = fn(*args, **kwargs)
+        ret = fn(self, *args, **kwargs) if not is_class_method else fn(*args, **kwargs)
 
         trace_entry["call"]["end"] = time.time_ns()
 
         if post_fn:
             # If a post_fn is specified, it can both record information
             # in a trace, as well as modify the value returned from fn
             post_trace, ret = post_fn(self, ret)
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/tree.py` & `lightning-app-2.0.3/src/lightning_app/utilities/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """Utilities for traversing the tree of components in an app."""
 from typing import Type, TYPE_CHECKING
 
 import lightning_app
 
 if TYPE_CHECKING:
     from lightning_app.utilities.types import Component, ComponentTuple
```

### Comparing `lightning-app-2.0.2/src/lightning_app/utilities/warnings.py` & `lightning-app-2.0.3/src/lightning_app/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.2/src/lightning_app.egg-info/PKG-INFO` & `lightning-app-2.0.3/src/lightning_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.2
+Version: 2.0.3
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,18 +21,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: components
-Provides-Extra: test
 Provides-Extra: ui
+Provides-Extra: components
 Provides-Extra: cloud
+Provides-Extra: test
 Provides-Extra: extra
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.2 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.3 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
 Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
 Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
@@ -10,17 +10,17 @@
 Language :: English Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: components Provides-Extra: test
-Provides-Extra: ui Provides-Extra: cloud Provides-Extra: extra Provides-Extra:
-all Provides-Extra: dev License-File: LICENSE
+Content-Type: text/markdown Provides-Extra: ui Provides-Extra: components
+Provides-Extra: cloud Provides-Extra: test Provides-Extra: extra Provides-
+Extra: all Provides-Extra: dev License-File: LICENSE
  [https://pl-flash-data.s3.amazonaws.com/brandmark.png] **With Lightning Apps,
 you build exactly what you need: from production-ready, multi-cloud ML systems
                           to simple research demos.**
     ______________________________________________________________________
             Website â¢ Docs â¢ Getting_started â¢ Help â¢ Slack
        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 lightning_app)](https://pypi.org/project/lightning_app/) [![PyPI Status](https:
```

### Comparing `lightning-app-2.0.2/src/lightning_app.egg-info/SOURCES.txt` & `lightning-app-2.0.3/src/lightning_app.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 README.md
 pyproject.toml
 setup.py
 .actions/assistant.py
 requirements/app/base.txt
 requirements/app/cloud.txt
 requirements/app/components.txt
-requirements/app/devel.txt
 requirements/app/docs.txt
 requirements/app/test.txt
 requirements/app/ui.txt
 src/version.info
 src/lightning_app/CHANGELOG.md
 src/lightning_app/MANIFEST.in
 src/lightning_app/README.md
 src/lightning_app/__about__.py
 src/lightning_app/__init__.py
 src/lightning_app/__main__.py
 src/lightning_app/__setup__.py
 src/lightning_app/__version__.py
+src/lightning_app/py.typed
 src/lightning_app/version.info
 src/lightning_app.egg-info/PKG-INFO
 src/lightning_app.egg-info/SOURCES.txt
 src/lightning_app.egg-info/dependency_links.txt
 src/lightning_app.egg-info/entry_points.txt
 src/lightning_app.egg-info/not-zip-safe
 src/lightning_app.egg-info/requires.txt
```

### Comparing `lightning-app-2.0.2/src/lightning_app.egg-info/requires.txt` & `lightning-app-2.0.3/src/lightning_app.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 traitlets<6.0,>=5.3.0
 arrow<2.0,>=1.2.0
 lightning-utilities<1.0,>=0.7.0
 beautifulsoup4<5.0,>=4.8.0
 inquirer<4.0,>=2.10.0
 psutil<6.0
 click<9.0
+python-multipart<1.0,>=0.0.5
 fastapi<0.89.0,>=0.69.0
 starlette
 pydantic<3.0,>=1.7.4
 dateutils<1.0
 Jinja2<4.0
 PyYAML<7.0
 requests<3.0
@@ -53,21 +54,22 @@
 s3fs<2023.0,>=2022.5.0
 streamlit<2.0,>=1.13.0
 panel<1.0,>=0.12.7
 lightning_api_access>=0.0.3
 aiohttp<4.0,>=3.8.0
 lightning-fabric>=1.9.0
 pytorch-lightning>=1.9.0
-coverage==6.5.0
-pytest==7.2.0
+coverage==7.2.5
+pytest==7.3.1
 pytest-timeout==2.1.0
 pytest-cov==4.0.0
 pytest-doctestplus>=0.9.0
 pytest-asyncio==0.20.3
-playwright==1.30.0
+pytest-rerunfailures<12.0
+playwright==1.32.1
 httpx
 trio<0.22.0
 pympler
 psutil
 setuptools<68.0
 requests-mock
 
@@ -79,21 +81,22 @@
 panel<1.0,>=0.12.7
 lightning_api_access>=0.0.3
 aiohttp<4.0,>=3.8.0
 lightning-fabric>=1.9.0
 pytorch-lightning>=1.9.0
 
 [test]
-coverage==6.5.0
-pytest==7.2.0
+coverage==7.2.5
+pytest==7.3.1
 pytest-timeout==2.1.0
 pytest-cov==4.0.0
 pytest-doctestplus>=0.9.0
 pytest-asyncio==0.20.3
-playwright==1.30.0
+pytest-rerunfailures<12.0
+playwright==1.32.1
 httpx
 trio<0.22.0
 pympler
 psutil
 setuptools<68.0
 requests-mock
```

