# Comparing `tmp/seveno-pyutil-0.8.0.tar.gz` & `tmp/seveno-pyutil-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seveno-pyutil-0.8.0.tar", last modified: Fri Feb 24 10:33:41 2023, max compression
+gzip compressed data, was "seveno-pyutil-0.8.1.tar", last modified: Wed Jun  7 13:24:51 2023, max compression
```

## Comparing `seveno-pyutil-0.8.0.tar` & `seveno-pyutil-0.8.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-24 10:33:41.060652 seveno-pyutil-0.8.0/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      307 2023-02-24 10:32:23.000000 seveno-pyutil-0.8.0/.bumpversion.cfg
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      427 2022-09-02 14:40:55.000000 seveno-pyutil-0.8.0/.readthedocs.yml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3396 2023-02-24 10:32:23.000000 seveno-pyutil-0.8.0/CHANGELOG.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1072 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.0/LICENSE
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      332 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.0/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2178 2023-02-24 10:33:41.060652 seveno-pyutil-0.8.0/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1128 2022-10-28 12:44:39.000000 seveno-pyutil-0.8.0/README.md
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-24 10:33:41.056652 seveno-pyutil-0.8.0/docs/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3396 2023-02-24 10:32:23.000000 seveno-pyutil-0.8.0/docs/CHANGELOG.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      613 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.0/docs/Makefile
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-24 10:33:41.056652 seveno-pyutil-0.8.0/docs/_static/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.0/docs/_static/.gitkeep
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-24 10:33:41.056652 seveno-pyutil-0.8.0/docs/_templates/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.0/docs/_templates/.gitkeep
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1349 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.0/docs/api.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1686 2023-02-24 10:32:23.000000 seveno-pyutil-0.8.0/docs/conf.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5575 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.0/docs/examples_and_usage.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      197 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.0/docs/index.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       48 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.0/docs/license.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      811 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.0/docs/make.bat
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2718 2023-02-24 10:32:23.000000 seveno-pyutil-0.8.0/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-02-24 10:33:41.064652 seveno-pyutil-0.8.0/setup.cfg
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       69 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.0/setup.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-24 10:33:41.052652 seveno-pyutil-0.8.0/src/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-24 10:33:41.060652 seveno-pyutil-0.8.0/src/seveno_pyutil/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      864 2023-02-24 10:32:23.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      631 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/benchmarking_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1322 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/collections_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5876 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/datetime_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     7235 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/error_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2796 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/file_utilities.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-24 10:33:41.060652 seveno-pyutil-0.8.0/src/seveno_pyutil/logging_utilities/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      220 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/logging_utilities/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2971 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/logging_utilities/pretty_formatter.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    12311 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/logging_utilities/sql_filter.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     1713 2023-02-24 09:53:12.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1318 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/logging_utilities/utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2906 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/metaprogramming_helpers.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      533 2017-10-23 09:03:29.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/os_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      503 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.0/src/seveno_pyutil/string_utilities.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-24 10:33:41.060652 seveno-pyutil-0.8.0/src/seveno_pyutil.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2178 2023-02-24 10:33:41.000000 seveno-pyutil-0.8.0/src/seveno_pyutil.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1454 2023-02-24 10:33:41.000000 seveno-pyutil-0.8.0/src/seveno_pyutil.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-02-24 10:33:41.000000 seveno-pyutil-0.8.0/src/seveno_pyutil.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2022-10-28 12:40:39.000000 seveno-pyutil-0.8.0/src/seveno_pyutil.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      368 2023-02-24 10:33:41.000000 seveno-pyutil-0.8.0/src/seveno_pyutil.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       14 2023-02-24 10:33:41.000000 seveno-pyutil-0.8.0/src/seveno_pyutil.egg-info/top_level.txt
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-24 10:33:41.060652 seveno-pyutil-0.8.0/tests/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       91 2017-09-26 08:22:57.000000 seveno-pyutil-0.8.0/tests/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      263 2018-03-29 15:58:00.000000 seveno-pyutil-0.8.0/tests/benchmarking_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      886 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.0/tests/collections_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      129 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.0/tests/conftest.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5585 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.0/tests/datetime_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3042 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.0/tests/error_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      472 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.0/tests/file_utilities_spec.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-24 10:33:41.060652 seveno-pyutil-0.8.0/tests/fixtures/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       50 2017-09-26 08:24:03.000000 seveno-pyutil-0.8.0/tests/fixtures/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      743 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.0/tests/metaprograming_helpers_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      529 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.0/tests/string_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      202 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.0/tests/test_helpers.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      307 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/.bumpversion.cfg
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      427 2022-09-02 14:40:55.000000 seveno-pyutil-0.8.1/.readthedocs.yml
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3503 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/CHANGELOG.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1072 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/LICENSE
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      332 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/MANIFEST.in
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2129 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/PKG-INFO
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1128 2022-10-28 12:44:39.000000 seveno-pyutil-0.8.1/README.md
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.712937 seveno-pyutil-0.8.1/docs/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3503 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/docs/CHANGELOG.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      613 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.1/docs/Makefile
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.712937 seveno-pyutil-0.8.1/docs/_static/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.1/docs/_static/.gitkeep
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.712937 seveno-pyutil-0.8.1/docs/_templates/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.1/docs/_templates/.gitkeep
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1349 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/docs/api.rst
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1686 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/docs/conf.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5575 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.1/docs/examples_and_usage.rst
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      197 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.1/docs/index.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       48 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.1/docs/license.rst
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      811 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.1/docs/make.bat
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2677 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/pyproject.toml
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/setup.cfg
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       69 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/setup.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.708937 seveno-pyutil-0.8.1/src/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.716937 seveno-pyutil-0.8.1/src/seveno_pyutil/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      883 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      631 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/benchmarking_utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1322 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/collections_utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5876 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/datetime_utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     7235 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/error_utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2796 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/file_utilities.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      235 2023-06-07 13:24:07.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2971 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/pretty_formatter.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    17011 2023-06-07 13:24:07.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/sql_filter.py
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     1713 2023-02-24 09:53:12.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1318 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2906 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/metaprogramming_helpers.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      533 2017-10-23 09:03:29.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/os_utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      503 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/string_utilities.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.716937 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2129 2023-06-07 13:24:51.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/PKG-INFO
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1454 2023-06-07 13:24:51.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-07 13:24:51.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-07 07:47:35.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/not-zip-safe
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      368 2023-06-07 13:24:51.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/requires.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       14 2023-06-07 13:24:51.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/top_level.txt
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/tests/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       91 2017-09-26 08:22:57.000000 seveno-pyutil-0.8.1/tests/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      263 2018-03-29 15:58:00.000000 seveno-pyutil-0.8.1/tests/benchmarking_utilities_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      886 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/collections_utilities_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      129 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/conftest.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5585 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.1/tests/datetime_utilities_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3042 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/error_utilities_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      472 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/file_utilities_spec.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/tests/fixtures/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       50 2017-09-26 08:24:03.000000 seveno-pyutil-0.8.1/tests/fixtures/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      743 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/metaprograming_helpers_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      529 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/string_utilities_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      202 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/test_helpers.py
```

### Comparing `seveno-pyutil-0.8.0/CHANGELOG.md` & `seveno-pyutil-0.8.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.8.1 (2023-06-07)
+
+- feat: SQLFiler can now sometimes print real SQL instead of query string + params
+
 ## 0.8.0 (2023-02-24)
 
 - feat: replaced logging formatters with `PrettyFormatter`
 - feat: added `next_working_day()`
 - feat: replaced dateutil timezones with `zoneinfo`
 - chore: added some `typing` annotations
