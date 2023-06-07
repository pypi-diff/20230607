# Comparing `tmp/seveno-pyutil-0.8.1.tar.gz` & `tmp/seveno-pyutil-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seveno-pyutil-0.8.1.tar", last modified: Wed Jun  7 13:24:51 2023, max compression
+gzip compressed data, was "seveno-pyutil-0.8.2.tar", last modified: Wed Jun  7 13:58:55 2023, max compression
```

## Comparing `seveno-pyutil-0.8.1.tar` & `seveno-pyutil-0.8.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      307 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/.bumpversion.cfg
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      427 2022-09-02 14:40:55.000000 seveno-pyutil-0.8.1/.readthedocs.yml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3503 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/CHANGELOG.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1072 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/LICENSE
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      332 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2129 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1128 2022-10-28 12:44:39.000000 seveno-pyutil-0.8.1/README.md
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.712937 seveno-pyutil-0.8.1/docs/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3503 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/docs/CHANGELOG.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      613 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.1/docs/Makefile
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.712937 seveno-pyutil-0.8.1/docs/_static/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.1/docs/_static/.gitkeep
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.712937 seveno-pyutil-0.8.1/docs/_templates/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.1/docs/_templates/.gitkeep
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1349 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/docs/api.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1686 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/docs/conf.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5575 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.1/docs/examples_and_usage.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      197 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.1/docs/index.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       48 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.1/docs/license.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      811 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.1/docs/make.bat
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2677 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/setup.cfg
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       69 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/setup.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.708937 seveno-pyutil-0.8.1/src/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.716937 seveno-pyutil-0.8.1/src/seveno_pyutil/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      883 2023-06-07 13:24:15.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      631 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/benchmarking_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1322 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/collections_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5876 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/datetime_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     7235 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/error_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2796 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/file_utilities.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      235 2023-06-07 13:24:07.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2971 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/pretty_formatter.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    17011 2023-06-07 13:24:07.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/sql_filter.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     1713 2023-02-24 09:53:12.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1318 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2906 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/metaprogramming_helpers.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      533 2017-10-23 09:03:29.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/os_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      503 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.1/src/seveno_pyutil/string_utilities.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.716937 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2129 2023-06-07 13:24:51.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1454 2023-06-07 13:24:51.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-07 13:24:51.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-07 07:47:35.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      368 2023-06-07 13:24:51.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       14 2023-06-07 13:24:51.000000 seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/top_level.txt
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/tests/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       91 2017-09-26 08:22:57.000000 seveno-pyutil-0.8.1/tests/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      263 2018-03-29 15:58:00.000000 seveno-pyutil-0.8.1/tests/benchmarking_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      886 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/collections_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      129 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/conftest.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5585 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.1/tests/datetime_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3042 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/error_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      472 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/file_utilities_spec.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:24:51.720937 seveno-pyutil-0.8.1/tests/fixtures/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       50 2017-09-26 08:24:03.000000 seveno-pyutil-0.8.1/tests/fixtures/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      743 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/metaprograming_helpers_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      529 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/string_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      202 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.1/tests/test_helpers.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.991728 seveno-pyutil-0.8.2/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      307 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/.bumpversion.cfg
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-07 13:58:04.000000 seveno-pyutil-0.8.2/.readthedocs.yml
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3582 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/CHANGELOG.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1072 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/LICENSE
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      332 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/MANIFEST.in
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2129 2023-06-07 13:58:55.991728 seveno-pyutil-0.8.2/PKG-INFO
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1128 2022-10-28 12:44:39.000000 seveno-pyutil-0.8.2/README.md
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.983728 seveno-pyutil-0.8.2/docs/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3582 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/docs/CHANGELOG.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      613 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.2/docs/Makefile
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.983728 seveno-pyutil-0.8.2/docs/_static/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.2/docs/_static/.gitkeep
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.983728 seveno-pyutil-0.8.2/docs/_templates/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.2/docs/_templates/.gitkeep
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1349 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/docs/api.rst
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1686 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/docs/conf.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5575 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.2/docs/examples_and_usage.rst
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      197 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.2/docs/index.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       48 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.2/docs/license.rst
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      811 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.2/docs/make.bat
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2677 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/pyproject.toml
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-07 13:58:55.991728 seveno-pyutil-0.8.2/setup.cfg
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       69 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/setup.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.979728 seveno-pyutil-0.8.2/src/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.987728 seveno-pyutil-0.8.2/src/seveno_pyutil/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      883 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      631 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/benchmarking_utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1322 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/collections_utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5876 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/datetime_utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     7235 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/error_utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2796 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/file_utilities.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.987728 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      235 2023-06-07 13:24:07.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2971 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/pretty_formatter.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    15725 2023-06-07 13:58:04.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/sql_filter.py
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     1713 2023-02-24 09:53:12.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1318 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2906 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/metaprogramming_helpers.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      533 2017-10-23 09:03:29.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/os_utilities.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      503 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/string_utilities.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.987728 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2129 2023-06-07 13:58:55.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/PKG-INFO
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1454 2023-06-07 13:58:55.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-07 13:58:55.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-07 07:47:35.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/not-zip-safe
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      368 2023-06-07 13:58:55.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/requires.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       14 2023-06-07 13:58:55.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/top_level.txt
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.991728 seveno-pyutil-0.8.2/tests/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       91 2017-09-26 08:22:57.000000 seveno-pyutil-0.8.2/tests/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      263 2018-03-29 15:58:00.000000 seveno-pyutil-0.8.2/tests/benchmarking_utilities_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      886 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/collections_utilities_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      129 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/conftest.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5585 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.2/tests/datetime_utilities_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3042 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/error_utilities_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      472 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/file_utilities_spec.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.991728 seveno-pyutil-0.8.2/tests/fixtures/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       50 2017-09-26 08:24:03.000000 seveno-pyutil-0.8.2/tests/fixtures/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      743 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/metaprograming_helpers_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      529 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/string_utilities_spec.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      202 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/test_helpers.py
```

### Comparing `seveno-pyutil-0.8.1/CHANGELOG.md` & `seveno-pyutil-0.8.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.8.2 (2023-06-07)
+
+- feat: prettier format for multiline SQL in SQLFilter
+
 ## 0.8.1 (2023-06-07)
 
 - feat: SQLFiler can now sometimes print real SQL instead of query string + params
 
 ## 0.8.0 (2023-02-24)
 
 - feat: replaced logging formatters with `PrettyFormatter`
