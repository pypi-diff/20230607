# Comparing `tmp/trsfile-2.1.0.tar.gz` & `tmp/trsfile-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trsfile-2.1.0.tar", last modified: Tue Apr 26 15:02:29 2022, max compression
+gzip compressed data, was "trsfile-2.2.0.tar", last modified: Wed Jun  7 06:16:58 2023, max compression
```

## Comparing `trsfile-2.1.0.tar` & `trsfile-2.2.0.tar`

### file list

```diff
@@ -1,56 +1,69 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:29.000000 trsfile-2.1.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1265 2022-04-26 15:02:02.000000 trsfile-2.1.0/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2022-04-26 15:02:02.000000 trsfile-2.1.0/.readthedocs.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1053 2022-04-26 15:02:02.000000 trsfile-2.1.0/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2022-04-26 15:02:02.000000 trsfile-2.1.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)    11220 2022-04-26 15:02:29.000000 trsfile-2.1.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    10390 2022-04-26 15:02:02.000000 trsfile-2.1.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:29.000000 trsfile-2.1.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2022-04-26 15:02:02.000000 trsfile-2.1.0/docs/Makefile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:29.000000 trsfile-2.1.0/docs/_static/
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2022-04-26 15:02:02.000000 trsfile-2.1.0/docs/_static/.gitkeep
--rw-rw-r--   0 travis    (2000) travis    (2000)      350 2022-04-26 15:02:02.000000 trsfile-2.1.0/docs/_static/theme_overrides.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:29.000000 trsfile-2.1.0/docs/_templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2022-04-26 15:02:02.000000 trsfile-2.1.0/docs/_templates/.gitkeep
--rw-rw-r--   0 travis    (2000) travis    (2000)     1692 2022-04-26 15:02:02.000000 trsfile-2.1.0/docs/api.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5327 2022-04-26 15:02:02.000000 trsfile-2.1.0/docs/conf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:29.000000 trsfile-2.1.0/docs/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8242 2022-04-26 15:02:02.000000 trsfile-2.1.0/docs/images/overview.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1471 2022-04-26 15:02:02.000000 trsfile-2.1.0/docs/images/overview.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      486 2022-04-26 15:02:02.000000 trsfile-2.1.0/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      775 2022-04-26 15:02:02.000000 trsfile-2.1.0/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2022-04-26 15:02:02.000000 trsfile-2.1.0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1019 2022-04-26 15:02:29.000000 trsfile-2.1.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-04-26 15:02:02.000000 trsfile-2.1.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:29.000000 trsfile-2.1.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:02.000000 trsfile-2.1.0/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:29.000000 trsfile-2.1.0/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)   182709 2022-04-26 15:02:02.000000 trsfile-2.1.0/tests/data/90x500xfloat.trs
--rw-rw-r--   0 travis    (2000) travis    (2000)    19850 2022-04-26 15:02:02.000000 trsfile-2.1.0/tests/test_creation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      930 2022-04-26 15:02:02.000000 trsfile-2.1.0/tests/test_generic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6410 2022-04-26 15:02:02.000000 trsfile-2.1.0/tests/test_header.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7629 2022-04-26 15:02:02.000000 trsfile-2.1.0/tests/test_parameter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11212 2022-04-26 15:02:02.000000 trsfile-2.1.0/tests/test_parametermap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1043 2022-04-26 15:02:02.000000 trsfile-2.1.0/tests/test_trace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1555 2022-04-26 15:02:02.000000 trsfile-2.1.0/tests/test_trsfile.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:29.000000 trsfile-2.1.0/trsfile/
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2022-04-26 15:02:11.000000 trsfile-2.1.0/trsfile/VERSION.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13854 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/common.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:29.000000 trsfile-2.1.0/trsfile/engine/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/engine/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3887 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/engine/engine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8477 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/engine/file.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27556 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/engine/trs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18475 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/parametermap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5857 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/standardparameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3868 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/trace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4587 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/trace_set.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10395 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/traceparameter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2022-04-26 15:02:02.000000 trsfile-2.1.0/trsfile/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-26 15:02:29.000000 trsfile-2.1.0/trsfile.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11220 2022-04-26 15:02:29.000000 trsfile-2.1.0/trsfile.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      939 2022-04-26 15:02:29.000000 trsfile-2.1.0/trsfile.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-04-26 15:02:29.000000 trsfile-2.1.0/trsfile.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2022-04-26 15:02:29.000000 trsfile-2.1.0/trsfile.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2022-04-26 15:02:29.000000 trsfile-2.1.0/trsfile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.637845 trsfile-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.617845 trsfile-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.625845 trsfile-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-07 06:16:45.000000 trsfile-2.2.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-07 06:16:45.000000 trsfile-2.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-07 06:16:45.000000 trsfile-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-07 06:16:45.000000 trsfile-2.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-07 06:16:45.000000 trsfile-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-07 06:16:58.637845 trsfile-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-06-07 06:16:45.000000 trsfile-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.617845 trsfile-2.2.0/dev_docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.625845 trsfile-2.2.0/dev_docs/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-07 06:16:45.000000 trsfile-2.2.0/dev_docs/decisions/0000-use-markdown-architectural-decision-records.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-07 06:16:45.000000 trsfile-2.2.0/dev_docs/decisions/0001-change-cicd-pipeline-service-provider.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-07 06:16:45.000000 trsfile-2.2.0/dev_docs/decisions/adr-template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-07 06:16:45.000000 trsfile-2.2.0/dev_docs/decisions/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.625845 trsfile-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-07 06:16:45.000000 trsfile-2.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.629845 trsfile-2.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 06:16:45.000000 trsfile-2.2.0/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-07 06:16:45.000000 trsfile-2.2.0/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.629845 trsfile-2.2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 06:16:45.000000 trsfile-2.2.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-07 06:16:45.000000 trsfile-2.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-07 06:16:45.000000 trsfile-2.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.629845 trsfile-2.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-06-07 06:16:45.000000 trsfile-2.2.0/docs/images/overview.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-07 06:16:45.000000 trsfile-2.2.0/docs/images/overview.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-07 06:16:45.000000 trsfile-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-07 06:16:45.000000 trsfile-2.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 06:16:45.000000 trsfile-2.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.629845 trsfile-2.2.0/riscure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:45.000000 trsfile-2.2.0/riscure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-07 06:16:45.000000 trsfile-2.2.0/riscure/chipwhisperer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-07 06:16:58.637845 trsfile-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 06:16:45.000000 trsfile-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.633845 trsfile-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:45.000000 trsfile-2.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.633845 trsfile-2.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   182709 2023-06-07 06:16:45.000000 trsfile-2.2.0/tests/data/90x500xfloat.trs
+-rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-06-07 06:16:45.000000 trsfile-2.2.0/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 06:16:45.000000 trsfile-2.2.0/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-07 06:16:45.000000 trsfile-2.2.0/tests/test_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-06-07 06:16:45.000000 trsfile-2.2.0/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-06-07 06:16:45.000000 trsfile-2.2.0/tests/test_parametermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-07 06:16:45.000000 trsfile-2.2.0/tests/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-07 06:16:45.000000 trsfile-2.2.0/tests/test_trsfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.633845 trsfile-2.2.0/trsfile/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 06:16:58.000000 trsfile-2.2.0/trsfile/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.637845 trsfile-2.2.0/trsfile/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/engine/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/engine/trs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25490 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/parametermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/standardparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/trace_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/traceparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-07 06:16:45.000000 trsfile-2.2.0/trsfile/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:16:58.637845 trsfile-2.2.0/trsfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-07 06:16:58.000000 trsfile-2.2.0/trsfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-07 06:16:58.000000 trsfile-2.2.0/trsfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:16:58.000000 trsfile-2.2.0/trsfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 06:16:58.000000 trsfile-2.2.0/trsfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 06:16:58.000000 trsfile-2.2.0/trsfile.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `trsfile-2.1.0/.gitignore` & `trsfile-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/LICENSE` & `trsfile-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/PKG-INFO` & `trsfile-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: trsfile
-Version: 2.1.0
+Version: 2.2.0
 Summary: Library to read and create Riscure Inspector trace set files (.trs)
 Home-page: https://github.com/riscure/python-trsfile
 Maintainer: Riscure
 Maintainer-email: inforequest@riscure.com
 License: BSD 3-Clause Clear License
 Project-URL: Documentation, https://trsfile.readthedocs.io/en/latest
 Project-URL: Bug Reports, https://github.com/riscure/python-trsfile/issues
 Project-URL: Riscure, https://www.riscure.com
 Keywords: trs,trace,inspector,riscure
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: DEV
@@ -215,17 +214,20 @@
 	new_traces.extend(traces)         # Extend the new trace set with the
 	                                  # traces from the old trace set
 ```
 
 ## Documentation
 The full documentation is available in the `docs` folder with a readable version on [Read the Docs](https://trsfile.readthedocs.io/).
 
-## Testing
+## Contributing
+
+### Testing
 The library supports Python `unittest` module and the tests can be executed with the following command:
 ```
 python -m unittest
 ```
 
+### Creating Releases
+We use Github Actions to publish packages to PYPy. Read the [Github docs on how to create a new release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository) and trigger the publishing workflow:
+
 ## License
 [BSD 3-Clause Clear License](https://choosealicense.com/licenses/bsd-3-clause-clear/)
-
-
```

### Comparing `trsfile-2.1.0/README.md` & `trsfile-2.2.0/trsfile.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: trsfile
+Version: 2.2.0
+Summary: Library to read and create Riscure Inspector trace set files (.trs)
+Home-page: https://github.com/riscure/python-trsfile
+Maintainer: Riscure
+Maintainer-email: inforequest@riscure.com
+License: BSD 3-Clause Clear License
+Project-URL: Documentation, https://trsfile.readthedocs.io/en/latest
+Project-URL: Bug Reports, https://github.com/riscure/python-trsfile/issues
+Project-URL: Riscure, https://www.riscure.com
+Keywords: trs,trace,inspector,riscure
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Topic :: Utilities
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: DEV
+License-File: LICENSE
+
 # Inspector Trace Set `.trs` file support in Python
 [![Build Status](https://app.travis-ci.com/Riscure/python-trsfile.svg?branch=master)](https://app.travis-ci.com/Riscure/python-trsfile)
 [![Documentation Status](https://readthedocs.org/projects/trsfile/badge/)](https://trsfile.readthedocs.io/)
 
 Riscure Inspector uses the `.trs` file format to save and read traces from disk. To better assist reading and writing trace set files from third parties, Riscure published this Python library.
 
 ## Quick start
@@ -193,15 +214,20 @@
 	new_traces.extend(traces)         # Extend the new trace set with the
 	                                  # traces from the old trace set
 ```
 
 ## Documentation
 The full documentation is available in the `docs` folder with a readable version on [Read the Docs](https://trsfile.readthedocs.io/).
 
-## Testing
+## Contributing
+
+### Testing
 The library supports Python `unittest` module and the tests can be executed with the following command:
 ```
 python -m unittest
 ```
 
+### Creating Releases
+We use Github Actions to publish packages to PYPy. Read the [Github docs on how to create a new release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository) and trigger the publishing workflow:
+
 ## License
 [BSD 3-Clause Clear License](https://choosealicense.com/licenses/bsd-3-clause-clear/)
```

### Comparing `trsfile-2.1.0/docs/Makefile` & `trsfile-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/docs/api.rst` & `trsfile-2.2.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/docs/conf.py` & `trsfile-2.2.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,29 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
+from datetime import date
+from importlib.metadata import metadata
+
 sys.path.insert(0, os.path.abspath('../'))
 
 import trsfile
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'trsfile'
-copyright = trsfile.__author__ + ', Riscure'
-author = trsfile.__author__
+
+author = metadata(project)["Maintainer"]
+copyright = f"{date.today().year}, {author}"
+
 
 # The short X.Y version
 version = '.'.join(trsfile.__version__.split('.')[0:2])
 # The full version, including alpha/beta/rc tags
 release = trsfile.__version__
 
 
@@ -41,15 +46,15 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.todo',
     'sphinx.ext.coverage',
     'sphinx.ext.viewcode',
-    'm2r',
+    'm2r2',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
@@ -138,15 +143,15 @@
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
     (master_doc, 'trsfile.tex', 'trsfile Documentation',
-     trsfile.__author__, 'manual'),
+     author, 'manual'),
 ]
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
```

### Comparing `trsfile-2.1.0/docs/images/overview.svg` & `trsfile-2.2.0/docs/images/overview.svg`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/docs/images/overview.xml` & `trsfile-2.2.0/docs/images/overview.xml`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/docs/make.bat` & `trsfile-2.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/setup.cfg` & `trsfile-2.2.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -23,24 +23,25 @@
 	Documentation = https://trsfile.readthedocs.io/en/latest
 	Bug Reports = https://github.com/riscure/python-trsfile/issues
 	Riscure = https://www.riscure.com
 
 [options]
 packages = 
 	trsfile
+	riscure
 install_requires = 
 	numpy
 include_package_data = True
 
 [options.extras_require]
 DEV = 
 	sphinx
 	sphinx-autobuild
 	sphinx_rtd_theme
-	m2r
+	m2r2
 
 [options.package_data]
 * = VERSION.txt
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trsfile-2.1.0/tests/data/90x500xfloat.trs` & `trsfile-2.2.0/tests/data/90x500xfloat.trs`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/tests/test_creation.py` & `trsfile-2.2.0/tests/test_creation.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 import tempfile
 import unittest
 import math
 import shutil
 
 from trsfile import Trace, SampleCoding, Header, TracePadding
-from trsfile.parametermap import TraceParameterMap, TraceParameterDefinitionMap, TraceSetParameterMap
+from trsfile.parametermap import TraceParameterMap, TraceParameterDefinitionMap, TraceSetParameterMap, RawTraceData
 from trsfile.standardparameters import StandardTraceSetParameters
 from trsfile.traceparameter import ByteArrayParameter, TraceParameterDefinition, ParameterType, StringParameter, \
     IntegerArrayParameter, BooleanArrayParameter, FloatArrayParameter
 
 
 def get_sample(x):
     return math.sin(0.5 * x) * 1000
@@ -174,14 +174,28 @@
                 expected_trace_set_parameters.add_standard_parameter(StandardTraceSetParameters.SETUP_XYZ_GRID_COUNT_X, 18)
                 expected_trace_set_parameters.add_standard_parameter(StandardTraceSetParameters.SETUP_XYZ_GRID_COUNT_Y, 19)
                 expected_trace_set_parameters.add_standard_parameter(StandardTraceSetParameters.SETUP_XYZ_MEASUREMENTS_PER_SPOT, 20)
                 self.assertDictEqual(trs_traces.get_headers()[Header.TRACE_SET_PARAMETERS], expected_trace_set_parameters)
         except Exception as e:
             self.fail('Exception occurred: ' + str(e))
 
+    def test_write_different_trace_sizes(self):
+        trace_count = 100
+        sample_count = 1000
+
+        with trsfile.open(self.tmp_path, 'w', padding_mode=TracePadding.AUTO) as trs_traces:
+            trs_traces.extend([
+                Trace(
+                    SampleCoding.FLOAT,
+                    [0] * sample_count,
+                    RawTraceData(i.to_bytes(8, byteorder='big'))
+                )
+                for i in range(0, trace_count)]
+            )
+
     def test_write_closed(self):
         trace_count = 100
         sample_count = 1000
 
         with trsfile.open(self.tmp_path, 'w', padding_mode=TracePadding.AUTO) as trs_traces:
             trs_traces.extend([
                 Trace(
@@ -192,14 +206,83 @@
                 for i in range(0, trace_count)]
             )
 
         # Should raise an "ValueError: I/O operation on closed trace set"
         with self.assertRaises(ValueError):
             print(trs_traces)
 
+    def test_write_different_trace_sizes(self):
+        trace_count = 100
+        sample_count = 1000
+
+        with trsfile.open(self.tmp_path, 'w', padding_mode=TracePadding.AUTO) as trs_traces:
+            trs_traces.extend([
+                Trace(
+                    SampleCoding.FLOAT,
+                    [0] * sample_count,
+                    TraceParameterMap({'LEGACY_DATA': ByteArrayParameter(i.to_bytes(8, byteorder='big'))})
+                )
+                for i in range(0, trace_count)]
+            )
+            with self.assertRaises(TypeError):
+                # The length is incorrect
+                # Should raise a Type error: The parameters of trace #0 do not match the trace set's definitions.
+                trs_traces.extend([
+                    Trace(
+                        SampleCoding.FLOAT,
+                        [0] * sample_count,
+                        TraceParameterMap({'LEGACY_DATA': ByteArrayParameter(bytes.fromhex('cafebabedeadbeef0102030405060708'))})
+                    )]
+                )
+            with self.assertRaises(TypeError):
+                # The name is incorrect
+                # Should raise a Type error: The parameters of trace #1 do not match the trace set's definitions.
+                trs_traces.extend([
+                    Trace(
+                        SampleCoding.FLOAT,
+                        [0] * sample_count,
+                        TraceParameterMap({'LEGACY_DATA': ByteArrayParameter(bytes.fromhex('0102030405060708'))})
+                    ),
+                    Trace(
+                        SampleCoding.FLOAT,
+                        [0] * sample_count,
+                        TraceParameterMap({'NEW_DATA': ByteArrayParameter(bytes.fromhex('0102030405060708'))})
+                    )]
+                )
+            with self.assertRaises(TypeError):
+                # The type is incorrect
+                # Should raise a Type error: The parameters of trace #0 do not match the trace set's definitions.
+                trs_traces.extend([
+                    Trace(
+                        SampleCoding.FLOAT,
+                        [0] * sample_count,
+                        TraceParameterMap({'LEGACY_DATA': IntegerArrayParameter([42, 74])})
+                    )]
+                )
+
+        with trsfile.open(self.tmp_path, 'w', padding_mode=TracePadding.AUTO) as trs_traces:
+            trs_traces.extend([
+                Trace(
+                    SampleCoding.FLOAT,
+                    [0] * sample_count,
+                    TraceParameterMap()
+                )
+                for i in range(0, trace_count)]
+            )
+            with self.assertRaises(TypeError):
+                # The length, data and name are incorrect
+                # Should raise a Type error: The parameters of trace #0 do not match the trace set's definitions.
+                trs_traces.extend([
+                    Trace(
+                        SampleCoding.FLOAT,
+                        [0] * sample_count,
+                        TraceParameterMap({'LEGACY_DATA': ByteArrayParameter(bytes.fromhex('cafebabedeadbeef0102030405060708'))})
+                    )]
+                )
+
     def test_read(self):
         trace_count = 100
         sample_count = 1000
 
         original_traces = [
                 Trace(
                     SampleCoding.FLOAT,
@@ -266,15 +349,15 @@
                 self.assertEqual(len(trs_traces), expected_length)
 
                 # Extend the trace file with 100 traces with each 1000 samples
                 trs_traces.extend([
                     Trace(
                         SampleCoding.FLOAT,
                         [0] * sample_count,
-                        TraceParameterMap({'LEGACY_DATA': ByteArrayParameter(i.to_bytes(8, byteorder='big'))})
+                        raw_data=i.to_bytes(8, byteorder='big')
                     )
                     for i in range(0, trace_count)]
                 )
 
                 expected_length += trace_count
                 self.assertEqual(len(trs_traces), expected_length)
```

### Comparing `trsfile-2.1.0/tests/test_generic.py` & `trsfile-2.2.0/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/tests/test_header.py` & `trsfile-2.2.0/tests/test_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,18 @@
             del trace_parameter_definitions["INPUT"]
         with self.assertRaises(TypeError):
             trace_parameter_definitions.pop("INPUT")
         with self.assertRaises(TypeError):
             trace_parameter_definitions.popitem()
         with self.assertRaises(TypeError):
             trace_parameter_definitions.clear()
+        with self.assertRaises(TypeError):
+            trace_parameter_definitions.append('input', ParameterType.BYTE, 16)
+        with self.assertRaises(TypeError):
+            trace_parameter_definitions.insert('output', ParameterType.BYTE, 16, 0)
 
         # Shallow copies still share references to the same trace set parameters as the original,
         # and should therefore not be modifiable if the original isn't
         with self.assertRaises(TypeError):
             shallow_copy = trace_parameter_definitions.copy()
             shallow_copy["OUTPUT"] = TraceParameterDefinition(ParameterType.BYTE, 16, 16)
         with self.assertRaises(TypeError):
```

### Comparing `trsfile-2.1.0/tests/test_parametermap.py` & `trsfile-2.2.0/tests/test_parametermap.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 
-from trsfile.parametermap import TraceSetParameterMap, TraceParameterDefinitionMap, TraceParameterMap
+from trsfile.parametermap import TraceSetParameterMap, TraceParameterDefinitionMap, TraceParameterMap, RawTraceData
 from trsfile.standardparameters import StandardTraceSetParameters, StandardTraceParameters
 from trsfile.traceparameter import *
 
 
 class TestTraceSetParameterMap(TestCase):
     SERIALIZED_MAP = b'\x09\x00' \
                      b'\x06\x00param1\x31\x05\x00\x01\x00\x00\x01\x01' \
@@ -72,17 +72,23 @@
         with self.assertRaises(TypeError):
             param_map.add_parameter('param10', [])
 
     def test_add_standard_parameter(self):
         param_map1 = TraceSetParameterMap()
         param_map1.add_standard_parameter(StandardTraceSetParameters.KEY,
                                           bytes.fromhex('cafebabedeadbeef0102030405060708'))
+        param_map1.add_standard_parameter(StandardTraceSetParameters.TVLA_CIPHER, "AES")
         param_map2 = TraceSetParameterMap()
         param_map2.add_parameter('KEY', bytes.fromhex('cafebabedeadbeef0102030405060708'))
+        param_map2.add_parameter('TVLA:CIPHER', "AES")
+        param_map3 = TraceSetParameterMap()
+        param_map3.add('key', bytes.fromhex('cafebabedeadbeef0102030405060708'))
+        param_map3.add('tvla_cipher', "AES")
         self.assertDictEqual(param_map1, param_map2)
+        self.assertDictEqual(param_map1, param_map3)
 
         # Verify that standard trace set parameters enforce a specific type
         with self.assertRaises(TypeError):
             param_map1.add_standard_parameter(StandardTraceSetParameters.KEY, 'cafebabedeadbeef0102030405060708')
         # Type checking even occurs when adding a parameter with the id of a standard trace set parameter
         # However, this type check only produces a warning
         with self.assertWarns(UserWarning):
@@ -100,14 +106,22 @@
         param_map = TraceParameterDefinitionMap()
         param_map['IN'] = TraceParameterDefinition(ParameterType.BYTE, 16, 0)
         param_map['TITLE'] = TraceParameterDefinition(ParameterType.STRING, 13, 16)
         param_map['中文'] = TraceParameterDefinition(ParameterType.STRING, 15, 29)
         return param_map
 
     @staticmethod
+    def create_std_parameterdefinitionmap() -> TraceParameterDefinitionMap:
+        param_map = TraceParameterDefinitionMap()
+        param_map['INPUT'] = TraceParameterDefinition(ParameterType.BYTE, 16, 0)
+        param_map['OUTPUT'] = TraceParameterDefinition(ParameterType.BYTE, 16, 16)
+        param_map['KEY'] = TraceParameterDefinition(ParameterType.BYTE, 16, 32)
+        return param_map
+
+    @staticmethod
     def create_traceparametermap() -> TraceParameterMap:
         param_map = TraceParameterMap()
         param_map['IN'] = ByteArrayParameter(bytes.fromhex('cafebabedeadbeef0102030405060708'))
         param_map['TITLE'] = StringParameter('Hello, world!')
         param_map['中文'] = StringParameter('你好，世界')
         return param_map
 
@@ -124,14 +138,42 @@
                          self.SERIALIZED_DEFINITION)
 
     def test_from_trace_params(self):
         param_map = TestTraceParameterDefinitionMap.create_traceparametermap()
         map_from_trace_params = TraceParameterDefinitionMap.from_trace_parameter_map(param_map)
         self.assertDictEqual(self.create_parameterdefinitionmap(), map_from_trace_params)
 
+    def test_append(self):
+        map_from_append = TraceParameterDefinitionMap()
+        map_from_append.append('IN', ParameterType.BYTE, 16)
+        map_from_append.append('TITLE', ParameterType.STRING, 13)
+        map_from_append.append('中文', ParameterType.STRING, 15)
+        self.assertDictEqual(self.create_parameterdefinitionmap(), map_from_append)
+
+        map_from_std_append = TraceParameterDefinitionMap()
+        map_from_std_append.append_std('INPUT', 16)
+        map_from_std_append.append_std('OUTPUT', 16)
+        map_from_std_append.append_std('KEY', 16)
+        self.assertDictEqual(self.create_std_parameterdefinitionmap(), map_from_std_append)
+
+    def test_insert(self):
+        map_from_insert = TraceParameterDefinitionMap()
+        map_from_insert.insert('TITLE', ParameterType.STRING, 13, 0)
+        with self.assertWarns(UserWarning):
+            map_from_insert.insert('中文', ParameterType.STRING, 15, 10)
+        map_from_insert.insert('IN', ParameterType.BYTE, 16, 0)
+        self.assertDictEqual(self.create_parameterdefinitionmap(), map_from_insert)
+
+        map_from_std_insert = TraceParameterDefinitionMap()
+        map_from_std_insert.insert_std('INPUT', 16, 0)
+        with self.assertWarns(UserWarning):
+            map_from_std_insert.insert_std('KEY', 16, 9)
+        map_from_std_insert.insert_std('OUTPUT', 16, 16)
+        self.assertDictEqual(self.create_std_parameterdefinitionmap(), map_from_std_insert)
+
 
 class TestTraceParameterMap(TestCase):
     CAFEBABE = bytes.fromhex('cafebabedeadbeef0102030405060708')
     SERIALIZED_MAP = CAFEBABE + \
                      b'Hello, world!' \
                      b'\xe4\xbd\xa0\xe5\xa5\xbd\xef\xbc\x8c\xe4\xb8\x96\xe7\x95\x8c'
 
@@ -195,18 +237,50 @@
         param_defs['HAS_KEY'] = TraceParameterDefinition(ParameterType.BOOL, 1, 44)
         self.assertFalse(param_map.matches(param_defs))
 
     def test_add_standard_parameter(self):
         param_map1 = TraceParameterMap()
         param_map1.add_standard_parameter(StandardTraceParameters.INPUT,
                                           bytes.fromhex('cafebabedeadbeef0102030405060708'))
+        param_map1.add_standard_parameter(StandardTraceParameters.TVLA_SET_INDEX, 1)
         param_map2 = TraceParameterMap()
         param_map2.add_parameter('INPUT', bytes.fromhex('cafebabedeadbeef0102030405060708'))
+        param_map2.add_parameter('TVLA:SET_INDEX', 1)
+        param_map3 = TraceParameterMap()
+        param_map3.add("input", bytes.fromhex('cafebabedeadbeef0102030405060708'))
+        param_map3.add("tvla_set_index", 1)
         self.assertDictEqual(param_map1, param_map2)
+        self.assertDictEqual(param_map1, param_map3)
 
         # Verify that standard trace parameters enforce a specific type
         with self.assertRaises(TypeError):
             param_map1.add_standard_parameter(StandardTraceParameters.INPUT, 'cafebabedeadbeef0102030405060708')
         # Type checking even occurs when adding a parameter with the id of a standard trace parameter
         # However, this type check only produces a warning
         with self.assertWarns(UserWarning):
             param_map1.add_parameter('INPUT', 'cafebabedeadbeef0102030405060708')
+
+    def test_raw_trace_data(self):
+        raw_data = RawTraceData(bytes.fromhex('cafebabedeadbeef0102030405060708'))
+        assert raw_data.serialize() == bytes.fromhex('cafebabedeadbeef0102030405060708')
+
+        # Verify that nothing can be added into a raw data TraceParameterMap
+        with self.assertRaises(KeyError):
+            raw_data['INPUT'] = ByteArrayParameter(bytes.fromhex('cafebabedeadbeef0102030405060708'))
+        with self.assertRaises(KeyError):
+            raw_data.add('input', bytes.fromhex('cafebabedeadbeef0102030405060708'))
+
+        # Verify that raw data can match any traceparameterdefinition map, as long as the length is correct
+        traceParamDefs = TraceParameterDefinitionMap()
+        traceParamDefs.append("INPUT", ParameterType.BYTE, 16)
+        assert raw_data.matches(traceParamDefs)
+
+        traceParamDefs = TraceParameterDefinitionMap()
+        traceParamDefs.append("INPUT", ParameterType.BYTE, 8)
+        traceParamDefs.append("OUTPUT", ParameterType.BYTE, 8)
+        assert raw_data.matches(traceParamDefs)
+        traceParamDefs.append("KEY", ParameterType.BYTE, 8)
+        assert not raw_data.matches(traceParamDefs)
+
+        with self.assertWarns(UserWarning):
+            TraceParameterDefinitionMap.from_trace_parameter_map(raw_data)
+
```

### Comparing `trsfile-2.1.0/tests/test_trace.py` & `trsfile-2.2.0/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/tests/test_trsfile.py` & `trsfile-2.2.0/tests/test_trsfile.py`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/trsfile/__init__.py` & `trsfile-2.2.0/trsfile/__init__.py`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/trsfile/common.py` & `trsfile-2.2.0/trsfile/common.py`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/trsfile/engine/engine.py` & `trsfile-2.2.0/trsfile/engine/engine.py`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/trsfile/engine/file.py` & `trsfile-2.2.0/trsfile/engine/file.py`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/trsfile/engine/trs.py` & `trsfile-2.2.0/trsfile/engine/trs.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,25 +169,26 @@
             # Check padding mode on how we are going to do this
             headers_updates[Header.NUMBER_SAMPLES] = max(lengths)
 
         if self.headers[Header.LENGTH_DATA] is None:
             if len(set([len(trace.parameters.serialize()) for trace in traces])) > 1:
                 raise TypeError('Traces have different data length, this is not supported in TRS files')
 
-            data_length = len(traces[0].parameters.serialize())
+            headers_updates[Header.LENGTH_DATA] = len(traces[0].parameters.serialize())
 
-            # Add a TraceParameterDefinitionMap if none is present, and verify its validity if one is present
-            if Header.TRACE_PARAMETER_DEFINITIONS not in self.headers:
-                if data_length > 0:
-                    headers_updates[Header.TRACE_PARAMETER_DEFINITIONS] = \
-                        TraceParameterDefinitionMap.from_trace_parameter_map(traces[0].parameters)
-            elif not traces[0].parameters.matches(self.headers[Header.TRACE_PARAMETER_DEFINITIONS]):
-                raise TypeError("The traces' parameters do not match the trace set's definitions")
-
-            headers_updates[Header.LENGTH_DATA] = data_length
+        # Add a TraceParameterDefinitionMap if none is present, and verify its validity if one is present
+        if Header.TRACE_PARAMETER_DEFINITIONS not in self.headers:
+            headers_updates[Header.TRACE_PARAMETER_DEFINITIONS] = \
+                TraceParameterDefinitionMap.from_trace_parameter_map(traces[0].parameters)
+        else:
+            for index, trace in enumerate(traces):
+                if not trace.parameters.matches(self.headers[Header.TRACE_PARAMETER_DEFINITIONS]):
+                    raise TypeError(f"The parameters of trace #{index} do not match the trace set's definitions.\n"
+                                    f"Please make sure the trace parameters match those of the other traces in type, "
+                                    f"size and name.")
 
         if self.headers[Header.SAMPLE_CODING] is None:
             if len(set([trace.sample_coding for trace in traces])) > 1:
                 raise TypeError('Traces have different sample coding, this is not supported in TRS files')
             headers_updates[Header.SAMPLE_CODING] = traces[0].sample_coding
 
         if self.headers[Header.TITLE_SPACE] is None:
```

### Comparing `trsfile-2.1.0/trsfile/parametermap.py` & `trsfile-2.2.0/trsfile/parametermap.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 import copy
 import numbers
 import warnings
 from typing import Any, Union, List, Dict
 
+from trsfile.compatibility import alias, aliased
 from trsfile.standardparameters import StandardTraceSetParameters, StandardTraceParameters
 from trsfile.traceparameter import TraceSetParameter, TraceParameter, TraceParameterDefinition, ParameterType, \
     BooleanArrayParameter, ByteArrayParameter, StringParameter, DoubleArrayParameter, IntegerArrayParameter, \
     LongArrayParameter, ShortArrayParameter
 from trsfile.utils import *
 
 UTF_8 = 'utf-8'
 SHORT_MIN = -2**15
 SHORT_MAX = 2**15-1
 INT_MIN = -2**31
 INT_MAX = 2**31-1
 
+
 class ParameterMapUtil:
     # A placeholder for integers that are actually shorts
     class ShortType(numbers.Rational):
         pass
 
     # A placeholder for integers that are actually longs
     class LongType(numbers.Rational):
@@ -171,14 +173,15 @@
         self._stop_if_locked()
         super().move_to_end(key, last)
 
     def lock_content(self):
         self._is_locked = True
 
 
+@aliased
 class TraceSetParameterMap(LockableDict):
     default_values = {
         StandardTraceSetParameters.DISPLAY_HINT_X_LABEL: "",
         StandardTraceSetParameters.DISPLAY_HINT_Y_LABEL: "",
         StandardTraceSetParameters.DISPLAY_HINT_NUM_TRACES_SHOWN: 1,
         StandardTraceSetParameters.DISPLAY_HINT_TRACES_OVERLAP: False,
         StandardTraceSetParameters.DISPLAY_HINT_USE_LOG_SCALE: False,
@@ -191,61 +194,69 @@
     def __setitem__(self, key: str, value: Union[TraceParameter, TraceSetParameter]):
         if not isinstance(value, TraceParameter) or type(value) is TraceSetParameter:
             raise TypeError('The value for a TraceSetParameterMap entry must be a specific subclass'
                             ' of TraceParameter (e.g. ByteArrayParameter).')
         self._stop_if_locked()
         super().__setitem__(key, value)
 
-    def add_parameter(self, name: str, value: ParameterMapUtil.ParameterValueType) -> None:
+    @alias("add")
+    def add_parameter(self, name: str, value: ParameterMapUtil.ParameterValueType) -> TraceSetParameterMap:
         """Add a trace set parameter with a given name and value.
         If the name matches the identifier of a standard trace set parameter,
         then the value's type should be the type that standard trace set parameter expects.
         If the parameter already exists within the map, it will be overwritten.
 
         :param name:  The name of the parameter that will be added
         :param value: The value of the parameter. If the name matches that of a standard trace set parameter, it is
                       recommended that the type of the value matches that of standard trace set parameter. Otherwise,
-                      valid types are: int, float, bool, List[int], List[float], List[bool], bytes, bytearray or str"""
+                      valid types are: int, float, bool, List[int], List[float], List[bool], bytes, bytearray or str
+        :return:      This TraceSetParameterMap after adding the new parameter"""
         try:
             std_param = StandardTraceSetParameters.from_identifier(name)
             typed_param = std_param.parameter_type.param_class
-            self[name] = typed_param(ParameterMapUtil.to_list_if_listable(value))
+            self[std_param.identifier] = typed_param(ParameterMapUtil.to_list_if_listable(value))
+            return self
         # if no std_param can be found, a ValueError is raised,
         # if adding the trace parameter to the map fails, a TypeError is raised
         except (ValueError, TypeError) as e:
             if isinstance(e, TypeError):
                 warnings.warn("Adding a trace set parameter with a name that matches a standard set trace parameter, "
                               "but with a type that doesn't match that standard trace set parameter.\nThis may lead to "
                               "unexpected behavior when displaying this traceset or processing it in Inspector")
             typed_param = ParameterMapUtil.get_typed_parameter(value)
             self[name] = typed_param(ParameterMapUtil.to_list_if_listable(value))
 
-    def add_standard_parameter(self, std_trace_set_param: StandardTraceSetParameters, value: ParameterMapUtil.ParameterValueType) -> None:
+    def add_standard_parameter(self, std_trace_set_param: StandardTraceSetParameters,
+                               value: ParameterMapUtil.ParameterValueType) -> TraceSetParameterMap:
         """Add a standard trace set parameter with a given value.
         If the parameter already exists within the map, it will be overwritten.
 
         :param std_trace_set_param: The standard trace set parameter that will be added
         :param value:               The value of the parameter. The type this value must have depends on
-                                    the standard trace set parameter."""
+                                    the standard trace set parameter.
+        :return:                    This TraceSetParameterMap after adding the new standard parameter"""
         typed_param = std_trace_set_param.parameter_type.param_class
         self[std_trace_set_param.identifier] = typed_param(ParameterMapUtil.to_list_if_listable(value))
+        return self
 
-    def fill_from_headers(self, headers: Dict['Header', Any]) -> None:
+    def fill_from_headers(self, headers: Dict['Header', Any]) -> TraceSetParameterMap:
         """Add to this trace set parameter map all data that is in the header
         and for which standard trace set parameters exist.
         Data that already exists in the map will not be overwritten.
 
-        :param headers: The headers dictionary from which data will be copied into the trace set parameter map"""
+        :param headers: The headers dictionary from which data will be copied into the trace set parameter map
+        :return:        This TraceSetParameterMap after adding the parameters based on the headers"""
         for header_tag, value in headers.items():
             std_param = header_tag.equivalent_std_param
             if std_param is not None and std_param.identifier not in self:
                 self.add_standard_parameter(std_param, value)
 
-    def add_defaults(self) -> None:
-        """If specific standard trace set parameters don't exist yet in the map, add them with default values"""
+    def add_defaults(self) -> TraceSetParameterMap:
+        """If specific standard trace set parameters don't exist yet in the map, add them with default values
+         :return: This TraceSetParameterMap after adding the default parameters"""
         for key, value in TraceSetParameterMap.default_values.items():
             if key.identifier not in self:
                 self.add_standard_parameter(key, value)
 
     @staticmethod
     def deserialize(raw: BytesIO) -> TraceSetParameterMap:
         result = TraceSetParameterMap()
@@ -285,14 +296,90 @@
     def __setitem__(self, key: str, value: TraceParameterDefinition):
         if type(value) is not TraceParameterDefinition:
             raise TypeError('The value for an entry in a TraceParameterDefinitionMap must be of '
                             'type TraceParameterDefinition')
         self._stop_if_locked()
         super().__setitem__(key, value)
 
+    def insert_std(self, name: str, size: int, offset: int) -> TraceParameterDefinitionMap:
+        """Insert a trace parameter definition of a StandardTraceParameter into this map in a specified location. If
+        the given offset would put the new TraceParameter in the middle of a parameter already present in the map, the
+        offset is increased to put the new parameter after that existing one instead. Any parameters already present
+        in the map that have a greater or equal offset than the new parameter, have their offset increased to make space
+        for the new parameter.
+
+        :param name:   The name of the TraceParameter for which to add a definition. This name must match that of a
+                       StandardTraceParameter
+        :param size:   The size of the TraceParameter, in number of elements
+        :param offset: The offset of the TraceParameter, in bytes
+        :return:       This TraceParameterDefinition map after adding the new definition
+        """
+        try:
+            type = StandardTraceParameters.from_identifier(name).parameter_type
+            return self.insert(name, type, size, offset)
+        except ValueError:
+            raise ValueError(f"No StandardTraceParameter found with name '{name}'. Either use the 'insert' method or "
+                             f"correct the name to match a standard trace parameter.")
+
+    def insert(self, name: str, type: ParameterType, size: int, offset: int) -> TraceParameterDefinitionMap:
+        """Insert a trace parameter definition into this map in a specified location. If the given offset would put the
+        new TraceParameter in the middle of a parameter already present in the map, the offset is increased to put the
+        new parameter after that existing one instead. Any parameters already present in the map that have a greater
+        or equal offset than the new parameter, have their offset increased to make space for the new parameter.
+
+        :param name:   The name of the TraceParameter for which to add a definition
+        :param type:   The type of the TraceParameter for which to add a definition
+        :param size:   The size of the TraceParameter, in number of elements
+        :param offset: The offset of the TraceParameter, in bytes
+        :return:       This TraceParameterDefinition map after adding the new definition
+        """
+        self._stop_if_locked()
+        params_to_move_back = []
+        for key, param in self.items():
+            if param.offset >= offset:
+                param.offset += size * type.byte_size
+                params_to_move_back.append(key)
+            elif param.offset + param.length * param.param_type.byte_size > offset:
+                offset = param.offset + param.length * param.param_type.byte_size
+                warnings.warn("Given offset would put a parameter inside another trace parameter.\n"
+                              f"Increased the offset of the inserted parameter definition to {offset} to prevent this.")
+
+        new_definition = TraceParameterDefinition(type, size, offset)
+        self.__setitem__(name, new_definition)
+        for param in params_to_move_back:
+            self.move_to_end(param)
+        return self
+
+    def append_std(self, name: str, size: int) -> TraceParameterDefinitionMap:
+        """Append a trace parameter definition of a StandardTraceParameter to this map. The parameter wil be added after
+       all parameter definitions already in the map.
+
+       :param name: The name of the TraceParameter for which to add a definition. This name must match that of a
+                    StandardTraceParameter
+       :param size: The size of the TraceParameter, in number of elements
+       :return:     This TraceParameterDefinition map after adding the new definition"""
+        try:
+            type = StandardTraceParameters.from_identifier(name).parameter_type
+            return self.append(name, type, size)
+        except ValueError:
+            raise ValueError(f"No StandardTraceParameter found with name '{name}'. Either use the 'append' method or "
+                             f"correct the name to match a standard trace parameter.")
+
+    def append(self, name: str, type: ParameterType, size: int) -> TraceParameterDefinitionMap:
+        """Append a trace parameter definition to this map. The parameter wil be added after all parameter definitions
+        already in the map.
+
+        :param name: The name of the TraceParameter for which to add a definition
+        :param type: The type of the TraceParameter for which to add a definition
+        :param size: The size of the TraceParameter, in number of elements
+        :return:     This TraceParameterDefinition map after adding the new definition"""
+        new_definition = TraceParameterDefinition(type, size, self.get_total_size())
+        self.__setitem__(name, new_definition)
+        return self
+
     @staticmethod
     def deserialize(raw: BytesIO) -> TraceParameterDefinitionMap:
         result = TraceParameterDefinitionMap()
         number_of_entries = read_short(raw)
         for _ in range(number_of_entries):
             name = read_parameter_name(raw)
             value = TraceParameterDefinition.deserialize(raw)
@@ -312,64 +399,77 @@
     @staticmethod
     def from_trace_parameter_map(trace_parameters: TraceParameterMap) -> TraceParameterDefinitionMap:
         """Create a trace parameters definition map from a trace parameter map.
 
         :param trace_parameters: The trace parameter map from which the definitions will be deduced
 
         :return:                 A parameter definition map that described the metadata of the input trace parameter map"""
+        if isinstance(trace_parameters, RawTraceData):
+            warnings.warn("Creating a trace parameter definition map from raw trace data.\nThis is not recommended, "
+                          "as it will not add any meta information about the trace data.\nEither manually define a "
+                          "TraceParameterDefinitionMap for the traceset or make sure the first trace you add to the "
+                          "traceset has a proper TraceParameterMap")
+
         offset = 0
         result = TraceParameterDefinitionMap()
         for key, trace_param in trace_parameters.items():
             size = len(trace_param)
             param_type = ParameterType.from_class(type(trace_param))
             result[key] = TraceParameterDefinition(param_type, size, offset)
             offset += size * param_type.byte_size
         return result
 
 
+@aliased
 class TraceParameterMap(StringKeyOrderedDict):
     def __setitem__(self, key: str, value: TraceParameter):
         if not isinstance(value, TraceParameter):
             raise TypeError('The value for a TraceParameterMap entry must be a specific subclass'
                             ' of TraceParameter (e.g. ByteArrayParameter).')
         super().__setitem__(key, value)
 
-    def add_parameter(self, name: str, value: ParameterMapUtil.ParameterValueType) -> None:
+    @alias("add")
+    def add_parameter(self, name: str, value: ParameterMapUtil.ParameterValueType) -> TraceParameterMap:
         """Add a trace parameter with a given name and value
         If the name matches the identifier of a standard trace parameter,
         then the value's type should be the type that standard trace parameter expects.
         If the parameter already exists within the map, it will be overwritten.
 
         :param name:  The name of the parameter that will be added
         :param value: The value of the parameter. If the name matches that of a standard trace parameter, it is
                       recommended that the type of the value matches that of standard trace set parameter. Otherwise,
-                      valid types are: int, float, bool, List[int], List[float], List[bool], bytes, bytearray or str"""
+                      valid types are: int, float, bool, List[int], List[float], List[bool], bytes, bytearray or str
+        :return:      This map after adding the parameter"""
         try:
             std_param = StandardTraceParameters.from_identifier(name)
             typed_param = std_param.parameter_type.param_class
-            self[name] = typed_param(ParameterMapUtil.to_list_if_listable(value))
+            self[std_param.identifier] = typed_param(ParameterMapUtil.to_list_if_listable(value))
         # if no std_param can be found, a ValueError is raised,
         # if adding the trace parameter to the map fails, a TypeError is raised
         except (TypeError, ValueError) as e:
             if isinstance(e, TypeError):
                 warnings.warn("Adding a trace parameter with a name that matches a standard trace parameter, but with "
                               "a type that doesn't match that standard trace parameter.\nThis may lead to unexpected "
                               "behavior when displaying this traceset or processing this trace in Inspector")
             typed_param = ParameterMapUtil.get_typed_parameter(value)
             self[name] = typed_param(ParameterMapUtil.to_list_if_listable(value))
+        return self
 
-    def add_standard_parameter(self, std_trace_param: StandardTraceParameters, value: ParameterMapUtil.ParameterValueType) -> None:
+    def add_standard_parameter(self, std_trace_param: StandardTraceParameters,
+                               value: ParameterMapUtil.ParameterValueType) -> TraceParameterMap:
         """Add a standard trace parameter with a given value.
         If the parameter already exists within the map, it will be overwritten.
 
         :param std_trace_param: The standard trace parameter that will be added
         :param value:           The value of the parameter. The type this value must have depends on
-                                the standard trace parameter."""
+                                the standard trace parameter.
+        :return:                This map after adding the parameter"""
         typed_param = std_trace_param.parameter_type.param_class
         self[std_trace_param.identifier] = typed_param(ParameterMapUtil.to_list_if_listable(value))
+        return self
 
     @staticmethod
     def deserialize(raw: bytes, definitions: TraceParameterDefinitionMap) -> TraceParameterMap:
         io_bytes = BytesIO(raw)
         result = TraceParameterMap()
         for key, val in definitions.items():
             io_bytes.seek(val.offset)
@@ -405,7 +505,24 @@
                 match &= ParameterType.from_class(type(value)) == definition.param_type
                 match &= definition.offset == offset
                 offset += len(value)
             if not match:
                 break
         match &= matched_keys == list(definitions.keys())
         return match
+
+
+class RawTraceData(TraceParameterMap):
+    def __init__(self, data: bytes):
+        super().__init__()
+        super().__setitem__("LEGACY_DATA", ByteArrayParameter(data))
+
+    def __setitem__(self, key: str, value: TraceParameter):
+        raise KeyError("Adding Trace Parameters into raw trace data is not allowed")
+
+    def matches(self, definitions: TraceParameterDefinitionMap) -> bool:
+        """Test whether this RawTraceData could be interpreted by given definitions
+
+        :param definitions: The trace parameter definition map to check this raw trace data against
+
+        :return:            A boolean that is true if the trace parameter definitions can interpret this raw trace data"""
+        return definitions.get_total_size() == len(self["LEGACY_DATA"])
```

### Comparing `trsfile-2.1.0/trsfile/standardparameters.py` & `trsfile-2.2.0/trsfile/standardparameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         obj.identifier = identifier
         obj.parameter_type = parameter_type
         return obj
 
     @staticmethod
     def from_identifier(identifier: str) -> StandardTraceSetParameters:
         for val in StandardTraceSetParameters:
-            if identifier == val.identifier:
+            if identifier.lower() == val.identifier.lower() or identifier.lower() == val.name.lower():
                 return val
         raise ValueError(f'{identifier} is not an identifier of a StandardTraceSetParameter')
 
     KEY = (0x01, 'KEY', ParameterType.BYTE)
     X_OFFSET = (0x02, 'X_OFFSET', ParameterType.INT)
     X_SCALE = (0x03, 'X_SCALE', ParameterType.FLOAT)
     Y_SCALE = (0x04, 'Y_SCALE', ParameterType.FLOAT)
@@ -75,15 +75,15 @@
         obj.identifier = identifier
         obj.parameter_type = parameter_type
         return obj
 
     @staticmethod
     def from_identifier(identifier: str) -> StandardTraceParameters:
         for val in StandardTraceParameters:
-            if identifier == val.identifier:
+            if identifier.lower() == val.identifier.lower() or identifier.lower() == val.name.lower():
                 return val
         raise ValueError('{} is not a name of a StandardTraceParameter'.format(identifier))
 
     INPUT = (0x01, 'INPUT', ParameterType.BYTE)
     OUTPUT = (0x02, 'OUTPUT', ParameterType.BYTE)
     KEY = (0x03, 'KEY', ParameterType.BYTE)
```

### Comparing `trsfile-2.1.0/trsfile/trace.py` & `trsfile-2.2.0/trsfile/trace.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,51 @@
 import numpy
 
-from trsfile.parametermap import TraceParameterMap
+from trsfile.parametermap import TraceParameterMap, RawTraceData
 from trsfile.common import Header, SampleCoding
 
+
 class Trace:
 	"""The :py:obj:`Trace` class behaves like a :py:obj:`list`
 	object were each item in the list is a sample of the trace.
 
 	When a :py:obj:`Trace` is initialized the samples are (optionally) converted to a
 	:py:class:`numpy.array` depending on the current type of the samples and the
 	provided :py:obj:`sample_coding`.
 	"""
 
-	def __init__(self, sample_coding, samples, parameters=TraceParameterMap(), title='trace', headers={}):
+	def __init__(self, sample_coding, samples, parameters=None, title='trace', headers=None, raw_data: bytes = bytes()):
+		""" Create a new Trace.
+		:param sample_coding: The encoding of all samples in the trace
+		:param samples: The array of samples of the trace
+		:param parameters: The trace parameter map that contains the trace's data and its meta information. Do not use
+			in combination with raw_data
+		:param title: The title of the trace
+		:param headers: The headers of the trs file to which this trace will be added. This is an optional parameter;
+			information from the headers may define the locations of the input, output and key data in the trace data,
+			but it is recommended to store that information in the trace parameter map now.
+		:param raw_data: A byte array with the raw trace data. Do not use in combination with parameters. If used, it is
+			recommended that a TraceParameterDefinitionMap is added to the headers of the trsfile that defines the meta
+			information of this raw trace data.
+		"""
+		if parameters is None:
+			if len(raw_data) > 0:
+				parameters = RawTraceData(raw_data)
+			else:
+				parameters = TraceParameterMap()
+		else:
+			if len(raw_data) > 0:
+				raise Warning("Parameter map and raw data were both defined, but cannot both be used at the same time.\n"
+							  "Only the parameter map will be used, raw data will be discarded.")
+		if headers is None:
+			headers = {}
 		self.title = title
 		self.parameters = parameters
-		if not type(self.parameters) is TraceParameterMap:
-			raise TypeError('Trace parameter data must be supplied as a TraceParameterMap')
+		if not isinstance(self.parameters, TraceParameterMap):
+			raise TypeError('Trace data must be supplied as a TraceParameterMap')
 
 		# Obtain sample coding
 		if not isinstance(sample_coding, SampleCoding):
 			raise TypeError('Trace requires sample_coding to be of type \'SampleCoding\'')
 		self.sample_coding = sample_coding
 
 		# Read in the sample and cast them automatically to the correct type
```

### Comparing `trsfile-2.1.0/trsfile/utils.py` & `trsfile-2.2.0/trsfile/utils.py`

 * *Files identical despite different names*

### Comparing `trsfile-2.1.0/trsfile.egg-info/PKG-INFO` & `trsfile-2.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: trsfile
-Version: 2.1.0
-Summary: Library to read and create Riscure Inspector trace set files (.trs)
-Home-page: https://github.com/riscure/python-trsfile
-Maintainer: Riscure
-Maintainer-email: inforequest@riscure.com
-License: BSD 3-Clause Clear License
-Project-URL: Documentation, https://trsfile.readthedocs.io/en/latest
-Project-URL: Bug Reports, https://github.com/riscure/python-trsfile/issues
-Project-URL: Riscure, https://www.riscure.com
-Keywords: trs,trace,inspector,riscure
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Topic :: Utilities
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: DEV
-License-File: LICENSE
-
 # Inspector Trace Set `.trs` file support in Python
 [![Build Status](https://app.travis-ci.com/Riscure/python-trsfile.svg?branch=master)](https://app.travis-ci.com/Riscure/python-trsfile)
 [![Documentation Status](https://readthedocs.org/projects/trsfile/badge/)](https://trsfile.readthedocs.io/)
 
 Riscure Inspector uses the `.trs` file format to save and read traces from disk. To better assist reading and writing trace set files from third parties, Riscure published this Python library.
 
 ## Quick start
@@ -215,17 +193,20 @@
 	new_traces.extend(traces)         # Extend the new trace set with the
 	                                  # traces from the old trace set
 ```
 
 ## Documentation
 The full documentation is available in the `docs` folder with a readable version on [Read the Docs](https://trsfile.readthedocs.io/).
 
-## Testing
+## Contributing
+
+### Testing
 The library supports Python `unittest` module and the tests can be executed with the following command:
 ```
 python -m unittest
 ```
 
+### Creating Releases
+We use Github Actions to publish packages to PYPy. Read the [Github docs on how to create a new release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository) and trigger the publishing workflow:
+
 ## License
 [BSD 3-Clause Clear License](https://choosealicense.com/licenses/bsd-3-clause-clear/)
-
-
```

