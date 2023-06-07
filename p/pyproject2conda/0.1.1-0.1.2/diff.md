# Comparing `tmp/pyproject2conda-0.1.1.tar.gz` & `tmp/pyproject2conda-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject2conda-0.1.1.tar", last modified: Wed Jun  7 18:25:15 2023, max compression
+gzip compressed data, was "pyproject2conda-0.1.2.tar", last modified: Wed Jun  7 21:01:46 2023, max compression
```

## Comparing `pyproject2conda-0.1.1.tar` & `pyproject2conda-0.1.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.923139 pyproject2conda-0.1.1/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.1.1/.cruft.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/.editorconfig
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.870581 pyproject2conda-0.1.1/.github/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      367 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.1.1/.gitignore
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      465 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/AUTHORS.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      178 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/CHANGELOG.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/LICENSE
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/MANIFEST.in
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11480 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/Makefile
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14929 2023-06-07 18:25:15.922321 pyproject2conda-0.1.1/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12136 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.870985 pyproject2conda-0.1.1/changelog.d/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.871380 pyproject2conda-0.1.1/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.872353 pyproject2conda-0.1.1/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.877330 pyproject2conda-0.1.1/docs/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/Makefile
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.856168 pyproject2conda-0.1.1/docs/_static/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.877867 pyproject2conda-0.1.1/docs/_static/css/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.879555 pyproject2conda-0.1.1/docs/_static/js/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.885167 pyproject2conda-0.1.1/docs/_templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.889095 pyproject2conda-0.1.1/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.891038 pyproject2conda-0.1.1/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/authors.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/changelog.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/conf.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.892504 pyproject2conda-0.1.1/docs/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      536 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/docs/examples/example-usage.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.893214 pyproject2conda-0.1.1/docs/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      241 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      936 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/docs/installation.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/license.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/make.bat
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.893854 pyproject2conda-0.1.1/docs/reference/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      143 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/reference/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.903206 pyproject2conda-0.1.1/environment/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      943 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      260 2023-06-07 14:20:27.000000 pyproject2conda-0.1.1/environment/dev.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      574 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      377 2023-06-07 14:20:28.000000 pyproject2conda-0.1.1/environment/docs.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      153 2023-06-07 14:20:29.000000 pyproject2conda-0.1.1/environment/lint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      144 2023-06-07 14:20:29.000000 pyproject2conda-0.1.1/environment/test.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/environment/tools.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      148 2023-06-07 14:20:17.000000 pyproject2conda-0.1.1/environment.yaml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.903998 pyproject2conda-0.1.1/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/examples/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.904742 pyproject2conda-0.1.1/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6304 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/pyproject.toml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.909471 pyproject2conda-0.1.1/scripts/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      846 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/lint.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/recipe-append.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-06-07 18:25:15.923399 pyproject2conda-0.1.1/setup.cfg
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.859799 pyproject2conda-0.1.1/src/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.911498 pyproject2conda-0.1.1/src/pyproject2conda/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      648 2023-06-07 15:56:44.000000 pyproject2conda-0.1.1/src/pyproject2conda/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3062 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/src/pyproject2conda/cli.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12606 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/src/pyproject2conda/parser.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.916877 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14929 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2413 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       60 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/entry_points.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      109 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       16 2023-06-07 18:25:15.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-05 17:19:50.000000 pyproject2conda-0.1.1/src/pyproject2conda.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-07 18:25:15.921119 pyproject2conda-0.1.1/tests/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       45 2023-06-05 16:53:11.000000 pyproject2conda-0.1.1/tests/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      611 2023-06-07 02:50:51.000000 pyproject2conda-0.1.1/tests/test-pyproject.toml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2694 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/tests/test_cli.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3738 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/tests/test_parser.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4101 2023-06-07 18:24:18.000000 pyproject2conda-0.1.1/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.938294 pyproject2conda-0.1.2/
+-rw-r--r--   0 wpk      (42033)    36681     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.1.2/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/.editorconfig
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.883517 pyproject2conda-0.1.2/.github/
+-rw-r--r--   0 wpk      (42033)    36681      367 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033)    36681     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.1.2/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      465 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681      178 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      258 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681    11480 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/Makefile
+-rw-r--r--   0 wpk      (42033)    36681    14929 2023-06-07 21:01:46.937458 pyproject2conda-0.1.2/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681    12136 2023-06-07 18:24:18.000000 pyproject2conda-0.1.2/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.883962 pyproject2conda-0.1.2/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.884371 pyproject2conda-0.1.2/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.885176 pyproject2conda-0.1.2/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.890953 pyproject2conda-0.1.2/docs/
+-rw-r--r--   0 wpk      (42033)    36681     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/Makefile
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.870567 pyproject2conda-0.1.2/docs/_static/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.891501 pyproject2conda-0.1.2/docs/_static/css/
+-rw-r--r--   0 wpk      (42033)    36681     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.893232 pyproject2conda-0.1.2/docs/_static/js/
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033)    36681      706 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.897324 pyproject2conda-0.1.2/docs/_templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.901163 pyproject2conda-0.1.2/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033)    36681      289 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      249 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033)    36681      405 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033)    36681      424 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      374 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.903355 pyproject2conda-0.1.2/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033)    36681      106 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033)    36681     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033)    36681     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033)    36681     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033)    36681     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033)    36681     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033)    36681     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681       69 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/authors.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/changelog.md
+-rw-r--r--   0 wpk      (42033)    36681    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/conf.py
+-rw-r--r--   0 wpk      (42033)    36681       74 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.904833 pyproject2conda-0.1.2/docs/examples/
+-rw-r--r--   0 wpk      (42033)    36681      536 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/docs/examples/example-usage.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.905703 pyproject2conda-0.1.2/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033)    36681      241 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/index.md
+-rw-r--r--   0 wpk      (42033)    36681      936 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/docs/installation.md
+-rw-r--r--   0 wpk      (42033)    36681       40 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/license.md
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/make.bat
+-rw-r--r--   0 wpk      (42033)    36681      169 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.906452 pyproject2conda-0.1.2/docs/reference/
+-rw-r--r--   0 wpk      (42033)    36681      143 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.915353 pyproject2conda-0.1.2/environment/
+-rw-r--r--   0 wpk      (42033)    36681      943 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      260 2023-06-07 14:20:27.000000 pyproject2conda-0.1.2/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      108 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681       79 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      574 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      377 2023-06-07 14:20:28.000000 pyproject2conda-0.1.2/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681       53 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      153 2023-06-07 14:20:29.000000 pyproject2conda-0.1.2/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033)    36681       25 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      144 2023-06-07 14:20:29.000000 pyproject2conda-0.1.2/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      299 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033)    36681      148 2023-06-07 14:20:17.000000 pyproject2conda-0.1.2/environment.yaml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.916065 pyproject2conda-0.1.2/examples/
+-rw-r--r--   0 wpk      (42033)    36681      222 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/examples/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.916831 pyproject2conda-0.1.2/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033)    36681     6304 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/pyproject.toml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.922848 pyproject2conda-0.1.2/scripts/
+-rw-r--r--   0 wpk      (42033)    36681      846 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033)    36681      312 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033)    36681     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681      266 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033)    36681      598 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033)    36681       91 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033)    36681      489 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033)    36681       38 2023-06-07 21:01:46.938481 pyproject2conda-0.1.2/setup.cfg
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.873853 pyproject2conda-0.1.2/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.927662 pyproject2conda-0.1.2/src/pyproject2conda/
+-rw-r--r--   0 wpk      (42033)    36681      648 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/src/pyproject2conda/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     3091 2023-06-07 21:01:07.000000 pyproject2conda-0.1.2/src/pyproject2conda/cli.py
+-rw-r--r--   0 wpk      (42033)    36681    12606 2023-06-07 18:24:18.000000 pyproject2conda-0.1.2/src/pyproject2conda/parser.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.933031 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681    14929 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2413 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681       60 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/entry_points.txt
+-rw-r--r--   0 wpk      (42033)    36681      109 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681       16 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-06-05 17:19:50.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.936422 pyproject2conda-0.1.2/tests/
+-rw-r--r--   0 wpk      (42033)    36681       45 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/tests/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681      611 2023-06-07 02:50:51.000000 pyproject2conda-0.1.2/tests/test-pyproject.toml
+-rw-r--r--   0 wpk      (42033)    36681     2694 2023-06-07 18:24:18.000000 pyproject2conda-0.1.2/tests/test_cli.py
+-rw-r--r--   0 wpk      (42033)    36681     3738 2023-06-07 18:24:18.000000 pyproject2conda-0.1.2/tests/test_parser.py
+-rw-r--r--   0 wpk      (42033)    36681     4101 2023-06-07 18:24:18.000000 pyproject2conda-0.1.2/tox.ini
```

### Comparing `pyproject2conda-0.1.1/.cruft.json` & `pyproject2conda-0.1.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/.editorconfig` & `pyproject2conda-0.1.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/.gitignore` & `pyproject2conda-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/.pre-commit-config.yaml` & `pyproject2conda-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/CONTRIBUTING.md` & `pyproject2conda-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/LICENSE` & `pyproject2conda-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/Makefile` & `pyproject2conda-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/PKG-INFO` & `pyproject2conda-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject2conda
-Version: 0.1.1
+Version: 0.1.2
 Summary: A script to convert a Python project declared on a pyproject.toml to a conda environment.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/wpk-nist-gov/pyproject2conda
 Project-URL: documentation, https://pages.nist.gov/pyproject2conda/
 Keywords: pyproject2conda
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pyproject2conda-0.1.1/README.md` & `pyproject2conda-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/changelog.d/templates/auto-changelog/template.jinja2` & `pyproject2conda-0.1.2/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/Makefile` & `pyproject2conda-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_static/css/nist-combined.css` & `pyproject2conda-0.1.2/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_static/js/leave_notice.js` & `pyproject2conda-0.1.2/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_static/js/nist-header-footer.js` & `pyproject2conda-0.1.2/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_templates/autosummary/class.rst` & `pyproject2conda-0.1.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_templates/autosummary/module.rst` & `pyproject2conda-0.1.2/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_templates/class-individual-pages.rst` & `pyproject2conda-0.1.2/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_templates/class-single-page.rst` & `pyproject2conda-0.1.2/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_templates/custom-module-template.rst` & `pyproject2conda-0.1.2/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_templates/module-custom-imported.rst` & `pyproject2conda-0.1.2/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_templates/module-custom.rst` & `pyproject2conda-0.1.2/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_templates/module-single.rst` & `pyproject2conda-0.1.2/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/_templates/module-template.rst` & `pyproject2conda-0.1.2/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/conf.py` & `pyproject2conda-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/examples/example-usage.md` & `pyproject2conda-0.1.2/docs/examples/example-usage.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/examples/usage/demo.ipynb` & `pyproject2conda-0.1.2/docs/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/installation.md` & `pyproject2conda-0.1.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/docs/make.bat` & `pyproject2conda-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/environment/dev-extras.yaml` & `pyproject2conda-0.1.2/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/environment/docs-extras.yaml` & `pyproject2conda-0.1.2/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/examples/usage/demo.ipynb` & `pyproject2conda-0.1.2/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/pyproject.toml` & `pyproject2conda-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/scripts/dist-conda.mk` & `pyproject2conda-0.1.2/scripts/dist-conda.mk`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/scripts/docs-examples-symlinks.sh` & `pyproject2conda-0.1.2/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/scripts/recipe-append.sh` & `pyproject2conda-0.1.2/scripts/recipe-append.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/src/pyproject2conda/__init__.py` & `pyproject2conda-0.1.2/src/pyproject2conda/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/src/pyproject2conda/cli.py` & `pyproject2conda-0.1.2/src/pyproject2conda/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,16 @@
     python,
 ):
     """Create yaml file from [tool.pyproject2conda.isolated-dependencies]"""
 
     if not channel:
         channel = None
     d = PyProject2Conda.from_path(filename)
-    s = d.to_conda_yaml(isolated=isolated, channels=channel, name=name, python=python)
+    s = d.to_conda_yaml(
+        isolated=isolated, channels=channel, name=name, python=python, stream=output
+    )
     if not output:
         click.echo(s, nl=False)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pyproject2conda-0.1.1/src/pyproject2conda/parser.py` & `pyproject2conda-0.1.2/src/pyproject2conda/parser.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/src/pyproject2conda.egg-info/PKG-INFO` & `pyproject2conda-0.1.2/src/pyproject2conda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject2conda
-Version: 0.1.1
+Version: 0.1.2
 Summary: A script to convert a Python project declared on a pyproject.toml to a conda environment.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/wpk-nist-gov/pyproject2conda
 Project-URL: documentation, https://pages.nist.gov/pyproject2conda/
 Keywords: pyproject2conda
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pyproject2conda-0.1.1/src/pyproject2conda.egg-info/SOURCES.txt` & `pyproject2conda-0.1.2/src/pyproject2conda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/tests/test-pyproject.toml` & `pyproject2conda-0.1.2/tests/test-pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/tests/test_cli.py` & `pyproject2conda-0.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/tests/test_parser.py` & `pyproject2conda-0.1.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.1/tox.ini` & `pyproject2conda-0.1.2/tox.ini`

 * *Files identical despite different names*