```

### Comparing `seveno-pyutil-0.8.0/LICENSE` & `seveno-pyutil-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/PKG-INFO` & `seveno-pyutil-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: seveno-pyutil
-Version: 0.8.0
+Version: 0.8.1
 Summary: Various unsorted Python utilities
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/seveno_pyutil
 Project-URL: Documentation, https://seveno-pyutil.readthedocs.io/en/latest/
 Keywords: utilities
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 # Overview
```

### Comparing `seveno-pyutil-0.8.0/README.md` & `seveno-pyutil-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/docs/CHANGELOG.md` & `seveno-pyutil-0.8.1/docs/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.8.1 (2023-06-07)
+
+- feat: SQLFiler can now sometimes print real SQL instead of query string + params
+
 ## 0.8.0 (2023-02-24)
 
 - feat: replaced logging formatters with `PrettyFormatter`
 - feat: added `next_working_day()`
 - feat: replaced dateutil timezones with `zoneinfo`
 - chore: added some `typing` annotations
```

### Comparing `seveno-pyutil-0.8.0/docs/Makefile` & `seveno-pyutil-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/docs/api.rst` & `seveno-pyutil-0.8.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/docs/conf.py` & `seveno-pyutil-0.8.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime
 
 author = "tadams42"
 project = "seveno-pyutil"
 copyright = (
     ", ".join(str(y) for y in range(2017, datetime.now().year + 1)) + ", " + author
 )
