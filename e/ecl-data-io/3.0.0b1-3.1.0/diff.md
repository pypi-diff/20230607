# Comparing `tmp/ecl-data-io-3.0.0b1.tar.gz` & `tmp/ecl-data-io-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecl-data-io-3.0.0b1.tar", last modified: Thu Apr 27 09:57:52 2023, max compression
+gzip compressed data, was "ecl-data-io-3.1.0.tar", last modified: Wed Jun  7 07:18:18 2023, max compression
```

## Comparing `ecl-data-io-3.0.0b1.tar` & `ecl-data-io-3.1.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.981689 ecl-data-io-3.0.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.973688 ecl-data-io-3.0.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.973688 ecl-data-io-3.0.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-27 09:57:52.981689 ecl-data-io-3.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.973688 ecl-data-io-3.0.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.977689 ecl-data-io-3.0.0b1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/api_doc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/developer_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/error_handling.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/example_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/docs/source/the_file_format.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-27 09:57:52.981689 ecl-data-io-3.0.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.973688 ecl-data-io-3.0.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.977689 ecl-data-io-3.0.0b1/src/ecl_data_io/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.977689 ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.977689 ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/array_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/src/ecl_data_io/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.977689 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-27 09:57:52.000000 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-27 09:57:52.000000 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:57:52.000000 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 09:57:52.000000 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 09:57:52.000000 ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:52.981689 ecl-data-io-3.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_formatted_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_formatted_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_formatted_read_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_formatted_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_read_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_type_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_unformatted_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_unformatted_read_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_unformatted_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 09:57:42.000000 ecl-data-io-3.0.0b1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:18.531672 ecl-data-io-3.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:18.519672 ecl-data-io-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:18.523672 ecl-data-io-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-07 07:18:18.531672 ecl-data-io-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:18.523672 ecl-data-io-3.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:18.527672 ecl-data-io-3.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/docs/source/api_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/docs/source/developer_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/docs/source/error_handling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/docs/source/example_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/docs/source/the_file_format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-07 07:18:18.531672 ecl-data-io-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:18.519672 ecl-data-io-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:18.527672 ecl-data-io-3.1.0/src/ecl_data_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:18.527672 ecl-data-io-3.1.0/src/ecl_data_io/_formatted/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/_formatted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/_formatted/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/_formatted/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:18.527672 ecl-data-io-3.1.0/src/ecl_data_io/_unformatted/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/_unformatted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/_unformatted/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/_unformatted/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/_unformatted/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/array_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/src/ecl_data_io/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:18.527672 ecl-data-io-3.1.0/src/ecl_data_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-07 07:18:18.000000 ecl-data-io-3.1.0/src/ecl_data_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-07 07:18:18.000000 ecl-data-io-3.1.0/src/ecl_data_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:18:18.000000 ecl-data-io-3.1.0/src/ecl_data_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-07 07:18:18.000000 ecl-data-io-3.1.0/src/ecl_data_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 07:18:18.000000 ecl-data-io-3.1.0/src/ecl_data_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:18.531672 ecl-data-io-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_formatted_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_formatted_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_formatted_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_formatted_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_type_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_unformatted_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_unformatted_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_unformatted_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-07 07:18:08.000000 ecl-data-io-3.1.0/tox.ini
```

### Comparing `ecl-data-io-3.0.0b1/.github/workflows/publish_to_pypi.yml` & `ecl-data-io-3.1.0/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/.github/workflows/testing.yml` & `ecl-data-io-3.1.0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/LICENSE.md` & `ecl-data-io-3.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/PKG-INFO` & `ecl-data-io-3.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecl-data-io
-Version: 3.0.0b1
+Version: 3.1.0
 Summary: A (lazy) parser and writer for the ecl output format.
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>
 License: LGPL-3.0
 Project-URL: Homepage, https://github.com/equinor/ecl-data-io
 Project-URL: Repository, https://github.com/equinor/ecl-data-io
 Project-URL: Documentation, https://ecl-data-io.readthedocs.io/en/stable/
