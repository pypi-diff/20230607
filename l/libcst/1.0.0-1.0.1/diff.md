# Comparing `tmp/libcst-1.0.0.tar.gz` & `tmp/libcst-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcst-1.0.0.tar", last modified: Thu May 25 19:14:47 2023, max compression
+gzip compressed data, was "libcst-1.0.1.tar", last modified: Wed Jun  7 12:52:39 2023, max compression
```

## Comparing `libcst-1.0.0.tar` & `libcst-1.0.1.tar`

### file list

```diff
@@ -1,494 +1,494 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/.cargo/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-25 19:11:37.000000 libcst-1.0.0/.cargo/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-25 19:11:37.000000 libcst-1.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-25 19:11:37.000000 libcst-1.0.0/.fixit.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-25 19:11:37.000000 libcst-1.0.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 19:11:37.000000 libcst-1.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/build-matrix.json
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/workflows/pypi_upload.yml
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-25 19:11:37.000000 libcst-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-25 19:11:37.000000 libcst-1.0.0/.pyre_configuration
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-25 19:11:37.000000 libcst-1.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 19:11:37.000000 libcst-1.0.0/.watchmanconfig
--rw-r--r--   0 runner    (1001) docker     (123)    37188 2023-05-25 19:11:37.000000 libcst-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-25 19:11:37.000000 libcst-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-25 19:11:37.000000 libcst-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-25 19:11:37.000000 libcst-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-25 19:11:37.000000 libcst-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-05-25 19:14:47.966725 libcst-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-25 19:11:37.000000 libcst-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 19:11:37.000000 libcst-1.0.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.902724 libcst-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/docs/source/_static/img/
--rw-r--r--   0 runner    (1001) docker     (123)   108465 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/img/python_scopes.png
--rw-r--r--   0 runner    (1001) docker     (123)    30400 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/img/python_scopes.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.914724 libcst-1.0.0/docs/source/_static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/favicon_16px.png
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/favicon_32px.png
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/horizontal_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/horizontal_white_sidebar.png
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/icon_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/vertical.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/vertical_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.914724 libcst-1.0.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/best_practices.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/codemods.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/codemods_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/experimental.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/helpers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/matchers.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/matchers_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/metadata_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/motivation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/nodes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/parser.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/scope_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/visitors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15454 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/why_libcst.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.914724 libcst-1.0.0/libcst/
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_add_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_batched_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_flatten_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_maybe_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_metadata_dependent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.918724 libcst-1.0.0/libcst/_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (123)   140091 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    31193 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/op.py
--rw-r--r--   0 runner    (1001) docker     (123)   131179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.926724 libcst-1.0.0/libcst/_nodes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_assert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_await.py
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_binary_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_boolean_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    22698 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_classdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_cst_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_del.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_dict_comp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_else.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_empty_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_flatten_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_for.py
--rw-r--r--   0 runner    (1001) docker     (123)    94136 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_funcdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_ifexp.py
--rw-r--r--   0 runner    (1001) docker     (123)    29777 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_indented_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    40077 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_leaf_small_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    22302 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_matrix_multiply.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_namedexpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_newline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_nonlocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_removal_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_simple_comp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_simple_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_simple_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_simple_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_small_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_subscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_trailing_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25792 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_try.py
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_unary_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_while.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_yield.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/whitespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.926724 libcst-1.0.0/libcst/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/base_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.926724 libcst-1.0.0/libcst/_parser/conversions/
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53078 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/params.py
--rw-r--r--   0 runner    (1001) docker     (123)    47301 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/terminals.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/custom_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/detect_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.926724 libcst-1.0.0/libcst/_parser/parso/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/parso/pgen2/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/pgen2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/pgen2/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/pgen2/grammar_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/parso/python/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/python/py_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/python/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    44145 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/python/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/parso/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/tests/test_fstring.py
--rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/production_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/py_whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/python_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_detect_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_footer_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_node_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_parse_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_version_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    83462 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_wrapped_tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/types/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/partials.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/py_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/py_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/py_whitespace_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/types/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/whitespace_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/wrapped_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_removal_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_type_enforce.py
--rw-r--r--   0 runner    (1001) docker     (123)   179734 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_typed_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_typed_visitor_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.934724 libcst-1.0.0/libcst/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/gen_matcher_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/gen_type_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/gen_visitor_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.934724 libcst-1.0.0/libcst/codegen/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/tests/test_codegen_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.934724 libcst-1.0.0/libcst/codemod/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24234 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_codemod.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_dummy_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.938724 libcst-1.0.0/libcst/codemod/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/add_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/add_trailing_commas.py
--rw-r--r--   0 runner    (1001) docker     (123)    16027 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/convert_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/convert_namedtuple_to_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/convert_percent_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (123)    32680 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/convert_type_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/ensure_import_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/fix_pyre_directives.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/remove_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/strip_strings_from_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.938724 libcst-1.0.0/libcst/codemod/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_add_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_add_trailing_commas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_convert_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_convert_type_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_ensure_import_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_fix_pyre_directives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_remove_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_strip_strings_from_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_unnecessary_format_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/unnecessary_format_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.938724 libcst-1.0.0/libcst/codemod/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/codemod_formatter_error_input.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/test_codemod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/test_codemod_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.942724 libcst-1.0.0/libcst/codemod/visitors/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17425 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_add_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    50584 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_apply_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_global_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_string_annotation_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    20494 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_remove_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.942724 libcst-1.0.0/libcst/codemod/visitors/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_add_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    54487 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_apply_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_global_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    23816 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_remove_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.942724 libcst-1.0.0/libcst/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19403 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.942724 libcst-1.0.0/libcst/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/tests/test_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.946725 libcst-1.0.0/libcst/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)   534993 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    81855 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/_matcher_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/_return_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    34798 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.950724 libcst-1.0.0/libcst/matchers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35211 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_findall.py
--rw-r--r--   0 runner    (1001) docker     (123)    53908 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_matchers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_matchers_with_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)    20190 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.950724 libcst-1.0.0/libcst/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/accessor_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/expression_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/file_path_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/full_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/name_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/parent_node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/position_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/reentrant_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/span_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/libcst/metadata/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_accessor_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_base_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_expression_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_file_path_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_full_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_metadata_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_metadata_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19965 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_name_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_parent_node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_position_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_reentrant_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    75819 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_span_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_type_inference_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/type_inference_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/libcst/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/libcst/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/libcst/tests/pyre/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/pyre/.pyre_configuration
--rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/pyre/simple_class.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/pyre/simple_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_add_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_batched_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_deep_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_deep_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_fuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_pyre_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25336 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_type_enforce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31223 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.918724 libcst-1.0.0/libcst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/native/
--rw-r--r--   0 runner    (1001) docker     (123)    25856 2023-05-25 19:11:37.000000 libcst-1.0.0/native/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 19:11:37.000000 libcst-1.0.0/native/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/native/libcst/
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    32411 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/Grammar
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.958725 libcst-1.0.0/native/libcst/benches/
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/benches/parser_benchmark.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.958725 libcst-1.0.0/native/libcst/src/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/bin.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.958725 libcst-1.0.0/native/libcst/src/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/codegen.rs
--rw-r--r--   0 runner    (1001) docker     (123)    80125 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/expression.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/inflate_helpers.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/macros.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/module.rs
--rw-r--r--   0 runner    (1001) docker     (123)    50731 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/op.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/parser_config.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/py_cached.rs
--rw-r--r--   0 runner    (1001) docker     (123)   104571 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/statement.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/test_utils.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/traits.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/whitespace.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.958725 libcst-1.0.0/native/libcst/src/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/parser/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)   109927 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/parser/grammar.rs
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/parser/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/parser/numbers.rs
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/py.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.958725 libcst-1.0.0/native/libcst/src/tokenizer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.962725 libcst-1.0.0/native/libcst/src/tokenizer/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/core/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/core/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    49644 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/core/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/core/string_types.rs
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/debug_utils.rs
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/operators.rs
--rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/tests.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.962725 libcst-1.0.0/native/libcst/src/tokenizer/text_position/
--rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/text_position/char_width.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/text_position/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/whitespace_parser.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.962725 libcst-1.0.0/native/libcst/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.962725 libcst-1.0.0/native/libcst/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/big_binary_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/class_craziness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/dangling_indent.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/decorated_function_without_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/dysfunctional_del.py
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/expr_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/fun_with_func_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/global_nonlocal.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/import.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/indents_but_no_eol_before_eof.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/just_a_comment_without_nl.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/malicious_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/pep646.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/raise.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/smol_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/spacious_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/starry_tries.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/suicidal_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/super_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/terrible_tries.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/trailing_comment_without_nl.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/tuple_shenanigans.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/vast_emptiness.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/with_wickedness.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/wonky_walrus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/parser_roundtrip.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.962725 libcst-1.0.0/native/libcst_derive/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/native/libcst_derive/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/codegen.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/cstnode.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/inflate.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/into_py.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/parenthesized_node.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.906724 libcst-1.0.0/native/libcst_derive/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/native/libcst_derive/tests/pass/
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/tests/pass/minimal_cst.rs
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/tests/pass/simple.rs
--rwxr-xr-x   0 runner    (1001) docker     (123)      270 2023-05-25 19:11:37.000000 libcst-1.0.0/native/roundtrip.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-25 19:11:37.000000 libcst-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-25 19:11:37.000000 libcst-1.0.0/scripts/check_copyright.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-25 19:11:37.000000 libcst-1.0.0/scripts/regenerate-fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:14:47.966725 libcst-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-25 19:11:37.000000 libcst-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/hypothesis.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/hypothesmith.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/stubs/libcst/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst/native.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/stubs/libcst_native/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst_native/parser_config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst_native/token_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst_native/tokenize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst_native/whitespace_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst_native/whitespace_state.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/setuptools.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/tokenize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/typing_inspect.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.549510 libcst-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.461506 libcst-1.0.1/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-07 12:48:36.000000 libcst-1.0.1/.cargo/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-07 12:48:36.000000 libcst-1.0.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-07 12:48:36.000000 libcst-1.0.1/.fixit.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-07 12:48:36.000000 libcst-1.0.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 12:48:36.000000 libcst-1.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.461506 libcst-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 12:48:36.000000 libcst-1.0.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-07 12:48:36.000000 libcst-1.0.1/.github/build-matrix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-07 12:48:36.000000 libcst-1.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.461506 libcst-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-07 12:48:36.000000 libcst-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-07 12:48:36.000000 libcst-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-07 12:48:36.000000 libcst-1.0.1/.github/workflows/pypi_upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-07 12:48:36.000000 libcst-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-07 12:48:36.000000 libcst-1.0.1/.pyre_configuration
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-07 12:48:36.000000 libcst-1.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-07 12:48:36.000000 libcst-1.0.1/.watchmanconfig
+-rw-r--r--   0 runner    (1001) docker     (123)    38090 2023-06-07 12:48:36.000000 libcst-1.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-07 12:48:36.000000 libcst-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-07 12:48:36.000000 libcst-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-07 12:48:36.000000 libcst-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-07 12:48:36.000000 libcst-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-06-07 12:52:39.549510 libcst-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-06-07 12:48:36.000000 libcst-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-07 12:48:36.000000 libcst-1.0.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.445505 libcst-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.465506 libcst-1.0.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.465506 libcst-1.0.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.465506 libcst-1.0.1/docs/source/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   108465 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/img/python_scopes.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30400 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/img/python_scopes.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.469506 libcst-1.0.1/docs/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/logo/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/logo/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/logo/favicon_16px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/logo/favicon_32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/logo/horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/logo/horizontal_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/logo/horizontal_white_sidebar.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/logo/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/logo/icon_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/logo/vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_static/logo/vertical_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.469506 libcst-1.0.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/best_practices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/codemods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/codemods_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/experimental.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/matchers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/matchers_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/metadata_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/parser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/scope_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/visitors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15454 2023-06-07 12:48:36.000000 libcst-1.0.1/docs/source/why_libcst.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.473506 libcst-1.0.1/libcst/
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_add_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_batched_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_flatten_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_maybe_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_metadata_dependent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.477506 libcst-1.0.1/libcst/_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141899 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31193 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131354 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.489507 libcst-1.0.1/libcst/_nodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_assert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_await.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_binary_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_boolean_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22698 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_classdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_cst_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_dict_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_else.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_empty_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_flatten_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94136 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_funcdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_ifexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29777 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_indented_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40904 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_leaf_small_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22302 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_matrix_multiply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_namedexpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_newline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_nonlocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_removal_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_simple_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_simple_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_simple_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_simple_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_small_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_trailing_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25792 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_try.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_unary_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_while.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/tests/test_yield.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_nodes/whitespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.489507 libcst-1.0.1/libcst/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/base_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.493507 libcst-1.0.1/libcst/_parser/conversions/
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/conversions/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53078 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/conversions/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/conversions/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/conversions/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47301 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/conversions/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/conversions/terminals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/custom_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/detect_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.493507 libcst-1.0.1/libcst/_parser/parso/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.493507 libcst-1.0.1/libcst/_parser/parso/pgen2/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/pgen2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/pgen2/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/pgen2/grammar_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.493507 libcst-1.0.1/libcst/_parser/parso/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/python/py_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/python/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44145 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/python/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.493507 libcst-1.0.1/libcst/_parser/parso/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/tests/test_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/parso/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/production_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/py_whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/python_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.497507 libcst-1.0.1/libcst/_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/tests/test_detect_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/tests/test_footer_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/tests/test_node_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/tests/test_parse_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/tests/test_version_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/tests/test_whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83462 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/tests/test_wrapped_tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.497507 libcst-1.0.1/libcst/_parser/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/partials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/py_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/py_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/py_whitespace_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.497507 libcst-1.0.1/libcst/_parser/types/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/types/whitespace_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_parser/wrapped_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_removal_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_type_enforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)   186896 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_typed_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_typed_visitor_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 12:52:39.000000 libcst-1.0.1/libcst/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.501507 libcst-1.0.1/libcst/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codegen/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codegen/gen_matcher_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codegen/gen_type_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codegen/gen_visitor_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codegen/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.501507 libcst-1.0.1/libcst/codegen/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codegen/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codegen/tests/test_codegen_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codegen/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.501507 libcst-1.0.1/libcst/codemod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/_dummy_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/_visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.505508 libcst-1.0.1/libcst/codemod/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/add_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/add_trailing_commas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16027 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/convert_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/convert_namedtuple_to_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/convert_percent_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32680 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/convert_type_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/ensure_import_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/fix_pyre_directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/remove_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/strip_strings_from_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.509508 libcst-1.0.1/libcst/codemod/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_add_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_add_trailing_commas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_convert_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_convert_type_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_ensure_import_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_fix_pyre_directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_remove_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_strip_strings_from_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/tests/test_unnecessary_format_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/commands/unnecessary_format_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.509508 libcst-1.0.1/libcst/codemod/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/tests/codemod_formatter_error_input.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/tests/test_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/tests/test_codemod_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.513508 libcst-1.0.1/libcst/codemod/visitors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17425 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/_add_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50584 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/_apply_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/_gather_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/_gather_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/_gather_global_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/_gather_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/_gather_string_annotation_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/_gather_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20494 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/_remove_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.513508 libcst-1.0.1/libcst/codemod/visitors/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/tests/test_add_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54487 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/tests/test_apply_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_global_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23816 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/codemod/visitors/tests/test_remove_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.517508 libcst-1.0.1/libcst/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19403 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/helpers/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/helpers/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/helpers/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/helpers/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.517508 libcst-1.0.1/libcst/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/helpers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/helpers/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/helpers/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/helpers/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/helpers/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.517508 libcst-1.0.1/libcst/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)   550740 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81855 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/_matcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/_return_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34798 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.521509 libcst-1.0.1/libcst/matchers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35211 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/tests/test_findall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53908 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/tests/test_matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/tests/test_matchers_with_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/tests/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20190 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/matchers/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.525509 libcst-1.0.1/libcst/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/accessor_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/expression_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/file_path_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/full_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/name_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/parent_node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/position_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/reentrant_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/span_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.529509 libcst-1.0.1/libcst/metadata/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_accessor_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_expression_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_file_path_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_full_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_metadata_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_metadata_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19965 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_name_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_parent_node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_position_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_reentrant_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75819 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_span_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/tests/test_type_inference_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/type_inference_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/metadata/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.529509 libcst-1.0.1/libcst/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.529509 libcst-1.0.1/libcst/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.529509 libcst-1.0.1/libcst/tests/pyre/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/pyre/.pyre_configuration
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/pyre/simple_class.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/pyre/simple_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_add_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_batched_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_deep_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_deep_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_pyre_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25336 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_type_enforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tests/test_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31223 2023-06-07 12:48:36.000000 libcst-1.0.1/libcst/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.473506 libcst-1.0.1/libcst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-06-07 12:52:39.000000 libcst-1.0.1/libcst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-06-07 12:52:39.000000 libcst-1.0.1/libcst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:52:39.000000 libcst-1.0.1/libcst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:52:39.000000 libcst-1.0.1/libcst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-07 12:52:39.000000 libcst-1.0.1/libcst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 12:52:39.000000 libcst-1.0.1/libcst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.533509 libcst-1.0.1/native/
+-rw-r--r--   0 runner    (1001) docker     (123)    25856 2023-06-07 12:48:36.000000 libcst-1.0.1/native/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 12:48:36.000000 libcst-1.0.1/native/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.533509 libcst-1.0.1/native/libcst/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    32411 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/Grammar
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.533509 libcst-1.0.1/native/libcst/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/benches/parser_benchmark.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.533509 libcst-1.0.1/native/libcst/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/bin.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.537509 libcst-1.0.1/native/libcst/src/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/codegen.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    80125 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/expression.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/inflate_helpers.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/macros.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/module.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    50731 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/op.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/parser_config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/py_cached.rs
+-rw-r--r--   0 runner    (1001) docker     (123)   104571 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/statement.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/test_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/nodes/whitespace.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.537509 libcst-1.0.1/native/libcst/src/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/parser/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (123)   109933 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/parser/grammar.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/parser/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/parser/numbers.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/py.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.537509 libcst-1.0.1/native/libcst/src/tokenizer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.537509 libcst-1.0.1/native/libcst/src/tokenizer/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/tokenizer/core/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/tokenizer/core/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    49413 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/tokenizer/core/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/tokenizer/core/string_types.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/tokenizer/debug_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/tokenizer/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/tokenizer/operators.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    23365 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/tokenizer/tests.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.541509 libcst-1.0.1/native/libcst/src/tokenizer/text_position/
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/tokenizer/text_position/char_width.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/tokenizer/text_position/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/src/tokenizer/whitespace_parser.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.541509 libcst-1.0.1/native/libcst/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.545510 libcst-1.0.1/native/libcst/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/big_binary_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/class_craziness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/dangling_indent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/decorated_function_without_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/dysfunctional_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/expr_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/fun_with_func_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/global_nonlocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/import.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/indents_but_no_eol_before_eof.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/just_a_comment_without_nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/malicious_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/pep646.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/smol_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/spacious_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/starry_tries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/suicidal_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/super_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/terrible_tries.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/trailing_comment_without_nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/tuple_shenanigans.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/vast_emptiness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/with_wickedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/fixtures/wonky_walrus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst/tests/parser_roundtrip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.545510 libcst-1.0.1/native/libcst_derive/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst_derive/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.545510 libcst-1.0.1/native/libcst_derive/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst_derive/src/codegen.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst_derive/src/cstnode.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst_derive/src/inflate.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst_derive/src/into_py.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst_derive/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst_derive/src/parenthesized_node.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.457505 libcst-1.0.1/native/libcst_derive/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.545510 libcst-1.0.1/native/libcst_derive/tests/pass/
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst_derive/tests/pass/minimal_cst.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-07 12:48:36.000000 libcst-1.0.1/native/libcst_derive/tests/pass/simple.rs
+-rwxr-xr-x   0 runner    (1001) docker     (123)      270 2023-06-07 12:48:36.000000 libcst-1.0.1/native/roundtrip.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-07 12:48:36.000000 libcst-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.545510 libcst-1.0.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-07 12:48:36.000000 libcst-1.0.1/scripts/check_copyright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-07 12:48:36.000000 libcst-1.0.1/scripts/regenerate-fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:52:39.549510 libcst-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-07 12:48:36.000000 libcst-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.549510 libcst-1.0.1/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 12:48:36.000000 libcst-1.0.1/stubs/hypothesis.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 12:48:36.000000 libcst-1.0.1/stubs/hypothesmith.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.549510 libcst-1.0.1/stubs/libcst/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-07 12:48:36.000000 libcst-1.0.1/stubs/libcst/native.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:52:39.549510 libcst-1.0.1/stubs/libcst_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-07 12:48:36.000000 libcst-1.0.1/stubs/libcst_native/parser_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-07 12:48:36.000000 libcst-1.0.1/stubs/libcst_native/token_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-07 12:48:36.000000 libcst-1.0.1/stubs/libcst_native/tokenize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-07 12:48:36.000000 libcst-1.0.1/stubs/libcst_native/whitespace_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-07 12:48:36.000000 libcst-1.0.1/stubs/libcst_native/whitespace_state.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 12:48:36.000000 libcst-1.0.1/stubs/setuptools.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-07 12:48:36.000000 libcst-1.0.1/stubs/tokenize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 12:48:36.000000 libcst-1.0.1/stubs/typing_inspect.pyi
```

### Comparing `libcst-1.0.0/.flake8` & `libcst-1.0.1/.flake8`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/.github/build-matrix.json` & `libcst-1.0.1/.github/build-matrix.json`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/.github/workflows/build.yml` & `libcst-1.0.1/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -54,12 +54,12 @@
         with:
           working-directory: native
       - name: Disable scmtools local scheme
         if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
         run: >-
           echo LIBCST_NO_LOCAL_SCHEME=1 >> $GITHUB_ENV
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.12.3
+        uses: pypa/cibuildwheel@v2.13.0
       - uses: actions/upload-artifact@v3
         with:
           path: wheelhouse/*.whl
           name: wheels
```

### Comparing `libcst-1.0.0/.github/workflows/ci.yml` & `libcst-1.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/.github/workflows/pypi_upload.yml` & `libcst-1.0.1/.github/workflows/pypi_upload.yml`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/CHANGELOG.md` & `libcst-1.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# 1.0.1 - 2023-06-07
+
+## Fixed
+* Fix type of `evaluated_value` on string to allow bytes by @ljodal in https://github.com/Instagram/LibCST/pull/721
+* Fix Sentinal typo by @kit1980 in https://github.com/Instagram/LibCST/pull/948
+* Allow no whitespace after lambda body in certain cases by @zsol in https://github.com/Instagram/LibCST/pull/939
+* Fix whitespace, fstring, walrus related parse errors (#939, #938, #937,
+#936, #935, #934, #933, #932, #931) by @zsol in https://github.com/Instagram/LibCST/pull/940
+* Codemod CLI: Print diff only when there is a change by @kit1980 in https://github.com/Instagram/LibCST/pull/945
+
+## New Contributors
+* @ljodal made their first contribution in https://github.com/Instagram/LibCST/pull/721
+* @kit1980 made their first contribution in https://github.com/Instagram/LibCST/pull/948
+
+**Full Changelog**: https://github.com/Instagram/LibCST/compare/v1.0.0...v1.0.1
+
 # 1.0.0 - 2023-05-25
 
 The first major release of LibCST is essentially the same as 0.4.10, but using the
 newer, Rust-based parser implementation by default. The old, pure Python parser is
 scheduled for removal in the next (non-patch) release. Until then, it is available with
 the `LIBCST_PARSER_TYPE` environment variable set to `pure`.
```

### Comparing `libcst-1.0.0/CODE_OF_CONDUCT.md` & `libcst-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/CONTRIBUTING.md` & `libcst-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/LICENSE` & `libcst-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/PKG-INFO` & `libcst-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcst
-Version: 1.0.0
+Version: 1.0.1
 Summary: A concrete syntax tree with AST-like properties for Python 3.5, 3.6, 3.7, 3.8, 3.9, and 3.10 programs.
 License: All contributions towards LibCST are MIT licensed.
         
         Some Python files have been derived from the standard library and are therefore
         PSF licensed. Modifications on these files are dual licensed (both MIT and
         PSF). These files are:
```

### Comparing `libcst-1.0.0/README.rst` & `libcst-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/img/python_scopes.png` & `libcst-1.0.1/docs/source/_static/img/python_scopes.png`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/img/python_scopes.svg` & `libcst-1.0.1/docs/source/_static/img/python_scopes.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/logo/favicon.ico` & `libcst-1.0.1/docs/source/_static/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/logo/favicon.svg` & `libcst-1.0.1/docs/source/_static/logo/favicon.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/logo/favicon_16px.png` & `libcst-1.0.1/docs/source/_static/logo/favicon_16px.png`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/logo/favicon_32px.png` & `libcst-1.0.1/docs/source/_static/logo/favicon_32px.png`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/logo/horizontal.svg` & `libcst-1.0.1/docs/source/_static/logo/horizontal.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/logo/horizontal_white.svg` & `libcst-1.0.1/docs/source/_static/logo/horizontal_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/logo/horizontal_white_sidebar.png` & `libcst-1.0.1/docs/source/_static/logo/horizontal_white_sidebar.png`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/logo/icon.svg` & `libcst-1.0.1/docs/source/_static/logo/icon.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/logo/icon_white.svg` & `libcst-1.0.1/docs/source/_static/logo/icon_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/logo/vertical.svg` & `libcst-1.0.1/docs/source/_static/logo/vertical.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/_static/logo/vertical_white.svg` & `libcst-1.0.1/docs/source/_static/logo/vertical_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/best_practices.rst` & `libcst-1.0.1/docs/source/best_practices.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/codemods.rst` & `libcst-1.0.1/docs/source/codemods.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/codemods_tutorial.rst` & `libcst-1.0.1/docs/source/codemods_tutorial.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/conf.py` & `libcst-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/helpers.rst` & `libcst-1.0.1/docs/source/helpers.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/index.rst` & `libcst-1.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/matchers.rst` & `libcst-1.0.1/docs/source/matchers.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/matchers_tutorial.ipynb` & `libcst-1.0.1/docs/source/matchers_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/metadata.rst` & `libcst-1.0.1/docs/source/metadata.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/metadata_tutorial.ipynb` & `libcst-1.0.1/docs/source/metadata_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/motivation.rst` & `libcst-1.0.1/docs/source/motivation.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/nodes.rst` & `libcst-1.0.1/docs/source/nodes.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/parser.rst` & `libcst-1.0.1/docs/source/parser.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/scope_tutorial.ipynb` & `libcst-1.0.1/docs/source/scope_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/tutorial.ipynb` & `libcst-1.0.1/docs/source/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/visitors.rst` & `libcst-1.0.1/docs/source/visitors.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/docs/source/why_libcst.rst` & `libcst-1.0.1/docs/source/why_libcst.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/__init__.py` & `libcst-1.0.1/libcst/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_add_slots.py` & `libcst-1.0.1/libcst/_add_slots.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_batched_visitor.py` & `libcst-1.0.1/libcst/_batched_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_exceptions.py` & `libcst-1.0.1/libcst/_exceptions.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_flatten_sentinel.py` & `libcst-1.0.1/libcst/_flatten_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_maybe_sentinel.py` & `libcst-1.0.1/libcst/_maybe_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_metadata_dependent.py` & `libcst-1.0.1/libcst/_metadata_dependent.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/base.py` & `libcst-1.0.1/libcst/_nodes/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
         a node's deep children with a new node. Note that if you have previously
         modified the tree in a way that ``old_node`` appears more than once as a deep
         child, all instances will be replaced.
         """
         new_tree = self.visit(_ChildReplacementTransformer(old_node, new_node))
         if isinstance(new_tree, (FlattenSentinel, RemovalSentinel)):
             # The above transform never returns *Sentinel, so this isn't possible
-            raise Exception("Logic error, cannot get a *Sentinal here!")
+            raise Exception("Logic error, cannot get a *Sentinel here!")
         return new_tree
 
     def deep_remove(
         self: _CSTNodeSelfT, old_node: "CSTNode"
     ) -> Union[_CSTNodeSelfT, RemovalSentinel]:
         """
         Recursively removes any instance of ``old_node`` by identity. Note that if you
```

### Comparing `libcst-1.0.0/libcst/_nodes/deep_equals.py` & `libcst-1.0.1/libcst/_nodes/deep_equals.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/expression.py` & `libcst-1.0.1/libcst/_nodes/expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -695,15 +695,15 @@
         )
 
     def _codegen_impl(self, state: CodegenState) -> None:
         with self._parenthesize(state):
             state.add_token(self.value)
 
     @property
-    def evaluated_value(self) -> str:
+    def evaluated_value(self) -> Union[str, bytes]:
         """
         Return an :func:`ast.literal_eval` evaluated str of :py:attr:`value`.
         """
         return literal_eval(self.value)
 
 
 class BaseFormattedStringContent(CSTNode, ABC):
@@ -1030,29 +1030,33 @@
     def _codegen_impl(self, state: CodegenState) -> None:
         with self._parenthesize(state):
             self.left._codegen(state)
             self.whitespace_between._codegen(state)
             self.right._codegen(state)
 
     @property
-    def evaluated_value(self) -> Optional[str]:
+    def evaluated_value(self) -> Union[str, bytes, None]:
         """
         Return an :func:`ast.literal_eval` evaluated str of recursively concatenated :py:attr:`left` and :py:attr:`right`
         if and only if both :py:attr:`left` and :py:attr:`right` are composed by :class:`SimpleString` or :class:`ConcatenatedString`
         (:class:`FormattedString` cannot be evaluated).
         """
         left = self.left
         right = self.right
         if isinstance(left, FormattedString) or isinstance(right, FormattedString):
             return None
         left_val = left.evaluated_value
         right_val = right.evaluated_value
         if right_val is None:
             return None
-        return left_val + right_val
+        if isinstance(left_val, bytes) and isinstance(right_val, bytes):
+            return left_val + right_val
+        if isinstance(left_val, str) and isinstance(right_val, str):
+            return left_val + right_val
+        return None
 
 
 @add_slots
 @dataclass(frozen=True)
 class ComparisonTarget(CSTNode):
     """
     A target for a :class:`Comparison`. Owns the comparison operator and the value to
@@ -1975,14 +1979,33 @@
             star_arg=visit_sentinel(self, "star_arg", self.star_arg, visitor),
             kwonly_params=visit_sequence(
                 self, "kwonly_params", self.kwonly_params, visitor
             ),
             star_kwarg=visit_optional(self, "star_kwarg", self.star_kwarg, visitor),
         )
 
+    def _safe_to_join_with_lambda(self) -> bool:
+        """
+        Determine if Parameters need a space after the `lambda` keyword. Returns True
+        iff it's safe to omit the space between `lambda` and these Parameters.
+
+        See also `BaseExpression._safe_to_use_with_word_operator`.
+
+        For example: `lambda*_: pass`
+        """
+        if len(self.posonly_params) != 0:
+            return False
+
+        # posonly_ind can't appear if above condition is false
+
+        if len(self.params) > 0 and self.params[0].star not in {"*", "**"}:
+            return False
+
+        return True
+
     def _codegen_impl(self, state: CodegenState) -> None:  # noqa: C901
         # Compute the star existence first so we can ask about whether
         # each element is the last in the list or not.
         star_arg = self.star_arg
         if isinstance(star_arg, MaybeSentinel):
             starincluded = len(self.kwonly_params) > 0
         elif isinstance(star_arg, (Param, ParamStar)):
@@ -2080,14 +2103,21 @@
     rpar: Sequence[RightParen] = ()
 
     #: Whitespace after the lambda keyword, but before any argument or the colon.
     whitespace_after_lambda: Union[
         BaseParenthesizableWhitespace, MaybeSentinel
     ] = MaybeSentinel.DEFAULT
 
+    def _safe_to_use_with_word_operator(self, position: ExpressionPosition) -> bool:
+        if position == ExpressionPosition.LEFT:
+            return len(self.rpar) > 0 or self.body._safe_to_use_with_word_operator(
+                position
+            )
+        return super()._safe_to_use_with_word_operator(position)
+
     def _validate(self) -> None:
         # Validate parents
         super(Lambda, self)._validate()
         # Sum up all parameters
         all_params = [
             *self.params.posonly_params,
             *self.params.params,
@@ -2107,14 +2137,15 @@
                     raise CSTValidationError(
                         "Lambda params cannot have type annotations."
                     )
             whitespace_after_lambda = self.whitespace_after_lambda
             if (
                 isinstance(whitespace_after_lambda, BaseParenthesizableWhitespace)
                 and whitespace_after_lambda.empty
+                and not self.params._safe_to_join_with_lambda()
             ):
                 raise CSTValidationError(
                     "Must have at least one space after lambda when specifying params"
                 )
 
     def _visit_and_replace_children(self, visitor: CSTVisitorT) -> "Lambda":
         return Lambda(
@@ -2484,14 +2515,20 @@
 
     #: Whitespace after the ``test`` expression, but before the ``else`` keyword.
     whitespace_before_else: BaseParenthesizableWhitespace = SimpleWhitespace.field(" ")
 
     #: Whitespace after the ``else`` keyword, but before the ``orelse`` expression.
     whitespace_after_else: BaseParenthesizableWhitespace = SimpleWhitespace.field(" ")
 
+    def _safe_to_use_with_word_operator(self, position: ExpressionPosition) -> bool:
+        if position == ExpressionPosition.RIGHT:
+            return self.body._safe_to_use_with_word_operator(position)
+        else:
+            return self.orelse._safe_to_use_with_word_operator(position)
+
     def _validate(self) -> None:
         # Paren validation and such
         super(IfExp, self)._validate()
         # Validate spacing rules
         if (
             self.whitespace_before_if.empty
             and not self.body._safe_to_use_with_word_operator(ExpressionPosition.LEFT)
@@ -3487,15 +3524,15 @@
     """
 
     __slots__ = ()
 
     #: The expression evaluated during each iteration of the comprehension. This
     #: lexically comes before the ``for_in`` clause, but it is semantically the
     #: inner-most element, evaluated inside the ``for_in`` clause.
-    elt: BaseAssignTargetExpression
+    elt: BaseExpression
 
     #: The ``for ... in ... if ...`` clause that lexically comes after ``elt``. This may
     #: be a nested structure for nested comprehensions. See :class:`CompFor` for
     #: details.
     for_in: CompFor
 
     def _validate(self) -> None:
@@ -3520,15 +3557,15 @@
     :attr:`CompFor.iter`.
 
     All ``for ... in ...`` and ``if ...`` clauses are stored as a recursive
     :class:`CompFor` data structure inside ``for_in``.
     """
 
     #: The expression evaluated and yielded during each iteration of the generator.
-    elt: BaseAssignTargetExpression
+    elt: BaseExpression
 
     #: The ``for ... in ... if ...`` clause that comes after ``elt``. This may be a
     #: nested structure for nested comprehensions. See :class:`CompFor` for details.
     for_in: CompFor
 
     lpar: Sequence[LeftParen] = field(default_factory=lambda: (LeftParen(),))
     #: Sequence of parentheses for precedence dictation. Generator expressions must
@@ -3571,15 +3608,15 @@
     :attr:`CompFor.iter`.
 
     All ``for ... in ...`` and ``if ...`` clauses are stored as a recursive
     :class:`CompFor` data structure inside ``for_in``.
     """
 
     #: The expression evaluated and stored during each iteration of the comprehension.
-    elt: BaseAssignTargetExpression
+    elt: BaseExpression
 
     #: The ``for ... in ... if ...`` clause that comes after ``elt``. This may be a
     #: nested structure for nested comprehensions. See :class:`CompFor` for details.
     for_in: CompFor
 
     lbracket: LeftSquareBracket = LeftSquareBracket.field()
     #: Brackets surrounding the list comprehension.
@@ -3613,15 +3650,15 @@
     :attr:`CompFor.iter`.
 
     All ``for ... in ...`` and ``if ...`` clauses are stored as a recursive
     :class:`CompFor` data structure inside ``for_in``.
     """
 
     #: The expression evaluated and stored during each iteration of the comprehension.
-    elt: BaseAssignTargetExpression
+    elt: BaseExpression
 
     #: The ``for ... in ... if ...`` clause that comes after ``elt``. This may be a
     #: nested structure for nested comprehensions. See :class:`CompFor` for details.
     for_in: CompFor
 
     lbrace: LeftCurlyBrace = LeftCurlyBrace.field()
     #: Braces surrounding the set comprehension.
@@ -3655,18 +3692,18 @@
     evaluated for each item.
 
     All ``for ... in ...`` and ``if ...`` clauses are stored as a recursive
     :class:`CompFor` data structure inside ``for_in``.
     """
 
     #: The key inserted into the dictionary during each iteration of the comprehension.
-    key: BaseAssignTargetExpression
+    key: BaseExpression
     #: The value associated with the ``key`` inserted into the dictionary during each
     #: iteration of the comprehension.
-    value: BaseAssignTargetExpression
+    value: BaseExpression
 
     #: The ``for ... in ... if ...`` clause that lexically comes after ``key`` and
     #: ``value``. This may be a nested structure for nested comprehensions. See
     #: :class:`CompFor` for details.
     for_in: CompFor
 
     lbrace: LeftCurlyBrace = LeftCurlyBrace.field()
@@ -3762,14 +3799,23 @@
             whitespace_after_walrus=visit_required(
                 self, "whitespace_after_walrus", self.whitespace_after_walrus, visitor
             ),
             value=visit_required(self, "value", self.value, visitor),
             rpar=visit_sequence(self, "rpar", self.rpar, visitor),
         )
 
+    def _safe_to_use_with_word_operator(self, position: ExpressionPosition) -> bool:
+        if position == ExpressionPosition.LEFT:
+            return len(self.rpar) > 0 or self.value._safe_to_use_with_word_operator(
+                position
+            )
+        return len(self.lpar) > 0 or self.target._safe_to_use_with_word_operator(
+            position
+        )
+
     def _codegen_impl(self, state: CodegenState) -> None:
         with self._parenthesize(state):
             self.target._codegen(state)
             self.whitespace_before_walrus._codegen(state)
             state.add_token(":=")
             self.whitespace_after_walrus._codegen(state)
             self.value._codegen(state)
```

### Comparing `libcst-1.0.0/libcst/_nodes/internal.py` & `libcst-1.0.1/libcst/_nodes/internal.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/module.py` & `libcst-1.0.1/libcst/_nodes/module.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/op.py` & `libcst-1.0.1/libcst/_nodes/op.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/statement.py` & `libcst-1.0.1/libcst/_nodes/statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,15 +741,18 @@
     #: Whitespace between the parent node and the ``as`` keyword.
     whitespace_before_as: BaseParenthesizableWhitespace = SimpleWhitespace.field(" ")
 
     #: Whitespace between the ``as`` keyword and the name.
     whitespace_after_as: BaseParenthesizableWhitespace = SimpleWhitespace.field(" ")
 
     def _validate(self) -> None:
-        if self.whitespace_after_as.empty:
+        if (
+            self.whitespace_after_as.empty
+            and not self.name._safe_to_use_with_word_operator(ExpressionPosition.RIGHT)
+        ):
             raise CSTValidationError(
                 "There must be at least one space between 'as' and name."
             )
 
     def _visit_and_replace_children(self, visitor: CSTVisitorT) -> "AsName":
         return AsName(
             whitespace_before_as=visit_required(
@@ -1682,14 +1685,16 @@
     if not isinstance(expr, Expr):
         return None
     val = expr.value
     if isinstance(val, (SimpleString, ConcatenatedString)):
         evaluated_value = val.evaluated_value
     else:
         return None
+    if isinstance(evaluated_value, bytes):
+        return None
 
     if evaluated_value is not None and clean:
         return inspect.cleandoc(evaluated_value)
     return evaluated_value
 
 
 @add_slots
```

### Comparing `libcst-1.0.0/libcst/_nodes/tests/base.py` & `libcst-1.0.1/libcst/_nodes/tests/base.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_assert.py` & `libcst-1.0.1/libcst/_nodes/tests/test_assert.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_assign.py` & `libcst-1.0.1/libcst/_nodes/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_atom.py` & `libcst-1.0.1/libcst/_nodes/tests/test_atom.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_attribute.py` & `libcst-1.0.1/libcst/_nodes/tests/test_attribute.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_await.py` & `libcst-1.0.1/libcst/_nodes/tests/test_await.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_binary_op.py` & `libcst-1.0.1/libcst/_nodes/tests/test_binary_op.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_boolean_op.py` & `libcst-1.0.1/libcst/_nodes/tests/test_boolean_op.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_call.py` & `libcst-1.0.1/libcst/_nodes/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_classdef.py` & `libcst-1.0.1/libcst/_nodes/tests/test_classdef.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_comment.py` & `libcst-1.0.1/libcst/_nodes/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_comparison.py` & `libcst-1.0.1/libcst/_nodes/tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_cst_node.py` & `libcst-1.0.1/libcst/_nodes/tests/test_cst_node.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_del.py` & `libcst-1.0.1/libcst/_nodes/tests/test_del.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_dict.py` & `libcst-1.0.1/libcst/_nodes/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_dict_comp.py` & `libcst-1.0.1/libcst/_nodes/tests/test_dict_comp.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,25 @@
                     cst.Name("v"),
                     cst.CompFor(target=cst.Name("a"), iter=cst.Name("b")),
                 ),
                 "code": "{k: v for a in b}",
                 "parser": parse_expression,
                 "expected_position": CodeRange((1, 0), (1, 17)),
             },
+            # non-trivial keys & values in DictComp
+            {
+                "node": cst.DictComp(
+                    cst.BinaryOperation(cst.Name("k1"), cst.Add(), cst.Name("k2")),
+                    cst.BinaryOperation(cst.Name("v1"), cst.Add(), cst.Name("v2")),
+                    cst.CompFor(target=cst.Name("a"), iter=cst.Name("b")),
+                ),
+                "code": "{k1 + k2: v1 + v2 for a in b}",
+                "parser": parse_expression,
+                "expected_position": CodeRange((1, 0), (1, 29)),
+            },
             # custom whitespace around colon
             {
                 "node": cst.DictComp(
                     cst.Name("k"),
                     cst.Name("v"),
                     cst.CompFor(target=cst.Name("a"), iter=cst.Name("b")),
                     whitespace_before_colon=cst.SimpleWhitespace("\t"),
```

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_docstring.py` & `libcst-1.0.1/libcst/_nodes/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_else.py` & `libcst-1.0.1/libcst/_nodes/tests/test_else.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_empty_line.py` & `libcst-1.0.1/libcst/_nodes/tests/test_empty_line.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_flatten_behavior.py` & `libcst-1.0.1/libcst/_nodes/tests/test_flatten_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_for.py` & `libcst-1.0.1/libcst/_nodes/tests/test_for.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_funcdef.py` & `libcst-1.0.1/libcst/_nodes/tests/test_funcdef.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_global.py` & `libcst-1.0.1/libcst/_nodes/tests/test_global.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_if.py` & `libcst-1.0.1/libcst/_nodes/tests/test_if.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_ifexp.py` & `libcst-1.0.1/libcst/_nodes/tests/test_unary_op.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,96 +8,81 @@
 import libcst as cst
 from libcst import parse_expression
 from libcst._nodes.tests.base import CSTNodeTest
 from libcst.metadata import CodeRange
 from libcst.testing.utils import data_provider
 
 
-class IfExpTest(CSTNodeTest):
+class UnaryOperationTest(CSTNodeTest):
     @data_provider(
         (
-            # Simple if experessions
+            # Simple unary operations
+            (cst.UnaryOperation(cst.Plus(), cst.Name("foo")), "+foo"),
+            (cst.UnaryOperation(cst.Minus(), cst.Name("foo")), "-foo"),
+            (cst.UnaryOperation(cst.BitInvert(), cst.Name("foo")), "~foo"),
+            (cst.UnaryOperation(cst.Not(), cst.Name("foo")), "not foo"),
+            # Parenthesized unary operation
             (
-                cst.IfExp(
-                    body=cst.Name("foo"), test=cst.Name("bar"), orelse=cst.Name("baz")
-                ),
-                "foo if bar else baz",
-            ),
-            # Parenthesized if expressions
-            (
-                cst.IfExp(
+                cst.UnaryOperation(
                     lpar=(cst.LeftParen(),),
-                    body=cst.Name("foo"),
-                    test=cst.Name("bar"),
-                    orelse=cst.Name("baz"),
+                    operator=cst.Not(),
+                    expression=cst.Name("foo"),
                     rpar=(cst.RightParen(),),
                 ),
-                "(foo if bar else baz)",
+                "(not foo)",
+                CodeRange((1, 1), (1, 8)),
             ),
             (
-                cst.IfExp(
-                    body=cst.Name(
+                cst.UnaryOperation(
+                    operator=cst.Not(whitespace_after=cst.SimpleWhitespace("")),
+                    expression=cst.Name(
                         "foo", lpar=(cst.LeftParen(),), rpar=(cst.RightParen(),)
                     ),
-                    whitespace_before_if=cst.SimpleWhitespace(""),
-                    whitespace_after_if=cst.SimpleWhitespace(""),
-                    test=cst.Name(
-                        "bar", lpar=(cst.LeftParen(),), rpar=(cst.RightParen(),)
-                    ),
-                    whitespace_before_else=cst.SimpleWhitespace(""),
-                    whitespace_after_else=cst.SimpleWhitespace(""),
-                    orelse=cst.Name(
-                        "baz", lpar=(cst.LeftParen(),), rpar=(cst.RightParen(),)
-                    ),
                 ),
-                "(foo)if(bar)else(baz)",
-                CodeRange((1, 0), (1, 21)),
+                "not(foo)",
+                CodeRange((1, 0), (1, 8)),
             ),
             # Make sure that spacing works
             (
-                cst.IfExp(
+                cst.UnaryOperation(
                     lpar=(cst.LeftParen(whitespace_after=cst.SimpleWhitespace(" ")),),
-                    body=cst.Name("foo"),
-                    whitespace_before_if=cst.SimpleWhitespace("  "),
-                    whitespace_after_if=cst.SimpleWhitespace("  "),
-                    test=cst.Name("bar"),
-                    whitespace_before_else=cst.SimpleWhitespace("  "),
-                    whitespace_after_else=cst.SimpleWhitespace("  "),
-                    orelse=cst.Name("baz"),
+                    operator=cst.Not(whitespace_after=cst.SimpleWhitespace("  ")),
+                    expression=cst.Name("foo"),
                     rpar=(cst.RightParen(whitespace_before=cst.SimpleWhitespace(" ")),),
                 ),
-                "( foo  if  bar  else  baz )",
-                CodeRange((1, 2), (1, 25)),
+                "( not  foo )",
+                CodeRange((1, 2), (1, 10)),
             ),
         )
     )
     def test_valid(
         self, node: cst.CSTNode, code: str, position: Optional[CodeRange] = None
     ) -> None:
         self.validate_node(node, code, parse_expression, expected_position=position)
 
     @data_provider(
         (
             (
-                lambda: cst.IfExp(
-                    cst.Name("bar"),
-                    cst.Name("foo"),
-                    cst.Name("baz"),
-                    lpar=(cst.LeftParen(),),
+                lambda: cst.UnaryOperation(
+                    cst.Plus(), cst.Name("foo"), lpar=(cst.LeftParen(),)
                 ),
                 "left paren without right paren",
             ),
             (
-                lambda: cst.IfExp(
-                    cst.Name("bar"),
-                    cst.Name("foo"),
-                    cst.Name("baz"),
-                    rpar=(cst.RightParen(),),
+                lambda: cst.UnaryOperation(
+                    cst.Plus(), cst.Name("foo"), rpar=(cst.RightParen(),)
                 ),
                 "right paren without left paren",
             ),
+            (
+                lambda: cst.UnaryOperation(
+                    operator=cst.Not(whitespace_after=cst.SimpleWhitespace("")),
+                    expression=cst.Name("foo"),
+                ),
+                "at least one space after not operator",
+            ),
         )
     )
     def test_invalid(
         self, get_node: Callable[[], cst.CSTNode], expected_re: str
     ) -> None:
         self.assert_invalid(get_node, expected_re)
```

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_import.py` & `libcst-1.0.1/libcst/_nodes/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_indented_block.py` & `libcst-1.0.1/libcst/_nodes/tests/test_indented_block.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_lambda.py` & `libcst-1.0.1/libcst/_nodes/tests/test_lambda.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,38 +301,14 @@
                     cst.Integer("5"),
                     whitespace_after_lambda=cst.SimpleWhitespace(""),
                 ),
                 "at least one space after lambda",
             ),
             (
                 lambda: cst.Lambda(
-                    cst.Parameters(star_arg=cst.Param(cst.Name("arg"))),
-                    cst.Integer("5"),
-                    whitespace_after_lambda=cst.SimpleWhitespace(""),
-                ),
-                "at least one space after lambda",
-            ),
-            (
-                lambda: cst.Lambda(
-                    cst.Parameters(kwonly_params=(cst.Param(cst.Name("arg")),)),
-                    cst.Integer("5"),
-                    whitespace_after_lambda=cst.SimpleWhitespace(""),
-                ),
-                "at least one space after lambda",
-            ),
-            (
-                lambda: cst.Lambda(
-                    cst.Parameters(star_kwarg=cst.Param(cst.Name("arg"))),
-                    cst.Integer("5"),
-                    whitespace_after_lambda=cst.SimpleWhitespace(""),
-                ),
-                "at least one space after lambda",
-            ),
-            (
-                lambda: cst.Lambda(
                     cst.Parameters(
                         star_kwarg=cst.Param(cst.Name("bar"), equal=cst.AssignEqual())
                     ),
                     cst.Integer("5"),
                 ),
                 "Must have a default when specifying an AssignEqual.",
             ),
@@ -940,14 +916,61 @@
                         whitespace_after=cst.SimpleWhitespace(" "),
                     ),
                     body=cst.Integer("5"),
                     rpar=(cst.RightParen(whitespace_before=cst.SimpleWhitespace(" ")),),
                 ),
                 "( lambda  : 5 )",
             ),
+            # No space between lambda and params
+            (
+                cst.Lambda(
+                    cst.Parameters(star_arg=cst.Param(cst.Name("args"), star="*")),
+                    cst.Integer("5"),
+                    whitespace_after_lambda=cst.SimpleWhitespace(""),
+                ),
+                "lambda*args: 5",
+            ),
+            (
+                cst.Lambda(
+                    cst.Parameters(star_kwarg=cst.Param(cst.Name("kwargs"), star="**")),
+                    cst.Integer("5"),
+                    whitespace_after_lambda=cst.SimpleWhitespace(""),
+                ),
+                "lambda**kwargs: 5",
+            ),
+            (
+                cst.Lambda(
+                    cst.Parameters(
+                        star_arg=cst.ParamStar(
+                            comma=cst.Comma(
+                                cst.SimpleWhitespace(""), cst.SimpleWhitespace("")
+                            )
+                        ),
+                        kwonly_params=[cst.Param(cst.Name("args"), star="")],
+                    ),
+                    cst.Integer("5"),
+                    whitespace_after_lambda=cst.SimpleWhitespace(""),
+                ),
+                "lambda*,args: 5",
+            ),
+            (
+                cst.ListComp(
+                    elt=cst.Lambda(
+                        params=cst.Parameters(),
+                        body=cst.Tuple(()),
+                        colon=cst.Colon(),
+                    ),
+                    for_in=cst.CompFor(
+                        target=cst.Name("_"),
+                        iter=cst.Name("_"),
+                        whitespace_before=cst.SimpleWhitespace(""),
+                    ),
+                ),
+                "[lambda:()for _ in _]",
+            ),
         )
     )
     def test_valid(
         self, node: cst.CSTNode, code: str, position: Optional[CodeRange] = None
     ) -> None:
         self.validate_node(node, code, parse_expression, position)
```

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_leaf_small_statements.py` & `libcst-1.0.1/libcst/_nodes/tests/test_leaf_small_statements.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_list.py` & `libcst-1.0.1/libcst/_nodes/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_match.py` & `libcst-1.0.1/libcst/_nodes/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_matrix_multiply.py` & `libcst-1.0.1/libcst/_nodes/tests/test_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_module.py` & `libcst-1.0.1/libcst/_nodes/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_namedexpr.py` & `libcst-1.0.1/libcst/_nodes/tests/test_namedexpr.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,14 +162,30 @@
                     ],
                     whitespace_before_args=cst.SimpleWhitespace("  "),
                 ),
                 "code": "f(  y   :=    1     )",
                 "parser": _parse_expression_force_38,
                 "expected_position": None,
             },
+            {
+                "node": cst.ListComp(
+                    elt=cst.NamedExpr(
+                        cst.Name("_"),
+                        cst.SimpleString("''"),
+                        whitespace_after_walrus=cst.SimpleWhitespace(""),
+                        whitespace_before_walrus=cst.SimpleWhitespace(""),
+                    ),
+                    for_in=cst.CompFor(
+                        target=cst.Name("_"),
+                        iter=cst.Name("_"),
+                        whitespace_before=cst.SimpleWhitespace(""),
+                    ),
+                ),
+                "code": "[_:=''for _ in _]",
+            },
         )
     )
     def test_valid(self, **kwargs: Any) -> None:
         self.validate_node(**kwargs)
 
     @data_provider(
         (
```

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_newline.py` & `libcst-1.0.1/libcst/_nodes/tests/test_newline.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_nonlocal.py` & `libcst-1.0.1/libcst/_nodes/tests/test_nonlocal.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_number.py` & `libcst-1.0.1/libcst/_nodes/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_raise.py` & `libcst-1.0.1/libcst/_nodes/tests/test_raise.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_removal_behavior.py` & `libcst-1.0.1/libcst/_nodes/tests/test_removal_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_return.py` & `libcst-1.0.1/libcst/_nodes/tests/test_return.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_set.py` & `libcst-1.0.1/libcst/_nodes/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_simple_comp.py` & `libcst-1.0.1/libcst/_nodes/tests/test_simple_comp.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,41 @@
             {
                 "node": cst.SetComp(
                     cst.Name("a"), cst.CompFor(target=cst.Name("b"), iter=cst.Name("c"))
                 ),
                 "code": "{a for b in c}",
                 "parser": parse_expression,
             },
+            # non-trivial elt in GeneratorExp
+            {
+                "node": cst.GeneratorExp(
+                    cst.BinaryOperation(cst.Name("a1"), cst.Add(), cst.Name("a2")),
+                    cst.CompFor(target=cst.Name("b"), iter=cst.Name("c")),
+                ),
+                "code": "(a1 + a2 for b in c)",
+                "parser": parse_expression,
+            },
+            # non-trivial elt in ListComp
+            {
+                "node": cst.ListComp(
+                    cst.BinaryOperation(cst.Name("a1"), cst.Add(), cst.Name("a2")),
+                    cst.CompFor(target=cst.Name("b"), iter=cst.Name("c")),
+                ),
+                "code": "[a1 + a2 for b in c]",
+                "parser": parse_expression,
+            },
+            # non-trivial elt in SetComp
+            {
+                "node": cst.SetComp(
+                    cst.BinaryOperation(cst.Name("a1"), cst.Add(), cst.Name("a2")),
+                    cst.CompFor(target=cst.Name("b"), iter=cst.Name("c")),
+                ),
+                "code": "{a1 + a2 for b in c}",
+                "parser": parse_expression,
+            },
             # async GeneratorExp
             {
                 "node": cst.GeneratorExp(
                     cst.Name("a"),
                     cst.CompFor(
                         target=cst.Name("b"),
                         iter=cst.Name("c"),
```

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_simple_statement.py` & `libcst-1.0.1/libcst/_nodes/tests/test_simple_statement.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_simple_string.py` & `libcst-1.0.1/libcst/_nodes/tests/test_simple_string.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_simple_whitespace.py` & `libcst-1.0.1/libcst/_nodes/tests/test_simple_whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_small_statement.py` & `libcst-1.0.1/libcst/_nodes/tests/test_small_statement.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_subscript.py` & `libcst-1.0.1/libcst/_nodes/tests/test_subscript.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_trailing_whitespace.py` & `libcst-1.0.1/libcst/_nodes/tests/test_trailing_whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_try.py` & `libcst-1.0.1/libcst/_nodes/tests/test_try.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_tuple.py` & `libcst-1.0.1/libcst/_nodes/tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_while.py` & `libcst-1.0.1/libcst/_nodes/tests/test_while.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_with.py` & `libcst-1.0.1/libcst/_nodes/tests/test_with.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,31 @@
                         ),
                     ),
                     cst.SimpleStatementSuite((cst.Pass(),)),
                 ),
                 "code": "with context_mgr() as ctx: pass\n",
                 "parser": parse_statement,
             },
+            {
+                "node": cst.With(
+                    (
+                        cst.WithItem(
+                            cst.Call(cst.Name("context_mgr")),
+                            cst.AsName(
+                                cst.Tuple(()),
+                                whitespace_after_as=cst.SimpleWhitespace(""),
+                                whitespace_before_as=cst.SimpleWhitespace(""),
+                            ),
+                        ),
+                    ),
+                    cst.SimpleStatementSuite((cst.Pass(),)),
+                ),
+                "code": "with context_mgr()as(): pass\n",
+                "parser": parse_statement,
+            },
             # indentation
             {
                 "node": DummyIndentedBlock(
                     "    ",
                     cst.With(
                         (cst.WithItem(cst.Call(cst.Name("context_mgr"))),),
                         cst.SimpleStatementSuite((cst.Pass(),)),
```

### Comparing `libcst-1.0.0/libcst/_nodes/tests/test_yield.py` & `libcst-1.0.1/libcst/_nodes/tests/test_yield.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_nodes/whitespace.py` & `libcst-1.0.1/libcst/_nodes/whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/base_parser.py` & `libcst-1.0.1/libcst/_parser/base_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/conversions/README.md` & `libcst-1.0.1/libcst/_parser/conversions/README.md`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/conversions/expression.py` & `libcst-1.0.1/libcst/_parser/conversions/expression.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/conversions/module.py` & `libcst-1.0.1/libcst/_parser/conversions/module.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/conversions/params.py` & `libcst-1.0.1/libcst/_parser/conversions/params.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/conversions/statement.py` & `libcst-1.0.1/libcst/_parser/conversions/statement.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/conversions/terminals.py` & `libcst-1.0.1/libcst/_parser/conversions/terminals.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/custom_itertools.py` & `libcst-1.0.1/libcst/_parser/custom_itertools.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/detect_config.py` & `libcst-1.0.1/libcst/_parser/detect_config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/entrypoints.py` & `libcst-1.0.1/libcst/_parser/entrypoints.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/grammar.py` & `libcst-1.0.1/libcst/_parser/grammar.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/parso/pgen2/generator.py` & `libcst-1.0.1/libcst/_parser/parso/pgen2/generator.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/parso/pgen2/grammar_parser.py` & `libcst-1.0.1/libcst/_parser/parso/pgen2/grammar_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/parso/python/py_token.py` & `libcst-1.0.1/libcst/_parser/parso/python/py_token.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/parso/python/token.py` & `libcst-1.0.1/libcst/_parser/parso/python/token.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/parso/python/tokenize.py` & `libcst-1.0.1/libcst/_parser/parso/python/tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/parso/tests/test_fstring.py` & `libcst-1.0.1/libcst/_parser/parso/tests/test_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/parso/tests/test_tokenize.py` & `libcst-1.0.1/libcst/_parser/parso/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/parso/tests/test_utils.py` & `libcst-1.0.1/libcst/_parser/parso/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/parso/utils.py` & `libcst-1.0.1/libcst/_parser/parso/utils.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/production_decorator.py` & `libcst-1.0.1/libcst/_parser/production_decorator.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/py_whitespace_parser.py` & `libcst-1.0.1/libcst/_parser/py_whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/python_parser.py` & `libcst-1.0.1/libcst/_parser/python_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/tests/test_config.py` & `libcst-1.0.1/libcst/_parser/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/tests/test_detect_config.py` & `libcst-1.0.1/libcst/_parser/tests/test_detect_config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/tests/test_footer_behavior.py` & `libcst-1.0.1/libcst/_parser/tests/test_footer_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/tests/test_node_identity.py` & `libcst-1.0.1/libcst/_parser/tests/test_node_identity.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/tests/test_parse_errors.py` & `libcst-1.0.1/libcst/_parser/tests/test_parse_errors.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/tests/test_version_compare.py` & `libcst-1.0.1/libcst/_parser/tests/test_version_compare.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/tests/test_whitespace_parser.py` & `libcst-1.0.1/libcst/_parser/tests/test_whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/tests/test_wrapped_tokenize.py` & `libcst-1.0.1/libcst/_parser/tests/test_wrapped_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/types/config.py` & `libcst-1.0.1/libcst/_parser/types/config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/types/conversions.py` & `libcst-1.0.1/libcst/_parser/types/conversions.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/types/partials.py` & `libcst-1.0.1/libcst/_parser/types/partials.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/types/py_config.py` & `libcst-1.0.1/libcst/_parser/types/py_config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/types/py_token.py` & `libcst-1.0.1/libcst/_parser/types/py_token.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/types/py_whitespace_state.py` & `libcst-1.0.1/libcst/_parser/types/py_whitespace_state.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/types/tests/test_config.py` & `libcst-1.0.1/libcst/_parser/types/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/whitespace_parser.py` & `libcst-1.0.1/libcst/_parser/whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_parser/wrapped_tokenize.py` & `libcst-1.0.1/libcst/_parser/wrapped_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_position.py` & `libcst-1.0.1/libcst/_position.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_removal_sentinel.py` & `libcst-1.0.1/libcst/_removal_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_tabs.py` & `libcst-1.0.1/libcst/_tabs.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_type_enforce.py` & `libcst-1.0.1/libcst/_type_enforce.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_typed_visitor_base.py` & `libcst-1.0.1/libcst/_typed_visitor_base.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/_visitors.py` & `libcst-1.0.1/libcst/_visitors.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codegen/gather.py` & `libcst-1.0.1/libcst/codegen/gather.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codegen/gen_matcher_classes.py` & `libcst-1.0.1/libcst/codegen/gen_matcher_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,17 @@
     aliases: List[Alias]
 
 
 def _get_raw_name(node: cst.CSTNode) -> Optional[str]:
     if isinstance(node, cst.Name):
         return node.value
     elif isinstance(node, cst.SimpleString):
-        return node.evaluated_value
+        evaluated_value = node.evaluated_value
+        if isinstance(evaluated_value, str):
+            return evaluated_value
     elif isinstance(node, cst.SubscriptElement):
         return _get_raw_name(node.slice)
     elif isinstance(node, cst.Index):
         return _get_raw_name(node.value)
     else:
         return None
```

### Comparing `libcst-1.0.0/libcst/codegen/gen_type_mapping.py` & `libcst-1.0.1/libcst/codegen/gen_type_mapping.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codegen/gen_visitor_functions.py` & `libcst-1.0.1/libcst/codegen/gen_visitor_functions.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codegen/generate.py` & `libcst-1.0.1/libcst/codegen/generate.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codegen/tests/test_codegen_clean.py` & `libcst-1.0.1/libcst/codegen/tests/test_codegen_clean.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codegen/transforms.py` & `libcst-1.0.1/libcst/codegen/transforms.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/__init__.py` & `libcst-1.0.1/libcst/codemod/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/_cli.py` & `libcst-1.0.1/libcst/codemod/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,15 +469,15 @@
             print(
                 f"Successfully codemodded {filename}"
                 + (" with warnings\n" if result.warning_messages else "\n"),
                 file=sys.stderr,
             )
 
         # In unified diff mode, the code is a diff we must print.
-        if unified_diff:
+        if unified_diff and result.code:
             print(result.code)
 
 
 @dataclass(frozen=True)
 class ParallelTransformResult:
     """
     The result of running
```

### Comparing `libcst-1.0.0/libcst/codemod/_codemod.py` & `libcst-1.0.1/libcst/codemod/_codemod.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/_command.py` & `libcst-1.0.1/libcst/codemod/_command.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/_context.py` & `libcst-1.0.1/libcst/codemod/_context.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/_dummy_pool.py` & `libcst-1.0.1/libcst/codemod/_dummy_pool.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/_runner.py` & `libcst-1.0.1/libcst/codemod/_runner.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/_testing.py` & `libcst-1.0.1/libcst/codemod/_testing.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/_visitor.py` & `libcst-1.0.1/libcst/codemod/_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/add_pyre_directive.py` & `libcst-1.0.1/libcst/codemod/commands/add_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/add_trailing_commas.py` & `libcst-1.0.1/libcst/codemod/commands/add_trailing_commas.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/convert_format_to_fstring.py` & `libcst-1.0.1/libcst/codemod/commands/convert_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/convert_namedtuple_to_dataclass.py` & `libcst-1.0.1/libcst/codemod/commands/convert_namedtuple_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/convert_percent_format_to_fstring.py` & `libcst-1.0.1/libcst/codemod/commands/convert_percent_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/convert_type_comments.py` & `libcst-1.0.1/libcst/codemod/commands/convert_type_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/ensure_import_present.py` & `libcst-1.0.1/libcst/codemod/commands/ensure_import_present.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/fix_pyre_directives.py` & `libcst-1.0.1/libcst/codemod/commands/fix_pyre_directives.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/remove_pyre_directive.py` & `libcst-1.0.1/libcst/codemod/commands/remove_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/remove_unused_imports.py` & `libcst-1.0.1/libcst/codemod/commands/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/rename.py` & `libcst-1.0.1/libcst/codemod/commands/rename.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/strip_strings_from_types.py` & `libcst-1.0.1/libcst/codemod/commands/strip_strings_from_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,12 +39,16 @@
             )
         )
     )
     def leave_SimpleString(
         self, original_node: libcst.SimpleString, updated_node: libcst.SimpleString
     ) -> Union[libcst.SimpleString, libcst.BaseExpression]:
         AddImportsVisitor.add_needed_import(self.context, "__future__", "annotations")
+        evaluated_value = updated_node.evaluated_value
         # Just use LibCST to evaluate the expression itself, and insert that as the
         # annotation.
-        return parse_expression(
-            updated_node.evaluated_value, config=self.module.config_for_parsing
-        )
+        if isinstance(evaluated_value, str):
+            return parse_expression(
+                evaluated_value, config=self.module.config_for_parsing
+            )
+        else:
+            return updated_node
```

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_add_pyre_directive.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_add_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_add_trailing_commas.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_add_trailing_commas.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_convert_format_to_fstring.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_convert_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_convert_type_comments.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_convert_type_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_ensure_import_present.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_ensure_import_present.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_fix_pyre_directives.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_fix_pyre_directives.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_noop.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_noop.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_remove_pyre_directive.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_remove_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_remove_unused_imports.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_rename.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_strip_strings_from_types.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_strip_strings_from_types.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/tests/test_unnecessary_format_string.py` & `libcst-1.0.1/libcst/codemod/commands/tests/test_unnecessary_format_string.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/commands/unnecessary_format_string.py` & `libcst-1.0.1/libcst/codemod/commands/unnecessary_format_string.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/tests/test_codemod.py` & `libcst-1.0.1/libcst/codemod/tests/test_codemod.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/tests/test_codemod_cli.py` & `libcst-1.0.1/libcst/codemod/tests/test_codemod_cli.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/tests/test_metadata.py` & `libcst-1.0.1/libcst/codemod/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/tests/test_runner.py` & `libcst-1.0.1/libcst/codemod/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/__init__.py` & `libcst-1.0.1/libcst/codemod/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/_add_imports.py` & `libcst-1.0.1/libcst/codemod/visitors/_add_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/_apply_type_annotations.py` & `libcst-1.0.1/libcst/codemod/visitors/_apply_type_annotations.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/_gather_comments.py` & `libcst-1.0.1/libcst/codemod/visitors/_gather_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/_gather_exports.py` & `libcst-1.0.1/libcst/codemod/visitors/_gather_exports.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,10 +136,10 @@
         return False
 
     def _handle_string_export(
         self, node: Union[cst.SimpleString, cst.ConcatenatedString]
     ) -> None:
         if self._in_assigned_export:
             name = node.evaluated_value
-            if name is None:
+            if not isinstance(name, str):
                 return
             self.explicit_exported_objects.add(name)
```

### Comparing `libcst-1.0.0/libcst/codemod/visitors/_gather_global_names.py` & `libcst-1.0.1/libcst/codemod/visitors/_gather_global_names.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/_gather_imports.py` & `libcst-1.0.1/libcst/codemod/visitors/_gather_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/_gather_string_annotation_names.py` & `libcst-1.0.1/libcst/codemod/visitors/_gather_string_annotation_names.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/_gather_unused_imports.py` & `libcst-1.0.1/libcst/codemod/visitors/_gather_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/_imports.py` & `libcst-1.0.1/libcst/codemod/visitors/_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/_remove_imports.py` & `libcst-1.0.1/libcst/codemod/visitors/_remove_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/tests/test_add_imports.py` & `libcst-1.0.1/libcst/codemod/visitors/tests/test_add_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/tests/test_apply_type_annotations.py` & `libcst-1.0.1/libcst/codemod/visitors/tests/test_apply_type_annotations.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_comments.py` & `libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_exports.py` & `libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_exports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_global_names.py` & `libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_global_names.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_imports.py` & `libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py` & `libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_unused_imports.py` & `libcst-1.0.1/libcst/codemod/visitors/tests/test_gather_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/codemod/visitors/tests/test_remove_imports.py` & `libcst-1.0.1/libcst/codemod/visitors/tests/test_remove_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/helpers/__init__.py` & `libcst-1.0.1/libcst/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/helpers/_template.py` & `libcst-1.0.1/libcst/helpers/_template.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/helpers/common.py` & `libcst-1.0.1/libcst/helpers/common.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/helpers/expression.py` & `libcst-1.0.1/libcst/helpers/expression.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/helpers/module.py` & `libcst-1.0.1/libcst/helpers/module.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/helpers/paths.py` & `libcst-1.0.1/libcst/helpers/paths.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/helpers/tests/test_expression.py` & `libcst-1.0.1/libcst/helpers/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/helpers/tests/test_module.py` & `libcst-1.0.1/libcst/helpers/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/helpers/tests/test_paths.py` & `libcst-1.0.1/libcst/helpers/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/helpers/tests/test_template.py` & `libcst-1.0.1/libcst/helpers/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/matchers/_decorators.py` & `libcst-1.0.1/libcst/matchers/_decorators.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/matchers/_matcher_base.py` & `libcst-1.0.1/libcst/matchers/_matcher_base.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/matchers/_visitors.py` & `libcst-1.0.1/libcst/matchers/_visitors.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/matchers/tests/test_decorators.py` & `libcst-1.0.1/libcst/matchers/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/matchers/tests/test_extract.py` & `libcst-1.0.1/libcst/matchers/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/matchers/tests/test_findall.py` & `libcst-1.0.1/libcst/matchers/tests/test_findall.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/matchers/tests/test_matchers.py` & `libcst-1.0.1/libcst/matchers/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/matchers/tests/test_matchers_with_metadata.py` & `libcst-1.0.1/libcst/matchers/tests/test_matchers_with_metadata.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/matchers/tests/test_replace.py` & `libcst-1.0.1/libcst/matchers/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/matchers/tests/test_visitors.py` & `libcst-1.0.1/libcst/matchers/tests/test_visitors.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/__init__.py` & `libcst-1.0.1/libcst/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/accessor_provider.py` & `libcst-1.0.1/libcst/metadata/accessor_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/base_provider.py` & `libcst-1.0.1/libcst/metadata/base_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/expression_context_provider.py` & `libcst-1.0.1/libcst/metadata/expression_context_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/file_path_provider.py` & `libcst-1.0.1/libcst/metadata/file_path_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/full_repo_manager.py` & `libcst-1.0.1/libcst/metadata/full_repo_manager.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/name_provider.py` & `libcst-1.0.1/libcst/metadata/name_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/parent_node_provider.py` & `libcst-1.0.1/libcst/metadata/parent_node_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/position_provider.py` & `libcst-1.0.1/libcst/metadata/position_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/reentrant_codegen.py` & `libcst-1.0.1/libcst/metadata/reentrant_codegen.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/scope_provider.py` & `libcst-1.0.1/libcst/metadata/scope_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/span_provider.py` & `libcst-1.0.1/libcst/metadata/span_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_accessor_provider.py` & `libcst-1.0.1/libcst/metadata/tests/test_accessor_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_base_provider.py` & `libcst-1.0.1/libcst/metadata/tests/test_base_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_expression_context_provider.py` & `libcst-1.0.1/libcst/metadata/tests/test_expression_context_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_file_path_provider.py` & `libcst-1.0.1/libcst/metadata/tests/test_file_path_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_full_repo_manager.py` & `libcst-1.0.1/libcst/metadata/tests/test_full_repo_manager.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_metadata_provider.py` & `libcst-1.0.1/libcst/metadata/tests/test_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_metadata_wrapper.py` & `libcst-1.0.1/libcst/metadata/tests/test_metadata_wrapper.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_name_provider.py` & `libcst-1.0.1/libcst/metadata/tests/test_name_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_parent_node_provider.py` & `libcst-1.0.1/libcst/metadata/tests/test_parent_node_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_position_provider.py` & `libcst-1.0.1/libcst/metadata/tests/test_position_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_reentrant_codegen.py` & `libcst-1.0.1/libcst/metadata/tests/test_reentrant_codegen.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_scope_provider.py` & `libcst-1.0.1/libcst/metadata/tests/test_scope_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_span_provider.py` & `libcst-1.0.1/libcst/metadata/tests/test_span_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/tests/test_type_inference_provider.py` & `libcst-1.0.1/libcst/metadata/tests/test_type_inference_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/type_inference_provider.py` & `libcst-1.0.1/libcst/metadata/type_inference_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/metadata/wrapper.py` & `libcst-1.0.1/libcst/metadata/wrapper.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/testing/utils.py` & `libcst-1.0.1/libcst/testing/utils.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/pyre/simple_class.json` & `libcst-1.0.1/libcst/tests/pyre/simple_class.json`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/pyre/simple_class.py` & `libcst-1.0.1/libcst/tests/pyre/simple_class.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_add_slots.py` & `libcst-1.0.1/libcst/tests/test_add_slots.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_batched_visitor.py` & `libcst-1.0.1/libcst/tests/test_batched_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_deep_clone.py` & `libcst-1.0.1/libcst/tests/test_deep_clone.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_deep_replace.py` & `libcst-1.0.1/libcst/tests/test_deep_replace.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_e2e.py` & `libcst-1.0.1/libcst/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_exceptions.py` & `libcst-1.0.1/libcst/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_fuzz.py` & `libcst-1.0.1/libcst/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_pyre_integration.py` & `libcst-1.0.1/libcst/tests/test_pyre_integration.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_tabs.py` & `libcst-1.0.1/libcst/tests/test_tabs.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_tool.py` & `libcst-1.0.1/libcst/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_type_enforce.py` & `libcst-1.0.1/libcst/tests/test_type_enforce.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tests/test_visitor.py` & `libcst-1.0.1/libcst/tests/test_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst/tool.py` & `libcst-1.0.1/libcst/tool.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/libcst.egg-info/PKG-INFO` & `libcst-1.0.1/libcst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcst
-Version: 1.0.0
+Version: 1.0.1
 Summary: A concrete syntax tree with AST-like properties for Python 3.5, 3.6, 3.7, 3.8, 3.9, and 3.10 programs.
 License: All contributions towards LibCST are MIT licensed.
         
         Some Python files have been derived from the standard library and are therefore
         PSF licensed. Modifications on these files are dual licensed (both MIT and
         PSF). These files are:
```

### Comparing `libcst-1.0.0/libcst.egg-info/SOURCES.txt` & `libcst-1.0.1/libcst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/Cargo.lock` & `libcst-1.0.1/native/Cargo.lock`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/Cargo.toml` & `libcst-1.0.1/native/libcst/Cargo.toml`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/Grammar` & `libcst-1.0.1/native/libcst/Grammar`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/README.md` & `libcst-1.0.1/native/libcst/README.md`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/benches/parser_benchmark.rs` & `libcst-1.0.1/native/libcst/benches/parser_benchmark.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/bin.rs` & `libcst-1.0.1/native/libcst/src/bin.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/lib.rs` & `libcst-1.0.1/native/libcst/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -146,14 +146,30 @@
 
     #[test]
     fn test_funcdef_params() {
         parse_module("def g(a, b): ...", None).expect("parse error");
     }
 
     #[test]
+    fn test_single_statement_with_no_newline() {
+        for src in &[
+            "(\n \\\n)",
+            "(\n  \\\n)",
+            "(\n    '''\n''')",
+            "del _",
+            "if _:\n    '''\n)'''",
+            "if _:\n    ('''\n''')",
+            "if _:\n     '''\n  '''",
+            "if _:\n        '''\n    ''' ",
+        ] {
+            parse_module(src, None).unwrap_or_else(|e| panic!("'{}' doesn't parse: {}", src, e));
+        }
+    }
+
+    #[test]
     fn bol_offset_first_line() {
         assert_eq!(0, bol_offset("hello", 1));
         assert_eq!(0, bol_offset("hello", 0));
         assert_eq!(0, bol_offset("hello\nhello", 1));
         assert_eq!(0, bol_offset("hello\nhello", 0));
     }
```

### Comparing `libcst-1.0.0/native/libcst/src/nodes/codegen.rs` & `libcst-1.0.1/native/libcst/src/nodes/codegen.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/expression.rs` & `libcst-1.0.1/native/libcst/src/nodes/expression.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/inflate_helpers.rs` & `libcst-1.0.1/native/libcst/src/nodes/inflate_helpers.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/macros.rs` & `libcst-1.0.1/native/libcst/src/nodes/macros.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/mod.rs` & `libcst-1.0.1/native/libcst/src/nodes/mod.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/module.rs` & `libcst-1.0.1/native/libcst/src/nodes/module.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/op.rs` & `libcst-1.0.1/native/libcst/src/nodes/op.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/parser_config.rs` & `libcst-1.0.1/native/libcst/src/nodes/parser_config.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/py_cached.rs` & `libcst-1.0.1/native/libcst/src/nodes/py_cached.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/statement.rs` & `libcst-1.0.1/native/libcst/src/nodes/statement.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/test_utils.rs` & `libcst-1.0.1/native/libcst/src/nodes/test_utils.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/traits.rs` & `libcst-1.0.1/native/libcst/src/nodes/traits.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/nodes/whitespace.rs` & `libcst-1.0.1/native/libcst/src/nodes/whitespace.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/parser/errors.rs` & `libcst-1.0.1/native/libcst/src/parser/errors.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/parser/grammar.rs` & `libcst-1.0.1/native/libcst/src/parser/grammar.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         rule slice() -> BaseSlice<'input, 'a>
             = l:expression()? col:lit(":") u:expression()?
                 rest:(c:lit(":") s:expression()? {(c, s)})? {
                     make_slice(l, col, u, rest)
             }
             / e:starred_expression() { make_index_from_arg(e) }
-            / v:expression() { make_index(v) }
+            / v:named_expression() { make_index(v) }
 
         rule atom() -> Expression<'input, 'a>
             = n:name() { Expression::Name(Box::new(n)) }
             / n:lit("True") { Expression::Name(Box::new(make_name(n))) }
             / n:lit("False") { Expression::Name(Box::new(make_name(n))) }
             / n:lit("None") { Expression::Name(Box::new(make_name(n))) }
             / &(tok(STRING, "") / tok(FStringStart, "")) s:strings() {s.into()}
```

### Comparing `libcst-1.0.0/native/libcst/src/parser/numbers.rs` & `libcst-1.0.1/native/libcst/src/parser/numbers.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/py.rs` & `libcst-1.0.1/native/libcst/src/py.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/tokenizer/core/LICENSE` & `libcst-1.0.1/native/libcst/src/tokenizer/core/LICENSE`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/tokenizer/core/mod.rs` & `libcst-1.0.1/native/libcst/src/tokenizer/core/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -110,20 +110,16 @@
     Number,
     Op,
     Newline,
     Indent,
     Dedent,
     Async,
     Await,
-    // TODO; add support for these
-    #[allow(dead_code)]
     FStringStart,
-    #[allow(dead_code)]
     FStringString,
-    #[allow(dead_code)]
     FStringEnd,
     EndMarker,
 }
 
 #[derive(Debug, thiserror::Error, Eq, PartialEq)]
 pub enum TokError<'t> {
     #[error("inconsistent mixing of tabs and spaces")]
@@ -330,18 +326,15 @@
 
             // Set start of current token
             self.start_pos = (&self.text_pos).into();
 
             return match self.text_pos.peek() {
                 // Check for EOF now
                 None => {
-                    if self.missing_nl_before_eof
-                        && self.text_pos.byte_column_number() != self.bol_width
-                        && !self.blank_line
-                    {
+                    if self.missing_nl_before_eof && !self.blank_line {
                         self.at_bol = true;
                         self.missing_nl_before_eof = false;
                         Ok(TokType::Newline)
                     } else {
                         let hanging_indents = self.indent_stack.len() as i32;
                         if self.pending_indents == 0 && hanging_indents != 0 {
                             // We've reached EOF but there are still pending indents not
```

### Comparing `libcst-1.0.0/native/libcst/src/tokenizer/core/string_types.rs` & `libcst-1.0.1/native/libcst/src/tokenizer/core/string_types.rs`

 * *Files 3% similar despite different names*

```diff
@@ -94,19 +94,18 @@
     }
 
     pub fn open_parentheses(&mut self) {
         self.parentheses_count += 1;
     }
 
     pub fn close_parentheses(&mut self) {
-        self.parentheses_count -= 1;
-        if self.parentheses_count == 0 {
-            // No parentheses means that the format spec is also finished.
-            self.format_spec_count = 0;
+        if self.is_in_format_spec() {
+            self.format_spec_count -= 1;
         }
+        self.parentheses_count -= 1;
     }
 
     pub fn allow_multiline(&self) -> bool {
         self.quote_size == StringQuoteSize::Triple
     }
 
     pub fn is_in_expr(&self) -> bool {
```

### Comparing `libcst-1.0.0/native/libcst/src/tokenizer/operators.rs` & `libcst-1.0.1/native/libcst/src/tokenizer/operators.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/tokenizer/tests.rs` & `libcst-1.0.1/native/libcst/src/tokenizer/tests.rs`

 * *Files 2% similar despite different names*

```diff
@@ -715,14 +715,27 @@
             (TokType::Newline, ""),
             (TokType::EndMarker, "")
         ])
     );
 }
 
 #[test]
+fn test_fake_newline_when_at_bol() {
+    assert_eq!(
+        tokenize_with_end_marker("(\n \\\n)", &default_config()),
+        Ok(vec![
+            (TokType::Op, "("),
+            (TokType::Op, ")"),
+            (TokType::Newline, ""),
+            (TokType::EndMarker, "")
+        ])
+    )
+}
+
+#[test]
 fn test_no_fake_newline_for_empty_input() {
     assert_eq!(
         tokenize_with_end_marker("", &default_config()),
         Ok(vec![(TokType::EndMarker, "")])
     );
 }
 
@@ -810,7 +823,33 @@
             (TokType::Indent, ""),
             (TokType::Name, "pass"),
             (TokType::Newline, "\n"),
             (TokType::Dedent, ""),
         ])
     )
 }
+
+#[test]
+fn test_nested_f_string_specs() {
+    let config = TokConfig {
+        split_fstring: true,
+        ..default_config()
+    };
+    assert_eq!(
+        tokenize_all("f'{_:{_:}{_}}'", &config),
+        Ok(vec![
+            (TokType::FStringStart, "f'"),
+            (TokType::Op, "{"),
+            (TokType::Name, "_"),
+            (TokType::Op, ":"),
+            (TokType::Op, "{"),
+            (TokType::Name, "_"),
+            (TokType::Op, ":"),
+            (TokType::Op, "}"),
+            (TokType::Op, "{"),
+            (TokType::Name, "_"),
+            (TokType::Op, "}"),
+            (TokType::Op, "}"),
+            (TokType::FStringEnd, "'")
+        ])
+    )
+}
```

### Comparing `libcst-1.0.0/native/libcst/src/tokenizer/text_position/char_width.rs` & `libcst-1.0.1/native/libcst/src/tokenizer/text_position/char_width.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/src/tokenizer/text_position/mod.rs` & `libcst-1.0.1/native/libcst/src/tokenizer/text_position/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,18 @@
         if let Some(cw) = self.char_widths.previous() {
             // If we tried to back up across a newline, we'd have to recompute char_column_number,
             // which would be expensive, so it's unsupported.
             self.inner_char_column_number = self
                 .inner_char_column_number
                 .checked_sub(1)
                 .expect("cannot back up past the beginning of a line.");
+            self.inner_byte_column_number = self
+                .inner_byte_column_number
+                .checked_sub(cw.byte_width)
+                .expect("cannot back up past the beginning of a line.");
             self.inner_byte_idx -= cw.byte_width;
         } else {
             panic!("Tried to backup past the beginning of the text.")
         }
     }
 
     /// Tries to consume the given TextPattern, moving the TextPosition forward. Returns false if no
@@ -213,14 +217,15 @@
 impl fmt::Debug for TextPosition<'_> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         f.debug_struct("TextPosition")
             .field("text", &EllipsisDebug)
             .field("char_widths", &EllipsisDebug)
             .field("inner_byte_idx", &self.inner_byte_idx)
             .field("inner_char_column_number", &self.inner_char_column_number)
+            .field("inner_byte_column_number", &self.inner_byte_column_number)
             .field("inner_line_number", &self.inner_line_number)
             .finish()
     }
 }
 
 impl From<&TextPosition<'_>> for TextPositionSnapshot {
     fn from(tp: &TextPosition) -> Self {
```

### Comparing `libcst-1.0.0/native/libcst/src/tokenizer/whitespace_parser.rs` & `libcst-1.0.1/native/libcst/src/tokenizer/whitespace_parser.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/tests/fixtures/big_binary_operator.py` & `libcst-1.0.1/native/libcst/tests/fixtures/big_binary_operator.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/tests/fixtures/comments.py` & `libcst-1.0.1/native/libcst/tests/fixtures/comments.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/tests/fixtures/expr.py` & `libcst-1.0.1/native/libcst/tests/fixtures/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 lambda a, b, c=True: a
 lambda a, b, c=True, *, d=(1 << v2), e='str': a
 lambda a, b, c=True, *vararg, d=(v1 << 2), e='str', **kwargs: a + b
 lambda a, b, c=True, *vararg, d=(v1 << 2), e='str', **kwargs : a + b
 manylambdas = lambda x=lambda y=lambda z=1: z: y(): x()
 foo = (lambda port_id, ignore_missing: {"port1": port1_resource, "port2": port2_resource}[port_id])
 1 if True else 2
+_ if 0else  _
 str or None if True else str or bytes or None
 (str or None) if True else (str or bytes or None)
 str or None if (1 if True else 2) else str or bytes or None
 (str or None) if (1 if True else 2) else (str or bytes or None)
 ((super_long_variable_name or None) if (1 if super_long_test_name else 2) else (str or bytes or None))
 {'2.7': dead, '3.7': (long_live or die_hard)}
 {'2.7': dead, '3.7': (long_live or die_hard), **{'3.6': verygood}}
```

### Comparing `libcst-1.0.0/native/libcst/tests/fixtures/fun_with_func_defs.py` & `libcst-1.0.1/native/libcst/tests/fixtures/fun_with_func_defs.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/tests/fixtures/malicious_match.py` & `libcst-1.0.1/native/libcst/tests/fixtures/malicious_match.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/tests/fixtures/pep646.py` & `libcst-1.0.1/native/libcst/tests/fixtures/pep646.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/tests/fixtures/super_strings.py` & `libcst-1.0.1/native/libcst/tests/fixtures/super_strings.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,7 +26,9 @@
 _(f"ok { expr = !r: aosidjhoi } end")
 
 print(f"{self.ERASE_CURRENT_LINE}{self._human_seconds(elapsed_time)} {percent:.{self.pretty_precision}f}% complete, {self.estimate_completion(elapsed_time, finished, left)} estimated for {left} files to go...")
 
 f'\{{\}}'
 f"regexp_like(path, '.*\{file_type}$')"
 f"\lfoo"
+
+f"{_:{_:}{a}}"
```

### Comparing `libcst-1.0.0/native/libcst/tests/fixtures/with_wickedness.py` & `libcst-1.0.1/native/libcst/tests/fixtures/with_wickedness.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst/tests/parser_roundtrip.rs` & `libcst-1.0.1/native/libcst/tests/parser_roundtrip.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst_derive/src/codegen.rs` & `libcst-1.0.1/native/libcst_derive/src/codegen.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst_derive/src/cstnode.rs` & `libcst-1.0.1/native/libcst_derive/src/cstnode.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst_derive/src/inflate.rs` & `libcst-1.0.1/native/libcst_derive/src/inflate.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst_derive/src/into_py.rs` & `libcst-1.0.1/native/libcst_derive/src/into_py.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst_derive/src/lib.rs` & `libcst-1.0.1/native/libcst_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst_derive/src/parenthesized_node.rs` & `libcst-1.0.1/native/libcst_derive/src/parenthesized_node.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst_derive/tests/pass/minimal_cst.rs` & `libcst-1.0.1/native/libcst_derive/tests/pass/minimal_cst.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/native/libcst_derive/tests/pass/simple.rs` & `libcst-1.0.1/native/libcst_derive/tests/pass/simple.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/pyproject.toml` & `libcst-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,31 +22,31 @@
     "typing_extensions>=3.7.4.2",
     "typing_inspect>=0.4.0",
     "pyyaml>=5.2",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "black==23.1.0",
+    "black==23.3.0",
     "coverage>=4.5.4",
     "build>=0.10.0",
     "fixit==0.1.1",
     "flake8>=3.7.8,<5",
     "Sphinx>=5.1.1",
     "hypothesis>=4.36.0",
     "hypothesmith>=0.0.4",
     "jupyter>=1.0.0",
-    "maturin>=0.8.3,<0.14",
+    "maturin>=0.8.3,<0.16",
     "nbsphinx>=0.4.2",
     "prompt-toolkit>=2.0.9",
     "pyre-check==0.9.10; platform_system != 'Windows'",
     "setuptools_scm>=6.0.1",
     "sphinx-rtd-theme>=0.4.3",
     "ufmt==2.1.0",
-    "usort==1.0.6",
+    "usort==1.0.7",
     "setuptools-rust>=1.5.2",
     "slotscheck>=0.7.1",
     "jinja2==3.1.2",
 ]
 
 [project.urls]
 Documentation = "https://libcst.readthedocs.io/en/latest/"
```

### Comparing `libcst-1.0.0/scripts/check_copyright.py` & `libcst-1.0.1/scripts/check_copyright.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/scripts/regenerate-fixtures.py` & `libcst-1.0.1/scripts/regenerate-fixtures.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/setup.py` & `libcst-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/stubs/libcst_native/parser_config.pyi` & `libcst-1.0.1/stubs/libcst_native/parser_config.pyi`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/stubs/libcst_native/token_type.pyi` & `libcst-1.0.1/stubs/libcst_native/token_type.pyi`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/stubs/libcst_native/tokenize.pyi` & `libcst-1.0.1/stubs/libcst_native/tokenize.pyi`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/stubs/libcst_native/whitespace_parser.pyi` & `libcst-1.0.1/stubs/libcst_native/whitespace_parser.pyi`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/stubs/libcst_native/whitespace_state.pyi` & `libcst-1.0.1/stubs/libcst_native/whitespace_state.pyi`

 * *Files identical despite different names*

### Comparing `libcst-1.0.0/stubs/tokenize.pyi` & `libcst-1.0.1/stubs/tokenize.pyi`

 * *Files identical despite different names*