-release = "0.8.0"
+release = "0.8.1"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
```

### Comparing `seveno-pyutil-0.8.0/docs/examples_and_usage.rst` & `seveno-pyutil-0.8.1/docs/examples_and_usage.rst`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/docs/make.bat` & `seveno-pyutil-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/pyproject.toml` & `seveno-pyutil-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "seveno-pyutil"
-version = "0.8.0"
+version = "0.8.1"
 description = "Various unsorted Python utilities"
 readme = "README.md"
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3",
-	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Programming Language :: Python :: 3 :: Only",
 	"Operating System :: OS Independent",
 	"Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
@@ -29,15 +28,15 @@
 	"pygments",
 	"python-dateutil>=2.6.0",
 	"sqlparse",
 	"tzlocal",
 ]
 keywords = ["utilities"]
 license = { text = "MIT" }
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 authors = [{ name = "Tomislav Adamic", email = "tomislav.adamic@gmail.com" }]
 
 
 [project.urls]
 Source = "https://github.com/tadams42/seveno_pyutil"
 Documentation = "https://seveno-pyutil.readthedocs.io/en/latest/"
```

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/__init__.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 
 import logging
 
 from .benchmarking_utilities import Stopwatch
 from .collections_utilities import in_batches
 from .datetime_utilities import ensure_tzinfo, iter_year_month
 from .error_utilities import ExceptionsAsErrors, add_error_to
@@ -11,14 +11,15 @@
     file_checksum,
     move_and_create_dest,
     silent_create_dirs,
     silent_remove,
     switch_extension,
 )
 from .logging_utilities import (
+    FlaskSQLStats,
     PrettyFormatter,
     SQLFilter,
     StandardMetadataFilter,
     log_to_console_for,
     log_to_tmp_file_for,
     silence_logger,
 )