```

### Comparing `ecl-data-io-3.0.0b1/README.md` & `ecl-data-io-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/docs/source/developer_guide.rst` & `ecl-data-io-3.1.0/docs/source/developer_guide.rst`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,14 @@
     pip install -e .
 
 Second, install the dev-requirements.txt, which contains the packages ecl-data-io
 require in order to run tests:
 
 .. code-block:: console
 
-    pip install -r dev-requirements.txt
+    pip install -e ".[dev]"
 
 At last, you can use pytest to run the tests
 
 .. code-block:: console
 
     pytest tests
```

### Comparing `ecl-data-io-3.0.0b1/docs/source/error_handling.rst` & `ecl-data-io-3.1.0/docs/source/error_handling.rst`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/docs/source/example_usage.rst` & `ecl-data-io-3.1.0/docs/source/example_usage.rst`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/docs/source/index.rst` & `ecl-data-io-3.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/docs/source/the_file_format.rst` & `ecl-data-io-3.1.0/docs/source/the_file_format.rst`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/pyproject.toml` & `ecl-data-io-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/read.py` & `ecl-data-io-3.1.0/src/ecl_data_io/_formatted/read.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io/_formatted/write.py` & `ecl-data-io-3.1.0/src/ecl_data_io/_formatted/write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/common.py` & `ecl-data-io-3.1.0/src/ecl_data_io/_unformatted/common.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/read.py` & `ecl-data-io-3.1.0/src/ecl_data_io/_unformatted/read.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io/_unformatted/write.py` & `ecl-data-io-3.1.0/src/ecl_data_io/_unformatted/write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io/array_entry.py` & `ecl-data-io-3.1.0/src/ecl_data_io/array_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Optional, Union
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike
 
-    from .types import ArrayValue
+    from .types import ReadArrayValue
 
 
 class EclArray(ABC):
     """
     An array entry in a ecl file.
 
     This class is not ment to be constructed directly, but rather
@@ -58,15 +58,15 @@
         :returns: The length of the array in number of entries.
         """
         if self._length is None:
             self._read()
         return self._length  # type: ignore
 
     @abstractmethod
-    def read_array(self) -> "ArrayValue":
+    def read_array(self) -> "ReadArrayValue":
         """
         Read the array from the unformatted ecl file.
 
         :returns: numpy array of values.
         """
         pass
```

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io/format.py` & `ecl-data-io-3.1.0/src/ecl_data_io/format.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io/read.py` & `ecl-data-io-3.1.0/src/ecl_data_io/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from ecl_data_io._formatted.read import FormattedEclArray
 from ecl_data_io._unformatted.read import UnformattedEclArray
 from ecl_data_io.array_entry import EclArray
 from ecl_data_io.format import Format, check_correct_mode, get_stream, guess_format
 
 if TYPE_CHECKING:
-    from .types import ArrayValue
+    from .types import ReadArrayValue
 
 
-def read(*args, **kwargs) -> List[Tuple[str, "ArrayValue"]]:
+def read(*args, **kwargs) -> List[Tuple[str, "ReadArrayValue"]]:
     """
     Read the contents of a ecl file and return a list of
     tuples (keyword, array). Takes the same parameters as
     lazy_read, but differs in return type
     """
     return [
         (arr.read_keyword(), arr.read_array()) for arr in lazy_read(*args, **kwargs)
```

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io/types.py` & `ecl-data-io-3.1.0/src/ecl_data_io/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     The MESS value is a sentinell object used to signal that the type of the
     array that is to be written should be an empty array of type MESS.
     """
 
     pass
 
 
-ArrayValue = Union[ArrayLike, MESS]
+ReadArrayValue = Union[np.ndarray, MESS]
+WriteArrayValue = Union[ArrayLike, MESS]
 
 
 def to_np_type(type_keyword):
     """
     :param type_keyword: A bytestring of a ecl type.
     :returns: A np dtype corresponding to the given
         ecl type.
