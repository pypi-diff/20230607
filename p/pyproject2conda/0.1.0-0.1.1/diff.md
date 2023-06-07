# Comparing `tmp/pyproject2conda-0.1.0.tar.gz` & `tmp/pyproject2conda-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject2conda-0.1.0.tar", last modified: Wed Jun  7 15:58:09 2023, max compression
+gzip compressed data, was "pyproject2conda-0.1.1.tar", last modified: Wed Jun  7 18:25:15 2023, max compression
```

## Comparing `pyproject2conda-0.1.0.tar` & `pyproject2conda-0.1.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.961698 pyproject2conda-0.1.0/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.1.0/.cruft.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/.editorconfig
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.916875 pyproject2conda-0.1.0/.github/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      367 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.1.0/.gitignore
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      465 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      178 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/LICENSE
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11480 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/Makefile
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13760 2023-06-07 15:58:09.961158 pyproject2conda-0.1.0/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10967 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.917372 pyproject2conda-0.1.0/changelog.d/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.917820 pyproject2conda-0.1.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.918865 pyproject2conda-0.1.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.926351 pyproject2conda-0.1.0/docs/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.902776 pyproject2conda-0.1.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.926747 pyproject2conda-0.1.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.927792 pyproject2conda-0.1.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.931287 pyproject2conda-0.1.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.933670 pyproject2conda-0.1.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.935544 pyproject2conda-0.1.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/authors.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/conf.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.936851 pyproject2conda-0.1.0/docs/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      536 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/docs/examples/example-usage.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.937541 pyproject2conda-0.1.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      241 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      936 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/docs/installation.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/license.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/make.bat
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.938288 pyproject2conda-0.1.0/docs/reference/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      143 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/reference/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.946011 pyproject2conda-0.1.0/environment/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      943 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      260 2023-06-07 14:20:27.000000 pyproject2conda-0.1.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      574 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      377 2023-06-07 14:20:28.000000 pyproject2conda-0.1.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      153 2023-06-07 14:20:29.000000 pyproject2conda-0.1.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      144 2023-06-07 14:20:29.000000 pyproject2conda-0.1.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      148 2023-06-07 14:20:17.000000 pyproject2conda-0.1.0/environment.yaml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.947017 pyproject2conda-0.1.0/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/examples/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.947721 pyproject2conda-0.1.0/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6304 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.953117 pyproject2conda-0.1.0/scripts/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      846 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/scripts/lint.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/scripts/recipe-append.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-06-07 15:58:09.961842 pyproject2conda-0.1.0/setup.cfg
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.906221 pyproject2conda-0.1.0/src/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.954606 pyproject2conda-0.1.0/src/pyproject2conda/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      648 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/src/pyproject2conda/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2399 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/src/pyproject2conda/cli.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12343 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/src/pyproject2conda/parser.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.958002 pyproject2conda-0.1.0/src/pyproject2conda.egg-info/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13760 2023-06-07 15:58:09.000000 pyproject2conda-0.1.0/src/pyproject2conda.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2413 2023-06-07 15:58:09.000000 pyproject2conda-0.1.0/src/pyproject2conda.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-07 15:58:09.000000 pyproject2conda-0.1.0/src/pyproject2conda.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       60 2023-06-07 15:58:09.000000 pyproject2conda-0.1.0/src/pyproject2conda.egg-info/entry_points.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      109 2023-06-07 15:58:09.000000 pyproject2conda-0.1.0/src/pyproject2conda.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       16 2023-06-07 15:58:09.000000 pyproject2conda-0.1.0/src/pyproject2conda.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-05 17:19:50.000000 pyproject2conda-0.1.0/src/pyproject2conda.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 15:58:09.960476 pyproject2conda-0.1.0/tests/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       45 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/tests/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      611 2023-06-07 02:50:51.000000 pyproject2conda-0.1.0/tests/test-pyproject.toml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2037 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/tests/test_cli.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3235 2023-06-07 15:56:44.000000 pyproject2conda-0.1.0/tests/test_parser.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4105 2023-06-05 16:53:11.000000 pyproject2conda-0.1.0/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.923139 pyproject2conda-0.1.1/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.1.1/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/.editorconfig
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.870581 pyproject2conda-0.1.1/.github/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      367 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.1.1/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      465 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      178 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11480 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14929 2023-06-07 18:25:15.922321 pyproject2conda-0.1.1/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12136 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.870985 pyproject2conda-0.1.1/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.871380 pyproject2conda-0.1.1/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.872353 pyproject2conda-0.1.1/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.877330 pyproject2conda-0.1.1/docs/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/Makefile
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.856168 pyproject2conda-0.1.1/docs/_static/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.877867 pyproject2conda-0.1.1/docs/_static/css/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.879555 pyproject2conda-0.1.1/docs/_static/js/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.885167 pyproject2conda-0.1.1/docs/_templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.889095 pyproject2conda-0.1.1/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.891038 pyproject2conda-0.1.1/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/authors.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/changelog.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/conf.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.892504 pyproject2conda-0.1.1/docs/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      536 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/docs/examples/example-usage.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.893214 pyproject2conda-0.1.1/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      241 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      936 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/docs/installation.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/license.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/make.bat
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.893854 pyproject2conda-0.1.1/docs/reference/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      143 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.903206 pyproject2conda-0.1.1/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      943 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      260 2023-06-07 14:20:27.000000 pyproject2conda-0.1.1/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      574 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      377 2023-06-07 14:20:28.000000 pyproject2conda-0.1.1/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      153 2023-06-07 14:20:29.000000 pyproject2conda-0.1.1/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      144 2023-06-07 14:20:29.000000 pyproject2conda-0.1.1/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      148 2023-06-07 14:20:17.000000 pyproject2conda-0.1.1/environment.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.903998 pyproject2conda-0.1.1/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/examples/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.904742 pyproject2conda-0.1.1/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6304 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/pyproject.toml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.909471 pyproject2conda-0.1.1/scripts/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      846 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-06-07 18:25:15.923399 pyproject2conda-0.1.1/setup.cfg
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.859799 pyproject2conda-0.1.1/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.911498 pyproject2conda-0.1.1/src/pyproject2conda/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      648 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/src/pyproject2conda/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3062 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/src/pyproject2conda/cli.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12606 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/src/pyproject2conda/parser.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.916877 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14929 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2413 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       60 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/entry_points.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      109 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       16 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-05 17:19:50.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.921119 pyproject2conda-0.1.1/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       45 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/tests/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      611 2023-06-07 02:50:51.000000 pyproject2conda-0.1.1/tests/test-pyproject.toml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2694 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/tests/test_cli.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3738 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/tests/test_parser.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4101 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/tox.ini
```

### Comparing `pyproject2conda-0.1.0/.cruft.json` & `pyproject2conda-0.1.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/.editorconfig` & `pyproject2conda-0.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/.gitignore` & `pyproject2conda-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/.pre-commit-config.yaml` & `pyproject2conda-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/CONTRIBUTING.md` & `pyproject2conda-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/LICENSE` & `pyproject2conda-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/Makefile` & `pyproject2conda-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/PKG-INFO` & `pyproject2conda-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject2conda
-Version: 0.1.0
+Version: 0.1.1
 Summary: A script to convert a Python project declared on a pyproject.toml to a conda environment.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/wpk-nist-gov/pyproject2conda
 Project-URL: documentation, https://pages.nist.gov/pyproject2conda/
 Keywords: pyproject2conda
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -136,14 +136,46 @@
   - pip:
       - athing
 ```
 
 Note that other comments can be mixed in. This also works with extras. For
 example, with the following:
 
+Also, by default, the python version is not included in the resulting conda
+output. To include the specification from pyproject.toml, use `-p/--python`
+option:
+
+```bash
+ ➜ pyproject2conda create -f tests/test-pyproject.toml -p
+channels:
+  - conda-forge
+dependencies:
+  - python>=3.8,<3.11
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+```
+
+To specify a value of python, pass a value with:
+
+```bash
+ ➜ pyproject2conda create -f tests/test-pyproject.toml -p python=3.9
+channels:
+  - conda-forge
+dependencies:
+  - python=3.9
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+```
+
 ```toml
 # ...
 [project.optional-dependencies]
 test = [
   "pandas",
   "pytest", # p2c: -c conda-forge
 
@@ -205,18 +237,19 @@
 `pyproject2conda` can also be used within python:
 
 ```pycon
 >>> from pyproject2conda import PyProject2Conda
 >>> p = PyProject2Conda.from_path("./tests/test-pyproject.toml")
 
 # Basic environment
->>> print(p.to_conda_yaml().strip())
+>>> print(p.to_conda_yaml(python="get").strip())
 channels:
   - conda-forge
 dependencies:
+  - python>=3.8,<3.11
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
 
 # Environment with extras
@@ -333,14 +366,17 @@
 
 ╭─ Options ───────────────────────────────────────────────────────────────────╮
 │ --channel  -c  TEXT  conda channel.  Can be specified multiple times.       │
 │                      Overrides [tool.pyproject2conda.channels]              │
 │ --file     -f  PATH  input pyproject.toml file                              │
 │ --name     -n  TEXT  Name of conda env                                      │
 │ --output   -o  PATH  File to output results                                 │
+│ --python   -p  TEXT  if flag passed without options, include python spec    │
+│                      from pyproject.toml in output.  If value passed, use   │
+│                      this value of python in the output                     │
 │ --help               Show this message and exit.                            │
 ╰─────────────────────────────────────────────────────────────────────────────╯
 
 
  ➜ pyproject2conda isolated --help
 
  Usage: pyproject2conda isolated [OPTIONS] ISOLATED...
@@ -349,14 +385,17 @@
 
 ╭─ Options ───────────────────────────────────────────────────────────────────╮
 │ --channel  -c  TEXT  conda channel.  Can be specified multiple times.       │
 │                      Overrides [tool.pyproject2conda.channels]              │
 │ --file     -f  PATH  input pyproject.toml file                              │
 │ --name     -n  TEXT  Name of conda env                                      │
 │ --output   -o  PATH  File to output results                                 │
+│ --python   -p  TEXT  if flag passed without options, include python spec    │
+│                      from pyproject.toml in output.  If value passed, use   │
+│                      this value of python in the output                     │
 │ --help               Show this message and exit.                            │
 ╰─────────────────────────────────────────────────────────────────────────────╯
 
 ```
 
 <!-- end-docs -->
```

### Comparing `pyproject2conda-0.1.0/README.md` & `pyproject2conda-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,46 @@
   - pip:
       - athing
 ```
 
 Note that other comments can be mixed in. This also works with extras. For
 example, with the following:
 
+Also, by default, the python version is not included in the resulting conda
+output. To include the specification from pyproject.toml, use `-p/--python`
+option:
+
+```bash
+ ➜ pyproject2conda create -f tests/test-pyproject.toml -p
+channels:
+  - conda-forge
+dependencies:
+  - python>=3.8,<3.11
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+```
+
+To specify a value of python, pass a value with:
+
+```bash
+ ➜ pyproject2conda create -f tests/test-pyproject.toml -p python=3.9
+channels:
+  - conda-forge
+dependencies:
+  - python=3.9
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+```
+
 ```toml
 # ...
 [project.optional-dependencies]
 test = [
   "pandas",
   "pytest", # p2c: -c conda-forge
 
@@ -181,18 +213,19 @@
 `pyproject2conda` can also be used within python:
 
 ```pycon
 >>> from pyproject2conda import PyProject2Conda
 >>> p = PyProject2Conda.from_path("./tests/test-pyproject.toml")
 
 # Basic environment
->>> print(p.to_conda_yaml().strip())
+>>> print(p.to_conda_yaml(python="get").strip())
 channels:
   - conda-forge
 dependencies:
+  - python>=3.8,<3.11
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
 
 # Environment with extras
@@ -309,14 +342,17 @@
 
 ╭─ Options ───────────────────────────────────────────────────────────────────╮
 │ --channel  -c  TEXT  conda channel.  Can be specified multiple times.       │
 │                      Overrides [tool.pyproject2conda.channels]              │
 │ --file     -f  PATH  input pyproject.toml file                              │
 │ --name     -n  TEXT  Name of conda env                                      │
 │ --output   -o  PATH  File to output results                                 │
+│ --python   -p  TEXT  if flag passed without options, include python spec    │
+│                      from pyproject.toml in output.  If value passed, use   │
+│                      this value of python in the output                     │
 │ --help               Show this message and exit.                            │
 ╰─────────────────────────────────────────────────────────────────────────────╯
 
 
  ➜ pyproject2conda isolated --help
 
  Usage: pyproject2conda isolated [OPTIONS] ISOLATED...
@@ -325,14 +361,17 @@
 
 ╭─ Options ───────────────────────────────────────────────────────────────────╮
 │ --channel  -c  TEXT  conda channel.  Can be specified multiple times.       │
 │                      Overrides [tool.pyproject2conda.channels]              │
 │ --file     -f  PATH  input pyproject.toml file                              │
 │ --name     -n  TEXT  Name of conda env                                      │
 │ --output   -o  PATH  File to output results                                 │
+│ --python   -p  TEXT  if flag passed without options, include python spec    │
+│                      from pyproject.toml in output.  If value passed, use   │
+│                      this value of python in the output                     │
 │ --help               Show this message and exit.                            │
 ╰─────────────────────────────────────────────────────────────────────────────╯
 
 ```
 
 <!-- end-docs -->
```

### Comparing `pyproject2conda-0.1.0/changelog.d/templates/auto-changelog/template.jinja2` & `pyproject2conda-0.1.1/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/Makefile` & `pyproject2conda-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_static/css/nist-combined.css` & `pyproject2conda-0.1.1/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_static/js/leave_notice.js` & `pyproject2conda-0.1.1/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_static/js/nist-header-footer.js` & `pyproject2conda-0.1.1/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_templates/autosummary/class.rst` & `pyproject2conda-0.1.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_templates/autosummary/module.rst` & `pyproject2conda-0.1.1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_templates/class-individual-pages.rst` & `pyproject2conda-0.1.1/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_templates/class-single-page.rst` & `pyproject2conda-0.1.1/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_templates/custom-module-template.rst` & `pyproject2conda-0.1.1/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_templates/module-custom-imported.rst` & `pyproject2conda-0.1.1/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_templates/module-custom.rst` & `pyproject2conda-0.1.1/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_templates/module-single.rst` & `pyproject2conda-0.1.1/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/_templates/module-template.rst` & `pyproject2conda-0.1.1/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/conf.py` & `pyproject2conda-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/examples/example-usage.md` & `pyproject2conda-0.1.1/docs/examples/example-usage.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/examples/usage/demo.ipynb` & `pyproject2conda-0.1.1/docs/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/installation.md` & `pyproject2conda-0.1.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/docs/make.bat` & `pyproject2conda-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/environment/dev-extras.yaml` & `pyproject2conda-0.1.1/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/environment/docs-extras.yaml` & `pyproject2conda-0.1.1/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/examples/usage/demo.ipynb` & `pyproject2conda-0.1.1/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/pyproject.toml` & `pyproject2conda-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/scripts/dist-conda.mk` & `pyproject2conda-0.1.1/scripts/dist-conda.mk`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/scripts/docs-examples-symlinks.sh` & `pyproject2conda-0.1.1/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/scripts/recipe-append.sh` & `pyproject2conda-0.1.1/scripts/recipe-append.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/src/pyproject2conda/__init__.py` & `pyproject2conda-0.1.1/src/pyproject2conda/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/src/pyproject2conda/cli.py` & `pyproject2conda-0.1.1/src/pyproject2conda/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,25 @@
     default=None,
     help="File to output results",
 )
 
 VERBOSE_CLI = click.option("-v", "--verbose", "verbose", is_flag=True, default=False)
 
 
+PYTHON_CLI = click.option(
+    "-p",
+    "--python",
+    "python",
+    is_flag=False,
+    flag_value="get",
+    default=None,
+    help="if flag passed without options, include python spec from pyproject.toml in output.  If value passed, use this value of python in the output",
+)
+
+
 @click.group()
 def app():
     pass
 
 
 @app.command()
 @FILE_CLI
@@ -67,49 +78,71 @@
 
 @app.command()
 @EXTRAS_CLI
 @CHANNEL_CLI
 @FILE_CLI
 @NAME_CLI
 @OUTPUT_CLI
+@PYTHON_CLI
 def create(
     extras,
     channel,
     filename,
     name,
     output,
+    python,
 ):
     """Create yaml file from dependencies and optional-dependencies."""
 
     if not channel:
         channel = None
     d = PyProject2Conda.from_path(filename)
-    s = d.to_conda_yaml(extras=extras, channels=channel, name=name, stream=output)
+    s = d.to_conda_yaml(
+        extras=extras, channels=channel, name=name, stream=output, python=python
+    )
     if not output:
         click.echo(s, nl=False)
 
 
+# @app.command("create-conda-req")
+# @EXTRAS_CLI
+# @PYTHON_CLI
+# @FILE_CLI
+# def conda_requirements(
+#         extras,
+#         python,
+#         filename,
+
+# ):
+#     d = PyProject2Conda.from_path(filename)
+
+#     output = d.to_conda_lists(extras=extras)
+#     click.echo(f"{output}")
+
+
 @app.command()
 @ISOLATED_CLI
 @CHANNEL_CLI
 @FILE_CLI
 @NAME_CLI
 @OUTPUT_CLI
+@PYTHON_CLI
 def isolated(
     isolated,
     channel,
     filename,
     name,
     output,
+    python,
 ):
     """Create yaml file from [tool.pyproject2conda.isolated-dependencies]"""
 
     if not channel:
         channel = None
     d = PyProject2Conda.from_path(filename)
-    s = d.to_conda_yaml(isolated=isolated, channels=channel, name=name)
+    s = d.to_conda_yaml(isolated=isolated, channels=channel, name=name, python=python)
     if not output:
         click.echo(s, nl=False)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pyproject2conda-0.1.0/src/pyproject2conda/parser.py` & `pyproject2conda-0.1.1/src/pyproject2conda/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
     data: str | Path | tomlkit.toml_document.TOMLDocument,
     extras: Tstr_seq_opt = None,
     isolated: Tstr_seq_opt = None,
     channels: Tstr_seq_opt = None,
     python: Tstr_opt = None,
 ):
     if python == "get":
-        python = "python" + get_in(["project", "requires-pythong"], data).unwrap()
+        python = "python" + get_in(["project", "requires-python"], data).unwrap()
 
     if channels is None:
         channels = get_in(["tool", "pyproject2conda", "channels"], data, None)
         if channels:
             channels = channels.unwrap()
     if isinstance(channels, str):
         channels = [channels]
@@ -464,7 +464,20 @@
 
         if not path.exists():
             raise ValueError(f"{path} does not exist")
 
         with open(path, "rb") as f:
             data = tomlkit.load(f)
         return cls(data=data, name=name, channels=channels, python=python)
+
+
+def _list_to_stream(values, stream=None):
+    value = "\n".join(values)
+    if isinstance(stream, (str, Path)):
+        with open(stream, "w") as f:
+            f.write(value)
+
+    elif stream is None:
+        return value
+
+    else:
+        stream.write(value)
```

### Comparing `pyproject2conda-0.1.0/src/pyproject2conda.egg-info/PKG-INFO` & `pyproject2conda-0.1.1/src/pyproject2conda.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject2conda
-Version: 0.1.0
+Version: 0.1.1
 Summary: A script to convert a Python project declared on a pyproject.toml to a conda environment.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/wpk-nist-gov/pyproject2conda
 Project-URL: documentation, https://pages.nist.gov/pyproject2conda/
 Keywords: pyproject2conda
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -136,14 +136,46 @@
   - pip:
       - athing
 ```
 
 Note that other comments can be mixed in. This also works with extras. For
 example, with the following:
 
+Also, by default, the python version is not included in the resulting conda
+output. To include the specification from pyproject.toml, use `-p/--python`
+option:
+
+```bash
+ ➜ pyproject2conda create -f tests/test-pyproject.toml -p
+channels:
+  - conda-forge
+dependencies:
+  - python>=3.8,<3.11
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+```
+
+To specify a value of python, pass a value with:
+
+```bash
+ ➜ pyproject2conda create -f tests/test-pyproject.toml -p python=3.9
+channels:
+  - conda-forge
+dependencies:
+  - python=3.9
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+```
+
 ```toml
 # ...
 [project.optional-dependencies]
 test = [
   "pandas",
   "pytest", # p2c: -c conda-forge
 
@@ -205,18 +237,19 @@
 `pyproject2conda` can also be used within python:
 
 ```pycon
 >>> from pyproject2conda import PyProject2Conda
 >>> p = PyProject2Conda.from_path("./tests/test-pyproject.toml")
 
 # Basic environment
->>> print(p.to_conda_yaml().strip())
+>>> print(p.to_conda_yaml(python="get").strip())
 channels:
   - conda-forge
 dependencies:
+  - python>=3.8,<3.11
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
 
 # Environment with extras
@@ -333,14 +366,17 @@
 
 ╭─ Options ───────────────────────────────────────────────────────────────────╮
 │ --channel  -c  TEXT  conda channel.  Can be specified multiple times.       │
 │                      Overrides [tool.pyproject2conda.channels]              │
 │ --file     -f  PATH  input pyproject.toml file                              │
 │ --name     -n  TEXT  Name of conda env                                      │
 │ --output   -o  PATH  File to output results                                 │
+│ --python   -p  TEXT  if flag passed without options, include python spec    │
+│                      from pyproject.toml in output.  If value passed, use   │
+│                      this value of python in the output                     │
 │ --help               Show this message and exit.                            │
 ╰─────────────────────────────────────────────────────────────────────────────╯
 
 
  ➜ pyproject2conda isolated --help
 
  Usage: pyproject2conda isolated [OPTIONS] ISOLATED...
@@ -349,14 +385,17 @@
 
 ╭─ Options ───────────────────────────────────────────────────────────────────╮
 │ --channel  -c  TEXT  conda channel.  Can be specified multiple times.       │
 │                      Overrides [tool.pyproject2conda.channels]              │
 │ --file     -f  PATH  input pyproject.toml file                              │
 │ --name     -n  TEXT  Name of conda env                                      │
 │ --output   -o  PATH  File to output results                                 │
+│ --python   -p  TEXT  if flag passed without options, include python spec    │
+│                      from pyproject.toml in output.  If value passed, use   │
+│                      this value of python in the output                     │
 │ --help               Show this message and exit.                            │
 ╰─────────────────────────────────────────────────────────────────────────────╯
 
 ```
 
 <!-- end-docs -->
```

### Comparing `pyproject2conda-0.1.0/src/pyproject2conda.egg-info/SOURCES.txt` & `pyproject2conda-0.1.1/src/pyproject2conda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/tests/test-pyproject.toml` & `pyproject2conda-0.1.1/tests/test-pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.0/tests/test_cli.py` & `pyproject2conda-0.1.1/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,51 @@
   - pip
   - pip:
       - athing
     """
 
     assert (result.output) == dedent(expected)
 
+    # -p flag
+    result = runner.invoke(
+        app, ["create", "-f", str(ROOT / "test-pyproject.toml"), "-p"]
+    )
+
+    expected = """\
+channels:
+  - conda-forge
+dependencies:
+  - python>=3.8,<3.11
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+    """
+
+    assert (result.output) == dedent(expected)
+
+    result = runner.invoke(
+        app, ["create", "-f", str(ROOT / "test-pyproject.toml"), "-p", "python=3.8"]
+    )
+
+    expected = """\
+channels:
+  - conda-forge
+dependencies:
+  - python=3.8
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+    """
+
+    assert (result.output) == dedent(expected)
+
     result = runner.invoke(
         app, ["create", "-f", str(ROOT / "test-pyproject.toml"), "dev"]
     )
 
     expected = """\
 channels:
   - conda-forge
```

### Comparing `pyproject2conda-0.1.0/tests/test_parser.py` & `pyproject2conda-0.1.1/tests/test_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,14 +93,47 @@
   - pip
   - pip:
       - athing
     """
 
     assert dedent(expected) == out
 
+    # test -p option
+    out = d.to_conda_yaml(python="get")
+
+    expected = """\
+channels:
+  - conda-forge
+dependencies:
+  - python>=3.8,<3.11
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+    """
+
+    assert dedent(expected) == out
+
+    out = d.to_conda_yaml(python="python=3.9")
+
+    expected = """\
+channels:
+  - conda-forge
+dependencies:
+  - python=3.9
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+    """
+
+    assert dedent(expected) == out
+
     out = d.to_conda_yaml(channels="hello")
 
     expected = """\
 channels:
   - hello
 dependencies:
   - bthing-conda
```

### Comparing `pyproject2conda-0.1.0/tox.ini` & `pyproject2conda-0.1.1/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -116,18 +116,18 @@
     using either
     local: local
     remote: remote
     versions.
 skip_install = True
 conda_env    = {toxinidir}/environment/test-extras.yaml
 conda_deps =
-    conda-remote,condaforge-remote: {[base]package_name}{env:TEST_VERSION:''}
+    conda-remote,condaforge-remote: {[base]package_name}{env:TEST_VERSION:}
     conda-local,condaforge-local: {posargs}
 deps =
-    pypi-remote: {[base]package_name}{env:TEST_VERSION:''}
+    pypi-remote: {[base]package_name}{env:TEST_VERSION:}
     pypi-local: {posargs}
 
 [testenv:testpip-py3{8, 9, 10, 11}]
 description  =
     Test package against pip installed packages
 usedevelop   = True
 extras = test
```

