# Comparing `tmp/ethpm-types-0.5.2.tar.gz` & `tmp/ethpm-types-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethpm-types-0.5.2.tar", last modified: Thu Jun  1 20:02:29 2023, max compression
+gzip compressed data, was "ethpm-types-0.5.3.tar", last modified: Wed Jun  7 21:02:35 2023, max compression
```

## Comparing `ethpm-types-0.5.2.tar` & `ethpm-types-0.5.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.505046 ethpm-types-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-01 20:02:29.505046 ethpm-types-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/methoddocs/abi.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/methoddocs/contract_type.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/methoddocs/manifest.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/methoddocs/source.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/ethpm_types/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/sourcemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/ethpm_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.489046 ethpm-types-0.5.2/ethpm_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 20:02:29.000000 ethpm-types-0.5.2/ethpm_types.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 20:02:29.505046 ethpm-types-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.493046 ethpm-types-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.485046 ethpm-types-0.5.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.505046 ethpm-types-0.5.2/tests/data/Compiled/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/HasError.json
--rw-r--r--   0 runner    (1001) docker     (123) 12327472 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/OpenZeppelinContracts.json
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/SolFallbackAndReceive.json
--rw-r--r--   0 runner    (1001) docker     (123)   227889 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/SolidityContract.json
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/TestStrategy.srcmap
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/VyDefault.json
--rw-r--r--   0 runner    (1001) docker     (123)   230644 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Compiled/VyperContract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:29.505046 ethpm-types-0.5.2/tests/data/Sources/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Sources/SolFallbackAndReceive.sol
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Sources/SolidityContract.sol
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Sources/VyDefault.vy
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/data/Sources/VyperContract.vy
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_cairo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_hexbytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_package_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_pc_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_schema_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-01 20:02:07.000000 ethpm-types-0.5.2/tests/test_sourcemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.762037 ethpm-types-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.738036 ethpm-types-0.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.738036 ethpm-types-0.5.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.738036 ethpm-types-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-07 21:02:35.762037 ethpm-types-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.738036 ethpm-types-0.5.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.738036 ethpm-types-0.5.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.738036 ethpm-types-0.5.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.738036 ethpm-types-0.5.3/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/methoddocs/abi.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/methoddocs/contract_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/methoddocs/manifest.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/methoddocs/source.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.738036 ethpm-types-0.5.3/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.742037 ethpm-types-0.5.3/ethpm_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/ethpm_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/ethpm_types/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/ethpm_types/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/ethpm_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/ethpm_types/contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/ethpm_types/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/ethpm_types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/ethpm_types/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/ethpm_types/sourcemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/ethpm_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 21:02:35.000000 ethpm-types-0.5.3/ethpm_types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.742037 ethpm-types-0.5.3/ethpm_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-07 21:02:35.000000 ethpm-types-0.5.3/ethpm_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-07 21:02:35.000000 ethpm-types-0.5.3/ethpm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:02:35.000000 ethpm-types-0.5.3/ethpm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:02:35.000000 ethpm-types-0.5.3/ethpm_types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-07 21:02:35.000000 ethpm-types-0.5.3/ethpm_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 21:02:35.000000 ethpm-types-0.5.3/ethpm_types.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-07 21:02:35.766037 ethpm-types-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.742037 ethpm-types-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.734037 ethpm-types-0.5.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.762037 ethpm-types-0.5.3/tests/data/Compiled/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Compiled/HasError.json
+-rw-r--r--   0 runner    (1001) docker     (123) 12327472 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Compiled/OpenZeppelinContracts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Compiled/SolFallbackAndReceive.json
+-rw-r--r--   0 runner    (1001) docker     (123)   227889 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Compiled/SolidityContract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Compiled/TestStrategy.srcmap
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Compiled/VyDefault.json
+-rw-r--r--   0 runner    (1001) docker     (123)   230644 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Compiled/VyperContract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:02:35.762037 ethpm-types-0.5.3/tests/data/Sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Sources/SolFallbackAndReceive.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Sources/SolidityContract.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Sources/VyDefault.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/data/Sources/VyperContract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/test_cairo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/test_contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/test_hexbytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/test_package_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/test_pc_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/test_schema_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-07 21:02:04.000000 ethpm-types-0.5.3/tests/test_sourcemap.py
```

### Comparing `ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/bug.md` & `ethpm-types-0.5.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/feature.md` & `ethpm-types-0.5.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/.github/ISSUE_TEMPLATE/work-item.md` & `ethpm-types-0.5.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/.github/release-drafter.yml` & `ethpm-types-0.5.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/.github/workflows/commitlint.yaml` & `ethpm-types-0.5.3/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/.github/workflows/docs.yaml` & `ethpm-types-0.5.3/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/.github/workflows/prtitle.yaml` & `ethpm-types-0.5.3/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/.github/workflows/publish.yaml` & `ethpm-types-0.5.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/.github/workflows/test.yaml` & `ethpm-types-0.5.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/.gitignore` & `ethpm-types-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/.pre-commit-config.yaml` & `ethpm-types-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/CONTRIBUTING.md` & `ethpm-types-0.5.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/LICENSE` & `ethpm-types-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/PKG-INFO` & `ethpm-types-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.5.2
+Version: 0.5.3
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ethpm-types-0.5.2/README.md` & `ethpm-types-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/build_docs.py` & `ethpm-types-0.5.3/build_docs.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/docs/_static/custom.css` & `ethpm-types-0.5.3/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/docs/_static/custom.js` & `ethpm-types-0.5.3/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/docs/_templates/layout.html` & `ethpm-types-0.5.3/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/docs/conf.py` & `ethpm-types-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/docs/favicon.ico` & `ethpm-types-0.5.3/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/docs/logo.gif` & `ethpm-types-0.5.3/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/ethpm_types/__init__.py` & `ethpm-types-0.5.3/ethpm_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/ethpm_types/abi.py` & `ethpm-types-0.5.3/ethpm_types/abi.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/ethpm_types/ast.py` & `ethpm-types-0.5.3/ethpm_types/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,19 @@
     """Unclassified AST type (default)."""
 
     FUNCTION = 1
     """ASTTypes related to defining a function."""
 
 
 class ASTNode(BaseModel):
