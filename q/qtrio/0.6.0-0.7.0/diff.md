# Comparing `tmp/qtrio-0.6.0.tar.gz` & `tmp/qtrio-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtrio-0.6.0.tar", last modified: Mon Nov 21 15:09:58 2022, max compression
+gzip compressed data, was "qtrio-0.7.0.tar", last modified: Wed Jun  7 15:36:38 2023, max compression
```

## Comparing `qtrio-0.6.0.tar` & `qtrio-0.7.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.942835 qtrio-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-11-21 15:09:36.000000 qtrio-0.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-21 15:09:36.000000 qtrio-0.6.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-11-21 15:09:36.000000 qtrio-0.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-11-21 15:09:36.000000 qtrio-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-21 15:09:36.000000 qtrio-0.6.0/LICENSE.APACHE2
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-11-21 15:09:36.000000 qtrio-0.6.0/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-11-21 15:09:36.000000 qtrio-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10305 2022-11-21 15:09:58.942835 qtrio-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8249 2022-11-21 15:09:36.000000 qtrio-0.6.0/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     1126 2022-11-21 15:09:36.000000 qtrio-0.6.0/check.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     3393 2022-11-21 15:09:36.000000 qtrio-0.6.0/ci.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.926835 qtrio-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.930835 qtrio-0.6.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     8683 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/core.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.930835 qtrio-0.6.0/docs/source/development/
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/development/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/development/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/development/reviewing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2457 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/development/testing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/development/use_latest_docs.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/dialogs.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.930835 qtrio-0.6.0/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/examples/download.rst
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/examples/emissions.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/examples/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/examples/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3793 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6650 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/lifetimes.rst
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-11-21 15:09:36.000000 qtrio-0.6.0/docs/source/testing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-11-21 15:09:36.000000 qtrio-0.6.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.930835 qtrio-0.6.0/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-11-21 15:09:36.000000 qtrio-0.6.0/newsfragments/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-21 15:09:36.000000 qtrio-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-11-21 15:09:36.000000 qtrio-0.6.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.934835 qtrio-0.6.0/qtrio/
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    26219 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3078 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_python.py
--rw-r--r--   0 runner    (1001) docker     (121)     4603 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_qt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.938835 qtrio-0.6.0/qtrio/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.938835 qtrio-0.6.0/qtrio/_tests/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.938835 qtrio-0.6.0/qtrio/_tests/examples/readme/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/examples/readme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/examples/readme/test_console.py
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/examples/readme/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/examples/readme/test_qtrio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/examples/test_buildingrespect.py
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/examples/test_crossingpaths.py
--rw-r--r--   0 runner    (1001) docker     (121)     8322 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/examples/test_download.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/examples/test_emissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    32020 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)    11894 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/test_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/test_pytest.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_tests/test_qtrio.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    24237 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.942835 qtrio-0.6.0/qtrio/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/examples/buildingrespect.py
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/examples/crossingpaths.py
--rw-r--r--   0 runner    (1001) docker     (121)     9509 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/examples/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/examples/emissions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.942835 qtrio-0.6.0/qtrio/examples/readme/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/examples/readme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/examples/readme/console.py
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/examples/readme/qt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/examples/readme/qtrio_example.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-11-21 15:09:36.000000 qtrio-0.6.0/qtrio/qt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:09:58.934835 qtrio-0.6.0/qtrio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10305 2022-11-21 15:09:58.000000 qtrio-0.6.0/qtrio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-11-21 15:09:58.000000 qtrio-0.6.0/qtrio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 15:09:58.000000 qtrio-0.6.0/qtrio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-21 15:09:58.000000 qtrio-0.6.0/qtrio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-11-21 15:09:58.000000 qtrio-0.6.0/qtrio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-21 15:09:58.000000 qtrio-0.6.0/qtrio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-11-21 15:09:58.942835 qtrio-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-21 15:09:36.000000 qtrio-0.6.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-11-21 15:09:36.000000 qtrio-0.6.0/towncrier.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.602129 qtrio-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-07 15:36:20.000000 qtrio-0.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 15:36:20.000000 qtrio-0.7.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-07 15:36:20.000000 qtrio-0.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-07 15:36:20.000000 qtrio-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-07 15:36:20.000000 qtrio-0.7.0/LICENSE.APACHE2
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-07 15:36:20.000000 qtrio-0.7.0/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-07 15:36:20.000000 qtrio-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-06-07 15:36:38.602129 qtrio-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-07 15:36:20.000000 qtrio-0.7.0/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1126 2023-06-07 15:36:20.000000 qtrio-0.7.0/check.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3393 2023-06-07 15:36:20.000000 qtrio-0.7.0/ci.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.594127 qtrio-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.598128 qtrio-0.7.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/core.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.598128 qtrio-0.7.0/docs/source/development/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/development/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/development/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/development/reviewing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/development/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/development/use_latest_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/dialogs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.598128 qtrio-0.7.0/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/examples/download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/examples/emissions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/examples/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/examples/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/lifetimes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-07 15:36:20.000000 qtrio-0.7.0/docs/source/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-07 15:36:20.000000 qtrio-0.7.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.598128 qtrio-0.7.0/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-07 15:36:20.000000 qtrio-0.7.0/newsfragments/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-07 15:36:20.000000 qtrio-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-07 15:36:20.000000 qtrio-0.7.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.598128 qtrio-0.7.0/qtrio/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26193 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_qt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.602129 qtrio-0.7.0/qtrio/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.602129 qtrio-0.7.0/qtrio/_tests/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.602129 qtrio-0.7.0/qtrio/_tests/examples/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/examples/readme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/examples/readme/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/examples/readme/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/examples/readme/test_qtrio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/examples/test_buildingrespect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/examples/test_crossingpaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/examples/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/examples/test_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/test_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_tests/test_qtrio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.602129 qtrio-0.7.0/qtrio/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/examples/buildingrespect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/examples/crossingpaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/examples/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/examples/emissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.602129 qtrio-0.7.0/qtrio/examples/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/examples/readme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/examples/readme/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/examples/readme/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/examples/readme/qtrio_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 15:36:20.000000 qtrio-0.7.0/qtrio/qt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:36:38.602129 qtrio-0.7.0/qtrio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-06-07 15:36:38.000000 qtrio-0.7.0/qtrio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-07 15:36:38.000000 qtrio-0.7.0/qtrio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:36:38.000000 qtrio-0.7.0/qtrio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 15:36:38.000000 qtrio-0.7.0/qtrio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-07 15:36:38.000000 qtrio-0.7.0/qtrio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 15:36:38.000000 qtrio-0.7.0/qtrio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-07 15:36:38.606130 qtrio-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 15:36:20.000000 qtrio-0.7.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-07 15:36:20.000000 qtrio-0.7.0/towncrier.toml
```

### Comparing `qtrio-0.6.0/LICENSE.APACHE2` & `qtrio-0.7.0/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/LICENSE.MIT` & `qtrio-0.7.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/PKG-INFO` & `qtrio-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtrio
-Version: 0.6.0
+Version: 0.7.0
 Summary: a library bringing Qt GUIs together with ``async`` and ``await`` via Trio
 Home-page: https://github.com/altendky/qtrio
 Author: Kyle Altendorf
 Author-email: sda@fstab.net
 License: MIT -or- Apache License 2.0
 Project-URL: Documentation, https://qtrio.readthedocs.io/
 Project-URL: Chat, https://gitter.im/python-trio/general