```

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/benchmarking_utilities.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/benchmarking_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/collections_utilities.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/collections_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/datetime_utilities.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/datetime_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/error_utilities.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/error_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/file_utilities.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/file_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/logging_utilities/pretty_formatter.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/pretty_formatter.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/logging_utilities/sql_filter.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/sql_filter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,38 @@
+from __future__ import annotations
+
 import enum
 import logging
 import timeit
+from dataclasses import dataclass, field
 from datetime import date, datetime, timedelta
+from typing import TYPE_CHECKING, Callable, ClassVar, Final
 
 import pygments
 import sqlparse
 
 # from pygments.formatters import TerminalTrueColorFormatter
 from pygments.formatters import Terminal256Formatter
 from pygments.lexers import SqlLexer
 
 try:
     import simplejson as json
 except Exception:
     import json
 
+HAS_FLASK = False
+try:
+    import flask
 
-class JsonEncoder(json.JSONEncoder):
-    def default(self, o):
-        if isinstance(o, (date, datetime)):
-            return o.isoformat()
-        if isinstance(o, enum.Enum):
-            return o.name
-        return super().default(o)
+    HAS_FLASK = True
+except Exception:
+    pass
+
+if TYPE_CHECKING:
+    from sqlalchemy.engine import Connection, Engine
 
 
 class SQLFilter(logging.Filter):
     """
     Filter for Django's and SQLAlchemy SQL loggers. Reformats and colorizes
     queries.
 
@@ -120,20 +126,19 @@
                     'handlers': ['console_django']
                 }
             }
         })
 
     """
 
-    KEY_SQL_CUMULATIVE_DURATION = "cumulative_duration"
-    KEY_SQL_COUNT = "statements_count"
-
     @classmethod
     def register_sqlalchemy_logging_events(
-        cls, logger, duration_threshold_ms=None, statistics_ctx_get=None
+        cls,
+        logger: str | logging.Logger,
+        duration_threshold_ms: int | float | timedelta | None = None,
     ):
         """
         Must be called when logging SQLAlchemy statements and durations.
 
         Arguments:
             logger: name of logger or logging.Logger instance that will be used to log
                 SQL messages.
@@ -165,180 +170,343 @@
                             )
                             flask.g["sqlalchemy_statistics"] = {}
         """
 
         from sqlalchemy import event
         from sqlalchemy.engine import Engine
 
-        _logger = logger
-        if isinstance(logger, str):
-            _logger = logging.getLogger(logger)
-
-        if duration_threshold_ms is not None and not isinstance(
-            duration_threshold_ms, timedelta
-        ):
-            duration_threshold_ms = timedelta(milliseconds=duration_threshold_ms)
-
-        def duration_ms(conn):
-            if conn:
-                return timedelta(
-                    milliseconds=(
-                        timeit.default_timer() - conn.info["query_start_time"].pop(-1)
-                    )
-                    * 1000.0
-                )
-            else:
-                return timedelta(milliseconds=0)
+        connection_enricher = ConnectionEnricher(logger, duration_threshold_ms)
 
         @event.listens_for(Engine, "before_cursor_execute")
         def before_cursor_execute(
-            conn, cursor, statement, parameters, context, executemany
+            conn: Connection,
+            cursor: "DBAPICursor",
+            statement: str,
+            parameters: dict,
+            context: "ExecutionContext",
+            executemany: bool,
         ):
-            if conn:
-                conn.info.setdefault("query_start_time", []).append(
-                    timeit.default_timer()
-                )
+            connection_enricher.start(conn)
 
         @event.listens_for(Engine, "after_cursor_execute")
         def after_cursor_execute(
-            conn, cursor, statement, parameters, context, executemany
+            conn: Connection,
+            cursor: "DBAPICursor",
+            statement: str,
+            parameters: dict,
+            context: "ExecutionContext",
+            executemany: bool,
         ):
-            statement_duration = duration_ms(conn)
-
-            warned = False
-            if (
-                duration_threshold_ms is not None
-                and statement_duration >= duration_threshold_ms
-            ):
-                _logger.warning(
-                    "Detected SQL query running longer than {:.2f} ms! ".format(
-                        duration_threshold_ms.total_seconds() * 1000
-                    ),
-                    extra={
-                        "sql_statement": str(statement),
-                        "sql_parameters": str(parameters),
-                        "sql_duration_ms": statement_duration.total_seconds() * 1000,
-                    },
-                )
-                warned = True
-
-            if not warned and statement_duration is not None:
-                _logger.debug(
-                    "",
-                    extra={
-                        "sql_statement": str(statement),
-                        "sql_parameters": str(parameters),
-                        "sql_duration_ms": statement_duration.total_seconds() * 1000,
-                    },
-                )
-
-            if statistics_ctx_get:
-                try:
-                    data = statistics_ctx_get()
-                    data.setdefault(cls.KEY_SQL_CUMULATIVE_DURATION, timedelta())
-                    data.setdefault(cls.KEY_SQL_COUNT, 0)
-                    data[cls.KEY_SQL_CUMULATIVE_DURATION] += statement_duration
-                    data[cls.KEY_SQL_COUNT] += 1
-
-                except Exception:
-                    _logger.error("Failed to collect SQL statistics!", exc_info=True)
+            connection_enricher.end(conn, cursor, statement, parameters)
 
         @event.listens_for(Engine, "handle_error")
         def receive_handle_error(exception_context):
-            msg = "SQL engine exception detected."
-            try:
-                msg = msg + " " + str(exception_context.original_exception).strip()
-            except Exception:
-                msg = "SQL engine exception detected. "
-
-            _logger.critical(
-                msg,
-                extra={
-                    "sql_statement": str(exception_context.statement),
-                    "sql_parameters": str(exception_context.parameters),
-                    "sql_duration_ms": duration_ms(
-                        exception_context.connection
-                    ).total_seconds()
-                    * 1000,
-                },
-            )
+            connection_enricher.error(exception_context)
 
     def __init__(
         self,
         colorize_queries=False,
         multiline_queries=False,
         shorten_logs=True,
         *args,
         **kwargs,
     ):
+        self.enricher = RecordEnricher(
+            colorize_queries, multiline_queries, shorten_logs
+        )
+        super().__init__(*args, **kwargs)
+
+    def filter(self, record: logging.LogRecord):
+        self.enricher.add_attributes(record)
+        return super().filter(record)
+
+
+class ConnectionEnricher:
+    _ATTR_START_TIME = "query_start_time"
+
+    def __init__(
+        self,
+        lgr: str | logging.Logger,
+        duration_threshold: int | float | timedelta | None,
+    ):
+        self.lgr: logging.Logger
+        if isinstance(lgr, str):
+            self.lgr = logging.getLogger(lgr)
+        else:
+            self.lgr = lgr
+
+        self.duration_threshold: timedelta | None = None
+        if duration_threshold is not None:
+            if isinstance(duration_threshold, timedelta):
+                self.duration_threshold = duration_threshold
+            else:
+                self.duration_threshold = timedelta(milliseconds=duration_threshold)
+
+    def start(self, conn: Connection | None):
+        if conn:
+            conn.info.setdefault(self._ATTR_START_TIME, []).append(
+                timeit.default_timer()
+            )
+
+    def end(
+        self, conn: Connection, cursor: "DBAPICursor", statement: str, parameters: dict
+    ):
+        statement_duration = self._execution_duration(conn)
+        FlaskSQLStats.incr_stats(self.lgr, statement_duration)
+
+        compiled = None
+        try:
+            compiled = cursor.mogrify(statement, parameters).decode()
+        except Exception:
+            compiled = None
+
+        warned = False
+        if (
+            self.duration_threshold is not None
+            and statement_duration >= self.duration_threshold
+        ):
+            self.lgr.warning(
+                "Detected SQL query running longer than {:.2f} ms! ".format(
+                    self.duration_threshold.total_seconds() * 1000
+                ),
+                extra={
+                    RecordEnricher.ATTR_DATA: SQLRecordedQuery(
+                        statement=str(statement),
+                        parameters=parameters,
+                        duration=statement_duration,
+                        compiled=compiled,
+                    )
+                },
+            )
+            warned = True
+
+        if not warned and statement_duration is not None:
+            self.lgr.debug(
+                "",
+                extra={
+                    RecordEnricher.ATTR_DATA: SQLRecordedQuery(
+                        statement=str(statement),
+                        parameters=parameters,
+                        duration=statement_duration,
+                        compiled=compiled,
+                    )
+                },
+            )
+
+    def error(self, exception_context):
+        msg = "SQL engine exception detected."
+
+        try:
+            msg = msg + " " + str(exception_context.original_exception).strip()
+        except Exception:
+            msg = "SQL engine exception detected. "
+
+        self.lgr.critical(
+            msg,
+            extra={
+                RecordEnricher.ATTR_DATA: SQLRecordedQuery(
+                    statement=str(exception_context.statement),
+                    parameters=exception_context.parameters,
+                    duration=self._execution_duration(exception_context.connection),
+                )
+            },
+        )
+
+    @classmethod
+    def _execution_duration(cls, conn: Connection | None) -> timedelta:
+        data: list[float] = getattr(conn, "info", dict()).get(cls._ATTR_START_TIME, [])
+        started_at = data.pop(-1) if data else 0
+        return timedelta(milliseconds=(timeit.default_timer() - started_at) * 1000.0)
+
+
+@dataclass
+class SQLRecordedQuery:
+    statement: str
+    parameters: dict
+    duration: timedelta
+    compiled: str | None = None
+    duration_ms: float = field(init=False, default=0)
+
+    def __post_init__(self):
+        td = None
+        if isinstance(self.duration, (int, float, str)):
+            td = timedelta(microseconds=float(self.duration))
+        elif isinstance(self.duration, timedelta):
+            td = self.duration
+        else:
+            td = timedelta()
+        self.duration_ms = td.total_seconds() * 1000
+
+
+class RecordEnricher:
+    ATTR_DATA = "_sql"
+    ATTR_SQL = "sql"
+    ATTR_DURATION = "sql_duration"
+
+    def __init__(
+        self, colorize_queries=False, multiline_queries=False, shorten_logs=True
+    ):
         self.colorize_queries = colorize_queries
         self.multiline_queries = multiline_queries
         self.shorten_logs = shorten_logs
-        super().__init__(*args, **kwargs)
 
-    def filter(self, record):
-        sql = (
-            # SQLAlchemy
-            getattr(record, "sql_statement", None)
-            # Django
-            or getattr(record, "sql", None)
-            or ""
-        )
+    def add_attributes(self, record: logging.LogRecord):
+        setattr(record, self.ATTR_SQL, "")
+        setattr(record, self.ATTR_DURATION, "")
+
+        recorded_query: SQLRecordedQuery | None = getattr(record, self.ATTR_DATA, None)
+        if not recorded_query:
+            return
+
+        query_str = self._format_query_string(recorded_query)
+        setattr(record, self.ATTR_SQL, query_str)
+
+        duration_str = self._format_duration_string(recorded_query)
+        setattr(record, self.ATTR_DURATION, duration_str)
+
+    def _format_query_string(self, recorded_query: SQLRecordedQuery) -> str:
+        if recorded_query.compiled:
+            sql = self._format_compiled(recorded_query.compiled)
+            return sql
+
+        else:
+            sql = self._format_statement_and_params(
+                recorded_query.statement, recorded_query.parameters
+            )
+            return sql
 
+    def _maybe_multiline(self, sql: str) -> str:
         if sql:
             if self.multiline_queries:
                 sql = sqlparse.format(sql, reindent=True, keyword_case="upper").strip()
             else:
                 sql = " ".join(
                     l.strip()
                     for l in sqlparse.format(
                         sql, reindent=True, keyword_case="upper"
                     ).splitlines()
                 ).strip()
 
             if sql and not sql.endswith(";"):
                 sql = sql + ";"
 
-        if hasattr(record, "sql_parameters"):
-            params_dict = record.sql_parameters
-            params = json.dumps(record.sql_parameters, cls=JsonEncoder).strip()
+        return sql or ""
+
+    def _maybe_colorized(self, sql: str) -> str:
+        if self.colorize_queries and sql:
+            sql = pygments.highlight(
+                sql, SqlLexer(), Terminal256Formatter(style="monokai")
+            ).strip()
+
+        return sql or ""
+
+    def _format_compiled(self, compiled: str | None) -> str:
+        sql = compiled or ""
+
+        sql = self._maybe_multiline(sql)
+        sql = self._maybe_colorized(sql)
+
+        if self.shorten_logs:
+            (sql or " SQL")[:1300]
+
+        return sql
+
+    def _format_statement_and_params(
+        self, statement: str | None, parameters: dict | None
+    ) -> str:
+        sql: str = statement or ""
+
+        sql = self._maybe_multiline(sql)
+        sql = self._maybe_colorized(sql)
+
+        if parameters:
+            params_dict = parameters
+            params = json.dumps(params_dict, cls=JsonEncoder).strip()
         else:
             params_dict = {}
             params = ""
 
-        if self.colorize_queries:
-            if sql:
-                sql = pygments.highlight(
-                    sql, SqlLexer(), Terminal256Formatter(style="monokai")
-                ).strip()
-
-            if params:
-                params = pygments.highlight(
-                    params,
-                    pygments.lexers.get_lexer_for_mimetype("application/json"),
-                    Terminal256Formatter(style="monokai"),
-                ).strip()
+        if self.colorize_queries and params:
+            params = pygments.highlight(
+                params,
+                pygments.lexers.get_lexer_for_mimetype("application/json"),
+                Terminal256Formatter(style="monokai"),
+            ).strip()
 
         # rsyslogd limits to 2048 bytes per message by default
         # We prefer to lose some params when shortening log line than to lose some SQL
-        # statement content. Either way, it is not possible to guarnatee both will
+        # statement content. Either way, it is not possible to guarantee both will
         # be fully logged in all contexts and log sinks
         if params and params_dict:
             if self.shorten_logs:
-                record.sql = "{} with params {}".format(sql[:1500], params[:500])
+                sql = "{} with params {}".format(sql[:1500], params[:500])
             else:
                 # params should always be shortened because they can be huge in when
                 # for exmple we are inserting into PostgreSQL JSONB columns
-                record.sql = "{} with params {}".format(sql, params[:500])
+                sql = "{} with params {}".format(sql, params[:500])
         else:
-            record.sql = (sql or " SQL")[:1300]
+            sql = (sql or " SQL")[:1300]
 
-        duration = getattr(record, "sql_duration_ms", None) or getattr(
-            record, "duration", None
-        )
+        return sql
 
-        if duration:
-            record.sql_duration = "{:.2f} ms".format(duration)
-        else:
-            record.sql_duration = "_.___ ms"
+    def _format_duration_string(self, recorded_query: SQLRecordedQuery) -> str:
+        dur = "_.___ ms"
+        if recorded_query.duration_ms:
+            dur = "{:.2f} ms".format(recorded_query.duration_ms)
+        return dur
 
-        return super().filter(record)
+
+class FlaskSQLStats:
+    _KEY_REQUEST_SQL_STATS = "sqlalchemy_statistics"
+    _KEY_SQL_CUMULATIVE_DURATION = "cumulative_duration"
+    _KEY_SQL_COUNT = "statements_count"
+
+    @classmethod
+    def get_statements_count(cls) -> int:
+        stats = cls.get()
+        if stats:
+            return stats[cls._KEY_SQL_COUNT] or 0
+        return 0
+
+    @classmethod
+    def get_cumulative_statements_duration(cls) -> timedelta:
+        stats = FlaskSQLStats.get()
+        if stats:
+            return stats[cls._KEY_SQL_CUMULATIVE_DURATION]
+        return timedelta()
+
+    @classmethod
+    def open(cls) -> dict | None:
+        if HAS_FLASK:
+            return flask.g.setdefault(cls._KEY_REQUEST_SQL_STATS, dict())
+
+    @classmethod
+    def close(cls):
+        if HAS_FLASK:
+            flask.g.pop(cls._KEY_REQUEST_SQL_STATS)
+
+    @classmethod
+    def get(cls) -> dict | None:
+        if HAS_FLASK:
+            return flask.g.get(cls._KEY_REQUEST_SQL_STATS)
+
+    @classmethod
+    def incr_stats(cls, lgr: logging.Logger, statement_duration: timedelta):
+        if HAS_FLASK:
+            try:
+                data = cls.open()
+                data.setdefault(cls._KEY_SQL_CUMULATIVE_DURATION, timedelta())
+                data.setdefault(cls._KEY_SQL_COUNT, 0)
+                data[cls._KEY_SQL_CUMULATIVE_DURATION] += statement_duration
+                data[cls._KEY_SQL_COUNT] += 1
+
+            except Exception:
+                lgr.error("Failed to collect SQL statistics!", exc_info=True)
+
+
+class JsonEncoder(json.JSONEncoder):
+    def default(self, o):
+        if isinstance(o, (date, datetime)):
+            return o.isoformat()
+        if isinstance(o, enum.Enum):
+            return o.name
+        return super().default(o)
```

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/logging_utilities/utilities.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/metaprogramming_helpers.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/metaprogramming_helpers.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil/os_utilities.py` & `seveno-pyutil-0.8.1/src/seveno_pyutil/os_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil.egg-info/PKG-INFO` & `seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: seveno-pyutil
-Version: 0.8.0
+Version: 0.8.1
 Summary: Various unsorted Python utilities
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/seveno_pyutil
 Project-URL: Documentation, https://seveno-pyutil.readthedocs.io/en/latest/
 Keywords: utilities
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 # Overview
```

### Comparing `seveno-pyutil-0.8.0/src/seveno_pyutil.egg-info/SOURCES.txt` & `seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/tests/collections_utilities_spec.py` & `seveno-pyutil-0.8.1/tests/collections_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/tests/datetime_utilities_spec.py` & `seveno-pyutil-0.8.1/tests/datetime_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/tests/error_utilities_spec.py` & `seveno-pyutil-0.8.1/tests/error_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/tests/metaprograming_helpers_spec.py` & `seveno-pyutil-0.8.1/tests/metaprograming_helpers_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.0/tests/string_utilities_spec.py` & `seveno-pyutil-0.8.1/tests/string_utilities_spec.py`

 * *Files identical despite different names*