+    name: Optional[str] = None
+    """
+    The node's name if it has one, such as a function name.
+    """
+
     ast_type: str
     """
     The compiler-given AST node type, such as ``FunctionDef``.
     """
 
     classification: ASTClassification = ASTClassification.UNCLASSIFIED
     """
```

### Comparing `ethpm-types-0.5.2/ethpm_types/base.py` & `ethpm-types-0.5.3/ethpm_types/base.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/ethpm_types/contract_type.py` & `ethpm-types-0.5.3/ethpm_types/contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/ethpm_types/manifest.py` & `ethpm-types-0.5.3/ethpm_types/manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/ethpm_types/source.py` & `ethpm-types-0.5.3/ethpm_types/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -324,14 +324,17 @@
     """
     A wrapper around code ran, such as a function.
     """
 
     name: str
     """The name of the definition."""
 
+    full_name: Optional[str] = None
+    """This is a unique name of the definition."""
+
 
 class Function(Closure):
     """
     Data about a function in a contract with known source code.
     """
 
     ast: ASTNode
@@ -372,15 +375,15 @@
         Args:
             location (``SourceLocation``): The location of the content.
 
         Returns:
             ``ethpm_types.source.Content``
         """
 
-        start = max(location[0], self.offset)
+        start = max(location[0], self.content.begin_lineno)
         stop = location[2] + 1
         content = {n: self.content[n] for n in range(start, stop) if n in self.content.line_numbers}
         return Content(__root__=content)
 
     def get_content_asts(self, location: SourceLocation) -> List[ASTNode]:
         """
         Get all AST nodes for the given location.
@@ -600,67 +603,71 @@
         if not ast:
             return None
 
         signature_lines, content_lines = self._parse_function(ast)
         if not signature_lines or not content_lines:
             return None
 
-        offset = ast.lineno + len(signature_lines)
+        signature_start = ast.lineno
+        offset = signature_start + len(signature_lines)
 
         # Check if method ID points to a calling method.
         name = None
+        full_name = None
         if method_id and method_id.hex() in self._function_ast_cache:
             cached_fn = self._function_ast_cache[method_id.hex()]
             if (
                 cached_fn.lineno == ast.lineno
                 and cached_fn.end_lineno == ast.end_lineno
                 and method_id in self.contract_type.methods
             ):
                 # Is the same function. It's safe to use the method ABI name.
                 method = self.contract_type.methods[method_id]
                 name = method.name
+                full_name = method.selector
 
         elif method_id and method_id in self.contract_type.methods:
             # Not in cache yet. Assume is calling.
             method = self.contract_type.methods[method_id]
             name = method.name
+            full_name = method.selector
             self._function_ast_cache[method_id.hex()] = ast
 
+        elif ast.name is not None:
+            # Use the AST name.
+            name = ast.name
+            full_name = _strip_function(signature_lines)
+
         if name is None:
             # This method is not present in the ABI, maybe because it is internal.
+            # Also, the name is missing from the AST node.
             # Combine the signature lines into a single string.
-            name = "".join([x.strip() for x in signature_lines]).rstrip()
-
-            # Strip off any common function definition prefixes, if found.
-            # def my_method -> my_method
-            common_prefixes = ("def ", "function ", "fn ", "func ")
-            for prefix in common_prefixes:
-                if not name.startswith(prefix):
-                    continue
-
-                name = name.split(prefix)[-1]
+            full_name = _strip_function(signature_lines)
+            name = full_name
 
             # If it looks like arguments are defined in parenthesis, remove those.
             # my_method(123) -> my_method
             if (
                 "(" in name
                 and ")" in name
-                and name.index("(") < len(name) - 1 - name[::-1].index(")")
+                and full_name.index("(") < len(name) - 1 - name[::-1].index(")")
             ):
-                name = name.split("(")[0]
+                name = full_name.split("(")[0]
 
+        signature_dict = {signature_start + i: ln for i, ln in enumerate(signature_lines)}
         content_dict = {offset + i: ln for i, ln in enumerate(content_lines)}
-        content = Content(__root__=content_dict)
+        content = Content(__root__={**signature_dict, **content_dict})
         Function.update_forward_refs()
 
         return Function(
             ast=ast,
+            content=content,
+            full_name=full_name,
             name=name,
             offset=offset,
-            content=content,
         )
 
     def _parse_function(self, function: ASTNode) -> Tuple[List[str], List[str]]:
         """
         Parse function AST into two groups. One being the list of
         lines making up the signature and the other being the content
         lines of the function.
