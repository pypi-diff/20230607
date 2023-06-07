# Comparing `tmp/napari-arboretum-0.1.1.tar.gz` & `tmp/napari-arboretum-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-arboretum-0.1.1.tar", last modified: Tue Sep 13 20:19:04 2022, max compression
+gzip compressed data, was "napari-arboretum-0.1.2.tar", last modified: Wed Jun  7 14:04:26 2023, max compression
```

## Comparing `napari-arboretum-0.1.1.tar` & `napari-arboretum-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 20:19:04.481803 napari-arboretum-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 20:19:04.465802 napari-arboretum-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 20:19:04.465802 napari-arboretum-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/.github/workflows/plugin_preview.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 20:19:04.465802 napari-arboretum-0.1.1/.napari/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/.napari/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2926 2022-09-13 20:19:04.481803 napari-arboretum-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2101 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 20:19:04.477803 napari-arboretum-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)  9372517 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/examples/arboretum.gif
--rw-r--r--   0 runner    (1001) docker     (121)  1372283 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/examples/arboretum.png
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/examples/show_large_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/examples/show_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 20:19:04.477803 napari-arboretum-0.1.1/napari_arboretum/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/_hookimpls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 20:19:04.481803 napari-arboretum-0.1.1/napari_arboretum/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/_tests/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/_tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/_tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-13 20:19:04.000000 napari-arboretum-0.1.1/napari_arboretum/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4840 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4152 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 20:19:04.481803 napari-arboretum-0.1.1/napari_arboretum/sample/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/sample/registry.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/sample/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2955 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 20:19:04.481803 napari-arboretum-0.1.1/napari_arboretum/visualisation/
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6334 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/visualisation/base_plotter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/visualisation/matplotlib_plotter.py
--rw-r--r--   0 runner    (1001) docker     (121)     7594 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/napari_arboretum/visualisation/vispy_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 20:19:04.481803 napari-arboretum-0.1.1/napari_arboretum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2926 2022-09-13 20:19:04.000000 napari-arboretum-0.1.1/napari_arboretum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-09-13 20:19:04.000000 napari-arboretum-0.1.1/napari_arboretum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 20:19:04.000000 napari-arboretum-0.1.1/napari_arboretum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-09-13 20:19:04.000000 napari-arboretum-0.1.1/napari_arboretum.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-13 20:19:04.000000 napari-arboretum-0.1.1/napari_arboretum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-13 20:19:04.000000 napari-arboretum-0.1.1/napari_arboretum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-09-13 20:19:04.481803 napari-arboretum-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-09-13 20:18:47.000000 napari-arboretum-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.428947 napari-arboretum-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.412947 napari-arboretum-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.416947 napari-arboretum-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/.github/workflows/plugin_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/.github/workflows/update_project_board.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.416947 napari-arboretum-0.1.2/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-07 14:04:26.428947 napari-arboretum-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.428947 napari-arboretum-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)  9372517 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/examples/arboretum.gif
+-rw-r--r--   0 runner    (1001) docker     (123)  1372283 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/examples/arboretum.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/examples/show_large_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/examples/show_multi_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/examples/show_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:04:26.428947 napari-arboretum-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.412947 napari-arboretum-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.428947 napari-arboretum-0.1.2/src/napari_arboretum/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/_hookimpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 14:04:26.000000 napari-arboretum-0.1.2/src/napari_arboretum/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.428947 napari-arboretum-0.1.2/src/napari_arboretum/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/io/svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.428947 napari-arboretum-0.1.2/src/napari_arboretum/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/sample/registry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/sample/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.428947 napari-arboretum-0.1.2/src/napari_arboretum/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/visualisation/base_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/visualisation/matplotlib_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/src/napari_arboretum/visualisation/vispy_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.428947 napari-arboretum-0.1.2/src/napari_arboretum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-07 14:04:26.000000 napari-arboretum-0.1.2/src/napari_arboretum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-07 14:04:26.000000 napari-arboretum-0.1.2/src/napari_arboretum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:04:26.000000 napari-arboretum-0.1.2/src/napari_arboretum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 14:04:26.000000 napari-arboretum-0.1.2/src/napari_arboretum.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 14:04:26.000000 napari-arboretum-0.1.2/src/napari_arboretum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 14:04:26.000000 napari-arboretum-0.1.2/src/napari_arboretum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:04:26.428947 napari-arboretum-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/tests/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-07 14:04:08.000000 napari-arboretum-0.1.2/tests/test_sample_data.py
```

### Comparing `napari-arboretum-0.1.1/.github/workflows/test_and_deploy.yml` & `napari-arboretum-0.1.2/.github/workflows/test_and_deploy.yml`

 * *Files 6% similar despite different names*

```diff
@@ -8,55 +8,51 @@
       - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
   pull_request:
     branches:
       - main
   workflow_dispatch:
 
 jobs:
-  linting:
-      runs-on: ubuntu-latest
-      steps:
-        - uses: UCL/composite-actions/pre-commit@v1
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
         # Run all supported Python versions on linux
         python-version: ["3.8", "3.9", "3.10"]
         platform: [ubuntu-latest]
         # Include one windows and macos run
         include:
-        - platform: macos-latest
-          python-version: "3.9"
-        - platform: windows-latest
-          python-version: "3.9"
+          - platform: macos-latest
+            python-version: "3.9"
+          - platform: windows-latest
+            python-version: "3.9"
 
     steps:
       # Setup pyqt libraries
       - uses: tlambert03/setup-qt-libs@v1
       # Run tests
       - uses: UCL/composite-actions/python/tox@v1
         with:
           python-version: ${{ matrix.python-version }}
       # Upload code coverage
       - name: Coverage
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v3
 
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your
     # github secrets (see readme for details)
     needs: [test]
     runs-on: ubuntu-latest
     if: contains(github.ref, 'tags')
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install build twine
       - name: Build and publish