```

### Comparing `qtrio-0.6.0/README.rst` & `qtrio-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/check.sh` & `qtrio-0.7.0/check.sh`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/ci.sh` & `qtrio-0.7.0/ci.sh`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/Makefile` & `qtrio-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/make.bat` & `qtrio-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/source/conf.py` & `qtrio-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/source/core.rst` & `qtrio-0.7.0/docs/source/core.rst`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/source/development/contributing.rst` & `qtrio-0.7.0/docs/source/development/contributing.rst`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/source/development/releasing.rst` & `qtrio-0.7.0/docs/source/development/releasing.rst`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/source/development/reviewing.rst` & `qtrio-0.7.0/docs/source/development/reviewing.rst`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/source/development/testing.rst` & `qtrio-0.7.0/docs/source/development/testing.rst`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/source/dialogs.rst` & `qtrio-0.7.0/docs/source/dialogs.rst`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/source/exceptions.rst` & `qtrio-0.7.0/docs/source/exceptions.rst`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/source/getting_started.rst` & `qtrio-0.7.0/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/docs/source/history.rst` & `qtrio-0.7.0/docs/source/history.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 Release history
 ===============
 
 .. currentmodule:: qtrio
 
 .. towncrier release notes start
 
+QTrio 0.7.0 (2023-06-07)
+------------------------
+
+For contributors
+~~~~~~~~~~~~~~~~
+
+- Updated to support trio-typing 0.8.0. (`#283 <https://github.com/altendky/qtrio/issues/283>`__)
+
+
 QTrio 0.6.0 (2022-11-21)
 ------------------------
 
 Headline features
 ~~~~~~~~~~~~~~~~~
 
 - Added support for CPython 3.10 and 3.11.
```

### Comparing `qtrio-0.6.0/docs/source/lifetimes.rst` & `qtrio-0.7.0/docs/source/lifetimes.rst`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/mypy.ini` & `qtrio-0.7.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/newsfragments/README.rst` & `qtrio-0.7.0/newsfragments/README.rst`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/__init__.py` & `qtrio-0.7.0/qtrio/__init__.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_cli.py` & `qtrio-0.7.0/qtrio/_cli.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_core.py` & `qtrio-0.7.0/qtrio/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,15 +648,15 @@
 
         trio.lowlevel.start_guest_run(
             self.trio_main,
             async_fn,
             args,
             run_sync_soon_threadsafe=self.run_sync_soon_threadsafe,
             done_callback=self.trio_done,
-            clock=self.clock,  # type: ignore[arg-type]
+            clock=self.clock,
             instruments=self.instruments,
         )
 
         if self.quit_application:
             self.application.aboutToQuit.connect(_early_quit_warning)
 
         if execute_application:
```

### Comparing `qtrio-0.6.0/qtrio/_exceptions.py` & `qtrio-0.7.0/qtrio/_exceptions.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_python.py` & `qtrio-0.7.0/qtrio/_python.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_qt.py` & `qtrio-0.7.0/qtrio/_qt.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/examples/readme/test_console.py` & `qtrio-0.7.0/qtrio/_tests/examples/readme/test_console.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/examples/readme/test_qt.py` & `qtrio-0.7.0/qtrio/_tests/examples/readme/test_qt.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/examples/readme/test_qtrio.py` & `qtrio-0.7.0/qtrio/_tests/examples/readme/test_qtrio.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/examples/test_buildingrespect.py` & `qtrio-0.7.0/qtrio/_tests/examples/test_buildingrespect.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/examples/test_crossingpaths.py` & `qtrio-0.7.0/qtrio/_tests/examples/test_crossingpaths.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/examples/test_download.py` & `qtrio-0.7.0/qtrio/_tests/examples/test_download.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/examples/test_emissions.py` & `qtrio-0.7.0/qtrio/_tests/examples/test_emissions.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/helpers.py` & `qtrio-0.7.0/qtrio/_tests/helpers.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/test_cli.py` & `qtrio-0.7.0/qtrio/_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/test_core.py` & `qtrio-0.7.0/qtrio/_tests/test_core.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/test_dialogs.py` & `qtrio-0.7.0/qtrio/_tests/test_dialogs.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/test_pytest.py` & `qtrio-0.7.0/qtrio/_tests/test_pytest.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/test_qt.py` & `qtrio-0.7.0/qtrio/_tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_tests/test_qtrio.py` & `qtrio-0.7.0/qtrio/_tests/test_qtrio.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/_util.py` & `qtrio-0.7.0/qtrio/_util.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/dialogs.py` & `qtrio-0.7.0/qtrio/dialogs.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/examples/buildingrespect.py` & `qtrio-0.7.0/qtrio/examples/buildingrespect.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/examples/crossingpaths.py` & `qtrio-0.7.0/qtrio/examples/crossingpaths.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/examples/download.py` & `qtrio-0.7.0/qtrio/examples/download.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/examples/emissions.py` & `qtrio-0.7.0/qtrio/examples/emissions.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/examples/readme/qt.py` & `qtrio-0.7.0/qtrio/examples/readme/qt.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/examples/readme/qtrio_example.py` & `qtrio-0.7.0/qtrio/examples/readme/qtrio_example.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio/qt.py` & `qtrio-0.7.0/qtrio/qt.py`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio.egg-info/PKG-INFO` & `qtrio-0.7.0/qtrio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtrio
-Version: 0.6.0
+Version: 0.7.0
 Summary: a library bringing Qt GUIs together with ``async`` and ``await`` via Trio
 Home-page: https://github.com/altendky/qtrio
 Author: Kyle Altendorf
 Author-email: sda@fstab.net
 License: MIT -or- Apache License 2.0
 Project-URL: Documentation, https://qtrio.readthedocs.io/
 Project-URL: Chat, https://gitter.im/python-trio/general
```

### Comparing `qtrio-0.6.0/qtrio.egg-info/SOURCES.txt` & `qtrio-0.7.0/qtrio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtrio-0.6.0/qtrio.egg-info/requires.txt` & `qtrio-0.7.0/qtrio.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 async_generator
 attrs
 decorator
 outcome
 qts~=0.3.0
-trio>=0.16
-trio-typing~=0.7.0
+trio>=0.17
+trio-typing~=0.8.0
 
 [:python_version < "3.8"]
 typing-extensions
 
 [cli]
 click~=8.1
```

### Comparing `qtrio-0.6.0/setup.cfg` & `qtrio-0.7.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 include_package_data = True
 install_requires = 
 	async_generator
 	attrs
 	decorator
 	outcome
 	qts ~= 0.3.0
-	trio >= 0.16
-	trio-typing ~= 0.7.0
+	trio >= 0.17
+	trio-typing ~= 0.8.0
 	typing-extensions; python_version < '3.8'
 packages = find:
 python_requires = >=3.7
 
 [options.entry_points]
 console_scripts = 
 	qtrio = qtrio._cli:cli
```

### Comparing `qtrio-0.6.0/towncrier.toml` & `qtrio-0.7.0/towncrier.toml`

 * *Files identical despite different names*