```

### Comparing `seveno-pyutil-0.8.1/LICENSE` & `seveno-pyutil-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/PKG-INFO` & `seveno-pyutil-0.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seveno-pyutil
-Version: 0.8.1
+Version: 0.8.2
 Summary: Various unsorted Python utilities
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/seveno_pyutil
 Project-URL: Documentation, https://seveno-pyutil.readthedocs.io/en/latest/
 Keywords: utilities
 Platform: any
```

### Comparing `seveno-pyutil-0.8.1/README.md` & `seveno-pyutil-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/docs/CHANGELOG.md` & `seveno-pyutil-0.8.2/docs/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.8.2 (2023-06-07)
+
+- feat: prettier format for multiline SQL in SQLFilter
+
 ## 0.8.1 (2023-06-07)
 
 - feat: SQLFiler can now sometimes print real SQL instead of query string + params
 
 ## 0.8.0 (2023-02-24)
 
 - feat: replaced logging formatters with `PrettyFormatter`
```

### Comparing `seveno-pyutil-0.8.1/docs/Makefile` & `seveno-pyutil-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/docs/api.rst` & `seveno-pyutil-0.8.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/docs/conf.py` & `seveno-pyutil-0.8.2/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime
 
 author = "tadams42"
 project = "seveno-pyutil"
 copyright = (
     ", ".join(str(y) for y in range(2017, datetime.now().year + 1)) + ", " + author
 )
-release = "0.8.1"
+release = "0.8.2"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
```

### Comparing `seveno-pyutil-0.8.1/docs/examples_and_usage.rst` & `seveno-pyutil-0.8.2/docs/examples_and_usage.rst`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/docs/make.bat` & `seveno-pyutil-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/pyproject.toml` & `seveno-pyutil-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "seveno-pyutil"
-version = "0.8.1"
+version = "0.8.2"
 description = "Various unsorted Python utilities"
 readme = "README.md"
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
```

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/__init__.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 import logging
 
 from .benchmarking_utilities import Stopwatch
 from .collections_utilities import in_batches
 from .datetime_utilities import ensure_tzinfo, iter_year_month
 from .error_utilities import ExceptionsAsErrors, add_error_to