```

### Comparing `napari-arboretum-0.1.1/LICENSE.md` & `napari-arboretum-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `napari-arboretum-0.1.1/PKG-INFO` & `napari-arboretum-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 Metadata-Version: 2.1
 Name: napari-arboretum
-Version: 0.1.1
+Version: 0.1.2
 Summary: Track graph and lineage tree visualization with napari
-Home-page: https://github.com/quantumjot/arboretum
-Author: Alan R. Lowe
-Author-email: a.lowe@ucl.ac.uk
-License: LICENCE.md
+Author-email: "Alan R. Lowe" <a.lowe@ucl.ac.uk>
+Project-URL: homepage, https://github.com/lowe-lab-ucl/arboretum
 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
-Classifier: Topic :: Software Development :: Testing
-Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
  <!--[![Downloads](https://pepy.tech/badge/napari-arboretum)](https://pepy.tech/project/napari-arboretum)-->
-[![License](https://img.shields.io/pypi/l/napari-arboretum.svg?color=green)](https://github.com/lowe-lab-ucl/napari-arboretum/raw/master/LICENSE)
+
+[![License](https://img.shields.io/pypi/l/napari-arboretum.svg?color=green)](https://github.com/lowe-lab-ucl/arboretum/blob/main/LICENSE.md)
 [![PyPI](https://img.shields.io/pypi/v/napari-arboretum.svg?color=green)](https://pypi.org/project/napari-arboretum)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-arboretum.svg?color=green)](https://python.org)
-[![tests](https://github.com/lowe-lab-ucl/arboretum/workflows/tests/badge.svg)](https://github.com/quantumjot/arboretum/actions)
-[![codecov](https://codecov.io/gh/lowe-lab-ucl/arboretum/branch/master/graph/badge.svg?token=2M2HhM60op)](https://codecov.io/gh/lowe-lab-ucl/arboretum)
+[![tests](https://github.com/lowe-lab-ucl/arboretum/workflows/tests/badge.svg)](https://github.com/lowe-lab-ucl/arboretum/actions)
+[![codecov](https://codecov.io/gh/lowe-lab-ucl/arboretum/branch/main/graph/badge.svg?token=2M2HhM60op)](https://app.codecov.io/gh/lowe-lab-ucl/arboretum/tree/main)
 
 # Arboretum
 
 
-![](https://raw.githubusercontent.com/lowe-lab-ucl/arboretum/master/examples/arboretum.gif)
-*Automated cell tracking and lineage tree reconstruction*.
+
+https://github.com/lowe-lab-ucl/arboretum/assets/8217795/d98c22c4-73bb-493a-9f8f-c224d615209d
+
+
+_Automated cell tracking and lineage tree reconstruction_.
 
 ### Overview
 
-A dockable widget for [Napari](https://github.com/napari) for visualizing cell lineage trees.
+A dockable widget for [Napari](https://github.com/napari/napari) for visualizing cell lineage trees.
 
 Features:
-+ Lineage tree plot widget
-+ Integration with [btrack](https://github.com/quantumjot/BayesianTracker)
+
+- Lineage tree plot widget
+- Integration with [btrack](https://github.com/quantumjot/btrack)
 
 ---
 
 ### Usage
 
-Once installed, Arboretum will be visible in the `Plugins > Add Dock Widget > napari-arboretum` menu in napari.  To visualize a lineage tree, (double) click on one of the tracks in a napari `Tracks` layer.
-
-
+Once installed, Arboretum will be visible in the `Plugins > Add Dock Widget > napari-arboretum` menu in napari. To visualize a lineage tree, (double) click on one of the tracks in a napari `Tracks` layer.
 
 ### Examples
 
 You can use the example script to display some sample tracking data in napari and load the arboretum tree viewer:
 
 ```sh
 python ./examples/show_sample_data.py
 ```
 
-Alternatively, you can use *btrack* to generate tracks from your image data. See the example notebook here:
-https://github.com/quantumjot/BayesianTracker/blob/master/examples
+Alternatively, you can use _btrack_ to generate tracks from your image data. See the example notebook here:
+https://github.com/quantumjot/btrack/blob/main/examples
 
 ---
 
 ### History
 
 This project has changed considerably. The `Tracks` layer, originally developed for this plugin, is now an official layer type in napari. Read the napari documentation here:
- https://napari.org/api/napari.layers.Tracks.html
-
+https://napari.org/stable/api/napari.layers.Tracks.html
 
 To view the legacy version of this plugin, visit the legacy branch:
 https://github.com/quantumjot/arboretum/tree/v1-legacy
```