@@ -682,7 +689,22 @@
 
         if content_start is None:
             # Shouldn't happen, but just in case, use only the first line.
             content_start = function.lineno + 1
 
         offset = content_start - function.lineno
         return lines[:offset], lines[offset:]
+
+
+def _strip_function(signature_lines: List[str]) -> str:
+    name = "".join([x.strip() for x in signature_lines]).rstrip()
+
+    # Strip off any common function definition prefixes, if found.
+    # def my_method -> my_method
+    common_prefixes = ("def ", "function ", "fn ", "func ")
+    for prefix in common_prefixes:
+        if not name.startswith(prefix):
+            continue
+
+        name = name.split(prefix)[-1]
+
+    return name.rstrip(":{ \n")
```

### Comparing `ethpm-types-0.5.2/ethpm_types/sourcemap.py` & `ethpm-types-0.5.3/ethpm_types/sourcemap.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/ethpm_types/utils.py` & `ethpm-types-0.5.3/ethpm_types/utils.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/ethpm_types.egg-info/PKG-INFO` & `ethpm-types-0.5.3/ethpm_types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.5.2
+Version: 0.5.3
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ethpm-types-0.5.2/ethpm_types.egg-info/SOURCES.txt` & `ethpm-types-0.5.3/ethpm_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/ethpm_types.egg-info/requires.txt` & `ethpm-types-0.5.3/ethpm_types.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/pyproject.toml` & `ethpm-types-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/setup.py` & `ethpm-types-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/conftest.py` & `ethpm-types-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/data/Compiled/HasError.json` & `ethpm-types-0.5.3/tests/data/Compiled/HasError.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/data/Compiled/OpenZeppelinContracts.json` & `ethpm-types-0.5.3/tests/data/Compiled/OpenZeppelinContracts.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/data/Compiled/SolFallbackAndReceive.json` & `ethpm-types-0.5.3/tests/data/Compiled/SolFallbackAndReceive.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/data/Compiled/SolidityContract.json` & `ethpm-types-0.5.3/tests/data/Compiled/SolidityContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/data/Compiled/TestStrategy.srcmap` & `ethpm-types-0.5.3/tests/data/Compiled/TestStrategy.srcmap`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/data/Compiled/VyDefault.json` & `ethpm-types-0.5.3/tests/data/Compiled/VyDefault.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/data/Compiled/VyperContract.json` & `ethpm-types-0.5.3/tests/data/Compiled/VyperContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/data/Sources/SolidityContract.sol` & `ethpm-types-0.5.3/tests/data/Sources/SolidityContract.sol`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/data/Sources/VyperContract.vy` & `ethpm-types-0.5.3/tests/data/Sources/VyperContract.vy`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/test_ast.py` & `ethpm-types-0.5.3/tests/test_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,14 +463,15 @@
     funcs = node.functions
     assert stmt.ast_type == "Compare"
     assert stmt.line_numbers == (7, 11, 7, 19)
     assert len(stmts) == 2
     assert stmts[0].ast_type == "arguments"
     assert stmts[1].ast_type == "arg"
     assert len(funcs) == 1
+    assert funcs[0].name == "setNumber"
     assert node.get_defining_function((7, 11, 7, 14)) == funcs[0]
     assert node.get_defining_function([7, 11, 7, 14]) == funcs[0]
     assert node.get_defining_function((55, 11, 56, 14)) is None
 
 
 def test_sol_ast():
     node = ASTNode.parse_obj(SOLIDITY_AST_JSON)
```

### Comparing `ethpm-types-0.5.2/tests/test_cairo.py` & `ethpm-types-0.5.3/tests/test_cairo.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/test_contract_type.py` & `ethpm-types-0.5.3/tests/test_contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/test_package_manifest.py` & `ethpm-types-0.5.3/tests/test_package_manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/test_pc_map.py` & `ethpm-types-0.5.3/tests/test_pc_map.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/test_schema_fuzzing.py` & `ethpm-types-0.5.3/tests/test_schema_fuzzing.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.2/tests/test_sourcemap.py` & `ethpm-types-0.5.3/tests/test_sourcemap.py`

 * *Files identical despite different names*

