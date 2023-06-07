# Comparing `tmp/json_explorer-0.0.2a0.tar.gz` & `tmp/json_explorer-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_explorer-0.0.2a0.tar", max compression
+gzip compressed data, was "json_explorer-0.0.3a0.tar", max compression
```

## Comparing `json_explorer-0.0.2a0.tar` & `json_explorer-0.0.3a0.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-06-05 22:24:50.705204 json_explorer-0.0.2a0/LICENSE
--rw-r--r--   0        0        0     2692 2023-06-05 22:24:50.705204 json_explorer-0.0.2a0/README.md
--rw-r--r--   0        0        0        0 2023-06-05 22:24:50.705204 json_explorer-0.0.2a0/json_explorer/__init__.py
--rw-r--r--   0        0        0      267 2023-06-05 22:24:50.705204 json_explorer-0.0.2a0/json_explorer/foo.py
--rw-r--r--   0        0        0     1875 2023-06-05 22:25:16.642382 json_explorer-0.0.2a0/pyproject.toml
--rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 json_explorer-0.0.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-07 01:09:26.744383 json_explorer-0.0.3a0/LICENSE
+-rw-r--r--   0        0        0      923 2023-06-07 01:09:26.744383 json_explorer-0.0.3a0/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 01:09:26.744383 json_explorer-0.0.3a0/json_explorer/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-07 01:09:26.744383 json_explorer-0.0.3a0/json_explorer/__main__.py
+-rw-r--r--   0        0        0     2055 2023-06-07 01:09:26.744383 json_explorer-0.0.3a0/json_explorer/cli.py
+-rw-r--r--   0        0        0    13487 2023-06-07 01:09:26.744383 json_explorer-0.0.3a0/json_explorer/explore.py
+-rw-r--r--   0        0        0     3602 2023-06-07 01:09:26.744383 json_explorer-0.0.3a0/json_explorer/style.css
+-rw-r--r--   0        0        0     1160 2023-06-07 01:09:26.744383 json_explorer-0.0.3a0/json_explorer/template.html
+-rw-r--r--   0        0        0     1687 2023-06-07 01:09:57.780549 json_explorer-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0     1681 1970-01-01 00:00:00.000000 json_explorer-0.0.3a0/PKG-INFO
```

### Comparing `json_explorer-0.0.2a0/LICENSE` & `json_explorer-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `json_explorer-0.0.2a0/pyproject.toml` & `json_explorer-0.0.3a0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 name = "json_explorer"
-version = "v0.0.2-alpha"
+version = "v0.0.3-alpha"
 description = "Explore the structure of a bunch of jsons"
 authors = ["Mike Stringer <fmike.stringer.internet@gmail.com>"]
 repository = "https://github.com/stringertheory/json-explorer"
 documentation = "https://stringertheory.github.io/json-explorer/"
 readme = "README.md"
 packages = [
   {include = "json_explorer"}
 ]
 
+[tool.poetry.scripts]
+greet = "json_explorer.explore:main"
+
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.7,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
-deptry = "^0.6.4"
-mypy = "^0.981"
 pre-commit = "^2.20.0"
 tox = "^3.25.1"
+beautifulsoup4 = "^4.12.2"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.5.10"
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 
 [build-system]
@@ -31,24 +33,14 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
 preview = true
 
-[tool.mypy]
-files = ["json_explorer"]
-disallow_untyped_defs = "True"
-disallow_any_unimported = "True"
-no_implicit_optional = "True"
-check_untyped_defs = "True"
-warn_return_any = "True"
-warn_unused_ignores = "True"
-show_error_codes = "True"
-
 [tool.ruff]
 target-version = "py37"
 line-length = 120
 fix = true
 select = [
     # flake8-2020
     "YTT",
```