### Comparing `napari-arboretum-0.1.1/README.md` & `napari-arboretum-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,52 @@
  <!--[![Downloads](https://pepy.tech/badge/napari-arboretum)](https://pepy.tech/project/napari-arboretum)-->
-[![License](https://img.shields.io/pypi/l/napari-arboretum.svg?color=green)](https://github.com/lowe-lab-ucl/napari-arboretum/raw/master/LICENSE)
+
+[![License](https://img.shields.io/pypi/l/napari-arboretum.svg?color=green)](https://github.com/lowe-lab-ucl/arboretum/blob/main/LICENSE.md)
 [![PyPI](https://img.shields.io/pypi/v/napari-arboretum.svg?color=green)](https://pypi.org/project/napari-arboretum)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-arboretum.svg?color=green)](https://python.org)
-[![tests](https://github.com/lowe-lab-ucl/arboretum/workflows/tests/badge.svg)](https://github.com/quantumjot/arboretum/actions)
-[![codecov](https://codecov.io/gh/lowe-lab-ucl/arboretum/branch/master/graph/badge.svg?token=2M2HhM60op)](https://codecov.io/gh/lowe-lab-ucl/arboretum)
+[![tests](https://github.com/lowe-lab-ucl/arboretum/workflows/tests/badge.svg)](https://github.com/lowe-lab-ucl/arboretum/actions)
+[![codecov](https://codecov.io/gh/lowe-lab-ucl/arboretum/branch/main/graph/badge.svg?token=2M2HhM60op)](https://app.codecov.io/gh/lowe-lab-ucl/arboretum/tree/main)
 
 # Arboretum
 
 
-![](https://raw.githubusercontent.com/lowe-lab-ucl/arboretum/master/examples/arboretum.gif)
-*Automated cell tracking and lineage tree reconstruction*.
+
+https://github.com/lowe-lab-ucl/arboretum/assets/8217795/d98c22c4-73bb-493a-9f8f-c224d615209d
+
+
+_Automated cell tracking and lineage tree reconstruction_.
 
 ### Overview
 
-A dockable widget for [Napari](https://github.com/napari) for visualizing cell lineage trees.
+A dockable widget for [Napari](https://github.com/napari/napari) for visualizing cell lineage trees.
 
 Features:
-+ Lineage tree plot widget
-+ Integration with [btrack](https://github.com/quantumjot/BayesianTracker)
+
+- Lineage tree plot widget
+- Integration with [btrack](https://github.com/quantumjot/btrack)
 
 ---
 
 ### Usage
 
-Once installed, Arboretum will be visible in the `Plugins > Add Dock Widget > napari-arboretum` menu in napari.  To visualize a lineage tree, (double) click on one of the tracks in a napari `Tracks` layer.
-
-
+Once installed, Arboretum will be visible in the `Plugins > Add Dock Widget > napari-arboretum` menu in napari. To visualize a lineage tree, (double) click on one of the tracks in a napari `Tracks` layer.
 
 ### Examples
 
 You can use the example script to display some sample tracking data in napari and load the arboretum tree viewer:
 
 ```sh
 python ./examples/show_sample_data.py
 ```
 
-Alternatively, you can use *btrack* to generate tracks from your image data. See the example notebook here:
-https://github.com/quantumjot/BayesianTracker/blob/master/examples
+Alternatively, you can use _btrack_ to generate tracks from your image data. See the example notebook here:
+https://github.com/quantumjot/btrack/blob/main/examples
 
 ---
 
 ### History
 
 This project has changed considerably. The `Tracks` layer, originally developed for this plugin, is now an official layer type in napari. Read the napari documentation here:
- https://napari.org/api/napari.layers.Tracks.html
-
+https://napari.org/stable/api/napari.layers.Tracks.html
 
 To view the legacy version of this plugin, visit the legacy branch:
 https://github.com/quantumjot/arboretum/tree/v1-legacy
```

### Comparing `napari-arboretum-0.1.1/examples/arboretum.gif` & `napari-arboretum-0.1.2/examples/arboretum.gif`

 * *Files identical despite different names*

### Comparing `napari-arboretum-0.1.1/examples/arboretum.png` & `napari-arboretum-0.1.2/examples/arboretum.png`

 * *Files identical despite different names*

### Comparing `napari-arboretum-0.1.1/examples/show_large_tree.py` & `napari-arboretum-0.1.2/examples/show_large_tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """
 Show a large tree in arboretum
 ==============================
 """
+import logging
 from copy import copy
 
 import napari
+import numpy as np
 
-from napari_arboretum import Arboretum
 from napari_arboretum.graph import TreeNode
 
 
 def generate_binary_tree(max_depth: int):
-    id = 0
-    nodes = [TreeNode(id, t=(0, 1), generation=1)]
+    track_id = 0
+    t = np.array([0, 1])
+    nodes = [TreeNode(track_id, t=t, generation=1)]
     for depth in range(1, max_depth):
         for node in copy(nodes):
             if node.generation == depth:
                 for _ in range(2):
                     # Add two children
-                    id += 1
-                    new_node = node.add_child(id, t_end=node.t[-1] + 1)
+                    track_id += 1
+                    new_node = node.add_child(track_id, t_end=node.t[-1] + 1)
                     nodes.append(new_node)
     return nodes
 
 
 nodes = generate_binary_tree(8)
-print(f"{len(nodes)} total nodes")
+logging.info(f"{len(nodes)} total nodes")
 
 
 viewer = napari.Viewer()
 _, widget = viewer.window.add_plugin_dock_widget(
     plugin_name="napari-arboretum", widget_name="Arboretum"
 )
 widget.plotter.draw_from_nodes(nodes)
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # The napari event loop needs to be run under here to allow the window
     # to be spawned from a Python script
     napari.run()
```

### Comparing `napari-arboretum-0.1.1/examples/show_sample_data.py` & `napari-arboretum-0.1.2/examples/show_sample_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 - loads some sample data
 - adds the data to a napari viewer
 - loads the arboretum plugin
 - opens the napari viewer
 """
 import napari
 
-from napari_arboretum import load_sample_data
+from napari_arboretum.sample.sample_data import load_sample_data
 
 track, segmentation = load_sample_data()
 
 viewer = napari.Viewer()
 viewer.add_layer(segmentation)
 viewer.add_layer(track)
 viewer.window.add_plugin_dock_widget(
     plugin_name="napari-arboretum", widget_name="Arboretum"
 )
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # The napari event loop needs to be run under here to allow the window
     # to be spawned from a Python script
     napari.run()
```

### Comparing `napari-arboretum-0.1.1/napari_arboretum/_tests/test_dock_widget.py` & `napari-arboretum-0.1.2/tests/test_dock_widget.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import pytest
 
-from napari_arboretum import napari_experimental_provide_dock_widget
-
 # this is your plugin name declared in your napari.plugins entry point
 MY_PLUGIN_NAME = "napari-arboretum"
 # the name of your widget(s)
 MY_WIDGET_NAMES = ["Arboretum"]
 
 
 @pytest.mark.parametrize("widget_name", MY_WIDGET_NAMES)
```

### Comparing `napari-arboretum-0.1.1/napari_arboretum/_tests/test_graph.py` & `napari-arboretum-0.1.2/tests/test_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-import pytest
 from napari.layers import Tracks
+from numpy.testing import assert_allclose
 
 from napari_arboretum import graph
 
 TEST_GRAPH = {1: [0], 2: [0], 3: [1], 4: [1], 5: [2], 6: [2]}
 TEST_GRAPH_REVERSE = {0: [1, 2], 1: [3, 4], 2: [5, 6]}
 TEST_GRAPH_ROOT = 0
 TEST_GRAPH_LINEAR = [0, 1, 2, 3, 4, 5, 6]
@@ -69,8 +69,8 @@
     assert node.is_leaf
     child = node.add_child(2, t_end=4)
 
     assert not node.is_leaf
     assert len(node.children) == 1
 
     assert child.is_leaf
-    assert child.t == (2, 4)
+    assert_allclose(child.t, (2, 4))
```

### Comparing `napari-arboretum-0.1.1/napari_arboretum/_tests/test_plugin.py` & `napari-arboretum-0.1.2/tests/test_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pytest
-from napari import layers
 
-from napari_arboretum import Arboretum, load_sample_data
+from napari_arboretum.plugin import Arboretum
+from napari_arboretum.sample.sample_data import load_sample_data
 
 
 @pytest.fixture
 def viewer_plugin(make_napari_viewer):
     """
     - Create a a napari viewer
     - Add sample tracks and segmentation
@@ -36,43 +36,43 @@
 
 def test_colormap_change(viewer_plugin):
     """
     Check that arboretum widget colours change when the track colourmap
     is changed.
     """
     viewer, plugin = viewer_plugin
-    id = 140
-    plugin.track_id = id
+    track_id = 140
+    plugin.track_id = track_id
 
     tree = plugin.plotter.tree
-    old_color = tree.get_branch_color(branch_id=id)
+    old_color = tree.get_branch_color(branch_id=track_id)
 
     # Change the colormap
     assert viewer.layers[0].colormap != "viridis"
     viewer.layers[0].colormap = "viridis"
 
     # Check that color has changed
-    new_color = tree.get_branch_color(branch_id=id)
+    new_color = tree.get_branch_color(branch_id=track_id)
     # Slice to remove alpha, which is 1 both before and after
     assert np.all(new_color[:, :3] != old_color[:, :3])
 
 
 def test_colorby_change(viewer_plugin):
     """
     Check that arboretum widget colours change when the attribute that the
     track is coloured by changes.
     """
     viewer, plugin = viewer_plugin
-    id = 140
-    plugin.track_id = id
+    track_id = 140
+    plugin.track_id = track_id
 
     tree = plugin.plotter.tree
-    old_color = tree.get_branch_color(branch_id=id)
+    old_color = tree.get_branch_color(branch_id=track_id)
 
     # Change the color by attribute
     assert viewer.layers[0].color_by != "generation"
     viewer.layers[0].color_by = "generation"
 
     # Check that color has changed
-    new_color = tree.get_branch_color(branch_id=id)
+    new_color = tree.get_branch_color(branch_id=track_id)
     # Slice to remove alpha, which is 1 both before and after
     assert np.all(new_color[:, :3] != old_color[:, :3])
```

### Comparing `napari-arboretum-0.1.1/napari_arboretum/graph.py` & `napari-arboretum-0.1.2/src/napari_arboretum/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 """
 Classes and functions for working with graphs.
 
 Note that this file should *not* contain code for laying out the graphs for
 visualisation. Code for this is kept in `tree.py`.
 """
+from __future__ import annotations
+
 from dataclasses import dataclass, field
-from typing import Dict, List, Set, Tuple, Union
 
 import napari
 import numpy as np
 
 
 @dataclass
 class TreeNode:
     """TreeNode."""
 
     ID: int
     t: np.ndarray
     generation: int
-    children: List[int] = field(default_factory=list)
+    children: list[int] = field(default_factory=list)
 
     @property
     def is_root(self) -> bool:
         return self.generation == 1
 
     @property
     def is_leaf(self) -> bool:
         return not self.children
 
-    def add_child(self, id: int, *, t_end: int):
+    def add_child(self, track_id: int, *, t_end: int):
         """
         Add a child to this node, and return the child.
         """
-        child = TreeNode(id, (self.t[-1], t_end), self.generation + 1)
-        self.children.append(id)
+        t = np.asarray([self.t[-1], t_end])
+        child = TreeNode(track_id, t, self.generation + 1)
+        self.children.append(track_id)
         return child
 
 
-def build_reverse_graph(graph: dict) -> Tuple[Union[list, set], Dict[int, List[int]]]:
+def build_reverse_graph(graph: dict) -> tuple[list | set, dict[int, list[int]]]:
     """Take the data from a Tracks layer graph and reverse it.
 
     Parameters
     ----------
     graph : dict
         A dictionary encoding the graph, taken from the napari.Tracks layer.
 
@@ -50,29 +52,29 @@
     -------
     roots : int, None
         A sorted list of integers represent the root node IDs
     reverse_graph : dict
         A reversed graph representing children of each parent node.
     """
     reverse_graph = {}
-    roots: Set[int] = set()
+    roots: set[int] = set()
 
     # iterate over the graph, reverse it and find the root nodes
     for node, parents in graph.items():
         for parent in parents:
             if parent not in reverse_graph:
                 reverse_graph[parent] = [node]
             else:
                 reverse_graph[parent].append(node)
 
             if parent not in graph.keys():
                 roots.add(parent)
 
     # sort the roots
-    sorted_roots = sorted(list(roots))
+    sorted_roots = sorted(roots)
 
     return sorted_roots, reverse_graph
 
 
 def linearise_tree(graph: dict, root: int) -> list:
     """Linearise a tree, i.e. return a list of track objects in the tree, but
     discard the heirarchy.
@@ -92,16 +94,15 @@
     """
     queue = [root]
     linear = []
     while queue:
         node = queue.pop(0)
         linear.append(node)
         if node in graph:
-            for child in graph[node]:
-                queue.append(child)
+            queue.extend(iter(graph[node]))
     return linear
 
 
 def get_root_id(layer: napari.layers.Tracks, search_node: int) -> int:
     """
     Get the root node of a given track ID.
 
@@ -124,15 +125,15 @@
     for root, tree in zip(roots, linear_trees):
         if search_node in tree:
             root_id = root
 
     return root_id
 
 
-def build_subgraph(layer: napari.layers.Tracks, search_node: int) -> List[TreeNode]:
+def build_subgraph(layer: napari.layers.Tracks, search_node: int) -> list[TreeNode]:
     """Build a subgraph containing the node.
 
     The search node may not be the root of a tree, therefore, this function
     searches the whole graph to find a subgraph (tree) that contains the search
     node.
 
     Parameters
@@ -148,16 +149,15 @@
     nodes :
         The nodes of the subtree that contain the search node.
     """
     _, reverse_graph = build_reverse_graph(layer.graph)
     root_id = get_root_id(layer, search_node)
 
     def _node_from_graph(_id):
-
-        idx = np.where(layer.data[:, 0] == _id)[0]
+        idx = layer.data[:, 0] == _id
         # t = (np.min(layer.data[idx, 1]), np.max(layer.data[idx, 1]))
         t = layer.data[idx, 1]
         node = TreeNode(ID=_id, t=t, generation=1)
 
         if _id in reverse_graph:
             node.children = reverse_graph[_id]
```

### Comparing `napari-arboretum-0.1.1/napari_arboretum/plugin.py` & `napari-arboretum-0.1.2/src/napari_arboretum/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,87 @@
-from typing import List, Optional
+from __future__ import annotations
 
 import napari
 from napari.layers import Tracks
 from napari.utils.events import Event
-from PyQt5.QtCore import Qt
-from qtpy.QtWidgets import QGridLayout, QLabel, QWidget
+from qtpy.QtCore import Qt
+from qtpy.QtWidgets import QFileDialog, QGridLayout, QLabel, QPushButton, QWidget
 
 from napari_arboretum.graph import get_root_id
-
-from .util import TrackPropertyMixin
-from .visualisation import (
-    MPLPropertyPlotter,
+from napari_arboretum.io.svg import export_svg
+from napari_arboretum.util import TrackPropertyMixin
+from napari_arboretum.visualisation.base_plotter import (
     PropertyPlotterBase,
     TreePlotterQWidgetBase,
-    VisPyPlotter,
 )
+from napari_arboretum.visualisation.matplotlib_plotter import MPLPropertyPlotter
+from napari_arboretum.visualisation.vispy_plotter import VisPyPlotter
 
-GUI_MAXIMUM_WIDTH = 400
+GUI_MAXIMUM_WIDTH = 500
 
 
 class Arboretum(QWidget, TrackPropertyMixin):
     """
     Tree viewer widget.
     """
 
-    def __init__(self, viewer: napari.Viewer, parent=None):
+    def __init__(self, viewer: napari.Viewer = None, parent=None):
         super().__init__(parent=parent)
+        viewer = napari.current_viewer() if viewer is None else viewer
         self.viewer = viewer
         self.title = QLabel()
         self.plotter: TreePlotterQWidgetBase = VisPyPlotter()
         self.property_plotter: PropertyPlotterBase = MPLPropertyPlotter(viewer)
+        self.setMaximumWidth(GUI_MAXIMUM_WIDTH)
 
         # Set plugin layout
         layout = QGridLayout()
 
         row, col = 0, 0
         # Add title
         layout.addWidget(self.title, row, col, Qt.AlignHCenter)
         self.title.setText("Arboretum")
 
         # Add tree plotter
         row = 1
         layout.addWidget(self.plotter.get_qwidget(), row, col)
-        # Add property plotter
+        # Add export button
         row = 2
+        self.export_button = QPushButton("Export tree as SVG")
+        layout.addWidget(self.export_button, row, col)
+        # Add property plotter
+        row = 3
         layout.addWidget(self.property_plotter.get_qwidget(), row, col)
         # Make the tree plot a bigger than the property plot
-        for row, stretch in zip([1, 2], [2, 1]):
+        for row, stretch in zip([1, 2, 3], [4, 1, 2]):
             layout.setRowStretch(row, stretch)
         self.setLayout(layout)
 
         # Update the list of tracks layers stored in this object if the layer
         # list changes
         self.viewer.layers.events.changed.connect(self.update_tracks_layers)
         # Update the horizontal time line if the current z-step changes
         self.viewer.dims.events.current_step.connect(self.draw_current_time_line)
+        # Save the tree as an SVG
+        self.export_button.clicked.connect(self.export_tree)
 
-        self.tracks_layers: List[Tracks] = []
+        self.tracks_layers: list[Tracks] = []
         self.update_tracks_layers()
 
     def on_tracks_change(self):
         self.plotter.tracks = self.tracks
         self.property_plotter.tracks = self.tracks
 
     def on_track_id_change(self):
         self.plotter.track_id = self.track_id
         self.property_plotter.track_id = self.track_id
         root_id = get_root_id(self.tracks, self.track_id)
         self.title.setText(f"Lineage Tree #{root_id}")
 
-    def update_tracks_layers(self, event: Optional[Event] = None) -> None:
+    def update_tracks_layers(self, event: Event | None = None) -> None:
         """
         Save a copy of all the tracks layers that are present in the viewer.
         """
         layers = [layer for layer in self.viewer.layers if isinstance(layer, Tracks)]
 
         for layer in layers:
             if layer not in self.tracks_layers:
@@ -101,13 +109,27 @@
             track_id = tracks.get_value(cursor_position, world=True)
             if track_id is not None:
                 # Setting this property automatically triggers re-drawing of the
                 # tree and property graph
                 self.track_id = track_id
                 self.draw_current_time_line()
 
-    def draw_current_time_line(self, event: Optional[Event] = None) -> None:
+    def draw_current_time_line(self, event: Event | None = None) -> None:
         if not self.plotter.has_tracks:
             return
         z_value = self.viewer.dims.current_step[0]
         self.plotter.draw_current_time_line(z_value)
         self.property_plotter.draw_current_time_line(z_value)
+
+    def export_tree(self) -> None:
+        """Export the tree as an SVG."""
+        root_id = get_root_id(self.tracks, self.track_id)
+        options = QFileDialog.Options()
+        filename, _ = QFileDialog.getSaveFileName(
+            self,
+            "Export tree as SVG",
+            f"tree_{root_id}.svg",
+            "SVG Files(*.svg)",
+            options=options,
+        )
+        if filename:
+            export_svg(filename, self.plotter.edges, self.plotter.annotations)
```

### Comparing `napari-arboretum-0.1.1/napari_arboretum/sample/registry.txt` & `napari-arboretum-0.1.2/src/napari_arboretum/sample/registry.txt`

 * *Files identical despite different names*

### Comparing `napari-arboretum-0.1.1/napari_arboretum/sample/sample_data.py` & `napari-arboretum-0.1.2/src/napari_arboretum/sample/sample_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Functions to load sample data.
 
 The sample data fetching/caching is handled by the `pooch` library. A registry
 of files and their expected hashes is stored in :file:``registry.txt``.
 """
 
+from __future__ import annotations
+
 import json
 import pathlib
-from typing import Tuple
 
 import napari.layers
 import pandas as pd
 import pooch
 from skimage.io import imread
 
 POOCH_BASE = "https://raw.githubusercontent.com/lowe-lab-ucl/btrack-examples/main/"
@@ -19,15 +20,15 @@
     path=pooch.os_cache("arboretum"), base_url=POOCH_BASE, registry=None
 )
 
 registry_file = pathlib.Path(__file__).parent / "registry.txt"
 POOCH.load_registry(registry_file)
 
 
-def load_sample_data() -> Tuple[napari.layers.Tracks, napari.layers.Labels]:
+def load_sample_data() -> tuple[napari.layers.Tracks, napari.layers.Labels]:
     """
     Load some sample data.
 
     Returns
     -------
     tracks : napari.layers.Tracks
     segmentation : napari.layers.Labels
```

### Comparing `napari-arboretum-0.1.1/napari_arboretum/util.py` & `napari-arboretum-0.1.2/src/napari_arboretum/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from napari.layers import Tracks
 
 
 class TrackPropertyMixin:
     """
     Mixin class to add ``.tracks`` and ``.track_id`` properties.
     """
```

### Comparing `napari-arboretum-0.1.1/napari_arboretum/visualisation/base_plotter.py` & `napari-arboretum-0.1.2/src/napari_arboretum/visualisation/base_plotter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+from __future__ import annotations
+
 import abc
-from typing import List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 from qtpy.QtWidgets import QWidget
 
-from ..graph import TreeNode, build_subgraph
-from ..tree import Annotation, Edge, layout_tree
-from ..util import TrackPropertyMixin
-
-# from ..profiler import profiler
+from napari_arboretum.graph import TreeNode, build_subgraph
+from napari_arboretum.tree import Annotation, Edge, layout_tree
+from napari_arboretum.util import TrackPropertyMixin
 
 GUI_MAXIMUM_WIDTH = 600
 
 __all__ = ["TreePlotterBase", "TreePlotterQWidgetBase"]
 
 
 class TreePlotterBase(abc.ABC, TrackPropertyMixin):
@@ -44,46 +43,43 @@
         """
         Plot the tree.
         """
         self.clear()
         subgraph_nodes = build_subgraph(self.tracks, self.track_id)
         self.draw_from_nodes(subgraph_nodes, self.track_id)
 
-    # @profiler("draw_from_nodes")
-    def draw_from_nodes(
-        self, tree_nodes: List[TreeNode], track_id: Optional[int] = None
-    ):
+    def draw_from_nodes(self, tree_nodes: list[TreeNode], track_id: int | None = None):
         self.edges, self.annotations = layout_tree(tree_nodes)
 
         if self.has_tracks:
             self.update_edge_colors(update_live=False)
 
         for e in self.edges:
             self.add_branch(e)
 
         # labels
         for a in self.annotations:
             self.add_annotation(a)
 
         self.draw_tree_visual()
 
-    def update_edge_colors(self, update_live: bool = True) -> None:
+    def update_edge_colors(self, *, update_live: bool = True) -> None:
         """
         Update tree edge colours from the track properties.
 
         Parameters
         ----------
         update_live : bool
             If `True`, also call `update_colors()` on the plotting backend
             to update the colors in a live plot.
         """
         for e in self.edges:
-            if e.id is not None:
+            if e.track_id is not None:
                 e.color = self.tracks.track_colors[
-                    self.tracks.properties["track_id"] == e.id
+                    self.tracks.properties["track_id"] == e.track_id
                 ]
 
         if update_live:
             self.update_colors()
 
     @abc.abstractmethod
     def update_colors(self) -> None:
@@ -163,29 +159,30 @@
         self.clear()
         self.plot(t, prop)
         self.set_xlabel("Time")
         self.set_ylabel("Property value")
         self.set_title(f"{self.tracks.color_by}, cell #{self.track_id}")
         self.redraw()
 
-    def get_track_properties(self) -> Tuple[np.ndarray, np.ndarray]:
+    def get_track_properties(self) -> tuple[np.ndarray, np.ndarray]:
         """
         For a given layer and track_id, get time values and property that
         the track is currently coloured by.
 
         Returns
         -------
         t :
             Time values.
         prop :
             Property values.
         """
         all_props = pd.DataFrame(self.tracks.properties)
         all_props = all_props.loc[all_props["track_id"] == self.track_id]
-        return all_props["t"].values, all_props[self.tracks.color_by].values
+        t = self.tracks.data[self.tracks.data[:, 0] == self.track_id, 1]
+        return t, all_props[self.tracks.color_by].values
 
     @abc.abstractmethod
     def get_qwidget(self) -> QWidget:
         """
         Return the native QWidget for embedding.
         """
```

### Comparing `napari-arboretum-0.1.1/napari_arboretum/visualisation/matplotlib_plotter.py` & `napari-arboretum-0.1.2/src/napari_arboretum/visualisation/matplotlib_plotter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Optional
+from __future__ import annotations
 
 import numpy as np
 from matplotlib.lines import Line2D
 from napari_matplotlib.base import NapariMPLWidget
 from qtpy.QtWidgets import QWidget
 
-from .base_plotter import PropertyPlotterBase
+from napari_arboretum.visualisation.base_plotter import PropertyPlotterBase
 
 
 class MPLPropertyPlotter(PropertyPlotterBase):
     def __init__(self, viewer):
         self.mpl_widget = NapariMPLWidget(viewer)
         self.figure = self.mpl_widget.canvas.figure
         self.axes = self.mpl_widget.canvas.figure.add_subplot(111)
-        self.mpl_time_line: Optional[Line2D] = None
+        self.mpl_time_line: Line2D | None = None
 
     def get_qwidget(self) -> QWidget:
         return self.mpl_widget
 
     def plot(self, x: np.ndarray, y: np.ndarray) -> None:
         self.axes.plot(x, y, label=f"id={self.track_id}")
```

### Comparing `napari-arboretum-0.1.1/napari_arboretum/visualisation/vispy_plotter.py` & `napari-arboretum-0.1.2/src/napari_arboretum/visualisation/vispy_plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 
 import numpy as np
 from qtpy.QtWidgets import QWidget
 from vispy import scene
 
-from ..tree import Annotation, Edge
-from .base_plotter import TreePlotterQWidgetBase
+from napari_arboretum.tree import Annotation, Edge
+from napari_arboretum.visualisation.base_plotter import TreePlotterQWidgetBase
 
 __all__ = ["VisPyPlotter"]
 
 
 DEFAULT_TEXT_SIZE = 8
 DEFAULT_BRANCH_WIDTH = 3
+TWO_DIM = 2
 
 
 @dataclass
 class Bounds:
     xmin: float
     xmax: float
     ymin: float
@@ -25,22 +28,20 @@
 @dataclass
 class TrackSubvisualProxy:
     pos: np.ndarray
     color: np.ndarray = np.array([1.0, 1.0, 1.0, 1.0])
 
     @property
     def connex(self):
-        connex = [True] * (self.pos.shape[0] - 1) + [False]
-        return connex
+        return [True] * (self.pos.shape[0] - 1) + [False]
 
     @property
     def safe_color(self) -> np.ndarray:
-        if self.color.ndim != 2:
-            safe_color = np.repeat([self.color], self.pos.shape[0], axis=0)
-            return safe_color
+        if self.color.ndim != TWO_DIM:
+            return np.repeat([self.color], self.pos.shape[0], axis=0)
         return self.color
 
 
 @dataclass
 class AnnotationSubvisualProxy:
     pos: np.ndarray
     text: str
@@ -77,55 +78,60 @@
 
     @property
     def bounds(self) -> Bounds:
         """
         Return (xmin, ymin, xmax, ymax) bounds of the drawn tree. This does
         not include any annoatations.
         """
-        xs = np.concatenate([track.pos[:, 0] for id, track in self.tree.tracks.items()])
-        ys = np.concatenate([track.pos[:, 1] for id, track in self.tree.tracks.items()])
+        xs = np.concatenate(
+            [track.pos[:, 0] for track_id, track in self.tree.tracks.items()]
+        )
+        ys = np.concatenate(
+            [track.pos[:, 1] for track_id, track in self.tree.tracks.items()]
+        )
         return Bounds(
             xmin=np.min(xs), ymin=np.min(ys), xmax=np.max(xs), ymax=np.max(ys)
         )
 
     def autoscale_view(self) -> None:
         """Scale the canvas so all branches are in view."""
-        xs = np.concatenate([track.pos[:, 0] for id, track in self.tree.tracks.items()])
-        ys = np.concatenate([track.pos[:, 1] for id, track in self.tree.tracks.items()])
+        xs = np.concatenate(
+            [track.pos[:, 0] for track_id, track in self.tree.tracks.items()]
+        )
+        ys = np.concatenate(
+            [track.pos[:, 1] for track_id, track in self.tree.tracks.items()]
+        )
         padding = 0.1
         width, height = np.ptp(xs), np.ptp(ys)
         rect = (
             np.min(xs) - padding * width,
             np.min(ys) - padding * height,
             width * (1 + 2 * padding),
             height * (1 + 2 * padding),
         )
 
         # change the aspect ratio of the camera if we have just a single branch
         # this will centre the camera on the single branch, otherwise, set the
         # aspect ratio to match the data
-        if width == 0:
-            self.view.camera.aspect = 1.0
-        else:
-            self.view.camera.aspect = None
+        self.view.camera.aspect = 1.0 if width == 0 else None
         self.view.camera.rect = rect
 
     def update_colors(self) -> None:
         """
         Update plotted track colors from the colors in self.edges.
         """
         for e in self.edges:
-            if e.id is not None:
-                self.tree.set_branch_color(e.id, e.color)
+            if e.track_id is not None:
+                self.tree.set_branch_color(e.track_id, e.color)
 
     def add_branch(self, e: Edge) -> None:
         """
         Add a single branch to the tree.
         """
-        # self.tree.add_track(e.id, np.column_stack((e.y, e.x)), e.color)
+        # self.tree.add_track(e.track_id, np.column_stack((e.y, e.x)), e.color)
         self.tree.add_track(e)
         self.autoscale_view()
 
     def add_annotation(self, a: Annotation) -> None:
         """
         Add a single label to the tree.
         """
@@ -214,23 +220,22 @@
             ys = np.asarray(e.node.t)  # np.arange(pos[0, 1], pos[1, 1] + 1)
             xs = np.ones(ys.size) * pos[0, 0]
             subvisual_proxy = TrackSubvisualProxy(
                 pos=np.column_stack((xs, ys)),
                 color=color,
             )
             # store a reference to this subvisual proxy
-            self.tracks[e.id] = subvisual_proxy
+            self.tracks[e.track_id] = subvisual_proxy
 
         self.edges.append(subvisual_proxy)
 
     def add_annotation(self, x: float, y: float, label: str, color):
-
         subvisual_proxy = AnnotationSubvisualProxy(
             text=label,
-            pos=[y, x, 0],
+            pos=np.array([y, x, 0]),
         )
 
         self.annotations.append(subvisual_proxy)
 
     def clear(self) -> None:
         """Remove all tracks."""
         self.tracks = {}
```

### Comparing `napari-arboretum-0.1.1/napari_arboretum.egg-info/PKG-INFO` & `napari-arboretum-0.1.2/src/napari_arboretum.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 Metadata-Version: 2.1
 Name: napari-arboretum
-Version: 0.1.1
+Version: 0.1.2
 Summary: Track graph and lineage tree visualization with napari
-Home-page: https://github.com/quantumjot/arboretum
-Author: Alan R. Lowe
-Author-email: a.lowe@ucl.ac.uk
-License: LICENCE.md
+Author-email: "Alan R. Lowe" <a.lowe@ucl.ac.uk>
+Project-URL: homepage, https://github.com/lowe-lab-ucl/arboretum
 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
-Classifier: Topic :: Software Development :: Testing
-Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
  <!--[![Downloads](https://pepy.tech/badge/napari-arboretum)](https://pepy.tech/project/napari-arboretum)-->
-[![License](https://img.shields.io/pypi/l/napari-arboretum.svg?color=green)](https://github.com/lowe-lab-ucl/napari-arboretum/raw/master/LICENSE)
+
+[![License](https://img.shields.io/pypi/l/napari-arboretum.svg?color=green)](https://github.com/lowe-lab-ucl/arboretum/blob/main/LICENSE.md)
 [![PyPI](https://img.shields.io/pypi/v/napari-arboretum.svg?color=green)](https://pypi.org/project/napari-arboretum)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-arboretum.svg?color=green)](https://python.org)
-[![tests](https://github.com/lowe-lab-ucl/arboretum/workflows/tests/badge.svg)](https://github.com/quantumjot/arboretum/actions)
-[![codecov](https://codecov.io/gh/lowe-lab-ucl/arboretum/branch/master/graph/badge.svg?token=2M2HhM60op)](https://codecov.io/gh/lowe-lab-ucl/arboretum)
+[![tests](https://github.com/lowe-lab-ucl/arboretum/workflows/tests/badge.svg)](https://github.com/lowe-lab-ucl/arboretum/actions)
+[![codecov](https://codecov.io/gh/lowe-lab-ucl/arboretum/branch/main/graph/badge.svg?token=2M2HhM60op)](https://app.codecov.io/gh/lowe-lab-ucl/arboretum/tree/main)
 
 # Arboretum
 
 
-![](https://raw.githubusercontent.com/lowe-lab-ucl/arboretum/master/examples/arboretum.gif)
-*Automated cell tracking and lineage tree reconstruction*.
+
+https://github.com/lowe-lab-ucl/arboretum/assets/8217795/d98c22c4-73bb-493a-9f8f-c224d615209d
+
+
+_Automated cell tracking and lineage tree reconstruction_.
 
 ### Overview
 
-A dockable widget for [Napari](https://github.com/napari) for visualizing cell lineage trees.
+A dockable widget for [Napari](https://github.com/napari/napari) for visualizing cell lineage trees.
 
 Features:
-+ Lineage tree plot widget
-+ Integration with [btrack](https://github.com/quantumjot/BayesianTracker)
+
+- Lineage tree plot widget
+- Integration with [btrack](https://github.com/quantumjot/btrack)
 
 ---
 
 ### Usage
 
-Once installed, Arboretum will be visible in the `Plugins > Add Dock Widget > napari-arboretum` menu in napari.  To visualize a lineage tree, (double) click on one of the tracks in a napari `Tracks` layer.
-
-
+Once installed, Arboretum will be visible in the `Plugins > Add Dock Widget > napari-arboretum` menu in napari. To visualize a lineage tree, (double) click on one of the tracks in a napari `Tracks` layer.
 
 ### Examples
 
 You can use the example script to display some sample tracking data in napari and load the arboretum tree viewer:
 
 ```sh
 python ./examples/show_sample_data.py
 ```
 
-Alternatively, you can use *btrack* to generate tracks from your image data. See the example notebook here:
-https://github.com/quantumjot/BayesianTracker/blob/master/examples
+Alternatively, you can use _btrack_ to generate tracks from your image data. See the example notebook here:
+https://github.com/quantumjot/btrack/blob/main/examples
 
 ---
 
 ### History
 
 This project has changed considerably. The `Tracks` layer, originally developed for this plugin, is now an official layer type in napari. Read the napari documentation here:
- https://napari.org/api/napari.layers.Tracks.html
-
+https://napari.org/stable/api/napari.layers.Tracks.html
 
 To view the legacy version of this plugin, visit the legacy branch:
 https://github.com/quantumjot/arboretum/tree/v1-legacy
```