```

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io/write.py` & `ecl-data-io-3.1.0/src/ecl_data_io/write.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Dict, Sequence, Tuple, Union
 
 from ecl_data_io._formatted.write import formatted_write
 from ecl_data_io._unformatted.write import unformatted_write
 from ecl_data_io.format import Format, check_correct_mode, get_stream
 
-from .types import ArrayValue
+from .types import WriteArrayValue
 
 
 def write(
     filelike,
-    contents: Union[Sequence[Tuple[str, ArrayValue]], Dict[str, ArrayValue]],
+    contents: Union[Sequence[Tuple[str, WriteArrayValue]], Dict[str, WriteArrayValue]],
     fileformat: Format = Format.UNFORMATTED,
 ):
     """
     Write the given contents to the given file in ecl format.
 
     :param filelike: Either filename, pathlib.Path or stream
         to write file to. For fileformat=Format.UNFORMATTED the
```

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/PKG-INFO` & `ecl-data-io-3.1.0/src/ecl_data_io.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecl-data-io
-Version: 3.0.0b1
+Version: 3.1.0
 Summary: A (lazy) parser and writer for the ecl output format.
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>
 License: LGPL-3.0
 Project-URL: Homepage, https://github.com/equinor/ecl-data-io
 Project-URL: Repository, https://github.com/equinor/ecl-data-io
 Project-URL: Documentation, https://ecl-data-io.readthedocs.io/en/stable/
```

### Comparing `ecl-data-io-3.0.0b1/src/ecl_data_io.egg-info/SOURCES.txt` & `ecl-data-io-3.1.0/src/ecl_data_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/generators.py` & `ecl-data-io-3.1.0/tests/generators.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/test_error_handling.py` & `ecl-data-io-3.1.0/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/test_formatted_common.py` & `ecl-data-io-3.1.0/tests/test_formatted_common.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/test_formatted_read.py` & `ecl-data-io-3.1.0/tests/test_formatted_read.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/test_formatted_read_write.py` & `ecl-data-io-3.1.0/tests/test_formatted_read_write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/test_formatted_write.py` & `ecl-data-io-3.1.0/tests/test_formatted_write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/test_read_write.py` & `ecl-data-io-3.1.0/tests/test_read_write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/test_type_resolution.py` & `ecl-data-io-3.1.0/tests/test_type_resolution.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/test_types.py` & `ecl-data-io-3.1.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/test_unformatted_read.py` & `ecl-data-io-3.1.0/tests/test_unformatted_read.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/test_unformatted_read_write.py` & `ecl-data-io-3.1.0/tests/test_unformatted_read_write.py`

 * *Files identical despite different names*

### Comparing `ecl-data-io-3.0.0b1/tests/test_unformatted_write.py` & `ecl-data-io-3.1.0/tests/test_unformatted_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     "array, expected_array",
     [
         (np.array([1], dtype=np.int32), np.array([1], dtype=np.int32)),
         (np.array([1.0], dtype=np.float32), np.array([1.0], dtype=np.float32)),
         (np.array([1.0], dtype=np.float64), np.array([1.0], dtype=np.float64)),
         (np.array([True, False], dtype=np.bool_), np.array([-1, 0], dtype=np.int32)),
         (np.array([10, 20], dtype=np.int8), np.array([10, 20], dtype=np.int32)),
-        (np.array([1.0], dtype=np.float128), np.array([1.0], dtype=np.float64)),
+        (np.array([1.0], dtype=np.longdouble), np.array([1.0], dtype=np.float64)),
     ],
 )
 def test_cast_array_to_ecl(array, expected_array):
     assert np.array_equal(ecl_unf_write.cast_array_to_ecl(array), expected_array)
 
 
 def test_cast_array_to_ecl_bad_type():
```

### Comparing `ecl-data-io-3.0.0b1/tests/test_update.py` & `ecl-data-io-3.1.0/tests/test_update.py`

 * *Files identical despite different names*

