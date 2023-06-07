# Comparing `tmp/datashuttle-0.0.1.tar.gz` & `tmp/datashuttle-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datashuttle-0.0.1.tar", last modified: Tue Oct 18 16:04:07 2022, max compression
+gzip compressed data, was "datashuttle-0.1.0rc1.tar", last modified: Wed Jun  7 15:19:58 2023, max compression
```

## Comparing `datashuttle-0.0.1.tar` & `datashuttle-0.1.0rc1.tar`

### file list

```diff
@@ -1,15 +1,85 @@
-drwxrwxrwx   0        0        0        0 2022-10-18 16:04:07.564334 datashuttle-0.0.1/
--rw-rw-rw-   0        0        0     1508 2022-10-18 16:02:32.000000 datashuttle-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      101 2022-10-18 16:02:32.000000 datashuttle-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      824 2022-10-18 16:04:07.564334 datashuttle-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       15 2022-10-18 16:02:32.000000 datashuttle-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-10-18 16:04:07.540334 datashuttle-0.0.1/datashuttle/
-drwxrwxrwx   0        0        0        0 2022-10-18 16:04:07.563333 datashuttle-0.0.1/datashuttle/datashuttle.egg-info/
--rw-rw-rw-   0        0        0      824 2022-10-18 16:04:07.000000 datashuttle-0.0.1/datashuttle/datashuttle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2022-10-18 16:04:07.000000 datashuttle-0.0.1/datashuttle/datashuttle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-18 16:04:07.000000 datashuttle-0.0.1/datashuttle/datashuttle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-18 16:04:07.000000 datashuttle-0.0.1/datashuttle/datashuttle.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       71 2022-10-18 16:04:07.000000 datashuttle-0.0.1/datashuttle/datashuttle.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2022-10-18 16:04:07.000000 datashuttle-0.0.1/datashuttle/datashuttle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      397 2022-10-18 16:02:32.000000 datashuttle-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1145 2022-10-18 16:04:07.565333 datashuttle-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.381699 datashuttle-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.369699 datashuttle-0.1.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.373699 datashuttle-0.1.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/.github/workflows/code_test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/.github/workflows/docs_build_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.373699 datashuttle-0.1.0rc1/datashuttle/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31473 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/command_line_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.373699 datashuttle-0.1.0rc1/datashuttle/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/canonical_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/canonical_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/canonical_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/config_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/load_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43692 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/datashuttle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.373699 datashuttle-0.1.0rc1/datashuttle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/ds_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/folder_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16658 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/rclone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.373699 datashuttle-0.1.0rc1/datashuttle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/dark-logo-gatsby.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/dark-logo-swc.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/dark-logo-ucl.png
+-rw-r--r--   0 runner    (1001) docker     (123)   171111 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/light-logo-gatsby.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/light-logo-swc.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39849 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/light-logo-ucl.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/logo_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/logo_light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_templates/footer_end.html
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_templates/footer_start.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/source/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/pages/api_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/pages/cli_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/pages/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/pages/get_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:19:58.381699 datashuttle-0.1.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/ssh_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/tests/tests_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    23408 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_command_line_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_file_conflicts_pathtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20185 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_filesystem_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18319 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_make_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_ssh_file_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_ssh_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/tests/tests_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_unit/test_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tox.ini
```

### Comparing `datashuttle-0.0.1/LICENSE` & `datashuttle-0.1.0rc1/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-
-Copyright (c) 2022, Adam Tyson
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of datashuttle nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+Copyright (c) 2023, University College London
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of movement nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