```

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/benchmarking_utilities.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/benchmarking_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/collections_utilities.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/collections_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/datetime_utilities.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/datetime_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/error_utilities.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/error_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/file_utilities.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/file_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/pretty_formatter.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/pretty_formatter.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/sql_filter.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/sql_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,23 +29,15 @@
 
 if TYPE_CHECKING:
     from sqlalchemy.engine import Connection, Engine
 
 
 class SQLFilter(logging.Filter):
     """
-    Filter for Django's and SQLAlchemy SQL loggers. Reformats and colorizes
-    queries.
-
-    To use it with Django:
-
-    - add it to ``django.db.backends`` and ``django.db.backends.schema``
-      loggers
-    - remove ``%(message)s`` from log format because it will cause to double
-      emit each SQL statement. Use this filter's placeholder's instead.
+    Filter for SQLAlchemy SQL loggers. Optionally reformats and colorizes queries.
 
     To use it with SQLAlchemy:
 
     - add it to ``sqlalchemy.engine`` logger and call
       `:meth:register_sqlalchemy_logging_events`
 
     Supports following logging placeholders:
@@ -79,55 +71,37 @@
         except ImportError:
             pass
 
         dictConfig({
             'version': 1,
             'disable_existing_loggers': False,
             'formatters': {
-                'django_sql': {'format': '(%(sql_duration)s) %(sql)s'},
                 'sqlalchemy_sql': {'format': '(%(sql_duration)s) %(sql)s %(message)s'}
             },
             'filters': {
                 'colored_sql': {
                     '()': 'seveno_pyutil.SQLFilter'
                     'colorize_queries': True,
                     'multiline_queries': True,
                 }
             },
             'handlers': {
-                'console_django': {
-                    'class': 'logging.StreamHandler',
-                    'level': 'DEBUG',
-                    'formatter': 'django_sql',
-                    'filters': ['colored_sql'],
-                    'stream': 'ext://sys.stdout'
-                },
                 'console_sqlalchemy': {
                     'class': 'logging.StreamHandler',
                     'level': 'DEBUG',
                     'formatter': 'sqlalchemy_sql',
                     'filters': ['colored_sql'],
                     'stream': 'ext://sys.stdout'
                 }
             },
             'loggers': {
                 'myapp.db': {
                     'level': 'DEBUG',
                     'propagate': False,
                     'handlers': ['console_sqlalchemy']
-                },
-                'django.db.backends': {
-                    'level': 'DEBUG',
-                    'propagate': False,
-                    'handlers': ['console_django']
-                },
-                'django.db.backends.schema': {
-                    'level': 'DEBUG',
-                    'propagate': False,
-                    'handlers': ['console_django']
                 }
             }
         })
 
     """
 
     @classmethod
@@ -147,32 +121,21 @@
             statistics_ctx_get: callable that returns mutable dict. If given, then each
                 time SQL query is executes, this dict will be updated.
 
                 It can be used for example in Flask to track SQL execution statistics
                 during one HTTP request::
 
                     import flask
-                    from seveno_pyutil import register_sqlalchemy_logging_events
-
-                    def sqlalchemy_stats():
-                        return flask.g.setdefault("sqlalchemy_statistics", {})
+                    from seveno_pyutil import FlaskSQLStats, SQLFilter
 
-                    register_sqlalchemy_logging_events(
-                        "may_app_sql_logger", statistics_ctx_get=sqlalchemy_stats
+                    SQLFilter.register_sqlalchemy_logging_events(
+                        "may_app_sql_logger", 100
                     )
 
-                    @flask.before_request
-                    def track_sqlalchemy():
-                        @flask.after_this_request
-                        def log_sqlalchemy_stats(response):
-                            logger.info(
-                                "SQLAlchemy statistics for request %s",
-                                sqlalchemy_stats()
-                            )
-                            flask.g["sqlalchemy_statistics"] = {}
+                    db.session.execute("select * from books")
         """
 
         from sqlalchemy import event
         from sqlalchemy.engine import Engine
 
         connection_enricher = ConnectionEnricher(logger, duration_threshold_ms)
 
@@ -370,24 +333,35 @@
 
         else:
             sql = self._format_statement_and_params(
                 recorded_query.statement, recorded_query.parameters
             )
             return sql
 
+    _SQL_FORMAT_OPTS = {
+        "reindent": True,
+        "keyword_case": "upper",
+        "truncate_strings": 25,
+        "reindent_aligned": True,
+        "wrap_after": 88,
+    }
+
     def _maybe_multiline(self, sql: str) -> str:
         if sql:
             if self.multiline_queries:
-                sql = sqlparse.format(sql, reindent=True, keyword_case="upper").strip()
+                sql = "\n".join(
+                    l.rstrip()
+                    for l in sqlparse.format(sql, **self._SQL_FORMAT_OPTS).splitlines()
+                    if l.strip()
+                ).strip()
             else:
                 sql = " ".join(
                     l.strip()
-                    for l in sqlparse.format(
-                        sql, reindent=True, keyword_case="upper"
-                    ).splitlines()
+                    for l in sqlparse.format(sql, **self._SQL_FORMAT_OPTS).splitlines()
+                    if l.strip()
                 ).strip()
 
             if sql and not sql.endswith(";"):
                 sql = sql + ";"
 
         return sql or ""
```

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/logging_utilities/utilities.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/metaprogramming_helpers.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/metaprogramming_helpers.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil/os_utilities.py` & `seveno-pyutil-0.8.2/src/seveno_pyutil/os_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/PKG-INFO` & `seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seveno-pyutil
-Version: 0.8.1
+Version: 0.8.2
 Summary: Various unsorted Python utilities
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/seveno_pyutil
 Project-URL: Documentation, https://seveno-pyutil.readthedocs.io/en/latest/
 Keywords: utilities
 Platform: any
```

### Comparing `seveno-pyutil-0.8.1/src/seveno_pyutil.egg-info/SOURCES.txt` & `seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/tests/collections_utilities_spec.py` & `seveno-pyutil-0.8.2/tests/collections_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/tests/datetime_utilities_spec.py` & `seveno-pyutil-0.8.2/tests/datetime_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/tests/error_utilities_spec.py` & `seveno-pyutil-0.8.2/tests/error_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/tests/metaprograming_helpers_spec.py` & `seveno-pyutil-0.8.2/tests/metaprograming_helpers_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.1/tests/string_utilities_spec.py` & `seveno-pyutil-0.8.2/tests/string_utilities_spec.py`

 * *Files identical despite different names*

